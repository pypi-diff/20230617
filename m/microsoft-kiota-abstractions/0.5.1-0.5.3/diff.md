# Comparing `tmp/microsoft-kiota-abstractions-0.5.1.tar.gz` & `tmp/microsoft_kiota_abstractions-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft-kiota-abstractions-0.5.1.tar", last modified: Wed May  3 10:16:24 2023, max compression
+gzip compressed data, was "microsoft_kiota_abstractions-0.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft-kiota-abstractions-0.5.1.tar` & `microsoft_kiota_abstractions-0.5.3.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0       82 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1732 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2538 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.gitignore
--rw-r--r--   0        0        0    15931 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.pylintrc
--rw-r--r--   0        0        0      687 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/LICENSE
--rw-r--r--   0        0        0      285 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/Pipfile
--rw-r--r--   0        0        0    29636 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/Pipfile.lock
--rw-r--r--   0        0        0     2512 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/README.md
--rw-r--r--   0        0        0     2757 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/SUPPORT.md
--rw-r--r--   0        0        0      119 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/__init__.py
--rw-r--r--   0        0        0       23 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/_version.py
--rw-r--r--   0        0        0     3566 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/api_client_builder.py
--rw-r--r--   0        0        0      962 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/api_error.py
--rw-r--r--   0        0        0      346 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/__init__.py
--rw-r--r--   0        0        0      836 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/access_token_provider.py
--rw-r--r--   0        0        0     2175 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/allowed_hosts_validator.py
--rw-r--r--   0        0        0      607 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/anonymous_authentication_provider.py
--rw-r--r--   0        0        0      473 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/authentication_provider.py
--rw-r--r--   0        0        0     1231 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py
--rw-r--r--   0        0        0      453 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/get_path_parameters.py
--rw-r--r--   0        0        0      529 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/method.py
--rw-r--r--   0        0        0      938 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/native_response_handler.py
--rw-r--r--   0        0        0     5164 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/request_adapter.py
--rw-r--r--   0        0        0     9048 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/request_information.py
--rw-r--r--   0        0        0      312 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/request_option.py
--rw-r--r--   0        0        0      965 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/response_handler.py
--rw-r--r--   0        0        0      632 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/__init__.py
--rw-r--r--   0        0        0      493 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/additional_data_holder.py
--rw-r--r--   0        0        0      961 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parsable.py
--rw-r--r--   0        0        0      642 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parsable_factory.py
--rw-r--r--   0        0        0     5793 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node.py
--rw-r--r--   0        0        0      903 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node_factory.py
--rw-r--r--   0        0        0     1972 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node_factory_registry.py
--rw-r--r--   0        0        0     2424 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node_proxy_factory.py
--rw-r--r--   0        0        0     9547 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer.py
--rw-r--r--   0        0        0      898 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer_factory.py
--rw-r--r--   0        0        0     2025 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer_factory_registry.py
--rw-r--r--   0        0        0     3132 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer_proxy_factory.py
--rw-r--r--   0        0        0      529 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/__init__.py
--rw-r--r--   0        0        0      398 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backed_model.py
--rw-r--r--   0        0        0     3892 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store.py
--rw-r--r--   0        0        0      424 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store_factory.py
--rw-r--r--   0        0        0      237 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store_factory_singleton.py
--rw-r--r--   0        0        0     1166 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store_parse_node_factory.py
--rw-r--r--   0        0        0     1809 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py
--rw-r--r--   0        0        0     4488 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/in_memory_backing_store.py
--rw-r--r--   0        0        0      380 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/in_memory_backing_store_factory.py
--rw-r--r--   0        0        0      899 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/utils.py
--rw-r--r--   0        0        0     1268 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/tests/authentication/__init__.py
--rw-r--r--   0        0        0     1041 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/tests/authentication/test_base_bearer_token_authentication.py
--rw-r--r--   0        0        0      831 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/tests/conftest.py
--rw-r--r--   0        0        0     5109 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/tests/test_request_information.py
--rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 microsoft-kiota-abstractions-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       82 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1927 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2538 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1097 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1799 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/.gitignore
+-rw-r--r--   0        0        0    15931 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/.pylintrc
+-rw-r--r--   0        0        0      867 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2512 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/README.md
+-rw-r--r--   0        0        0     2757 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/SUPPORT.md
+-rw-r--r--   0        0        0      119 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/_version.py
+-rw-r--r--   0        0        0     3566 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/api_client_builder.py
+-rw-r--r--   0        0        0      399 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/api_error.py
+-rw-r--r--   0        0        0      346 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/authentication/__init__.py
+-rw-r--r--   0        0        0      836 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/authentication/access_token_provider.py
+-rw-r--r--   0        0        0     2120 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/authentication/allowed_hosts_validator.py
+-rw-r--r--   0        0        0      607 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/authentication/anonymous_authentication_provider.py
+-rw-r--r--   0        0        0      473 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/authentication/authentication_provider.py
+-rw-r--r--   0        0        0     1231 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py
+-rw-r--r--   0        0        0      453 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/get_path_parameters.py
+-rw-r--r--   0        0        0      529 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/method.py
+-rw-r--r--   0        0        0      938 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/native_response_handler.py
+-rw-r--r--   0        0        0     5164 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/request_adapter.py
+-rw-r--r--   0        0        0     9048 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/request_information.py
+-rw-r--r--   0        0        0      312 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/request_option.py
+-rw-r--r--   0        0        0      965 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/response_handler.py
+-rw-r--r--   0        0        0      679 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/__init__.py
+-rw-r--r--   0        0        0      374 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/additional_data_holder.py
+-rw-r--r--   0        0        0     1006 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parsable.py
+-rw-r--r--   0        0        0      642 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parsable_factory.py
+-rw-r--r--   0        0        0     5793 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parse_node.py
+-rw-r--r--   0        0        0      903 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parse_node_factory.py
+-rw-r--r--   0        0        0     1972 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parse_node_factory_registry.py
+-rw-r--r--   0        0        0      948 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parse_node_helper.py
+-rw-r--r--   0        0        0     2424 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parse_node_proxy_factory.py
+-rw-r--r--   0        0        0     9768 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/serialization_writer.py
+-rw-r--r--   0        0        0      898 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/serialization_writer_factory.py
+-rw-r--r--   0        0        0     2025 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/serialization_writer_factory_registry.py
+-rw-r--r--   0        0        0     3132 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/serialization_writer_proxy_factory.py
+-rw-r--r--   0        0        0      529 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/__init__.py
+-rw-r--r--   0        0        0      398 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/backed_model.py
+-rw-r--r--   0        0        0     3892 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/backing_store.py
+-rw-r--r--   0        0        0      424 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/backing_store_factory.py
+-rw-r--r--   0        0        0      237 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/backing_store_factory_singleton.py
+-rw-r--r--   0        0        0     1166 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/backing_store_parse_node_factory.py
+-rw-r--r--   0        0        0     1809 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py
+-rw-r--r--   0        0        0     4488 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/in_memory_backing_store.py
+-rw-r--r--   0        0        0      380 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/in_memory_backing_store_factory.py
+-rw-r--r--   0        0        0      899 2023-06-17 21:30:33.271239 microsoft_kiota_abstractions-0.5.3/kiota_abstractions/utils.py
+-rw-r--r--   0        0        0     1268 2023-06-17 21:30:33.275239 microsoft_kiota_abstractions-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1130 2023-06-17 21:30:33.275239 microsoft_kiota_abstractions-0.5.3/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-06-17 21:30:33.275239 microsoft_kiota_abstractions-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 21:30:33.275239 microsoft_kiota_abstractions-0.5.3/tests/authentication/__init__.py
+-rw-r--r--   0        0        0     1041 2023-06-17 21:30:33.275239 microsoft_kiota_abstractions-0.5.3/tests/authentication/test_base_bearer_token_authentication.py
+-rw-r--r--   0        0        0      831 2023-06-17 21:30:33.275239 microsoft_kiota_abstractions-0.5.3/tests/conftest.py
+-rw-r--r--   0        0        0     5109 2023-06-17 21:30:33.275239 microsoft_kiota_abstractions-0.5.3/tests/test_request_information.py
+-rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 microsoft_kiota_abstractions-0.5.3/PKG-INFO
```

### Comparing `microsoft-kiota-abstractions-0.5.1/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_abstractions-0.5.3/.github/workflows/auto-merge-dependabot.yml`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     runs-on: ubuntu-latest
 
     if: ${{ github.actor == 'dependabot[bot]' }}
 
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.4.0
+        uses: dependabot/fetch-metadata@v1.5.1
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
 
       - name: Enable auto-merge for Dependabot PRs
         # Only if version bump is not a major version change
         if: ${{steps.metadata.outputs.update-type != 'version-update:semver-major'}}
         run: gh pr merge --auto --merge "$PR_URL"
```

