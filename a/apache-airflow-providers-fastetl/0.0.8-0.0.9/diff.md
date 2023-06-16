# Comparing `tmp/apache-airflow-providers-fastetl-0.0.8.tar.gz` & `tmp/apache-airflow-providers-fastetl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-fastetl-0.0.8.tar", last modified: Mon Apr 17 20:32:38 2023, max compression
+gzip compressed data, was "apache-airflow-providers-fastetl-0.0.9.tar", last modified: Tue Apr 18 22:36:41 2023, max compression
```

## Comparing `apache-airflow-providers-fastetl-0.0.8.tar` & `apache-airflow-providers-fastetl-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.540189 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-17 20:32:38.000000 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-17 20:32:38.000000 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:32:38.000000 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 20:32:38.000000 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-17 20:32:38.000000 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 20:32:38.000000 apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.540189 apache-airflow-providers-fastetl-0.0.8/fastetl/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.540189 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/copy_db_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/fast_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)    48313 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/patchwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/samba_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/db_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/encode_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/get_table_cols_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/load_env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/load_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    17949 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/odf_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/string_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/table_comments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/bacen_STA_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/ckan_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/dadosgovbr_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/db_to_db_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/dou_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/gsheet_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/osrm_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/datapackage_to_datadictionary_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/db_to_csv_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/db_to_db_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/gsheet_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/fastetl/operators/osrm_distance_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:32:38.544189 apache-airflow-providers-fastetl-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/tests/test_db_to_db_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/tests/test_odf_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-17 20:32:21.000000 apache-airflow-providers-fastetl-0.0.8/tests/test_osrm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:41.885321 apache-airflow-providers-fastetl-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-18 22:36:41.885321 apache-airflow-providers-fastetl-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:41.877320 apache-airflow-providers-fastetl-0.0.9/apache_airflow_providers_fastetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-18 22:36:41.000000 apache-airflow-providers-fastetl-0.0.9/apache_airflow_providers_fastetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-18 22:36:41.000000 apache-airflow-providers-fastetl-0.0.9/apache_airflow_providers_fastetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:36:41.000000 apache-airflow-providers-fastetl-0.0.9/apache_airflow_providers_fastetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-18 22:36:41.000000 apache-airflow-providers-fastetl-0.0.9/apache_airflow_providers_fastetl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-18 22:36:41.000000 apache-airflow-providers-fastetl-0.0.9/apache_airflow_providers_fastetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 22:36:41.000000 apache-airflow-providers-fastetl-0.0.9/apache_airflow_providers_fastetl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:41.877320 apache-airflow-providers-fastetl-0.0.9/fastetl/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:41.877320 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/copy_db_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28724 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/fast_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48313 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/patchwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/samba_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:41.881320 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/encode_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/get_table_cols_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/load_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/load_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17949 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/odf_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/string_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/table_comments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:41.881320 apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/bacen_STA_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/ckan_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/dadosgovbr_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/db_to_db_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/dou_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/gsheet_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/osrm_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:41.881320 apache-airflow-providers-fastetl-0.0.9/fastetl/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/operators/datapackage_to_datadictionary_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/operators/db_to_csv_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/operators/db_to_db_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/operators/gsheet_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/fastetl/operators/osrm_distance_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 22:36:41.885321 apache-airflow-providers-fastetl-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:41.885321 apache-airflow-providers-fastetl-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/tests/test_db_to_db_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/tests/test_odf_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-18 22:36:13.000000 apache-airflow-providers-fastetl-0.0.9/tests/test_osrm.py
```

### Comparing `apache-airflow-providers-fastetl-0.0.8/LICENSE` & `apache-airflow-providers-fastetl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/PKG-INFO` & `apache-airflow-providers-fastetl-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-fastetl
-Version: 0.0.8
+Version: 0.0.9
 Summary: FastETL custom package Apache Airflow provider.
 Home-page: https://github.com/economiagovbr/FastETL
 Author: Time de Dados CGINF
 Author-email: seges.cginf@economia.gov.br
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

