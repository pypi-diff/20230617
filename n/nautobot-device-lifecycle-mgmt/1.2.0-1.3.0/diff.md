# Comparing `tmp/nautobot_device_lifecycle_mgmt-1.2.0.tar.gz` & `tmp/nautobot_device_lifecycle_mgmt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_device_lifecycle_mgmt-1.2.0.tar", max compression
+gzip compressed data, was "nautobot_device_lifecycle_mgmt-1.3.0.tar", max compression
```

## Comparing `nautobot_device_lifecycle_mgmt-1.2.0.tar` & `nautobot_device_lifecycle_mgmt-1.3.0.tar`

### file list

```diff
@@ -1,76 +1,82 @@
--rw-r--r--   0        0        0      591 2023-04-21 15:38:36.765759 nautobot_device_lifecycle_mgmt-1.2.0/LICENSE
--rw-r--r--   0        0        0     4965 2023-04-21 15:38:36.765759 nautobot_device_lifecycle_mgmt-1.2.0/README.md
--rw-r--r--   0        0        0     1418 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/__init__.py
--rw-r--r--   0        0        0      328 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/admin.py
--rw-r--r--   0        0        0       65 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/__init__.py
--rw-r--r--   0        0        0     2970 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/nested_serializers.py
--rw-r--r--   0        0        0     9639 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/serializers.py
--rw-r--r--   0        0        0      926 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/urls.py
--rw-r--r--   0        0        0     3403 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/views.py
--rw-r--r--   0        0        0     2141 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/choices.py
--rw-r--r--   0        0        0     1188 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/const.py
--rw-r--r--   0        0        0    28481 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/filters.py
--rw-r--r--   0        0        0    39107 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/forms.py
--rw-r--r--   0        0        0      685 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/graphql/types.py
--rw-r--r--   0        0        0      327 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/jobs/__init__.py
--rw-r--r--   0        0        0     3191 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py
--rw-r--r--   0        0        0     3060 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py
--rw-r--r--   0        0        0     3449 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py
--rw-r--r--   0        0        0     4319 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py
--rw-r--r--   0        0        0     5580 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py
--rw-r--r--   0        0        0     2378 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py
--rw-r--r--   0        0        0     4405 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py
--rw-r--r--   0        0        0     4794 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py
--rw-r--r--   0        0        0     3131 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py
--rw-r--r--   0        0        0     1123 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py
--rw-r--r--   0        0        0      612 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py
--rw-r--r--   0        0        0        0 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/__init__.py
--rw-r--r--   0        0        0    29626 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/models.py
--rw-r--r--   0        0        0    13356 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/navigation.py
--rw-r--r--   0        0        0     5407 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/signals.py
--rw-r--r--   0        0        0     2995 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/software.py
--rw-r--r--   0        0        0     8101 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/software_filters.py
--rw-r--r--   0        0        0    14122 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tables.py
--rw-r--r--   0        0        0     4326 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/template_content.py
--rw-r--r--   0        0        0     2094 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html
--rw-r--r--   0        0        0     5904 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html
--rw-r--r--   0        0        0     2429 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html
--rw-r--r--   0        0        0     2613 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html
--rw-r--r--   0        0        0      939 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html
--rw-r--r--   0        0        0     1523 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html
--rw-r--r--   0        0        0     5632 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html
--rw-r--r--   0        0        0     2160 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html
--rw-r--r--   0        0        0      513 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html
--rw-r--r--   0        0        0     1113 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html
--rw-r--r--   0        0        0      365 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validatedsoftware_info.html
--rw-r--r--   0        0        0     3447 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html
--rw-r--r--   0        0        0     4705 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html
--rw-r--r--   0        0        0      263 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_delete.html
--rw-r--r--   0        0        0     1917 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html
--rw-r--r--   0        0        0       92 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_list.html
--rw-r--r--   0        0        0     3138 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html
--rw-r--r--   0        0        0      251 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_delete.html
--rw-r--r--   0        0        0       86 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_list.html
--rw-r--r--   0        0        0      392 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_software_images.html
--rw-r--r--   0        0        0     4234 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html
--rw-r--r--   0        0        0     4313 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html
--rw-r--r--   0        0        0     5686 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html
--rw-r--r--   0        0        0      269 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_delete.html
--rw-r--r--   0        0        0     1942 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html
--rw-r--r--   0        0        0       96 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_list.html
--rw-r--r--   0        0        0     1599 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html
--rw-r--r--   0        0        0      615 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html
--rw-r--r--   0        0        0       67 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/__init__.py
--rw-r--r--   0        0        0     3933 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/conftest.py
--rw-r--r--   0        0        0    24710 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_api.py
--rw-r--r--   0        0        0     1535 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_basic.py
--rw-r--r--   0        0        0    30041 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_filters.py
--rw-r--r--   0        0        0    23393 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_forms.py
--rw-r--r--   0        0        0    24237 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_model.py
--rw-r--r--   0        0        0    11840 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py
--rw-r--r--   0        0        0    11615 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_views.py
--rw-r--r--   0        0        0     9524 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/urls.py
--rw-r--r--   0        0        0      423 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/utils.py
--rw-r--r--   0        0        0    42336 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/views.py
--rw-r--r--   0        0        0     2771 2023-04-21 15:38:49.794005 nautobot_device_lifecycle_mgmt-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5958 1970-01-01 00:00:00.000000 nautobot_device_lifecycle_mgmt-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-06-17 20:01:15.064929 nautobot_device_lifecycle_mgmt-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5939 2023-06-17 20:01:15.064929 nautobot_device_lifecycle_mgmt-1.3.0/README.md
+-rw-r--r--   0        0        0     1418 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/__init__.py
+-rw-r--r--   0        0        0     3052 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/nested_serializers.py
+-rw-r--r--   0        0        0    11452 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/serializers.py
+-rw-r--r--   0        0        0     1234 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/urls.py
+-rw-r--r--   0        0        0     4602 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/views.py
+-rw-r--r--   0        0        0     2141 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/choices.py
+-rw-r--r--   0        0        0     1188 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/const.py
+-rw-r--r--   0        0        0    30000 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/filters.py
+-rw-r--r--   0        0        0    40491 2023-06-17 20:01:15.084929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/forms.py
+-rw-r--r--   0        0        0      685 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/graphql/types.py
+-rw-r--r--   0        0        0      327 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/jobs/__init__.py
+-rw-r--r--   0        0        0     3191 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py
+-rw-r--r--   0        0        0     3287 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py
+-rw-r--r--   0        0        0     9475 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/metrics.py
+-rw-r--r--   0        0        0     3449 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py
+-rw-r--r--   0        0        0     4319 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py
+-rw-r--r--   0        0        0     5580 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py
+-rw-r--r--   0        0        0     2378 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py
+-rw-r--r--   0        0        0     4405 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py
+-rw-r--r--   0        0        0     4794 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py
+-rw-r--r--   0        0        0     3131 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py
+-rw-r--r--   0        0        0     1123 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py
+-rw-r--r--   0        0        0      612 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py
+-rw-r--r--   0        0        0      463 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0010_softwareimagelcm_hash_algorithm.py
+-rw-r--r--   0        0        0      984 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py
+-rw-r--r--   0        0        0      902 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py
+-rw-r--r--   0        0        0        0 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/__init__.py
+-rw-r--r--   0        0        0    31202 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/models.py
+-rw-r--r--   0        0        0    14180 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/navigation.py
+-rw-r--r--   0        0        0     5407 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/signals.py
+-rw-r--r--   0        0        0     2995 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/software.py
+-rw-r--r--   0        0        0     8101 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/software_filters.py
+-rw-r--r--   0        0        0    20020 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tables.py
+-rw-r--r--   0        0        0     4326 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/template_content.py
+-rw-r--r--   0        0        0     2094 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html
+-rw-r--r--   0        0        0     5904 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html
+-rw-r--r--   0        0        0     2429 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html
+-rw-r--r--   0        0        0      492 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/devicesoftwarevalidationresult_list.html
+-rw-r--r--   0        0        0     2613 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html
+-rw-r--r--   0        0        0      939 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html
+-rw-r--r--   0        0        0     1523 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html
+-rw-r--r--   0        0        0     5632 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html
+-rw-r--r--   0        0        0     2160 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html
+-rw-r--r--   0        0        0      513 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html
+-rw-r--r--   0        0        0     1113 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html
+-rw-r--r--   0        0        0      747 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html
+-rw-r--r--   0        0        0      365 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validatedsoftware_info.html
+-rw-r--r--   0        0        0      505 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inventoryitemsoftwarevalidationresult_list.html
+-rw-r--r--   0        0        0     3605 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html
+-rw-r--r--   0        0        0     5075 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html
+-rw-r--r--   0        0        0      263 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_delete.html
+-rw-r--r--   0        0        0     1971 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html
+-rw-r--r--   0        0        0       92 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_list.html
+-rw-r--r--   0        0        0     3138 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html
+-rw-r--r--   0        0        0      251 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_delete.html
+-rw-r--r--   0        0        0       86 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_list.html
+-rw-r--r--   0        0        0      392 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_software_images.html
+-rw-r--r--   0        0        0     5784 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html
+-rw-r--r--   0        0        0     5885 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html
+-rw-r--r--   0        0        0     5686 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html
+-rw-r--r--   0        0        0      269 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_delete.html
+-rw-r--r--   0        0        0     1942 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html
+-rw-r--r--   0        0        0       96 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_list.html
+-rw-r--r--   0        0        0     1599 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html
+-rw-r--r--   0        0        0      615 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html
+-rw-r--r--   0        0        0       67 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/__init__.py
+-rw-r--r--   0        0        0     5247 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/conftest.py
+-rw-r--r--   0        0        0    27988 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_api.py
+-rw-r--r--   0        0        0     1535 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_basic.py
+-rw-r--r--   0        0        0    30831 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_filters.py
+-rw-r--r--   0        0        0    23393 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_forms.py
+-rw-r--r--   0        0        0    30032 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_model.py
+-rw-r--r--   0        0        0    11840 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py
+-rw-r--r--   0        0        0    16523 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_views.py
+-rw-r--r--   0        0        0    11497 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/urls.py
+-rw-r--r--   0        0        0      423 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/utils.py
+-rw-r--r--   0        0        0    43490 2023-06-17 20:01:15.088929 nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/views.py
+-rw-r--r--   0        0        0     2771 2023-06-17 20:01:28.468865 nautobot_device_lifecycle_mgmt-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6932 1970-01-01 00:00:00.000000 nautobot_device_lifecycle_mgmt-1.3.0/PKG-INFO
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/LICENSE` & `nautobot_device_lifecycle_mgmt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/README.md` & `nautobot_device_lifecycle_mgmt-1.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -33,14 +33,31 @@
 
 **Software Lifecycle Management List View**
 
 You can view the list of Software versions as well as filter the table.
 
 ![](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/lcm_software_list_view.png)
 
