# Comparing `tmp/vstutils-5.4.9.tar.gz` & `tmp/vstutils-5.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.4.9.tar", last modified: Fri May 26 06:06:53 2023, max compression
+gzip compressed data, was "vstutils-5.5.0a1.tar", last modified: Sat Jun 17 04:45:38 2023, max compression
```

## Comparing `vstutils-5.4.9.tar` & `vstutils-5.5.0a1.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.424696 vstutils-5.4.9/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.4.9/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.4.9/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.4.9/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4459 2023-05-26 06:06:53.424696 vstutils-5.4.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2393 2022-12-19 05:43:06.000000 vstutils-5.4.9/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-25 10:44:35.000000 vstutils-5.4.9/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.4.9/requirements-git.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.4.9/requirements-ldap.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-13 04:11:10.000000 vstutils-5.4.9/requirements-prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-03-18 02:33:32.000000 vstutils-5.4.9/requirements-rpc.txt
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-03-29 01:47:58.000000 vstutils-5.4.9/requirements-stubs.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-13 04:11:10.000000 vstutils-5.4.9/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-05-26 04:04:11.000000 vstutils-5.4.9/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-05-26 06:06:53.424696 vstutils-5.4.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    16893 2023-04-13 03:48:29.000000 vstutils-5.4.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.384695 vstutils-5.4.9/vstutils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-26 00:26:03.000000 vstutils-5.4.9/vstutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.392696 vstutils-5.4.9/vstutils/api/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15370 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/api/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/api/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    13063 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/api/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    28220 2023-05-26 03:10:25.000000 vstutils-5.4.9/vstutils/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    24054 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/api/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/api/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/doc_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    18802 2023-02-07 05:18:57.000000 vstutils-5.4.9/vstutils/api/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)    51728 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    11754 2023-05-13 04:11:10.000000 vstutils-5.4.9/vstutils/api/filter_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/health.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.392696 vstutils-5.4.9/vstutils/api/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/0002_two_factor.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/0003_tfa_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/0004_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/0005_db_translations.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/0006_fix_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4591 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/api/models.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/responses.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/responses.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/api/routers.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/api/routers.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.396695 vstutils-5.4.9/vstutils/api/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/api/schema/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/api/schema/info.py
--rw-rw-rw-   0 root         (0) root         (0)    26465 2023-03-17 01:28:59.000000 vstutils-5.4.9/vstutils/api/schema/inspectors.py
--rw-rw-rw-   0 root         (0) root         (0)     9648 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/api/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/schema/views.py
--rw-rw-rw-   0 root         (0) root         (0)     7340 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)    10784 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/api/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     5660 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/views.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2695 2023-05-26 04:04:11.000000 vstutils-5.4.9/vstutils/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-02-13 06:24:20.000000 vstutils-5.4.9/vstutils/asgi_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4232 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/auth.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/celery_beat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.376695 vstutils-5.4.9/vstutils/doc_themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.396695 vstutils-5.4.9/vstutils/doc_themes/vst-sphinx-theme/
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/doc_themes/vst-sphinx-theme/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.396695 vstutils-5.4.9/vstutils/doc_themes/vst-sphinx-theme/static/
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-26 06:06:53.432696 vstutils-5.4.9/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/doc_themes/vst-sphinx-theme/theme.conf
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/environment.pyi
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.396695 vstutils-5.4.9/vstutils/gui/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/gui/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/gui/pwa_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/gui/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/ldap_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.396695 vstutils-5.4.9/vstutils/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.396695 vstutils-5.4.9/vstutils/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7832 2023-03-16 06:05:23.000000 vstutils-5.4.9/vstutils/management/commands/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/commands/celery_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/commands/dockermigrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/commands/dockerrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/management/commands/newproject.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/commands/run_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/commands/runrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.4.9/vstutils/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/management/commands/web.py
--rw-rw-rw-   0 root         (0) root         (0)    10646 2023-02-13 06:24:20.000000 vstutils-5.4.9/vstutils/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.400696 vstutils-5.4.9/vstutils/models/
--rw-rw-rw-   0 root         (0) root         (0)    10704 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25308 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/models/cent_notify.py
--rw-rw-rw-   0 root         (0) root         (0)    11620 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/models/custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/models/custom_model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/models/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7971 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/models/queryset.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/settings.ini
--rw-rw-rw-   0 root         (0) root         (0)    55118 2023-05-26 04:17:32.000000 vstutils-5.4.9/vstutils/settings.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-26 00:26:03.000000 vstutils-5.4.9/vstutils/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.376695 vstutils-5.4.9/vstutils/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.408696 vstutils-5.4.9/vstutils/static/bundle/
--rw-r--r--   0 root         (0) root         (0)      155 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/157.chunk.js
--rw-r--r--   0 root         (0) root         (0)   126295 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/281.chunk.js
--rw-r--r--   0 root         (0) root         (0)      171 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/281.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1553 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/296.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/296.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   136100 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/345.chunk.js
--rw-r--r--   0 root         (0) root         (0)    15726 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/368.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1066719 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/421.js
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/421.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      321 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/463.chunk.js
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/564.chunk.js
--rw-r--r--   0 root         (0) root         (0)    38336 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/618.js
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/618.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2235 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/683.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/683.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    71086 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/686.js
--rw-r--r--   0 root         (0) root         (0)   536206 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/742.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/742.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    89997 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/755.js
--rw-r--r--   0 root         (0) root         (0)      476 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/755.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   355788 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/826.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/826.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   177828 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/844.js
--rw-r--r--   0 root         (0) root         (0)  1798980 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/959.js
--rw-r--r--   0 root         (0) root         (0)     2191 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/959.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    77026 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/app_loader.js
--rw-r--r--   0 root         (0) root         (0)   303656 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/base.js
--rw-r--r--   0 root         (0) root         (0)    16276 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
--rw-r--r--   0 root         (0) root         (0)   101648 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
--rw-r--r--   0 root         (0) root         (0)      748 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils/static/bundle/output.json
--rw-r--r--   0 root         (0) root         (0)     3597 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/spa.js
--rw-r--r--   0 root         (0) root         (0)   432625 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/vstutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.408696 vstutils-5.4.9/vstutils/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/static/img/anonymous.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.412696 vstutils-5.4.9/vstutils/static/img/logo/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/static/img/logo/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/static_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5181 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.412696 vstutils-5.4.9/vstutils/templates/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.4.9/vstutils/templates/400.html
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.4.9/vstutils/templates/403.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.4.9/vstutils/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.4.9/vstutils/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.412696 vstutils-5.4.9/vstutils/templates/auth/
--rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/auth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/auth/language_selector.html
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/auth/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/auth/tfa.html
--rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.4.9/vstutils/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.4.9/vstutils/templates/base_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.412696 vstutils-5.4.9/vstutils/templates/configs/
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/configs/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.412696 vstutils-5.4.9/vstutils/templates/drf-yasg/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/drf-yasg/swagger-ui.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.4.9/vstutils/templates/go_back_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.412696 vstutils-5.4.9/vstutils/templates/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/gui/base.html
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/gui/gui.html
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/gui/manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/gui/offline.html
--rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/gui/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.416696 vstutils-5.4.9/vstutils/templates/newproject/
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/.coveragerc.template
--rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/.gitignore.template
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/.pep8.template
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/MANIFEST.in.template
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/README.rst.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.416696 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/.babelrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/.editorconfig.template
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/.prettierrc.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.416696 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/app/index.js.template
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/package.json.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templates/newproject/project_name/
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/__main__.py.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templates/newproject/project_name/models/
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/models/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/settings.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/settings.py.template
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/web.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/wsgi.py.template
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/requirements-test.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/requirements.txt.template
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/setup.cfg.template
--rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.4.9/vstutils/templates/newproject/setup.py.template
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/test.py.template
--rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/tox.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/tox_build.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/webpack.config.js.default.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/base.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/base_agreements.html
--rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.4.9/vstutils/templates/registration/confirm_email.html
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/user_registration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/rest_framework/admin.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templates/vst_inclusion_tags/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templates/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/widgets/agreement_widget.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/templatetags/request_static.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templatetags/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templatetags/vst_gravatar.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/templatetags/vst_html_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templatetags/vstconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)    17731 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.424696 vstutils-5.4.9/vstutils/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16196 2023-03-15 02:43:46.000000 vstutils-5.4.9/vstutils/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/translations/en.py
--rw-rw-rw-   0 root         (0) root         (0)    23941 2023-03-15 02:43:46.000000 vstutils-5.4.9/vstutils/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-15 02:43:46.000000 vstutils-5.4.9/vstutils/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     2721 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    44730 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/web.ini
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.388696 vstutils-5.4.9/vstutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4459 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7664 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1914 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.306711 vstutils-5.5.0a1/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-06-17 04:45:38.306711 vstutils-5.5.0a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-01 04:30:57.000000 vstutils-5.5.0a1/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/requirements-git.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/requirements-ldap.txt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/requirements-prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-07 23:11:00.000000 vstutils-5.5.0a1/requirements-rpc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/requirements-stubs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-06-16 02:15:53.000000 vstutils-5.5.0a1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-06-17 04:45:38.306711 vstutils-5.5.0a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    16554 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.254711 vstutils-5.5.0a1/vstutils/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-16 04:50:59.000000 vstutils-5.5.0a1/vstutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.262711 vstutils-5.5.0a1/vstutils/api/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:52.000000 vstutils-5.5.0a1/vstutils/api/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    29374 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:42.000000 vstutils-5.5.0a1/vstutils/api/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    15852 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/doc_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:42.000000 vstutils-5.5.0a1/vstutils/api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    13792 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/filter_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:14:38.000000 vstutils-5.5.0a1/vstutils/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.262711 vstutils-5.5.0a1/vstutils/api/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/0002_two_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/0003_tfa_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/0004_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/0005_db_translations.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/0006_fix_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/responses.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9015 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/routers.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.262711 vstutils-5.5.0a1/vstutils/api/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/schema/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/schema/info.py
+-rw-rw-rw-   0 root         (0) root         (0)    28263 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/schema/inspectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     9995 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/schema/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:14:38.000000 vstutils-5.5.0a1/vstutils/api/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5660 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/views.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/asgi_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-17 04:39:03.000000 vstutils-5.5.0a1/vstutils/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/auth.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/celery_beat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.238711 vstutils-5.5.0a1/vstutils/doc_themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.266711 vstutils-5.5.0a1/vstutils/doc_themes/vst-sphinx-theme/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/doc_themes/vst-sphinx-theme/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.266711 vstutils-5.5.0a1/vstutils/doc_themes/vst-sphinx-theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-06-17 04:45:38.326711 vstutils-5.5.0a1/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/doc_themes/vst-sphinx-theme/theme.conf
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/environment.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.266711 vstutils-5.5.0a1/vstutils/gui/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2023-06-01 04:30:57.000000 vstutils-5.5.0a1/vstutils/gui/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/gui/pwa_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/gui/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/ldap_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.266711 vstutils-5.5.0a1/vstutils/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.266711 vstutils-5.5.0a1/vstutils/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7832 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/management/commands/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/management/commands/celery_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/management/commands/dockermigrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/management/commands/dockerrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/management/commands/newproject.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/management/commands/run_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/management/commands/runrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/management/commands/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    10689 2023-06-07 00:01:26.000000 vstutils-5.5.0a1/vstutils/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.270711 vstutils-5.5.0a1/vstutils/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:53.000000 vstutils-5.5.0a1/vstutils/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25943 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/models/cent_notify.py
+-rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:53.000000 vstutils-5.5.0a1/vstutils/models/custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:53.000000 vstutils-5.5.0a1/vstutils/models/custom_model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/models/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:14:38.000000 vstutils-5.5.0a1/vstutils/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/models/queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/settings.ini
+-rw-rw-rw-   0 root         (0) root         (0)    55685 2023-06-17 04:39:03.000000 vstutils-5.5.0a1/vstutils/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:30:57.000000 vstutils-5.5.0a1/vstutils/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.238711 vstutils-5.5.0a1/vstutils/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.290711 vstutils-5.5.0a1/vstutils/static/bundle/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/157.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   126295 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/281.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/281.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/296.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/296.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   136100 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/345.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    15726 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/368.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1066719 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/421.js
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/421.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/463.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/564.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    38336 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/618.js
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/618.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/683.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/683.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    71086 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/686.js
+-rw-r--r--   0 root         (0) root         (0)   536206 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/742.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/742.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    89997 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/755.js
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/755.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   355788 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/826.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/826.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   177828 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/844.js
+-rw-r--r--   0 root         (0) root         (0)  1798980 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/959.js
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/959.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    77026 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/app_loader.js
+-rw-r--r--   0 root         (0) root         (0)   303656 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/base.js
+-rw-r--r--   0 root         (0) root         (0)    16276 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0 root         (0) root         (0)   101648 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0 root         (0) root         (0)      748 2023-06-17 04:45:37.000000 vstutils-5.5.0a1/vstutils/static/bundle/output.json
+-rw-r--r--   0 root         (0) root         (0)     3597 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/spa.js
+-rw-r--r--   0 root         (0) root         (0)   433009 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/vstutils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.290711 vstutils-5.5.0a1/vstutils/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/static/img/anonymous.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.290711 vstutils-5.5.0a1/vstutils/static/img/logo/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/static/img/logo/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/static_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5182 2023-05-29 08:14:38.000000 vstutils-5.5.0a1/vstutils/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.290711 vstutils-5.5.0a1/vstutils/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/400.html
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/403.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.294711 vstutils-5.5.0a1/vstutils/templates/auth/
+-rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/auth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/auth/language_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/auth/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/auth/tfa.html
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 07:56:30.000000 vstutils-5.5.0a1/vstutils/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/base_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.294711 vstutils-5.5.0a1/vstutils/templates/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/configs/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.294711 vstutils-5.5.0a1/vstutils/templates/drf-yasg/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/drf-yasg/swagger-ui.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/go_back_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.294711 vstutils-5.5.0a1/vstutils/templates/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/gui/base.html
+-rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/gui/gui.html
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/gui/manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/gui/offline.html
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/gui/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.298711 vstutils-5.5.0a1/vstutils/templates/newproject/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/.coveragerc.template
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/.gitignore.template
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/.pep8.template
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/MANIFEST.in.template
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/README.rst.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.298711 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/.babelrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/.editorconfig.template
+-rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/.prettierrc.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.298711 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/app/index.js.template
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/package.json.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/__main__.py.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/models/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/models/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/settings.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/settings.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/web.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/wsgi.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/requirements-test.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/requirements.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/newproject/setup.cfg.template
+-rw-rw-rw-   0 root         (0) root         (0)    14520 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/newproject/setup.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/test.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/newproject/tox.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/tox_build.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/webpack.config.js.default.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/base_agreements.html
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/registration/confirm_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/user_registration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/rest_framework/admin.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templates/vst_inclusion_tags/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
+-rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templates/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/widgets/agreement_widget.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templatetags/request_static.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templatetags/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templatetags/vst_gravatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templatetags/vst_html_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templatetags/vstconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18153 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.306711 vstutils-5.5.0a1/vstutils/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16196 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/translations/en.py
+-rw-rw-rw-   0 root         (0) root         (0)    23941 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)    18983 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.5.0a1/vstutils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    47153 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-06-06 00:37:44.000000 vstutils-5.5.0a1/vstutils/web.ini
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.254711 vstutils-5.5.0a1/vstutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-06-17 04:45:38.000000 vstutils-5.5.0a1/vstutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7664 2023-06-17 04:45:38.000000 vstutils-5.5.0a1/vstutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-17 04:45:38.000000 vstutils-5.5.0a1/vstutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-17 04:45:38.000000 vstutils-5.5.0a1/vstutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 04:43:25.000000 vstutils-5.5.0a1/vstutils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-06-17 04:45:38.000000 vstutils-5.5.0a1/vstutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-17 04:45:38.000000 vstutils-5.5.0a1/vstutils.egg-info/top_level.txt
```

### Comparing `vstutils-5.4.9/LICENSE` & `vstutils-5.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/MANIFEST.in` & `vstutils-5.5.0a1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/NOTICE` & `vstutils-5.5.0a1/NOTICE`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/PKG-INFO` & `vstutils-5.5.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.4.9
+Version: 5.5.0a1
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
 Project-URL: Releases, https://pypi.org/project/vstutils/#history
 Project-URL: Documentation, https://vstutils.vstconsulting.net/
 Keywords: web,app,spa,vue,pwa,framework,openapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -40,15 +40,14 @@
 Provides-Extra: ldap
 Provides-Extra: doc
 Provides-Extra: prod
 Provides-Extra: stubs
 Provides-Extra: pil
 Provides-Extra: boto3
 Provides-Extra: sqs
-Provides-Extra: librabbitmq
 Provides-Extra: all
 License-File: LICENSE
 License-File: NOTICE
 
 VSTUtils Framework
 ==================
```

### Comparing `vstutils-5.4.9/README.rst` & `vstutils-5.5.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/setup.cfg` & `vstutils-5.5.0a1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 author_email = sergey.k@vstconsulting.net
 url = https://github.com/vstconsulting/vstutils
 keywords = web, app, spa, vue, pwa, framework, openapi
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Operating System :: POSIX
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

### Comparing `vstutils-5.4.9/setup.py` & `vstutils-5.5.0a1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -419,15 +419,15 @@
     packages=find_packages(exclude=['tests', 'test_proj']+ext_list),
     ext_modules_list=ext_list,
     static_exclude_min=[
         'vstutils/templates/.*\.js$',
         'vstutils/static/bundle/.*\.js$'
     ],
     install_requires=[
-        "django~=" + (os.environ.get('DJANGO_DEP', "") or "4.1.7"),
+        "django~=" + (os.environ.get('DJANGO_DEP', "") or "4.2.2"),
     ]
     + requirements
     + load_requirements('requirements-doc.txt'),
     extras_require={
         'test': load_requirements('requirements-test.txt'),
         'rpc': requirements_rpc,
         'ldap': load_requirements('requirements-ldap.txt'),
@@ -436,26 +436,15 @@
         'stubs': load_requirements('requirements-stubs.txt'),
         'pil': ['Pillow~=9.4.0'],
         'boto3': [
             i.replace('libcloud', 'libcloud,boto3')
             for i in requirements
             if isinstance(i, str) and 'django-storages' in i
         ],
-        'sqs': [
-            i.replace('redis', 'sqs,redis')
-            if isinstance(i, str) and 'celery' in i
-            else i
-            for i in requirements_rpc
-        ],
-        'librabbitmq': [
-            i.replace('redis', 'librabbitmq,redis')
-            if isinstance(i, str) and 'celery' in i
-            else i
-            for i in requirements_rpc
-        ],
+        'sqs': requirements_rpc + ['pycurl~=7.45.2'],
     },
     dependency_links=[
     ] + load_requirements('requirements-git.txt'),
     entry_points={
         'console_scripts': ['vstutilsctl=vstutils.__main__:cmd_execution']
     },
     project_urls={
@@ -464,13 +453,13 @@
         "Releases": "https://pypi.org/project/vstutils/#history",
         "Documentation": "https://vstutils.vstconsulting.net/",
     }
 )
 
 all_deps = []
 for key, deps in kwargs['extras_require'].items():
-    if key not in ('sqs', 'librabbitmq', 'stubs'):
+    if key not in ('stubs', 'sqs'):
         all_deps += deps
 
 kwargs['extras_require']['all'] = all_deps
 
 make_setup(**kwargs)
```

### Comparing `vstutils-5.4.9/vstutils/api/actions.py` & `vstutils-5.5.0a1/vstutils/api/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         'result_serializer_class',
         'query_serializer',
         'action_kwargs',
         'multi',
         'title',
         'icons',
         'is_list',
+        'hidden',
     )
     method_response_mapping = {
         "HEAD": HTTP_200_OK,
         "GET": HTTP_200_OK,
         "PUT": HTTP_200_OK,
         "PATCH": HTTP_200_OK,
         "POST": HTTP_201_CREATED,
@@ -96,26 +97,28 @@
         serializer_class: _t.Type[serializers.Serializer] = DataSerializer,
         result_serializer_class: _t.Type[serializers.Serializer] = None,
         query_serializer: _t.Type[serializers.Serializer] = None,
         multi: bool = False,
         title: _t.Text = None,
         icons: _t.Union[_t.Text, _t.Iterable] = None,
         is_list: bool = False,
+        hidden: bool = False,
         **kwargs,
     ):
         # pylint: disable=too-many-arguments
         self.detail = detail
         self.methods = list(map(str.upper, methods or ['POST'])) or None
         self.serializer_class = serializer_class
         self.result_serializer_class = result_serializer_class
         self.query_serializer = query_serializer
         self.multi = multi
         self.title = title
         self.icons = icons
         self.is_list = is_list
+        self.hidden = hidden
         self.action_kwargs = kwargs
         if self.query_serializer:
             self.action_kwargs['query_serializer'] = self.query_serializer
 
     @property
     def is_page(self):
         return 'GET' in self.methods