### Comparing `microsoft-kiota-abstractions-0.5.1/.github/workflows/ci.yml` & `microsoft_kiota_abstractions-0.5.3/.github/workflows/build.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,50 @@
-name: Python abstractions
+# This workflow will install Python dependencies, run tests and lint with a variety of Python versions
+# For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
+
+name: Build and Test
 
 on:
   workflow_dispatch:
   push:
-    branches: [ main ]
+    branches: [main]
   pull_request:
-    branches: [ main, dev ]
+    branches: [main, dev]
 
 jobs:
   build:
     runs-on: ubuntu-latest
+    timeout-minutes: 40
     strategy:
+      max-parallel: 5
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - name: Checkout
         uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install pipenv
-          pipenv install --dev --skip-lock
+          pip install -r requirements-dev.txt
       - name: Check code format
         run: |
-          pipenv run yapf -dr kiota_abstractions
+          yapf -dr kiota_abstractions
       - name: Check import order
         run: |
-          pipenv run isort kiota_abstractions
+          isort kiota_abstractions
       - name: Lint with Pylint
         run: |
-          pipenv run pylint kiota_abstractions --disable=W --rcfile=.pylintrc
+          pylint kiota_abstractions --disable=W --rcfile=.pylintrc
       - name: Static type checking with Mypy
         run: |
