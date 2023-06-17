# Comparing `tmp/django-admin-action-tools-1.1.6a1.tar.gz` & `tmp/django_admin_action_tools-1.1.6a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-action-tools-1.1.6a1.tar", last modified: Tue Feb 14 14:44:04 2023, max compression
+gzip compressed data, was "django_admin_action_tools-1.1.6a2.tar", max compression
```

## Comparing `django-admin-action-tools-1.1.6a1.tar` & `django_admin_action_tools-1.1.6a2.tar`

### file list

```diff
@@ -1,47 +1,46 @@
--rw-r--r--   0        0        0    11358 2023-02-14 14:43:50.277011 django-admin-action-tools-1.1.6a1/LICENSE
--rw-r--r--   0        0        0     9571 2023-02-14 14:43:50.277011 django-admin-action-tools-1.1.6a1/README.md
--rw-r--r--   0        0        0       47 2023-02-14 14:43:50.277011 django-admin-action-tools-1.1.6a1/admin_action_tools/__init__.py
--rw-r--r--   0        0        0      278 2023-02-14 14:43:50.277011 django-admin-action-tools-1.1.6a1/admin_action_tools/admin/__init__.py
--rw-r--r--   0        0        0     2722 2023-02-14 14:43:50.277011 django-admin-action-tools-1.1.6a1/admin_action_tools/admin/base.py
--rw-r--r--   0        0        0    19366 2023-02-14 14:43:50.277011 django-admin-action-tools-1.1.6a1/admin_action_tools/admin/confirm_tool.py
--rw-r--r--   0        0        0     4402 2023-02-14 14:43:50.277011 django-admin-action-tools-1.1.6a1/admin_action_tools/admin/form_tool.py
--rw-r--r--   0        0        0      968 2023-02-14 14:43:50.277011 django-admin-action-tools-1.1.6a1/admin_action_tools/constants.py
--rw-r--r--   0        0        0     3680 2023-02-14 14:43:50.277011 django-admin-action-tools-1.1.6a1/admin_action_tools/file_cache.py
--rw-r--r--   0        0        0      800 2023-02-14 14:43:50.277011 django-admin-action-tools-1.1.6a1/admin_action_tools/static/admin/css/confirmation.css
--rw-r--r--   0        0        0     1968 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/templates/admin/confirm_tool/action_confirmation.html
--rw-r--r--   0        0        0     2705 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/templates/admin/confirm_tool/change_confirmation.html
--rw-r--r--   0        0        0     1580 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/templates/admin/form_tool/action_form.html
--rw-r--r--   0        0        0      292 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/templates/admin/submit_line.html
--rw-r--r--   0        0        0      532 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/templates/include/change_data.html
--rw-r--r--   0        0        0      477 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/templates/include/form.html
--rw-r--r--   0        0        0      556 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/templates/include/submit_row.html
--rw-r--r--   0        0        0        0 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/templatetags/__init__.py
--rw-r--r--   0        0        0     1010 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/templatetags/formatting.py
--rw-r--r--   0        0        0     4908 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/helpers.py
--rw-r--r--   0        0        0     7962 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/confirm-tool/test_with_cache.py
--rw-r--r--   0        0        0     2066 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/confirm-tool/test_with_change_actions.py
--rw-r--r--   0        0        0     5291 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/confirm-tool/test_with_form_input_types.py
--rw-r--r--   0        0        0     7503 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/confirm-tool/test_with_inlines.py
--rw-r--r--   0        0        0     7470 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/confirm-tool/test_with_s3_storage.py
--rw-r--r--   0        0        0     7832 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/confirm-tool/test_with_validators_integration.py
--rw-r--r--   0        0        0     5285 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/form-tool/test_with_form_actions.py
--rw-r--r--   0        0        0     3757 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/form-tool/test_with_multiple_forms.py
--rw-r--r--   0        0        0      332 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/test_smoke.py
--rw-r--r--   0        0        0   109790 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/snapshot/screenshot.png
--rw-r--r--   0        0        0    11629 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_admin_options.py
--rw-r--r--   0        0        0    11056 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_confirm_actions.py
--rw-r--r--   0        0        0    13935 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add.py
--rw-r--r--   0        0        0     8025 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add_m2m_field.py
--rw-r--r--   0        0        0    16779 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_confirm_save_actions.py
--rw-r--r--   0        0        0    16460 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_confirmation_cache.py
--rw-r--r--   0        0        0    33930 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_confirmation_using_file_cache.py
--rw-r--r--   0        0        0     1042 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_file_cache.py
--rw-r--r--   0        0        0     4507 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_model_field_types.py
--rw-r--r--   0        0        0    12545 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_with_validators.py
--rw-r--r--   0        0        0     3370 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/form-tool/test_form_action.py
--rw-r--r--   0        0        0     2136 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/test_toolchain.py
--rw-r--r--   0        0        0     4236 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/toolchain.py
--rw-r--r--   0        0        0      667 2023-02-14 14:43:50.281011 django-admin-action-tools-1.1.6a1/admin_action_tools/utils.py
--rw-r--r--   0        0        0     3297 2023-02-14 14:44:00.572948 django-admin-action-tools-1.1.6a1/pyproject.toml
--rw-r--r--   0        0        0    11321 2023-02-14 14:44:04.757847 django-admin-action-tools-1.1.6a1/setup.py
--rw-r--r--   0        0        0    10482 2023-02-14 14:44:04.758689 django-admin-action-tools-1.1.6a1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-17 15:04:20.540795 django_admin_action_tools-1.1.6a2/LICENSE
+-rw-r--r--   0        0        0     9571 2023-06-17 15:04:20.540795 django_admin_action_tools-1.1.6a2/README.md
+-rw-r--r--   0        0        0       47 2023-06-17 15:04:20.540795 django_admin_action_tools-1.1.6a2/admin_action_tools/__init__.py
+-rw-r--r--   0        0        0      278 2023-06-17 15:04:20.540795 django_admin_action_tools-1.1.6a2/admin_action_tools/admin/__init__.py
+-rw-r--r--   0        0        0     2722 2023-06-17 15:04:20.540795 django_admin_action_tools-1.1.6a2/admin_action_tools/admin/base.py
+-rw-r--r--   0        0        0    19366 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/admin/confirm_tool.py
+-rw-r--r--   0        0        0     4402 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/admin/form_tool.py
+-rw-r--r--   0        0        0      968 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/constants.py
+-rw-r--r--   0        0        0     3680 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/file_cache.py
+-rw-r--r--   0        0        0      800 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/static/admin/css/confirmation.css
+-rw-r--r--   0        0        0     1968 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/templates/admin/confirm_tool/action_confirmation.html
+-rw-r--r--   0        0        0     2705 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/templates/admin/confirm_tool/change_confirmation.html
+-rw-r--r--   0        0        0     1580 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/templates/admin/form_tool/action_form.html
+-rw-r--r--   0        0        0      292 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/templates/admin/submit_line.html
+-rw-r--r--   0        0        0      532 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/templates/include/change_data.html
+-rw-r--r--   0        0        0      477 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/templates/include/form.html
+-rw-r--r--   0        0        0      556 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/templates/include/submit_row.html
+-rw-r--r--   0        0        0        0 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/templatetags/__init__.py
+-rw-r--r--   0        0        0     1010 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/templatetags/formatting.py
+-rw-r--r--   0        0        0     4908 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/helpers.py
+-rw-r--r--   0        0        0     7962 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/confirm-tool/test_with_cache.py
+-rw-r--r--   0        0        0     2066 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/confirm-tool/test_with_change_actions.py
+-rw-r--r--   0        0        0     5291 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/confirm-tool/test_with_form_input_types.py
+-rw-r--r--   0        0        0     7503 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/confirm-tool/test_with_inlines.py
+-rw-r--r--   0        0        0     7470 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/confirm-tool/test_with_s3_storage.py
+-rw-r--r--   0        0        0     7832 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/confirm-tool/test_with_validators_integration.py
+-rw-r--r--   0        0        0     5285 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/form-tool/test_with_form_actions.py
+-rw-r--r--   0        0        0     3757 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/form-tool/test_with_multiple_forms.py
+-rw-r--r--   0        0        0      332 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/test_smoke.py
+-rw-r--r--   0        0        0   109790 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/snapshot/screenshot.png
+-rw-r--r--   0        0        0    11629 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_admin_options.py
+-rw-r--r--   0        0        0    11056 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_confirm_actions.py
+-rw-r--r--   0        0        0    13935 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add.py
+-rw-r--r--   0        0        0     8025 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add_m2m_field.py
+-rw-r--r--   0        0        0    16779 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_confirm_save_actions.py
+-rw-r--r--   0        0        0    16460 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_confirmation_cache.py
+-rw-r--r--   0        0        0    33930 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_confirmation_using_file_cache.py
+-rw-r--r--   0        0        0     1042 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_file_cache.py
+-rw-r--r--   0        0        0     4507 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_model_field_types.py
+-rw-r--r--   0        0        0    12545 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_with_validators.py
+-rw-r--r--   0        0        0     3370 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/form-tool/test_form_action.py
+-rw-r--r--   0        0        0     2136 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/test_toolchain.py
+-rw-r--r--   0        0        0     4236 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/toolchain.py
+-rw-r--r--   0        0        0      667 2023-06-17 15:04:20.544797 django_admin_action_tools-1.1.6a2/admin_action_tools/utils.py
+-rw-r--r--   0        0        0     3297 2023-06-17 15:04:31.185184 django_admin_action_tools-1.1.6a2/pyproject.toml
+-rw-r--r--   0        0        0    10584 1970-01-01 00:00:00.000000 django_admin_action_tools-1.1.6a2/PKG-INFO
```

### Comparing `django-admin-action-tools-1.1.6a1/LICENSE` & `django_admin_action_tools-1.1.6a2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/README.md` & `django_admin_action_tools-1.1.6a2/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/admin/base.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/admin/base.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/admin/confirm_tool.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/admin/confirm_tool.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/admin/form_tool.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/admin/form_tool.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/constants.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/constants.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/file_cache.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/file_cache.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/static/admin/css/confirmation.css` & `django_admin_action_tools-1.1.6a2/admin_action_tools/static/admin/css/confirmation.css`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/templates/admin/confirm_tool/action_confirmation.html` & `django_admin_action_tools-1.1.6a2/admin_action_tools/templates/admin/confirm_tool/action_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/templates/admin/confirm_tool/change_confirmation.html` & `django_admin_action_tools-1.1.6a2/admin_action_tools/templates/admin/confirm_tool/change_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/templates/admin/form_tool/action_form.html` & `django_admin_action_tools-1.1.6a2/admin_action_tools/templates/admin/form_tool/action_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/templates/include/change_data.html` & `django_admin_action_tools-1.1.6a2/admin_action_tools/templates/include/change_data.html`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/templates/include/submit_row.html` & `django_admin_action_tools-1.1.6a2/admin_action_tools/templates/include/submit_row.html`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/templatetags/formatting.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/templatetags/formatting.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/helpers.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/confirm-tool/test_with_cache.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/confirm-tool/test_with_cache.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/confirm-tool/test_with_change_actions.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/confirm-tool/test_with_change_actions.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/confirm-tool/test_with_form_input_types.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/confirm-tool/test_with_form_input_types.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/confirm-tool/test_with_inlines.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/confirm-tool/test_with_inlines.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/confirm-tool/test_with_s3_storage.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/confirm-tool/test_with_s3_storage.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/confirm-tool/test_with_validators_integration.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/confirm-tool/test_with_validators_integration.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/form-tool/test_with_form_actions.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/form-tool/test_with_form_actions.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/integration/form-tool/test_with_multiple_forms.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/integration/form-tool/test_with_multiple_forms.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/snapshot/screenshot.png` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/snapshot/screenshot.png`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_admin_options.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_admin_options.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_confirm_actions.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_confirm_actions.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add_m2m_field.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add_m2m_field.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_confirm_save_actions.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_confirm_save_actions.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_confirmation_cache.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_confirmation_cache.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_confirmation_using_file_cache.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_confirmation_using_file_cache.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_file_cache.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_file_cache.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_model_field_types.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_model_field_types.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/confirm-tool/test_with_validators.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/confirm-tool/test_with_validators.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/form-tool/test_form_action.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/form-tool/test_form_action.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/tests/unit/test_toolchain.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/tests/unit/test_toolchain.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/toolchain.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/toolchain.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/admin_action_tools/utils.py` & `django_admin_action_tools-1.1.6a2/admin_action_tools/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-action-tools-1.1.6a1/pyproject.toml` & `django_admin_action_tools-1.1.6a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 name = "django-admin-action-tools"
 authors = [
     "Thu Trang Pham <thuutrangpham@gmail.com>",
     "jeanloup.monnier <jean-loup.monnier@spikeelabs.fr>",
 ]
 maintainers = ["jeanloup.monnier <jean-loup.monnier@spikeelabs.fr>"]
-version = "1.1.6-alpha.1"
+version = "1.1.6-alpha.2"
 description = "Tools for django admin"
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/SpikeeLabs/django-admin-action-tools"
 classifiers = [
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3 :: Only",
 ]
 packages = [{ include = "admin_action_tools" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-Django = ">=3.2, <= 4.2"
+Django = ">=3.2, <= 4.3"
 django-widget-tweaks = "^1.4"
 
 [tool.poetry.dev-dependencies]
 factory-boy = "^3.0"
 coverage = "^5.4"
 pytest = "^7"
 pytest-django = "^4.1"
@@ -43,14 +43,18 @@
 black = "^22"
 pre-commit = "^2.16"
 pylama = "^8.4.1"
 Pillow = "^9.2.0"
 toml = "^0.10.2"
 django-object-actions = "^4.0.0"
 
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
 [tool.black]
 exclude = '''
 (
     /(
         \.git
         |\.tox
         |migrations
@@ -105,11 +109,7 @@
 [tool.coverage.report]
 fail_under = 100
 
 [tool.pytest.ini_options]
 testpaths = "admin_action_tools/tests"
 DJANGO_SETTINGS_MODULE = "tests.test_project.settings.test"
 addopts = "--doctest-modules -ra -l --tb=short --show-capture=all --color=yes"
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
```

### Comparing `django-admin-action-tools-1.1.6a1/PKG-INFO` & `django_admin_action_tools-1.1.6a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: django-admin-action-tools
-Version: 1.1.6a1
+Version: 1.1.6a2
 Summary: Tools for django admin
 Home-page: https://github.com/SpikeeLabs/django-admin-action-tools
 License: Apache-2.0
 Author: Thu Trang Pham
 Author-email: thuutrangpham@gmail.com
 Maintainer: jeanloup.monnier
 Maintainer-email: jean-loup.monnier@spikeelabs.fr
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Django (>=3.2,<=4.2)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Dist: Django (>=3.2,<=4.3)
 Requires-Dist: django-widget-tweaks (>=1.4,<2.0)
 Project-URL: Repository, https://github.com/SpikeeLabs/django-admin-action-tools
 Description-Content-Type: text/markdown
 
 # Django Admin Confirm
 
 [![PyPI](https://img.shields.io/pypi/v/django-admin-action-tools?color=blue)](https://pypi.org/project/django-admin-action-tools/)
```