@@ -130,14 +133,15 @@
 
         name = func.__name__.replace('_', ' ').capitalize()
         swagger_kwargs = {
             'operation_description': (func.__doc__ or name).strip(),
             'methods': self.methods,
             'x-multiaction': self.multi if not self.is_page else False,
             'x-title': self.title or (None if self.is_page else name),
+            'x-hidden': self.hidden,
         }
         if self.query_serializer:
             swagger_kwargs['query_serializer'] = self.query_serializer
         if self.icons:
             swagger_kwargs['x-icons'] = self.icons.split(' ') if isinstance(self.icons, _t.Text) else list(self.icons)
         if self.is_page:
             swagger_kwargs['x-list'] = self.is_list
```

### Comparing `vstutils-5.4.9/vstutils/api/admin.py` & `vstutils-5.5.0a1/vstutils/api/admin.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/auth.py` & `vstutils-5.5.0a1/vstutils/api/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from django.db import transaction
 from django.conf import settings
 from django.utils.functional import SimpleLazyObject, cached_property
 from django_filters import BooleanFilter, CharFilter
 from rest_framework import serializers, exceptions, request as drf_request
 from vstutils.api import fields, base, permissions, responses, decorators as deco
 from vstutils.api.filters import DefaultIDFilter, name_filter, name_help
-from vstutils.api.serializers import VSTSerializer, DataSerializer, BaseSerializer, update_declared_fields
+from vstutils.api.serializers import VSTSerializer, BaseSerializer, update_declared_fields
 from vstutils.api.models import TwoFactor, RecoveryCode, UserSettings
 from vstutils.utils import raise_context_decorator_with_default, translate, lazy_translate as __
 
 User: _t.Type[AbstractUser] = get_user_model()  # type: ignore[override]
 
 
 class ChangePasswordPermission(permissions.IsAuthenticatedOpenApiRequest):  # type: ignore
@@ -118,15 +118,15 @@
         if validated_data['password'] != validated_data.pop('password2', None):
             raise exceptions.ValidationError({
                 "password": [translate('Passwords do not match.')],
             })
         return validated_data
 
 
-class ChangePasswordSerializer(DataSerializer):
+class ChangePasswordSerializer(BaseSerializer):
     old_password = fields.PasswordField(required=True)
     password = fields.PasswordField(required=True, label='New password')
     password2 = fields.PasswordField(required=True, label='Confirm new password')
 
     def update(self, instance, validated_data):
         if not instance.check_password(validated_data['old_password']):
             raise exceptions.AuthenticationFailed()
@@ -241,15 +241,15 @@
 
     model: _t.Type[AbstractUser] = User
     serializer_class: _t.Type[UserSerializer] = update_declared_fields(UserSerializer)  # type: ignore
     serializer_class_one: _t.Type[OneUserSerializer] = update_declared_fields(OneUserSerializer)  # type: ignore
     serializer_class_create: _t.Type[CreateUserSerializer] = update_declared_fields(  # type: ignore
         CreateUserSerializer
     )
-    serializer_class_change_password: _t.Type[DataSerializer] = ChangePasswordSerializer
+    serializer_class_change_password: _t.Type[BaseSerializer] = ChangePasswordSerializer
     serializer_class_twofa: _t.Type[serializers.BaseSerializer] = update_declared_fields(  # type: ignore
         TwoFASerializer
     )
     serializer_class__settings: _t.Type[serializers.BaseSerializer] = UserSettingsSerializer
     filterset_class = UserFilter
     permission_classes = (permissions.SuperUserPermission,)
     optimize_get_by_values = False
```

### Comparing `vstutils-5.4.9/vstutils/api/base.py` & `vstutils-5.5.0a1/vstutils/api/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Default ViewSets for web-api.
 """
-
+import hashlib
 import re
 import io
 import json
 import logging
 import inspect
 import traceback
 import datetime
@@ -17,15 +17,14 @@
 from django.conf import settings
 from django.core import exceptions as djexcs
 from django.http.response import Http404, FileResponse, HttpResponseNotModified
 from django.db.models.query import QuerySet
 from django.db import transaction, models
 from django.utils.functional import cached_property, lazy
 from django.utils.http import urlencode
-from django.contrib.contenttypes.fields import GenericForeignKey
 from rest_framework.reverse import reverse
 from rest_framework import viewsets as vsets, views as rvs, mixins as drf_mixins, exceptions, status
 from rest_framework.serializers import BaseSerializer
 from rest_framework.response import Response as RestResponse
 from rest_framework.request import Request
 from rest_framework.decorators import action
 from rest_framework.schemas import AutoSchema as DRFAutoSchema
@@ -294,25 +293,25 @@
 
     def create_action_serializer(self, *args, **kwargs):
         """
         A method that implements the standard logic for actions.
         It relies on the passed arguments to build logic.
         So, if the named argument data was passed, then the serializer will be validated and saved.
 
-        :param autosave: Enables / disables the execution of saving by the serializer if named argument `data` passed.
+        :param autosave: Enables/disables the execution of saving by the serializer if named argument `data` passed.
                          Enabled by default.
         :type autosave: bool
         :param: data: Default serializer class argument with serializable data. Enables validation and saving.
         :type data: dict
         :param: instance: Default serializer class argument with serializable instance.
         :type instance: typing.Any
         :param custom_data: Dict with data which will passed to `validated_data` without validation.
         :type custom_data: dict
         :param serializer_class: Serializer class for this execution.
-                                 May be usefull when request and response serializers is different.
+                                 May be useful when request and response serializers are different.
         :type serializer_class: None,type[rest_framework.serializers.Serializer]
         :return: Ready serializer with default logic performed.
         :rtype: rest_framework.serializers.Serializer
         """
         self.serializer_class = kwargs.pop('serializer_class', None) or self.get_serializer_class()
         save_kwargs = kwargs.pop('custom_data', {})
         should_save = kwargs.pop('autosave', True) or save_kwargs
@@ -341,15 +340,15 @@
             if issubclass(serializer_class, BaseSerializer):
                 read_fields = get_serializer_readable_fields(serializer_class())
                 _fields = queryset.model._meta.get_fields()
                 model_fields = {f.name for f in _fields}
                 fk_related_fields = {
                     f.name
                     for f in _fields
-                    if isinstance(f, (models.ForeignKey, models.ManyToManyField, GenericForeignKey))
+                    if isinstance(f, models.ForeignKey)
                 }
                 deferable_fields = (
                         model_fields -
                         read_fields -
                         fk_related_fields -
                         set(getattr(queryset.model, '_required_fields', None) or set())
                 )
@@ -402,14 +401,19 @@
             request: Request,
             query_serializer: _t.Type[BaseSerializer] = None,
             raise_exception: bool = True,
     ) -> _t.Dict:
         """
         Get request query data and serialize values if `query_serializer_class` attribute exists
         or attribute was send.
+
+        :param request: DRF request object.
+        :param query_serializer: serializer class for processing parameters in query_params.
+        :param raise_exception: flag that indicates whether an exception should be thrown during validation in
+                                the serializer or not.
         """
         serializer_class: _t.Optional[_t.Type[BaseSerializer]] = (
                 query_serializer or getattr(self, 'query_serializer', None)
         )
         assert serializer_class is not None, "You must setup 'query_serializer_class' in arguments or view attribute."
 
         serializer: BaseSerializer = serializer_class(data=request.query_params, context=self.get_serializer_context())
@@ -474,49 +478,73 @@
     """
 
     class NotModifiedException(exceptions.APIException):
         status_code = 304
         default_detail = ''
         default_code = 'cached'
 
+    class PreconditionFailedException(exceptions.APIException):
+        status_code = 412
+        default_detail = ''
+
     @cached_property
     def model_class(self):
         return getattr(self, 'model', None) or self.queryset.model
 
     @cached_property
     @raise_context_decorator_with_default(default=False)
     def is_main_action(self):
         if hasattr(self, 'should_cache') and not self.should_cache():
             return False
         return self.action in main_actions or getattr(getattr(self, self.action, None), '_nested_view', None) is None
 
     def get_etag_value(self, model_class, request):
+        pk = self.kwargs.get(self.lookup_url_kwarg or self.lookup_field)
+        if isinstance(model_class, (list, tuple, set)):
+            etag_value = hashlib.md5(
+                "_".join(mc.get_etag_value(pk) for mc in model_class).encode('utf-8')
+            ).hexdigest()
+        else:
+            etag_value = model_class.get_etag_value(pk)
         return (
-            f'{model_class.get_etag_value()}'
+            f'{etag_value}'
             f'_'
             f'{request.COOKIES.get(settings.LANGUAGE_COOKIE_NAME, settings.LANGUAGE_CODE)}'
         )
 
     def _get_etag(self, model_class, request):
         return f'"{self.get_etag_value(model_class, request)}"'
 
     def check_etag(self, request, model_class=None):
-        if request.method == "GET":
-            header = request.headers.get("If-None-Match", None)
-            if not header:
-                return
-            data = self._get_etag(model_class or self.model_class, request)
-            header = str(header)
-            if header[:2] in ('W/', "w/"):
-                header = header[2:]
-            if header[0] != '"':
-                header = f'"{header}"'
-            if data == header:
-                raise self.NotModifiedException("")
-        # TODO: Workflow with ETag on PUT/PATCH/DELETE
+        should_check, header_name, exception, operation_handler = False, "", Exception(), str.__eq__
+        if request.method in {"GET", "HEAD"}:
+            should_check = True
+            exception = self.NotModifiedException("")
+            header_name = "If-None-Match"
+        elif request.method in getattr(self, 'etag_match_methods', {request.method}):
+            should_check = True
+            exception = self.PreconditionFailedException("")
+            header_name = "If-Match"
+            operation_handler = str.__ne__
+
+        if not should_check:
+            # For non-standart request methods
+            return  # nocv
+
+        header = request.headers.get(header_name, None)
+        if not header:
+            return
+        data = self._get_etag(model_class or self.model_class, request)
+        header = str(header)
+        if header[:2] in ('W/', "w/"):
+            header = header[2:]
+        if header[0] != '"':
+            header = f'"{header}"'
+        if operation_handler(data, header):
+            raise exception
 
     def finalize_response(self, request: Request, response: RestResponse, *args, **kwargs) -> RestResponse:
         result_response = super().finalize_response(request, response, *args, **kwargs)
         if self.is_main_action and 'ETag' not in result_response.headers:
             result_response.headers['ETag'] = lazy(self._get_etag, str)(self.model_class, request)
         return result_response
 
@@ -563,15 +591,15 @@
         serializer.is_valid(raise_exception=True)
         serializer.save()
         return responses.HTTP_201_CREATED(serializer.data)
 
 
 class FileResponseRetrieveMixin(GenericViewSet):
     """
-    ViewSet mixin for retriving FileResponse from models with file fields data.
+    ViewSet mixin for retrieving FileResponse from models with file fields data.
 
     Example:
 
         .. literalinclude:: ../test_src/test_proj/models/files.py
            :lines: 1-22,59-77
     """
```

### Comparing `vstutils-5.4.9/vstutils/api/decorators.py` & `vstutils-5.5.0a1/vstutils/api/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,30 +326,30 @@
     By default, DRF does not support nested views.
     This decorator solves this problem.
 
     You need two or more models with nested relationship (Many-to-Many or Many-to-One)
     and two viewsets. Decorator nests viewset to parent viewset class and
     generate paths in API.
 
-    :param name: -- Name of nested path. Also used as default name for related queryset (see `manager_name`).
+    :param name: Name of nested path. Also used as default name for related queryset (see `manager_name`).
     :type name: str
-    :param arg: -- Name of nested primary key field.
+    :param arg: Name of nested primary key field.
     :type arg: str
-    :param view: -- Nested viewset class.
+    :param view: Nested viewset class.
     :type view:
         vstutils.api.base.ModelViewSet,
         vstutils.api.base.HistoryModelViewSet,
         vstutils.api.base.ReadOnlyModelViewSet
-    :param allow_append: -- Flag for allowing to append existed instances.
+    :param allow_append: Flag for allowing to append existed instances.
     :type allow_append: bool
-    :param manager_name: -- Name of model-object attr which contains nested queryset.
+    :param manager_name: Name of model-object attr which contains nested queryset.
     :type manager_name: str,typing.Callable
-    :param methods: -- List of allowed methods to nested view endpoints.
+    :param methods: List of allowed methods to nested view endpoints.
     :type methods: list
-    :param subs: -- List of allowed subviews or actions to nested view endpoints.
+    :param subs: List of allowed subviews or actions to nested view endpoints.
     :type subs: list,None
     :param queryset_filters: List of callable objects which returns filtered queryset of main.
 
 
     .. note::
         Some view methods will not call for performance reasons.
         This also applies to some of the class attributes that are usually initialized in the methods.
@@ -374,18 +374,18 @@
             class TaskViewSet(ModelViewSet):
                 model = sers.models.Task
                 serializer_class = sers.TaskSerializer
 
 
         This code generates api paths:
 
-         * `/tasks/` - GET,POST
-         * `/tasks/{id}/` - GET,PUT,PATCH,DELETE
-         * `/tasks/{id}/stages/` - GET,POST
-         * `/tasks/{id}/stages/{stages_id}/` - GET,PUT,PATCH,DELETE
+         * `/tasks/` - GET, POST
+         * `/tasks/{id}/` - GET, PUT, PATCH, DELETE
+         * `/tasks/{id}/stages/` - GET, POST
+         * `/tasks/{id}/stages/{stages_id}/` - GET, PUT, PATCH, DELETE
 
     """
     __slots__ = (
         'view',
         'allowed_subs',
         '_subs',
         'methods',
```

### Comparing `vstutils-5.4.9/vstutils/api/decorators.pyi` & `vstutils-5.5.0a1/vstutils/api/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/doc_generator.py` & `vstutils-5.5.0a1/vstutils/api/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/endpoint.py` & `vstutils-5.5.0a1/vstutils/api/endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -301,23 +301,29 @@
         if 'query' in validated_data and validated_data['query']:
             url += '?' + str(validated_data['query'])
         if method_name != 'get':
             method = transaction.atomic()(method)
         data = validated_data['data']
         if data and method_name != 'get':
             data = self.renderer.render(data, media_type=self.renderer.media_type)
+
+        headers: dict = validated_data['headers']  # type: ignore
+        # Fixing oldstyle headers
+        for old_style_header in tuple(filter(lambda x: x.startswith('HTTP_'), headers.keys())):
+            headers[old_style_header[5:].replace('_', '-').lower()] = headers.pop(old_style_header)  # nocv
+
         result = ParseResponseDict(
             path=url,
             method=method_name,
             response=method(  # type: ignore
                 url,
                 content_type=self.renderer.media_type,
                 secure=self.context['request']._request.is_secure(),
                 data=data,
-                **validated_data['headers']
+                headers=headers,
             )
         )
         if 'let' in validated_data:
             self.context['variables'][validated_data['let']] = result
         return result
```

### Comparing `vstutils-5.4.9/vstutils/api/fields.py` & `vstutils-5.5.0a1/vstutils/api/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     def __init__(self, **kwargs):
         kwargs['style'] = {'input_type': 'password'}
         super().__init__(**kwargs)
 
 
 class BinFileInStringField(FileInStringField):
     """
-    Field extends :class:`.FileInStringField`, but work with binary(base64) files.
+    Field extends :class:`.FileInStringField`, but works with binary (base64) files.
 
     :param media_types: List of MIME types to select on the user's side.
                         Supported syntax using ``*``. Default: `['*/*']`
     :type media_types: tuple,list
 
     .. note::
         Effective only in GUI. Works similar to :class:`.VSTCharField` in API.
@@ -99,15 +99,15 @@
 class CSVFileField(FileInStringField):
     """
     Field extends :class:`.FileInStringField`, using for works with csv files.
     This field provides the display of the loaded data in the form of a table.
 
     :param items: The config of the table. This is a drf or vst serializer which includes char fields
                   which are the keys in the dictionaries into which the data from csv is serialized
-                  and the  names for columns in a table.
+                  and the names for columns in a table.
                   The fields must be in the order you want them to appear in the table.
                   Following options may be included:
 
                   - ``label``: human readable column name
                   - ``required``: Defines whether the field should be required. False by default.
 
     :type items: Serializer
@@ -159,24 +159,24 @@
 
 
 class AutoCompletionField(VSTCharField):
     """
     Field that provides autocompletion on frontend, using specified list of objects.
 
     :param autocomplete: Autocompletion reference. You can set list/tuple with
-                         values or set OpenApi schema definition name.
+                         values or set OpenAPI schema definition name.
                          For definition name GUI will find optimal link and
                          will show values based on ``autocomplete_property`` and
                          ``autocomplete_represent`` arguments.
     :type autocomplete: list,tuple,str
     :param autocomplete_property: this argument indicates which attribute will be
-                                  get from OpenApi schema definition model as value.
+                                  get from OpenAPI schema definition model as value.
     :type autocomplete_property: str
     :param autocomplete_represent: this argument indicates which attribute will be
-                                   get from OpenApi schema definition model as represent value.
+                                   get from OpenAPI schema definition model as represent value.
     :param use_prefetch: prefetch values on frontend at list-view. Default is ``True``.
     :type use_prefetch: bool
 
     .. note::
         Effective only in GUI. Works similar to :class:`.VSTCharField` in API.
     """
 
@@ -193,31 +193,31 @@
             self.autocomplete_represent = kwargs.pop('autocomplete_represent', 'name')
             self.use_prefetch = kwargs.pop('use_prefetch', True)
         super().__init__(**kwargs)
 
 
 class CommaMultiSelect(VSTCharField):
     """
-    Field containing a list of values with specified separator(default: ",").
+    Field containing a list of values with specified separator (default: ",").
     Gets list of values from another model or custom list. Provides autocompletion as :class:`.AutoCompletionField`,
     but with comma-lists.
     Suited for property-fields in model where main logic is already implemented or
-    with :class:`CharField`.
+    with :class:`model.CharField`.
 
-    :param select: OpenApi schema definition name or list with values.
+    :param select: OpenAPI schema definition name or list with values.
     :type select: str,tuple,list
     :param select_separator: separator of values. Default is comma.
     :type select_separator: str
     :param select_property,select_represent: work as ``autocomplete_property`` and ``autocomplete_represent``.
                                              Default is ``name``.
     :param use_prefetch: prefetch values on frontend at list-view. Default is ``False``.
     :param make_link: Show value as link to model. Default is ``True``.
-    :param dependence: Dictionary, where keys are name of field from the same model, and values are name of query filter
-                       .If at least one of the fields that we depend on is non nullable, required and set to null,
-                       autocompletion list will be empty and field will be disabled.
+    :param dependence: Dictionary, where keys are name of field from the same model, and values are name of query
+                       filter. If at least one of the fields that we depend on is non nullable, required and set to
+                       null, autocompletion list will be empty and field will be disabled.
     :type dependence: dict
 
 
     .. note::
         Effective only in GUI. Works similar to :class:`.VSTCharField` in API.
     """
 
@@ -254,21 +254,21 @@
     """
     Field which type is based on another field. It converts value to internal string
     and represent field as json object.
 
     :param field: field in model which value change will change type of current value.
     :type field: str
     :param types: key-value mapping where key is value of subscribed field and
-                  value is type (in OpenApi format) of current field.
+                  value is type (in OpenAPI format) of current field.
     :type type: dict
     :param choices: variants of choices for different subscribed field values.
                     Uses mapping where key is value of subscribed field and
                     value is list with values to choice.
     :type choices: dict
-    :param source_view: Allows to to use parent views data as source for field creation.
+    :param source_view: Allows to use parent views data as source for field creation.
                         Exact view path (`/user/{id}/`) or relative parent specifier
                         (`<<parent>>.<<parent>>.<<parent>>`) can be provided. For example if current page is
                         `/user/1/role/2/` and `source_view` is `<<parent>>.<<parent>>` then data
                         from `/user/1/` will be used. Only detail views if supported.
     :type source_view: str
 
 
@@ -335,15 +335,15 @@
     """
     Field extends :class:`DynamicJsonTypeField` but its value is not transformed to json and would be given as is.
     Useful for :class:`property` in models or for actions.
 
     :param field: field in model which value change will change type of current value.
     :type field: str
     :param types: key-value mapping where key is value of subscribed field and
-                  value is type (in OpenApi format) of current field.
+                  value is type (in OpenAPI format) of current field.
     :type type: dict
     :param choices: variants of choices for different subscribed field values.
                     Uses mapping where key is value of subscribed field and
                     value is list with values to choice.
     :type choices: dict
 
 
@@ -363,15 +363,15 @@
 
     - **key** - string representation of value type which is received from related instance :attr:`.field_attribute`.
     - **value** - :class:`rest_framework.Field` instance for validation.
 
     :param field: field in model which value change changes type of current value.
                   Field must be :class:`.FkModelField`.
     :type field: str
-    :param field_attribute: attribute of model related model instance with name of type.
+    :param field_attribute: attribute of related model instance with name of type.
     :type field_attribute: str
 
     .. warning::
         ``field_attribute`` in related model must be :class:`rest_framework.ChoicesField` or
         GUI will show field as simple text.
 
     """
