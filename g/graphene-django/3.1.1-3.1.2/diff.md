# Comparing `tmp/graphene-django-3.1.1.tar.gz` & `tmp/graphene-django-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-django-3.1.1.tar", last modified: Wed May 24 13:11:31 2023, max compression
+gzip compressed data, was "graphene-django-3.1.2.tar", last modified: Sat Jun 17 06:42:35 2023, max compression
```

## Comparing `graphene-django-3.1.1.tar` & `graphene-django-3.1.2.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.939906 graphene-django-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-24 13:11:28.000000 graphene-django-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-24 13:11:28.000000 graphene-django-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-24 13:11:31.939906 graphene-django-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-24 13:11:28.000000 graphene-django-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook/cookbook/ingredients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook/cookbook/ingredients/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-24 13:11:28.000000 graphene-django-3.1.1/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook-plain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook-plain/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook-plain/cookbook/ingredients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook-plain/cookbook/ingredients/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-24 13:11:28.000000 graphene-django-3.1.1/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/debug/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/debug/exception/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/exception/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/exception/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/debug/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/sql/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/sql/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/debug/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/filter/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filters/array_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filters/global_id_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filters/list_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filters/range_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filters/typed_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filterset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/filter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_array_field_contains_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_array_field_exact_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_array_field_overlap_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_enum_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)    37395 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_in_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_range_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_typed_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/forms/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/mutation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/forms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/tests/test_djangoinputobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/management/commands/graphql_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/serializer_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/rest_framework/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/tests/test_field_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/tests/test_multiple_model_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/graphene_django/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/static/graphene_django/
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/static/graphene_django/graphiql.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/graphene_django/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.935906 graphene-django-3.1.1/graphene_django/templates/graphene/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/templates/graphene/graphiql.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.935906 graphene-django-3.1.1/graphene_django/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.935906 graphene-django-3.1.1/graphene_django/tests/issues/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/issues/test_520.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/schema_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20326 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_get_queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    49750 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23821 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/urls_inherited.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/urls_pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.935906 graphene-django-3.1.1/graphene_django/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/str_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.935906 graphene-django-3.1.1/graphene_django/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/tests/test_str_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-24 13:11:31.000000 graphene-django-3.1.1/graphene_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-24 13:11:31.000000 graphene-django-3.1.1/graphene_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:11:31.000000 graphene-django-3.1.1/graphene_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:11:31.000000 graphene-django-3.1.1/graphene_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-24 13:11:31.000000 graphene-django-3.1.1/graphene_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 13:11:31.000000 graphene-django-3.1.1/graphene_django.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-24 13:11:31.939906 graphene-django-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-24 13:11:28.000000 graphene-django-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-17 06:42:31.000000 graphene-django-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-17 06:42:31.000000 graphene-django-3.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-17 06:42:35.762130 graphene-django-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-06-17 06:42:31.000000 graphene-django-3.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook/cookbook/ingredients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook/cookbook/ingredients/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-17 06:42:31.000000 graphene-django-3.1.2/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook-plain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook-plain/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook-plain/cookbook/ingredients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook-plain/cookbook/ingredients/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-17 06:42:31.000000 graphene-django-3.1.2/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/graphene_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/debug/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/exception/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/exception/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/debug/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/sql/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/sql/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/debug/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/filter/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filters/array_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filters/global_id_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filters/list_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filters/range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filters/typed_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filterset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/filter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_array_field_contains_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_array_field_exact_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_array_field_overlap_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_enum_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37395 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_in_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_typed_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/mutation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/forms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/tests/test_djangoinputobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/management/commands/graphql_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/serializer_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/rest_framework/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/tests/test_field_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/tests/test_multiple_model_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/graphene_django/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/static/graphene_django/
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/static/graphene_django/graphiql.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/graphene_django/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/templates/graphene/
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/templates/graphene/graphiql.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/tests/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/issues/test_520.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/schema_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20326 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_get_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49738 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23821 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/urls_inherited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/urls_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/tests/test_str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-17 06:42:35.000000 graphene-django-3.1.2/graphene_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-17 06:42:35.000000 graphene-django-3.1.2/graphene_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 06:42:35.000000 graphene-django-3.1.2/graphene_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 06:42:35.000000 graphene-django-3.1.2/graphene_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-17 06:42:35.000000 graphene-django-3.1.2/graphene_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 06:42:35.000000 graphene-django-3.1.2/graphene_django.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-17 06:42:35.762130 graphene-django-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-17 06:42:31.000000 graphene-django-3.1.2/setup.py
```

### Comparing `graphene-django-3.1.1/LICENSE` & `graphene-django-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/PKG-INFO` & `graphene-django-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django
-Version: 3.1.1
+Version: 3.1.2
 Summary: Graphene Django integration
 Home-page: https://github.com/graphql-python/graphene-django
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Keywords: api graphql protocol rest relay graphene
 Platform: any
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: rest_framework
 Provides-Extra: dev
 License-File: LICENSE
 
 # ![Graphene Logo](http://graphene-python.org/favicon.png) Graphene-Django