-          pipenv run mypy kiota_abstractions
+          mypy kiota_abstractions
 
   publish:
     name: Publish distribution to PyPI
     if: ${{ github.ref == 'refs/heads/main' }}
     runs-on: ubuntu-latest
     environment: pypi_prod
     needs: [build]
```

### Comparing `microsoft-kiota-abstractions-0.5.1/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_abstractions-0.5.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_abstractions-0.5.3/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/.gitignore` & `microsoft_kiota_abstractions-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/.pylintrc` & `microsoft_kiota_abstractions-0.5.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/CHANGELOG.md` & `microsoft_kiota_abstractions-0.5.3/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+
+## [0.5.2] - 2023-06-05
+
+### Added
+
+### Changed
+
+- Changed Parsable and APIError to dataclasses.
+- Added support for merging of object values for intersection types
+
 ## [0.5.1] - 2023-04-29
 
 ### Added
 
 - Adds the response headers to the APIError class.
 
+### Changed
+
 ## [0.5.0] - 2023-02-07
 
 ### Added
 
 - Added support for multi-valued request headers.
 
 ### Changed
```

### Comparing `microsoft-kiota-abstractions-0.5.1/LICENSE` & `microsoft_kiota_abstractions-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/README.md` & `microsoft_kiota_abstractions-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/SECURITY.md` & `microsoft_kiota_abstractions-0.5.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/SUPPORT.md` & `microsoft_kiota_abstractions-0.5.3/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/api_client_builder.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/api_client_builder.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/access_token_provider.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/authentication/access_token_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/allowed_hosts_validator.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/authentication/allowed_hosts_validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,19 +45,14 @@
             url (str): The url to check.
 
         Returns:
             bool: [description]
         """
         if not url:
             return False
-        if not self.allowed_hosts:
+        if not self.get_allowed_hosts():
             return True
-
         # Format: urlparse("scheme://netloc/path;parameters?query#fragment")
-        #Returns: ParseResult(scheme='scheme', netloc='netloc', path='/path;parameters', params='',
+        # Returns: ParseResult(scheme='scheme', netloc='netloc', path='/path;parameters', params='',
         #    query='query', fragment='fragment')
         o = urlparse(url)
-
-        if o.netloc:
-            return o.netloc.lower() in self.allowed_hosts
-
-        return False
+        return all([o.scheme, o.netloc])
```

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/anonymous_authentication_provider.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/authentication/anonymous_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/method.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/method.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/native_response_handler.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/native_response_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/request_adapter.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/request_adapter.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/request_information.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/request_information.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/response_handler.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/response_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/__init__.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .additional_data_holder import AdditionalDataHolder
 from .parsable import Parsable
 from .parsable_factory import ParsableFactory
 from .parse_node import ParseNode
 from .parse_node_factory import ParseNodeFactory
 from .parse_node_factory_registry import ParseNodeFactoryRegistry
+from .parse_node_helper import ParseNodeHelper
 from .parse_node_proxy_factory import ParseNodeProxyFactory
 from .serialization_writer import SerializationWriter
 from .serialization_writer_factory import SerializationWriterFactory
 from .serialization_writer_factory_registry import SerializationWriterFactoryRegistry
 from .serialization_writer_proxy_factory import SerializationWriterProxyFactory
```

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parsable.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parsable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from abc import ABC, abstractmethod
+from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Callable, Dict, TypeVar
 
 T = TypeVar("T")
 
 if TYPE_CHECKING:
     from .parse_node import ParseNode
     from .serialization_writer import SerializationWriter
 
 
+@dataclass
 class Parsable(ABC):
     """
     Defines a serializable model object.
     """
 
     @abstractmethod
     def get_field_deserializers(self) -> Dict[str, Callable[['ParseNode'], None]]:
```

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parsable_factory.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parsable_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parse_node.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node_factory.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node_factory_registry.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parse_node_factory_registry.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node_proxy_factory.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/parse_node_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/serialization_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,20 +153,24 @@
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (BytesIO): The byte array to be written.
         """
         pass
 
     @abstractmethod