### Comparing `apache-airflow-providers-fastetl-0.0.8/README.md` & `apache-airflow-providers-fastetl-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/PKG-INFO` & `apache-airflow-providers-fastetl-0.0.9/apache_airflow_providers_fastetl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-fastetl
-Version: 0.0.8
+Version: 0.0.9
 Summary: FastETL custom package Apache Airflow provider.
 Home-page: https://github.com/economiagovbr/FastETL
 Author: Time de Dados CGINF
 Author-email: seges.cginf@economia.gov.br
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

### Comparing `apache-airflow-providers-fastetl-0.0.8/apache_airflow_providers_fastetl.egg-info/SOURCES.txt` & `apache-airflow-providers-fastetl-0.0.9/apache_airflow_providers_fastetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/__init__.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/copy_db_extensions.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/copy_db_extensions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/fast_etl.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/fast_etl.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,15 +343,18 @@
         r"from\s+\"?\'?\[?[\w|\.|\"|\'|\]|\]]*\"?\'?\]?", query, re.IGNORECASE
     ).group()
     # split "from " from "schema.table" and get schema.table[-1]
     db_schema_table = sintax_from.split()[-1]
     # clean `[`, `]`, `"`, `'`
     db_schema_table = re.sub(r"\[|\]|\"|\'", "", db_schema_table)
     # clean "dbo." if exists as dbo.schema.table
-    schema, table = db_schema_table.split(".")[-2:]
+    try:
+        schema, table = db_schema_table.split(".")[-2:]
+    except ValueError:
+        schema, table = "multiple", "multiple"
 
     return schema, table
 
 
 def copy_db_to_db(
     source: Dict[str, str],
     destination: Dict[str, str],
```

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/patchwork.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/patchwork.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/samba_services.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/samba_services.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/date.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/date.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/db_connection.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/db_connection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/encode_html.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/encode_html.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/get_table_cols_name.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/get_table_cols_name.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/load_env_var.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/load_env_var.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/load_info.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/load_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/odf_tables.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/odf_tables.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/string_formatting.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/string_formatting.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/custom_functions/utils/table_comments.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/custom_functions/utils/table_comments.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/bacen_STA_hook.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/bacen_STA_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/ckan_hook.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/ckan_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/dadosgovbr_hook.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/dadosgovbr_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/db_to_db_hook.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/db_to_db_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/dou_hook.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/dou_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/gsheet_hook.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/gsheet_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/hooks/osrm_hook.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/hooks/osrm_hook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/operators/datapackage_to_datadictionary_operator.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/operators/datapackage_to_datadictionary_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/operators/db_to_csv_operator.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/operators/db_to_csv_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/operators/db_to_db_operator.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/operators/db_to_db_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 from typing import Dict
 
 from airflow.models.baseoperator import BaseOperator
 
 from fastetl.hooks.db_to_db_hook import DbToDbHook
 
 class DbToDbOperator(BaseOperator):
+    template_fields = ('source')
 
     def __init__(
             self,
             source: Dict[str, str],
             destination: Dict[str, str],
             columns_to_ignore: list = None,
             destination_truncate: bool = True,
```

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/operators/gsheet_operator.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/operators/gsheet_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/fastetl/operators/osrm_distance_operator.py` & `apache-airflow-providers-fastetl-0.0.9/fastetl/operators/osrm_distance_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/setup.py` & `apache-airflow-providers-fastetl-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 """Perform the package apache-airflow-providers-fastetl setup."""
 setup(
     name="apache-airflow-providers-fastetl",
     version=__version__,
     description="FastETL custom package Apache Airflow provider.",
     long_description=long_description,
```

### Comparing `apache-airflow-providers-fastetl-0.0.8/tests/test_dag.py` & `apache-airflow-providers-fastetl-0.0.9/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/tests/test_db_to_db_operator.py` & `apache-airflow-providers-fastetl-0.0.9/tests/test_db_to_db_operator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/tests/test_odf_tables.py` & `apache-airflow-providers-fastetl-0.0.9/tests/test_odf_tables.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-fastetl-0.0.8/tests/test_osrm.py` & `apache-airflow-providers-fastetl-0.0.9/tests/test_osrm.py`

 * *Files identical despite different names*