+**Software Lifecycle Reporting**
+
+Reports can be created from the Nautobot's software validation jobs **Device Software Validation - Report** or **Inventory Item Software Validation - Report**.
+
+![](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/lcm_software_validation_report_run_graph.png)
+
+Individual CSV files can be exported per platform or inventory item.
+
+![](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/lcm_software_validation_report_run_detailed_summary.png)
+
+Sample CSV.
+
+![](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/lcm_software_validation_report_csv_small.png)
+
+You can also view validation results as a list from the Nautobot GUI.
+
+![](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/lcm_software_validation_report_run_results_list.png)
 
 ## Try it out!
 
 This App is installed in the Nautobot Community Sandbox found over at [demo.nautobot.com](https://demo.nautobot.com/)!
 
 > For a full list of all the available always-on sandbox environments, head over to the main page on [networktocode.com](https://www.networktocode.com/nautobot/sandbox-environments/).
```

#### html2text {}

```diff
@@ -24,39 +24,52 @@
 Detail View** You can also click a Hardware/Software Notice and see the detail
 view. This view provides links to the devices that are part affected by this
 EoX notice due to their device type. ![](https://raw.githubusercontent.com/
 nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/
 lcm_hardware_detail_view.png) **Software Lifecycle Management List View** You
 can view the list of Software versions as well as filter the table. ![](https:/
 /raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/
-develop/docs/images/lcm_software_list_view.png) ## Try it out! This App is
-installed in the Nautobot Community Sandbox found over at [demo.nautobot.com]
-(https://demo.nautobot.com/)! > For a full list of all the available always-on
-sandbox environments, head over to the main page on [networktocode.com](https:/
-/www.networktocode.com/nautobot/sandbox-environments/). ## Documentation Full
-web-based HTML documentation for this app can be found over on the [Nautobot
-Docs](https://docs.nautobot.com) website: - [User Guide](https://
-docs.nautobot.com/projects/device-lifecycle/en/latest/user/app_overview/) -
-Overview, Using the App, Getting Started. - [Administrator Guide](https://
-docs.nautobot.com/projects/device-lifecycle/en/latest/admin/install/) - How to
-Install, Configure, Upgrade, or Uninstall the App. - [Developer Guide](https://
-docs.nautobot.com/projects/device-lifecycle/en/latest/dev/contributing/) -
-Extending the App, Code Reference, Contribution Guide. - [Release Notes /
-Changelog](https://docs.nautobot.com/projects/device-lifecycle/en/latest/admin/
-release_notes/). - [Frequently Asked Questions](https://docs.nautobot.com/
-projects/device-lifecycle/en/latest/user/faq/). ### Contributing to the Docs
-You can find all the Markdown source for the App documentation under the [docs]
-(https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/tree/
-develop/docs) folder in this repository. For simple edits, a Markdown capable
-editor is sufficient - clone the repository and edit away. If you need to view
-the fully generated documentation site, you can build it with [mkdocs](https://
-www.mkdocs.org/). A container hosting the docs will be started using the invoke
-commands (details in the [Development Environment Guide](https://
-docs.nautobot.com/projects/device-lifecycle/en/latest/dev/dev_environment/
-#docker-development-environment)) on [http://localhost:8001](http://localhost:
-8001). As your changes are saved, the live docs will be automatically reloaded.
-Any PRs with fixes or improvements are very welcome! ## Questions For any
-questions or comments, please check the [FAQ](https://docs.nautobot.com/
-projects/device-lifecycle/en/latest/user/faq/) first. Feel free to also swing
-by the [Network to Code Slack](https://networktocode.slack.com/) (channel
-`#nautobot`), sign up [here](http://slack.networktocode.com/) if you don't have
-an account.
+develop/docs/images/lcm_software_list_view.png) **Software Lifecycle
+Reporting** Reports can be created from the Nautobot's software validation jobs
+**Device Software Validation - Report** or **Inventory Item Software Validation
+- Report**. ![](https://raw.githubusercontent.com/nautobot/nautobot-plugin-
+device-lifecycle-mgmt/develop/docs/images/
+lcm_software_validation_report_run_graph.png) Individual CSV files can be
+exported per platform or inventory item. ![](https://raw.githubusercontent.com/
+nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/
+lcm_software_validation_report_run_detailed_summary.png) Sample CSV. ![](https:
+//raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/
+develop/docs/images/lcm_software_validation_report_csv_small.png) You can also
+view validation results as a list from the Nautobot GUI. ![](https://
+raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/
+develop/docs/images/lcm_software_validation_report_run_results_list.png) ## Try
+it out! This App is installed in the Nautobot Community Sandbox found over at
+[demo.nautobot.com](https://demo.nautobot.com/)! > For a full list of all the
+available always-on sandbox environments, head over to the main page on
+[networktocode.com](https://www.networktocode.com/nautobot/sandbox-
+environments/). ## Documentation Full web-based HTML documentation for this app
+can be found over on the [Nautobot Docs](https://docs.nautobot.com) website: -
+[User Guide](https://docs.nautobot.com/projects/device-lifecycle/en/latest/
+user/app_overview/) - Overview, Using the App, Getting Started. -
+[Administrator Guide](https://docs.nautobot.com/projects/device-lifecycle/en/
+latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall the
+App. - [Developer Guide](https://docs.nautobot.com/projects/device-lifecycle/
+en/latest/dev/contributing/) - Extending the App, Code Reference, Contribution
+Guide. - [Release Notes / Changelog](https://docs.nautobot.com/projects/device-
+lifecycle/en/latest/admin/release_notes/). - [Frequently Asked Questions]
+(https://docs.nautobot.com/projects/device-lifecycle/en/latest/user/faq/). ###
+Contributing to the Docs You can find all the Markdown source for the App
+documentation under the [docs](https://github.com/nautobot/nautobot-plugin-
+device-lifecycle-mgmt/tree/develop/docs) folder in this repository. For simple
+edits, a Markdown capable editor is sufficient - clone the repository and edit
+away. If you need to view the fully generated documentation site, you can build
+it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be
+started using the invoke commands (details in the [Development Environment
+Guide](https://docs.nautobot.com/projects/device-lifecycle/en/latest/dev/
+dev_environment/#docker-development-environment)) on [http://localhost:8001]
+(http://localhost:8001). As your changes are saved, the live docs will be
+automatically reloaded. Any PRs with fixes or improvements are very welcome! ##
+Questions For any questions or comments, please check the [FAQ](https://
+docs.nautobot.com/projects/device-lifecycle/en/latest/user/faq/) first. Feel
+free to also swing by the [Network to Code Slack](https://
+networktocode.slack.com/) (channel `#nautobot`), sign up [here](http://
+slack.networktocode.com/) if you don't have an account.
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/__init__.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/nested_serializers.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/nested_serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
             "url",
             "image_file_name",
             "device_types",
             "inventory_items",
             "object_tags",
             "download_url",
             "image_file_checksum",
+            "hashing_algorithm",
             "default_image",
         ]
 
 
 class NestedProviderLCMSerializer(WritableNestedSerializer):
     """Nested serializer for the provider class."""
 
@@ -54,16 +55,18 @@
 
         model = models.ProviderLCM
         fields = [
             "id",
             "name",
             "description",
             "physical_address",
+            "country",
             "phone",
             "email",
+            "portal_url",
             "comments",
         ]
 
 
 class NestedContractLCMSerializer(WritableNestedSerializer):
     """API serializer."""
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/serializers.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     ContractLCM,
     HardwareLCM,
     ProviderLCM,
     SoftwareImageLCM,
     SoftwareLCM,
     ValidatedSoftwareLCM,
     VulnerabilityLCM,
+    DeviceSoftwareValidationResult,
+    InventoryItemSoftwareValidationResult,
 )
 
 from .nested_serializers import (
     NestedContractLCMSerializer,
     NestedCVELCMSerializer,
     NestedProviderLCMSerializer,
     NestedSoftwareImageLCMSerializer,
@@ -97,16 +99,18 @@
         model = ProviderLCM
         fields = [
             "url",
             "id",
             "name",
             "description",
             "physical_address",
+            "country",
             "phone",
             "email",
+            "portal_url",
             "comments",
             "custom_fields",
             "tags",
         ]
 
 
 class ContractLCMSerializer(*serializer_base_classes):  # pylint: disable=R0901,too-few-public-methods
@@ -216,14 +220,15 @@
             "image_file_name",
             "software",
             "device_types",
             "inventory_items",
             "object_tags",
             "download_url",
             "image_file_checksum",
+            "hashing_algorithm",
             "default_image",
             "custom_fields",
             "tags",
         ]
 
 
 class ValidatedSoftwareLCMSerializer(*serializer_base_classes):  # pylint: disable=too-few-public-methods
@@ -320,7 +325,57 @@
             "display",
             "url",
             "cve",
             "software",
             "device",
             "inventory_item",
         ]
+
+
+class DeviceSoftwareValidationResultSerializer(*serializer_base_classes):  # pylint: disable=too-few-public-methods
+    """REST API serializer for DeviceSoftwareValidationResult records."""
+
+    url = serializers.HyperlinkedIdentityField(
+        view_name="plugins-api:nautobot_device_lifecycle_mgmt-api:devicesoftwarevalidationresult-detail"
+    )
+    device = NestedDeviceSerializer(read_only=True)
+    software = NestedSoftwareLCMSerializer(read_only=True)
+
+    class Meta:  # pylint: disable=too-few-public-methods
+        """Meta attributes."""
+
+        model = DeviceSoftwareValidationResult
+        fields = [
+            "device",
+            "software",
+            "is_validated",
+            "last_run",
+            "run_type",
+            "valid_software",
+            "url",
+        ]
+
+
+class InventoryItemSoftwareValidationResultSerializer(
+    *serializer_base_classes
+):  # pylint: disable=too-few-public-methods
+    """REST API serializer for InventoryItemSoftwareValidationResult records."""
+
+    url = serializers.HyperlinkedIdentityField(
+        view_name="plugins-api:nautobot_device_lifecycle_mgmt-api:inventoryitemsoftwarevalidationresult-detail"
+    )
+    inventory_item = NestedDeviceSerializer(read_only=True)
+    software = NestedSoftwareLCMSerializer(read_only=True)
+
+    class Meta:  # pylint: disable=too-few-public-methods
+        """Meta attributes."""
+
+        model = InventoryItemSoftwareValidationResult
+        fields = [
+            "inventory_item",
+            "software",
+            "is_validated",
+            "last_run",
+            "run_type",
+            "valid_software",
+            "url",
+        ]
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/urls.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/api/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,28 @@
     ProviderLCMView,
     ContactLCMView,
     SoftwareLCMViewSet,
     SoftwareImageLCMViewSet,
     ValidatedSoftwareLCMViewSet,
     CVELCMViewSet,
     VulnerabilityLCMViewSet,
+    DeviceSoftwareValidationResultListViewSet,
+    InventoryItemSoftwareValidationResultListViewSet,
 )
 
 router = routers.DefaultRouter()
 
 router.register(r"hardware", HardwareLCMView)
 router.register(r"contract", ContractLCMView)
 router.register(r"provider", ProviderLCMView)
 router.register(r"contact", ContactLCMView)
 router.register(r"software", SoftwareLCMViewSet)
 router.register(r"software-image", SoftwareImageLCMViewSet)
 router.register(r"validated-software", ValidatedSoftwareLCMViewSet)
 router.register(r"cve", CVELCMViewSet)
 router.register(r"vulnerability", VulnerabilityLCMViewSet)
+router.register(r"device-validated-software-result", DeviceSoftwareValidationResultListViewSet)
+router.register(r"inventory-item-validated-software-result", InventoryItemSoftwareValidationResultListViewSet)
 
 app_name = "nautobot_device_lifecycle_mgmt"
 
 urlpatterns = router.urls
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/choices.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/const.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/const.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/filters.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Filtering implementation for the Lifecycle Management plugin."""
 import datetime
 
 import django_filters
 from django.db.models import Q
-from nautobot.dcim.models import Device, DeviceRole, DeviceType, InventoryItem, Platform, Region, Site
+from nautobot.dcim.models import Device, DeviceRole, DeviceType, InventoryItem, Platform, Region, Site, Manufacturer
 from nautobot.extras.filters import StatusFilter, StatusModelFilterSetMixin, TagFilter
 from nautobot.extras.models import Tag
 
 try:
     from nautobot.extras.filters import NautobotFilterSet
 except ImportError:
     # TODO: Remove once plugin no longer supports Nautobot < 1.4.0
@@ -212,14 +212,15 @@
         model = SoftwareImageLCM
 
         fields = [
             "image_file_name",
             "software",
             "software_version",
             "image_file_checksum",
+            "hashing_algorithm",
             "download_url",
             "device_types",
             "inventory_items",
             "object_tags",
             "default_image",
         ]
 
@@ -419,14 +420,23 @@
 
     software = django_filters.ModelMultipleChoiceFilter(
         field_name="software__version",
         to_field_name="version",
         queryset=SoftwareLCM.objects.all(),
         label="Software",
     )
+    valid = django_filters.BooleanFilter(
+        label="Valid",
+        field_name="is_validated",
+    )
+    platform = django_filters.ModelMultipleChoiceFilter(
+        field_name="device__platform",
+        queryset=Platform.objects.all(),
+        label="Platform",
+    )
     site_id = django_filters.ModelMultipleChoiceFilter(
         field_name="device__site",
         queryset=Site.objects.all(),
         label="Site",
     )
     site = django_filters.ModelMultipleChoiceFilter(
         field_name="device__site__slug",
@@ -478,28 +488,34 @@
         to_field_name="slug",
         label="Device Role (slug)",
     )
     exclude_sw_missing = django_filters.BooleanFilter(
         method="_exclude_sw_missing",
         label="Exclude missing software",
     )
+    sw_missing_only = django_filters.BooleanFilter(
+        method="_sw_missing_only",
+        label="Show only missing software",
+    )
 
     class Meta:
         """Meta attributes for filter."""
 
         model = DeviceSoftwareValidationResult
 
         fields = [
             "software",
+            "platform",
             "site",
             "region",
             "device",
             "device_type",
             "device_role",
             "exclude_sw_missing",
+            "sw_missing_only",
         ]
 
     def search(self, queryset, name, value):  # pylint: disable=unused-argument, no-self-use
         """Perform the filtered search."""
         if not value.strip():
             return queryset
         qs_filter = Q(device__name__icontains=value) | Q(software__version__icontains=value)
@@ -508,26 +524,42 @@
     def _exclude_sw_missing(self, queryset, name, value):  # pylint: disable=unused-argument, no-self-use
         """Exclude devices with missing software."""
         if value:
             return queryset.filter(~Q(software=None))
 
         return queryset
 
+    def _sw_missing_only(self, queryset, name, value):  # pylint: disable=unused-argument, no-self-use
+        """Only show devices with missing software."""
+        if value:
+            return queryset.filter(Q(software=None))
+
+        return queryset
+
 
 class InventoryItemSoftwareValidationResultFilterSet(NautobotFilterSet):
     """Filter for InventoryItemSoftwareValidationResult."""
 
     q = django_filters.CharFilter(method="search", label="Search")
 
     software = django_filters.ModelMultipleChoiceFilter(
         field_name="software__version",
         to_field_name="version",
         queryset=SoftwareLCM.objects.all(),
         label="Software",
     )
+    valid = django_filters.BooleanFilter(
+        label="Valid",
+        field_name="is_validated",
+    )
+    manufacturer = django_filters.ModelMultipleChoiceFilter(
+        field_name="inventory_item__manufacturer",
+        queryset=Manufacturer.objects.all(),
+        label="Manufacturer",
+    )
     site_id = django_filters.ModelMultipleChoiceFilter(
         field_name="inventory_item__device__site",
         queryset=Site.objects.all(),
         label="Site",
     )
     site = django_filters.ModelMultipleChoiceFilter(
         field_name="inventory_item__device__site__slug",
@@ -591,30 +623,36 @@
         to_field_name="slug",
         label="Device Role (slug)",
     )
     exclude_sw_missing = django_filters.BooleanFilter(
         method="_exclude_sw_missing",
         label="Exclude missing software",
     )
+    sw_missing_only = django_filters.BooleanFilter(
+        method="_sw_missing_only",
+        label="Show only missing software",
+    )
 
     class Meta:
         """Meta attributes for filter."""
 
         model = InventoryItemSoftwareValidationResult
 
         fields = [
             "software",
+            "manufacturer",
             "site",
             "region",
             "inventory_item",
             "part_id",
             "device",
             "device_type",
             "device_role",
             "exclude_sw_missing",
+            "sw_missing_only",
         ]
 
     def search(self, queryset, name, value):  # pylint: disable=unused-argument, no-self-use
         """Perform the filtered search."""
         if not value.strip():
             return queryset
         qs_filter = (
@@ -634,14 +672,21 @@
     def _exclude_sw_missing(self, queryset, name, value):  # pylint: disable=unused-argument, no-self-use
         """Exclude devices with missing software."""
         if value:
             return queryset.filter(~Q(software=None))
 
         return queryset
 
+    def _sw_missing_only(self, queryset, name, value):  # pylint: disable=unused-argument, no-self-use
+        """Only show devices with missing software."""
+        if value:
+            return queryset.filter(Q(software=None))
+
+        return queryset
+
 
 class ContractLCMFilterSet(NautobotFilterSet):
     """Filter for ContractLCMFilter."""
 
     q = django_filters.CharFilter(method="search", label="Search")
 
     provider = django_filters.ModelMultipleChoiceFilter(
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/forms.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Forms implementation for the Lifecycle Management plugin."""
 import logging
 from django import forms
 from django.db.models import Q
 
-from nautobot.dcim.models import Device, DeviceRole, DeviceType, InventoryItem, Platform, Region, Site
+from nautobot.dcim.models import Device, DeviceRole, DeviceType, InventoryItem, Platform, Region, Site, Manufacturer
 from nautobot.extras.forms import (
     CustomFieldModelCSVForm,
     CustomFieldModelForm,
     CustomFieldFilterForm,
     CustomFieldBulkEditForm,
     RelationshipModelForm,
     StatusBulkEditFormMixin,
@@ -365,24 +365,29 @@
     )
     object_tags = DynamicModelMultipleChoiceField(
         queryset=Tag.objects.all(),
         to_field_name="slug",
         required=False,
     )
     default_image = forms.BooleanField(required=False, widget=StaticSelect2(choices=BOOLEAN_WITH_BLANK_CHOICES))
+    hashing_algorithm = forms.CharField(
+        required=False,
+        label="Hashing Algorithm",
+    )
 
     class Meta:
         """Meta attributes."""
 
         model = SoftwareImageLCM
         fields = [
             "q",
             "software",
             "image_file_name",
             "image_file_checksum",
+            "hashing_algorithm",
             "download_url",
             "device_types",
             "inventory_items",
             "object_tags",
             "default_image",
         ]
 
@@ -534,14 +539,24 @@
         label="Search",
     )
     software = DynamicModelMultipleChoiceField(
         queryset=SoftwareLCM.objects.all(),
         to_field_name="version",
         required=False,
     )
+    platform = DynamicModelMultipleChoiceField(
+        queryset=Platform.objects.all(),
+        label="Platform",
+        required=False,
+    )
+    valid = forms.BooleanField(
+        required=False,
+        widget=StaticSelect2(choices=BOOLEAN_WITH_BLANK_CHOICES),
+        label="Valid",
+    )
     site = DynamicModelMultipleChoiceField(
         queryset=Site.objects.all(),
         to_field_name="slug",
         required=False,
     )
     region = DynamicModelMultipleChoiceField(
         queryset=Region.objects.all(),
@@ -564,34 +579,61 @@
         required=False,
     )
     exclude_sw_missing = forms.BooleanField(
         required=False,
         widget=StaticSelect2(choices=BOOLEAN_WITH_BLANK_CHOICES),
         label="Exclude missing software",
     )
+    sw_missing_only = forms.BooleanField(
+        required=False,
+        widget=StaticSelect2(choices=BOOLEAN_WITH_BLANK_CHOICES),
+        label="Show only missing software",
+    )
 
     class Meta:
         """Meta attributes."""
 
         model = DeviceSoftwareValidationResult
-        fields = ["q", "software", "site", "region", "device", "device_type", "device_role", "exclude_sw_missing"]
+        fields = [
+            "q",
+            "software",
+            "valid",
+            "platform",
+            "site",
+            "region",
+            "device",
+            "device_type",
+            "device_role",
+            "exclude_sw_missing",
+            "sw_missing_only",
+        ]
 
 
 class InventoryItemSoftwareValidationResultFilterForm(BootstrapMixin, CustomFieldModelForm, RelationshipModelForm):
     """Filter form to filter searches for InventoryItemSoftwareValidationResult."""
 
     q = forms.CharField(
         required=False,
         label="Search",
     )
     software = DynamicModelMultipleChoiceField(
         queryset=SoftwareLCM.objects.all(),
         to_field_name="version",
         required=False,
     )
+    valid = forms.BooleanField(
+        required=False,
+        widget=StaticSelect2(choices=BOOLEAN_WITH_BLANK_CHOICES),
+        label="Valid",
+    )
+    manufacturer = DynamicModelMultipleChoiceField(
+        queryset=Manufacturer.objects.all(),
+        label="Manufacturer",
+        required=False,
+    )
     site = DynamicModelMultipleChoiceField(
         queryset=Site.objects.all(),
         to_field_name="slug",
         required=False,
     )
     region = DynamicModelMultipleChoiceField(
         queryset=Region.objects.all(),
@@ -623,30 +665,38 @@
         required=False,
     )
     exclude_sw_missing = forms.BooleanField(
         required=False,
         widget=StaticSelect2(choices=BOOLEAN_WITH_BLANK_CHOICES),
         label="Exclude missing software",
     )
+    sw_missing_only = forms.BooleanField(
+        required=False,
+        widget=StaticSelect2(choices=BOOLEAN_WITH_BLANK_CHOICES),
+        label="Show only missing software",
+    )
 
     class Meta:
         """Meta attributes."""
 
         model = InventoryItemSoftwareValidationResult
         fields = [
             "q",
             "software",
+            "valid",
+            "manufacturer",
             "site",
             "region",
             "inventory_item",
             "part_id",
             "device",
             "device_type",
             "device_role",
             "exclude_sw_missing",
+            "sw_missing_only",
         ]
 
 
 class ValidatedSoftwareLCMCSVForm(CustomFieldModelCSVForm):
     """Form for bulk creating ValidatedSoftwareLCM objects."""
 
     devices = CSVMultipleModelChoiceField(
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/graphql/types.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/graphql/types.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from nautobot.dcim.models import Device, InventoryItem
 from nautobot.extras.jobs import Job
 
 from nautobot_device_lifecycle_mgmt import choices
 from nautobot_device_lifecycle_mgmt.models import (
     DeviceSoftwareValidationResult,
     InventoryItemSoftwareValidationResult,
+    ValidatedSoftwareLCM,
 )
 from nautobot_device_lifecycle_mgmt.software import DeviceSoftware, InventoryItemSoftware
 
 
 name = "Device/Software Lifecycle Reporting"  # pylint: disable=invalid-name
 
 
@@ -33,14 +34,15 @@
         job_run_time = datetime.now()
 
         for device in devices:
             device_software = DeviceSoftware(device)
 
             validate_obj, _ = DeviceSoftwareValidationResult.objects.get_or_create(device=device)
             validate_obj.is_validated = device_software.validate_software()
+            validate_obj.valid_software.set(ValidatedSoftwareLCM.objects.get_for_object(device))
             validate_obj.software = device_software.software
             validate_obj.last_run = job_run_time
             validate_obj.run_type = choices.ReportRunTypeChoices.REPORT_FULL_RUN
             validate_obj.validated_save()
         self.log_success(message=f"Performed validation on: {devices.count()} devices.")
 
 
@@ -62,13 +64,14 @@
         job_run_time = datetime.now()
 
         for inventoryitem in inventory_items:
             inventoryitem_software = InventoryItemSoftware(inventoryitem)
 
             validate_obj, _ = InventoryItemSoftwareValidationResult.objects.get_or_create(inventory_item=inventoryitem)
             validate_obj.is_validated = inventoryitem_software.validate_software()
+            validate_obj.valid_software.set(ValidatedSoftwareLCM.objects.get_for_object(inventoryitem))
             validate_obj.software = inventoryitem_software.software
             validate_obj.last_run = job_run_time
             validate_obj.run_type = choices.ReportRunTypeChoices.REPORT_FULL_RUN
             validate_obj.validated_save()
 
         self.log_success(message=f"Performed validation on: {inventory_items.count()} inventory items.")
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/models.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,24 +272,26 @@
         to="SoftwareLCM", on_delete=models.CASCADE, related_name="software_images", verbose_name="Software Version"
     )
     device_types = models.ManyToManyField(to="dcim.DeviceType", related_name="+", blank=True)
     inventory_items = models.ManyToManyField(to="dcim.InventoryItem", related_name="+", blank=True)
     object_tags = models.ManyToManyField(to="extras.Tag", related_name="+", blank=True)
     download_url = models.URLField(blank=True, verbose_name="Download URL")
     image_file_checksum = models.CharField(blank=True, max_length=256, verbose_name="Image File Checksum")
+    hashing_algorithm = models.CharField(default="", blank=True, max_length=32, verbose_name="Hashing Algorithm")
     default_image = models.BooleanField(verbose_name="Default Image", default=False)
 
     csv_headers = [
         "image_file_name",
         "software",
         "device_types",
         "inventory_items",
         "object_tags",
         "download_url",
         "image_file_checksum",
+        "hashing_algorithm",
         "default_image",
     ]
 
     class Meta:
         """Meta attributes for SoftwareImageLCM."""
 
         verbose_name = "Software Image"
@@ -311,14 +313,15 @@
             self.image_file_name,
             self.software.id,
             ",".join(str(device_type["model"]) for device_type in self.device_types.values()),
             ",".join(str(inventory_item["id"]) for inventory_item in self.inventory_items.values()),
             ",".join(str(object_tag["slug"]) for object_tag in self.object_tags.values()),
             self.download_url,
             self.image_file_checksum,
+            self.hashing_algorithm,
             self.default_image,
         )
 
     objects = SoftwareImageLCMQuerySet.as_manager()
 
 
 class ValidatedSoftwareLCMQuerySet(RestrictedQuerySet):
@@ -447,24 +450,51 @@
     )
     software = models.ForeignKey(
         to="SoftwareLCM", on_delete=models.CASCADE, help_text="Device software", null=True, blank=True, related_name="+"
     )
     is_validated = models.BooleanField(null=True, blank=True)
     last_run = models.DateTimeField(null=True, blank=True)
     run_type = models.CharField(max_length=50, choices=choices.ReportRunTypeChoices)
+    valid_software = models.ManyToManyField(
+        to="ValidatedSoftwareLCM", related_name="device_software_validation_results"
+    )
+
+    csv_headers = [
+        "device",
+        "software",
+        "valid",
+        "last_run",
+        "run_type",
+        "approved_software",
+    ]
 
     class Meta:
         """Meta attributes for DeviceSoftwareValidationResult."""
 
         verbose_name = "Device Software Validation Report"
         ordering = ("device",)
 
+    def __str__(self):
+        """String representation of DeviceSoftwareValidationResult."""
+        if self.is_validated:
+            msg = f"Device: {self.device} - Valid"
+        else:
+            msg = f"Device: {self.device} - Not Valid"
+        return msg
+
     def to_csv(self):
         """Indicates model fields to return as csv."""
-        return (self.device.name, self.software.version, self.is_validated, self.last_run, self.run_type)
+        return (
+            self.device.name,
+            self.software if self.software else "None",
+            str(self.is_validated),
+            self.last_run.strftime("%Y-%m-%d %H:%M:%S") if self.last_run else "-",
+            self.run_type,
+            ",".join(str(valid.software) for valid in ValidatedSoftwareLCM.objects.get_for_object(self.device)),
+        )
 
 
 @extras_features(
     "graphql",
 )
 class InventoryItemSoftwareValidationResult(PrimaryModel):
     """InventoryItem Software validation details model."""
@@ -477,24 +507,43 @@
     )
     software = models.ForeignKey(
         to="SoftwareLCM", on_delete=models.CASCADE, help_text="Inventory Item software", blank=True, null=True
     )
     is_validated = models.BooleanField(null=True, blank=True)
     last_run = models.DateTimeField(null=True, blank=True)
     run_type = models.CharField(max_length=50, choices=choices.ReportRunTypeChoices)
+    valid_software = models.ManyToManyField(
+        to="ValidatedSoftwareLCM", related_name="inventory_item_software_validation_results"
+    )
+
+    csv_headers = [
+        "inventory_item",
+        "software",
+        "valid",
+        "last_run",
+        "run_type",
+        "approved_software",
+    ]
 
     class Meta:
         """Meta attributes for InventoryItemSoftwareValidationResult."""
 
         verbose_name = "Inventory Item Software Validation Report"
         ordering = ("inventory_item",)
 
     def to_csv(self):
         """Indicates model fields to return as csv."""
-        return (self.inventory_item.name, self.software.version, self.is_validated, self.last_run, self.run_type)
+        return (
+            self.inventory_item.part_id,
+            self.software if self.software else "None",
+            str(self.is_validated),
+            self.last_run.strftime("%Y-%m-%d %H:%M:%S") if self.last_run else "-",
+            self.run_type,
+            ",".join(str(valid.software) for valid in ValidatedSoftwareLCM.objects.get_for_object(self.inventory_item)),
+        )
 
 
 @extras_features(
     "custom_fields",
     "custom_links",
     "custom_validators",
     "export_templates",
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/navigation.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,24 +244,38 @@
             ),
             NavMenuGroup(
                 name="Reports",
                 weight=100,
                 items=(
                     NavMenuItem(
                         link="plugins:nautobot_device_lifecycle_mgmt:validatedsoftware_device_report",
-                        name="Device Software Validation",
+                        name="Device Software Validation - Report",
                         permissions=[
                             "nautobot_device_lifecycle_mgmt.view_validatedsoftwarelcm",
                         ],
                     ),
                     NavMenuItem(
+                        link="plugins:nautobot_device_lifecycle_mgmt:devicesoftwarevalidationresult_list",
+                        name="Device Software Validation - List",
+                        permissions=[
+                            "nautobot_device_lifecycle_mgmt.view_devicesoftwarevalidationresult",
+                        ],
+                    ),
+                    NavMenuItem(
                         link="plugins:nautobot_device_lifecycle_mgmt:validatedsoftware_inventoryitem_report",
-                        name="Inventory Item Software Validation",
+                        name="Inventory Item Software Validation - Report",
                         permissions=[
                             "nautobot_device_lifecycle_mgmt.view_validatedsoftwarelcm",
                         ],
                     ),
+                    NavMenuItem(
+                        link="plugins:nautobot_device_lifecycle_mgmt:inventoryitemsoftwarevalidationresult_list",
+                        name="Inventory Item Software Validation - List",
+                        permissions=[
+                            "nautobot_device_lifecycle_mgmt.view_inventoryitemsoftwarevalidationresult",
+                        ],
+                    ),
                 ),
             ),
         ),
     ),
 )
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/signals.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/software.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/software.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/software_filters.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/software_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/template_content.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,18 @@
                 </td>
             </tr>
             <tr>
                 <td>Country</td>
                 <td>{{ object.country|placeholder }}</td>
             </tr>
             <tr>