```

### Comparing `graphene-django-3.1.1/README.md` & `graphene-django-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json` & `graphene-django-3.1.2/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json` & `graphene-django-3.1.2/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/converter.py` & `graphene-django-3.1.2/graphene_django/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 try:
     from graphql import assert_name
 except ImportError:
     # Support for older versions of graphql
     from graphql import assert_valid_name as assert_name
 from graphql.pyutils import register_description
 
-from .compat import ArrayField, HStoreField, JSONField, PGJSONField, RangeField
+from .compat import ArrayField, HStoreField, RangeField
 from .fields import DjangoListField, DjangoConnectionField
 from .settings import graphene_settings
 from .utils.str_converters import to_const
 
 
 class BlankValueField(Field):
     def wrap_resolve(self, parent_resolver):
@@ -342,17 +342,16 @@
         inner_type,
         description=get_django_field_description(field),
         required=not field.null,
     )
 
 
 @convert_django_field.register(HStoreField)
-@convert_django_field.register(PGJSONField)
-@convert_django_field.register(JSONField)
-def convert_pg_and_json_field_to_string(field, registry=None):
+@convert_django_field.register(models.JSONField)
+def convert_json_field_to_string(field, registry=None):
     return JSONString(
         description=get_django_field_description(field), required=not field.null
     )
 
 
 @convert_django_field.register(RangeField)
 def convert_postgres_range_to_string(field, registry=None):