@@ -442,60 +442,60 @@
     .. note::
         Effective only in GUI. Works similar to :class:`.VSTCharField` in API.
     """
 
 
 class FkField(IntegerField):
     """
-    Implementation of ForeignKeyField.You can specify which field of a related model will be
-    stored in field(default: "id"), and which will represent field on frontend.
+    Implementation of ForeignKeyField. You can specify which field of a related model will be
+    stored in field (default: "id"), and which will represent field on frontend.
 
-    :param select: OpenApi schema definition name.
+    :param select: OpenAPI schema definition name.
     :type select: str
     :param autocomplete_property: this argument indicates which attribute will be
-                                  get from OpenApi schema definition model as value.
+                                  get from OpenAPI schema definition model as value.
                                   Default is ``id``.
     :type autocomplete_property: str
     :param autocomplete_represent: this argument indicates which attribute will be
-                                   get from OpenApi schema definition model as represent value.
+                                   get from OpenAPI schema definition model as represent value.
                                    Default is ``name``.
     :param field_type: defines the autocomplete_property type for further definition in the schema
                        and casting to the type from the api. Default is passthroughs but require `int` or `str` objects.
     :type field_type: type
     :param use_prefetch: prefetch values on frontend at list-view. Default is ``True``.
     :type use_prefetch: bool
     :param make_link: show value as link to model. Default is ``True``.
     :type make_link: bool
     :param dependence: dictionary, where keys are names of a field from the same model,
-                       and keys are name of query filter.
+                       and values are names of query filter.
                        If at least one of the fields that we depend on is non nullable, required and set to null,
                        autocompletion list will be empty and field will be disabled.
 
                        There are some special keys for dependence dictionary to get data that is stored
                        on frontend without additional database query:
 
-                       ``'<<pk>>'``, - get primary key of current instance
+                       ``'<<pk>>'`` gets primary key of current instance,
 
-                       ``'<<view_name>>'`` get view name from Vue component,
+                       ``'<<view_name>>'`` gets view name from Vue component,
 
-                       ``'<<parent_view_name>>'`` get view name from Vue component,
+                       ``'<<parent_view_name>>'`` gets parent view name from Vue component,
 
-                       ``'<<view_level>>'`` get view level,
+                       ``'<<view_level>>'`` gets view level,
 
-                       ``'<<operation_id>>'`` get operation_id,
+                       ``'<<operation_id>>'`` gets operation_id,
 
-                       ``'<<parent_operation_id'>>`` get parent_operation_id
+                       ``'<<parent_operation_id'>>`` gets parent_operation_id.
     :type dependence: dict
 
     Examples:
         .. sourcecode:: python
 
             field = FkField(select=Category, dependence={'<<pk>>': 'my_filter'})
 
-    This filter  will get pk of current object and make query on frontend '/category?my_filter=3'
+    This filter will get pk of current object and make query on frontend '/category?my_filter=3'
     where '3' is primary key of current instance.
 
 
     :param filters: dictionary, where keys are names of a field from a related (by this FkField) model,
                     and values are values of that field.
     :type filters: dict
 
@@ -539,22 +539,22 @@
 
 class FkModelField(FkField):
     """
     Extends :class:`.FkField`, but stores referred model class.
     This field is useful for :class:`django.db.models.ForeignKey` fields in model to set.
 
     :param select: model class (based on :class:`vstutils.models.BModel`) or serializer class
-                   which used in API and has path in OpenApi schema.
+                   which used in API and has path in OpenAPI schema.
     :type select: vstutils.models.BModel,vstutils.api.serializers.VSTSerializer
     :param autocomplete_property: this argument indicates which attribute will be
-                                  get from OpenApi schema definition model as value.
+                                  get from OpenAPI schema definition model as value.
                                   Default is ``id``.
     :type autocomplete_property: str
     :param autocomplete_represent: this argument indicates which attribute will be
-                                   get from OpenApi schema definition model as represent value.
+                                   get from OpenAPI schema definition model as represent value.
                                    Default is ``name``.
     :param use_prefetch: prefetch values on frontend at list-view. Default is ``True``.
     :param make_link: Show value as link to model. Default is ``True``.
 
 
     .. warning::
         Model class get object from database during `.to_internal_value` execution. Be careful on mass save executions.
@@ -642,30 +642,30 @@
         super().__init__(**kwargs)
         self.only_last_child = only_last_child
         self.parent_field_name = parent_field_name
 
 
 class UptimeField(IntegerField):
     """
-    Field for some uptime(time duration), in seconds, for example.
+    Time duration field, in seconds. May be used to compute some uptime.
 
     .. note::
         Effective only in GUI. Works similar to :class:`rest_framework.IntegerField` in API.
 
     """
 
 
 class RedirectFieldMixin:
     """
     Field mixin indicates that this field is used to send redirect address to frontend after some action.
 
     :param operation_name: prefix for operation_id, for example if operation_id is `history_get`
            then operation_name is `history`
     :type operation_name: str
-    :param depend_field: name of the field that we depend on, its' value will be used for operation_id
+    :param depend_field: name of the field that we depend on, its value will be used for operation_id
     :type depend_field: str
     :param concat_field_name: if True then name of the field will be added at the end of operation_id
     :type concat_field_name: bool
     """
     redirect: bool = True
 
     def __init__(self, **kwargs):
@@ -695,15 +695,15 @@
     """
 
 
 class NamedBinaryFileInJsonField(VSTCharField):
     """
     Field that takes JSON with properties:
     * name - string - name of file;
-    * mediaType - string - MIME type of file
+    * mediaType - string - MIME type of file;
     * content - base64 string - content of file.
 
     This field is useful for saving binary files with their names in :class:`django.db.models.CharField`
     or :class:`django.db.models.TextField` model fields. All manipulations with decoding and encoding
     binary content data executes on client. This imposes reasonable limits on file size.
 
     Additionally, this field can construct :class:`django.core.files.uploadedfile.SimpleUploadedFile`
@@ -824,15 +824,15 @@
             return self._handle_file(data)
         return super().to_internal_value(data)
 
 
 class NamedBinaryImageInJsonField(NamedBinaryFileInJsonField):
     """
     Extends :class:`.NamedBinaryFileInJsonField` to represent image on frontend
-    (if binary image is valid).Validate this field with
+    (if binary image is valid). Validate this field with
     :class:`vstutils.api.validators.ImageValidator`.
 
     :param background_fill_color: Color to fill area that is not covered by image after cropping.
         Transparent by default but will be black if image format is not supporting transparency.
         Can be any valid CSS color.
     :type background_fill_color: str
     """
@@ -944,15 +944,15 @@
     as a list of related instances.
 
     To use it, you specify 'related_name' kwarg (related_manager for reverse ForeignKey)
     and 'fields' kwarg (list or tuple of fields from related model, which needs to be included).
 
     By default :class:`.VSTCharField` used to serialize all field values and represent it on
     frontend. You can specify `serializer_class` and override fields as you need. For example title, description
-    and other field properties can be set to customize frontend behaviour.
+    and other field properties can be set to customize frontend behavior.
 
     :param related_name: name of a related manager for reverse foreign key
     :type related_name: str
     :param fields: list of related model fields.
     :type fields: list[str], tuple[str]
     :param view_type: determines how field are represented on frontend. Must be either 'list' or 'table'.
     :type view_type: str
@@ -1095,20 +1095,20 @@
         # get related mapping with id and name of instances
         return lazy(lambda: self._prep_data(value), tuple)()
 
 
 class RatingField(FloatField):
     """
     Extends class 'rest_framework.serializers.FloatField'. This field represents a rating form input on frontend.
-    Grading limits can be specified with 'min_value=' and 'max_value=', defaults are 0 to 5.Minimal step between
-    grades are specified in 'step=', default - 1.Frontend visual representation can be chosen
+    Grading limits can be specified with 'min_value=' and 'max_value=', defaults are 0 to 5. Minimal step between
+    grades are specified in 'step=', default - 1. Frontend visual representation can be chosen
     with 'front_style=', available variants are listed in 'self.valid_front_styles'.
 
-    for 'slider' front style, you can specify slider color, by passing valid color to 'color='.
-    for 'fa_icon' front style, you can specify FontAwesome icon that would be used for displaying rating, by passing a
+    For 'slider' front style, you can specify slider color, by passing valid color to 'color='.
+    For 'fa_icon' front style, you can specify FontAwesome icon that would be used for displaying rating, by passing a
     valid FontAwesome icon code to 'fa_class='.
 
     :param min_value: minimal level
     :type min_value: float, int
     :param max_value: maximal level
     :type max_value: float, int
     :param step: minimal step between levels
@@ -1151,29 +1151,29 @@
             translate('This field must contain only digits but input: ') + f'{value}.'
         )
 
 
 class PhoneField(CharField):
     """
     Extends class 'rest_framework.serializers.CharField'.
-    Field for for phone in international format
+    Field for phone in international format
     """
 
     def __init__(self, **kwargs):
         kwargs['min_length'] = 8
         kwargs['max_length'] = 16
         super().__init__(**kwargs)
 
         self.validators.append(is_all_digits_validator)
 
 
 class MaskedField(CharField):
     """
     Extends class 'rest_framework.serializers.CharField'.
-    Field that applies mask to value
+    Field that applies mask to value.
 
     :param mask: `IMask <https://imask.js.org/guide.html>`_
     :type mask: dict, str
 
     .. note::
         Effective only on frontend.
     """