+                <td>Portal URL</td>
+                <td><a href="{{ object.portal_url }}">{{ object.portal_url }}</a></td>
+            </tr>
+            <tr>
                 <td>Comments</td>
                 <td>
                     {% if object.comments %}
                     <pre>{{ object.comments }}</pre>
                     {% else %} &mdash; {% endif %}
                 </td>
             </tr>
```

#### html2text {}

```diff
@@ -7,14 +7,15 @@
 Description {{ object.description|placeholder }}
 E-Mail      {% if object.email %} {{_object.email_}}{% else %} — {% endif %}
 Phone       {{ object.phone|placeholder }}
             {% if object.physical_address %}
 Address      Map_it
             {{ object.physical_address|linebreaksbr }} {% else %} — {% endif %}
 Country     {{ object.country|placeholder }}
+Portal URL  {{_object.portal_url_}}
             {% if object.comments %}
 Comments    {{ object.comments }}
             {% else %} — {% endif %}
 {% endblock %} {% block content_right_page %} {% if contracts.count > 0 %}
 Service Contracts
 Name          Start Date                 End Date                 Support Level          Type
 {             {                          {                        {                      {
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,24 @@
                     <p class="break-word">{{ object.image_file_checksum }}</p>
                 {% else %}
                     <span class="text-muted"></span>&mdash;</span>
                 {% endif %}
                 </td>
             </tr>
             <tr>
+                <td>Hashing Algorithm</td>
+                <td>
+                {% if object.hashing_algorithm %}
+                    <p class="break-word">{{ object.hashing_algorithm }}</p>
+                {% else %}
+                    <span class="text-muted"></span>&mdash;</span>
+                {% endif %}
+                </td>
+            </tr>
+            <tr>
                 <td>Default Image</td>
                 <td>
                 {% if object.default_image is True %}
                     <span class="text-success"><i class="mdi mdi-check-bold"></i></span>
                 {% else %}
                     <span class="text-danger"><i class="mdi mdi-close"></i></span>
                 {% endif %}
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
 {% extends 'generic/object_detail.html' %} {% block masthead %}
 ***** {% block title %}{{ object }}{% endblock %} *****
 {% endblock masthead %} {% block content_left_page %}
 Software Image
-Software {{_object.software_}}
+Software  {{_object.software_}}
 Version
-Image
-File     {{ object.image_file_name }}
-Name
-Download {% if object.download_url %} {{_object.download_url_}} {% else %} — {% endif
-URL      %}
-Image    {% if object.image_file_checksum %}
-File     {{ object.image_file_checksum }}
-Checksum {% else %} — {% endif %}
-Default  {% if object.default_image is True %}  {% else %}  {% endif %}
+Image     {{ object.image_file_name }}
+File Name
+Download  {% if object.download_url %} {{_object.download_url_}} {% else %} — {% endif
+URL       %}
+Image     {% if object.image_file_checksum %}
+File      {{ object.image_file_checksum }}
+Checksum  {% else %} — {% endif %}
+Hashing   {% if object.hashing_algorithm %}
+Algorithm {{ object.hashing_algorithm }}
+          {% else %} — {% endif %}
+Default   {% if object.default_image is True %}  {% else %}  {% endif %}
 Image
 {% endblock %} {% block content_right_page %}
 Device assignments
              {% if object.device_types.all %}
                  * {% for device_type in object.device_types.all %}
 Device Types     * {{_device_type_}}
                  * {% endfor %}
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     <div class="panel panel-default">
         <div class="panel-heading"><strong>Attributes</strong></div>
         <div class="panel-body">
             {% render_field form.image_file_name %}
             {% render_field form.software %}
             {% render_field form.download_url %}
             {% render_field form.image_file_checksum %}
+            {% render_field form.hashing_algorithm %}
             {% render_field form.default_image %}
         </div>
     </div>
     <div class="panel panel-default">
         <div class="panel-heading"><strong>Objects Assigned To</strong></div>
         <div class="panel-body">
             <ul class="nav nav-tabs" role="tablist">
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% extends 'generic/object_edit.html' %} {% load static %} {% load form_helpers
 %} {% load helpers %} {% block form %} {% block pre_form %}{% endblock %}
 Attributes
 {% render_field form.image_file_name %} {% render_field form.software %} {%
 render_field form.download_url %} {% render_field form.image_file_checksum %}
-{% render_field form.default_image %}
+{% render_field form.hashing_algorithm %} {% render_field form.default_image %}
 Objects Assigned To
     * Device_Types
     * Inventory_Items
     * Object_Tags
 {% render_field form.device_types %}
 {% render_field form.inventory_items %}
 {% render_field form.object_tags %}
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html`

 * *Files 20% similar despite different names*

```diff
@@ -46,28 +46,56 @@
                         <th><a>Type</a></th>
                         <th><a>Total</a></th>
                         <th><a>Valid</a></th>
                         <th><a>Invalid</a></th>
                         <th><a>No Software</a></th>
                         <th><a>Compliance (%)</a></th>
                         <th><a>Summary</a></th>
+                        <th><a>Export Data</a></th>
                     </tr>
                 </thead>
                 <tbody>
                     <tr class="even">
-                        <td>Devices</td>
-                        <td>{% if device_aggr.total is not None %} {{ device_aggr.total }} {% else %} -- {% endif %}</td>
-                        <td>{% if device_aggr.valid is not None %} {{ device_aggr.valid }} {% else %} -- {% endif %}</td>
-                        <td>{% if device_aggr.invalid is not None %} {{ device_aggr.invalid }} {% else %} -- {% endif %}</td>
-                        <td>{% if device_aggr.no_software is not None %} {{ device_aggr.no_software }} {% else %} -- {% endif %}</td>
+                        <td>
+                            <a href="/plugins/nautobot-device-lifecycle-mgmt/device-validated-software-result/">
+                                Devices
+                            </a>
+                        </td>
+                        <td>
+                            <a href="/plugins/nautobot-device-lifecycle-mgmt/device-validated-software-result/">
+                                {% if device_aggr.total is not None %} {{ device_aggr.total }} {% else %} -- {% endif %}
+                            </a>
+                        </td>
+                        <td>
+                            <a href="/plugins/nautobot-device-lifecycle-mgmt/device-validated-software-result/?&valid=True">
+                                {% if device_aggr.valid is not None %} {{ device_aggr.valid }} {% else %} -- {% endif %}
+                            </a>
+                        </td>
+                        <td>
+                            <a href="/plugins/nautobot-device-lifecycle-mgmt/device-validated-software-result/?&valid=False">
+                                {% if device_aggr.invalid is not None %} {{ device_aggr.invalid }} {% else %} -- {% endif %}
+                            </a>
+                        </td>
+                        <td>
+                            <a href="/plugins/nautobot-device-lifecycle-mgmt/device-validated-software-result/?&sw_missing_only=True">
+                                {% if device_aggr.no_software is not None %} {{ device_aggr.no_software }} {% else %} -- {% endif %}
+                            </a>
+                        </td>
                         <td>{% if device_aggr.valid_percent is not None %} {{ device_aggr.valid_percent }} % {% else %} -- {% endif %}</td>
-                        <td><a target="_blank" href="data:image/png;base64,{{ device_visual|safe }}" title="Devices Pie Chart">
+                        <td>
+                            <a target="_blank" href="data:image/png;base64,{{ device_visual|safe }}" title="Devices Pie Chart">
                             <img style="width:150px;" src="data:image/png;base64,{{ device_visual|safe }}" alt="Devices Pie Chart">
                             </a>
                         </td>
+                        <td>
+                            <a href="/plugins/nautobot-device-lifecycle-mgmt/device-validated-software-result/?export" 
+                                class="btn btn-default btn-xs" title="Export data for all device types" aria-hidden="true"> 
+                                <i class="mdi mdi-download"></i>
+                            </a>
+                        </td>
                     </tr>
                 </tbody>
             </table>
             <h3 class="text-center m-2 p-3">Device Type Summary</h3>
             {% include 'utilities/obj_table.html' %}
             </div>
         <div class="col-md-3 noprint">
```

#### html2text {}

```diff
@@ -13,21 +13,22 @@
 *** Last full run of the report: {{ report_last_run }} - {
 { report_last_run|timesince }} ago ***
 {% endif %} {% if bar_chart is not None %} {% block graphic %}
 [Platform Bar Chart]
 {% endblock %} {% else %} -- Oops, no config validation found, visual not made!
 -- {% endif %}
 **** Executive Summary ****
-Type    Total             Valid             Invalid             No Software             Compliance (%)            Summary
-        {% if             {% if             {% if               {% if                   {% if
+Type    Total             Valid             Invalid             No Software             Compliance (%)            Summary  Export
+                                                                                                                           Data
+        {%_if             {%_if             {%_if               {%_if                   {% if
         device_aggr.total device_aggr.valid device_aggr.invalid device_aggr.no_software device_aggr.valid_percent
-        is not None %} {  is not None %} {  is not None %} {    is not None %} {        is not None %} {          [Devices
+        is_not_None_%}_{  is_not_None_%}_{  is_not_None_%}_{    is_not_None_%}_{        is not None %} {          [Devices
 Devices {                 {                 {                   {                       {                         Pie
         device_aggr.total device_aggr.valid device_aggr.invalid device_aggr.no_software device_aggr.valid_percent Chart]
-        }} {% else %} --  }} {% else %} --  }} {% else %} -- {% }} {% else %} -- {%     }} % {% else %} -- {%
-        {% endif %}       {% endif %}       endif %}            endif %}                endif %}
+        }}_{%_else_%}_--_ }}_{%_else_%}_--_ }}_{%_else_%}_--_{% }}_{%_else_%}_--_{%     }} % {% else %} -- {%
+        {%_endif_%}       {%_endif_%}       endif_%}            endif_%}                endif %}
 **** Device Type Summary ****
 {% include 'utilities/obj_table.html' %}
 {% include 'inc/search_panel.html' %}
 {% table_config_form table table_name="ObjectTable" %} {% endblock %} {% block
 javascript %}
  {% endblock %}
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html`

 * *Files 27% similar despite different names*

```diff
@@ -47,28 +47,55 @@
                         <th><a>Type</a></th>
                         <th><a>Total</a></th>
                         <th><a>Valid</a></th>
                         <th><a>Invalid</a></th>
                         <th><a>No Software</a></th>
                         <th><a>Validation (%)</a></th>
                         <th><a>Summary</a></th>
