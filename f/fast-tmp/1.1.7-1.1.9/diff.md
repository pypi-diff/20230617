# Comparing `tmp/fast_tmp-1.1.7.tar.gz` & `tmp/fast_tmp-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_tmp-1.1.7.tar", max compression
+gzip compressed data, was "fast_tmp-1.1.9.tar", max compression
```

## Comparing `fast_tmp-1.1.7.tar` & `fast_tmp-1.1.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0    11357 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/LICENSE
--rw-r--r--   0        0        0     3101 2022-10-18 03:29:07.000000 fast_tmp-1.1.7/README.md
--rw-r--r--   0        0        0        0 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/__init__.py
--rw-r--r--   0        0        0        0 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/admin/__init__.py
--rw-r--r--   0        0        0     1051 2022-10-12 10:00:24.000000 fast_tmp-1.1.7/fast_tmp/admin/depends.py
--rw-r--r--   0        0        0     4933 2023-01-31 04:59:54.802217 fast_tmp-1.1.7/fast_tmp/admin/endpoint.py
--rw-r--r--   0        0        0      848 2022-09-29 08:13:27.000000 fast_tmp-1.1.7/fast_tmp/admin/exception_handlers.py
--rw-r--r--   0        0        0      645 2022-10-13 02:18:55.000000 fast_tmp-1.1.7/fast_tmp/admin/register.py
--rw-r--r--   0        0        0     5595 2023-01-31 04:59:54.858218 fast_tmp-1.1.7/fast_tmp/admin/server.py
--rw-r--r--   0        0        0     1989 2023-01-31 04:59:54.738216 fast_tmp-1.1.7/fast_tmp/admin/site.py
--rw-r--r--   0        0        0        0 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/admin/template.py
--rw-r--r--   0        0        0     1086 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/admin/templates/base.html
--rw-r--r--   0        0        0     7437 2022-11-11 02:06:15.000000 fast_tmp-1.1.7/fast_tmp/admin/templates/index.html
--rw-r--r--   0        0        0     3516 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/admin/templates/login.html
--rw-r--r--   0        0        0        0 2022-12-01 07:00:20.000000 fast_tmp-1.1.7/fast_tmp/amis/__init__.py
--rw-r--r--   0        0        0     1437 2022-11-11 02:03:40.000000 fast_tmp-1.1.7/fast_tmp/amis/actions.py
--rw-r--r--   0        0        0      810 2022-11-11 02:03:40.000000 fast_tmp-1.1.7/fast_tmp/amis/base.py
--rw-r--r--   0        0        0     1576 2023-01-31 04:51:01.424473 fast_tmp-1.1.7/fast_tmp/amis/column.py
--rw-r--r--   0        0        0      670 2022-11-11 02:03:40.000000 fast_tmp-1.1.7/fast_tmp/amis/crud.py
--rw-r--r--   0        0        0     1083 2022-11-11 02:03:40.000000 fast_tmp-1.1.7/fast_tmp/amis/enums.py
--rw-r--r--   0        0        0    17747 2022-11-14 05:58:48.000000 fast_tmp-1.1.7/fast_tmp/amis/formitem.py
--rw-r--r--   0        0        0      841 2022-11-11 02:03:40.000000 fast_tmp-1.1.7/fast_tmp/amis/forms/__init__.py
--rw-r--r--   0        0        0      543 2022-10-10 08:51:27.000000 fast_tmp-1.1.7/fast_tmp/amis/frame.py
--rw-r--r--   0        0        0      236 2022-11-11 02:03:40.000000 fast_tmp-1.1.7/fast_tmp/amis/nav.py
--rw-r--r--   0        0        0     2198 2022-11-11 02:03:40.000000 fast_tmp-1.1.7/fast_tmp/amis/page.py
--rw-r--r--   0        0        0       43 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/amis/response.py
--rw-r--r--   0        0        0      556 2022-11-11 02:03:40.000000 fast_tmp-1.1.7/fast_tmp/amis/style.py
--rw-r--r--   0        0        0     1592 2022-11-11 02:03:40.000000 fast_tmp-1.1.7/fast_tmp/amis/validate.py
--rw-r--r--   0        0        0        0 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/amis/view/__init__.py
--rw-r--r--   0        0        0      424 2022-11-11 02:03:40.000000 fast_tmp-1.1.7/fast_tmp/amis/view/card.py
--rw-r--r--   0        0        0      134 2022-11-11 02:03:40.000000 fast_tmp-1.1.7/fast_tmp/amis/view/divider.py
--rw-r--r--   0        0        0     2383 2022-11-11 02:03:40.000000 fast_tmp-1.1.7/fast_tmp/amis/wizard.py
--rw-r--r--   0        0        0     4187 2023-01-31 02:21:15.340699 fast_tmp-1.1.7/fast_tmp/conf/__init__.py
--rw-r--r--   0        0        0        0 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/contrib/__init__.py
--rw-r--r--   0        0        0        0 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/contrib/auth/__init__.py
--rw-r--r--   0        0        0    22149 2023-01-31 04:59:54.870218 fast_tmp-1.1.7/fast_tmp/contrib/auth/hashers.py
--rw-r--r--   0        0        0    17557 2022-10-10 08:51:27.000000 fast_tmp-1.1.7/fast_tmp/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0        0 2022-10-09 08:04:27.000000 fast_tmp-1.1.7/fast_tmp/contrib/tortoise/__init__.py
--rw-r--r--   0        0        0     3167 2023-01-31 04:59:54.754217 fast_tmp-1.1.7/fast_tmp/contrib/tortoise/fields.py
--rw-r--r--   0        0        0      737 2022-10-09 08:04:27.000000 fast_tmp-1.1.7/fast_tmp/contrib/tortoise/validators.py
--rw-r--r--   0        0        0     1161 2022-10-19 01:35:49.000000 fast_tmp-1.1.7/fast_tmp/exceptions.py
--rw-r--r--   0        0        0      795 2022-12-01 06:18:24.000000 fast_tmp-1.1.7/fast_tmp/factory.py
--rw-r--r--   0        0        0       57 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/jinja_extension/__init__.py
--rw-r--r--   0        0        0      537 2022-10-09 08:04:27.000000 fast_tmp-1.1.7/fast_tmp/jinja_extension/tags.py
--rw-r--r--   0        0        0     4030 2022-11-18 02:32:08.000000 fast_tmp-1.1.7/fast_tmp/models.py
--rw-r--r--   0        0        0      372 2022-10-19 01:34:35.000000 fast_tmp-1.1.7/fast_tmp/responses.py
--rw-r--r--   0        0        0    17244 2023-01-31 04:59:55.010220 fast_tmp-1.1.7/fast_tmp/site/__init__.py
--rw-r--r--   0        0        0    10247 2023-01-31 04:59:54.878218 fast_tmp-1.1.7/fast_tmp/site/base.py
--rw-r--r--   0        0        0    21504 2023-01-31 04:59:55.062221 fast_tmp-1.1.7/fast_tmp/site/field.py
--rw-r--r--   0        0        0     2329 2022-12-19 02:48:03.000000 fast_tmp-1.1.7/fast_tmp/site/filter.py
--rw-r--r--   0        0        0      625 2022-11-14 05:58:48.000000 fast_tmp-1.1.7/fast_tmp/utils/__init__.py
--rw-r--r--   0        0        0     2778 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/utils/crypto.py
--rw-r--r--   0        0        0      431 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/utils/db.py
--rw-r--r--   0        0        0     1669 2022-09-29 08:09:41.000000 fast_tmp-1.1.7/fast_tmp/utils/encoding.py
--rw-r--r--   0        0        0      742 2022-10-10 08:51:27.000000 fast_tmp-1.1.7/fast_tmp/utils/model.py
--rw-r--r--   0        0        0      565 2022-12-21 02:38:53.000000 fast_tmp-1.1.7/fast_tmp/utils/token.py
--rw-r--r--   0        0        0     2666 2022-10-10 08:51:27.000000 fast_tmp-1.1.7/fast_tmp_cli/__init__.py
--rw-r--r--   0        0        0      232 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/cookiecutter.json
--rw-r--r--   0        0        0      690 2022-10-13 03:06:31.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/app.py
--rw-r--r--   0        0        0       78 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/conftest.py
--rw-r--r--   0        0        0    59305 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/css/fontawesome.min.css
--rw-r--r--   0        0        0       46 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/css/main.css
--rw-r--r--   0        0        0   279740 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/css/tabler.min.css
--rw-r--r--   0        0        0     2996 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/img/logo.svg
--rw-r--r--   0        0        0  1196706 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/fontawesome.min.js
--rw-r--r--   0        0        0    89501 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/jquery.min.js
--rw-r--r--   0        0        0      352 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/logout.js
--rw-r--r--   0        0        0      576 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/main.js
--rw-r--r--   0        0        0    58889 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/moment.min.js
--rw-r--r--   0        0        0   137925 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/tabler.min.js
--rw-r--r--   0        0        0     6242 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/logo.png
--rw-r--r--   0        0        0        0 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
--rw-r--r--   0        0        0        0 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/admin.py
--rw-r--r--   0        0        0        0 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/models.py
--rw-r--r--   0        0        0      567 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/settings.py
--rw-r--r--   0        0        0        2 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/static/cookiecutter.json
--rw-r--r--   0        0        0  1206703 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/static/static/redoc.standalone.js
--rw-r--r--   0        0        0  1097449 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/static/static/swagger-ui-bundle.js
--rw-r--r--   0        0        0   143410 2022-09-29 08:03:53.000000 fast_tmp-1.1.7/fast_tmp_cli/tpl/static/static/swagger-ui.css
--rw-r--r--   0        0        0     1397 2023-01-31 05:45:36.640802 fast_tmp-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     1840 1970-01-01 00:00:00.000000 fast_tmp-1.1.7/setup.py
--rw-r--r--   0        0        0      902 1970-01-01 00:00:00.000000 fast_tmp-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/LICENSE
+-rw-r--r--   0        0        0     3101 2023-01-31 06:26:10.842170 fast_tmp-1.1.9/README.md
+-rw-r--r--   0        0        0        0 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/admin/__init__.py
+-rw-r--r--   0        0        0     1051 2022-10-12 10:00:24.000000 fast_tmp-1.1.9/fast_tmp/admin/depends.py
+-rw-r--r--   0        0        0     4933 2023-01-31 04:59:54.802217 fast_tmp-1.1.9/fast_tmp/admin/endpoint.py
+-rw-r--r--   0        0        0      848 2022-09-29 08:13:27.000000 fast_tmp-1.1.9/fast_tmp/admin/exception_handlers.py
+-rw-r--r--   0        0        0      645 2022-10-13 02:18:55.000000 fast_tmp-1.1.9/fast_tmp/admin/register.py
+-rw-r--r--   0        0        0     5597 2023-01-31 07:54:39.433334 fast_tmp-1.1.9/fast_tmp/admin/server.py
+-rw-r--r--   0        0        0     1989 2023-01-31 04:59:54.738216 fast_tmp-1.1.9/fast_tmp/admin/site.py
+-rw-r--r--   0        0        0        0 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/admin/template.py
+-rw-r--r--   0        0        0     1086 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/admin/templates/base.html
+-rw-r--r--   0        0        0     7437 2022-11-11 02:06:15.000000 fast_tmp-1.1.9/fast_tmp/admin/templates/index.html
+-rw-r--r--   0        0        0     3516 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/admin/templates/login.html
+-rw-r--r--   0        0        0        0 2022-12-01 07:00:20.000000 fast_tmp-1.1.9/fast_tmp/amis/__init__.py
+-rw-r--r--   0        0        0     1437 2022-11-11 02:03:40.000000 fast_tmp-1.1.9/fast_tmp/amis/actions.py
+-rw-r--r--   0        0        0      810 2022-11-11 02:03:40.000000 fast_tmp-1.1.9/fast_tmp/amis/base.py
+-rw-r--r--   0        0        0     1576 2023-01-31 04:51:01.424473 fast_tmp-1.1.9/fast_tmp/amis/column.py
+-rw-r--r--   0        0        0      670 2022-11-11 02:03:40.000000 fast_tmp-1.1.9/fast_tmp/amis/crud.py
+-rw-r--r--   0        0        0     1083 2022-11-11 02:03:40.000000 fast_tmp-1.1.9/fast_tmp/amis/enums.py
+-rw-r--r--   0        0        0    17747 2022-11-14 05:58:48.000000 fast_tmp-1.1.9/fast_tmp/amis/formitem.py
+-rw-r--r--   0        0        0      841 2022-11-11 02:03:40.000000 fast_tmp-1.1.9/fast_tmp/amis/forms/__init__.py
+-rw-r--r--   0        0        0      543 2022-10-10 08:51:27.000000 fast_tmp-1.1.9/fast_tmp/amis/frame.py
+-rw-r--r--   0        0        0      236 2022-11-11 02:03:40.000000 fast_tmp-1.1.9/fast_tmp/amis/nav.py
+-rw-r--r--   0        0        0     2198 2022-11-11 02:03:40.000000 fast_tmp-1.1.9/fast_tmp/amis/page.py
+-rw-r--r--   0        0        0       43 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/amis/response.py
+-rw-r--r--   0        0        0      556 2022-11-11 02:03:40.000000 fast_tmp-1.1.9/fast_tmp/amis/style.py
+-rw-r--r--   0        0        0     1592 2022-11-11 02:03:40.000000 fast_tmp-1.1.9/fast_tmp/amis/validate.py
+-rw-r--r--   0        0        0        0 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/amis/view/__init__.py
+-rw-r--r--   0        0        0      424 2022-11-11 02:03:40.000000 fast_tmp-1.1.9/fast_tmp/amis/view/card.py
+-rw-r--r--   0        0        0      134 2022-11-11 02:03:40.000000 fast_tmp-1.1.9/fast_tmp/amis/view/divider.py
+-rw-r--r--   0        0        0     2383 2022-11-11 02:03:40.000000 fast_tmp-1.1.9/fast_tmp/amis/wizard.py
+-rw-r--r--   0        0        0     4187 2023-01-31 02:21:15.340699 fast_tmp-1.1.9/fast_tmp/conf/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/contrib/auth/__init__.py
+-rw-r--r--   0        0        0    22149 2023-01-31 07:54:39.505335 fast_tmp-1.1.9/fast_tmp/contrib/auth/hashers.py
+-rw-r--r--   0        0        0    17557 2022-10-10 08:51:27.000000 fast_tmp-1.1.9/fast_tmp/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-09 08:04:27.000000 fast_tmp-1.1.9/fast_tmp/contrib/tortoise/__init__.py
+-rw-r--r--   0        0        0     3167 2023-01-31 07:54:39.397334 fast_tmp-1.1.9/fast_tmp/contrib/tortoise/fields.py
+-rw-r--r--   0        0        0      737 2022-10-09 08:04:27.000000 fast_tmp-1.1.9/fast_tmp/contrib/tortoise/validators.py
+-rw-r--r--   0        0        0     1161 2022-10-19 01:35:49.000000 fast_tmp-1.1.9/fast_tmp/exceptions.py
+-rw-r--r--   0        0        0      795 2022-12-01 06:18:24.000000 fast_tmp-1.1.9/fast_tmp/factory.py
+-rw-r--r--   0        0        0       57 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/jinja_extension/__init__.py
+-rw-r--r--   0        0        0      537 2022-10-09 08:04:27.000000 fast_tmp-1.1.9/fast_tmp/jinja_extension/tags.py
+-rw-r--r--   0        0        0     4030 2022-11-18 02:32:08.000000 fast_tmp-1.1.9/fast_tmp/models.py
+-rw-r--r--   0        0        0      372 2022-10-19 01:34:35.000000 fast_tmp-1.1.9/fast_tmp/responses.py
+-rw-r--r--   0        0        0    17294 2023-01-31 07:54:39.709337 fast_tmp-1.1.9/fast_tmp/site/__init__.py
+-rw-r--r--   0        0        0    10247 2023-01-31 04:59:54.878218 fast_tmp-1.1.9/fast_tmp/site/base.py
+-rw-r--r--   0        0        0    21504 2023-01-31 07:54:39.649336 fast_tmp-1.1.9/fast_tmp/site/field.py
+-rw-r--r--   0        0        0     2329 2022-12-19 02:48:03.000000 fast_tmp-1.1.9/fast_tmp/site/filter.py
+-rw-r--r--   0        0        0      625 2022-11-14 05:58:48.000000 fast_tmp-1.1.9/fast_tmp/utils/__init__.py
+-rw-r--r--   0        0        0     2778 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/utils/crypto.py
+-rw-r--r--   0        0        0      431 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/utils/db.py
+-rw-r--r--   0        0        0     1669 2022-09-29 08:09:41.000000 fast_tmp-1.1.9/fast_tmp/utils/encoding.py
+-rw-r--r--   0        0        0      742 2022-10-10 08:51:27.000000 fast_tmp-1.1.9/fast_tmp/utils/model.py
+-rw-r--r--   0        0        0      565 2022-12-21 02:38:53.000000 fast_tmp-1.1.9/fast_tmp/utils/token.py
+-rw-r--r--   0        0        0     2666 2022-10-10 08:51:27.000000 fast_tmp-1.1.9/fast_tmp_cli/__init__.py
+-rw-r--r--   0        0        0      232 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/cookiecutter.json
+-rw-r--r--   0        0        0      690 2022-10-13 03:06:31.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/app.py
+-rw-r--r--   0        0        0       78 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/conftest.py
+-rw-r--r--   0        0        0    59305 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/css/fontawesome.min.css
+-rw-r--r--   0        0        0       46 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/css/main.css
+-rw-r--r--   0        0        0   279740 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/css/tabler.min.css
+-rw-r--r--   0        0        0     2996 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/img/logo.svg
+-rw-r--r--   0        0        0  1196706 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/fontawesome.min.js
+-rw-r--r--   0        0        0    89501 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/jquery.min.js
+-rw-r--r--   0        0        0      352 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/logout.js
+-rw-r--r--   0        0        0      576 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/main.js
+-rw-r--r--   0        0        0    58889 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/moment.min.js
+-rw-r--r--   0        0        0   137925 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/tabler.min.js
+-rw-r--r--   0        0        0     6242 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/logo.png
+-rw-r--r--   0        0        0        0 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/admin.py
+-rw-r--r--   0        0        0        0 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/models.py
+-rw-r--r--   0        0        0      567 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/settings.py
+-rw-r--r--   0        0        0        2 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/static/cookiecutter.json
+-rw-r--r--   0        0        0  1206703 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/static/static/redoc.standalone.js
+-rw-r--r--   0        0        0  1097449 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/static/static/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   143410 2022-09-29 08:03:53.000000 fast_tmp-1.1.9/fast_tmp_cli/tpl/static/static/swagger-ui.css
+-rw-r--r--   0        0        0     1397 2023-02-01 04:30:39.932055 fast_tmp-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1840 1970-01-01 00:00:00.000000 fast_tmp-1.1.9/setup.py
+-rw-r--r--   0        0        0      902 1970-01-01 00:00:00.000000 fast_tmp-1.1.9/PKG-INFO
```

### Comparing `fast_tmp-1.1.7/LICENSE` & `fast_tmp-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/README.md` & `fast_tmp-1.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # fast-tmp
 
 演示方式：
 通过docker拉镜像：
 
 ```shell
-sudo docker run -p 8000:8000 chise123/fast-tmp-example:v1.0.1
+sudo docker run -p 8000:8000 chise123/fast-tmp-example:v1.0.2
 ```
 
 然后访问```http://127.0.0.1:8000/admin```即可，
 超级用户的账户密码为```admin/123456```
 项目模板
 
 ## 概述
