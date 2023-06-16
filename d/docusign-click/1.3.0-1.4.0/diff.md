# Comparing `tmp/docusign-click-1.3.0.tar.gz` & `tmp/docusign-click-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/docusign-click-1.3.0.tar", last modified: Thu Feb 16 17:09:24 2023, max compression
+gzip compressed data, was "dist/docusign-click-1.4.0.tar", last modified: Fri Jun 16 22:00:55 2023, max compression
```

## Comparing `docusign-click-1.3.0.tar` & `docusign-click-1.4.0.tar`

### file list

```diff
@@ -1,63 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:09:24.000000 docusign-click-1.3.0/
--rwxr-xr-x   0 root         (0) root         (0)     1102 2023-02-16 17:09:21.000000 docusign-click-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3709 2023-02-16 17:09:24.000000 docusign-click-1.3.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     3474 2023-02-16 17:09:21.000000 docusign-click-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:09:24.000000 docusign-click-1.3.0/docusign_click/
--rw-r--r--   0 root         (0) root         (0)     2837 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:09:24.000000 docusign-click-1.3.0/docusign_click/apis/
--rw-r--r--   0 root         (0) root         (0)      125 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127904 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/apis/accounts_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:09:24.000000 docusign-click-1.3.0/docusign_click/client/
--rwxr-xr-x   0 root         (0) root         (0)      283 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/client/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    35235 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/client/api_client.py
--rwxr-xr-x   0 root         (0) root         (0)     1503 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/client/api_exception.py
--rwxr-xr-x   0 root         (0) root         (0)    11315 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/client/api_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:09:24.000000 docusign-click-1.3.0/docusign_click/client/auth/
--rwxr-xr-x   0 root         (0) root         (0)      219 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/client/auth/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    14756 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/client/auth/oauth.py
--rwxr-xr-x   0 root         (0) root         (0)     7254 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/client/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:09:24.000000 docusign-click-1.3.0/docusign_click/models/
--rw-r--r--   0 root         (0) root         (0)     2371 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5483 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/bulk_clickwrap_request.py
--rw-r--r--   0 root         (0) root         (0)     7743 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_agreements_response.py
--rw-r--r--   0 root         (0) root         (0)     8135 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_delete_response.py
--rw-r--r--   0 root         (0) root         (0)    17018 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_request.py
--rw-r--r--   0 root         (0) root         (0)    14983 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_response.py
--rw-r--r--   0 root         (0) root         (0)     6707 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_scheduled_reacceptance.py
--rw-r--r--   0 root         (0) root         (0)    13727 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_summary_response.py
--rw-r--r--   0 root         (0) root         (0)     5203 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)    14468 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_version.py
--rw-r--r--   0 root         (0) root         (0)    13164 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_version_delete_info.py
--rw-r--r--   0 root         (0) root         (0)    17745 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_version_delete_response.py
--rw-r--r--   0 root         (0) root         (0)    19371 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_version_response.py
--rw-r--r--   0 root         (0) root         (0)    17998 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_version_summary_response.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_versions_delete_response.py
--rw-r--r--   0 root         (0) root         (0)     9396 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_versions_paged_response.py
--rw-r--r--   0 root         (0) root         (0)     6717 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwrap_versions_response.py
--rw-r--r--   0 root         (0) root         (0)     3993 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwraps_delete_response.py
--rw-r--r--   0 root         (0) root         (0)     5715 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/clickwraps_response.py
--rw-r--r--   0 root         (0) root         (0)     4728 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/conversion_document.py
--rw-r--r--   0 root         (0) root         (0)     4836 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/data_field.py
--rw-r--r--   0 root         (0) root         (0)    19755 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/display_settings.py
--rw-r--r--   0 root         (0) root         (0)     9588 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/document.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/document_conversion_request.py
--rw-r--r--   0 root         (0) root         (0)     3358 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/document_conversion_response.py
--rw-r--r--   0 root         (0) root         (0)     7714 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/document_data.py
--rw-r--r--   0 root         (0) root         (0)     4472 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/error_details.py
--rw-r--r--   0 root         (0) root         (0)     3746 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/html_result.py
--rw-r--r--   0 root         (0) root         (0)     8669 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/service_information.py
--rw-r--r--   0 root         (0) root         (0)     4634 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/service_version.py
--rw-r--r--   0 root         (0) root         (0)     7624 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/user_agreement_request.py
--rw-r--r--   0 root         (0) root         (0)    24181 2023-02-16 17:09:21.000000 docusign-click-1.3.0/docusign_click/models/user_agreement_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:09:24.000000 docusign-click-1.3.0/docusign_click.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3709 2023-02-16 17:09:23.000000 docusign-click-1.3.0/docusign_click.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2173 2023-02-16 17:09:24.000000 docusign-click-1.3.0/docusign_click.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-16 17:09:24.000000 docusign-click-1.3.0/docusign_click.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      128 2023-02-16 17:09:24.000000 docusign-click-1.3.0/docusign_click.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-02-16 17:09:24.000000 docusign-click-1.3.0/docusign_click.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)       79 2023-02-16 17:09:24.000000 docusign-click-1.3.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1838 2023-02-16 17:09:21.000000 docusign-click-1.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:09:24.000000 docusign-click-1.3.0/test/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:09:21.000000 docusign-click-1.3.0/test/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4754 2023-02-16 17:09:21.000000 docusign-click-1.3.0/test/test_oauth.py
--rwxr-xr-x   0 root         (0) root         (0)     2916 2023-02-16 17:09:21.000000 docusign-click-1.3.0/test/unit_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:00:55.000000 docusign-click-1.4.0/
+-rwxr-xr-x   0 root         (0) root         (0)     1102 2023-06-16 22:00:52.000000 docusign-click-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-06-16 22:00:55.000000 docusign-click-1.4.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     3474 2023-06-16 22:00:52.000000 docusign-click-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:00:55.000000 docusign-click-1.4.0/docusign_click/
+-rw-r--r--   0 root         (0) root         (0)     3532 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:00:55.000000 docusign-click-1.4.0/docusign_click/apis/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127904 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/apis/accounts_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:00:55.000000 docusign-click-1.4.0/docusign_click/client/
+-rwxr-xr-x   0 root         (0) root         (0)      283 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/client/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    35235 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/client/api_client.py
+-rwxr-xr-x   0 root         (0) root         (0)     1503 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/client/api_exception.py
+-rwxr-xr-x   0 root         (0) root         (0)    11315 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/client/api_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:00:55.000000 docusign-click-1.4.0/docusign_click/client/auth/
+-rwxr-xr-x   0 root         (0) root         (0)      219 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/client/auth/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    14756 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/client/auth/oauth.py
+-rwxr-xr-x   0 root         (0) root         (0)     7254 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/client/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:00:55.000000 docusign-click-1.4.0/docusign_click/models/
+-rw-r--r--   0 root         (0) root         (0)     3066 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21089 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/agree_button_styles.py
+-rw-r--r--   0 root         (0) root         (0)     8518 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/agreement_statement_styles.py
+-rw-r--r--   0 root         (0) root         (0)    18908 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/base_agree_button_styles.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/bulk_clickwrap_request.py
+-rw-r--r--   0 root         (0) root         (0)     7743 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_agreements_response.py
+-rw-r--r--   0 root         (0) root         (0)     8135 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_delete_response.py
+-rw-r--r--   0 root         (0) root         (0)    17018 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_request.py
+-rw-r--r--   0 root         (0) root         (0)    14983 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_response.py
+-rw-r--r--   0 root         (0) root         (0)     6707 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_scheduled_reacceptance.py
+-rw-r--r--   0 root         (0) root         (0)    13727 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_summary_response.py
+-rw-r--r--   0 root         (0) root         (0)     5203 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)    14468 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_version.py
+-rw-r--r--   0 root         (0) root         (0)    13164 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_version_delete_info.py
+-rw-r--r--   0 root         (0) root         (0)    17745 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_version_delete_response.py
+-rw-r--r--   0 root         (0) root         (0)    19371 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_version_response.py
+-rw-r--r--   0 root         (0) root         (0)    17998 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_version_summary_response.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_versions_delete_response.py
+-rw-r--r--   0 root         (0) root         (0)     9396 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_versions_paged_response.py
+-rw-r--r--   0 root         (0) root         (0)     6717 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwrap_versions_response.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwraps_delete_response.py
+-rw-r--r--   0 root         (0) root         (0)     5715 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/clickwraps_response.py
+-rw-r--r--   0 root         (0) root         (0)     7633 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/container_styles.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/conversion_document.py
+-rw-r--r--   0 root         (0) root         (0)     4836 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/data_field.py
+-rw-r--r--   0 root         (0) root         (0)     4035 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/disclosure_link_styles.py
+-rw-r--r--   0 root         (0) root         (0)    19755 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/display_settings.py
+-rw-r--r--   0 root         (0) root         (0)     9588 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/document.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/document_conversion_request.py
+-rw-r--r--   0 root         (0) root         (0)     3358 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/document_conversion_response.py
+-rw-r--r--   0 root         (0) root         (0)     7714 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/document_data.py
+-rw-r--r--   0 root         (0) root         (0)    11697 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/document_link_styles.py
+-rw-r--r--   0 root         (0) root         (0)    10540 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/document_link_styles_focus.py
+-rw-r--r--   0 root         (0) root         (0)     4472 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/error_details.py
+-rw-r--r--   0 root         (0) root         (0)     9093 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/header_styles.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/html_result.py
+-rw-r--r--   0 root         (0) root         (0)     8669 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/service_information.py
+-rw-r--r--   0 root         (0) root         (0)     4634 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/service_version.py
+-rw-r--r--   0 root         (0) root         (0)     7624 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/user_agreement_request.py
+-rw-r--r--   0 root         (0) root         (0)    23709 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/user_agreement_response.py
+-rw-r--r--   0 root         (0) root         (0)    10421 2023-06-16 22:00:52.000000 docusign-click-1.4.0/docusign_click/models/user_agreement_response_style.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:00:55.000000 docusign-click-1.4.0/docusign_click.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-06-16 22:00:55.000000 docusign-click-1.4.0/docusign_click.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2602 2023-06-16 22:00:55.000000 docusign-click-1.4.0/docusign_click.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 22:00:55.000000 docusign-click-1.4.0/docusign_click.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      128 2023-06-16 22:00:55.000000 docusign-click-1.4.0/docusign_click.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-16 22:00:55.000000 docusign-click-1.4.0/docusign_click.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)       79 2023-06-16 22:00:55.000000 docusign-click-1.4.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1838 2023-06-16 22:00:52.000000 docusign-click-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:00:55.000000 docusign-click-1.4.0/test/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:00:52.000000 docusign-click-1.4.0/test/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4754 2023-06-16 22:00:52.000000 docusign-click-1.4.0/test/test_oauth.py
+-rwxr-xr-x   0 root         (0) root         (0)     2916 2023-06-16 22:00:52.000000 docusign-click-1.4.0/test/unit_tests.py
```

### Comparing `docusign-click-1.3.0/LICENSE` & `docusign-click-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/PKG-INFO` & `docusign-click-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docusign-click
-Version: 1.3.0
+Version: 1.4.0
 Summary: DocuSign Click API
 Home-page: 
 Author-email: devcenter@docusign.com
 Keywords: Swagger,DocuSign Click API
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docusign-click Version: 1.3.0 Summary: DocuSign
+Metadata-Version: 2.1 Name: docusign-click Version: 1.4.0 Summary: DocuSign
 Click API Home-page: Author-email: devcenter@docusign.com Keywords:
 Swagger,DocuSign Click API Description-Content-Type: text/markdown License-
 File: LICENSE # The Official DocuSign Click Python Client [![PyPI version]
 [pypi-image]][pypi-url]  [![Build status][travis-image]][travis-url] [PyPI
 module](https://pypi.python.org/pypi/docusign_click) that wraps the DocuSign
 Click API [Documentation about the DocuSign Click API](https://
 developers.docusign.com/) ## Requirements - Python 2.7 (3.7+ recommended) -
```

### Comparing `docusign-click-1.3.0/README.md` & `docusign-click-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/__init__.py` & `docusign-click-1.4.0/docusign_click/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,48 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     DocuSign Click API
 
     Elastic signing (also known as DocuSign Click)  lets you capture consent to standard agreement terms with a single click: terms and conditions, terms of service, terms of use, privacy policies, and more. The Click API lets you include this customizable elastic template solution in your DocuSign integrations.  # noqa: E501
 
     OpenAPI spec version: v1
     Contact: devcenter@docusign.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from .apis.accounts_api import AccountsApi
-
-# import ApiClient
-from .client.api_client import ApiClient
-from .client.configuration import Configuration
-from .client.api_exception import ApiException
-
-from .client.auth.oauth import OAuth	
-from .client.auth.oauth import OAuthToken	
-from .client.auth.oauth import Account	
-from .client.auth.oauth import Organization	
-from .client.auth.oauth import Link
-
-# import models into sdk package
+# import models into model package
+from docusign_click.models.agree_button_styles import AgreeButtonStyles
+from docusign_click.models.agreement_statement_styles import AgreementStatementStyles
+from docusign_click.models.base_agree_button_styles import BaseAgreeButtonStyles
 from docusign_click.models.bulk_clickwrap_request import BulkClickwrapRequest
 from docusign_click.models.clickwrap_agreements_response import ClickwrapAgreementsResponse
 from docusign_click.models.clickwrap_delete_response import ClickwrapDeleteResponse
 from docusign_click.models.clickwrap_request import ClickwrapRequest
 from docusign_click.models.clickwrap_scheduled_reacceptance import ClickwrapScheduledReacceptance
 from docusign_click.models.clickwrap_transfer_request import ClickwrapTransferRequest
 from docusign_click.models.clickwrap_version import ClickwrapVersion
 from docusign_click.models.clickwrap_version_delete_response import ClickwrapVersionDeleteResponse
 from docusign_click.models.clickwrap_version_response import ClickwrapVersionResponse
 from docusign_click.models.clickwrap_version_summary_response import ClickwrapVersionSummaryResponse
 from docusign_click.models.clickwrap_versions_delete_response import ClickwrapVersionsDeleteResponse
 from docusign_click.models.clickwrap_versions_paged_response import ClickwrapVersionsPagedResponse
 from docusign_click.models.clickwrap_versions_response import ClickwrapVersionsResponse
 from docusign_click.models.clickwraps_delete_response import ClickwrapsDeleteResponse
+from docusign_click.models.container_styles import ContainerStyles
 from docusign_click.models.data_field import DataField
+from docusign_click.models.disclosure_link_styles import DisclosureLinkStyles
 from docusign_click.models.display_settings import DisplaySettings
 from docusign_click.models.document import Document
+from docusign_click.models.document_link_styles import DocumentLinkStyles
+from docusign_click.models.document_link_styles_focus import DocumentLinkStylesFocus
 from docusign_click.models.error_details import ErrorDetails
+from docusign_click.models.header_styles import HeaderStyles
 from docusign_click.models.service_information import ServiceInformation
 from docusign_click.models.service_version import ServiceVersion
 from docusign_click.models.user_agreement_request import UserAgreementRequest
 from docusign_click.models.user_agreement_response import UserAgreementResponse
-
-
-configuration = Configuration()
+from docusign_click.models.user_agreement_response_style import UserAgreementResponseStyle
```

### Comparing `docusign-click-1.3.0/docusign_click/apis/accounts_api.py` & `docusign-click-1.4.0/docusign_click/apis/accounts_api.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/client/api_client.py` & `docusign-click-1.4.0/docusign_click/client/api_client.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/client/api_exception.py` & `docusign-click-1.4.0/docusign_click/client/api_exception.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/client/api_response.py` & `docusign-click-1.4.0/docusign_click/client/api_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/client/auth/oauth.py` & `docusign-click-1.4.0/docusign_click/client/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/client/configuration.py` & `docusign-click-1.4.0/docusign_click/client/configuration.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/bulk_clickwrap_request.py` & `docusign-click-1.4.0/docusign_click/models/bulk_clickwrap_request.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_agreements_response.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_agreements_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_delete_response.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_delete_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_request.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_request.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_response.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_scheduled_reacceptance.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_scheduled_reacceptance.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_summary_response.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_summary_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_transfer_request.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_transfer_request.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_version.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_version.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_version_delete_info.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_version_delete_info.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_version_delete_response.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_version_delete_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_version_response.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_version_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_version_summary_response.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_version_summary_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_versions_delete_response.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_versions_delete_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_versions_paged_response.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_versions_paged_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwrap_versions_response.py` & `docusign-click-1.4.0/docusign_click/models/clickwrap_versions_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwraps_delete_response.py` & `docusign-click-1.4.0/docusign_click/models/clickwraps_delete_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/clickwraps_response.py` & `docusign-click-1.4.0/docusign_click/models/clickwraps_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/conversion_document.py` & `docusign-click-1.4.0/docusign_click/models/conversion_document.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/data_field.py` & `docusign-click-1.4.0/docusign_click/models/data_field.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/display_settings.py` & `docusign-click-1.4.0/docusign_click/models/display_settings.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/document.py` & `docusign-click-1.4.0/docusign_click/models/document.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/document_conversion_request.py` & `docusign-click-1.4.0/docusign_click/models/document_conversion_request.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/document_conversion_response.py` & `docusign-click-1.4.0/docusign_click/models/document_conversion_response.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/document_data.py` & `docusign-click-1.4.0/docusign_click/models/document_data.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/error_details.py` & `docusign-click-1.4.0/docusign_click/models/error_details.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/html_result.py` & `docusign-click-1.4.0/docusign_click/models/html_result.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/service_information.py` & `docusign-click-1.4.0/docusign_click/models/service_information.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/service_version.py` & `docusign-click-1.4.0/docusign_click/models/service_version.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/user_agreement_request.py` & `docusign-click-1.4.0/docusign_click/models/user_agreement_request.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/docusign_click/models/user_agreement_response.py` & `docusign-click-1.4.0/docusign_click/models/user_agreement_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'declined_on': 'object',
         'document_data': 'dict(str, str)',
         'documents': 'list[Document]',
         'metadata': 'str',
         'return_url': 'str',
         'settings': 'DisplaySettings',
         'status': 'str',
-        'style': 'dict(str, str)',
+        'style': 'UserAgreementResponseStyle',
         'version': 'str',
         'version_id': 'str',
         'version_number': 'int'
     }
 
     attribute_map = {
         'account_id': 'accountId',
@@ -522,29 +522,27 @@
 
         self._status = status
 
     @property
     def style(self):
         """Gets the style of this UserAgreementResponse.  # noqa: E501
 
-        This property specifies the custom style provided when the agreement was created by [customizing the template appearance][].    [customizing the template appearance]: /docs/click-api/click101/customize-elastic-template-appearance/   # noqa: E501
 
         :return: The style of this UserAgreementResponse.  # noqa: E501
-        :rtype: dict(str, str)
+        :rtype: UserAgreementResponseStyle
         """
         return self._style
 
     @style.setter
     def style(self, style):
         """Sets the style of this UserAgreementResponse.
 
-        This property specifies the custom style provided when the agreement was created by [customizing the template appearance][].    [customizing the template appearance]: /docs/click-api/click101/customize-elastic-template-appearance/   # noqa: E501
 
         :param style: The style of this UserAgreementResponse.  # noqa: E501
-        :type: dict(str, str)
+        :type: UserAgreementResponseStyle
         """
 
         self._style = style
 
     @property
     def version(self):
         """Gets the version of this UserAgreementResponse.  # noqa: E501
```

### Comparing `docusign-click-1.3.0/docusign_click.egg-info/PKG-INFO` & `docusign-click-1.4.0/docusign_click.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docusign-click
-Version: 1.3.0
+Version: 1.4.0
 Summary: DocuSign Click API
 Home-page: 
 Author-email: devcenter@docusign.com
 Keywords: Swagger,DocuSign Click API
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docusign-click Version: 1.3.0 Summary: DocuSign
+Metadata-Version: 2.1 Name: docusign-click Version: 1.4.0 Summary: DocuSign
 Click API Home-page: Author-email: devcenter@docusign.com Keywords:
 Swagger,DocuSign Click API Description-Content-Type: text/markdown License-
 File: LICENSE # The Official DocuSign Click Python Client [![PyPI version]
 [pypi-image]][pypi-url]  [![Build status][travis-image]][travis-url] [PyPI
 module](https://pypi.python.org/pypi/docusign_click) that wraps the DocuSign
 Click API [Documentation about the DocuSign Click API](https://
 developers.docusign.com/) ## Requirements - Python 2.7 (3.7+ recommended) -
```

### Comparing `docusign-click-1.3.0/docusign_click.egg-info/SOURCES.txt` & `docusign-click-1.4.0/docusign_click.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 docusign_click/client/api_client.py
 docusign_click/client/api_exception.py
 docusign_click/client/api_response.py
 docusign_click/client/configuration.py
 docusign_click/client/auth/__init__.py
 docusign_click/client/auth/oauth.py
 docusign_click/models/__init__.py
+docusign_click/models/agree_button_styles.py
+docusign_click/models/agreement_statement_styles.py
+docusign_click/models/base_agree_button_styles.py
 docusign_click/models/bulk_clickwrap_request.py
 docusign_click/models/clickwrap_agreements_response.py
 docusign_click/models/clickwrap_delete_response.py
 docusign_click/models/clickwrap_request.py
 docusign_click/models/clickwrap_response.py
 docusign_click/models/clickwrap_scheduled_reacceptance.py
 docusign_click/models/clickwrap_summary_response.py
@@ -32,23 +35,29 @@
 docusign_click/models/clickwrap_version_response.py
 docusign_click/models/clickwrap_version_summary_response.py
 docusign_click/models/clickwrap_versions_delete_response.py
 docusign_click/models/clickwrap_versions_paged_response.py
 docusign_click/models/clickwrap_versions_response.py
 docusign_click/models/clickwraps_delete_response.py
 docusign_click/models/clickwraps_response.py
+docusign_click/models/container_styles.py
 docusign_click/models/conversion_document.py
 docusign_click/models/data_field.py
+docusign_click/models/disclosure_link_styles.py
 docusign_click/models/display_settings.py
 docusign_click/models/document.py
 docusign_click/models/document_conversion_request.py
 docusign_click/models/document_conversion_response.py
 docusign_click/models/document_data.py
+docusign_click/models/document_link_styles.py
+docusign_click/models/document_link_styles_focus.py
 docusign_click/models/error_details.py
+docusign_click/models/header_styles.py
 docusign_click/models/html_result.py
 docusign_click/models/service_information.py
 docusign_click/models/service_version.py
 docusign_click/models/user_agreement_request.py
 docusign_click/models/user_agreement_response.py
+docusign_click/models/user_agreement_response_style.py
 test/__init__.py
 test/test_oauth.py
 test/unit_tests.py
```

### Comparing `docusign-click-1.3.0/setup.py` & `docusign-click-1.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages, Command, os  # noqa: H301	
 
 NAME = "docusign-click"
-VERSION = "1.3.0"
+VERSION = "1.4.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `docusign-click-1.3.0/test/test_oauth.py` & `docusign-click-1.4.0/test/test_oauth.py`

 * *Files identical despite different names*

### Comparing `docusign-click-1.3.0/test/unit_tests.py` & `docusign-click-1.4.0/test/unit_tests.py`

 * *Files identical despite different names*