+                        <th><a>Export Data</a></th>
                     </tr>
                 </thead>
                 <tbody>
                     <tr class="even">
-                        <td>Inventory Items</td>
-                        <td>{% if inventory_aggr.total is not None %} {{ inventory_aggr.total }} {% else %} -- {% endif %}</td>
-                        <td>{% if inventory_aggr.valid is not None %} {{ inventory_aggr.valid }} {% else %} -- {% endif %}</td>
-                        <td>{% if inventory_aggr.invalid is not None %} {{ inventory_aggr.invalid }} {% else %} -- {% endif %}</td>
-                        <td>{% if inventory_aggr.no_software is not None %} {{ inventory_aggr.no_software }} {% else %} -- {% endif %}</td>
+                        <td>
+                            <a href="/plugins/nautobot-device-lifecycle-mgmt/inventory-item-validated-software-result/">
+                                Inventory Items
+                            </a>
+                        </td>
+                        <td>
+                            <a href="/plugins/nautobot-device-lifecycle-mgmt/inventory-item-validated-software-result/">
+                                {% if inventory_aggr.total is not None %} {{ inventory_aggr.total }} {% else %} -- {% endif %}
+                            </a>
+                        </td>
+                        <td>
+                            <a href="/plugins/nautobot-device-lifecycle-mgmt/inventory-item-validated-software-result/?&valid=True">
+                                {% if inventory_aggr.valid is not None %} {{ inventory_aggr.valid }} {% else %} -- {% endif %}
+                            </a>
+                        </td>
+                        <td>
+                            <a href="/plugins/nautobot-device-lifecycle-mgmt/inventory-item-validated-software-result/?&valid=False">
+                                {% if inventory_aggr.invalid is not None %} {{ inventory_aggr.invalid }} {% else %} -- {% endif %}
+                            </a>
+                        </td>
+                        <td>
+                            <a href="/plugins/nautobot-device-lifecycle-mgmt/inventory-item-validated-software-result/?&sw_missing_only=True">
+                                {% if inventory_aggr.no_software is not None %} {{ inventory_aggr.no_software }} {% else %} -- {% endif %}
+                            </a>
+                        </td>
                         <td>{% if inventory_aggr.valid_percent is not None %} {{ inventory_aggr.valid_percent }} % {% else %} -- {% endif %}</td>
                         <td><a target="_blank" href="data:image/png;base64,{{ inventory_visual|safe }}" title="Inventory Pie Chart">
                             <img style="width:150px;" src="data:image/png;base64,{{ inventory_visual|safe }}" alt="Inventory Pie Chart">
                             </a>
                         </td>