```

### Comparing `fast_tmp-1.1.7/fast_tmp/admin/depends.py` & `fast_tmp-1.1.9/fast_tmp/admin/depends.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/admin/endpoint.py` & `fast_tmp-1.1.9/fast_tmp/admin/endpoint.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/admin/exception_handlers.py` & `fast_tmp-1.1.9/fast_tmp/admin/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/admin/register.py` & `fast_tmp-1.1.9/fast_tmp/admin/register.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/admin/server.py` & `fast_tmp-1.1.9/fast_tmp/admin/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         perms = [
             i.codename
             for i in await Permission.filter(groups__users=user, codename__endswith="list")
         ]
         for name, ml in model_list.items():
             ml_p = []
             for model in ml:
-                if model.name + "_list" in perms:
+                if model.prefix + "_list" in perms:
                     if not index_page:
                         index_page = model
                     ml_p.append(model)
             if len(ml_p) == 0:
                 continue
             pages.append(
                 {
```

### Comparing `fast_tmp-1.1.7/fast_tmp/admin/site.py` & `fast_tmp-1.1.9/fast_tmp/admin/site.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/admin/templates/base.html` & `fast_tmp-1.1.9/fast_tmp/admin/templates/base.html`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/admin/templates/index.html` & `fast_tmp-1.1.9/fast_tmp/admin/templates/index.html`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/admin/templates/login.html` & `fast_tmp-1.1.9/fast_tmp/admin/templates/login.html`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/amis/actions.py` & `fast_tmp-1.1.9/fast_tmp/amis/actions.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/amis/base.py` & `fast_tmp-1.1.9/fast_tmp/amis/base.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/amis/column.py` & `fast_tmp-1.1.9/fast_tmp/amis/column.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/amis/crud.py` & `fast_tmp-1.1.9/fast_tmp/amis/crud.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/amis/enums.py` & `fast_tmp-1.1.9/fast_tmp/amis/enums.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/amis/formitem.py` & `fast_tmp-1.1.9/fast_tmp/amis/formitem.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/amis/forms/__init__.py` & `fast_tmp-1.1.9/fast_tmp/amis/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/amis/frame.py` & `fast_tmp-1.1.9/fast_tmp/amis/frame.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/amis/page.py` & `fast_tmp-1.1.9/fast_tmp/amis/page.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/amis/style.py` & `fast_tmp-1.1.9/fast_tmp/amis/style.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/amis/validate.py` & `fast_tmp-1.1.9/fast_tmp/amis/validate.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/amis/wizard.py` & `fast_tmp-1.1.9/fast_tmp/amis/wizard.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/conf/__init__.py` & `fast_tmp-1.1.9/fast_tmp/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/contrib/auth/hashers.py` & `fast_tmp-1.1.9/fast_tmp/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/contrib/pydantic/__init__.py` & `fast_tmp-1.1.9/fast_tmp/contrib/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/contrib/tortoise/fields.py` & `fast_tmp-1.1.9/fast_tmp/contrib/tortoise/fields.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/contrib/tortoise/validators.py` & `fast_tmp-1.1.9/fast_tmp/contrib/tortoise/validators.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/exceptions.py` & `fast_tmp-1.1.9/fast_tmp/exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/factory.py` & `fast_tmp-1.1.9/fast_tmp/factory.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/jinja_extension/tags.py` & `fast_tmp-1.1.9/fast_tmp/jinja_extension/tags.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/models.py` & `fast_tmp-1.1.9/fast_tmp/models.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/site/__init__.py` & `fast_tmp-1.1.9/fast_tmp/site/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,17 +155,17 @@
                     initApi="get:" + self.prefix + "/update/$pk",
                 ),
             ),
         )
 
     def get_operation(self, request: Request, codenames: List[str]):
         buttons = []
-        if "put" in self.methods and self.update_fields and self.name + "_update" in codenames:
+        if "put" in self.methods and self.update_fields and self.prefix + "_update" in codenames:
             buttons.append(self.get_update_one_button(request, codenames))
-        if "delete" in self.methods and self.name + "_delete" in codenames:
+        if "delete" in self.methods and self.prefix + "_delete" in codenames:
             buttons.append(self.get_del_one_button())
         if len(buttons) > 0:
             return Operation(buttons=buttons)
         return None
 
     def get_filter_page(self, request: Request):
         """
@@ -174,28 +174,28 @@
         return FilterModel(
             body=[v.filter_control(request) for v in self.get_filters(request).values()]
         )
 
     def get_crud(self, request: Request, codenames: List[str]):
         body: List[BaseAmisModel] = []
         columns = []
-        if "create" in self.methods and self.create_fields and self.name + "_create" in codenames:
+        if "create" in self.methods and self.create_fields and self.prefix + "_create" in codenames:
             body.extend(self.get_create_dialogation_button(request, codenames))
-        if "list" in self.methods and self.list_display and self.name + "_list" in codenames:
+        if "list" in self.methods and self.list_display and self.prefix + "_list" in codenames:
             columns.extend(self.get_list_fields(request))
         buttons = self.get_operation(request, codenames)
         if buttons:
             columns.append(buttons)
         crud = CRUD(
             api=self._prefix + "/list",
             columns=columns,
             quickSaveItemApi=self._prefix + "/patch/" + "$pk",
             syncLocation=False,
         )
-        if len(self.get_filters(request)) > 0 and self.name + "_list" in codenames:
+        if len(self.get_filters(request)) > 0 and self.prefix + "_list" in codenames:
             crud.filter = self.get_filter_page(request)
         body.append(crud)
         return body
 
     def get_list_distplay(self) -> Dict[str, BaseAdminControl]:
         return {i: self.get_formitem_field(i) for i in self.list_display}
 
@@ -332,18 +332,18 @@
 
     async def permission_code(self, request: Request):
         """
         判断用户拥有的权限
         """
         if self._permissions is None:
             self._permissions = [
-                self.name + "_list",
-                self.name + "_create",
-                self.name + "_update",
-                self.name + "_delete",
+                self.prefix.lower() + "_list",
+                self.prefix.lower() + "_create",
+                self.prefix.lower() + "_update",
+                self.prefix.lower() + "_delete",
             ]
         user = request.user
         if user.is_superuser:
             return self._permissions
         return [
             i.codename
             for i in await Permission.filter(groups__users=user, codename__in=self._permissions)
@@ -377,29 +377,29 @@
         ret = self.fields.get(name)
         if ret is None:
             raise NotFoundError("can not found field:" + name)
         return ret
 
     def __init__(self, prefix: Optional[str] = None, label: Optional[str] = None):
         if not prefix:
-            prefix = self.model.__name__
+            prefix = self.model.__name__.lower()
         if not label:
             try:
                 self._name = self.model.table_description  # type: ignore
             except AttributeError:
                 doc = self.model.__doc__
                 if doc:
                     docs = doc.split("\n")
                     for i in docs:
                         if i:
                             label = i.replace(" ", "")
                             break
                 pass
 
-        super().__init__(prefix, label or self.model.__name__.lower())
+        super().__init__(prefix, label or self.model.__name__)
         if not self.fields:
             self.fields = {}
         self.make_fields()
         col_set = set(self.get_list_distplay())
         for i in self.inline:
             if i not in col_set:
                 logger.warning("inline field " + i + " not in list_display")
```

### Comparing `fast_tmp-1.1.7/fast_tmp/site/base.py` & `fast_tmp-1.1.9/fast_tmp/site/base.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/site/field.py` & `fast_tmp-1.1.9/fast_tmp/site/field.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/site/filter.py` & `fast_tmp-1.1.9/fast_tmp/site/filter.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/utils/__init__.py` & `fast_tmp-1.1.9/fast_tmp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/utils/crypto.py` & `fast_tmp-1.1.9/fast_tmp/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/utils/encoding.py` & `fast_tmp-1.1.9/fast_tmp/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/utils/model.py` & `fast_tmp-1.1.9/fast_tmp/utils/model.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp/utils/token.py` & `fast_tmp-1.1.9/fast_tmp/utils/token.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/__init__.py` & `fast_tmp-1.1.9/fast_tmp_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/app.py` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/app.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/css/fontawesome.min.css` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/css/tabler.min.css` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/img/logo.svg` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/fontawesome.min.js` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/jquery.min.js` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/main.js` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/main.js`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/moment.min.js` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/tabler.min.js` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/logo.png` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/static/logo.png`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/settings.py` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/project/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/settings.py`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/static/static/redoc.standalone.js` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/static/static/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/static/static/swagger-ui-bundle.js` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/static/static/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/fast_tmp_cli/tpl/static/static/swagger-ui.css` & `fast_tmp-1.1.9/fast_tmp_cli/tpl/static/static/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `fast_tmp-1.1.7/pyproject.toml` & `fast_tmp-1.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "fast-tmp"
-version = "1.1.7"
+version = "1.1.9"
 description = "fastapi tortoise amis admin"
 authors = ["Chise1 <chise123@live.com>"]
 include = ["LICENSE", "README.md"]
 license = "Apache-2.0"
 packages = [
     { include = "fast_tmp_cli" },
     { include = "fast_tmp" }
 ]
 repository = "https://github.com/Chise1/fast-tmp"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typer = "^0.7.0"
-fastapi = "^0.88.0"
+fastapi = "^0.89.0"
 python-jose = "^3.3.0"
 asgiref = "^3.5.2"
 tortoise-orm = "^0.19.2"
 python-multipart = "^0.0.5"
 toml = "^0.10.2"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `fast_tmp-1.1.7/setup.py` & `fast_tmp-1.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,27 +27,27 @@
  'fast_tmp_cli.tpl.project.{{cookiecutter.project_slug}}': ['static/*',
                                                             'static/css/*',
                                                             'static/img/*',
                                                             'static/js/*']}
 
 install_requires = \
 ['asgiref>=3.5.2,<4.0.0',
- 'fastapi>=0.88.0,<0.89.0',
+ 'fastapi>=0.89.0,<0.90.0',
  'python-jose>=3.3.0,<4.0.0',
  'python-multipart>=0.0.5,<0.0.6',
  'toml>=0.10.2,<0.11.0',
  'tortoise-orm>=0.19.2,<0.20.0',
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['fast-tmp = fast_tmp_cli:main']}
 
 setup_kwargs = {
     'name': 'fast-tmp',
-    'version': '1.1.7',
+    'version': '1.1.9',
     'description': 'fastapi tortoise amis admin',
     'long_description': 'None',
     'author': 'Chise1',
     'author_email': 'chise123@live.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Chise1/fast-tmp',
```

### Comparing `fast_tmp-1.1.7/PKG-INFO` & `fast_tmp-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fast-tmp
-Version: 1.1.7
+Version: 1.1.9
 Summary: fastapi tortoise amis admin
 Home-page: https://github.com/Chise1/fast-tmp
 License: Apache-2.0
 Author: Chise1
 Author-email: chise123@live.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asgiref (>=3.5.2,<4.0.0)
-Requires-Dist: fastapi (>=0.88.0,<0.89.0)
+Requires-Dist: fastapi (>=0.89.0,<0.90.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tortoise-orm (>=0.19.2,<0.20.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/Chise1/fast-tmp
```