-    def write_object_value(self, key: Optional[str], value: U) -> None:
+    def write_object_value(
+        self, key: Optional[str], value: U, additional_values_to_merge: Optional[List[U]]
+    ) -> None:
         """Writes the specified model object to the stream with an optional given key.
 
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Parsable): The model object to be written.
+            additional_values_to_merge (List[Parsable]): The additional values to merge to the
+            main value when serializing an intersection wrapper.
         """
         pass
 
     @abstractmethod
     def write_enum_value(self, key: Optional[str], value: Optional[Enum]) -> None:
         """Writes the specified enum value to the stream with an optional given key.
```

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer_factory.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer_factory_registry.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/serialization_writer_factory_registry.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer_proxy_factory.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/serialization/serialization_writer_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/__init__.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/__init__.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/backing_store.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store_parse_node_factory.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/backing_store_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/in_memory_backing_store.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/store/in_memory_backing_store.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/utils.py` & `microsoft_kiota_abstractions-0.5.3/kiota_abstractions/utils.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/pyproject.toml` & `microsoft_kiota_abstractions-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/tests/authentication/test_base_bearer_token_authentication.py` & `microsoft_kiota_abstractions-0.5.3/tests/authentication/test_base_bearer_token_authentication.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/tests/conftest.py` & `microsoft_kiota_abstractions-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/tests/test_request_information.py` & `microsoft_kiota_abstractions-0.5.3/tests/test_request_information.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.1/PKG-INFO` & `microsoft_kiota_abstractions-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-abstractions
-Version: 0.5.1
+Version: 0.5.3
 Summary: Core abstractions for kiota generated libraries in Python
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