+                        <td>
+                            <a href="/plugins/nautobot-device-lifecycle-mgmt/inventory-item-validated-software-result/?export" 
+                                class="btn btn-default btn-xs" title="Export data for all inventory items" aria-hidden="true"> 
+                                <i class="mdi mdi-download"></i>
+                            </a>
+                        </td>
                     </tr>
                 </tbody>
             </table>
             <h3 class="text-center m-2 p-3">Inventory Item Part ID Summary</h3>
             {% include 'utilities/obj_table.html' %}
             </div>
         <div class="col-md-3 noprint">
```

#### html2text {}

```diff
@@ -14,21 +14,22 @@
 *** Last full run of the report: {{ report_last_run }} - {
 { report_last_run|timesince }} ago ***
 {% endif %} {% if bar_chart is not None %} {% block graphic %}
 [Platform Bar Chart]
 {% endblock %} {% else %} -- Oops, no config validation found, visual not made!
 -- {% endif %}
 **** Executive Summary ****
-Type      Total                Valid                Invalid                No Software                Validation (%)               Summary
-          {% if                {% if                {% if                  {% if                      {% if
+Type      Total                Valid                Invalid                No Software                Validation (%)               Summary    Export
+                                                                                                                                              Data
+          {%_if                {%_if                {%_if                  {%_if                      {% if
           inventory_aggr.total inventory_aggr.valid inventory_aggr.invalid inventory_aggr.no_software inventory_aggr.valid_percent
-Inventory is not None %} {     is not None %} {     is not None %} {       is not None %} {           is not None %} {             [Inventory
+Inventory is_not_None_%}_{     is_not_None_%}_{     is_not_None_%}_{       is_not_None_%}_{           is not None %} {             [Inventory
 Items     {                    {                    {                      {                          {                            Pie_Chart]
           inventory_aggr.total inventory_aggr.valid inventory_aggr.invalid inventory_aggr.no_software inventory_aggr.valid_percent
-          }} {% else %} -- {%  }} {% else %} -- {%  }} {% else %} -- {%    }} {% else %} -- {% endif  }} % {% else %} -- {% endif
-          endif %}             endif %}             endif %}               %}                         %}
+          }}_{%_else_%}_--_{%  }}_{%_else_%}_--_{%  }}_{%_else_%}_--_{%    }}_{%_else_%}_--_{%_endif  }} % {% else %} -- {% endif
+          endif_%}             endif_%}             endif_%}               %}                         %}
 **** Inventory Item Part ID Summary ****
 {% include 'utilities/obj_table.html' %}
 {% include 'inc/search_panel.html' %}
 {% table_config_form table table_name="ObjectTable" %} {% endblock %} {% block
 javascript %}
  {% endblock %}
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/conftest.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Params for testing."""
+from datetime import date
 from nautobot.dcim.models import DeviceType, Manufacturer, Platform, Site, Device, DeviceRole, InventoryItem
 from nautobot.extras.models import Status
 
-from nautobot_device_lifecycle_mgmt.models import CVELCM, SoftwareLCM
+from nautobot_device_lifecycle_mgmt.models import CVELCM, SoftwareLCM, ValidatedSoftwareLCM
 
 
 def create_devices():
     """Create devices for tests."""
     device_platform, _ = Platform.objects.get_or_create(name="Cisco IOS", slug="cisco_ios")
     manufacturer, _ = Manufacturer.objects.get_or_create(slug="cisco")
     device_type = DeviceType.objects.create(manufacturer=manufacturer, model="6509-E", slug="6509-e")
@@ -102,7 +103,45 @@
         SoftwareLCM.objects.create(device_platform=device_platform_ios, version="15.1(2)M"),
         SoftwareLCM.objects.create(device_platform=device_platform_ios, version="4.22.9M"),
         SoftwareLCM.objects.create(device_platform=device_platform_ios, version="21.4R3"),
         SoftwareLCM.objects.create(device_platform=device_platform_eos, version="4.17.1M"),
         SoftwareLCM.objects.create(device_platform=device_platform_eos, version="4.25.1F"),
     )
     return softwares
+
+
+def create_validated_softwares():
+    """Create ValidatedSoftwareLCM"""
+    manufacturer, _ = Manufacturer.objects.get_or_create(slug="cisco")
+    device_platform_ios, _ = Platform.objects.get_or_create(name="Cisco IOS", slug="cisco_ios")
+    device_type = DeviceType.objects.create(manufacturer=manufacturer, model="ASR-1000", slug="asr-1000")
+    software_one = SoftwareLCM.objects.create(
+        device_platform=device_platform_ios,
+        version="17.3.3 MD",
+        release_date="2019-01-10",
+    )
+    validatedsoftwarelcm = ValidatedSoftwareLCM(
+        software=software_one,
+        start=date(2019, 1, 10),
+    )
+    validatedsoftwarelcm.device_types.set([device_type])
+    validatedsoftwarelcm.save()
+    software_two = SoftwareLCM.objects.create(
+        device_platform=device_platform_ios,
+        version="20.0.0 MD",
+        release_date="2019-01-10",
+    )
+    validatedsoftwarelcm_two = ValidatedSoftwareLCM(
+        software=software_two,
+        start=date(2019, 1, 10),
+    )
+    validatedsoftwarelcm_two.device_types.set([device_type])
+    validatedsoftwarelcm_two.save()
+
+    validated_items = (
+        software_one,
+        software_two,
+        validatedsoftwarelcm,
+        validatedsoftwarelcm_two,
+    )
+
+    return validated_items
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_api.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -533,14 +533,15 @@
 
     model = SoftwareImageLCM
     brief_fields = [
         "default_image",
         "device_types",
         "display",
         "download_url",
+        "hashing_algorithm",
         "id",
         "image_file_checksum",
         "image_file_name",
         "inventory_items",
         "object_tags",
         "url",
     ]
@@ -670,7 +671,105 @@
         """Currently don't support bulk operations."""
 
     def test_bulk_update_objects(self):
         """Currently don't support bulk operations."""
 
     def test_notes_url_on_object(self):
         """Currently don't support notes."""
+
+
+class ProviderLCMAPITest(APIViewTestCases.APIViewTestCase):
+    """Test the ProviderLCMLCM API."""
+
+    model = ProviderLCM
+    brief_fields = [
+        "name",
+        "description",
+        "physical_address",
+        "phone",
+        "email",
+        "portal_url",
+        "comments",
+    ]
+
+    @classmethod
+    def setUpTestData(cls):
+        """Create a Provider for API calls."""
+
+        cls.create_data = [
+            {
+                "name": "Arista",
+                "description": "Arista Support",
+                "physical_address": "123 Arista Way, San Jose, CA",
+                "country": "USA",
+                "phone": "(123) 456-7890",
+                "email": "email@Arista.com",
+                "portal_url": "https://www.Arista.com/",
+                "comments": "Test Comment",
+            },
+            {
+                "name": "Erricson",
+                "description": "Erricson Support",
+                "physical_address": "123 Erricson Way, San Jose, CA",
+                "country": "USA",
+                "phone": "(123) 456-7890",
+                "email": "email@Erricson.com",
+                "portal_url": "https://www.Erricson.com/",
+                "comments": "Test Comment",
+            },
+            {
+                "name": "Linksys",
+                "description": "Linksys Support",
+                "physical_address": "123 Linksys Way, San Jose, CA",
+                "country": "USA",
+                "phone": "(123) 456-7890",
+                "email": "email@Linksys.com",
+                "portal_url": "https://www.Linksys.com/",
+                "comments": "Test Comment",
+            },
+        ]
+
+        ProviderLCM.objects.create(
+            name="Cisco",
+            description="Cisco Support",
+            physical_address="123 Cisco Way, San Jose, CA",
+            country="USA",
+            phone="(123) 456-7890",
+            email="email@cisco.com",
+            portal_url="https://www.cisco.com/",
+            comments="Test Comment",
+        )
+        ProviderLCM.objects.create(
+            name="HP",
+            description="HP Support",
+            physical_address="123 HP Way, San Jose, CA",
+            country="USA",
+            phone="(123) 456-0000",
+            email="email@HP.com",
+            portal_url="https://www.HP.com/",
+            comments="Test Comment",
+        )
+        ProviderLCM.objects.create(
+            name="Juniper",
+            description="Juniper Support",
+            physical_address="123 Juniper Way, San Jose, CA",
+            country="USA",
+            phone="(123) 456-5890",
+            email="email@Juniper.com",
+            portal_url="https://www.Juniper.com/",
+            comments="Test Comment",
+        )
+
+    def test_bulk_create_objects(self):
+        """Currently don't support bulk operations."""
+
+    def test_bulk_delete_objects(self):
+        """Currently don't support bulk operations."""
+
+    def test_bulk_update_objects(self):
+        """Currently don't support bulk operations."""
+
+    def test_notes_url_on_object(self):
+        """Currently don't support notes."""
+
+    def test_list_objects_brief(self):
+        """Nautobot 1.4 adds 'created' and 'last_updated' causing testing mismatch with previous versions."""
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_basic.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_filters.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,14 +382,24 @@
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
     def test_sw_missing(self):
         """Test sw_missing filter."""
         params = {"exclude_sw_missing": True}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
+    def test_platform(self):
+        """Test software version filter."""
+        params = {"platform": [self.platform]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 3)
+
+    def test_sw_missing_only(self):
+        """Test sw_missing filter."""
+        params = {"sw_missing_only": True}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 1)
+
 
 class InventoryItemSoftwareValidationResultFilterSetTestCase(TestCase):
     """Tests for the DeviceSoftwareValidationResult model."""
 
     queryset = InventoryItemSoftwareValidationResult.objects.all()
     filterset = InventoryItemSoftwareValidationResultFilterSet
 
