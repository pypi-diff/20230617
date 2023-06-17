# Comparing `tmp/control_rod-2023.6.16.0.tar.gz` & `tmp/control_rod-2023.6.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control_rod-2023.6.16.0.tar", last modified: Sat Jun 17 00:00:33 2023, max compression
+gzip compressed data, was "control_rod-2023.6.16.1.tar", last modified: Sat Jun 17 04:36:13 2023, max compression
```

## Comparing `control_rod-2023.6.16.0.tar` & `control_rod-2023.6.16.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:00:33.165854 control_rod-2023.6.16.0/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-17 00:00:33.165854 control_rod-2023.6.16.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:00:33.161854 control_rod-2023.6.16.0/abobjs/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/auditable_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/auditable_entity_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/auditable_entity_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    28364 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/buisness_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/continuous_monitoring_monitor_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/continuous_monitoring_monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/continuous_monitoring_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/controlrod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/controls_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/departments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/effectiveness_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/fn_register_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/status_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/test_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/vendor_criticalities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/abobjs/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:00:33.161854 control_rod-2023.6.16.0/control_rod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-17 00:00:33.000000 control_rod-2023.6.16.0/control_rod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-17 00:00:33.000000 control_rod-2023.6.16.0/control_rod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 00:00:33.000000 control_rod-2023.6.16.0/control_rod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-17 00:00:33.000000 control_rod-2023.6.16.0/control_rod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 00:00:33.000000 control_rod-2023.6.16.0/control_rod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-17 00:00:33.165854 control_rod-2023.6.16.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:00:33.165854 control_rod-2023.6.16.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_controlrod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_controlsdatum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_effectivenessoption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_status_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_testsection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_testtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-17 00:00:17.000000 control_rod-2023.6.16.0/tests/test_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:36:13.463416 control_rod-2023.6.16.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-17 04:36:13.463416 control_rod-2023.6.16.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:36:13.459416 control_rod-2023.6.16.1/abobjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/auditable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/auditable_entity_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/auditable_entity_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28364 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/buisness_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/continuous_monitoring_monitor_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/continuous_monitoring_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/continuous_monitoring_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/controlrod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/controls_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/departments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/effectiveness_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/fn_register_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/status_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/vendor_criticalities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/abobjs/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:36:13.463416 control_rod-2023.6.16.1/control_rod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-17 04:36:13.000000 control_rod-2023.6.16.1/control_rod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-17 04:36:13.000000 control_rod-2023.6.16.1/control_rod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 04:36:13.000000 control_rod-2023.6.16.1/control_rod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-17 04:36:13.000000 control_rod-2023.6.16.1/control_rod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 04:36:13.000000 control_rod-2023.6.16.1/control_rod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-17 04:36:13.467416 control_rod-2023.6.16.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:36:13.463416 control_rod-2023.6.16.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_controlrod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_controlsdatum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_effectivenessoption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_status_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_testsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_testtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-17 04:35:55.000000 control_rod-2023.6.16.1/tests/test_workspace.py
```

### Comparing `control_rod-2023.6.16.0/abobjs/__init__.py` & `control_rod-2023.6.16.1/abobjs/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,13 +50,17 @@
              "auditable_entity_reference_ids": {"obj": AB_Auditable_Entities}, # How AE's reference other AE's
              "auditable_entity_region_id": {"obj": AB_Auditable_Entity_Regions},
              "vendor_criticalities_id": {"obj": AB_Vendor_Criticality},
              "department_ids": {"obj": AB_Departments},
              "created_by_user_id": {"obj": AB_User},
              "tprm_user_ids": {"obj": AB_User},
              "owner_user_ids": {"obj": AB_User},
+             "svp_owner_user_id": {"obj": AB_User},
+             "additional_owner_user_ids": {"obj": AB_User},
+             "auditor_user_ids": {"obj": AB_User},
+             "product_manager_user_ids": {"obj": AB_User}
             }
 
 from .fn_register_cf import fn_register_custom_fields
 from .controlrod import AB_ControlRod
 
 USER_AGENT = "control_rod/2023.6.13.0"