```

### Comparing `graphene-django-3.1.1/graphene_django/debug/middleware.py` & `graphene-django-3.1.2/graphene_django/debug/middleware.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/debug/sql/tracking.py` & `graphene-django-3.1.2/graphene_django/debug/sql/tracking.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/debug/sql/types.py` & `graphene-django-3.1.2/graphene_django/debug/sql/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/debug/tests/test_query.py` & `graphene-django-3.1.2/graphene_django/debug/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/fields.py` & `graphene-django-3.1.2/graphene_django/fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/__init__.py` & `graphene-django-3.1.2/graphene_django/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/fields.py` & `graphene-django-3.1.2/graphene_django/filter/fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/filters/__init__.py` & `graphene-django-3.1.2/graphene_django/filter/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/filters/array_filter.py` & `graphene-django-3.1.2/graphene_django/filter/filters/array_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/filters/global_id_filter.py` & `graphene-django-3.1.2/graphene_django/filter/filters/global_id_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/filters/list_filter.py` & `graphene-django-3.1.2/graphene_django/filter/filters/list_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/filters/range_filter.py` & `graphene-django-3.1.2/graphene_django/filter/filters/range_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/filters/typed_filter.py` & `graphene-django-3.1.2/graphene_django/filter/filters/typed_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/filterset.py` & `graphene-django-3.1.2/graphene_django/filter/filterset.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/tests/conftest.py` & `graphene-django-3.1.2/graphene_django/filter/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/tests/filters.py` & `graphene-django-3.1.2/graphene_django/filter/tests/filters.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/tests/test_array_field_contains_filter.py` & `graphene-django-3.1.2/graphene_django/filter/tests/test_array_field_contains_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/tests/test_array_field_exact_filter.py` & `graphene-django-3.1.2/graphene_django/filter/tests/test_array_field_exact_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/tests/test_array_field_overlap_filter.py` & `graphene-django-3.1.2/graphene_django/filter/tests/test_array_field_overlap_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/tests/test_enum_filtering.py` & `graphene-django-3.1.2/graphene_django/filter/tests/test_enum_filtering.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/tests/test_fields.py` & `graphene-django-3.1.2/graphene_django/filter/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/tests/test_in_filter.py` & `graphene-django-3.1.2/graphene_django/filter/tests/test_in_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/tests/test_range_filter.py` & `graphene-django-3.1.2/graphene_django/filter/tests/test_range_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/tests/test_typed_filter.py` & `graphene-django-3.1.2/graphene_django/filter/tests/test_typed_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/filter/utils.py` & `graphene-django-3.1.2/graphene_django/filter/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/forms/converter.py` & `graphene-django-3.1.2/graphene_django/forms/converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/forms/forms.py` & `graphene-django-3.1.2/graphene_django/forms/forms.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/forms/mutation.py` & `graphene-django-3.1.2/graphene_django/forms/mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/forms/tests/test_converter.py` & `graphene-django-3.1.2/graphene_django/forms/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/forms/tests/test_djangoinputobject.py` & `graphene-django-3.1.2/graphene_django/forms/tests/test_djangoinputobject.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/forms/tests/test_mutation.py` & `graphene-django-3.1.2/graphene_django/forms/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/forms/types.py` & `graphene-django-3.1.2/graphene_django/forms/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/management/commands/graphql_schema.py` & `graphene-django-3.1.2/graphene_django/management/commands/graphql_schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/registry.py` & `graphene-django-3.1.2/graphene_django/registry.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/rest_framework/mutation.py` & `graphene-django-3.1.2/graphene_django/rest_framework/mutation.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,17 @@
             [
                 name in exclude_fields,
                 field.write_only
                 and not is_input,  # don't show write_only fields in Query
                 field.read_only
                 and is_input
                 and lookup_field != name,  # don't show read_only fields in Input
+                isinstance(
+                    field, serializers.HiddenField
+                ),  # don't show hidden fields in Input
             ]
         )
 
         if is_not_in_only or is_excluded:
             continue
 
         fields[name] = convert_serializer_field(
```

### Comparing `graphene-django-3.1.1/graphene_django/rest_framework/serializer_converter.py` & `graphene-django-3.1.2/graphene_django/rest_framework/serializer_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/rest_framework/tests/test_field_converter.py` & `graphene-django-3.1.2/graphene_django/rest_framework/tests/test_field_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/rest_framework/tests/test_multiple_model_serializers.py` & `graphene-django-3.1.2/graphene_django/rest_framework/tests/test_multiple_model_serializers.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/rest_framework/tests/test_mutation.py` & `graphene-django-3.1.2/graphene_django/rest_framework/tests/test_mutation.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,29 @@
     assert "password" in MyMutation.Input._meta.fields
     assert "id" in MyMutation.Input._meta.fields
     assert (
         "cool_name" not in MyMutation.Input._meta.fields
     ), "'cool_name' is read_only field and shouldn't be on arguments"
 
 
+def test_hidden_fields():
+    class SerializerWithHiddenField(serializers.Serializer):
+        cool_name = serializers.CharField()
+        user = serializers.HiddenField(default=serializers.CurrentUserDefault())
+
+    class MyMutation(SerializerMutation):
+        class Meta:
+            serializer_class = SerializerWithHiddenField
+
+    assert "cool_name" in MyMutation.Input._meta.fields
+    assert (
+        "user" not in MyMutation.Input._meta.fields
+    ), "'user' is hidden field and shouldn't be on arguments"
+
+
 def test_nested_model():
     class MyFakeModelGrapheneType(DjangoObjectType):
         class Meta:
             model = MyFakeModel
             fields = "__all__"
 
     class MyMutation(SerializerMutation):
```

### Comparing `graphene-django-3.1.1/graphene_django/settings.py` & `graphene-django-3.1.2/graphene_django/settings.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/static/graphene_django/graphiql.js` & `graphene-django-3.1.2/graphene_django/static/graphene_django/graphiql.js`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/templates/graphene/graphiql.html` & `graphene-django-3.1.2/graphene_django/templates/graphene/graphiql.html`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,18 @@
       width: 100%;
     }
   </style>
   <link href="https://cdn.jsdelivr.net/npm/graphiql@{{graphiql_version}}/graphiql.min.css"
         integrity="{{graphiql_css_sri}}"
         rel="stylesheet"
         crossorigin="anonymous" />