@@ -462,14 +472,24 @@
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
     def test_sw_missing(self):
         """Test sw_missing filter."""
         params = {"exclude_sw_missing": True}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
+    def test_platform(self):
+        """Test software version filter."""
+        params = {"platform": [self.platform]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 3)
+
+    def test_sw_missing_only(self):
+        """Test sw_missing filter."""
+        params = {"sw_missing_only": True}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 1)
+
 
 class CVELCMTestCase(TestCase):
     """Tests for CVELCMFilter."""
 
     queryset = CVELCM.objects.all()
     filterset = CVELCMFilterSet
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_forms.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_model.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,16 +16,24 @@
     InventoryItemSoftwareValidationResult,
     SoftwareLCM,
     ValidatedSoftwareLCM,
     DeviceSoftwareValidationResult,
     CVELCM,
     VulnerabilityLCM,
     SoftwareImageLCM,
+    ProviderLCM,
+    ContractLCM,
+)
+from .conftest import (
+    create_devices,
+    create_inventory_items,
+    create_cves,
+    create_softwares,
+    create_validated_softwares,
 )
-from .conftest import create_devices, create_inventory_items, create_cves, create_softwares
 
 
 class HardwareLCMTestCase(TestCase):
     """Tests for the HardwareLCM models."""
 
     def setUp(self):
         """Set up base objects."""
@@ -257,65 +265,116 @@
             self.assertEqual(validatedsoftwarelcm_start_end.valid, False)
 
         with time_machine.travel(date_start_valid):
             self.assertEqual(validatedsoftwarelcm_start_only.valid, True)
             self.assertEqual(validatedsoftwarelcm_start_end.valid, True)
 
 
-class DeviceSoftwareValidationResultTestCase(TestCase):
+class DeviceSoftwareValidationResultTestCase(TestCase):  # pylint: disable=too-many-instance-attributes
     """Tests for the DeviceSoftwareValidationResult model."""
 
     def setUp(self):
         """Set up test objects."""
         self.device = create_devices()[0]
         self.platform = Platform.objects.all().first()
-        self.software = SoftwareLCM.objects.create(
-            device_platform=self.platform,
-            version="17.3.3 MD",
-            release_date="2019-01-10",
-        )
+        (
+            self.software_one,
+            self.software_two,
+            self.validatedsoftwarelcm,
+            self.validatedsoftwarelcm_two,
+        ) = create_validated_softwares()
+        self.validated_software_qs = ValidatedSoftwareLCM.objects.get_for_object(self.validatedsoftwarelcm)
+        self.validated_software_qs_two = ValidatedSoftwareLCM.objects.get_for_object(self.validatedsoftwarelcm_two)
 
     def test_create_devicesoftwarevalidationresult(self):
         """Successfully create SoftwareLCM with required fields only."""
         validation_result = DeviceSoftwareValidationResult.objects.create(
             device=self.device,
-            software=self.software,
+            software=self.software_one,
             is_validated=True,
         )
 
         self.assertEqual(validation_result.device, self.device)
-        self.assertEqual(validation_result.software, self.software)
+        self.assertEqual(validation_result.software, self.software_one)
         self.assertEqual(validation_result.is_validated, True)
 
+    def test_create_devicesoftwarevalidationresult_one_valid_software(self):
+        """Successfully create DeviceSoftwareValidationResult with one valid software."""
+        validation_result = DeviceSoftwareValidationResult.objects.create(
+            device=self.device,
+            software=self.software_one,
+            is_validated=True,
+        )
+        validation_result.valid_software.set(self.validated_software_qs)
+        self.assertEqual(validation_result.valid_software.values()[0]["software_id"], self.software_one.id)
+
+    def test_create_devicesoftwarevalidationresult_two_valid_softwares(self):
+        """Successfully create DeviceSoftwareValidationResult with two valid software."""
+        validation_result = DeviceSoftwareValidationResult.objects.create(
+            device=self.device,
+            software=self.software_one,
+            is_validated=True,
+        )
+        validation_result.valid_software.set(self.validated_software_qs)
+        validation_result.valid_software.set(self.validated_software_qs_two)
+        self.assertEqual(validation_result.valid_software.values()[0]["software_id"], self.software_one.id)
+        self.assertEqual(validation_result.valid_software.values()[1]["software_id"], self.software_two.id)
 
-class InventoryItemSoftwareValidationResultTestCase(TestCase):
+
+class InventoryItemSoftwareValidationResultTestCase(TestCase):  # pylint: disable=too-many-instance-attributes
     """Tests for the DeviceSoftwareValidationResult model."""
 
     def setUp(self):
         """Set up test objects."""
         self.inventory_item = create_inventory_items()[0]
         self.platform = Platform.objects.all().first()
-        self.software = SoftwareLCM.objects.create(
-            device_platform=self.platform,
-            version="17.3.3 MD",
-            release_date="2019-01-10",
-        )
+        self.platform = Platform.objects.all().first()
+        (
+            self.software_one,
+            self.software_two,
+            self.validatedsoftwarelcm,
+            self.validatedsoftwarelcm_two,
+        ) = create_validated_softwares()
+        self.validated_software_qs = ValidatedSoftwareLCM.objects.get_for_object(self.validatedsoftwarelcm)
+        self.validated_software_qs_two = ValidatedSoftwareLCM.objects.get_for_object(self.validatedsoftwarelcm_two)
 
-    def test_create_devicesoftwarevalidationresult(self):
+    def test_create_itemsoftwarevalidationresult(self):
         """Successfully create SoftwareLCM with required fields only."""
         validation_result = InventoryItemSoftwareValidationResult.objects.create(
             inventory_item=self.inventory_item,
-            software=self.software,
+            software=self.software_one,
             is_validated=True,
         )
 
         self.assertEqual(validation_result.inventory_item, self.inventory_item)
-        self.assertEqual(validation_result.software, self.software)
+        self.assertEqual(validation_result.software, self.software_one)
         self.assertEqual(validation_result.is_validated, True)
 
+    def test_create_itemsoftwarevalidationresult_one_valid_software(self):
+        """Successfully create InventoryItemSoftwareValidationResult with one valid software."""
+        validation_result = InventoryItemSoftwareValidationResult.objects.create(
+            inventory_item=self.inventory_item,
+            software=self.software_one,
+            is_validated=True,
+        )
+        validation_result.valid_software.set(self.validated_software_qs)
+        self.assertEqual(validation_result.valid_software.values()[0]["software_id"], self.software_one.id)
+
+    def test_create_itemsoftwarevalidationresult_two_valid_softwares(self):
+        """Successfully create InventoryItemSoftwareValidationResult with two valid software."""
+        validation_result = InventoryItemSoftwareValidationResult.objects.create(
+            inventory_item=self.inventory_item,
+            software=self.software_one,
+            is_validated=True,
+        )
+        validation_result.valid_software.set(self.validated_software_qs)
+        validation_result.valid_software.set(self.validated_software_qs_two)
+        self.assertEqual(validation_result.valid_software.values()[0]["software_id"], self.software_one.id)
+        self.assertEqual(validation_result.valid_software.values()[1]["software_id"], self.software_two.id)
+
 
 class CVELCMTestCase(TestCase):
     """Tests for the CVELCM model."""
 
     def setUp(self):
         """Set up the test objects."""
         self.device_platform = Platform.objects.create(name="Cisco IOS", slug="cisco_ios")
@@ -505,7 +564,65 @@
         validatedsoftwarelcm_start_only = ValidatedSoftwareLCM(
             software=self.software,
             start=date(2020, 4, 15),
             preferred=False,
         )
         validatedsoftwarelcm_start_only.device_types.set([self.device_type_1])
         validatedsoftwarelcm_start_only.save()
+
+
+class ProviderLCMTestCase(TestCase):
+    """Tests for the HardwareLCM models."""
+
+    def test_provider_creation(self):
+        provider = ProviderLCM.objects.create(
+            name="Cisco",
+            description="Cisco Support",
+            physical_address="123 Cisco Way, San Jose, CA",
+            country="USA",
+            phone="(123) 456-7890",
+            email="email@cisco.com",
+            portal_url="https://www.cisco.com/",
+            comments="Test Comment",
+        )
+        self.assertEqual(provider.name, "Cisco")
+        self.assertEqual(provider.description, "Cisco Support")
+        self.assertEqual(provider.physical_address, "123 Cisco Way, San Jose, CA")
+        self.assertEqual(provider.country, "USA")
+        self.assertEqual(provider.phone, "(123) 456-7890")
+        self.assertEqual(provider.email, "email@cisco.com")
+        self.assertEqual(provider.portal_url, "https://www.cisco.com/")
+        self.assertEqual(provider.comments, "Test Comment")
+
+    def test_provider_assignment(self):
+        ProviderLCM.objects.create(
+            name="Cisco",
+            description="Cisco Support",
+            physical_address="123 Cisco Way, San Jose, CA",
+            country="USA",
+            phone="(123) 456-7890",
+            email="email@cisco.com",
+            portal_url="https://www.cisco.com/",
+            comments="Test Comment",
+        )
+        cisco_contract = ContractLCM.objects.create(
+            provider=ProviderLCM.objects.get(name="Cisco"),
+            name="Cisco Contract",
+            number="888-8888",
+            start=date(2020, 4, 1),
+            end=date(2025, 4, 15),
+            cost=10.00,
+            support_level="Tier 1",
+            currency="USD",
+            contract_type="Hardware",
+            comments="Cisco gave us discount",
+        )
+        self.assertEqual(cisco_contract.provider, ProviderLCM.objects.get(name="Cisco"))
+        self.assertEqual(cisco_contract.name, "Cisco Contract")
+        self.assertEqual(cisco_contract.number, "888-8888")
+        self.assertEqual(str(cisco_contract.start), "2020-04-01")
+        self.assertEqual(str(cisco_contract.end), "2025-04-15")
+        self.assertEqual(cisco_contract.cost, 10.00)
+        self.assertEqual(cisco_contract.support_level, "Tier 1")
+        self.assertEqual(cisco_contract.currency, "USD")
+        self.assertEqual(cisco_contract.contract_type, "Hardware")
+        self.assertEqual(cisco_contract.comments, "Cisco gave us discount")
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_views.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/tests/test_views.py`

 * *Files 21% similar despite different names*

```diff
@@ -124,14 +124,18 @@
 
     def test_list_objects_unknown_filter_no_strict_filtering(self):
         pass
 
     def test_list_objects_with_permission(self):
         pass
 
+    # Disable Temp until we get headers fixed for csv
+    def test_queryset_to_csv(self):
+        pass
+
 
 class ValidatedSoftwareInventoryItemReportViewTest(ViewTestCases.ListObjectsViewTestCase):
     """Test ValidatedSoftwareInventoryItemReportView"""
 
     model = InventoryItemSoftwareValidationResult
 
     def _get_base_url(self):
@@ -189,14 +193,18 @@
 
     def test_list_objects_unknown_filter_no_strict_filtering(self):
         pass
 
     def test_list_objects_with_permission(self):
         pass
 
+    # Disable Temp until we get headers fixed for csv
+    def test_queryset_to_csv(self):
+        pass
+
 
 class CVELCMViewTest(ViewTestCases.PrimaryObjectViewTestCase):
     """Test the CVELCM views."""
 
     model = CVELCM
     bulk_edit_data = {"description": "Bulk edit views"}
 
@@ -337,14 +345,169 @@
         )
 
     def test_bulk_edit_objects_with_constrained_permission(self):
         pass
 
     def test_bulk_edit_objects_with_permission(self):
         pass