```

### Comparing `control_rod-2023.6.16.0/abobjs/assertion.py` & `control_rod-2023.6.16.1/abobjs/assertion.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/auditable_entity.py` & `control_rod-2023.6.16.1/abobjs/auditable_entity.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/auditable_entity_regions.py` & `control_rod-2023.6.16.1/abobjs/auditable_entity_regions.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/auditable_entity_types.py` & `control_rod-2023.6.16.1/abobjs/auditable_entity_types.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/base.py` & `control_rod-2023.6.16.1/abobjs/base.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/buisness_units.py` & `control_rod-2023.6.16.1/abobjs/buisness_units.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/continuous_monitoring_monitor_results.py` & `control_rod-2023.6.16.1/abobjs/continuous_monitoring_monitor_results.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/continuous_monitoring_monitors.py` & `control_rod-2023.6.16.1/abobjs/continuous_monitoring_monitors.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/continuous_monitoring_systems.py` & `control_rod-2023.6.16.1/abobjs/continuous_monitoring_systems.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/control.py` & `control_rod-2023.6.16.1/abobjs/control.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/controlrod.py` & `control_rod-2023.6.16.1/abobjs/controlrod.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/controls_data.py` & `control_rod-2023.6.16.1/abobjs/controls_data.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/custom_field.py` & `control_rod-2023.6.16.1/abobjs/custom_field.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/departments.py` & `control_rod-2023.6.16.1/abobjs/departments.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/effectiveness_option.py` & `control_rod-2023.6.16.1/abobjs/effectiveness_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/entity.py` & `control_rod-2023.6.16.1/abobjs/entity.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/file.py` & `control_rod-2023.6.16.1/abobjs/file.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/fn_register_cf.py` & `control_rod-2023.6.16.1/abobjs/fn_register_cf.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/multi.py` & `control_rod-2023.6.16.1/abobjs/multi.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/process.py` & `control_rod-2023.6.16.1/abobjs/process.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/region.py` & `control_rod-2023.6.16.1/abobjs/region.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/risk.py` & `control_rod-2023.6.16.1/abobjs/risk.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/status_option.py` & `control_rod-2023.6.16.1/abobjs/status_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/subprocess.py` & `control_rod-2023.6.16.1/abobjs/subprocess.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/test.py` & `control_rod-2023.6.16.1/abobjs/test.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/test_section.py` & `control_rod-2023.6.16.1/abobjs/test_section.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/test_type.py` & `control_rod-2023.6.16.1/abobjs/test_type.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/user.py` & `control_rod-2023.6.16.1/abobjs/user.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/vendor_criticalities.py` & `control_rod-2023.6.16.1/abobjs/vendor_criticalities.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/abobjs/workspace.py` & `control_rod-2023.6.16.1/abobjs/workspace.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/control_rod.egg-info/SOURCES.txt` & `control_rod-2023.6.16.1/control_rod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/setup.cfg` & `control_rod-2023.6.16.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = control_rod
-version = 2023.06.16.0
+version = 2023.06.16.1
 author = Chris Halbersma
 author_email = chalbersma@auditboard.com
 description = An expiremental auditboard api client
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/soxhub/control_rod
 classifiers =
```

### Comparing `control_rod-2023.6.16.0/tests/test_assertion.py` & `control_rod-2023.6.16.1/tests/test_assertion.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_control.py` & `control_rod-2023.6.16.1/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_controlrod.py` & `control_rod-2023.6.16.1/tests/test_controlrod.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_controlsdatum.py` & `control_rod-2023.6.16.1/tests/test_controlsdatum.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_effectivenessoption.py` & `control_rod-2023.6.16.1/tests/test_effectivenessoption.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_entity.py` & `control_rod-2023.6.16.1/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_files.py` & `control_rod-2023.6.16.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_process.py` & `control_rod-2023.6.16.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_region.py` & `control_rod-2023.6.16.1/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_risk.py` & `control_rod-2023.6.16.1/tests/test_risk.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_status_option.py` & `control_rod-2023.6.16.1/tests/test_status_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_subprocess.py` & `control_rod-2023.6.16.1/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_test.py` & `control_rod-2023.6.16.1/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_testsection.py` & `control_rod-2023.6.16.1/tests/test_testsection.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_testtypes.py` & `control_rod-2023.6.16.1/tests/test_testtypes.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.6.16.0/tests/test_workspace.py` & `control_rod-2023.6.16.1/tests/test_workspace.py`

 * *Files identical despite different names*