+  <link href="https://cdn.jsdelivr.net/npm/@graphiql/plugin-explorer@{{graphiql_plugin_explorer_version}}/dist/style.css"
+        integrity="{{graphiql_plugin_explorer_css_sri}}"
+        rel="stylesheet"
+        crossorigin="anonymous" />
   <script src="https://cdn.jsdelivr.net/npm/whatwg-fetch@{{whatwg_fetch_version}}/dist/fetch.umd.js"
           integrity="{{whatwg_fetch_sri}}"
           crossorigin="anonymous"></script>
   <script src="https://cdn.jsdelivr.net/npm/react@{{react_version}}/umd/react.production.min.js"
           integrity="{{react_sri}}"
           crossorigin="anonymous"></script>
   <script src="https://cdn.jsdelivr.net/npm/react-dom@{{react_version}}/umd/react-dom.production.min.js"
```

#### html2text {}

```diff
@@ -1,3 +1,4 @@
  {% load static %}
 
+
 {% csrf_token %}
```

### Comparing `graphene-django-3.1.1/graphene_django/tests/issues/test_520.py` & `graphene-django-3.1.2/graphene_django/tests/issues/test_520.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/tests/models.py` & `graphene-django-3.1.2/graphene_django/tests/models.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/tests/schema.py` & `graphene-django-3.1.2/graphene_django/tests/schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/tests/schema_view.py` & `graphene-django-3.1.2/graphene_django/tests/schema_view.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/tests/test_command.py` & `graphene-django-3.1.2/graphene_django/tests/test_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         management.call_command(
             "graphql_schema", schema=mock_schema, out="schema.graphql"
         )
 
     open_mock.assert_called_once()
 
     handle = open_mock()