```

### Comparing `vstutils-5.4.9/vstutils/api/filter_backends.py` & `vstutils-5.5.0a1/vstutils/models/custom_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,297 +1,403 @@
-import typing as _t
+# cython: binding=True
+# pylint: disable=unused-import
+from copy import deepcopy
+from functools import partial
+
+from yaml import load
+try:
+    from yaml import CSafeLoader as Loader
+except ImportError:  # nocv
+    from yaml import SafeLoader as Loader
+from django.db.models.query import ModelIterable
+from django.db.models.fields import CharField, TextField, IntegerField, BooleanField, AutoField    # noqa: F401
+
+from . import BQuerySet, BaseModel
+from .base import ModelBaseClass
+from ..utils import raise_context
+from ..tools import get_file_value, multikeysort  # pylint: disable=import-error
+
+
+class Query(dict):
+    distinct_fields = False
+
+    def __init__(self, queryset, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.queryset = queryset
+        self.combinator = None
+        self.is_sliced = False
+        self.select_for_update = False
+        self.select_related = False
+        self['standard_ordering'] = True
+
+    @property
+    def model(self):
+        return self.queryset.model
+
+    @property
+    def standard_ordering(self):
+        return self['standard_ordering']
+
+    @standard_ordering.setter
+    def standard_ordering(self, value):
+        self['standard_ordering'] = bool(value)
+
+    def chain(self):
+        return self.clone()
+
+    def clone(self):
+        query = deepcopy(self)
+        if 'custom_queryset_kwargs' in self:
+            query['custom_queryset_kwargs'] = self['custom_queryset_kwargs']
+        return query
+
+    def _check_data(self, check_type, data):
+        # pylint: disable=protected-access,too-many-return-statements
+        if getattr(self, 'empty', False):
+            return False
+        check_data = self.get(check_type, {})
+        if check_type == 'exclude' and not check_data:
+            return False
+        meta = self.model._meta
+        for filter_name, filter_data in check_data.items():
+            filter_name = filter_name.replace('__exact', '')
+            filter_name__cleared, search_format = (filter_name.split('__', maxsplit=1) + [None])[:2]
+            if filter_name__cleared == 'pk':
+                filter_name__cleared = meta.pk.attname
+            try:
+                value = data[filter_name__cleared]
+            except KeyError:
+                continue
+            field = meta._forward_fields_map[filter_name__cleared]
+            if isinstance(filter_data, (list, tuple, set)):
+                filter_data = map(field.to_python, filter_data)
+            else:
+                filter_data = field.to_python(filter_data)
+            if search_format == 'in':
+                if value not in filter_data:
+                    return False
+            elif search_format == 'contains' and isinstance(filter_data, str):
+                if filter_data not in value:
+                    return False
+            elif search_format == 'icontains' and isinstance(filter_data, str):
+                if filter_data.upper() not in value.upper():
+                    return False
+            elif search_format is None:
+                if filter_data != value:
+                    return False
+        return True
+
+    def check_in_query(self, data):
+        return self._check_data('filter', data) and not self._check_data('exclude', data)
+
+    def set_empty(self):
+        self.empty = True
+
+    def set_limits(self, low: int = None, high: int = None):
+        self['low_mark'], self['high_mark'] = low, high
+        self.is_sliced = True
 
-from django.utils.encoding import force_str
-from django.db import models
-from rest_framework.filters import BaseFilterBackend, OrderingFilter
-from django_filters.rest_framework.backends import DjangoFilterBackend as BaseDjangoFilterBackend
-from django_filters import compat, filters, filterset
-from vstutils.utils import raise_context, translate as _
-
-from .filters import extra_filter
-
-
-def get_serializer_readable_fields(serializer):
-    # pylint: disable=protected-access
-    return {
-        f.source if f.source and '.' not in f.source else f.field_name
-        for f in serializer._readable_fields
-    }
-
-
-class DjangoFilterBackend(BaseDjangoFilterBackend):
-    def get_coreschema_field(self, field):
-        kwargs = {
-            'description': str(field.extra.get('help_text', '')),
-        }
-        if isinstance(field, filters.NumberFilter):
-            field_cls = compat.coreschema.Number
-        elif isinstance(field, filters.BooleanFilter):
-            field_cls = compat.coreschema.Boolean
-        elif isinstance(field, filters.ChoiceFilter):
-            field_cls = compat.coreschema.Enum
-            kwargs['enum'] = tuple(dict(field.field.choices).keys())
+    def has_results(self, *args, **kwargs):
+        # pylint: disable=unused-argument
+        return bool(self.queryset.all()[:2])
+
+    def get_count(self, using):
+        # pylint: disable=unused-argument
+        model = self.model
+        if hasattr(model, 'get_data_generator_count'):
+            return model.get_data_generator_count(self)
+        return len(self.queryset.all())
+
+    def can_filter(self):
+        return self.get('low_mark', None) is None and self.get('high_mark', None) is None
+
+    def clear_ordering(self, *args, **kwargs):
+        # pylint: disable=unused-argument
+        self['ordering'] = []
+
+    def add_ordering(self, *ordering):
+        self['ordering'] = ordering
+
+    @property
+    def order_by(self):
+        return self.get('ordering', ())
+
+
+class CustomModelIterable(ModelIterable):
+    def values_handler(self, unit, fields, pk_name):
+        # pylint: disable=no-member
+        return {f: unit.get(f) if f != 'pk' else unit.get(pk_name) for f in fields}
+
+    def construct_instance(self, data, model, only_fields, defer_fields):
+        if only_fields is not None:
+            data = {k: v for k, v in data.items() if k in only_fields}
+        elif defer_fields is not None:
+            data = {k: v for k, v in data.items() if k not in defer_fields}
+        for field in model._meta.get_fields():
+            if field.attname in data:
+                with raise_context():
+                    data[field.attname] = field.to_python(data[field.attname])
+        return model(**data)
+
+    def __iter__(self):
+        # pylint: disable=protected-access
+        queryset = self.queryset
+        model = queryset.model
+        query = queryset.query
+
+        if hasattr(model, 'get_data_generator'):
+            model_data = model.get_data_generator(query=query)
         else:
-            field_cls = compat.coreschema.String
-        if field.method == extra_filter:  # pylint: disable=comparison-with-callable
-            result = compat.coreschema.Array(
-                items=field_cls(),
-                min_items=1,
-                unique_items=True,
-                **kwargs
+            model_data = model._get_data(
+                chunked_fetch=self.chunked_fetch,
+                **query.get('custom_queryset_kwargs', {})
+            )
+            if isinstance(model._meta.pk, AutoField):
+                for idx, item in enumerate(model_data, 1):
+                    item[model._meta.pk.attname] = idx
+            model_data = list(filter(query.check_in_query, model_data))
+            ordering = query.order_by
+            if ordering:
+                ordering = list(ordering)
+                for idx, value in enumerate(ordering):
+                    if value in ('pk', '-pk'):
+                        ordering[idx] = value.replace('pk', model._meta.pk.name)
+                model_data = multikeysort(
+                    model_data,
+                    ordering,
+                    not query.standard_ordering
+                )
+            elif not query.standard_ordering:
+                model_data.reverse()
+            low = query.get('low_mark', 0)
+            high = query.get('high_mark', len(model_data))
+            model_data = model_data[low:high]
+
+        fields = getattr(self, 'fields', None)
+        if fields is None:
+            handler = partial(
+                self.construct_instance,
+                model=model,
+                only_fields=getattr(self, 'only_fields', None),
+                defer_fields=getattr(self, 'defer_fields', None),
             )
         else:
-            result = field_cls(**kwargs)
-        return result
+            handler = partial(
+                self.values_handler,
+                fields=tuple(fields) or {f.name for f in model._meta.get_fields()},
+                pk_name=model._meta.pk.name,
+            )
+        for data in model_data:
+            yield handler(data)
 
 
-class OrderingFilterBackend(OrderingFilter):
-    def _get_fields_for_schema(self, view):
-        for field in self.get_valid_fields(view.get_queryset(), view, {'request': view.request}):
-            yield field[0]
-            yield f'-{field[0]}'
-
-    def get_schema_fields(self, view):
-        fields = tuple(self._get_fields_for_schema(view))
-        return [
-            compat.coreapi.Field(
-                name=self.ordering_param,
-                required=False,
-                location='query',
-                schema=compat.coreschema.Array(
-                    title=_(force_str(self.ordering_title)),
-                    description=_(force_str(self.ordering_description)),
-                    items=compat.coreschema.Enum(enum=fields),
-                    min_items=1,
-                    unique_items=True,
-                )
+class CustomQuerySet(BQuerySet):
+    custom_iterable_class = CustomModelIterable
+    custom_query_class = Query
+
+    def _filter_or_exclude(self, negate, *args, **kwargs):
+        clone = self._chain()
+        if negate:
+            filter_type = 'exclude'
+        else:
+            filter_type = 'filter'
+        clone.query[filter_type] = clone.query.get(filter_type, {})
+        clone.query[filter_type].update(kwargs)
+        for q_arg in filter(lambda x: isinstance(x, dict), filter(bool, args)):
+            clone.query[filter_type].update(q_arg)  # nocv
+        return clone
+
+    _filter_or_exclude_inplace = _filter_or_exclude
+
+    def last(self):
+        return self.reverse().first()
+
+    def first(self):
+        return next(iter(self), None)
+
+    def values(self, *fields, **expressions):
+        assert not expressions, 'Expressions is not supported on custom non-database models.'
+        clone = self._clone()
+        clone.__iterable_class__ = type('CustomModelIterableValues', (CustomModelIterable,), {'fields': fields})
+        return clone
+
+    def setup_custom_queryset_kwargs(self, **kwargs):
+        qs = self._chain()
+        qs.query['custom_queryset_kwargs'] = kwargs
+        return qs
+
+    def only(self, *fields):
+        clone = self._clone()
+        clone.__iterable_class__ = type('CustomModelIterable', (CustomModelIterable,), {'only_fields': fields})
+        return clone
+
+    def defer(self, *fields):
+        clone = self._clone()
+        clone.__iterable_class__ = type('CustomModelIterable', (CustomModelIterable,), {'defer_fields': fields})
+        return clone
+
+
+class CustomModelBase(ModelBaseClass):
+    def __new__(mcs, name, bases, attrs, **kwargs):
+        new_class = super(CustomModelBase, mcs).__new__(mcs, name, bases, attrs, **kwargs)
+        if not new_class._meta.abstract:
+            pk_name = new_class._meta.pk.attname
+            new_class.add_to_class(
+                pk_name,
+                property(new_class.get_pk_value, new_class.set_pk_value)
             )
-        ]
+        return new_class
 
 
-# Call standard filtering
-class VSTFilterBackend(BaseFilterBackend):
+class ListModel(BaseModel, metaclass=CustomModelBase):
     """
-    A base filter backend class to be inherited from.
-    Example:
+    Custom model which uses a list of dicts with data (attribute `ListModel.data`) instead of database records.
+    Useful when you have a simple list of data.
 
+    Examples:
         .. sourcecode:: python
 
-            from django.utils import timezone
-            from django.db.models import Value, DateTimeField
-
-            from vstutils.api.filter_backends import VSTFilterBackend
+            from vstutils.custom_model import ListModel, CharField
 
-            class CurrentTimeFilterBackend(VSTFilterBackend):
-                def filter_queryset(self, request, queryset, view):
-                    return queryset.annotate(current_time=Value(timezone.now(), output_field=DateTimeField()))
 
-        In this example Filter Backend annotates time in current timezone to any connected
-        model's queryset.
+            class Authors(ListModel):
+                name = CharField(max_length=512)
 
-    In some cases it may be necessary to provide a parameter from a query of request.
-    To define this parameter in the schema, you must overload the get_schema_fields
-    function and specify a list of parameters to use.
+                data = [
+                    {"name": "Sergey Klyuykov"},
+                    {"name": "Michael Taran"},
+                ]
 
-    Example:
+    Sometimes, it may be necessary to switch the data source. For these purposes,
+    you should use the `setup_custom_queryset_kwargs` function, which takes various named arguments,
+    which are also passed to the data initialization function.
+    One such argument for :class:`ListModel` is date_source, which takes any iterable object.
 
+    Examples:
         .. sourcecode:: python
 
-            from django.utils import timezone
-            from django.db.models import Value, DateTimeField
+            from vstutils.custom_model import ListModel, CharField
 
-            from vstutils.api.filter_backends import VSTFilterBackend
 
-            class ConstantCurrentTimeForQueryFilterBackend(VSTFilterBackend):
-                query_param = 'constant'
+            class Authors(ListModel):
+                name = CharField(max_length=512)
 
-                def filter_queryset(self, request, queryset, view):
-                    if self.query_param in request.query_params and request.query_params[self.query_param]:
-                        queryset = queryset.annotate(**{
-                            request.query_params[self.query_param]: Value(timezone.now(), output_field=DateTimeField())
-                        })
-                    return queryset
-
-                    def get_schema_fields(self, view):
-                        return [
-                            compat.coreapi.Field(
-                                name=self.query_param,
-                                required=False,
-                                location='query',
-                                schema=compat.coreschema.String(
-                                    description='Annotate value to queryset'
-                                ),
-                            )
-                        ]
+            qs = Authors.objects.setup_custom_queryset_kwargs(data_source=[
+                {"name": "Sergey Klyuykov"},
+                {"name": "Michael Taran"},
+            ])
 
-        In this example Filter Backend annotates time in current timezone to any connected
-        model's queryset with field name from query `constant`.
+    In this case, we setup source list via `setup_custom_queryset_kwargs` function, and any other chained call
+    is going to work with this data.
     """
-    required = False
-
-    def filter_queryset(self, request, queryset, view):
-        raise NotImplementedError  # nocv
-
-    def get_schema_fields(self, view):
-        """
-        You can also make the filter controls available to the schema autogeneration that REST framework provides,
-        by implementing this method. The method should return a list of coreapi.Field instances.
-        """
-        # pylint: disable=unused-argument
-        return []
 
+    #: List with data dicts. Empty by default.
+    data = []
+    objects = CustomQuerySet.as_manager()
+
+    class Meta:
+        abstract = True
+
+    def get_pk_value(self):
+        return getattr(
+            self,
+            f'_{self.__class__._meta.pk.attname}',
+            None
+        )
 
-class HideHiddenFilterBackend(VSTFilterBackend):
-    """Filter Backend that hides all objects with hidden=True from the queryset"""
-    required = True
+    def set_pk_value(self, value):
+        setattr(
+            self,
+            f'_{self.__class__._meta.pk.attname}',
+            value
+        )
 
-    def filter_queryset(self, request, queryset, view):
+    @classmethod
+    def _get_data(cls, chunked_fetch=False, data_source=None):
         # pylint: disable=unused-argument
-        """
-        Clear objects with hidden attr from queryset.
-        """
-        return getattr(queryset, 'cleared', queryset.all)()
+        return deepcopy(cls.data if data_source is None else data_source)
 
 
-class SelectRelatedFilterBackend(VSTFilterBackend):
-    """
-    Filter Backend that will automatically call prefetch_related and select_related on all relations in queryset.
+class FileModel(ListModel):
     """
-    required = True
-    fields_fetch_map = {
-        'select': (models.ForeignKey,),
-        'prefetch': (models.ManyToManyField, models.ManyToManyField.rel_class)
-    }
-
-    def filter_model_fields(self, view, field_types):
-        serializer = view.get_serializer_class()()
-        readable_fields = get_serializer_readable_fields(serializer)
-        return tuple(
-            f.name
-            for f in serializer.Meta.model()._meta.fields
-            if isinstance(f, field_types) and f.name in readable_fields
-        )
+    Custom model which loads data from YAML-file instead of database.
+    Path to the file stored in `FileModel.file_path` attribute.
 
-    def filter_by_func(self, queryset, queryset_func_name, related):
-        if related:
-            return getattr(queryset, queryset_func_name)(*related)
-        return queryset
-
-    def prefetch(self, queryset_func_name, view, queryset):
-        with raise_context():
-            queryset = self.filter_by_func(
-                queryset,
-                f'{queryset_func_name}_related',
-                self.filter_model_fields(view, self.fields_fetch_map[queryset_func_name])
-            )
-        return queryset
 
-    def filter_queryset(self, request, queryset, view):
-        """
-        Select+prefetch related in queryset.
-        """
-        if request.method != 'GET':
-            return queryset
+    Examples:
+        Source file stored in `/etc/authors.yaml` with content:
 
-        if not queryset.query.select_related and getattr(view, 'select_related', True):
-            queryset = self.prefetch('select', view, queryset)
+        .. sourcecode:: YAML
 
-        # pylint: disable=protected-access
-        if not queryset._prefetch_related_lookups and getattr(view, 'prefetch_related', True):
-            queryset = self.prefetch('prefetch', view, queryset)
-        return queryset
+            - name: "Sergey Klyuykov"
+            - name: "Michael Taran"
 
+        Example:
 
-class DeepViewFilterBackend(VSTFilterBackend):
-    """
-    Backend that filters queryset by column from `deep_parent_field` property of the model.
-    Value for filtering must be provided in query param `__deep_parent`.
+        .. sourcecode:: python
 
-    If param is missing then no filtering is applied.
+            from vstutils.custom_model import FileModel, CharField
 
-    If param is empty value (`/?__deep_parent=`) then objects with no parent (the value of the field whose name is
-    stored in the property `deep_parent_field` of the model is None) returned.
 
-    This filter backend and nested view is automatically added when model has `deep_parent_field` property.
+            class Authors(FileModel):
+                name = CharField(max_length=512)
 
-    Example:
-        .. sourcecode:: python
+                file_path = '/etc/authors.yaml'
 
-            from django.db import models
-            from vstutils.models import BModel
+    """
 
-            class DeepNestedModel(BModel):
-                name = models.CharField(max_length=10)
-                parent = models.ForeignKey('self', null=True, default=None, on_delete=models.CASCADE)
+    class Meta:
+        abstract = True
 
-                deep_parent_field = 'parent'
-                deep_parent_allow_append = True
+    @classmethod
+    def load_file_data(cls):
+        # pylint: disable=no-member
+        return get_file_value(cls.file_path, strip=False)
 
-                class Meta:
-                    default_related_name = 'deepnested'
+    @classmethod
+    def _get_data(cls, chunked_fetch=False):
+        return load(cls.load_file_data(), Loader=Loader)
 
-    In example above if we add this model under path '`deep`', following views will be created: `/deep/` and
-    `/deep/{id}/deepnested/`.
 
-    Filter backend can be used as `/deep/?__deep_parent=1` and will return all `DeepNestedModel` objects
-    whose parent's primary key is `1`.
+class ExternalCustomModel(ListModel):
+    """
+    This custom model is intended for self-implementation of requests to external services.
+    The model allows you to pass filtering, limiting and sorting parameters to an external request,
+    receiving already limited data.
 
-    You can also use generic DRF views, for that you still must set `deep_parent_field`
-    to your model and manually add `DeepViewFilterBackend` to
-    `filter_backends <https://www.django-rest-framework.org/api-guide/filtering/#djangofilterbackend>`_ list.
+    To start using this model, it is enough to implement the ``get_data_generator()`` class method,
+    which receives the query object with the necessary parameters as an argument.
     """
-    field_name = '__deep_parent'
-    field_types = {
-        compat.coreschema.Integer: filters.NumberFilter,  # type: ignore
-        compat.coreschema.String: filters.CharFilter,  # type: ignore
-    }
+    class Meta:
+        abstract = True
 
-    def filter_queryset(self, request, queryset, view):
-        model = queryset.model
-        parent_name: _t.Optional[_t.Text] = getattr(model, 'deep_parent_field', None)
-        nested = getattr(view, 'nested_id', False) or getattr(getattr(view, 'nested_parent_object', None), 'id', None)
-        if view.action != 'list':
-            if parent_name and nested:
-                return queryset.get_children(with_current=True)
-            return queryset
-        if not parent_name or self.field_name not in request.query_params:
-            return queryset
-        filter_data, filter_type_class = self.get_filter_class_with_data(model, request.query_params)
-        if not filter_data:
-            return queryset.filter(**{f'{parent_name}__isnull': True})
-        pk_name = model._meta.pk.attname
-        parent_qs = model.objects.filter(**{pk_name: filter_data})
-        parent_qs = getattr(parent_qs, 'cleared', parent_qs.all)()
-        if nested:
-            queryset = model.objects.all()
-        return filter_type_class(field_name=parent_name, lookup_expr='in').filter(
-            queryset,
-            value=parent_qs.values(pk_name)
-        )
+    @classmethod
+    def get_data_generator(cls, query):
+        raise NotImplementedError
 
-    def get_filter_class_with_data(self, model: _t.Type[models.Model], data: _t.Mapping):
-        # pylint: disable=protected-access
-        filterset_type = self.field_types[type(self.get_coreschema_field(model))]
-        filterset_class = type('FilterSet', (filterset.FilterSet,), {self.field_name: filterset_type()})
-        filterset_object = filterset_class(data, model._default_manager.all())
-        filterset_object.is_valid()
-        return filterset_object.form.cleaned_data[self.field_name], filterset_type
-
-    def get_coreschema_field(self, model: _t.Type[models.Model]):
-        primary_key_field: _t.Optional[models.Field] = model._meta.pk
-        if isinstance(primary_key_field, models.IntegerField):
-            field_cls = compat.coreschema.Integer  # type: ignore
-        else:  # nocv
-            field_cls = compat.coreschema.String  # type: ignore
-        return field_cls(
-            description=''
-        )
 
-    def get_schema_fields(self, view):
-        return [
-            compat.coreapi.Field(
-                name=self.field_name,
-                required=False,
-                location='query',
-                schema=self.get_coreschema_field(view.get_queryset().model),
-            )
-        ]
+class ViewCustomModel(ExternalCustomModel):
+    """
+    This model implements the SQL View programming mechanism over other models.
+    In the ``get_view_queryset()`` method, a query is prepared, and all further actions are implemented on top of it.
+    """
+
+    class Meta:
+        abstract = True
+
+    @classmethod
+    def get_view_queryset(cls):
+        raise NotImplementedError
+
+    @classmethod
+    def get_data_generator(cls, query):
+        qs = cls.get_view_queryset()\
+            .filter(**query.get('filter', {}))\
+            .exclude(**query.get('exclude', {}))\
+            .order_by(*query.order_by)
+        if query.is_sliced:
+            qs = qs[query.get('low_mark'):query.get('high_mark')]
+        return qs.values(*{f.name for f in cls._meta.get_fields()})
+
+    @classmethod
+    def get_data_generator_count(cls, query):
+        return cls.get_data_generator(query).count()
```

### Comparing `vstutils-5.4.9/vstutils/api/filters.py` & `vstutils-5.5.0a1/vstutils/api/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 class FkFilterHandler:
     """
     Simple handler for filtering by relational fields.
 
     :param related_pk: Field name of related model's primary key. Default is 'id'.
     :param related_name: Field name of related model's charfield. Default is 'name'.
-    :param pk_handler: Changes handler for checking value before search. Sends "0" in handler falls. Default is 'int()'.
+    :param pk_handler: Changes handler for checking value before search. Sends "0" if handler falls. Default is 'int()'.
 
     Example:
         .. sourcecode:: python
 
             class CustomFilterSet(filters.FilterSet):
                 author = CharFilter(method=vst_filters.FkFilterHandler(related_pk='pk', related_name='email'))
```

### Comparing `vstutils-5.4.9/vstutils/api/health.py` & `vstutils-5.5.0a1/vstutils/api/health.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/meta.py` & `vstutils-5.5.0a1/vstutils/api/meta.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/metrics.py` & `vstutils-5.5.0a1/vstutils/api/metrics.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/migrations/0001_initial.py` & `vstutils-5.5.0a1/vstutils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/migrations/0002_two_factor.py` & `vstutils-5.5.0a1/vstutils/api/migrations/0002_two_factor.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/migrations/0003_tfa_indexes.py` & `vstutils-5.5.0a1/vstutils/api/migrations/0003_tfa_indexes.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/migrations/0004_user_settings.py` & `vstutils-5.5.0a1/vstutils/api/migrations/0004_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/migrations/0005_db_translations.py` & `vstutils-5.5.0a1/vstutils/api/migrations/0005_db_translations.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/migrations/0006_fix_user_settings.py` & `vstutils-5.5.0a1/vstutils/api/migrations/0006_fix_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/models.py` & `vstutils-5.5.0a1/vstutils/api/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,18 +23,18 @@
         {'code': code, 'name': name}
         for code, name in settings.LANGUAGES
     ]
     code = CharField(primary_key=True, max_length=5)
     name = CharField(max_length=128)
 
     @classmethod
-    def get_etag_value(cls):
-        hashable_str = '_'.join(c for c, _ in settings.LANGUAGES)
+    def get_etag_value(cls, pk=None):
+        hashable_str = '_'.join(c for c, _ in settings.LANGUAGES) + (f'_{pk}' if pk is not None else '')
         if settings.ENABLE_CUSTOM_TRANSLATIONS:
-            hashable_str += CustomTranslations.get_etag_value()
+            hashable_str += CustomTranslations.get_etag_value(pk)
         return hashlib.md5(hashable_str.encode('utf-8')).hexdigest()
 
     def _get_translation_data(self, module_path_string, code, for_server=False):
         data = {}
         for dict_name in filter(bool, ['TRANSLATION'] + ['SERVER_TRANSLATION' if for_server else None]):
             try:
                 translation_data = import_class(module_path_string + '.translations.' + code + f'.{dict_name}')
```

### Comparing `vstutils-5.4.9/vstutils/api/pagination.py` & `vstutils-5.5.0a1/vstutils/api/pagination.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/parsers.py` & `vstutils-5.5.0a1/vstutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/permissions.py` & `vstutils-5.5.0a1/vstutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/renderers.py` & `vstutils-5.5.0a1/vstutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/responses.py` & `vstutils-5.5.0a1/vstutils/api/responses.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/responses.pyi` & `vstutils-5.5.0a1/vstutils/api/responses.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/routers.py` & `vstutils-5.5.0a1/vstutils/api/routers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/routers.pyi` & `vstutils-5.5.0a1/vstutils/api/routers.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/schema/generators.py` & `vstutils-5.5.0a1/vstutils/api/schema/generators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/schema/info.py` & `vstutils-5.5.0a1/vstutils/api/schema/info.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/schema/inspectors.py` & `vstutils-5.5.0a1/vstutils/api/schema/inspectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import warnings
 from copy import deepcopy
 from typing import Dict, Type, Text, Any, Union, Set
 from collections import OrderedDict
 
 from django.http import FileResponse
 from django.db import models
 from django.utils.functional import cached_property
-from drf_yasg.inspectors.base import FieldInspector, NotHandled
+from drf_yasg.inspectors.base import FieldInspector, FilterInspector, NotHandled
 from drf_yasg.inspectors.field import ReferencingSerializerInspector, decimal_field_type
 from drf_yasg import openapi
 from drf_yasg.inspectors.query import CoreAPICompatInspector, force_real_str, coreschema  # type: ignore
 from rest_framework.fields import Field, JSONField, DecimalField, ListField, empty
 from rest_framework.serializers import Serializer
 
 from .. import fields, serializers, validators
@@ -221,23 +222,24 @@
             return NotHandled
 
         SwaggerType, ChildSwaggerType = self._get_partial_types(
             field, swagger_object_type, use_references, **kw
         )
 
         field_format = FORMAT_FK
+        in_ = kw.get('in_')
         options = {
             'model': openapi.SchemaRef(
                 self.components.with_scope(openapi.SCHEMA_DEFINITIONS),
                 field.select_model, ignore_unresolved=True
             ),
             'value_field': field.autocomplete_property,
             'view_field': field.autocomplete_represent,
-            'usePrefetch': field.use_prefetch,
-            'makeLink': field.make_link,
+            'usePrefetch': field.use_prefetch if in_ != 'query' else False,
+            'makeLink': field.make_link if in_ != 'query' else False,
             'dependence': field.dependence,
             'filters': field.filters,
         }
 
         if isinstance(field, fields.DeepFkField):
             field_format = FORMAT_DEEP_FK
             options = {
@@ -402,15 +404,15 @@
                 if 'x-options' not in items:
                     items['x-options'] = {}
                 items['x-options']['backgroundFillColor'] = field.background_fill_color
 
         if field.max_content_size:
             items['properties']['content']['maxLength'] = field.max_content_size
         if field.min_content_size:
-            items['properties']['content']['minLength'] = field.max_content_size
+            items['properties']['content']['minLength'] = field.min_content_size
 
         x_validators: Dict[str, Union[Set, int, str]]
         x_validators = items['x-validators'] = {
             'extensions': set()
         }
         for validator in filter(lambda x: isinstance(x, validators.FileMediaTypeValidator), field.validators):
             if isinstance(validator, validators.ImageBaseSizeValidator) and items['x-format'] == FORMAT_NAMED_BIN_IMAGE:
@@ -540,49 +542,70 @@
 
         if field.default != empty:
             kwargs['default'] = str(field.default)
 
         return SwaggerType(**field_extra_handler(field, **kwargs))
 
 
-class NestedFilterInspector(CoreAPICompatInspector):
-    def get_filter_parameters(self, filter_backend):  # nocv
-        subaction_list_actions = [
-            f'{name}_list'
-            for name in getattr(self.view, '_nested_args', {}).keys()
-        ]
-        if self.view.action not in subaction_list_actions:
-            return NotHandled
-        if self.method != 'GET':
-            return NotHandled
-        nested_view = getattr(self.view, self.view.action, None)
-        nested_view_filter_class = getattr(nested_view, '_nested_filter_class', None)
-        filter_class = getattr(self.view, 'filterset_class', getattr(self.view, 'filter_class', None))
-        self.view.filter_class = nested_view_filter_class
-        result = super().get_filter_parameters(filter_backend)
-        self.view.filter_class = filter_class
-        return result
+class SerializedFilterBackendsInspector(FilterInspector):
+    def get_filter_parameters(self, filter_backend):
+        if getattr(filter_backend, 'serializer_class', None) is None or \
+                getattr(filter_backend, 'no_schema_serializer', False):
+            return NotHandled
+        # pylint: disable=protected-access
+        return self.request._schema.serializer_to_parameters(
+            serializer=filter_backend.serializer_class(),
+            in_=openapi.IN_QUERY
+        )
 
 
 class ArrayFilterQueryInspector(CoreAPICompatInspector):
     @cached_property
-    def fields_map(self):
+    def fields_map(self):  # nocv
+        warnings.warn(
+            "CoreAPI and coreschema is deprecated and will removed in 6.x.",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
         return {
             f.name: f
             for f in self.view.get_queryset().model._meta.fields
         }
 
-    def coreapi_field_to_parameter(self, field, schema=None):
+    def param_to_schema(self, param):
+        return openapi.Parameter(
+            name=param['name'],
+            in_=param['in'],
+            description=param.get('description'),
+            **param['schema'],
+        )
+
+    def get_paginator_parameters(self, paginator):
+        if hasattr(paginator, 'get_schema_operation_parameters'):
+            return list(map(self.param_to_schema, paginator.get_schema_operation_parameters(self.view)))
+        return super().get_paginator_parameters(paginator)  # nocv
+
+    def get_filter_parameters(self, filter_backend):
+        if hasattr(filter_backend, 'get_schema_operation_parameters'):
+            return list(map(self.param_to_schema, filter_backend.get_schema_operation_parameters(self.view)))
+        return super().get_filter_parameters(filter_backend)
+
+    def coreapi_field_to_parameter(self, field, schema=None):  # nocv
         """
         Convert an instance of `coreapi.Field` to a swagger :class:`.Parameter` object.
 
         :param coreapi.Field field:
         :param coreschema..Schema schema:
         :rtype: openapi.Parameter
         """
+        warnings.warn(
+            "CoreAPI and coreschema is deprecated and will removed in 6.x.",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
         location_to_in = {
             'query': openapi.IN_QUERY,
             'path': openapi.IN_PATH,
             'form': openapi.IN_FORM,
             'body': openapi.IN_FORM,
         }
         coreapi_types = {
@@ -623,14 +646,33 @@
             description=force_real_str(schema_field.description) if schema_field else None,
             type=schema_type,
             **OrderedDict((attr, getattr(schema_field, attr, None)) for attr in coreschema_attrs),
             **attributes
         )
 
 
+class NestedFilterInspector(ArrayFilterQueryInspector):
+    def get_filter_parameters(self, filter_backend):  # nocv
+        subaction_list_actions = [
+            f'{name}_list'
+            for name in getattr(self.view, '_nested_args', {}).keys()
+        ]
+        if self.view.action not in subaction_list_actions:
+            return NotHandled
+        if self.method != 'GET':
+            return NotHandled
+        nested_view = getattr(self.view, self.view.action, None)
+        nested_view_filter_class = getattr(nested_view, '_nested_filter_class', None)
+        filter_class = getattr(self.view, 'filterset_class', getattr(self.view, 'filter_class', None))
+        self.view.filter_class = nested_view_filter_class
+        result = super().get_filter_parameters(filter_backend)
+        self.view.filter_class = filter_class
+        return result
+
+
 class VSTReferencingSerializerInspector(ReferencingSerializerInspector):
     def get_serializer_ref_name(self, serializer: Any):
         if isinstance(serializer, serializers.serializers.ListSerializer):
             return super().get_serializer_ref_name(serializer.child)
         return super().get_serializer_ref_name(serializer)
 
     def handle_schema(self, field: Serializer, schema: openapi.SwaggerDict, use_references: bool = True):
```

### Comparing `vstutils-5.4.9/vstutils/api/schema/schema.py` & `vstutils-5.5.0a1/vstutils/api/schema/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from ...models.base import get_proxy_labels
 from ..decorators import NestedWithAppendMixin
 from ..base import detail_actions
 from . import inspectors as vst_inspectors
 
 
 class VSTAutoSchema(SwaggerAutoSchema):
+    paginator_inspectors = [
+        vst_inspectors.ArrayFilterQueryInspector,
+    ] + swagger_settings.DEFAULT_PAGINATOR_INSPECTORS
     field_inspectors = [
         vst_inspectors.CommaMultiSelectFieldInspector,
         vst_inspectors.FkFieldInspector,
         vst_inspectors.DynamicJsonTypeFieldInspector,
         vst_inspectors.AutoCompletionFieldInspector,
         vst_inspectors.VSTFieldInspector,
         vst_inspectors.VSTReferencingSerializerInspector,
@@ -31,26 +34,28 @@
         vst_inspectors.DecimalFieldInspector,
         vst_inspectors.CSVFileFieldInspector,
         vst_inspectors.FileInStringInspector,
     ] + swagger_settings.DEFAULT_FIELD_INSPECTORS
 
     filter_inspectors = [
         vst_inspectors.NestedFilterInspector,
+        vst_inspectors.SerializedFilterBackendsInspector,
         vst_inspectors.ArrayFilterQueryInspector,
     ] + swagger_settings.DEFAULT_FILTER_INSPECTORS
 
     default_status_messages: dict = {
         s[1]: ' '.join(s[2:])
         for s in map(lambda j: j.split('_'), filter(lambda x: x.startswith("HTTP_"), dir(status)))
     }
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._sch = args[0].schema
         self._sch.view = args[0]
+        self.request._schema = self
 
     def _get_nested_view_class(self, nested_view, view_action_func):
         # pylint: disable=protected-access
         if not hasattr(view_action_func, '_nested_name'):
             return nested_view
 
         nested_action_name = '_'.join(view_action_func._nested_name.split('_')[1:])
@@ -192,14 +197,17 @@
     def get_operation(self, operation_keys=None):
         result: Operation = self.__perform_with_nested('get_operation', operation_keys)
         _nested_wrapped_view = getattr(self.view, '_nested_wrapped_view', None)
         if result['operationId'].endswith('_add') and _nested_wrapped_view:
             # pylint: disable=protected-access
             result['x-allow-append'] = issubclass(_nested_wrapped_view, NestedWithAppendMixin)
 
+        if getattr(self.view, 'hidden', None) or self.overrides.get('x-hidden'):
+            result['x-hidden'] = True
+
         params_to_override = ('x-title', 'x-icons')
         if self.method.lower() == 'get':
             subscribe_view = self.__get_nested_view_and_subaction(self.view)[0]
             queryset = getattr(subscribe_view, 'queryset', None)
             if queryset is not None:
                 # pylint: disable=protected-access
                 subscribe_labels = [queryset.model._meta.label, *get_proxy_labels(queryset.model)]
```

### Comparing `vstutils-5.4.9/vstutils/api/serializers.py` & `vstutils-5.5.0a1/vstutils/api/serializers.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 import typing as _t
 
 import orjson
 from django.db import models
 from django.http.request import QueryDict
-from rest_framework import serializers
+from rest_framework import serializers, fields as drf_fields
 from rest_framework.utils.field_mapping import get_relation_kwargs
 
 from . import fields
 from .. import utils
 from ..models.fields import (
     NamedBinaryFileInJSONField,
     NamedBinaryImageInJSONField,
@@ -53,37 +53,59 @@
             }
             for depend_field in missed_interfield_connections:
                 data[depend_field.field_name] = getattr(self.instance, depend_field.field_name, None)
 
         return super().to_internal_value(data)
 
 
-class BaseSerializer(DependFromFkSerializerMixin, serializers.Serializer):
+class SerializerMetaClass(serializers.SerializerMetaclass):
+    @classmethod
+    def _get_declared_fields(
+            mcs,
+            bases: _t.Sequence[type],
+            attrs: _t.Dict[str, _t.Any]
+    ) -> _t.Dict[str, drf_fields.Field]:
+        if (meta := attrs.get('Meta')) and (generated_fields := getattr(meta, 'generated_fields', None)):
+            field_fabric = getattr(
+                meta,
+                'generated_field_factory',
+                lambda f: drf_fields.CharField(required=False, allow_blank=True, allow_null=True)
+            )
+            for field in generated_fields:
+                field_name = field.replace('.', '_')
+                if field_name not in attrs:
+                    attrs[field_name] = field_fabric(field)
+        return super()._get_declared_fields(bases=bases, attrs=attrs)
+
+
+class BaseSerializer(DependFromFkSerializerMixin, serializers.Serializer, metaclass=SerializerMetaClass):
     """
     Default serializer with logic to work with objects.
     Read more in `DRF serializer's documentation
     <https://www.django-rest-framework.org/api-guide/serializers/#serializers>`_
     how to create Serializers and work with them.
-    """
 
-    # pylint: disable=abstract-method
+    .. note::
+        You can also setup ``generated_fields`` in class attribute ``Meta`` to get serializer
+        with default CharField fields. Setup attribute ``generated_field_factory`` to change default fabric method.
+    """
 
     def create(self, validated_data):  # nocv
         return validated_data
 
     def update(self, instance, validated_data):  # nocv
         if isinstance(instance, dict):
             instance.update(validated_data)
         else:
             for key, value in validated_data.items():
                 setattr(instance, key, value)
         return instance
 
 
-class VSTSerializer(DependFromFkSerializerMixin, serializers.ModelSerializer):
+class VSTSerializer(DependFromFkSerializerMixin, serializers.ModelSerializer, metaclass=SerializerMetaClass):
     """
     Default model serializer based on :class:`rest_framework.serializers.ModelSerializer`.
     Read more in `DRF documentation <https://www.django-rest-framework.org/api-guide/serializers/#modelserializer>`_
     how to create Model Serializers.
     This serializer matches model fields to extended set of serializer fields.
     List of available pairs specified in  `VSTSerializer.serializer_field_mapping`.
     For example, to set :class:`vstutils.api.fields.FkModelField` in serializer use
@@ -141,15 +163,15 @@
         # if DRF ForeignField in model or related_model is not BModel, perform default DRF logic
         return super().build_relational_field(field_name, relation_info)
 
 
 class EmptySerializer(BaseSerializer):
     """
     Default serializer for empty responses.
-    In generated GUI this means that action button which will not show additional view before execution.
+    In generated GUI this means that action button won't show additional view before execution.
     """
 
 
 class DataSerializer(EmptySerializer):
     allowed_data_types = (
         str,
         dict,
```

### Comparing `vstutils-5.4.9/vstutils/api/throttling.py` & `vstutils-5.5.0a1/vstutils/api/throttling.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/api/validators.py` & `vstutils-5.5.0a1/vstutils/api/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,17 +173,17 @@
                 f' ({",".join(self.extensions)}).'
             )
         self.media_type = file_media_type.split(sep='/')[1].upper()
 
 
 class ImageValidator(FileMediaTypeValidator):
     """
-        Base Image Validation class
-        Validates image format
-        Won't work if Pillow isn't installed
+        Base Image Validation class.
+        Validates image format.
+        Won't work if Pillow isn't installed.
         Base Image Validation class.
         Validates media types.
 
         :param extensions: Tuple or List of file extensions, that should pass the validation
 
         Raises rest_framework.exceptions.ValidationError: in case file extension are not in the list
         """
@@ -228,15 +228,15 @@
             self.img = Image.open(BytesIO(base64.b64decode(value['content'])))
         except UnidentifiedImageError as err:
             raise serializers.ValidationError(self.error_msg) from err
 
 
 class ImageBaseSizeValidator(ImageOpenValidator):
     """
-    Validates image size
+    Validates image size.
     To use this class for validating image width/height, rewrite
     self.orientation to ('height',) or ('width',) or ('height', 'width')
 
     Raises rest_framework.exceptions.ValidationError: if not(min <= (height or width) <= max)
     """
     orientation: _t.Union[_t.Union[_t.Tuple[str], _t.Tuple[str, str]], _t.Tuple] = ()
```

### Comparing `vstutils-5.4.9/vstutils/api/views.py` & `vstutils-5.5.0a1/vstutils/api/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/asgi.py` & `vstutils-5.5.0a1/vstutils/asgi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import posixpath
+import time
 
 from django.conf import settings
 from django.core.asgi import get_asgi_application
 from django.contrib.staticfiles import finders
 from fastapi import FastAPI, Request
-from fastapi.responses import PlainTextResponse, FileResponse
+from fastapi.responses import PlainTextResponse, FileResponse, ORJSONResponse
 from fastapi.middleware.gzip import GZipMiddleware
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.staticfiles import StaticFiles
 from starlette.staticfiles import NotModifiedResponse
 
 from .signals import before_mount_app
 
@@ -59,9 +60,23 @@
 @application.get('/.well-known/{file_path:path}')
 async def well_known(file_path: str, request: Request):
     return await static(f'.well-known/{file_path}', request)
 
 
 before_mount_app.send(sender=application, static=static)
 
+if not any(m.path == f'/{settings.API_URL}/live/' for m in application.routes):
+    @application.get(f'/{settings.API_URL}/live/')
+    async def api_live_check():
+        return ORJSONResponse({"status": "ok"})
+
+
+@application.middleware('http')
+async def add_server_timing_header(request: Request, call_next):
+    start_time = time.time()
+    response = await call_next(request)
+    response.headers['Server-Timing'] = f'total;dur={round((time.time()-start_time)*1000, 2)}'
+    return response
+
+
 if not any(m.path == '/' for m in application.routes):
     application.mount("/", get_asgi_application())
```

### Comparing `vstutils-5.4.9/vstutils/asgi_worker.py` & `vstutils-5.5.0a1/vstutils/asgi_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/auth.py` & `vstutils-5.5.0a1/vstutils/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import traceback
+import warnings
 
 from django.core.cache import cache
 from django.contrib.auth import get_user_model, backends
 from django.db.models import signals, QuerySet
 from django.dispatch import receiver
 from django.conf import settings
 from django.http.request import HttpRequest
@@ -19,14 +20,20 @@
 UserModel = get_user_model()
 logger = logging.getLogger(settings.VST_PROJECT_LIB)
 user_cache_prefix = 'auth_user_id_val'
 secure_serializer = SecurePickling()
 
 
 if settings.CACHE_AUTH_USER:
+    warnings.warn(
+        "This feature is deprecated and will removed in 6.x version",
+        category=DeprecationWarning,
+        stacklevel=2
+    )
+
     @receiver(signals.post_save, sender=UserModel)
     @receiver(signals.post_delete, sender=UserModel)
     def invalidate_user_from_cache(instance: UserModel, created=False, *args, **kwargs):
         if created:
             return
         cache.delete(f'{user_cache_prefix}_{instance.id}')
```

### Comparing `vstutils-5.4.9/vstutils/auth.pyi` & `vstutils-5.5.0a1/vstutils/auth.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/celery_beat_scheduler.py` & `vstutils-5.5.0a1/vstutils/celery_beat_scheduler.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/doc_themes/vst-sphinx-theme/layout.html` & `vstutils-5.5.0a1/vstutils/doc_themes/vst-sphinx-theme/layout.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/environment.py` & `vstutils-5.5.0a1/vstutils/environment.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/exceptions.py` & `vstutils-5.5.0a1/vstutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/gui/context.py` & `vstutils-5.5.0a1/vstutils/gui/context.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/gui/forms.py` & `vstutils-5.5.0a1/vstutils/gui/forms.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/gui/pwa_manifest.py` & `vstutils-5.5.0a1/vstutils/gui/pwa_manifest.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/gui/views.py` & `vstutils-5.5.0a1/vstutils/gui/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/ldap_utils.py` & `vstutils-5.5.0a1/vstutils/ldap_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/management/commands/_base.py` & `vstutils-5.5.0a1/vstutils/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/management/commands/celery_inspect.py` & `vstutils-5.5.0a1/vstutils/management/commands/celery_inspect.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/management/commands/dockerrun.py` & `vstutils-5.5.0a1/vstutils/management/commands/dockerrun.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/management/commands/newproject.py` & `vstutils-5.5.0a1/vstutils/management/commands/newproject.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/management/commands/run_task.py` & `vstutils-5.5.0a1/vstutils/management/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/management/commands/runrpc.py` & `vstutils-5.5.0a1/vstutils/management/commands/runrpc.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/management/commands/runserver.py` & `vstutils-5.5.0a1/vstutils/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/management/commands/web.py` & `vstutils-5.5.0a1/vstutils/management/commands/web.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/middleware.py` & `vstutils-5.5.0a1/vstutils/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
             response['Response-Time'] = str(total_time)
         else:
             if response_durations:
                 response_durations = f', {", ".join(map(self.__duration_handler, response_durations.items()))}'
             else:
                 response_durations = ""
             response_durations += f', db_execution_time;dur={self._round_time(ql.queries_time)}'
-            response['Server-Timing'] = f'total;dur={total_time}{response_durations or ""}'
+            response['Server-Timing'] = f'total_app;dur={total_time}{response_durations or ""}'
         return response
 
 
 class LangMiddleware(BaseMiddleware):
     __slots__ = ()
 
     def get_lang_object(self, request: HttpRequest) -> _t.Tuple[Language, bool]:
@@ -238,14 +238,15 @@
             response.set_cookie('lang', request.language.code, domain=settings.SESSION_COOKIE_DOMAIN)  # type: ignore
         if 'Content-Language' not in response:
             response['Content-Language'] = request.language.code  # type: ignore
         return response
 
 
 class TwoFaMiddleware(BaseMiddleware):
+    redirect_name = 'login'
     pass_names = (
         'login',
         'logout',
         'pwa_manifest',
         'service_worker',
         'offline_gui',
         'user_registration',
@@ -265,15 +266,15 @@
         return any([
             url_name not in self.pass_names,
             url_name is not None and url_name.startswith('password_reset')
         ])
 
     def get_response_handler(self, request: HttpRequest) -> ResponseHandlerType:
         if request.user.need_twofa and self.check_url_name(request):  # type: ignore
-            return redirect('login')
+            return redirect(self.redirect_name)
         return super().get_response_handler(request)
 
 
 class FrontendChangesNotifications(BaseMiddleware):
     __slots__ = ('notificator_class',)
 
     def __init__(self, *args, **kwargs):
```

### Comparing `vstutils-5.4.9/vstutils/models/__init__.py` & `vstutils-5.5.0a1/vstutils/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Default Django model classes overrides in `vstutils.models` module.
 """
 import logging
-import orjson
 
 from django.apps import apps
 from django.db import models
 from django.conf import settings
 
 from .base import ModelBaseClass, get_proxy_labels, LAZY_MODEL
 from .queryset import BQuerySet, _Manager
@@ -16,15 +15,15 @@
     NamedBinaryFileInJSONField,
     NamedBinaryImageInJSONField,
     MultipleNamedBinaryFileInJSONField,
     MultipleNamedBinaryImageInJSONField,
     FkModelField
 )
 from ..utils import raise_context
-from .custom_model import ListModel, FileModel, CustomQuerySet
+from .custom_model import ListModel, FileModel, ExternalCustomModel, ViewCustomModel, CustomQuerySet
 
 
 logger = logging.getLogger('vstutils')
 
 
 class Manager(_Manager.from_queryset(BQuerySet)):
     """
@@ -103,15 +102,15 @@
 
             API[VST_API_VERSION][r'task'] = {
                 'model': 'your_application.models.Task'
             }
 
         For primary access to generated view inherit from `Task.generated_view` property.
 
-        To make translation on frontend easier use ``_translate_model`` attribute with model_name
+        To make translation on frontend easier use ``_translate_model`` attribute with model_name.
 
         List of meta-attributes for generating a view:
 
         - ``_view_class`` - list of additional view classes to inherit from,
           class or string to import with base class ViewSet.
           Constants are also supported:
 
@@ -148,15 +147,15 @@
           :class:`vstutils.api.filters.DefaultNameFilter`. If both conditions are present, inheritance will be from all
           of the above classes.
           Possible values include `list` of fields to filter or `dict` where key is a field name and value is
           a Filter class. Dict extends attribute functionality and provides ability to override filter field class
           (None value disables overriding).
         - ``_search_fields`` - tuple or list of fields using for search requests.
           By default (or `None`) get all filterable fields in detail view.
-        - ``_copy_attrs`` - list of model-instance attributes indicates that object is copiable with this attrs.
+        - ``_copy_attrs`` - list of model-instance attributes indicates that object is copyable with this attrs.
         - ``_nested`` - key-value mapping with nested views (key - nested name,
           kwargs for :class:`vstutils.api.decorators.nested_view` decorator but supports
           ``model`` attribute as nested). ``model`` can be string for import.
         - ``_extra_view_attributes`` - key-value mapping with additional view attributes,
           but has less priority over generated attributes.
```

### Comparing `vstutils-5.4.9/vstutils/models/base.py` & `vstutils-5.5.0a1/vstutils/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,16 @@
     # additional attrs which means that this view allowed to copy elements
     "copy_attrs": None,
     # key-value mapping with nested views (key - nested name, kwargs for nested decorator)
     "nested": None,
     # additional view's settings
     **dict(reduce(operator.add, [((f'pre_{i}', None), (i, None), (f'override_{i}', False)) for i in view_settings])),
     "extra_view_attributes": None,
+    # if true - view will be hidden on frontend
+    "hidden": False,
 }
 
 
 # Handlers
 def _translate_search_help_text(field_name, related_name):
     return _("Search by {}'s primary key or {}").format(_(field_name), _(related_name))
 
@@ -134,15 +136,16 @@
     result = {}
     for items in reversed(list(mro_items)):
         result.update(get_append_to_view(items, is_inherit_append_to_view))
     return result
 
 
 def update_cache_for_model(instance, **kwargs):
-    kwargs.get('cached_model_class', instance.__class__).set_etag_value()
+    cached_model_class = kwargs.get('cached_model_class', instance.__class__)
+    cached_model_class.set_etag_value(instance.pk if isinstance(instance, cached_model_class) else None)
 
 
 def get_first_match_name(field_names, default=None):
     return next(
         (i for i in field_names if i in DEFAULT_VIEW_FIELD_NAMES),
         next(iter(field_names[1:]), default)
     )
@@ -264,25 +267,31 @@
                 receiver(post_save, sender=label)(update_cache_for_model_related)
                 receiver(post_delete, sender=label)(update_cache_for_model_related)
         return model_class
 
     def get_proxy_labels(cls):
         return get_proxy_labels(cls)  # nocv
 
-    def get_api_cache_name(cls):
-        return f'api_caching_table_{cls._meta.db_table}'
+    def get_api_cache_name(cls, pk=None):
+        return f'api_caching_table_{cls._meta.db_table}' + (f'_{pk}' if pk is not None else "")
 
-    def get_etag_value(cls):
+    def get_etag_value(cls, pk=None):
         # pylint: disable=no-value-for-parameter
-        return str(django_caches['etag'].get_or_set(cls.get_api_cache_name(), str(uuid.uuid4())))
+        if pk and django_caches['etag'].get(f'clear_{cls.get_api_cache_name()}') == 1:
+            return cls.set_etag_value(pk)
+        return str(django_caches['etag'].get_or_set(cls.get_api_cache_name(pk), str(uuid.uuid4())))
 
-    def set_etag_value(cls):
+    def set_etag_value(cls, pk=None):
         # pylint: disable=no-value-for-parameter
         new_value = str(uuid.uuid4())
         django_caches['etag'].set(cls.get_api_cache_name(), new_value)
+        if pk:
+            django_caches['etag'].set(cls.get_api_cache_name(pk), new_value)
+        else:
+            django_caches['etag'].set(f'clear_{cls.get_api_cache_name()}', 1)
         return new_value
 
     @classproperty
     @lru_cache()
     def generated_view(cls):
         # pylint: disable=no-value-for-parameter
         return cls.get_view_class()
@@ -535,14 +544,16 @@
         # pylint: disable=no-value-for-parameter
         metadata = cls.get_extra_metadata()
         metadata.update(extra_options)
         list_fields = _ensure_pk_in_fields(cls, metadata['list_fields'])
         detail_fields = _ensure_pk_in_fields(cls, metadata['detail_fields'] or list_fields)
 
         view_attributes = {'model': cls, **(metadata['extra_view_attributes'] or {})}
+        if metadata['hidden']:
+            view_attributes['hidden'] = True
 
         serializer_class = metadata['serializer_class']
         serializers = {
             'serializer_class': cls.get_serializer_class(  # pylint: disable=no-value-for-parameter
                 serializer_class=serializer_class,
                 serializer_class_name=cls.get_list_serializer_name(metadata),  # pylint: disable=no-value-for-parameter
                 fields=list_fields,
```

### Comparing `vstutils-5.4.9/vstutils/models/cent_notify.py` & `vstutils-5.5.0a1/vstutils/models/cent_notify.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/models/custom_model.pyi` & `vstutils-5.5.0a1/vstutils/models/custom_model.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     @classmethod
     def load_file_data(cls) -> _t.Text:
         ...
 
 
 class Query(_t.Dict):
     distinct_fields: _t.ClassVar[bool]
+    is_sliced: _t.ClassVar[bool]
     queryset: CustomQuerySet
     standard_ordering: _t.Union[bool, property]
     model: _t.Union[ListModel, property]
 
     def __init__(self, queryset: CustomQuerySet, *args, **kwargs):
         ...
 
@@ -110,7 +111,29 @@
         ...
 
     def clear_ordering(self, *args, **kwargs) -> None:
         ...
 
     def add_ordering(self, *ordering) -> None:
         ...
+
+
+class ExternalCustomModel(ListModel):
+    @classmethod
+    def get_data_generator(cls, query: Query):
+        raise NotImplementedError
+
+
+class ViewCustomModel(ExternalCustomModel):
+    view_queryset: BQuerySet
+
+    @classmethod
+    def get_view_queryset(cls) -> BQuerySet:
+        ...
+
+    @classmethod
+    def get_data_generator(cls, query: Query) -> BQuerySet:
+        ...
+
+    @classmethod
+    def get_data_generator_count(cls, query: Query) -> int:
+        ...
```

### Comparing `vstutils-5.4.9/vstutils/models/decorators.py` & `vstutils-5.5.0a1/vstutils/models/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/models/fields.py` & `vstutils-5.5.0a1/vstutils/models/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 class MultipleFieldFile(FieldFile):
     """
     Subclasses :class:`django.db.models.fields.files.FieldFile`. Provides :meth:`MultipleFieldFile.save`
     and :meth:`MultipleFieldFile.delete` to manipulate the underlying file, as well as update the
     associated model instance.
     """
+
     def __init__(self, instance, field, name):
         super(MultipleFieldFile, self).__init__(instance, field, name)
         self._old_name = self.name
 
     def _set_attr_value(self):
         """
         Set new value of file to object attr.
@@ -89,17 +90,18 @@
 
     .. sourcecode:: python
 
         from myapp.models import MyModel
         instance = MyModel.objects.get(pk=1)
         instance.files[0].size
     """
+
     def get_file(self, file, instance):
         """
-        Always return valid attr_class object.For details on logic see
+        Always return valid attr_class object. For details on logic see
         :meth:`django.db.models.fields.files.FileDescriptor.__get__`.
         """
         if isinstance(file, str) or file is None:
             attr = self.field.attr_class(instance, self.field, file)
             file = attr
 
         elif isinstance(file, SimpleUploadedFile):
@@ -131,14 +133,15 @@
 
 
 class MultipleFileMixin:
     """
     Mixin suited to use with :class:`django.db.models.fields.files.FieldFile` to transform it to
     a Field with list of files.
     """
+
     def __init__(self, **kwargs):
         kwargs['max_length'] = None
         super().__init__(**kwargs)
 
     def pre_save(self, model_instance, add):
         """
         Call .save() method on every file in list
@@ -183,14 +186,15 @@
 
 
 class MultipleImageFieldFile(ImageFile, MultipleFieldFile):
     """
     Subclasses :class:`MultipleFieldFile` and :class:`ImageFile mixin`,
     handles deleting _dimensions_cache when file is deleted.
     """
+
     def delete(self, save=True):
         if hasattr(self, '_dimensions_cache'):
             del self._dimensions_cache
         super().delete(save)
 
 
 class MultipleImageField(MultipleFileMixin, ImageField):
@@ -227,17 +231,17 @@
     `vstutils.api.MultipleNamedBinaryFileInJSONField` in serializer.
     """
 
 
 class MultipleNamedBinaryImageInJSONField(MultipleNamedBinaryFileInJSONField):
     """
     Extends :class:`django.db.models.TextField`. Use this field in :class:`vstutils.models.BModel` to get
-    `vstutils.api.MultipleNamedBinaryImageInJSONField in serializer`.
+    `vstutils.api.MultipleNamedBinaryImageInJSONField` in serializer.
     """
 
 
 class FkModelField(ForeignKey):
     """
     Extends :class:`django.db.models.ForeignKey`. Use this field in :class:`vstutils.models.BModel` to get
-    `vstutils.api.FkModelField in serializer`. To set Foreign Key relation set `to` argument to string path to model
+    `vstutils.api.FkModelField` in serializer. To set Foreign Key relation set `to` argument to string path to model
     or to Model Class as in :class:`django.db.models.ForeignKey`
     """
```

### Comparing `vstutils-5.4.9/vstutils/models/queryset.py` & `vstutils-5.5.0a1/vstutils/models/queryset.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/settings.ini` & `vstutils-5.5.0a1/vstutils/settings.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/settings.py` & `vstutils-5.5.0a1/vstutils/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,14 @@
         'cors_expose_headers': ConfigListType,
         'cors_allow_methods': ConfigListType,
         'cors_allow_headers': ConfigListType,
         'cors_preflight_max_age': ConfigIntSecondsType,
         'session_timeout': ConfigIntSecondsType,
         'page_limit': ConfigIntType,
         'rest_page_limit': ConfigIntType,
-        'public_openapi': ConfigBoolType,
         'openapi_cache_timeout': ConfigIntType,
         'enable_gravatar': ConfigBoolType,
         'rest_swagger': ConfigBoolType,
         'request_max_size': cconfig.BytesSizeType(),
         'x_frame_options': cconfig.StrType(),
         'use_x_forwarded_host': ConfigBoolType,
         'use_x_forwarded_port': ConfigBoolType,
@@ -188,15 +187,15 @@
         'max_tfa_attempts': ConfigIntType,
         'etag_default_timeout': ConfigIntSecondsType,
         'allow_auto_image_resize': ConfigBoolType,
         'enable_metrics': ConfigBoolType,
     }
 
 
-class UvicornSection(cconfig.Section):
+class UvicornSection(BaseAppendSection):
     types_map = {
         'ws_max_size': ConfigIntType,
         'ws_ping_interval': ConfigFloatType,
         'ws_ping_timeout': ConfigFloatType,
         'ws_per_message_deflate': ConfigBoolType,
         'access_log': ConfigBoolType,
         'use_colors': ConfigBoolType,
@@ -240,14 +239,15 @@
 class DBOptionsSection(cconfig.Section):
     types_map = {
         'timeout': ConfigIntSecondsType,
         'connect_timeout': ConfigIntSecondsType,
         'read_timeout': ConfigIntSecondsType,
         'write_timeout': ConfigIntSecondsType,
         'isolation_level': ConfigIntType,
+        'server_side_binding': ConfigBoolType,
     }
 
 
 class CacheSection(BackendSection):
     types_map = {
         'timeout': ConfigIntSecondsType,
         'location': LocationsType(),
@@ -441,15 +441,14 @@
             'session_timeout': env.str(f"{ENV_NAME}_SESSION_TIMEOUT", default='2w'),
             'static_files_url': '/static/',
             'page_limit': env.int(f'{ENV_NAME}_WEB_PAGE_LIMIT', default=20),
             'rest_page_limit': env.int(f'{ENV_NAME}_WEB_REST_PAGE_LIMIT', default=1000),
             'rest_swagger_description': (
                     vst_project_module.__doc__ or vst_lib_module.__doc__ or ''
             ).replace('\n', '\\n').replace('\r', '\\r'),
-            'public_openapi': False,
             'openapi_cache_timeout': env.int(f'{ENV_NAME}_WEB_OPENAPI_CACHE_TIMEOUT', default=120),
             'enable_gravatar': env.bool(f'{ENV_NAME}_WEB_ENABLE_GRAVATAR', default=True),
             'request_max_size': env.int(f'{ENV_NAME}_WEB_REQUEST_MAX_SIZE', default=2621440),
             'x_frame_options': 'SAMEORIGIN',
             'use_x_forwarded_host': env.bool(f'{ENV_NAME}_WEB_USE_X_FORWARDED_HOST', default=False),
             'use_x_forwarded_port': env.bool(f'{ENV_NAME}_WEB_USE_X_FORWARDED_PORT', default=False),
             'password_reset_timeout_days': env.int(f'{ENV_NAME}_WEB_PASSWORD_RESET_TIMEOUT_DAYS', default=1),
@@ -544,14 +543,16 @@
         'throttle': {
             'rate': os.getenv(f'{ENV_NAME}_GLOBAL_THROTTLE_RATE', ''),
             'actions': ConfigListType(os.getenv(f'{ENV_NAME}_GLOBAL_THROTTLE_ACTIONS', ('update', 'partial_update'))),
             'views': {},
         },
         'uvicorn': {
             'loop': 'auto',
+            'limit_concurrency': 512,
+            'backlog': 512,
         }
     },
     section_overload={
         'main': MainSection,
         'web': WebSection,
         'databases': DatabasesSection,
         'database': DBSection,
@@ -1430,30 +1431,44 @@
     return 'django.core.files.storage.FileSystemStorage'  # nocv
 
 
 storages = config['storages']
 LIBCLOUD_PROVIDERS: _t.Dict[_t.Text, _t.Dict] = {}
 MEDIA_ROOT = storages['filesystem']['media_root']
 MEDIA_URL = storages['filesystem']['media_url']
+STORAGES = {
+    'filesystem': {
+        "BACKEND": "django.core.files.storage.FileSystemStorage",
+    },
+    "staticfiles": {
+        "BACKEND": "django.contrib.staticfiles.storage.StaticFilesStorage",
+    },
+}
 
 if 'libcloud' in storages:
 
     LIBCLOUD_PROVIDERS = {
         store_name: store_settings
         for store_name, store_settings in storages['libcloud'].all().items()
         if isinstance(store_settings, dict)
     }
 
     if LIBCLOUD_PROVIDERS and 'default' not in LIBCLOUD_PROVIDERS:
         DEFAULT_LIBCLOUD_PROVIDER = next(iter(LIBCLOUD_PROVIDERS))
 
+    STORAGES['libcloud'] = {"BACKEND": 'storages.backends.apache_libcloud.LibCloudStorage'}
+
 if 'boto3' in storages:
     globals().update( storages['boto3'].all())
+    STORAGES['libcloud'] = {"BACKEND": 'storages.backends.s3boto3.S3Boto3Storage'}
+
 
-DEFAULT_FILE_STORAGE = storages.get('default', fallback=get_default_storage_class())
+STORAGES['default'] = {
+    "BACKEND": get_default_storage_class()
+}
 
 DOCKERRUN_MIGRATE_LOCK_ID = config['docker'].get('migrate_lock_id', VST_PROJECT_LIB_NAME)
 
 DOCKERRUN_MIGRATE_LOCK_TIMEOUT = config['docker'].getint('migrate_lock_timeout', 15)
 
 # Test settings for speedup tests
 ##############################################################
@@ -1471,16 +1486,19 @@
     CELERY_CACHE_BACKEND = 'memory'
     CACHES = {
         name: {'BACKEND': 'django.core.cache.backends.locmem.LocMemCache'}
         for name in CACHES
     }
     BULK_THREADS = 10
     SEND_EMAIL_RETRIES = 10
-    DEFAULT_FILE_STORAGE = lazy(lambda: 'inmemorystorage.InMemoryStorage', str)()
+    for storage_name in filter('staticfiles'.__ne__, STORAGES):
+        STORAGES[storage_name] = {"BACKEND": 'django.core.files.storage.InMemoryStorage'}
     CENTRIFUGO_CLIENT_KWARGS = {}
+    __import__('pysqlite3')
+    sys.modules['sqlite3'] = sys.modules.pop('pysqlite3')
 
 
 if not TESTSERVER_RUN and TESTS_RUN:
     SESSION_ENGINE = 'django.contrib.sessions.backends.cache'
 
 # User settings
 ##############################################################
```

### Comparing `vstutils-5.4.9/vstutils/static/bundle/281.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/281.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/296.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/296.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/345.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/345.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/368.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/368.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/421.js` & `vstutils-5.5.0a1/vstutils/static/bundle/421.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/421.js.LICENSE.txt` & `vstutils-5.5.0a1/vstutils/static/bundle/421.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/618.js` & `vstutils-5.5.0a1/vstutils/static/bundle/618.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/683.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/683.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/686.js` & `vstutils-5.5.0a1/vstutils/static/bundle/686.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/742.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/742.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/742.chunk.js.LICENSE.txt` & `vstutils-5.5.0a1/vstutils/static/bundle/742.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/755.js` & `vstutils-5.5.0a1/vstutils/static/bundle/755.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/826.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/826.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/826.chunk.js.LICENSE.txt` & `vstutils-5.5.0a1/vstutils/static/bundle/826.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/844.js` & `vstutils-5.5.0a1/vstutils/static/bundle/844.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/959.js` & `vstutils-5.5.0a1/vstutils/static/bundle/959.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/959.js.LICENSE.txt` & `vstutils-5.5.0a1/vstutils/static/bundle/959.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/app_loader.js` & `vstutils-5.5.0a1/vstutils/static/bundle/app_loader.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/base.js` & `vstutils-5.5.0a1/vstutils/static/bundle/base.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/bb58e57c48a3e911f15f.woff` & `vstutils-5.5.0a1/vstutils/static/bundle/bb58e57c48a3e911f15f.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff` & `vstutils-5.5.0a1/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/output.json` & `vstutils-5.5.0a1/vstutils/static/bundle/output.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964192708333334%*

 * *Differences: {"'entrypoints'": "{'spa': {'assets': {0: {'size': 433009}}, 'assetsSize': 3679552}}"}*

```diff
@@ -26,15 +26,15 @@
             "filteredAuxiliaryAssets": 0,
             "name": "base"
         },
         "spa": {
             "assets": [
                 {
                     "name": "vstutils.js",
-                    "size": 432625
+                    "size": 433009
                 },
                 {
                     "name": "755.js",
                     "size": 89997
                 },
                 {
                     "name": "421.js",
@@ -57,15 +57,15 @@
                     "size": 1798980
                 },
                 {
                     "name": "spa.js",
                     "size": 3597
                 }
             ],
-            "assetsSize": 3679168,
+            "assetsSize": 3679552,
             "auxiliaryAssetsSize": 117924,
             "filteredAssets": 0,
             "filteredAuxiliaryAssets": 2,
             "name": "spa"
         }
     },
     "errors": []
```

### Comparing `vstutils-5.4.9/vstutils/static/bundle/spa.js` & `vstutils-5.5.0a1/vstutils/static/bundle/spa.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static/bundle/vstutils.js` & `vstutils-5.5.0a1/vstutils/static/bundle/vstutils.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3552,30 +3552,30 @@
                         if (!i) throw new Error("Cannot find queryset for model: ".concat(n));
                         e.nestedQueryset = i
                     }
                 }
                 _setParents(e) {
                     for (const [t, n] of e) {
                         const i = e.get(t.replace(/[^/]+\/$/, ""));
-                        i && (n.parent = i)
+                        i && (n.parent = i, i.hidden && (n.hidden = !0))
                     }
                 }
                 generateViews(e) {
                     const t = this.getViews(e);
                     if (!t.has("/")) {
                         const e = new u.G7({
                             path: "/",
                             routeName: "home"
                         }, null, [k]);
                         t.set("/", e)
                     }
                     if (!t.has("*")) {
                         const e = new u.G7({
                             path: "*",
-                            routeName: "404"
+                            routeName: a.NOT_FOUND_ROUTE_NAME
                         }, null, [T]);
                         e.showOperationButtons = !1, t.set("*", e)
                     }
                     return t
                 }
             }
         },
@@ -6527,15 +6527,15 @@
                     var e = this._self._c;
                     return this._self._setupProxy, e("span", {
                         staticClass: "input-group-text"
                     }, [e("i", {
                         staticClass: "fa-spin fas fa-sync-alt"
                     })])
                 }], !1, null, "3aacc6cb", null).exports,
-                V = n(29384),
+                V = n(32900),
                 M = (0, l.defineComponent)({
                     components: {
                         field_content_edit: E,
                         field_content_readonly: V.Z,
                         field_list_view: V.Z
                     },
                     mixins: [s.BaseFieldMixin]
@@ -9133,17 +9133,17 @@
 
             function cn(e, t) {
                 var n, i, s, a;
                 const r = null === (n = e.options.properties) || void 0 === n || null === (i = n.content) || void 0 === i ? void 0 : i.minLength,
                     o = null === (s = e.options.properties) || void 0 === s || null === (a = s.content) || void 0 === a ? void 0 : a.maxLength;
                 let l = !0;
                 if (void 0 !== r)
-                    for (const e of t) e.content.length < r && (an.guiPopUp.error(Mt(e.name)), l = !1);
+                    for (const e of t) e.content.length < r && (an.guiPopUp.error(It(e.name)), l = !1);
                 if (void 0 !== o)
-                    for (const e of t) e.content.length > o && (an.guiPopUp.error(It(e.name)), l = !1);
+                    for (const e of t) e.content.length > o && (an.guiPopUp.error(Mt(e.name)), l = !1);
                 return l
             }
 
             function pn(e, t) {
                 const n = e.options.minLength,
                     i = e.options.maxLength;
                 if (void 0 !== n || void 0 !== i) {
@@ -12062,15 +12062,15 @@
                         }
                     }
                 },
                 Ys = n(80306),
                 Ks = {};
             Ks.styleTagTransform = le(), Ks.setAttributes = se(), Ks.insert = ne().bind(null, "head"), Ks.domAPI = ee(), Ks.insertStyleElement = re(), J()(Ys.Z, Ks), Ys.Z && Ys.Z.locals && Ys.Z.locals;
             var Js = (0, L.Z)(Qs, Ws, [], !1, null, "6009ed91", null).exports,
-                Xs = n(29384),
+                Xs = n(32900),
                 ea = {
                     mixins: [A.BaseFieldMixin],
                     components: {
                         field_content_edit: Js,
                         field_content_readonly: Xs.Z,
                         field_list_view: Xs.Z
                     }
@@ -14600,19 +14600,20 @@
                                 }];
                                 for (const {
                                         view: n,
                                         path: i,
                                         state: s
                                     }
                                     of e.store.viewItems) {
+                                    if ((0, r.isNotFoundView)(n)) continue;
                                     let e = i,
                                         a = "",
-                                        r = n.getTitle(s);
-                                    n.isNewPage() ? (e = "", a = "fas fa-plus") : n.isEditPage() && !n.isEditStyleOnly && (e = "", a = "fas fa-pen", r = ""), t.push({
-                                        name: r,
+                                        o = n.getTitle(s);
+                                    n.isNewPage() ? (e = "", a = "fas fa-plus") : n.isEditPage() && !n.isEditStyleOnly && (e = "", a = "fas fa-pen", o = ""), t.push({
+                                        name: o,
                                         link: e,
                                         iconClasses: a
                                     })
                                 }
                                 return t.at(-1).link = "", t.length > 4 ? [...t.slice(0, 2), {
                                     name: "..."
                                 }, ...t.slice(-2)] : t
@@ -15595,14 +15596,17 @@
                 },
                 HttpMethods: function() {
                     return o
                 },
                 IGNORED_FILTERS: function() {
                     return a.le
                 },
+                NOT_FOUND_ROUTE_NAME: function() {
+                    return E
+                },
                 ObjectPropertyRetriever: function() {
                     return a.zr
                 },
                 RequestTypes: function() {
                     return x
                 },
                 SCHEMA_DATA_TYPE: function() {
@@ -15718,14 +15722,17 @@
                 },
                 isEmptyObject: function() {
                     return a.Qr
                 },
                 isInstancesEqual: function() {
                     return a.MU
                 },
+                isNotFoundView: function() {
+                    return V
+                },
                 isObject: function() {
                     return a.Kn
                 },
                 iterFind: function() {
                     return a.mF
                 },
                 joinPaths: function() {
@@ -15970,15 +15977,15 @@
 
             function T(e) {
                 const t = (0, s.M)().router;
                 if ("object" == typeof e) {
                     if (e.path && e.params) {
                         var n, a;
                         const i = t.resolve(e).route;
-                        !i.name || "404" === i.name || null !== (n = i.meta) && void 0 !== n && null !== (a = n.view) && void 0 !== a && a.isDeepNested || (e.name = i.name, delete e.path)
+                        !i.name || i.name === E || null !== (n = i.meta) && void 0 !== n && null !== (a = n.view) && void 0 !== a && a.isDeepNested || (e.name = i.name, delete e.path)
                     }
                 } else e = {
                     path: e
                 };
                 return t.push(e).catch((e => {
                     if (!i.ZP.isNavigationFailure(e)) throw e
                 }))
@@ -15990,14 +15997,19 @@
                     if (n.changed) try {
                         await n.save(), t = !0
                     } catch (t) {
                         return e.error_handler.defineErrorAndShow(t), !1
                     }
                 return t
             }
+            const E = "404";
+
+            function V(e) {
+                return e.routeName === E
+            }
         },
         8905: function(e, t, n) {
             n.d(t, {
                 B4: function() {
                     return v
                 },
                 Bv: function() {
@@ -16768,20 +16780,20 @@
         55392: function(e, t, n) {
             var i = n(8081),
                 s = n.n(i),
                 a = n(23645),
                 r = n.n(a)()(s());
             r.push([e.id, ".input-group[data-v-3aacc6cb] .select2-selection{width:100%}", ""]), t.Z = r
         },
-        29151: function(e, t, n) {
+        70779: function(e, t, n) {
             var i = n(8081),
                 s = n.n(i),
                 a = n(23645),
                 r = n.n(a)()(s());
-            r.push([e.id, ".object-link[data-v-784c8aee]{margin-top:5px;text-align:center}.field-component.type-list .loader[data-v-784c8aee]{text-align:center}", ""]), t.Z = r
+            r.push([e.id, ".object-link[data-v-ee46bd7e]{margin-top:5px;text-align:center}.field-component.type-list .loader[data-v-ee46bd7e]{text-align:center}", ""]), t.Z = r
         },
         92469: function(e, t, n) {
             var i = n(8081),
                 s = n.n(i),
                 a = n(23645),
                 r = n.n(a)()(s());
             r.push([e.id, ".json-field-readonly[data-v-e3f84444] .card{margin:10px 0}.json-field-readonly[data-v-e3f84444] .card-header{height:30px;padding:7px}.json-field-readonly[data-v-e3f84444] .card-title{font-size:1rem;line-height:1rem}.json-field-readonly[data-v-e3f84444] .btn-tool{margin:-0.45rem 0 0 0}.json-field-readonly[data-v-e3f84444] .card-body{padding:10px 0 0 20px}", ""]), t.Z = r
@@ -21114,18 +21126,18 @@
                 m = n(44589),
                 v = n.n(m),
                 g = n(92824),
                 _ = {};
             _.styleTagTransform = v(), _.setAttributes = p(), _.insert = d().bind(null, "head"), _.domAPI = l(), _.insertStyleElement = h(), r()(g.Z, _), g.Z && g.Z.locals && g.Z.locals;
             var b = (0, n(51900).Z)(s, i, [], !1, null, "2c165615", null).exports
         },
-        29384: function(e, t, n) {
+        32900: function(e, t, n) {
             n.d(t, {
                 Z: function() {
-                    return x
+                    return C
                 }
             });
             var i = function() {
                 var e = this,
                     t = e._self._c,
                     n = e._self._setupProxy;
                 return e.field.showLoader && n.loading ? t("div", {
@@ -21154,71 +21166,84 @@
                     }
                 }, [e._v("\n            " + e._s(n.text) + "\n        ")]) : t("span", [e._v(e._s(n.text))])]], 2)
             };
             i._withStripped = !0;
             var s = n(70538),
                 a = n(59802),
                 r = n(87444),
-                o = (0, s.defineComponent)({
+                o = n(59198),
+                l = (0, s.defineComponent)({
                     __name: "FKFieldContentReadonly",
                     props: r.FieldReadonlyPropsDef,
                     setup(e) {
                         const t = e,
+                            n = (0, o.getApp)(),
                             {
-                                queryset: n
+                                queryset: i
                             } = (0, a.e)(t.field, t.data),
-                            i = t.field.fkModel.fields.get(t.field.viewField),
-                            r = (0, s.computed)((() => null == i ? void 0 : i.fkLinkable)),
-                            o = (0, s.computed)((() => t.field.makeLink && (!t.value || !t.value.__notFound))),
-                            l = (0, s.computed)((() => t.field.getValueFieldValue(t.value))),
-                            u = (0, s.computed)((() => {
-                                if (l.value) {
+                            r = t.field.fkModel.fields.get(t.field.viewField),
+                            l = (0, s.computed)((() => null == r ? void 0 : r.fkLinkable)),
+                            u = (0, s.computed)((() => t.field.getValueFieldValue(t.value))),
+                            d = (0, s.computed)((() => {
+                                if (u.value) {
                                     var e;
                                     if (t.field.props.linkGenerator) return null !== (e = t.field.props.linkGenerator({
                                         ...t,
                                         value: t.value
                                     })) && void 0 !== e ? e : "";
-                                    if (n.value) return n.value.url + l.value
+                                    if (i.value) return i.value.url + u.value
                                 }
                                 return ""
                             })),
-                            d = (0, s.computed)((() => t.value ? t.field.translateValue(t.value) : "")),
+                            c = (0, s.computed)((() => {
+                                var e;
+                                if (!t.field.makeLink) return !1;
+                                if (!t.value || t.value.__notFound) return !1;
+                                const s = null === (e = i.value) || void 0 === e ? void 0 : e.pattern;
+                                if (s) {
+                                    const e = n.views.get(s);
+                                    if (!e || e.hidden) return !1
+                                }
+                                return !0
+                            })),
+                            p = (0, s.computed)((() => t.value ? t.field.translateValue(t.value) : "")),
                             {
-                                loading: c
+                                loading: f
                             } = (0, a.I)(t.field, (0, s.toRef)(t, "value"));
                         return {
                             __sfc: !0,
                             props: t,
-                            queryset: n,
-                            representField: i,
-                            linkable: r,
-                            withLink: o,
-                            fk: l,
-                            href: u,
-                            text: d,
-                            loading: c
+                            app: n,
+                            queryset: i,
+                            representField: r,
+                            linkable: l,
+                            fk: u,
+                            href: d,
+                            withLink: c,
+                            text: p,
+                            loading: f
                         }
                     }
                 }),
-                l = n(93379),
-                u = n.n(l),
-                d = n(7795),
-                c = n.n(d),
-                p = n(90569),
-                f = n.n(p),
-                h = n(3565),
-                m = n.n(h),
-                v = n(19216),
-                g = n.n(v),
-                _ = n(44589),
-                b = n.n(_),
-                y = n(29151),
-                w = {};
-            w.styleTagTransform = b(), w.setAttributes = m(), w.insert = f().bind(null, "head"), w.domAPI = c(), w.insertStyleElement = g(), u()(y.Z, w), y.Z && y.Z.locals && y.Z.locals;
-            var x = (0, n(51900).Z)(o, i, [], !1, null, "784c8aee", null).exports
+                u = n(93379),
+                d = n.n(u),
+                c = n(7795),
+                p = n.n(c),
+                f = n(90569),
+                h = n.n(f),
+                m = n(3565),
+                v = n.n(m),
+                g = n(19216),
+                _ = n.n(g),
+                b = n(44589),
+                y = n.n(b),
+                w = n(70779),
+                x = {};
+            x.styleTagTransform = y(), x.setAttributes = v(), x.insert = h().bind(null, "head"), x.domAPI = p(), x.insertStyleElement = _(), d()(w.Z, x), w.Z && w.Z.locals && w.Z.locals;
+            var C = (0, n(51900).Z)(l, i, [], !1, null, "ee46bd7e", null).exports
         },
         24389: function(e, t, n) {
             n.d(t, {
                 Z: function() {
                     return c
                 }
             });
```

### Comparing `vstutils-5.4.9/vstutils/static/img/anonymous.png` & `vstutils-5.5.0a1/vstutils/static/img/anonymous.png`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/static_files.py` & `vstutils-5.5.0a1/vstutils/static_files.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/tasks.py` & `vstutils-5.5.0a1/vstutils/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
             app.register_task(Foo())
 
     Now you can call your task with various methods:
         - by executing ``Foo.do(*args, **kwargs)``
         - get registered task instance like that - app.tasks['full_path.to.task.class.Foo']
 
-    Also you can make you registered task periodic, by adding it to CELERY_BEAT_SCHEDULE in settings.py:
+    Also you can make your registered task periodic, by adding it to CELERY_BEAT_SCHEDULE in settings.py:
 
         .. sourcecode:: python
 
             CELERY_BEAT_SCHEDULE = {
                 'foo-execute-every-month': {
                     'task': 'full_path.to.task.class.Foo',
                     'schedule': crontab(day_of_month=1),
```

### Comparing `vstutils-5.4.9/vstutils/templates/auth/base.html` & `vstutils-5.5.0a1/vstutils/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/auth/language_selector.html` & `vstutils-5.5.0a1/vstutils/templates/auth/language_selector.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/auth/tfa.html` & `vstutils-5.5.0a1/vstutils/templates/auth/tfa.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/base.html` & `vstutils-5.5.0a1/vstutils/templates/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/gui/base.html` & `vstutils-5.5.0a1/vstutils/templates/gui/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/gui/offline.html` & `vstutils-5.5.0a1/vstutils/templates/gui/offline.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/gui/service-worker.js` & `vstutils-5.5.0a1/vstutils/templates/gui/service-worker.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/newproject/.gitignore.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/.gitignore.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/newproject/frontend_src/.eslintrc.js.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/.eslintrc.js.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/newproject/package.json.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/package.json.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/newproject/project_name/settings.py.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/project_name/settings.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/newproject/setup.cfg.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/newproject/setup.py.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/setup.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/newproject/test.py.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/test.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/newproject/tox.ini.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/tox.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/newproject/tox_build.ini.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/tox_build.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/newproject/webpack.config.js.default.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/webpack.config.js.default.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/registration/confirm_email.html` & `vstutils-5.5.0a1/vstutils/templates/registration/confirm_email.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/registration/password_reset_confirm.html` & `vstutils-5.5.0a1/vstutils/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/registration/password_reset_form.html` & `vstutils-5.5.0a1/vstutils/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/registration/user_registration.html` & `vstutils-5.5.0a1/vstutils/templates/registration/user_registration.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/rest_framework/admin.html` & `vstutils-5.5.0a1/vstutils/templates/rest_framework/admin.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/vst_inclusion_tags/bootstrap_form.html` & `vstutils-5.5.0a1/vstutils/templates/vst_inclusion_tags/bootstrap_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templates/widgets/agreement_widget.html` & `vstutils-5.5.0a1/vstutils/templates/widgets/agreement_widget.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templatetags/request_static.py` & `vstutils-5.5.0a1/vstutils/templatetags/request_static.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templatetags/translation.py` & `vstutils-5.5.0a1/vstutils/templatetags/translation.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templatetags/vst_gravatar.py` & `vstutils-5.5.0a1/vstutils/templatetags/vst_gravatar.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templatetags/vst_html_tags.py` & `vstutils-5.5.0a1/vstutils/templatetags/vst_html_tags.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/templatetags/vstconfigs.py` & `vstutils-5.5.0a1/vstutils/templatetags/vstconfigs.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/tests.py` & `vstutils-5.5.0a1/vstutils/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pylint: disable=unused-import
 import typing as _t
 import random  # noqa: F401
 import string  # noqa: F401
 import os  # noqa: F401
 import uuid
+import warnings
 from unittest.mock import patch, Mock
 import json  # noqa: F401
 
 import ormsgpack
 from django.apps import apps
 from django.http import StreamingHttpResponse
 from django.db import transaction, models as django_models
@@ -24,15 +25,15 @@
 
 BulkDataType = _t.Union[_t.List[_t.Dict[_t.Text, _t.Any]], str, bytes, bytearray]
 ApiResultType = _t.Union[BulkDataType, _t.Dict, _t.Sequence[BulkDataType]]
 
 
 class BaseTestCase(TestCase):
     """
-    Main testcase class extends :class:`django.test.TestCase`.
+    Main test case class extends :class:`django.test.TestCase`.
     """
     server_name = 'vstutilstestserver'
 
     #: Attribute with default project models module.
     models = None
 
     #: Default http status codes for different http methods. Uses in :meth:`.get_result`
@@ -205,15 +206,15 @@
         """
         return patch.object(model._meta.get_field(field_name), 'get_default', new=lambda: value)
 
     def get_model_class(self, model) -> django_models.Model:
         """
         Getting model class by string or return model arg.
 
-        :param model: string which contains model name (if attribute ``model`` is set to the testcase class),
+        :param model: string which contains model name (if attribute ``model`` is set to the test case class),
                       module import, ``app.ModelName`` or :class:`django.db.models.Model`.
         :type model: str,django.db.models.Model
         :return: Model class.
         :rtype: django.db.models.Model
 
         """
 
@@ -234,28 +235,28 @@
         return model
 
     def get_model_filter(self, model, **kwargs):
         """
         Simple wrapper over :meth:`.get_model_class` which returns filtered
         queryset from model.
 
-        :param model: string which contains model name (if attribute ``model`` is set to the testcase class),
+        :param model: string which contains model name (if attribute ``model`` is set to the test case class),
                       module import, ``app.ModelName`` or :class:`django.db.models.Model`.
         :type model: str,django.db.models.Model
         :param kwargs: named arguments to :meth:`django.db.models.query.QuerySet.filter`.
         :rtype: django.db.models.query.QuerySet
 
         """
         return self.get_model_class(model).objects.filter(**kwargs)
 
     def get_count(self, model, **kwargs):
         """
         Simple wrapper over :meth:`.get_model_filter` which returns counter of items.
 
-        :param model: string which contains model name (if attribute ``model`` is set to the testcase class),
+        :param model: string which contains model name (if attribute ``model`` is set to the test case class),
                       module import, ``app.ModelName`` or :class:`django.db.models.Model`.
         :type model: str,django.db.models.Model
         :param kwargs: named arguments to :meth:`django.db.models.query.QuerySet.filter`.
         :return: number of instances in database.
         :rtype: int
         """
         return self.get_model_filter(model, **kwargs).count()
@@ -273,15 +274,15 @@
         response = request(url, secure=True, *args, **kwargs)
         self.last_response = response
         self.assertRCode(response, code, url)
         return self.render_api_response(response)
 
     def assertCount(self, iterable: _t.Sized, count: int, msg: _t.Any = None):
         """
-        Call :func:`len` over ``iterable`` and check equals with ``count``.
+        Calls :func:`len` over ``iterable`` and checks equality with ``count``.
 
         :param iterable: any iterable object which could be sended to :func:`len`.
         :param count: expected result.
         :param msg: error message
 
         """
         self.assertEqual(len(iterable), count, msg)
@@ -316,15 +317,15 @@
             )
 
     def post_result(self, url, code=None, *args, **kwargs):
         return self.get_result("post", url, code, *args, **kwargs)
 
     def get_result(self, rtype, url, code: int = None, *args, **kwargs) -> ApiResultType:
         """
-        Execute and test response code on request with returning parsed result of request.
+        Executes and tests response code on request with returning parsed result of request.
         The method uses the following procedure:
 
         - Test client authorization (with :attr:`.user` which creates in :meth:`.setUp`).
         - Executing a request (sending args and kwargs to request method).
         - Parsing the result (converts json string to python-object).
         - Checking the http status code with :meth:`.assertRCode`
           (if you have not specified it,
@@ -401,15 +402,15 @@
         result = self.get_result("get", url)
         self.assertTrue(isinstance(result, dict))
         for key, value in kwargs.items():
             self.assertEqual(result[key], value)
 
     def endpoint_call(self, data: BulkDataType = None, method: str = 'get', code: int = 200, **kwargs) -> ApiResultType:
         """
-        Make request to endpoint and assert response status code if specified (default is 200).
+        Makes request to endpoint and asserts response status code if specified (default is 200).
         Uses :meth:`.get_result` method for execution.
 
         :param data: request data
         :param method: http request method
         :param code: http status to assert
         :param query: dict with query data (working only with `get`)
         :return: bulk response
@@ -422,34 +423,43 @@
                 data = json.dumps(data)
 
         if method == 'get' and 'query' in kwargs and kwargs['query']:
             query = f'?{"&".join(map("=".join, kwargs.pop("query").items()))}'
         else:
             query = ''
 
+        headers = kwargs.pop('headers', {})
+        headers['accept-encoding'] = 'gzip'
+        oldstyle_headers = set(filter(lambda x: x.startswith('HTTP_'), kwargs.keys()))
+
+        if oldstyle_headers:
+            warnings.warn("You should setup 'headers' instead of kwargs", DeprecationWarning)  # nocv
+
+        for key in oldstyle_headers:
+            headers.setdefault(key[5:].replace('_', '-').lower(), kwargs[key])  # nocv
+
         return self.get_result(
             method,
             f'/{self._settings("VST_API_URL")}/endpoint/{query}',
             data=data,
             code=code,
-            HTTP_ACCEPT_ENCODING='gzip',
             **kwargs
         )
 
     def endpoint_schema(self, **kwargs):
         """
         Make request to schema. Returns dict with swagger data.
 
         :param version: API version for schema parser.
         """
         return self.endpoint_call(query={**kwargs, 'format': 'openapi'})
 
     def bulk(self, data: BulkDataType, code: int = 200, **kwargs) -> ApiResultType:
         """
-        Make non transactional bulk request and assert status code (default is 200)
+        Makes non-transactional bulk request and asserts status code (default is 200)
 
         :param data: request data
         :param code: http status to assert
         :param kwargs: named arguments for :meth:`.get_result`
         :return: bulk response
         """
         return self.endpoint_call(data, method='put', code=code, **kwargs)
```

### Comparing `vstutils-5.4.9/vstutils/tools.py` & `vstutils-5.5.0a1/vstutils/tools.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/translations/cn.py` & `vstutils-5.5.0a1/vstutils/translations/cn.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/translations/ru.py` & `vstutils-5.5.0a1/vstutils/translations/ru.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/translations/vi.py` & `vstutils-5.5.0a1/vstutils/translations/vi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils/urls.py` & `vstutils-5.5.0a1/vstutils/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from rest_framework import permissions
 
 from .api.routers import MainRouter
 from .utils import URLHandlers
 from .api.views import HealthView, MetricsView
 
 static_serve = functools.partial(serve_static, insecure=True)
+gui_enabled = not getattr(settings, 'API_ONLY', False)
 
 
 def get_valid_url(*args):
     return os.path.join('/', *map(lambda x: x.lstrip('^/'), filter(bool, args + ('/',))))
 
 
 class AdminLoginLogoutRedirectView(RedirectView):
@@ -34,23 +35,24 @@
     router.register_view('metrics', MetricsView.as_view({'get': 'list'}), 'metrics')
 
 
 admin.site.site_header = 'Admin panel'
 admin.site.site_title = settings.VST_PROJECT
 admin.site.index_title = f"{settings.VST_PROJECT.upper()} Settings Panel"
 admin.site.site_url = "/"
+# TODO: make it depends on 'gui_enabled' when auth migrate to API
 admin.site.login = AdminLoginLogoutRedirectView.as_view(  # type: ignore
     url=get_valid_url(settings.ACCOUNT_URL, settings.LOGIN_URL)
 )
 admin.site.logout = AdminLoginLogoutRedirectView.as_view(  # type: ignore
     url=get_valid_url(settings.ACCOUNT_URL, settings.LOGOUT_URL)
 )
 doc_url = getattr(settings, 'DOC_URL', '/docs/')[1:]
 
-urlpatterns = list(URLHandlers())
+urlpatterns = list(URLHandlers()) if gui_enabled else []
 
 urlpatterns += [
     path(settings.ACCOUNT_URL, include(list(URLHandlers('ACCOUNT_URLS'))))
 ]
 
 urlpatterns += [
     path('admin/', admin.site.urls),
```

### Comparing `vstutils-5.4.9/vstutils/utils.py` & `vstutils-5.5.0a1/vstutils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import codecs
 import io
 import logging
 import os
 import pickle
 import random
 import subprocess
+import asyncio
 import sys
 import tempfile
 import time
 import json
 import traceback
 import types
 import typing as tp
 import uuid
 import warnings
 from functools import lru_cache, wraps
 from pathlib import Path
-from threading import Thread
 from enum import Enum, EnumMeta
 
+from asgiref.sync import sync_to_async
 from django.conf import settings
 from django.middleware.gzip import GZipMiddleware
 from django.urls import re_path, path, include
 from django.core.mail import get_connection, EmailMultiAlternatives
 from django.core.cache import caches, InvalidCacheBackendError
 from django.core.paginator import Paginator as BasePaginator
 from django.template import loader
@@ -40,17 +41,21 @@
 
 logger: logging.Logger = logging.getLogger('vstutils')
 ON_POSIX = 'posix' in sys.builtin_module_names
 _gzip_object = GZipMiddleware(lambda *args, **kwargs: None)  # type: ignore
 
 
 def deprecated(func: tp.Callable):
-    """This is a decorator which can be used to mark functions
+    """
+    This is a decorator which can be used to mark functions
     as deprecated. It will result in a warning being emitted
-    when the function is used."""
+    when the function is used.
+
+    :param func: any callable that will be wrapped and will issue a deprecation warning when called.
+    """
 
     def new_func(*args, **kwargs):
         warnings.warn(f'Call to deprecated function {func.__name__}.',
                       category=DeprecationWarning,
                       stacklevel=2)
         return func(*args, **kwargs)
 
@@ -111,15 +116,15 @@
 
 def encode(key, clear):
     """
     Encode string by Vigenère cipher.
 
     :param key: -- secret key for encoding
     :type key: str
-    :param clear: -- clear value  for encoding
+    :param clear: -- clear value for encoding
     :type clear: str
     :return: -- encoded string
     :rtype: str
     """
     # pylint: disable=consider-using-enumerate
 
     enc = []
@@ -227,15 +232,14 @@
         **kwargs
     )
 
 
 def send_template_email(sync: bool = False, **kwargs):
     """
     Function executing sync or async email sending; according `sync` argument and settings variable "RPC_ENABLED".
-    You can use this function to send message, it sends message asynchronously or synchronously.
     If you don't set settings for celery or don't have celery it sends synchronously mail.
     If celery is installed and configured and `sync` argument of the function is set to `False`,
     it sends asynchronously email.
 
     :param sync: argument for determining how send email, asynchronously or synchronously
     :param subject: mail subject.
     :param email: list of strings or single string, with email addresses of recipients
@@ -418,24 +422,27 @@
                 @classproperty
                 def value(cls):
                     return cls.some_value
 
                 @value.setter
                 def value(cls, new_value):
                     cls.some_value = new_value
+
+    :param fget: function for getting an attribute value.
+    :param fset: function for setting an attribute value.
     """
 
 
 class redirect_stdany:
     """
     Context for redirect any output to own stream.
 
     .. note::
-        - On context return stream object.
-        - On exit return old streams
+        - On context returns stream object.
+        - On exit returns old streams.
     """
     __slots__ = ('stream', 'streams', '_old_streams')
 
     _streams: tp.ClassVar[tp.List[tp.Text]] = ["stdout", "stderr"]
 
     def __init__(self, new_stream=io.StringIO(), streams=None):
         """
@@ -479,15 +486,15 @@
 
     **Attributes**:
 
     :param data: -- string to write in tmp file.
     :type data: str
     :param mode: -- file open mode. Default 'w'.
     :type mode: str
-    :param bufsize: -- bufer size for tempfile.NamedTemporaryFile
+    :param bufsize: -- buffer size for tempfile.NamedTemporaryFile
     :type bufsize: int
     :param kwargs:  -- other kwargs for tempfile.NamedTemporaryFile
 
     """
     __slots__ = ('fd', 'path')
 
     def __init__(self, data: tp.Text = "", mode: tp.Text = "w", bufsize: int = -1, **kwargs):
@@ -745,128 +752,181 @@
         return self._encode(codecs.encode(pickle.dumps(value), "base64").decode())
 
 
 class Executor(BaseVstObject):
     """
     Command executor with realtime output write and line handling.
     By default and by design executor initialize string attribute ``output``
-    which will be modifyed by ``+=`` operator with new lines by :meth:`.Executor.write_output`
+    which will be modified by ``+=`` operator with new lines by :meth:`.Executor.write_output`
     procedure. Override the method if you want change behavior.
 
     Executor class supports periodically (0.01 sec) handling process and execute some checks
     by overriding :meth:`.Executor.working_handler` procedure method. If you want disable this behavior
     override the method by None value or use :class:`.UnhandledExecutor`.
     """
     __slots__ = ('output', '__stdout__', '__stderr__', 'env')
 
     CANCEL_PREFIX: tp.ClassVar[tp.Text] = "CANCEL_EXECUTE_"
-    newlines: tp.ClassVar[tp.List[tp.Text]] = ['\n', '\r\n', '\r']
     STDOUT: tp.ClassVar[int] = subprocess.PIPE
     STDERR: tp.ClassVar[int] = subprocess.STDOUT
     DEVNULL: tp.ClassVar[int] = subprocess.DEVNULL
     CalledProcessError: tp.ClassVar[tp.Type[subprocess.CalledProcessError]] = subprocess.CalledProcessError
+    env: tp.Dict[str, str]
 
-    env: tp.Dict[tp.Text, tp.Text]
-
-    def __init__(self, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, **environ_variables):
-        """
-        :type stdout: BinaryIO,int
-        :type stderr: BinaryIO,int
-        """
+    def __init__(
+            self,
+            stdout: tp.Union[tp.BinaryIO, int] = subprocess.PIPE,
+            stderr: tp.Union[tp.BinaryIO, int] = subprocess.STDOUT,
+            **environ_variables: str,
+    ):
         self.output = ''
         self.__stdout__ = stdout
         self.__stderr__ = stderr
         self.env = environ_variables
 
     def write_output(self, line: tp.Text) -> None:
         """
         :param line: -- line from command output
         :type line: str
         :return: None
         :rtype: None
         """
         self.output += str(line)
 
-    def _handle_process(self, proc: subprocess.Popen, stream: tp.Text):
-        stream_object = getattr(proc, stream)
-        while not stream_object.closed:
-            self.working_handler(proc)
-            time.sleep(0.01)
-
-    def working_handler(self, proc: subprocess.Popen) -> None:
+    async def working_handler(self, proc: asyncio.subprocess.Process):
         # pylint: disable=unused-argument
         """
         Additional handler for executions.
 
-        :type proc: subprocess.Popen
+        :arg proc: running process
+        :type proc: asyncio.subprocess.Process
         """
 
-    def _unbuffered(self, proc: subprocess.Popen, stream: tp.Text = 'stdout'):
-        """
-        Unbuffered output handler.
+    async def line_handler(self, line: tp.Text) -> None:
+        write_output = self.write_output
+        if not asyncio.iscoroutinefunction(write_output):
+            write_output = sync_to_async(write_output, thread_sensitive=True)
+        if line is not None:  # pragma: no branch
+            with raise_context():
+                await write_output(line)
 
-        :type proc: subprocess.Popen
-        :type stream: str
-        :return:
-        """
+    async def _handle_process(self, proc: asyncio.subprocess.Process, stream: tp.Text = 'stdout'):
+        stream_object: asyncio.StreamReader = getattr(proc, stream)
+        working_handler = self.working_handler
+        if not asyncio.iscoroutinefunction(working_handler):
+            working_handler = sync_to_async(working_handler, thread_sensitive=True)  # nocv
+
+        # Run handler periodically until stream object is closed
+        while not stream_object.at_eof():
+            await working_handler(proc)
+            await asyncio.sleep(0.01)
+
+    async def _unbuffered_read(self, proc: asyncio.subprocess.Process, stream: tp.Text = 'stdout'):
+        async for line in getattr(proc, stream):
+            await self.line_handler(line.decode('utf-8'))
+
+    async def _run_subprocess(self, cmd, cwd, env_vars=None):
+        # Run pre execution hook.
+        await self.pre_execute(
+            cmd=cmd,
+            cwd=cwd,
+            env=env_vars,
+        )
+        # Cleanup output variable
+        self.output = ""
+        # Setup environment variables
+        env = os.environ.copy()
+        env.update(self.env)
+        if env_vars:
+            env.update(env_vars)
+
+        # Start execution process
+        proc = await asyncio.create_subprocess_exec(
+            *cmd,
+            stdout=self.__stdout__,
+            stderr=self.__stderr__,
+            env=env,
+            cwd=str(cwd),
+            bufsize=0,
+            close_fds=ON_POSIX,
+        )
+
+        # Setup process output handlers
+        # and wait until it ends
+        tasks = [self._unbuffered_read(proc)]
         if self.working_handler is not None:
-            t = Thread(target=self._handle_process, args=(proc, stream))
-            t.start()
-        out = getattr(proc, stream)
+            tasks.append(self._handle_process(proc))
+        await asyncio.gather(*tasks)
+
+        # Parse return code and handle post execution hook
+        return_code = proc.returncode
         try:
-            retcode = None
-            while retcode is None:
-                for line in iter(out.readline, ""):
-                    yield line.rstrip()
-                retcode = proc.poll()
+            if return_code:
+                logger.error(self.output)
+                raise self.CalledProcessError(
+                    return_code, cmd, output=str(self.output)
+                )
         finally:
-            out.close()
+            await self.post_execute(
+                cmd=cmd,
+                cwd=cwd,
+                env=env_vars,
+                return_code=return_code,
+            )
 
-    def line_handler(self, line: tp.Text) -> None:
-        if line is not None:  # pragma: no branch
-            with raise_context():
-                self.write_output(line)
+    async def pre_execute(self, cmd: tp.Iterable[tp.Text], cwd: tp.Union[tp.Text, Path], env: dict):
+        """
+        Runs before execution starts.
 
-    def execute(self, cmd: tp.List[tp.Text], cwd: tp.Union[tp.Text, Path]) -> tp.Text:
+        :param cmd: -- list of cmd command and arguments
+        :param cwd: -- workdir for executions
+        :param env: -- extra environment variables which overrides defaults
+        """
+
+    async def post_execute(self, cmd: tp.Iterable[tp.Text], cwd: tp.Union[tp.Text, Path], env: dict, return_code: int):
+        """
+        Runs after execution end.
+
+        :param cmd: -- list of cmd command and arguments
+        :param cwd: -- workdir for executions
+        :param env: -- extra environment variables which overrides defaults
+        :param return_code: -- return code of executed process
         """
-        Execute commands and output this.
+
+    async def aexecute(self, cmd: tp.Iterable[tp.Text], cwd: tp.Union[tp.Text, Path], env: dict = None) -> tp.Text:
+        """
+        Executes commands and outputs its result. Asynchronous implementation.
 
         :param cmd: -- list of cmd command and arguments
-        :type cmd: list
         :param cwd: -- workdir for executions
-        :type cwd: str
+        :param env: -- extra environment variables which overrides defaults
         :return: -- string with full output
-        :rtype: str
         """
-        self.output = ""
-        env = os.environ.copy()
-        env.update(self.env)
-        with subprocess.Popen(
-            cmd, stdout=self.__stdout__, stderr=self.__stderr__,
-            bufsize=0, universal_newlines=True,
-            cwd=str(cwd), env=env,
-            close_fds=ON_POSIX
-        ) as proc:
-            for line in self._unbuffered(proc):
-                self.line_handler(line)
-            return_code = proc.poll()
-            if return_code:
-                logger.error(self.output)
-                raise subprocess.CalledProcessError(
-                    return_code, cmd, output=str(self.output)
-                )
+        await self._run_subprocess(cmd, cwd, env)
+        return self.output
+
+    def execute(self, cmd: tp.Iterable[tp.Text], cwd: tp.Union[tp.Text, Path], env: dict = None) -> tp.Text:
+        """
+        Executes commands and outputs its result.
+
+        :param cmd: -- list of cmd command and arguments
+        :param cwd: -- workdir for executions
+        :param env: -- extra environment variables which overrides defaults
+        :return: -- string with full output
+        """
+        asyncio.run(self.aexecute(cmd, cwd, env))
         return self.output
 
 
 class UnhandledExecutor(Executor):
     """
     Class based on :class:`.Executor` but disables `working_handler`.
     """
     __slots__ = ()
-    working_handler = None  # type: ignore
+    working_handler = None
 
 
 class KVExchanger(BaseVstObject):
     """
     Class for transmit data using key-value fast (cache-like) storage between
     services. Uses same cache-backend as Lock.
     """
@@ -957,15 +1017,15 @@
     """
     __slots__ = ('id', 'payload_data')
     TIMEOUT: tp.ClassVar[int] = 60 * 60 * 24
     GLOBAL: tp.ClassVar[tp.Text] = "global-deploy"
     SCHEDULER: tp.ClassVar[tp.Text] = "celery-beat"
 
     class AcquireLockException(Exception):
-        """ Exception which will raised on unreleased lock. """
+        """ Exception which will be raised on unreleased lock. """
 
     @classproperty
     def PREFIX(cls):
         # pylint: disable=no-self-argument
         return f"{cls.get_django_settings('VST_PROJECT_LIB')}_lock_"
 
     def __init__(self, id, payload=1, repeat=1, err_msg="", timeout=None):
@@ -1098,26 +1158,25 @@
             # Get class handler for 'one'
             one_backend_class = handlers['one']
             # Get object of backend 'two'
             two_obj = handlers.get_object()
             # Get object of backend 'two' with overriding constructor named arg
             two_obj_overrided = handlers.get_object(some_named_arg='another_value')
 
+    :param type_name: type name for backends.Like name in dict.
+    :type type_name: str
+
     """
 
     __slots__ = ('type', 'err_message', '__list__', '__loaded_backends__')
 
     type: tp.Text
     err_message: tp.Optional[tp.Text]
 
     def __init__(self, type_name: tp.Text, err_message: tp.Optional[tp.Text] = None):
-        """
-        :param type_name: -- type name for backends.Like name in dict.
-        :type type_name: str
-        """
         self.type = type_name
         self.err_message = err_message
         self.__list__: tp.Optional[tp.Dict[tp.Text, tp.Any]] = None
         self.__loaded_backends__: tp.Dict[tp.Text, tp.Any] = {}
 
     @property
     def objects(self):
@@ -1216,14 +1275,15 @@
 
     :param objects: -- dict of objects like: ``{<name>: <backend_class>}``
     :type objects: dict
     :param keys: -- names of supported backends
     :type keys: list
     :param values: -- supported backends classes
     :type values: list
+    :param type_name: type name for backends.Like name in dict.
     """
 
     __slots__ = ()
 
     def get_object(self, name: tp.Text, obj) -> tp.Any:  # type: ignore
         """
         :param name: -- string name of backend
@@ -1245,14 +1305,15 @@
         .. sourcecode:: python
 
             from vstutils.utils import URLHandlers
 
 
             # By default gets from `GUI_VIEWS` in `settings.py`
             urlpatterns = list(URLHandlers())
+    :param type_name: type name for backends.Like name in dict.
     """
     __slots__ = ('additional_handlers', '__handlers__', 'default_namespace')
 
     settings_urls: tp.ClassVar[tp.List[tp.Text]] = [
         'LOGIN_URL',
         'LOGOUT_URL'
     ]
@@ -1264,18 +1325,14 @@
         self.__handlers__ = None
         super().__init__(type_name, *args, **kwargs)
 
     @property
     def view_handlers(self):
         if not self.__handlers__:
             self.__handlers__ = tuple(map(self.__class__, self.additional_handlers))
-            # self.__handlers__ = []
-            # handler_class = self.__class__
-            # for handler_settings_name in self.additional_handlers:
-            #     self.__handlers__.append(handler_class(handler_settings_name))
         return self.__handlers__
 
     def get_backend_data(self, name: tp.Text):
         data = super().get_backend_data(name)
         if isinstance(data, str):
             for handler in self.view_handlers:
                 try:
@@ -1287,16 +1344,16 @@
 
     def get_object(self, name: tp.Text, *argv, **kwargs):
         """
         Get url object tuple for urls.py
 
         :param name: url regexp from
         :type name: str
-        :param argv: overrided args
-        :param kwargs: overrided kwargs
+        :param argv: overridden args
+        :param kwargs: overridden kwargs
         :return: url object
         :rtype: django.urls.re_path
         """
         regexp = name
         options = self.opts(regexp)
         options.update(kwargs)
         args = options.pop('view_args', argv)
@@ -1350,15 +1407,18 @@
             elif value is metacls.UPPER:
                 dict.__setitem__(classdict, key, key.upper())
                 mutated_types[key] = str.upper
             elif value is metacls.SAME:
                 dict.__setitem__(classdict, key, key)
                 mutated_types[key] = str
         classdict['__mutated_types__'] = mutated_types
-        return super().__new__(metacls, cls, bases, classdict)
+        result = super().__new__(metacls, cls, bases, classdict)
+        if result.__members__:
+            result.max_len = max(len(i) for i in result.__members__)
+        return result
 
 
 class VstEnum(Enum, metaclass=VstEnumMeta):
     pass
 
 
 class BaseEnum(str, VstEnum):
@@ -1375,15 +1435,15 @@
             class ItemCLasses(BaseEnum):
                 FIRST = BaseEnum.SAME
                 SECOND = BaseEnum.SAME
                 THIRD = BaseEnum.SAME
 
 
             class MyDjangoModel(BModel):
-                item_class = models.CharField(max_length=1024, choices=ItemCLasses.to_choices())
+                item_class = models.CharField(max_length=ItemCLasses.max_len, choices=ItemCLasses.to_choices())
 
                 @property
                 def is_second(self):
                     # Function check is item has second class of instance
                     return ItemCLasses.SECOND.is_equal(self.item_class)
 
     .. note::
```

### Comparing `vstutils-5.4.9/vstutils/wsgi.py` & `vstutils-5.5.0a1/vstutils/wsgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils.egg-info/PKG-INFO` & `vstutils-5.5.0a1/vstutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.4.9
+Version: 5.5.0a1
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
 Project-URL: Releases, https://pypi.org/project/vstutils/#history
 Project-URL: Documentation, https://vstutils.vstconsulting.net/
 Keywords: web,app,spa,vue,pwa,framework,openapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -40,15 +40,14 @@
 Provides-Extra: ldap
 Provides-Extra: doc
 Provides-Extra: prod
 Provides-Extra: stubs
 Provides-Extra: pil
 Provides-Extra: boto3
 Provides-Extra: sqs
-Provides-Extra: librabbitmq
 Provides-Extra: all
 License-File: LICENSE
 License-File: NOTICE
 
 VSTUtils Framework
 ==================
```

### Comparing `vstutils-5.4.9/vstutils.egg-info/SOURCES.txt` & `vstutils-5.5.0a1/vstutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.9/vstutils.egg-info/requires.txt` & `vstutils-5.5.0a1/vstutils.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-django~=4.1.7
+django~=4.2.2
 configparser~=5.3.0
 configparserc~=1.4.0
 Markdown==3.4.1
 django-environ~=0.10.0
 djangorestframework~=3.14.0
-drf-yasg==1.21.5
+drf-yasg==1.21.6
 MarkupSafe==2.0.1
 django-filter==23.2
 django-crispy-forms~=1.14.0
 drf_orjson_renderer~=1.7.1
 ormsgpack==1.2.6
 uvicorn~=0.22.0
 pyuwsgi==2.0.21
-fastapi~=0.95.1
+fastapi==0.97.0
 cent~=4.1.0
 PyJWT~=2.7.0
 jsmin~=3.0.1
 django-htmlmin~=0.11.0
 pyotp~=2.8.0
 django-storages[libcloud]==1.13.2
 sphinx~=5.3.0
@@ -24,21 +24,20 @@
 sphinxcontrib-httpdomain~=1.8.0
 sphinxcontrib-websupport~=1.2.4
 sphinxcontrib-mermaid~=0.7.1
 sphinx-autodoc-typehints~=1.23.0
 sphinx-rtd-theme~=1.2.1
 
 [all]
-coverage~=7.2.3
+coverage~=7.2.7
 fakeldap==0.6.1
 tblib~=1.7.0
 beautifulsoup4~=4.12.2
-dj-inmemorystorage~=2.1.0
-httpx~=0.24.0
-celery[redis]==5.2.7
+httpx~=0.24.1
+celery[redis]==5.3.0
 django-celery-beat~=2.5.0
 python-ldap==3.4.0
 sphinx~=5.3.0
 sphinx-autobuild~=2021.3.14
 sphinxcontrib-httpdomain~=1.8.0
 sphinxcontrib-websupport~=1.2.4
 sphinxcontrib-mermaid~=0.7.1
@@ -59,42 +58,38 @@
 sphinxcontrib-mermaid~=0.7.1
 sphinx-autodoc-typehints~=1.23.0
 sphinx-rtd-theme~=1.2.1
 
 [ldap]
 python-ldap==3.4.0
 
-[librabbitmq]
-celery[librabbitmq,redis]==5.2.7
-django-celery-beat~=2.5.0
-
 [pil]
 Pillow~=9.4.0
 
 [prod]
 redis[hiredis]~=4.5.5
 
 [rpc]
-celery[redis]==5.2.7
+celery[redis]==5.3.0
 django-celery-beat~=2.5.0
 
 [sqs]
-celery[redis,sqs]==5.2.7
+celery[redis]==5.3.0
 django-celery-beat~=2.5.0
+pycurl~=7.45.2
 
 [stubs]
-django-stubs[compatible-mypy]~=1.16.0
-djangorestframework-stubs[compatible-mypy]~=1.10.0
+django-stubs[compatible-mypy]~=4.2.1
+djangorestframework-stubs[compatible-mypy]~=3.14.1
 celery-stubs~=0.1.3
 drf-yasg-stubs~=0.1.3
 django-filter-stubs~=0.1.2
 types-PyMySQL~=1.0.19.6
 types-Markdown~=3.4.2.6
 types-docutils~=0.19.1.7
 
 [test]
-coverage~=7.2.3
+coverage~=7.2.7
 fakeldap==0.6.1
 tblib~=1.7.0
 beautifulsoup4~=4.12.2
-dj-inmemorystorage~=2.1.0
-httpx~=0.24.0
+httpx~=0.24.1
```

