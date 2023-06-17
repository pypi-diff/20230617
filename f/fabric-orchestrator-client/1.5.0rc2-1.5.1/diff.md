# Comparing `tmp/fabric-orchestrator-client-1.5.0rc2.tar.gz` & `tmp/fabric-orchestrator-client-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-orchestrator-client-1.5.0rc2.tar", last modified: Fri May 12 13:46:59 2023, max compression
+gzip compressed data, was "fabric-orchestrator-client-1.5.1.tar", last modified: Sat Jun 17 10:06:11 2023, max compression
```

## Comparing `fabric-orchestrator-client-1.5.0rc2.tar` & `fabric-orchestrator-client-1.5.1.tar`

### file list

```diff
@@ -1,81 +1,101 @@
--rw-r--r--   0        0        0      793 2023-05-11 17:37:01.210207 fabric-orchestrator-client-1.5.0rc2/.gitignore
--rw-r--r--   0        0        0     1030 2023-05-11 17:37:01.210355 fabric-orchestrator-client-1.5.0rc2/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2023-05-11 17:37:01.210524 fabric-orchestrator-client-1.5.0rc2/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2023-05-11 17:37:01.210626 fabric-orchestrator-client-1.5.0rc2/.travis.yml
--rw-r--r--   0        0        0      770 2023-05-11 17:37:01.210729 fabric-orchestrator-client-1.5.0rc2/CODEGEN.md
--rw-r--r--   0        0        0     1071 2023-05-11 17:37:01.210862 fabric-orchestrator-client-1.5.0rc2/LICENSE
--rw-r--r--   0        0        0       59 2023-05-11 17:37:01.210963 fabric-orchestrator-client-1.5.0rc2/MANIFEST.in
--rw-r--r--   0        0        0     9238 2023-05-11 17:37:01.211113 fabric-orchestrator-client-1.5.0rc2/README.md
--rw-r--r--   0        0        0     4263 2023-05-11 17:37:01.211350 fabric-orchestrator-client-1.5.0rc2/docs/ResourcesApi.md
--rw-r--r--   0        0        0    17437 2023-05-11 17:37:01.211531 fabric-orchestrator-client-1.5.0rc2/docs/SlicesApi.md
--rw-r--r--   0        0        0     3740 2023-05-11 17:37:01.211677 fabric-orchestrator-client-1.5.0rc2/docs/SliversApi.md
--rw-r--r--   0        0        0      335 2023-05-11 17:37:01.211789 fabric-orchestrator-client-1.5.0rc2/docs/Success.md
--rw-r--r--   0        0        0      352 2023-05-11 17:37:01.211912 fabric-orchestrator-client-1.5.0rc2/docs/Version.md
--rw-r--r--   0        0        0       25 2023-05-12 13:46:55.675728 fabric-orchestrator-client-1.5.0rc2/fabric_cf/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 17:37:01.212158 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0        0        0    18242 2023-05-11 17:37:01.212367 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/orchestrator_proxy.py
--rw-r--r--   0        0        0     3004 2023-05-11 17:37:01.212646 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/__init__.py
--rw-r--r--   0        0        0      397 2023-05-11 17:37:01.212849 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/__init__.py
--rw-r--r--   0        0        0     9597 2023-05-11 17:37:01.213024 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/resources_api.py
--rw-r--r--   0        0        0    37827 2023-05-11 17:37:01.213284 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/slices_api.py
--rw-r--r--   0        0        0     8826 2023-05-11 17:37:01.213492 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
--rw-r--r--   0        0        0     3748 2023-05-11 17:37:01.213724 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25128 2023-05-11 17:37:01.213944 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api_client.py
--rw-r--r--   0        0        0     8240 2023-05-11 17:37:01.214372 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/configuration.py
--rw-r--r--   0        0        0     2496 2023-05-11 17:37:01.214654 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     3055 2023-05-11 17:37:01.214908 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/resource.py
--rw-r--r--   0        0        0     3420 2023-05-11 17:37:01.215233 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/resources.py
--rw-r--r--   0        0        0     8496 2023-05-11 17:37:01.215453 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slice.py
--rw-r--r--   0        0        0     3435 2023-05-11 17:37:01.215578 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slice_details.py
--rw-r--r--   0        0        0     3412 2023-05-11 17:37:01.215680 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slices.py
--rw-r--r--   0        0        0    10903 2023-05-11 17:37:01.215821 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/sliver.py
--rw-r--r--   0        0        0     3422 2023-05-11 17:37:01.216181 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slivers.py
--rw-r--r--   0        0        0     4999 2023-05-11 17:37:01.216373 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3832 2023-05-11 17:37:01.216668 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     6211 2023-05-11 17:37:01.216937 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     4253 2023-05-11 17:37:01.217164 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3163 2023-05-11 17:37:01.217341 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5771 2023-05-11 17:37:01.217534 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5063 2023-05-11 17:37:01.217713 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3870 2023-05-11 17:37:01.217919 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     4994 2023-05-11 17:37:01.218148 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3831 2023-05-11 17:37:01.218431 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4971 2023-05-11 17:37:01.218623 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3819 2023-05-11 17:37:01.218944 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5224 2023-05-11 17:37:01.219262 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3963 2023-05-11 17:37:01.219487 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     3413 2023-05-11 17:37:01.219669 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/version.py
--rw-r--r--   0        0        0     3882 2023-05-11 17:37:01.219920 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    12988 2023-05-11 17:37:01.220174 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2023-05-11 17:37:01.220383 fabric-orchestrator-client-1.5.0rc2/git_push.sh
--rw-r--r--   0        0        0     1026 2023-05-12 13:46:49.514872 fabric-orchestrator-client-1.5.0rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 17:37:01.221004 fabric-orchestrator-client-1.5.0rc2/test/__init__.py
--rw-r--r--   0        0        0      896 2023-05-11 17:37:01.221224 fabric-orchestrator-client-1.5.0rc2/test/test_resource.py
--rw-r--r--   0        0        0      950 2023-05-11 17:37:01.221397 fabric-orchestrator-client-1.5.0rc2/test/test_resources.py
--rw-r--r--   0        0        0     1206 2023-05-11 17:37:01.221693 fabric-orchestrator-client-1.5.0rc2/test/test_resources_api.py
--rw-r--r--   0        0        0      872 2023-05-11 17:37:01.221929 fabric-orchestrator-client-1.5.0rc2/test/test_slice.py
--rw-r--r--   0        0        0      930 2023-05-11 17:37:01.222101 fabric-orchestrator-client-1.5.0rc2/test/test_slice_details.py
--rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222270 fabric-orchestrator-client-1.5.0rc2/test/test_slices.py
--rw-r--r--   0        0        0     2018 2023-05-11 17:37:01.222442 fabric-orchestrator-client-1.5.0rc2/test/test_slices_api.py
--rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222608 fabric-orchestrator-client-1.5.0rc2/test/test_sliver.py
--rw-r--r--   0        0        0      888 2023-05-11 17:37:01.222785 fabric-orchestrator-client-1.5.0rc2/test/test_slivers.py
--rw-r--r--   0        0        0      998 2023-05-11 17:37:01.223106 fabric-orchestrator-client-1.5.0rc2/test/test_slivers_api.py
--rw-r--r--   0        0        0      998 2023-05-11 17:37:01.223296 fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1032 2023-05-11 17:37:01.223607 fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      996 2023-05-11 17:37:01.223847 fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_paginated.py
--rw-r--r--   0        0        0      972 2023-05-11 17:37:01.224081 fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      988 2023-05-11 17:37:01.224292 fabric-orchestrator-client-1.5.0rc2/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1038 2023-05-11 17:37:01.224535 fabric-orchestrator-client-1.5.0rc2/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0     1002 2023-05-11 17:37:01.224771 fabric-orchestrator-client-1.5.0rc2/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1052 2023-05-11 17:37:01.225030 fabric-orchestrator-client-1.5.0rc2/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      978 2023-05-11 17:37:01.225269 fabric-orchestrator-client-1.5.0rc2/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1028 2023-05-11 17:37:01.225554 fabric-orchestrator-client-1.5.0rc2/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      972 2023-05-11 17:37:01.225840 fabric-orchestrator-client-1.5.0rc2/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1022 2023-05-11 17:37:01.226137 fabric-orchestrator-client-1.5.0rc2/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1062 2023-05-11 17:37:01.226327 fabric-orchestrator-client-1.5.0rc2/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1112 2023-05-11 17:37:01.226547 fabric-orchestrator-client-1.5.0rc2/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      888 2023-05-11 17:37:01.226964 fabric-orchestrator-client-1.5.0rc2/test/test_version.py
--rw-r--r--   0        0        0      814 2023-05-11 17:37:01.227150 fabric-orchestrator-client-1.5.0rc2/test/test_version_api.py
--rw-r--r--   0        0        0      922 2023-05-11 17:37:01.227332 fabric-orchestrator-client-1.5.0rc2/test/test_version_data.py
--rw-r--r--   0        0        0      143 2023-05-11 17:37:01.227515 fabric-orchestrator-client-1.5.0rc2/tox.ini
--rw-r--r--   0        0        0    10192 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.5.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      793 2023-05-11 17:37:01.210207 fabric-orchestrator-client-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1030 2023-05-11 17:37:01.210355 fabric-orchestrator-client-1.5.1/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2023-06-10 11:27:02.431890 fabric-orchestrator-client-1.5.1/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2023-05-11 17:37:01.210626 fabric-orchestrator-client-1.5.1/.travis.yml
+-rw-r--r--   0        0        0      770 2023-05-11 17:37:01.210729 fabric-orchestrator-client-1.5.1/CODEGEN.md
+-rw-r--r--   0        0        0     1071 2023-05-11 17:37:01.210862 fabric-orchestrator-client-1.5.1/LICENSE
+-rw-r--r--   0        0        0       59 2023-05-11 17:37:01.210963 fabric-orchestrator-client-1.5.1/MANIFEST.in
+-rw-r--r--   0        0        0     9867 2023-06-12 16:30:43.340015 fabric-orchestrator-client-1.5.1/README.md
+-rw-r--r--   0        0        0      340 2023-06-10 11:27:02.433089 fabric-orchestrator-client-1.5.1/docs/Poa.md
+-rw-r--r--   0        0        0      557 2023-06-12 16:30:43.340871 fabric-orchestrator-client-1.5.1/docs/PoaData.md
+-rw-r--r--   0        0        0      376 2023-06-10 11:27:02.434037 fabric-orchestrator-client-1.5.1/docs/PoaPost.md
+-rw-r--r--   0        0        0      430 2023-06-10 11:27:02.434323 fabric-orchestrator-client-1.5.1/docs/PoaPostData.md
+-rw-r--r--   0        0        0      369 2023-06-10 11:27:02.434841 fabric-orchestrator-client-1.5.1/docs/PoaPostDataVcpuCpuMap.md
+-rw-r--r--   0        0        0     6404 2023-06-12 16:30:43.341529 fabric-orchestrator-client-1.5.1/docs/PoasApi.md
+-rw-r--r--   0        0        0     4263 2023-05-11 17:37:01.211350 fabric-orchestrator-client-1.5.1/docs/ResourcesApi.md
+-rw-r--r--   0        0        0    20667 2023-06-12 16:30:43.341882 fabric-orchestrator-client-1.5.1/docs/SlicesApi.md
+-rw-r--r--   0        0        0     4102 2023-06-12 16:30:43.342523 fabric-orchestrator-client-1.5.1/docs/SliversApi.md
+-rw-r--r--   0        0        0      335 2023-05-11 17:37:01.211789 fabric-orchestrator-client-1.5.1/docs/Success.md
+-rw-r--r--   0        0        0      352 2023-05-11 17:37:01.211912 fabric-orchestrator-client-1.5.1/docs/Version.md
+-rw-r--r--   0        0        0       22 2023-06-17 09:55:40.714963 fabric-orchestrator-client-1.5.1/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:37:01.212158 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0    21840 2023-06-12 16:30:43.343170 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/orchestrator_proxy.py
+-rw-r--r--   0        0        0     3557 2023-06-12 16:30:43.344093 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/__init__.py
+-rw-r--r--   0        0        0      468 2023-06-12 16:30:43.344852 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0    13515 2023-06-12 16:30:43.345710 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/poas_api.py
+-rw-r--r--   0        0        0     9597 2023-05-11 17:37:01.213024 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/resources_api.py
+-rw-r--r--   0        0        0    44360 2023-06-12 17:06:53.843598 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/slices_api.py
+-rw-r--r--   0        0        0     9260 2023-06-12 16:30:43.347087 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
+-rw-r--r--   0        0        0     3748 2023-05-11 17:37:01.213724 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25128 2023-05-11 17:37:01.213944 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8240 2023-05-11 17:37:01.214372 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/configuration.py
+-rw-r--r--   0        0        0     2978 2023-06-10 11:27:02.438784 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     3427 2023-06-10 11:27:02.439359 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa.py
+-rw-r--r--   0        0        0     6654 2023-06-12 16:30:43.348013 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa_data.py
+-rw-r--r--   0        0        0     4034 2023-06-10 11:27:02.440677 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa_post.py
+-rw-r--r--   0        0        0     3878 2023-06-10 11:27:02.441305 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
+-rw-r--r--   0        0        0     3648 2023-06-10 11:27:02.441612 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     3055 2023-05-11 17:37:01.214908 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/resource.py
+-rw-r--r--   0        0        0     3420 2023-05-11 17:37:01.215233 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/resources.py
+-rw-r--r--   0        0        0     8496 2023-05-11 17:37:01.215453 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slice.py
+-rw-r--r--   0        0        0     3444 2023-06-12 16:30:43.348954 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slice_details.py
+-rw-r--r--   0        0        0     3412 2023-05-11 17:37:01.215680 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slices.py
+-rw-r--r--   0        0        0     3951 2023-06-10 11:27:02.442381 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slices_post.py
+-rw-r--r--   0        0        0    10905 2023-06-10 11:27:02.443007 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/sliver.py
+-rw-r--r--   0        0        0     3422 2023-05-11 17:37:01.216181 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slivers.py
+-rw-r--r--   0        0        0     4999 2023-05-11 17:37:01.216373 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3832 2023-05-11 17:37:01.216668 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     6211 2023-05-11 17:37:01.216937 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4253 2023-05-11 17:37:01.217164 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3163 2023-05-11 17:37:01.217341 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5771 2023-05-11 17:37:01.217534 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5063 2023-05-11 17:37:01.217713 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3870 2023-05-11 17:37:01.217919 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     4994 2023-05-11 17:37:01.218148 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3831 2023-05-11 17:37:01.218431 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4971 2023-05-11 17:37:01.218623 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3819 2023-05-11 17:37:01.218944 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5224 2023-05-11 17:37:01.219262 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3963 2023-05-11 17:37:01.219487 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3413 2023-05-11 17:37:01.219669 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3882 2023-05-11 17:37:01.219920 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    12988 2023-05-11 17:37:01.220174 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2023-05-11 17:37:01.220383 fabric-orchestrator-client-1.5.1/git_push.sh
+-rw-r--r--   0        0        0     1024 2023-06-17 09:55:40.699613 fabric-orchestrator-client-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-06-10 11:27:02.444133 fabric-orchestrator-client-1.5.1/test/__init__.py
+-rw-r--r--   0        0        0      809 2023-06-10 11:27:02.444942 fabric-orchestrator-client-1.5.1/test/test_poa.py
+-rw-r--r--   0        0        0      843 2023-06-10 11:27:02.445598 fabric-orchestrator-client-1.5.1/test/test_poa_data.py
+-rw-r--r--   0        0        0      843 2023-06-10 11:27:02.446320 fabric-orchestrator-client-1.5.1/test/test_poa_post.py
+-rw-r--r--   0        0        0      877 2023-06-10 11:27:02.447271 fabric-orchestrator-client-1.5.1/test/test_poa_post_data.py
+-rw-r--r--   0        0        0      963 2023-06-10 11:27:02.448091 fabric-orchestrator-client-1.5.1/test/test_poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     1157 2023-06-12 16:30:43.349539 fabric-orchestrator-client-1.5.1/test/test_poas_api.py
+-rw-r--r--   0        0        0      896 2023-05-11 17:37:01.221224 fabric-orchestrator-client-1.5.1/test/test_resource.py
+-rw-r--r--   0        0        0      950 2023-05-11 17:37:01.221397 fabric-orchestrator-client-1.5.1/test/test_resources.py
+-rw-r--r--   0        0        0     1206 2023-05-11 17:37:01.221693 fabric-orchestrator-client-1.5.1/test/test_resources_api.py
+-rw-r--r--   0        0        0      872 2023-05-11 17:37:01.221929 fabric-orchestrator-client-1.5.1/test/test_slice.py
+-rw-r--r--   0        0        0      930 2023-05-11 17:37:01.222101 fabric-orchestrator-client-1.5.1/test/test_slice_details.py
+-rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222270 fabric-orchestrator-client-1.5.1/test/test_slices.py
+-rw-r--r--   0        0        0     2165 2023-06-12 16:30:43.349919 fabric-orchestrator-client-1.5.1/test/test_slices_api.py
+-rw-r--r--   0        0        0      867 2023-06-10 11:27:02.448859 fabric-orchestrator-client-1.5.1/test/test_slices_post.py
+-rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222608 fabric-orchestrator-client-1.5.1/test/test_sliver.py
+-rw-r--r--   0        0        0      888 2023-05-11 17:37:01.222785 fabric-orchestrator-client-1.5.1/test/test_slivers.py
+-rw-r--r--   0        0        0      974 2023-06-12 16:30:43.350780 fabric-orchestrator-client-1.5.1/test/test_slivers_api.py
+-rw-r--r--   0        0        0      998 2023-05-11 17:37:01.223296 fabric-orchestrator-client-1.5.1/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1032 2023-05-11 17:37:01.223607 fabric-orchestrator-client-1.5.1/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      996 2023-05-11 17:37:01.223847 fabric-orchestrator-client-1.5.1/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      972 2023-05-11 17:37:01.224081 fabric-orchestrator-client-1.5.1/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      988 2023-05-11 17:37:01.224292 fabric-orchestrator-client-1.5.1/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1038 2023-05-11 17:37:01.224535 fabric-orchestrator-client-1.5.1/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0     1002 2023-05-11 17:37:01.224771 fabric-orchestrator-client-1.5.1/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1052 2023-05-11 17:37:01.225030 fabric-orchestrator-client-1.5.1/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      978 2023-05-11 17:37:01.225269 fabric-orchestrator-client-1.5.1/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1028 2023-05-11 17:37:01.225554 fabric-orchestrator-client-1.5.1/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      972 2023-05-11 17:37:01.225840 fabric-orchestrator-client-1.5.1/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1022 2023-05-11 17:37:01.226137 fabric-orchestrator-client-1.5.1/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1062 2023-05-11 17:37:01.226327 fabric-orchestrator-client-1.5.1/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1112 2023-05-11 17:37:01.226547 fabric-orchestrator-client-1.5.1/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      888 2023-05-11 17:37:01.226964 fabric-orchestrator-client-1.5.1/test/test_version.py
+-rw-r--r--   0        0        0      814 2023-05-11 17:37:01.227150 fabric-orchestrator-client-1.5.1/test/test_version_api.py
+-rw-r--r--   0        0        0      922 2023-05-11 17:37:01.227332 fabric-orchestrator-client-1.5.1/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2023-05-11 17:37:01.227515 fabric-orchestrator-client-1.5.1/tox.ini
+-rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.5.1/PKG-INFO
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/.gitignore` & `fabric-orchestrator-client-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/.swagger-codegen-ignore` & `fabric-orchestrator-client-1.5.1/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/CODEGEN.md` & `fabric-orchestrator-client-1.5.1/CODEGEN.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/LICENSE` & `fabric-orchestrator-client-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/README.md` & `fabric-orchestrator-client-1.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,40 @@
+Metadata-Version: 2.1
+Name: fabric-orchestrator-client
+Version: 1.5.1
+Summary: Fabric Orchestrator API
+Keywords: Swagger,Fabric Orchestrator API
+Author-email: Komal Thareja <kthare10@renci.org>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Dist: certifi >= 14.05.14
+Requires-Dist: six >= 1.10
+Requires-Dist: python_dateutil >= 2.5.3
+Requires-Dist: requests>=2.28.1
+Requires-Dist: fabric-fim==1.5.2
+Requires-Dist: coverage>=4.0.3 ; extra == "test"
+Requires-Dist: nose>=1.3.7 ; extra == "test"
+Requires-Dist: pluggy>=0.3.1 ; extra == "test"
+Requires-Dist: py>=1.4.31 ; extra == "test"
+Requires-Dist: randomize>=0.13 ; extra == "test"
+Project-URL: Home, https://fabric-testbed.net/
+Project-URL: Sources, https://github.com/fabric-testbed/OrchestratorClient
+Provides-Extra: test
+
 [![PyPI](https://img.shields.io/pypi/v/fabric-orchestrator-client?style=plastic)](https://pypi.org/project/fabric-orchestrator-client/)
 
 # Fabric Orchestrator swagger-client
 This is Fabric Orchestrator API
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.0.0
+- API version: 1.0.1
 - Package version: 1.0.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Generating the Client Code
 Due to a BUG in swagger-code-gen, Please follow the steps below
 
 That said, there's a bug in the Python generator of Swagger Codegen 3.x, it doesn't generate the code for Bearer authentication in OpenAPI 3.0 definitions. 
@@ -101,14 +126,17 @@
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://127.0.0.1:8700/*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*PoasApi* | [**poas_create_sliver_id_post**](docs/PoasApi.md#poas_create_sliver_id_post) | **POST** /poas/create/{sliver_id} | Perform an operational action on a sliver.
+*PoasApi* | [**poas_get**](docs/PoasApi.md#poas_get) | **GET** /poas/ | Request get the status of the POAs.
+*PoasApi* | [**poas_poa_id_get**](docs/PoasApi.md#poas_poa_id_get) | **GET** /poas/{poa_id} | Perform an operational action on a sliver.
 *ResourcesApi* | [**portalresources_get**](docs/ResourcesApi.md#portalresources_get) | **GET** /portalresources | Retrieve a listing and description of available resources for portal
 *ResourcesApi* | [**resources_get**](docs/ResourcesApi.md#resources_get) | **GET** /resources | Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
 *SlicesApi* | [**slices_create_post**](docs/SlicesApi.md#slices_create_post) | **POST** /slices/create | Create slice
 *SlicesApi* | [**slices_delete_delete**](docs/SlicesApi.md#slices_delete_delete) | **DELETE** /slices/delete | Delete all slices for a User within a project.
 *SlicesApi* | [**slices_delete_slice_id_delete**](docs/SlicesApi.md#slices_delete_slice_id_delete) | **DELETE** /slices/delete/{slice_id} | Delete slice.
 *SlicesApi* | [**slices_get**](docs/SlicesApi.md#slices_get) | **GET** /slices | Retrieve a listing of user slices
 *SlicesApi* | [**slices_modify_slice_id_accept_post**](docs/SlicesApi.md#slices_modify_slice_id_accept_post) | **POST** /slices/modify/{slice_id}/accept | Accept the last modify an existing slice
@@ -117,19 +145,25 @@
 *SlicesApi* | [**slices_slice_id_get**](docs/SlicesApi.md#slices_slice_id_get) | **GET** /slices/{slice_id} | slice properties
 *SliversApi* | [**slivers_get**](docs/SliversApi.md#slivers_get) | **GET** /slivers | Retrieve a listing of user slivers
 *SliversApi* | [**slivers_sliver_id_get**](docs/SliversApi.md#slivers_sliver_id_get) | **GET** /slivers/{sliver_id} | slivers properties
 *VersionApi* | [**version_get**](docs/VersionApi.md#version_get) | **GET** /version | Version
 
 ## Documentation For Models
 
+ - [Poa](docs/Poa.md)
+ - [PoaData](docs/PoaData.md)
+ - [PoaPost](docs/PoaPost.md)
+ - [PoaPostData](docs/PoaPostData.md)
+ - [PoaPostDataVcpuCpuMap](docs/PoaPostDataVcpuCpuMap.md)
  - [Resource](docs/Resource.md)
  - [Resources](docs/Resources.md)
  - [Slice](docs/Slice.md)
  - [SliceDetails](docs/SliceDetails.md)
  - [Slices](docs/Slices.md)
+ - [SlicesPost](docs/SlicesPost.md)
  - [Sliver](docs/Sliver.md)
  - [Slivers](docs/Slivers.md)
  - [Status200OkNoContent](docs/Status200OkNoContent.md)
  - [Status200OkNoContentData](docs/Status200OkNoContentData.md)
  - [Status200OkPaginated](docs/Status200OkPaginated.md)
  - [Status200OkSingle](docs/Status200OkSingle.md)
  - [Status400BadRequest](docs/Status400BadRequest.md)
@@ -227,7 +261,8 @@
 proxy = OrchestratorProxy(orchestrator_host=orchestrator_host)
 status, reservation = proxy.renew_slice(token=token, slice_id=slice_id,
                                         new_lease_end_time=new_time.strftime('%Y-%m-%d %H:%M:%S %z'))
 ```
 ## Author
 
 kthare10@unc.edu
+
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/docs/ResourcesApi.md` & `fabric-orchestrator-client-1.5.1/docs/ResourcesApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/docs/SlicesApi.md` & `fabric-orchestrator-client-1.5.1/docs/SlicesApi.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SlicesApi
 
 All URIs are relative to *http://127.0.0.1:8700/*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
 [**slices_create_post**](SlicesApi.md#slices_create_post) | **POST** /slices/create | Create slice
+[**slices_creates_post**](SlicesApi.md#slices_creates_post) | **POST** /slices/creates | Create slice
 [**slices_delete_delete**](SlicesApi.md#slices_delete_delete) | **DELETE** /slices/delete | Delete all slices for a User within a project.
 [**slices_delete_slice_id_delete**](SlicesApi.md#slices_delete_slice_id_delete) | **DELETE** /slices/delete/{slice_id} | Delete slice.
 [**slices_get**](SlicesApi.md#slices_get) | **GET** /slices | Retrieve a listing of user slices
 [**slices_modify_slice_id_accept_post**](SlicesApi.md#slices_modify_slice_id_accept_post) | **POST** /slices/modify/{slice_id}/accept | Accept the last modify an existing slice
 [**slices_modify_slice_id_put**](SlicesApi.md#slices_modify_slice_id_put) | **PUT** /slices/modify/{slice_id} | Modify an existing slice
 [**slices_renew_slice_id_post**](SlicesApi.md#slices_renew_slice_id_post) | **POST** /slices/renew/{slice_id} | Renew slice
 [**slices_slice_id_get**](SlicesApi.md#slices_slice_id_get) | **GET** /slices/{slice_id} | slice properties
@@ -22,28 +23,29 @@
 
 ### Example
 ```python
 from __future__ import print_function
 import time
 from fabric_cf.orchestrator.swagger_client import SlicesApi, Configuration, ApiClient
 from fabric_cf.orchestrator.swagger_client.rest import ApiException
+from fabric_cf.orchestrator.swagger_client.models import SlicesPost
 from pprint import pprint
 
 # Configure API key authorization: bearerAuth
 configuration = Configuration()
 configuration.api_key['Authorization'] = 'YOUR_API_KEY'
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['Authorization'] = 'Bearer'
 
 # create an instance of the API class
 api_instance = SlicesApi(ApiClient(configuration))
 body = 'body_example' # str | 
 name = 'name_example' # str | Slice Name
 ssh_key = 'ssh_key_example' # str | User SSH Key
-lease_end_time = 'lease_end_time_example' # str | New Lease End Time for the Slice (optional)
+lease_end_time = 'lease_end_time_example' # str | Lease End Time for the Slice (optional)
 
 try:
     # Create slice
     api_response = api_instance.slices_create_post(body, name, ssh_key, lease_end_time=lease_end_time)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling SlicesApi->slices_create_post: %s\n" % e)
@@ -52,15 +54,15 @@
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **body** | [**str**](str.md)|  | 
  **name** | **str**| Slice Name | 
  **ssh_key** | **str**| User SSH Key | 
- **lease_end_time** | **str**| New Lease End Time for the Slice | [optional] 
+ **lease_end_time** | **str**| Lease End Time for the Slice | [optional] 
 
 ### Return type
 
 [**Slivers**](Slivers.md)
 
 ### Authorization
 
@@ -69,14 +71,73 @@
 ### HTTP request headers
 
  - **Content-Type**: text/plain
  - **Accept**: application/json
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
+# **slices_creates_post**
+> Slivers slices_creates_post(body, name, lease_end_time=lease_end_time)
+
+Create slice
+
+Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.  
+
+### Example
+```python
+from __future__ import print_function
+from fabric_cf.orchestrator.swagger_client import SlicesApi, Configuration, ApiClient
+from fabric_cf.orchestrator.swagger_client.rest import ApiException
+from fabric_cf.orchestrator.swagger_client.models import SlicesPost
+from pprint import pprint
+
+# Configure API key authorization: bearerAuth
+configuration = Configuration()
+configuration.api_key['Authorization'] = 'YOUR_API_KEY'
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['Authorization'] = 'Bearer'
+
+
+# create an instance of the API class
+api_instance = SlicesApi(ApiClient(configuration))
+body = SlicesPost() # SlicesPost | Create new Slice
+name = 'name_example' # str | Slice Name
+lease_end_time = 'lease_end_time_example' # str | Lease End Time for the Slice (optional)
+
+try:
+    # Create slice
+    api_response = api_instance.slices_creates_post(body, name, lease_end_time=lease_end_time)
+    pprint(api_response)
+except ApiException as e:
+    print("Exception when calling SlicesApi->slices_creates_post: %s\n" % e)
+```
+
+### Parameters
+
+Name | Type | Description  | Notes
+------------- | ------------- | ------------- | -------------
+ **body** | [**SlicesPost**](SlicesPost.md)| Create new Slice | 
+ **name** | **str**| Slice Name | 
+ **lease_end_time** | **str**| Lease End Time for the Slice | [optional] 
+
+### Return type
+
+[**Slivers**](Slivers.md)
+
+### Authorization
+
+[bearerAuth](../README.md#bearerAuth)
+
+### HTTP request headers
+
+ - **Content-Type**: application/json
+ - **Accept**: application/json
+
+[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
+
 # **slices_delete_delete**
 > Status200OkNoContent slices_delete_delete()
 
 Delete all slices for a User within a project.
 
 Delete all slices for a User within a project. User identity email and project id is available in the bearer token. 
 
@@ -175,19 +236,19 @@
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **slices_get**
-> Slices slices_get(name=name, states=states, limit=limit, offset=offset)
+> Slices slices_get(name=name, as_self=as_self, states=states, limit=limit, offset=offset)
 
 Retrieve a listing of user slices
 
-Retrieve a listing of user slices
+Retrieve a listing of user slices. It returns list of all slices belonging to all members in a project when 'as_self' is False otherwise returns only the all user's slices in a project.
 
 ### Example
 ```python
 from __future__ import print_function
 import time
 from fabric_cf.orchestrator.swagger_client import SlicesApi, Configuration, ApiClient
 from fabric_cf.orchestrator.swagger_client.rest import ApiException
@@ -198,31 +259,33 @@
 configuration.api_key['Authorization'] = 'YOUR_API_KEY'
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['Authorization'] = 'Bearer'
 
 # create an instance of the API class
 api_instance = SlicesApi(ApiClient(configuration))
 name = 'name_example' # str | Search for Slices with the name (optional)
+as_self = true # bool | GET object as Self (optional) (default to true)
 states = ['states_example'] # list[str] | Search for Slices in the specified states (optional)
 limit = 5 # int | maximum number of results to return per page (1 or more) (optional) (default to 5)
 offset = 0 # int | number of items to skip before starting to collect the result set (optional) (default to 0)
 
 try:
     # Retrieve a listing of user slices
-    api_response = api_instance.slices_get(name=name, states=states, limit=limit, offset=offset)
+    api_response = api_instance.slices_get(name=name, as_self=as_self, states=states, limit=limit, offset=offset)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling SlicesApi->slices_get: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **name** | **str**| Search for Slices with the name | [optional] 
+ **as_self** | **bool**| GET object as Self | [optional] [default to true]
  **states** | [**list[str]**](str.md)| Search for Slices in the specified states | [optional] 
  **limit** | **int**| maximum number of results to return per page (1 or more) | [optional] [default to 5]
  **offset** | **int**| number of items to skip before starting to collect the result set | [optional] [default to 0]
 
 ### Return type
 
 [**Slices**](Slices.md)
@@ -312,30 +375,30 @@
 configuration = Configuration()
 configuration.api_key['Authorization'] = 'YOUR_API_KEY'
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['Authorization'] = 'Bearer'
 
 # create an instance of the API class
 api_instance = SlicesApi(ApiClient(configuration))
-body = 'body_example' # str | 
+body = 'body_example' # str | Modify a Slice
 slice_id = 'slice_id_example' # str | Slice identified by universally unique identifier
 
 try:
     # Modify an existing slice
     api_response = api_instance.slices_modify_slice_id_put(body, slice_id)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling SlicesApi->slices_modify_slice_id_put: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
- **body** | [**str**](str.md)|  | 
+ **body** | [**str**](str.md)|  | Modify a Slice
  **slice_id** | **str**| Slice identified by universally unique identifier | 
 
 ### Return type
 
 [**Slivers**](Slivers.md)
 
 ### Authorization
@@ -402,15 +465,15 @@
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **slices_slice_id_get**
-> SliceDetails slices_slice_id_get(slice_id, graph_format)
+> SliceDetails slices_slice_id_get(slice_id, graph_format, as_self=as_self)
 
 slice properties
 
 Retrieve Slice properties
 
 ### Example
 ```python
@@ -426,29 +489,31 @@
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['Authorization'] = 'Bearer'
 
 # create an instance of the API class
 api_instance = SlicesApi(ApiClient(configuration))
 slice_id = 'slice_id_example' # str | Slice identified by universally unique identifier
 graph_format = 'GRAPHML' # str | graph format (default to GRAPHML)
+as_self = true # bool | GET object as Self (optional) (default to true)
 
 try:
     # slice properties
-    api_response = api_instance.slices_slice_id_get(slice_id, graph_format)
+    api_response = api_instance.slices_slice_id_get(slice_id, graph_format, as_self=as_self)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling SlicesApi->slices_slice_id_get: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **slice_id** | **str**| Slice identified by universally unique identifier | 
  **graph_format** | **str**| graph format | [default to GRAPHML]
+ **as_self** | **bool**| GET object as Self | [optional] [default to true]
 
 ### Return type
 
 [**SliceDetails**](SliceDetails.md)
 
 ### Authorization
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/docs/SliversApi.md` & `fabric-orchestrator-client-1.5.1/docs/SliversApi.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
 [**slivers_get**](SliversApi.md#slivers_get) | **GET** /slivers | Retrieve a listing of user slivers
 [**slivers_sliver_id_get**](SliversApi.md#slivers_sliver_id_get) | **GET** /slivers/{sliver_id} | slivers properties
 
 # **slivers_get**
-> Slivers slivers_get(slice_id)
+> Slivers slivers_get(slice_id, as_self=as_self)
 
 Retrieve a listing of user slivers
 
 Retrieve a listing of user slivers
 
 ### Example
 ```python
@@ -27,28 +27,30 @@
 configuration.api_key['Authorization'] = 'YOUR_API_KEY'
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['Authorization'] = 'Bearer'
 
 # create an instance of the API class
 api_instance = SliversApi(ApiClient(configuration))
 slice_id = 'slice_id_example' # str | Slice identifier as UUID
+as_self = True # bool | GET object as Self (optional) (default to true)
 
 try:
     # Retrieve a listing of user slivers
-    api_response = api_instance.slivers_get(slice_id)
+    api_response = api_instance.slivers_get(slice_id, as_self=as_self)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling SliversApi->slivers_get: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **slice_id** | **str**| Slice identifier as UUID | 
+ **as_self** | **bool**| GET object as Self | [optional] [default to true]
 
 ### Return type
 
 [**Slivers**](Slivers.md)
 
 ### Authorization
 
@@ -58,15 +60,15 @@
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **slivers_sliver_id_get**
-> Slivers slivers_sliver_id_get(slice_id, sliver_id)
+> Slivers slivers_sliver_id_get(slice_id, sliver_id, as_self=as_self)
 
 slivers properties
 
 Retrieve Sliver properties
 
 ### Example
 ```python
@@ -83,29 +85,31 @@
 # configuration.api_key_prefix['Authorization'] = 'Bearer'
 
 # create an instance of the API class
 api_instance = SliversApi(ApiClient(configuration))
 
 slice_id = 'slice_id_example' # str | Slice identified by universally unique identifier
 sliver_id = 'sliver_id_example' # str | Sliver identified by universally unique identifier
+as_self = True # bool | GET object as Self (optional) (default to true)
 
 try:
     # slivers properties
-    api_response = api_instance.slivers_sliver_id_get(slice_id, sliver_id)
+    api_response = api_instance.slivers_sliver_id_get(slice_id, sliver_id, as_self=as_self)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling SliversApi->slivers_sliver_id_get: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **slice_id** | **str**| Slice identified by universally unique identifier | 
  **sliver_id** | **str**| Sliver identified by universally unique identifier | 
+ **as_self** | **bool**| GET object as Self | [optional] [default to true]
 
 ### Return type
 
 [**Slivers**](Slivers.md)
 
 ### Authorization
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/orchestrator_proxy.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/orchestrator_proxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import enum
 import traceback
 from datetime import datetime
-from typing import Tuple, Union, List
+from typing import Tuple, Union, List, Dict
 
 from fim.user import GraphFormat
 
 from fabric_cf.orchestrator import swagger_client
 from fim.user.topology import ExperimentTopology, AdvertizedTopology
 
-from fabric_cf.orchestrator.swagger_client import Sliver, Slice
+from fabric_cf.orchestrator.swagger_client import Sliver, Slice, SlicesPost
+from fabric_cf.orchestrator.swagger_client.models import PoaPost, PoaData, PoaPostData, Poa
 
 
 class OrchestratorProxyException(Exception):
     """
     Orchestrator Exceptions
     """
     pass
@@ -117,31 +118,33 @@
             configuration = swagger_client.configuration.Configuration()
             #configuration.verify_ssl = False
             configuration.host = f"https://{orchestrator_host}/"
             api_instance = swagger_client.ApiClient(configuration)
             self.slices_api = swagger_client.SlicesApi(api_client=api_instance)
             self.slivers_api = swagger_client.SliversApi(api_client=api_instance)
             self.resources_api = swagger_client.ResourcesApi(api_client=api_instance)
+            self.poas_api = swagger_client.PoasApi(api_client=api_instance)
 
     def __set_tokens(self, *, token: str):
         """
         Set tokens
         @param token token
         """
         # Set the tokens
         self.slices_api.api_client.configuration.api_key[self.PROP_AUTHORIZATION] = token
         self.slices_api.api_client.configuration.api_key_prefix[self.PROP_AUTHORIZATION] = self.PROP_BEARER
 
-    def create(self, *, token: str, slice_name: str, ssh_key: str, topology: ExperimentTopology = None,
-               slice_graph: str = None, lease_end_time: str = None) -> Tuple[Status, Union[Exception, List[Sliver]]]:
+    def create(self, *, token: str, slice_name: str, ssh_key: Union[str, List[str]],
+               topology: ExperimentTopology = None, slice_graph: str = None,
+               lease_end_time: str = None) -> Tuple[Status, Union[Exception, List[Sliver]]]:
         """
         Create a slice
         @param token fabric token
         @param slice_name slice name
-        @param ssh_key SSH Key
+        @param ssh_key SSH Key(s)
         @param topology Experiment topology
         @param slice_graph Slice Graph string
         @param lease_end_time Lease End Time
         @return Tuple containing Status and Exception/Json containing slivers created
         """
         if token is None:
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Token {token} must be specified")
@@ -156,29 +159,32 @@
                                                                         f"be specified")
 
         if lease_end_time is not None:
             try:
                 datetime.strptime(lease_end_time, self.TIME_FORMAT)
             except Exception as e:
                 return Status.INVALID_ARGUMENTS, OrchestratorProxyException(
-                    f"Lease End Time {lease_end_time} should be in format: {self.TIME_FORMAT}")
+                    f"Lease End Time {lease_end_time} should be in format: {self.TIME_FORMAT} e: {e}")
 
         try:
             # Set the tokens
             self.__set_tokens(token=token)
 
             if topology is not None:
                 slice_graph = topology.serialize()
 
-            response = None
+            if isinstance(ssh_key, str):
+                ssh_keys = [ssh_key]
+            else:
+                ssh_keys = ssh_key
+            body = SlicesPost(graph_model=slice_graph, ssh_keys=ssh_keys)
             if lease_end_time is not None:
-                slivers = self.slices_api.slices_create_post(name=slice_name, body=slice_graph, ssh_key=ssh_key,
-                                                             lease_end_time=lease_end_time)
+                slivers = self.slices_api.slices_creates_post(name=slice_name, body=body, lease_end_time=lease_end_time)
             else:
-                slivers = self.slices_api.slices_create_post(name=slice_name, body=slice_graph, ssh_key=ssh_key)
+                slivers = self.slices_api.slices_creates_post(name=slice_name, body=body)
 
             return Status.OK, slivers.data if slivers.data is not None else []
         except Exception as e:
             return Status.FAILURE, e
 
     def modify(self, *, token: str, slice_id: str, topology: ExperimentTopology = None,
                slice_graph: str = None) -> Tuple[Status, Union[Exception, List[Sliver]]]:
@@ -267,24 +273,26 @@
                 self.slices_api.slices_delete_delete()
 
             return Status.OK, None
         except Exception as e:
             return Status.FAILURE, e
 
     def slices(self, *, token: str, includes: List[SliceState] = None, excludes: List[SliceState] = None,
-               name: str = None, limit: int = 20, offset: int = 0, slice_id: str = None) -> Tuple[Status, Union[Exception, List[Slice]]]:
+               name: str = None, limit: int = 20, offset: int = 0, slice_id: str = None,
+               as_self: bool = True) -> Tuple[Status, Union[Exception, List[Slice]]]:
         """
         Get slices
         @param token fabric token
         @param includes list of the slice state used to include the slices in the output
         @param excludes list of the slice state used to exclude the slices from the output
         @param name name of the slice
         @param limit maximum number of slices to return
         @param offset offset of the first slice to return
         @param slice_id Slice Id
+        @param as_self
         @return Tuple containing Status and Exception/Json containing slices
         """
         if token is None:
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Token {token} must be specified")
 
         try:
             # Set the tokens
@@ -298,81 +306,87 @@
 
             if excludes is not None:
                 for x in excludes:
                     if x in states:
                         states.remove(x)
 
             if slice_id is not None:
-                slices = self.slices_api.slices_slice_id_get(slice_id=slice_id, graph_format=GraphFormat.GRAPHML.name)
+                slices = self.slices_api.slices_slice_id_get(slice_id=slice_id, graph_format=GraphFormat.GRAPHML.name,
+                                                             as_self=as_self)
             elif name is not None:
                 slices = self.slices_api.slices_get(states=SliceState.state_list_to_str_list(states), name=name,
-                                                    limit=limit, offset=offset)
+                                                    limit=limit, offset=offset, as_self=as_self)
             else:
                 slices = self.slices_api.slices_get(states=SliceState.state_list_to_str_list(states), limit=limit,
-                                                    offset=offset)
+                                                    offset=offset, as_self=as_self)
 
             return Status.OK, slices.data if slices.data is not None else []
         except Exception as e:
             return Status.FAILURE, e
 
     def get_slice(self, *, token: str, slice_id: str = None,
-                  graph_format: GraphFormat = GraphFormat.GRAPHML) -> Tuple[Status,
-                                                                            Union[Exception, ExperimentTopology, dict]]:
+                  graph_format: GraphFormat = GraphFormat.GRAPHML,
+                  as_self: bool = True) -> Tuple[Status, Union[Exception, ExperimentTopology, dict]]:
         """
         Get slice
         @param token fabric token
         @param slice_id slice id
         @param graph_format
+        @param as_self
         @return Tuple containing Status and Exception/Json containing slice
         """
         if token is None:
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Token {token} must be specified")
 
         if slice_id is None:
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Slice Id {slice_id} must be specified")
 
         try:
             # Set the tokens
             self.__set_tokens(token=token)
 
-            slice_details = self.slices_api.slices_slice_id_get(slice_id=slice_id, graph_format=graph_format.name)
+            slice_details = self.slices_api.slices_slice_id_get(slice_id=slice_id, graph_format=graph_format.name,
+                                                                as_self=as_self)
 
             model = slice_details.data[0].model if slice_details.data is not None else None
             topology = None
             if model is not None:
                 topology = ExperimentTopology()
                 topology.load(graph_string=model)
 
             return Status.OK, topology
         except Exception as e:
             return Status.FAILURE, e
 
     def slivers(self, *, token: str, slice_id: str,
-                sliver_id: str = None) -> Tuple[Status, Union[Exception, List[Sliver]]]:
+                sliver_id: str = None,
+                as_self: bool = True) -> Tuple[Status, Union[Exception, List[Sliver]]]:
         """
         Get slivers
         @param token fabric token
         @param slice_id slice id
         @param sliver_id slice sliver_id
+        @param as_self
         @return Tuple containing Status and Exception/Json containing Sliver(s)
         """
         if token is None:
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Token {token} must be specified")
 
         if slice_id is None:
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Slice Id {slice_id} must be specified")
 
         try:
             # Set the tokens
             self.__set_tokens(token=token)
 
             if sliver_id is None:
-                slivers = self.slivers_api.slivers_get(slice_id=slice_id)
+                slivers = self.slivers_api.slivers_get(slice_id=slice_id, as_self=as_self)
             else:
-                slivers = self.slivers_api.slivers_sliver_id_get(slice_id=slice_id, sliver_id=sliver_id)
+                slivers = self.slivers_api.slivers_sliver_id_get(slice_id=slice_id, sliver_id=sliver_id,
+                                                                 as_self=as_self)
 
             return Status.OK, slivers.data if slivers.data is not None else []
         except Exception as e:
             return Status.FAILURE, e
 
     def resources(self, *, token: str, level: int = 1,
                   force_refresh: bool = False) -> Tuple[Status, Union[Exception, AdvertizedTopology]]:
@@ -447,7 +461,75 @@
             self.__set_tokens(token=token)
 
             self.slices_api.slices_renew_slice_id_post(slice_id=slice_id, lease_end_time=new_lease_end_time)
 
             return Status.OK, None
         except Exception as e:
             return Status.FAILURE, e
+
+    def poa(self, *, token: str, sliver_id: str, operation: str, vcpu_cpu_map: List[Dict[str, str]] = None,
+            node_set: List[str] = None) -> Tuple[Status, Union[Exception, List[PoaData]]]:
+        """
+        Modify a slice
+        @param token fabric token
+        @param sliver_id Sliver Id
+        @param operation POA operation
+        @param vcpu_cpu_map vCPU to physical CPU Map
+        @param node_set List of Numa nodes
+        @return Tuple containing Status and Exception/Json containing poa info created
+        """
+        if token is None:
+            return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Token {token} must be specified")
+
+        if sliver_id is None:
+            return Status.INVALID_ARGUMENTS, \
+                   OrchestratorProxyException(f"Sliver Id {sliver_id} must be specified")
+
+        try:
+            # Set the tokens
+            self.__set_tokens(token=token)
+
+            body = PoaPost(operation=operation)
+            if vcpu_cpu_map is not None or node_set is not None:
+                post_data = PoaPostData()
+                post_data.vcpu_cpu_map = vcpu_cpu_map
+                post_data.node_set = node_set
+                body.data = post_data
+
+            poa_data = self.poas_api.poas_create_sliver_id_post(sliver_id=sliver_id, body=body)
+
+            return Status.OK, poa_data.data if poa_data.data is not None else None
+        except Exception as e:
+            return Status.FAILURE, e
+
+    def get_poas(self, *, token: str, sliver_id: str = None,
+                 poa_id: str = None, limit: int = 20, offset: int = 0) -> Tuple[Status, Union[Exception, List[PoaData]]]:
+        """
+        Modify a slice
+        @param token fabric token
+        @param sliver_id Sliver Id
+        @param poa_id POA request id
+        @param limit maximum number of poas to return
+        @param offset offset of the first poas to return
+        @return Tuple containing Status and Exception/Json containing poa info created
+        """
+        if token is None:
+            return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Token {token} must be specified")
+
+        if sliver_id is None and poa_id is None:
+            return Status.INVALID_ARGUMENTS, \
+                   OrchestratorProxyException(f"Sliver Id {sliver_id} or Poa ID {poa_id} must be specified")
+
+        try:
+            # Set the tokens
+            self.__set_tokens(token=token)
+
+            if poa_id is not None:
+                poa_data = self.poas_api.poas_poa_id_get(poa_id=poa_id)
+            elif sliver_id is not None:
+                poa_data = self.poas_api.poas_get(sliver_id=sliver_id, limit=limit, offset=offset)
+            else:
+                raise Exception("Invalid Arguments")
+
+            return Status.OK, poa_data.data if poa_data.data is not None else None
+        except Exception as e:
+            return Status.FAILURE, e
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/__init__.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     Fabric Orchestrator API
 
     This is Fabric Orchestrator API  # noqa: E501
 
     OpenAPI spec version: 1.0.1
     Contact: kthare10@unc.edu
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from fabric_cf.orchestrator.swagger_client.api.resources_api import ResourcesApi
-from fabric_cf.orchestrator.swagger_client.api.slices_api import SlicesApi
-from fabric_cf.orchestrator.swagger_client.api.slivers_api import SliversApi
-from fabric_cf.orchestrator.swagger_client.api.version_api import VersionApi
-# import ApiClient
-from fabric_cf.orchestrator.swagger_client.api_client import ApiClient
-from fabric_cf.orchestrator.swagger_client.configuration import Configuration
-# import models into sdk package
+# import models into model package
+from fabric_cf.orchestrator.swagger_client.models.poa import Poa
+from fabric_cf.orchestrator.swagger_client.models.poa_data import PoaData
+from fabric_cf.orchestrator.swagger_client.models.poa_post import PoaPost
+from fabric_cf.orchestrator.swagger_client.models.poa_post_data import PoaPostData
+from fabric_cf.orchestrator.swagger_client.models.poa_post_data_vcpu_cpu_map import PoaPostDataVcpuCpuMap
 from fabric_cf.orchestrator.swagger_client.models.resource import Resource
 from fabric_cf.orchestrator.swagger_client.models.resources import Resources
 from fabric_cf.orchestrator.swagger_client.models.slice import Slice
 from fabric_cf.orchestrator.swagger_client.models.slice_details import SliceDetails
 from fabric_cf.orchestrator.swagger_client.models.slices import Slices
+from fabric_cf.orchestrator.swagger_client.models.slices_post import SlicesPost
 from fabric_cf.orchestrator.swagger_client.models.sliver import Sliver
 from fabric_cf.orchestrator.swagger_client.models.slivers import Slivers
 from fabric_cf.orchestrator.swagger_client.models.status200_ok_no_content import Status200OkNoContent
 from fabric_cf.orchestrator.swagger_client.models.status200_ok_no_content_data import Status200OkNoContentData
 from fabric_cf.orchestrator.swagger_client.models.status200_ok_paginated import Status200OkPaginated
 from fabric_cf.orchestrator.swagger_client.models.status200_ok_single import Status200OkSingle
 from fabric_cf.orchestrator.swagger_client.models.status400_bad_request import Status400BadRequest
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/resources_api.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/slices_api.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/slices_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,47 +27,51 @@
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def slices_create_post(self, body, name, ssh_key, **kwargs):  # noqa: E501
         """Create slice  # noqa: E501
+
         Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.    # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_create_post(body, name, ssh_key, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str body: (required)
         :param str name: Slice Name (required)
         :param str ssh_key: User SSH Key (required)
-        :param str lease_end_time: New Lease End Time for the Slice
+        :param str lease_end_time: Lease End Time for the Slice
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.slices_create_post_with_http_info(body, name, ssh_key, **kwargs)  # noqa: E501
         else:
             (data) = self.slices_create_post_with_http_info(body, name, ssh_key, **kwargs)  # noqa: E501
             return data
 
     def slices_create_post_with_http_info(self, body, name, ssh_key, **kwargs):  # noqa: E501
         """Create slice  # noqa: E501
+
         Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.    # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_create_post_with_http_info(body, name, ssh_key, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str body: (required)
         :param str name: Slice Name (required)
         :param str ssh_key: User SSH Key (required)
-        :param str lease_end_time: New Lease End Time for the Slice
+        :param str lease_end_time: Lease End Time for the Slice
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body', 'name', 'ssh_key', 'lease_end_time']  # noqa: E501
         all_params.append('async_req')
@@ -140,14 +144,125 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def slices_creates_post(self, body, name, **kwargs):  # noqa: E501
+        """Create slice  # noqa: E501
+
+        Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.    # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.slices_creates_post(body, name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param SlicesPost body: Create new Slice (required)
+        :param str name: Slice Name (required)
+        :param str lease_end_time: Lease End Time for the Slice
+        :return: Slivers
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.slices_creates_post_with_http_info(body, name, **kwargs)  # noqa: E501
+        else:
+            (data) = self.slices_creates_post_with_http_info(body, name, **kwargs)  # noqa: E501
+            return data
+
+    def slices_creates_post_with_http_info(self, body, name, **kwargs):  # noqa: E501
+        """Create slice  # noqa: E501
+
+        Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.    # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.slices_creates_post_with_http_info(body, name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param SlicesPost body: Create new Slice (required)
+        :param str name: Slice Name (required)
+        :param str lease_end_time: Lease End Time for the Slice
+        :return: Slivers
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body', 'name', 'lease_end_time']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method slices_creates_post" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `slices_creates_post`")  # noqa: E501
+        # verify the required parameter 'name' is set
+        if ('name' not in params or
+                params['name'] is None):
+            raise ValueError("Missing the required parameter `name` when calling `slices_creates_post`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'name' in params:
+            query_params.append(('name', params['name']))  # noqa: E501
+        if 'lease_end_time' in params:
+            query_params.append(('lease_end_time', params['lease_end_time']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['bearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slices/creates', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='Slivers',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def slices_delete_delete(self, **kwargs):  # noqa: E501
         """Delete all slices for a User within a project.  # noqa: E501
 
         Delete all slices for a User within a project. User identity email and project id is available in the bearer token.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_delete_delete(async_req=True)
@@ -235,14 +350,15 @@
         """Delete slice.  # noqa: E501
 
         Request to delete slice. On success, resources associated with slice or sliver are stopped if necessary, de-provisioned and un-allocated at the respective sites.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_delete_slice_id_delete(slice_id, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str slice_id: Slice identified by universally unique identifier (required)
         :return: Status200OkNoContent
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
@@ -250,19 +366,21 @@
             return self.slices_delete_slice_id_delete_with_http_info(slice_id, **kwargs)  # noqa: E501
         else:
             (data) = self.slices_delete_slice_id_delete_with_http_info(slice_id, **kwargs)  # noqa: E501
             return data
 
     def slices_delete_slice_id_delete_with_http_info(self, slice_id, **kwargs):  # noqa: E501
         """Delete slice.  # noqa: E501
+
         Request to delete slice. On success, resources associated with slice or sliver are stopped if necessary, de-provisioned and un-allocated at the respective sites.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_delete_slice_id_delete_with_http_info(slice_id, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str slice_id: Slice identified by universally unique identifier (required)
         :return: Status200OkNoContent
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
@@ -321,21 +439,24 @@
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def slices_get(self, **kwargs):  # noqa: E501
         """Retrieve a listing of user slices  # noqa: E501
-        Retrieve a listing of user slices  # noqa: E501
+
+        Retrieve a listing of user slices. It returns list of all slices belonging to all members in a project when 'as_self' is False otherwise returns only the all user's slices in a project.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_get(async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str name: Search for Slices with the name
+        :param bool as_self: GET object as Self
         :param list[str] states: Search for Slices in the specified states
         :param int limit: maximum number of results to return per page (1 or more)
         :param int offset: number of items to skip before starting to collect the result set
         :return: Slices
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -344,30 +465,33 @@
             return self.slices_get_with_http_info(**kwargs)  # noqa: E501
         else:
             (data) = self.slices_get_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def slices_get_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve a listing of user slices  # noqa: E501
-        Retrieve a listing of user slices  # noqa: E501
+
+        Retrieve a listing of user slices. It returns list of all slices belonging to all members in a project when 'as_self' is False otherwise returns only the all user's slices in a project.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_get_with_http_info(async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str name: Search for Slices with the name
+        :param bool as_self: GET object as Self
         :param list[str] states: Search for Slices in the specified states
         :param int limit: maximum number of results to return per page (1 or more)
         :param int offset: number of items to skip before starting to collect the result set
         :return: Slices
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['name', 'states', 'limit', 'offset']  # noqa: E501
+        all_params = ['name', 'as_self', 'states', 'limit', 'offset']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -382,14 +506,16 @@
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'name' in params:
             query_params.append(('name', params['name']))  # noqa: E501
+        if 'as_self' in params:
+            query_params.append(('as_self', params['as_self']))  # noqa: E501
         if 'states' in params:
             query_params.append(('states', params['states']))  # noqa: E501
             collection_formats['states'] = 'multi'  # noqa: E501
         if 'limit' in params:
             query_params.append(('limit', params['limit']))  # noqa: E501
         if 'offset' in params:
             query_params.append(('offset', params['offset']))  # noqa: E501
@@ -421,19 +547,21 @@
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def slices_modify_slice_id_accept_post(self, slice_id, **kwargs):  # noqa: E501
         """Accept the last modify an existing slice  # noqa: E501
+
         Accept the last modify and prune any failed resources from the Slice. Also return the accepted slice model back to the user.    # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_modify_slice_id_accept_post(slice_id, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str slice_id: Slice identified by universally unique identifier (required)
         :return: SliceDetails
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
@@ -441,19 +569,21 @@
             return self.slices_modify_slice_id_accept_post_with_http_info(slice_id, **kwargs)  # noqa: E501
         else:
             (data) = self.slices_modify_slice_id_accept_post_with_http_info(slice_id, **kwargs)  # noqa: E501
             return data
 
     def slices_modify_slice_id_accept_post_with_http_info(self, slice_id, **kwargs):  # noqa: E501
         """Accept the last modify an existing slice  # noqa: E501
+
         Accept the last modify and prune any failed resources from the Slice. Also return the accepted slice model back to the user.    # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_modify_slice_id_accept_post_with_http_info(slice_id, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str slice_id: Slice identified by universally unique identifier (required)
         :return: SliceDetails
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
@@ -512,42 +642,46 @@
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def slices_modify_slice_id_put(self, body, slice_id, **kwargs):  # noqa: E501
         """Modify an existing slice  # noqa: E501
+
         Request to modify an existing slice as described in the request. Request would be a graph ML describing the experiment topolgy expected after a modify. The supported modify actions include adding or removing nodes, components, network services or interfaces of the slice. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.    # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_modify_slice_id_put(body, slice_id, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
-        :param str body: (required)
+        :param str body: Modify a Slice (required)
         :param str slice_id: Slice identified by universally unique identifier (required)
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.slices_modify_slice_id_put_with_http_info(body, slice_id, **kwargs)  # noqa: E501
         else:
             (data) = self.slices_modify_slice_id_put_with_http_info(body, slice_id, **kwargs)  # noqa: E501
             return data
 
     def slices_modify_slice_id_put_with_http_info(self, body, slice_id, **kwargs):  # noqa: E501
         """Modify an existing slice  # noqa: E501
+
         Request to modify an existing slice as described in the request. Request would be a graph ML describing the experiment topolgy expected after a modify. The supported modify actions include adding or removing nodes, components, network services or interfaces of the slice. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.    # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_modify_slice_id_put_with_http_info(body, slice_id, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
-        :param str body: (required)
+        :param str body: Modify a Slice (required)
         :param str slice_id: Slice identified by universally unique identifier (required)
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body', 'slice_id']  # noqa: E501
@@ -615,19 +749,21 @@
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def slices_renew_slice_id_post(self, slice_id, lease_end_time, **kwargs):  # noqa: E501
         """Renew slice  # noqa: E501
+
         Request to extend slice be renewed with their expiration extended. If possible, the orchestrator should extend the slivers to the requested expiration time, or to a sooner time if policy limits apply.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_renew_slice_id_post(slice_id, lease_end_time, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str slice_id: Slice identified by universally unique identifier (required)
         :param str lease_end_time: New Lease End Time for the Slice (required)
         :return: Status200OkNoContent
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -636,19 +772,21 @@
             return self.slices_renew_slice_id_post_with_http_info(slice_id, lease_end_time, **kwargs)  # noqa: E501
         else:
             (data) = self.slices_renew_slice_id_post_with_http_info(slice_id, lease_end_time, **kwargs)  # noqa: E501
             return data
 
     def slices_renew_slice_id_post_with_http_info(self, slice_id, lease_end_time, **kwargs):  # noqa: E501
         """Renew slice  # noqa: E501
+
         Request to extend slice be renewed with their expiration extended. If possible, the orchestrator should extend the slivers to the requested expiration time, or to a sooner time if policy limits apply.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_renew_slice_id_post_with_http_info(slice_id, lease_end_time, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str slice_id: Slice identified by universally unique identifier (required)
         :param str lease_end_time: New Lease End Time for the Slice (required)
         :return: Status200OkNoContent
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -714,49 +852,55 @@
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def slices_slice_id_get(self, slice_id, graph_format, **kwargs):  # noqa: E501
         """slice properties  # noqa: E501
+
         Retrieve Slice properties  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_slice_id_get(slice_id, graph_format, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str slice_id: Slice identified by universally unique identifier (required)
         :param str graph_format: graph format (required)
+        :param bool as_self: GET object as Self
         :return: SliceDetails
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.slices_slice_id_get_with_http_info(slice_id, graph_format, **kwargs)  # noqa: E501
         else:
             (data) = self.slices_slice_id_get_with_http_info(slice_id, graph_format, **kwargs)  # noqa: E501
             return data
 
     def slices_slice_id_get_with_http_info(self, slice_id, graph_format, **kwargs):  # noqa: E501
         """slice properties  # noqa: E501
+
         Retrieve Slice properties  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_slice_id_get_with_http_info(slice_id, graph_format, async_req=True)
         >>> result = thread.get()
+
         :param async_req bool
         :param str slice_id: Slice identified by universally unique identifier (required)
         :param str graph_format: graph format (required)
+        :param bool as_self: GET object as Self
         :return: SliceDetails
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['slice_id', 'graph_format']  # noqa: E501
+        all_params = ['slice_id', 'graph_format', 'as_self']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -779,14 +923,16 @@
         collection_formats = {}
 
         path_params = {}
         if 'slice_id' in params:
             path_params['slice_id'] = params['slice_id']  # noqa: E501
 
         query_params = []
+        if 'as_self' in params:
+            query_params.append(('as_self', params['as_self']))  # noqa: E501
         if 'graph_format' in params:
             query_params.append(('graph_format', params['graph_format']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slivers_get(slice_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str slice_id: Slice identifier as UUID (required)
+        :param bool as_self: GET object as Self
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.slivers_get_with_http_info(slice_id, **kwargs)  # noqa: E501
@@ -61,20 +62,21 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slivers_get_with_http_info(slice_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str slice_id: Slice identifier as UUID (required)
+        :param bool as_self: GET object as Self
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['slice_id']  # noqa: E501
+        all_params = ['slice_id', 'as_self']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -93,14 +95,16 @@
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'slice_id' in params:
             query_params.append(('slice_id', params['slice_id']))  # noqa: E501
+        if 'as_self' in params:
+            query_params.append(('as_self', params['as_self']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -135,14 +139,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slivers_sliver_id_get(slice_id, sliver_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str slice_id: Slice identified by universally unique identifier (required)
         :param str sliver_id: Sliver identified by universally unique identifier (required)
+        :param bool as_self: GET object as Self
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.slivers_sliver_id_get_with_http_info(slice_id, sliver_id, **kwargs)  # noqa: E501
@@ -158,20 +163,21 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slivers_sliver_id_get_with_http_info(slice_id, sliver_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str slice_id: Slice identified by universally unique identifier (required)
         :param str sliver_id: Sliver identified by universally unique identifier (required)
+        :param bool as_self: GET object as Self
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['slice_id', 'sliver_id']  # noqa: E501
+        all_params = ['slice_id', 'sliver_id', 'as_self']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -196,14 +202,16 @@
         path_params = {}
         if 'sliver_id' in params:
             path_params['sliver_id'] = params['sliver_id']  # noqa: E501
 
         query_params = []
         if 'slice_id' in params:
             query_params.append(('slice_id', params['slice_id']))  # noqa: E501
+        if 'as_self' in params:
+            query_params.append(('as_self', params['as_self']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/version_api.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api_client.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/configuration.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/__init__.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 # coding: utf-8
 
 # flake8: noqa
+
 """
     Fabric Orchestrator API
 
     This is Fabric Orchestrator API  # noqa: E501
 
     OpenAPI spec version: 1.0.1
     Contact: kthare10@unc.edu
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import models into model package
+# import apis into sdk package
+from fabric_cf.orchestrator.swagger_client.api.poas_api import PoasApi
+from fabric_cf.orchestrator.swagger_client.api.resources_api import ResourcesApi
+from fabric_cf.orchestrator.swagger_client.api.slices_api import SlicesApi
+from fabric_cf.orchestrator.swagger_client.api.slivers_api import SliversApi
+from fabric_cf.orchestrator.swagger_client.api.version_api import VersionApi
+# import ApiClient
+from fabric_cf.orchestrator.swagger_client.api_client import ApiClient
+from fabric_cf.orchestrator.swagger_client.configuration import Configuration
+# import models into sdk package
+from fabric_cf.orchestrator.swagger_client.models.poa import Poa
+from fabric_cf.orchestrator.swagger_client.models.poa_data import PoaData
+from fabric_cf.orchestrator.swagger_client.models.poa_post import PoaPost
+from fabric_cf.orchestrator.swagger_client.models.poa_post_data import PoaPostData
+from fabric_cf.orchestrator.swagger_client.models.poa_post_data_vcpu_cpu_map import PoaPostDataVcpuCpuMap
 from fabric_cf.orchestrator.swagger_client.models.resource import Resource
 from fabric_cf.orchestrator.swagger_client.models.resources import Resources
 from fabric_cf.orchestrator.swagger_client.models.slice import Slice
 from fabric_cf.orchestrator.swagger_client.models.slice_details import SliceDetails
 from fabric_cf.orchestrator.swagger_client.models.slices import Slices
+from fabric_cf.orchestrator.swagger_client.models.slices_post import SlicesPost
 from fabric_cf.orchestrator.swagger_client.models.sliver import Sliver
 from fabric_cf.orchestrator.swagger_client.models.slivers import Slivers
 from fabric_cf.orchestrator.swagger_client.models.status200_ok_no_content import Status200OkNoContent
 from fabric_cf.orchestrator.swagger_client.models.status200_ok_no_content_data import Status200OkNoContentData
 from fabric_cf.orchestrator.swagger_client.models.status200_ok_paginated import Status200OkPaginated
 from fabric_cf.orchestrator.swagger_client.models.status200_ok_single import Status200OkSingle
 from fabric_cf.orchestrator.swagger_client.models.status400_bad_request import Status400BadRequest
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/resource.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/resources.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slice.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slice_details.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slice_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     def __init__(self, data=None, *args, **kwargs):  # noqa: E501
         """SliceDetails - a model defined in Swagger"""  # noqa: E501
         self._data = None
         self.discriminator = None
         if data is not None:
             self.data = data
         Status200OkSingle.__init__(self, *args, **kwargs)
+        
 
     @property
     def data(self):
         """Gets the data of this SliceDetails.  # noqa: E501
 
 
         :return: The data of this SliceDetails.  # noqa: E501
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slices.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/sliver.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/sliver.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
     @property
     def sliver(self):
         """Gets the sliver of this Sliver.  # noqa: E501
 
 
         :return: The sliver of this Sliver.  # noqa: E501
-        :rtype: dict
+        :rtype: object
         """
         return self._sliver
 
     @sliver.setter
     def sliver(self, sliver):
         """Sets the sliver of this Sliver.
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slivers.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/version.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/version_data.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/rest.py` & `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/git_push.sh` & `fabric-orchestrator-client-1.5.1/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/pyproject.toml` & `fabric-orchestrator-client-1.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 requires-python = '>=3.9'
 dependencies = [
     "certifi >= 14.05.14",
     "six >= 1.10",
     "python_dateutil >= 2.5.3",
     "requests>=2.28.1",
-    "fabric-fim==1.5.0b4",
+    "fabric-fim==1.5.2",
     ]
 
 [project.optional-dependencies]
 test = ["coverage>=4.0.3",
         "nose>=1.3.7",
         "pluggy>=0.3.1",
         "py>=1.4.31",
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_resource.py` & `fabric-orchestrator-client-1.5.1/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_resources.py` & `fabric-orchestrator-client-1.5.1/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_resources_api.py` & `fabric-orchestrator-client-1.5.1/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_slice.py` & `fabric-orchestrator-client-1.5.1/test/test_slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_slice_details.py` & `fabric-orchestrator-client-1.5.1/test/test_slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_slices.py` & `fabric-orchestrator-client-1.5.1/test/test_slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_slices_api.py` & `fabric-orchestrator-client-1.5.1/test/test_slices_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,21 @@
     def test_slices_create_post(self):
         """Test case for slices_create_post
 
         Create slice  # noqa: E501
         """
         pass
 
+    def test_slices_creates_post(self):
+        """Test case for slices_creates_post
+
+        Create slice  # noqa: E501
+        """
+        pass
+
     def test_slices_delete_delete(self):
         """Test case for slices_delete_delete
 
         Delete all slices for a User within a project.  # noqa: E501
         """
         pass
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_sliver.py` & `fabric-orchestrator-client-1.5.1/test/test_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_slivers.py` & `fabric-orchestrator-client-1.5.1/test/test_slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_slivers_api.py` & `fabric-orchestrator-client-1.5.1/test/test_slivers_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
-from fabric_cf.orchestrator.swagger_client.api.slivers_api import SliversApi  # noqa: E501
-from fabric_cf.orchestrator.swagger_client.rest import ApiException
+import swagger_client
+from swagger_client.api.slivers_api import SliversApi  # noqa: E501
+from swagger_client.rest import ApiException
 
 
 class TestSliversApi(unittest.TestCase):
     """SliversApi unit test stubs"""
 
     def setUp(self):
         self.api = SliversApi()  # noqa: E501
```

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_no_content.py` & `fabric-orchestrator-client-1.5.1/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.5.1/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_paginated.py` & `fabric-orchestrator-client-1.5.1/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_single.py` & `fabric-orchestrator-client-1.5.1/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status400_bad_request.py` & `fabric-orchestrator-client-1.5.1/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status400_bad_request_errors.py` & `fabric-orchestrator-client-1.5.1/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status401_unauthorized.py` & `fabric-orchestrator-client-1.5.1/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.5.1/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status403_forbidden.py` & `fabric-orchestrator-client-1.5.1/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status403_forbidden_errors.py` & `fabric-orchestrator-client-1.5.1/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status404_not_found.py` & `fabric-orchestrator-client-1.5.1/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status404_not_found_errors.py` & `fabric-orchestrator-client-1.5.1/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status500_internal_server_error.py` & `fabric-orchestrator-client-1.5.1/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.5.1/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_version.py` & `fabric-orchestrator-client-1.5.1/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_version_api.py` & `fabric-orchestrator-client-1.5.1/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/test/test_version_data.py` & `fabric-orchestrator-client-1.5.1/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc2/PKG-INFO` & `fabric-orchestrator-client-1.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,15 @@
-Metadata-Version: 2.1
-Name: fabric-orchestrator-client
-Version: 1.5.0rc2
-Summary: Fabric Orchestrator API
-Keywords: Swagger,Fabric Orchestrator API
-Author-email: Komal Thareja <kthare10@renci.org>
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Dist: certifi >= 14.05.14
-Requires-Dist: six >= 1.10
-Requires-Dist: python_dateutil >= 2.5.3
-Requires-Dist: requests>=2.28.1
-Requires-Dist: fabric-fim==1.5.0b4
-Requires-Dist: coverage>=4.0.3 ; extra == "test"
-Requires-Dist: nose>=1.3.7 ; extra == "test"
-Requires-Dist: pluggy>=0.3.1 ; extra == "test"
-Requires-Dist: py>=1.4.31 ; extra == "test"
-Requires-Dist: randomize>=0.13 ; extra == "test"
-Project-URL: Home, https://fabric-testbed.net/
-Project-URL: Sources, https://github.com/fabric-testbed/OrchestratorClient
-Provides-Extra: test
-
 [![PyPI](https://img.shields.io/pypi/v/fabric-orchestrator-client?style=plastic)](https://pypi.org/project/fabric-orchestrator-client/)
 
 # Fabric Orchestrator swagger-client
 This is Fabric Orchestrator API
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.0.0
+- API version: 1.0.1
 - Package version: 1.0.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Generating the Client Code
 Due to a BUG in swagger-code-gen, Please follow the steps below
 
 That said, there's a bug in the Python generator of Swagger Codegen 3.x, it doesn't generate the code for Bearer authentication in OpenAPI 3.0 definitions. 
@@ -126,14 +101,17 @@
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://127.0.0.1:8700/*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*PoasApi* | [**poas_create_sliver_id_post**](docs/PoasApi.md#poas_create_sliver_id_post) | **POST** /poas/create/{sliver_id} | Perform an operational action on a sliver.
+*PoasApi* | [**poas_get**](docs/PoasApi.md#poas_get) | **GET** /poas/ | Request get the status of the POAs.
+*PoasApi* | [**poas_poa_id_get**](docs/PoasApi.md#poas_poa_id_get) | **GET** /poas/{poa_id} | Perform an operational action on a sliver.
 *ResourcesApi* | [**portalresources_get**](docs/ResourcesApi.md#portalresources_get) | **GET** /portalresources | Retrieve a listing and description of available resources for portal
 *ResourcesApi* | [**resources_get**](docs/ResourcesApi.md#resources_get) | **GET** /resources | Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
 *SlicesApi* | [**slices_create_post**](docs/SlicesApi.md#slices_create_post) | **POST** /slices/create | Create slice
 *SlicesApi* | [**slices_delete_delete**](docs/SlicesApi.md#slices_delete_delete) | **DELETE** /slices/delete | Delete all slices for a User within a project.
 *SlicesApi* | [**slices_delete_slice_id_delete**](docs/SlicesApi.md#slices_delete_slice_id_delete) | **DELETE** /slices/delete/{slice_id} | Delete slice.
 *SlicesApi* | [**slices_get**](docs/SlicesApi.md#slices_get) | **GET** /slices | Retrieve a listing of user slices
 *SlicesApi* | [**slices_modify_slice_id_accept_post**](docs/SlicesApi.md#slices_modify_slice_id_accept_post) | **POST** /slices/modify/{slice_id}/accept | Accept the last modify an existing slice
@@ -142,19 +120,25 @@
 *SlicesApi* | [**slices_slice_id_get**](docs/SlicesApi.md#slices_slice_id_get) | **GET** /slices/{slice_id} | slice properties
 *SliversApi* | [**slivers_get**](docs/SliversApi.md#slivers_get) | **GET** /slivers | Retrieve a listing of user slivers
 *SliversApi* | [**slivers_sliver_id_get**](docs/SliversApi.md#slivers_sliver_id_get) | **GET** /slivers/{sliver_id} | slivers properties
 *VersionApi* | [**version_get**](docs/VersionApi.md#version_get) | **GET** /version | Version
 
 ## Documentation For Models
 
+ - [Poa](docs/Poa.md)
+ - [PoaData](docs/PoaData.md)
+ - [PoaPost](docs/PoaPost.md)
+ - [PoaPostData](docs/PoaPostData.md)
+ - [PoaPostDataVcpuCpuMap](docs/PoaPostDataVcpuCpuMap.md)
  - [Resource](docs/Resource.md)
  - [Resources](docs/Resources.md)
  - [Slice](docs/Slice.md)
  - [SliceDetails](docs/SliceDetails.md)
  - [Slices](docs/Slices.md)
+ - [SlicesPost](docs/SlicesPost.md)
  - [Sliver](docs/Sliver.md)
  - [Slivers](docs/Slivers.md)
  - [Status200OkNoContent](docs/Status200OkNoContent.md)
  - [Status200OkNoContentData](docs/Status200OkNoContentData.md)
  - [Status200OkPaginated](docs/Status200OkPaginated.md)
  - [Status200OkSingle](docs/Status200OkSingle.md)
  - [Status400BadRequest](docs/Status400BadRequest.md)
@@ -252,8 +236,7 @@
 proxy = OrchestratorProxy(orchestrator_host=orchestrator_host)
 status, reservation = proxy.renew_slice(token=token, slice_id=slice_id,
                                         new_lease_end_time=new_time.strftime('%Y-%m-%d %H:%M:%S %z'))
 ```
 ## Author
 
 kthare10@unc.edu
-
```