-    assert handle.write.called_once()
+    handle.write.assert_called_once()
 
     schema_output = handle.write.call_args[0][0]
     assert schema_output == dedent(
         """\
         type Query {
           hi: String
         }"""
```

### Comparing `graphene-django-3.1.1/graphene_django/tests/test_converter.py` & `graphene-django-3.1.2/graphene_django/tests/test_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 from graphene.types.datetime import Date, DateTime, Time
 from graphene.types.json import JSONString
 from graphene.types.scalars import BigInt
 
 from ..compat import (
     ArrayField,
     HStoreField,
-    JSONField,
-    PGJSONField,
     MissingType,
     RangeField,
 )
 from ..converter import (
     convert_django_field,
     convert_django_field_with_choices,
     generate_enum_name,
@@ -368,24 +366,14 @@
 
 
 @pytest.mark.skipif(HStoreField is MissingType, reason="HStoreField should exist")
 def test_should_postgres_hstore_convert_string():
     assert_conversion(HStoreField, JSONString)
 
 
-@pytest.mark.skipif(PGJSONField is MissingType, reason="PGJSONField should exist")
-def test_should_postgres_json_convert_string():
-    assert_conversion(PGJSONField, JSONString)
-
-
-@pytest.mark.skipif(JSONField is MissingType, reason="JSONField should exist")
-def test_should_json_convert_string():
-    assert_conversion(JSONField, JSONString)
-
-
 @pytest.mark.skipif(RangeField is MissingType, reason="RangeField should exist")
 def test_should_postgres_range_convert_list():
     from django.contrib.postgres.fields import IntegerRangeField
 
     field = assert_conversion(IntegerRangeField, graphene.List)
     assert isinstance(field.type, graphene.NonNull)
     assert isinstance(field.type.of_type, graphene.List)
```

### Comparing `graphene-django-3.1.1/graphene_django/tests/test_fields.py` & `graphene-django-3.1.2/graphene_django/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/tests/test_forms.py` & `graphene-django-3.1.2/graphene_django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/tests/test_get_queryset.py` & `graphene-django-3.1.2/graphene_django/tests/test_get_queryset.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/tests/test_query.py` & `graphene-django-3.1.2/graphene_django/tests/test_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,21 +115,20 @@
 
 
 @pytest.mark.skipif(IntegerRangeField is MissingType, reason="RangeField should exist")
 def test_should_query_postgres_fields():
     from django.contrib.postgres.fields import (
         IntegerRangeField,
         ArrayField,
-        JSONField,
         HStoreField,
     )
 
     class Event(models.Model):
         ages = IntegerRangeField(help_text="The age ranges")
-        data = JSONField(help_text="Data")
+        data = models.JSONField(help_text="Data")
         store = HStoreField()
         tags = ArrayField(models.CharField(max_length=50))
 
     class EventType(DjangoObjectType):
         class Meta:
             model = Event
             fields = "__all__"
```

### Comparing `graphene-django-3.1.1/graphene_django/tests/test_schema.py` & `graphene-django-3.1.2/graphene_django/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/tests/test_types.py` & `graphene-django-3.1.2/graphene_django/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/tests/test_utils.py` & `graphene-django-3.1.2/graphene_django/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/tests/test_views.py` & `graphene-django-3.1.2/graphene_django/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/types.py` & `graphene-django-3.1.2/graphene_django/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/utils/testing.py` & `graphene-django-3.1.2/graphene_django/utils/testing.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/utils/tests/test_testing.py` & `graphene-django-3.1.2/graphene_django/utils/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/utils/utils.py` & `graphene-django-3.1.2/graphene_django/utils/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django/views.py` & `graphene-django-3.1.2/graphene_django/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,26 +62,29 @@
 
     # React and ReactDOM.
     react_version = "17.0.2"
     react_sri = "sha256-Ipu/TQ50iCCVZBUsZyNJfxrDk0E2yhaEIz0vqI+kFG8="
     react_dom_sri = "sha256-nbMykgB6tsOFJ7OdVmPpdqMFVk4ZsqWocT6issAPUF0="
 
     # The GraphiQL React app.
-    graphiql_version = "2.4.1"  # "1.0.3"
-    graphiql_sri = "sha256-s+f7CFAPSUIygFnRC2nfoiEKd3liCUy+snSdYFAoLUc="  # "sha256-VR4buIDY9ZXSyCNFHFNik6uSe0MhigCzgN4u7moCOTk="
-    graphiql_css_sri = "sha256-88yn8FJMyGboGs4Bj+Pbb3kWOWXo7jmb+XCRHE+282k="  # "sha256-LwqxjyZgqXDYbpxQJ5zLQeNcf7WVNSJ+r8yp2rnWE/E="
+    graphiql_version = "2.4.7"
+    graphiql_sri = "sha256-n/LKaELupC1H/PU6joz+ybeRJHT2xCdekEt6OYMOOZU="
+    graphiql_css_sri = "sha256-OsbM+LQHcnFHi0iH7AUKueZvDcEBoy/z4hJ7jx1cpsM="
 
     # The websocket transport library for subscriptions.
-    subscriptions_transport_ws_version = "5.12.1"
+    subscriptions_transport_ws_version = "5.13.1"
     subscriptions_transport_ws_sri = (
         "sha256-EZhvg6ANJrBsgLvLAa0uuHNLepLJVCFYS+xlb5U/bqw="
     )
 
     graphiql_plugin_explorer_version = "0.1.15"
     graphiql_plugin_explorer_sri = "sha256-3hUuhBXdXlfCj6RTeEkJFtEh/kUG+TCDASFpFPLrzvE="
+    graphiql_plugin_explorer_css_sri = (
+        "sha256-fA0LPUlukMNR6L4SPSeFqDTYav8QdWjQ2nr559Zln1U="
+    )
 
     schema = None
     graphiql = False
     middleware = None
     root_value = None
     pretty = False
     batch = False
```

### Comparing `graphene-django-3.1.1/graphene_django.egg-info/PKG-INFO` & `graphene-django-3.1.2/graphene_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django
-Version: 3.1.1
+Version: 3.1.2
 Summary: Graphene Django integration
 Home-page: https://github.com/graphql-python/graphene-django
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Keywords: api graphql protocol rest relay graphene
 Platform: any
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: rest_framework
 Provides-Extra: dev
 License-File: LICENSE
 
 # ![Graphene Logo](http://graphene-python.org/favicon.png) Graphene-Django
```

### Comparing `graphene-django-3.1.1/graphene_django.egg-info/SOURCES.txt` & `graphene-django-3.1.2/graphene_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/graphene_django.egg-info/requires.txt` & `graphene-django-3.1.2/graphene_django.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/setup.cfg` & `graphene-django-3.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.1/setup.py` & `graphene-django-3.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ] + tests_require
 
 setup(
     name="graphene-django",
     version=version,
     description="Graphene Django integration",
     long_description=open("README.md").read(),
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     url="https://github.com/graphql-python/graphene-django",
     author="Syrus Akbary",
     author_email="me@syrusakbary.com",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
@@ -52,16 +52,16 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
     ],
     keywords="api graphql protocol rest relay graphene",
     packages=find_packages(exclude=["tests", "examples", "examples.*"]),
     install_requires=[
         "graphene>=3.0,<4",
         "graphql-core>=3.1.0,<4",
         "graphql-relay>=3.1.1,<4",
```