+
+    def test_bulk_edit_objects_without_permission(self):
+        pass
+
+    def test_bulk_edit_form_contains_all_pks(self):
+        pass
+
+    def test_has_advanced_tab(self):
+        pass
+
+    def test_get_object_notes(self):
+        pass
+
+    def test_bulk_import_objects_with_permission_csv_file(self):
+        pass
+
+    def test_list_objects_with_permission(self):
+        pass
+
+
+class DeviceSoftwareValidationResultListViewTest(ViewTestCases.ListObjectsViewTestCase):
+    """Test DeviceSoftwareValidationResultListView"""
+
+    model = DeviceSoftwareValidationResult
+
+    def _get_base_url(self):
+        return "plugins:nautobot_device_lifecycle_mgmt:devicesoftwarevalidationresult_list"
+
+    @classmethod
+    def setUpTestData(cls):
+        """Set up test objects."""
+        device_1, device_2, _ = create_devices()
+        DeviceSoftwareValidationResult.objects.create(
+            device=device_1,
+            software=None,
+            is_validated=False,
+        )
+        DeviceSoftwareValidationResult.objects.create(
+            device=device_2,
+            software=None,
+            is_validated=False,
+        )
+
+    def test_device_software_list_view_without_permission(self):
+        """Test the SoftwareReportOverview."""
+
+        self.assertHttpStatus(
+            self.client.get(
+                reverse(
+                    "plugins:nautobot_device_lifecycle_mgmt:devicesoftwarevalidationresult_list",
+                )
+            ),
+            403,
+        )
+
+    def test_device_software_list_view_with_permission(self):
+        """Test the SoftwareReportOverview."""
+        obj_perm = ObjectPermission(name="Test permission", actions=["view"])
+        obj_perm.save()
+        obj_perm.users.add(self.user)
+        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        self.assertHttpStatus(
+            self.client.get(
+                reverse(
+                    "plugins:nautobot_device_lifecycle_mgmt:devicesoftwarevalidationresult_list",
+                )
+            ),
+            200,
+        )
+
+    def test_bulk_edit_objects_with_constrained_permission(self):
+        pass
+
+    def test_bulk_edit_objects_with_permission(self):
+        pass
+
+    def test_bulk_edit_objects_without_permission(self):
+        pass
+
+    def test_bulk_edit_form_contains_all_pks(self):
+        pass
+
+    def test_has_advanced_tab(self):
+        pass
+
+    def test_get_object_notes(self):
+        pass
+
+    def test_bulk_import_objects_with_permission_csv_file(self):
+        pass
+
+    def test_list_objects_with_permission(self):
+        pass
+
+
+class InventoryItemSoftwareValidationResultListViewTest(ViewTestCases.ListObjectsViewTestCase):
+    """Test InventoryItemSoftwareValidationResultListView"""
+
+    model = InventoryItemSoftwareValidationResult
+
+    def _get_base_url(self):
+        return "plugins:nautobot_device_lifecycle_mgmt:inventoryitemsoftwarevalidationresult_list"
+
+    @classmethod
+    def setUpTestData(cls):
+        """Set up test objects."""
+        inventory_items = create_inventory_items()
+        InventoryItemSoftwareValidationResult.objects.create(
+            inventory_item=inventory_items[0],
+            software=None,
+            is_validated=False,
+        )
+        InventoryItemSoftwareValidationResult.objects.create(
+            inventory_item=inventory_items[1],
+            software=None,
+            is_validated=False,
+        )
+        InventoryItemSoftwareValidationResult.objects.create(
+            inventory_item=inventory_items[2],
+            software=None,
+            is_validated=False,
+        )
+
+    def test_inventoryitem_software_list_view_without_permission(self):
+        """Test the SoftwareReportOverview."""
+
+        self.assertHttpStatus(
+            self.client.get(
+                reverse(
+                    "plugins:nautobot_device_lifecycle_mgmt:inventoryitemsoftwarevalidationresult_list",
+                )
+            ),
+            403,
+        )
+
+    def test_inventoryitem_software_list_view_with_permission(self):
+        """Test the SoftwareReportOverview."""
+        obj_perm = ObjectPermission(name="Test permission", actions=["view"])
+        obj_perm.save()
+        obj_perm.users.add(self.user)
+        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        self.assertHttpStatus(
+            self.client.get(
+                reverse(
+                    "plugins:nautobot_device_lifecycle_mgmt:inventoryitemsoftwarevalidationresult_list",
+                )
+            ),
+            200,
+        )
+
+    def test_bulk_edit_objects_with_constrained_permission(self):
+        pass
+
+    def test_bulk_edit_objects_with_permission(self):
+        pass
 
     def test_bulk_edit_objects_without_permission(self):
         pass
 
     def test_bulk_edit_form_contains_all_pks(self):
         pass
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/urls.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/urls.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Django urlpatterns declaration for the Lifecycle Management plugin."""
 from django.urls import path
-from nautobot.extras.views import ObjectChangeLogView
+from nautobot.extras.views import ObjectChangeLogView, ObjectNotesView
 from nautobot_device_lifecycle_mgmt import views
 from nautobot_device_lifecycle_mgmt.models import (
     HardwareLCM,
     SoftwareImageLCM,
     SoftwareLCM,
     ValidatedSoftwareLCM,
     ContractLCM,
@@ -26,27 +26,39 @@
     path("hardware/<uuid:pk>/edit/", views.HardwareLCMEditView.as_view(), name="hardwarelcm_edit"),
     path(
         "hardware/<uuid:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="hardwarelcm_changelog",
         kwargs={"model": HardwareLCM},
     ),
+    path(
+        "hardware/<uuid:pk>/notes/",
+        ObjectNotesView.as_view(),
+        name="hardwarelcm_notes",
+        kwargs={"model": HardwareLCM},
+    ),
     path("hardware/import/", views.HardwareLCMBulkImportView.as_view(), name="hardwarelcm_import"),
     # Software Lifecycle Management URLs
     path("software/", views.SoftwareLCMListView.as_view(), name="softwarelcm_list"),
     path("software/<uuid:pk>/", views.SoftwareLCMView.as_view(), name="softwarelcm"),
     path("software/add/", views.SoftwareLCMCreateView.as_view(), name="softwarelcm_add"),
     path("software/<uuid:pk>/delete/", views.SoftwareLCMDeleteView.as_view(), name="softwarelcm_delete"),
     path("software/<uuid:pk>/edit/", views.SoftwareLCMEditView.as_view(), name="softwarelcm_edit"),
     path(
         "software/<uuid:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="softwarelcm_changelog",
         kwargs={"model": SoftwareLCM},
     ),
+    path(
+        "software/<uuid:pk>/notes/",
+        ObjectNotesView.as_view(),
+        name="softwarelcm_notes",
+        kwargs={"model": SoftwareLCM},
+    ),
     path("software/import/", views.SoftwareLCMBulkImportView.as_view(), name="softwarelcm_import"),
     path(
         "software/<uuid:pk>/software-images/",
         views.SoftwareSoftwareImagesLCMView.as_view(),
         name="software_software_images",
     ),
     # SoftwareImage
@@ -61,14 +73,20 @@
     path(
         "software-image/<uuid:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="softwareimagelcm_changelog",
         kwargs={"model": SoftwareImageLCM},
     ),
     path(
+        "software-image/<uuid:pk>/notes/",
+        ObjectNotesView.as_view(),
+        name="softwareimagelcm_notes",
+        kwargs={"model": SoftwareImageLCM},
+    ),
+    path(
         "software-image/import/",
         views.SoftwareImageLCMBulkImportView.as_view(),
         name="softwareimagelcm_import",
     ),
     # ValidatedSoftware
     path("validated-software/", views.ValidatedSoftwareLCMListView.as_view(), name="validatedsoftwarelcm_list"),
     path("validated-software/<uuid:pk>/", views.ValidatedSoftwareLCMView.as_view(), name="validatedsoftwarelcm"),
@@ -86,42 +104,66 @@
     path(
         "validated-software/<uuid:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="validatedsoftwarelcm_changelog",
         kwargs={"model": ValidatedSoftwareLCM},
     ),
     path(
+        "validated-software/<uuid:pk>/notes/",
+        ObjectNotesView.as_view(),
+        name="validatedsoftwarelcm_notes",
+        kwargs={"model": ValidatedSoftwareLCM},
+    ),
+    path(
         "validated-software/import/",
         views.ValidatedSoftwareLCMBulkImportView.as_view(),
         name="validatedsoftwarelcm_import",
     ),
     path(
         "validated-software/device-report/",
         views.ValidatedSoftwareDeviceReportView.as_view(),
         name="validatedsoftware_device_report",
     ),
     path(
         "validated-software/inventoryitem-report/",
         views.ValidatedSoftwareInventoryItemReportView.as_view(),
         name="validatedsoftware_inventoryitem_report",
     ),
+    # DeviceValidatedSoftwareResult
+    path(
+        "device-validated-software-result/",
+        views.DeviceSoftwareValidationResultListView.as_view(),
+        name="devicesoftwarevalidationresult_list",
+    ),
+    # InventoryItemValidatedSoftwareResult
+    path(
+        "inventory-item-validated-software-result/",
+        views.InventoryItemSoftwareValidationResultListView.as_view(),
+        name="inventoryitemsoftwarevalidationresult_list",
+    ),
     # Contract Lifecycle Management URLs
     path("contract/", views.ContractLCMListView.as_view(), name="contractlcm_list"),
     path("contract/<uuid:pk>/", views.ContractLCMView.as_view(), name="contractlcm"),
     path("contract/add/", views.ContractLCMCreateView.as_view(), name="contractlcm_add"),
     path("contract/delete/", views.ContractLCMBulkDeleteView.as_view(), name="contractlcm_bulk_delete"),
     path("contract/edit/", views.ContractLCMBulkEditView.as_view(), name="contractlcm_bulk_edit"),
     path("contract/<uuid:pk>/delete/", views.ContractLCMDeleteView.as_view(), name="contractlcm_delete"),
     path("contract/<uuid:pk>/edit/", views.ContractLCMEditView.as_view(), name="contractlcm_edit"),
     path(
         "contract/<uuid:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="contractlcm_changelog",
         kwargs={"model": ContractLCM},
     ),
+    path(
+        "contract/<uuid:pk>/notes/",
+        ObjectNotesView.as_view(),
+        name="contractlcm_notes",
+        kwargs={"model": ContractLCM},
+    ),
     path("contract/import/", views.ContractLCMBulkImportView.as_view(), name="contractlcm_import"),
     # Contract Provider Lifecycle Management URLs
     path("provider/", views.ProviderLCMListView.as_view(), name="providerlcm_list"),
     path("provider/<uuid:pk>/", views.ProviderLCMView.as_view(), name="providerlcm"),
     path("provider/add/", views.ProviderLCMCreateView.as_view(), name="providerlcm_add"),
     path("provider/delete/", views.ProviderLCMBulkDeleteView.as_view(), name="providerlcm_bulk_delete"),
     path("provider/edit/", views.ProviderLCMBulkEditView.as_view(), name="providerlcm_bulk_edit"),
@@ -129,14 +171,20 @@
     path("provider/<uuid:pk>/edit/", views.ProviderLCMEditView.as_view(), name="providerlcm_edit"),
     path(
         "provider/<uuid:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="providerlcm_changelog",
         kwargs={"model": ProviderLCM},
     ),
+    path(
+        "provider/<uuid:pk>/notes/",
+        ObjectNotesView.as_view(),
+        name="providerlcm_notes",
+        kwargs={"model": ProviderLCM},
+    ),
     path("provider/import/", views.ProviderLCMBulkImportView.as_view(), name="providerlcm_import"),
     # Contract Resources Lifecycle Management URLs
     path("contact/", views.ContactLCMListView.as_view(), name="contactlcm_list"),
     path("contact/<uuid:pk>/", views.ContactLCMView.as_view(), name="contactlcm"),
     path("contact/add/", views.ContactLCMCreateView.as_view(), name="contactlcm_add"),
     path("contact/delete/", views.ContactLCMBulkDeleteView.as_view(), name="contactlcm_bulk_delete"),
     path("contact/edit/", views.ContactLCMBulkEditView.as_view(), name="contactlcm_bulk_edit"),
@@ -144,14 +192,20 @@
     path("contact/<uuid:pk>/edit/", views.ContactLCMEditView.as_view(), name="contactlcm_edit"),
     path(
         "contact/<uuid:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="contactlcm_changelog",
         kwargs={"model": ContactLCM},
     ),
+    path(
+        "contact/<uuid:pk>/notes/",
+        ObjectNotesView.as_view(),
+        name="contactlcm_notes",
+        kwargs={"model": ContactLCM},
+    ),
     path("contact/import/", views.ContactLCMBulkImportView.as_view(), name="contactlcm_import"),
     # CVE Lifecycle Management URLs
     path("cve/", views.CVELCMListView.as_view(), name="cvelcm_list"),
     path("cve/<uuid:pk>/", views.CVELCMView.as_view(), name="cvelcm"),
     path("cve/add/", views.CVELCMCreateView.as_view(), name="cvelcm_add"),
     path("cve/delete/", views.CVELCMBulkDeleteView.as_view(), name="cvelcm_bulk_delete"),
     path("cve/edit/", views.CVELCMBulkEditView.as_view(), name="cvelcm_bulk_edit"),
@@ -159,22 +213,34 @@
     path("cve/<uuid:pk>/edit/", views.CVELCMEditView.as_view(), name="cvelcm_edit"),
     path(
         "cve/<uuid:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="cvelcm_changelog",
         kwargs={"model": CVELCM},
     ),
+    path(
+        "cve/<uuid:pk>/notes/",
+        ObjectNotesView.as_view(),
+        name="cvelcm_notes",
+        kwargs={"model": CVELCM},
+    ),
     path("cve/import/", views.CVELCMBulkImportView.as_view(), name="cvelcm_import"),
     # Vulnerability Lifecycle Management URLs
     path("vulnerability/", views.VulnerabilityLCMListView.as_view(), name="vulnerabilitylcm_list"),
     path("vulnerability/<uuid:pk>/", views.VulnerabilityLCMView.as_view(), name="vulnerabilitylcm"),
     path("vulnerability/delete/", views.VulnerabilityLCMBulkDeleteView.as_view(), name="vulnerabilitylcm_bulk_delete"),
     path("vulnerability/edit/", views.VulnerabilityLCMBulkEditView.as_view(), name="vulnerabilitylcm_bulk_edit"),
     path("vulnerability/<uuid:pk>/delete/", views.VulnerabilityLCMDeleteView.as_view(), name="vulnerabilitylcm_delete"),
     path("vulnerability/<uuid:pk>/edit/", views.VulnerabilityLCMEditView.as_view(), name="vulnerabilitylcm_edit"),
     path(
         "vulnerability/<uuid:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="vulnerabilitylcm_changelog",
         kwargs={"model": VulnerabilityLCM},
     ),
+    path(
+        "vulnerability/<uuid:pk>/notes/",
+        ObjectNotesView.as_view(),
+        name="vulnerabilitylcm_notes",
+        kwargs={"model": VulnerabilityLCM},
+    ),
 ]
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/views.py` & `nautobot_device_lifecycle_mgmt-1.3.0/nautobot_device_lifecycle_mgmt/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,17 @@
     SoftwareImageLCM,
 )
 from nautobot_device_lifecycle_mgmt.tables import (
     HardwareLCMTable,
     SoftwareLCMTable,
     ValidatedSoftwareLCMTable,
     DeviceSoftwareValidationResultTable,
+    DeviceSoftwareValidationResultListTable,
     InventoryItemSoftwareValidationResultTable,
+    InventoryItemSoftwareValidationResultListTable,
     ContractLCMTable,
     ProviderLCMTable,
     ContactLCMTable,
     CVELCMTable,
     VulnerabilityLCMTable,
     SoftwareImageLCMTable,
 )
@@ -570,15 +572,15 @@
     """View for executive report on software Validation."""
 
     filterset = DeviceSoftwareValidationResultFilterSet
     filterset_form = DeviceSoftwareValidationResultFilterForm
     table = DeviceSoftwareValidationResultTable
     template_name = "nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html"
     queryset = (
-        DeviceSoftwareValidationResult.objects.values("device__device_type__model")
+        DeviceSoftwareValidationResult.objects.values("device__device_type__model", "device__device_type__pk")
         .distinct()
         .annotate(
             total=Count("device__device_type__model"),
             valid=Count("device__device_type__model", filter=Q(is_validated=True)),
             invalid=Count("device__device_type__model", filter=Q(is_validated=False) & ~Q(software=None)),
             no_software=Count("device__device_type__model", filter=Q(software=None)),
             valid_percent=ExpressionWrapper(100 * F("valid") / (F("total")), output_field=FloatField()),
@@ -694,23 +696,34 @@
             csv_data.append(
                 ",".join([f"{str(val)} %" if key == "valid_percent" else str(val) for key, val in obj.items()])
             )
 
         return "\n".join(csv_data)
 
 
+class DeviceSoftwareValidationResultListView(generic.ObjectListView):
+    """DeviceSoftawareValidationResult List view."""
+
+    queryset = DeviceSoftwareValidationResult.objects.all()
+    filterset = DeviceSoftwareValidationResultFilterSet
+    filterset_form = DeviceSoftwareValidationResultFilterForm
+    table = DeviceSoftwareValidationResultListTable
+    action_buttons = ("export",)
+    template_name = "nautobot_device_lifecycle_mgmt/devicesoftwarevalidationresult_list.html"
+
+
 class ValidatedSoftwareInventoryItemReportView(generic.ObjectListView):
     """View for executive report on inventory item software validation."""
 
     filterset = InventoryItemSoftwareValidationResultFilterSet
     filterset_form = InventoryItemSoftwareValidationResultFilterForm
     table = InventoryItemSoftwareValidationResultTable
     template_name = "nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html"
     queryset = (
-        InventoryItemSoftwareValidationResult.objects.values("inventory_item__part_id")
+        InventoryItemSoftwareValidationResult.objects.values("inventory_item__part_id", "inventory_item__pk")
         .distinct()
         .annotate(
             total=Count("inventory_item__part_id"),
             valid=Count("inventory_item__part_id", filter=Q(is_validated=True)),
             invalid=Count("inventory_item__part_id", filter=Q(is_validated=False) & ~Q(software=None)),
             no_software=Count("inventory_item__part_id", filter=Q(software=None)),
             valid_percent=ExpressionWrapper(100 * F("valid") / (F("total")), output_field=FloatField()),
@@ -829,14 +842,25 @@
             csv_data.append(
                 ",".join([f"{str(val)} %" if key == "valid_percent" else str(val) for key, val in obj.items()])
             )
 
         return "\n".join(csv_data)
 
 
+class InventoryItemSoftwareValidationResultListView(generic.ObjectListView):
+    """DeviceSoftawareValidationResult List view."""
+
+    queryset = InventoryItemSoftwareValidationResult.objects.all()
+    filterset = InventoryItemSoftwareValidationResultFilterSet
+    filterset_form = InventoryItemSoftwareValidationResultFilterForm
+    table = InventoryItemSoftwareValidationResultListTable
+    action_buttons = ("export",)
+    template_name = "nautobot_device_lifecycle_mgmt/inventoryitemsoftwarevalidationresult_list.html"
+
+
 # ---------------------------------------------------------------------------------
 #  Contract Lifecycle Management Views
 # ---------------------------------------------------------------------------------
 
 
 class ContractLCMListView(generic.ObjectListView):
     """List view."""
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/pyproject.toml` & `nautobot_device_lifecycle_mgmt-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-device-lifecycle-mgmt"
-version = "v1.2.0"
+version = "v1.3.0"
 description = "Manages device lifecycles for platforms and software."
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt"
 repository = "https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt"
 keywords = ["nautobot", "nautobot-plugin"]
```

### Comparing `nautobot_device_lifecycle_mgmt-1.2.0/PKG-INFO` & `nautobot_device_lifecycle_mgmt-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-device-lifecycle-mgmt
-Version: 1.2.0
+Version: 1.3.0
 Summary: Manages device lifecycles for platforms and software.
 Home-page: https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: opensource@networktocode.com
 Requires-Python: >=3.7,<4.0
@@ -56,14 +56,31 @@
 
 **Software Lifecycle Management List View**
 
 You can view the list of Software versions as well as filter the table.
 
 ![](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/lcm_software_list_view.png)
 
+**Software Lifecycle Reporting**
+
+Reports can be created from the Nautobot's software validation jobs **Device Software Validation - Report** or **Inventory Item Software Validation - Report**.
+
+![](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/lcm_software_validation_report_run_graph.png)
+
+Individual CSV files can be exported per platform or inventory item.
+
+![](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/lcm_software_validation_report_run_detailed_summary.png)
+
+Sample CSV.
+
+![](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/lcm_software_validation_report_csv_small.png)
+
+You can also view validation results as a list from the Nautobot GUI.
+
+![](https://raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/lcm_software_validation_report_run_results_list.png)
 
 ## Try it out!
 
 This App is installed in the Nautobot Community Sandbox found over at [demo.nautobot.com](https://demo.nautobot.com/)!
 
 > For a full list of all the available always-on sandbox environments, head over to the main page on [networktocode.com](https://www.networktocode.com/nautobot/sandbox-environments/).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nautobot-device-lifecycle-mgmt Version: 1.2.0
+Metadata-Version: 2.1 Name: nautobot-device-lifecycle-mgmt Version: 1.3.0
 Summary: Manages device lifecycles for platforms and software. Home-page:
 https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt License:
 Apache-2.0 Keywords: nautobot,nautobot-plugin Author: Network to Code, LLC
 Author-email: opensource@networktocode.com Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -37,39 +37,52 @@
 Detail View** You can also click a Hardware/Software Notice and see the detail
 view. This view provides links to the devices that are part affected by this
 EoX notice due to their device type. ![](https://raw.githubusercontent.com/
 nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/
 lcm_hardware_detail_view.png) **Software Lifecycle Management List View** You
 can view the list of Software versions as well as filter the table. ![](https:/
 /raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/
-develop/docs/images/lcm_software_list_view.png) ## Try it out! This App is
-installed in the Nautobot Community Sandbox found over at [demo.nautobot.com]
-(https://demo.nautobot.com/)! > For a full list of all the available always-on
-sandbox environments, head over to the main page on [networktocode.com](https:/
-/www.networktocode.com/nautobot/sandbox-environments/). ## Documentation Full
-web-based HTML documentation for this app can be found over on the [Nautobot
-Docs](https://docs.nautobot.com) website: - [User Guide](https://
-docs.nautobot.com/projects/device-lifecycle/en/latest/user/app_overview/) -
-Overview, Using the App, Getting Started. - [Administrator Guide](https://
-docs.nautobot.com/projects/device-lifecycle/en/latest/admin/install/) - How to
-Install, Configure, Upgrade, or Uninstall the App. - [Developer Guide](https://
-docs.nautobot.com/projects/device-lifecycle/en/latest/dev/contributing/) -
-Extending the App, Code Reference, Contribution Guide. - [Release Notes /
-Changelog](https://docs.nautobot.com/projects/device-lifecycle/en/latest/admin/
-release_notes/). - [Frequently Asked Questions](https://docs.nautobot.com/
-projects/device-lifecycle/en/latest/user/faq/). ### Contributing to the Docs
-You can find all the Markdown source for the App documentation under the [docs]
-(https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/tree/
-develop/docs) folder in this repository. For simple edits, a Markdown capable
-editor is sufficient - clone the repository and edit away. If you need to view
-the fully generated documentation site, you can build it with [mkdocs](https://
-www.mkdocs.org/). A container hosting the docs will be started using the invoke
-commands (details in the [Development Environment Guide](https://
-docs.nautobot.com/projects/device-lifecycle/en/latest/dev/dev_environment/
-#docker-development-environment)) on [http://localhost:8001](http://localhost:
-8001). As your changes are saved, the live docs will be automatically reloaded.
-Any PRs with fixes or improvements are very welcome! ## Questions For any
-questions or comments, please check the [FAQ](https://docs.nautobot.com/
-projects/device-lifecycle/en/latest/user/faq/) first. Feel free to also swing
-by the [Network to Code Slack](https://networktocode.slack.com/) (channel
-`#nautobot`), sign up [here](http://slack.networktocode.com/) if you don't have
-an account.
+develop/docs/images/lcm_software_list_view.png) **Software Lifecycle
+Reporting** Reports can be created from the Nautobot's software validation jobs
+**Device Software Validation - Report** or **Inventory Item Software Validation
+- Report**. ![](https://raw.githubusercontent.com/nautobot/nautobot-plugin-
+device-lifecycle-mgmt/develop/docs/images/
+lcm_software_validation_report_run_graph.png) Individual CSV files can be
+exported per platform or inventory item. ![](https://raw.githubusercontent.com/
+nautobot/nautobot-plugin-device-lifecycle-mgmt/develop/docs/images/
+lcm_software_validation_report_run_detailed_summary.png) Sample CSV. ![](https:
+//raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/
+develop/docs/images/lcm_software_validation_report_csv_small.png) You can also
+view validation results as a list from the Nautobot GUI. ![](https://
+raw.githubusercontent.com/nautobot/nautobot-plugin-device-lifecycle-mgmt/
+develop/docs/images/lcm_software_validation_report_run_results_list.png) ## Try
+it out! This App is installed in the Nautobot Community Sandbox found over at
+[demo.nautobot.com](https://demo.nautobot.com/)! > For a full list of all the
+available always-on sandbox environments, head over to the main page on
+[networktocode.com](https://www.networktocode.com/nautobot/sandbox-
+environments/). ## Documentation Full web-based HTML documentation for this app
+can be found over on the [Nautobot Docs](https://docs.nautobot.com) website: -
+[User Guide](https://docs.nautobot.com/projects/device-lifecycle/en/latest/
+user/app_overview/) - Overview, Using the App, Getting Started. -
+[Administrator Guide](https://docs.nautobot.com/projects/device-lifecycle/en/
+latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall the
+App. - [Developer Guide](https://docs.nautobot.com/projects/device-lifecycle/
+en/latest/dev/contributing/) - Extending the App, Code Reference, Contribution
+Guide. - [Release Notes / Changelog](https://docs.nautobot.com/projects/device-
+lifecycle/en/latest/admin/release_notes/). - [Frequently Asked Questions]
+(https://docs.nautobot.com/projects/device-lifecycle/en/latest/user/faq/). ###
+Contributing to the Docs You can find all the Markdown source for the App
+documentation under the [docs](https://github.com/nautobot/nautobot-plugin-
+device-lifecycle-mgmt/tree/develop/docs) folder in this repository. For simple
+edits, a Markdown capable editor is sufficient - clone the repository and edit
+away. If you need to view the fully generated documentation site, you can build
+it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be
+started using the invoke commands (details in the [Development Environment
+Guide](https://docs.nautobot.com/projects/device-lifecycle/en/latest/dev/
+dev_environment/#docker-development-environment)) on [http://localhost:8001]
+(http://localhost:8001). As your changes are saved, the live docs will be
+automatically reloaded. Any PRs with fixes or improvements are very welcome! ##
+Questions For any questions or comments, please check the [FAQ](https://
+docs.nautobot.com/projects/device-lifecycle/en/latest/user/faq/) first. Feel
+free to also swing by the [Network to Code Slack](https://
+networktocode.slack.com/) (channel `#nautobot`), sign up [here](http://
+slack.networktocode.com/) if you don't have an account.
```

