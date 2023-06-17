# Comparing `tmp/hvac-1.1.0.tar.gz` & `tmp/hvac-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hvac-1.1.0.tar", max compression
+gzip compressed data, was "hvac-1.1.1.tar", max compression
```

## Comparing `hvac-1.1.0.tar` & `hvac-1.1.1.tar`

### file list

```diff
@@ -1,71 +1,70 @@
--rw-r--r--   0        0        0    11358 2023-03-06 14:09:37.051335 hvac-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2061 2023-03-06 14:09:37.051335 hvac-1.1.0/README.md
--rw-r--r--   0        0        0       50 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/__init__.py
--rw-r--r--   0        0        0    14277 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/adapters.py
--rw-r--r--   0        0        0      423 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/__init__.py
--rw-r--r--   0        0        0     2206 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/__init__.py
--rw-r--r--   0        0        0    20692 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/approle.py
--rw-r--r--   0        0        0    39862 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/aws.py
--rw-r--r--   0        0        0    13325 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/azure.py
--rw-r--r--   0        0        0    14682 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/cert.py
--rw-r--r--   0        0        0    18932 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/gcp.py
--rw-r--r--   0        0        0     8499 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/github.py
--rw-r--r--   0        0        0    19063 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/jwt.py
--rw-r--r--   0        0        0    11595 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/kubernetes.py
--rw-r--r--   0        0        0    16646 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/ldap.py
--rw-r--r--   0        0        0     6539 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/legacy_mfa.py
--rw-r--r--   0        0        0     7228 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/mfa.py
--rw-r--r--   0        0        0     8199 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/oidc.py
--rw-r--r--   0        0        0    11402 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/okta.py
--rw-r--r--   0        0        0     8448 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/radius.py
--rw-r--r--   0        0        0    25670 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/token.py
--rw-r--r--   0        0        0     5582 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/auth_methods/userpass.py
--rw-r--r--   0        0        0     1639 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/__init__.py
--rw-r--r--   0        0        0     7150 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/active_directory.py
--rw-r--r--   0        0        0    17328 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/aws.py
--rw-r--r--   0        0        0     7356 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/azure.py
--rw-r--r--   0        0        0     6728 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/consul.py
--rw-r--r--   0        0        0    13590 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/database.py
--rw-r--r--   0        0        0    13115 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/gcp.py
--rw-r--r--   0        0        0    59390 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/identity.py
--rw-r--r--   0        0        0     2901 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/kv.py
--rw-r--r--   0        0        0     5811 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/kv_v1.py
--rw-r--r--   0        0        0    20340 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/kv_v2.py
--rw-r--r--   0        0        0    24600 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/pki.py
--rw-r--r--   0        0        0     5823 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/rabbitmq.py
--rw-r--r--   0        0        0    21208 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/ssh.py
--rw-r--r--   0        0        0    45095 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/transform.py
--rw-r--r--   0        0        0    50198 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/secrets_engines/transit.py
--rw-r--r--   0        0        0     1699 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/system_backend/__init__.py
--rw-r--r--   0        0        0     3741 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/system_backend/audit.py
--rw-r--r--   0        0        0     9289 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/system_backend/auth.py
--rw-r--r--   0        0        0     1668 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/system_backend/capabilities.py
--rw-r--r--   0        0        0     3310 2023-03-06 14:09:37.055334 hvac-1.1.0/hvac/api/system_backend/health.py
--rw-r--r--   0        0        0     4952 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/system_backend/init.py
--rw-r--r--   0        0        0    15889 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/system_backend/key.py
--rw-r--r--   0        0        0     1161 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/system_backend/leader.py
--rw-r--r--   0        0        0     4326 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/system_backend/lease.py
--rw-r--r--   0        0        0    10108 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/system_backend/mount.py
--rw-r--r--   0        0        0     1393 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/system_backend/namespace.py
--rw-r--r--   0        0        0     2794 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/system_backend/policy.py
--rw-r--r--   0        0        0     5646 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/system_backend/raft.py
--rw-r--r--   0        0        0     3471 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/system_backend/seal.py
--rw-r--r--   0        0        0      265 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/system_backend/system_backend_mixin.py
--rw-r--r--   0        0        0     1146 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/system_backend/wrapping.py
--rw-r--r--   0        0        0      479 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/vault_api_base.py
--rw-r--r--   0        0        0     3599 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/api/vault_api_category.py
--rw-r--r--   0        0        0     3607 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/aws_utils.py
--rw-r--r--   0        0        0        0 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/constants/__init__.py
--rw-r--r--   0        0        0      220 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/constants/approle.py
--rw-r--r--   0        0        0      363 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/constants/aws.py
--rw-r--r--   0        0        0      221 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/constants/azure.py
--rw-r--r--   0        0        0      731 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/constants/client.py
--rw-r--r--   0        0        0      515 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/constants/gcp.py
--rw-r--r--   0        0        0      137 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/constants/identity.py
--rw-r--r--   0        0        0      900 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/constants/transit.py
--rw-r--r--   0        0        0     1450 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/exceptions.py
--rw-r--r--   0        0        0    13097 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/utils.py
--rw-r--r--   0        0        0    13974 2023-03-06 14:09:37.059334 hvac-1.1.0/hvac/v1/__init__.py
--rw-r--r--   0        0        0     1658 2023-03-06 14:09:37.059334 hvac-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2893 2023-03-06 14:10:32.487416 hvac-1.1.0/setup.py
--rw-r--r--   0        0        0     3073 2023-03-06 14:10:32.487805 hvac-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-17 20:06:13.186544 hvac-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2061 2023-06-17 20:06:13.186544 hvac-1.1.1/README.md
+-rw-r--r--   0        0        0       50 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/__init__.py
+-rw-r--r--   0        0        0    14277 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/adapters.py
+-rw-r--r--   0        0        0      423 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/__init__.py
+-rw-r--r--   0        0        0     2206 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/__init__.py
+-rw-r--r--   0        0        0    20692 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/approle.py
+-rw-r--r--   0        0        0    39862 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/aws.py
+-rw-r--r--   0        0        0    13325 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/azure.py
+-rw-r--r--   0        0        0    14682 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/cert.py
+-rw-r--r--   0        0        0    18932 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/gcp.py
+-rw-r--r--   0        0        0     8499 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/github.py
+-rw-r--r--   0        0        0    19063 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/jwt.py
+-rw-r--r--   0        0        0    11595 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/kubernetes.py
+-rw-r--r--   0        0        0    16646 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/ldap.py
+-rw-r--r--   0        0        0     6539 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/legacy_mfa.py
+-rw-r--r--   0        0        0     7228 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/mfa.py
+-rw-r--r--   0        0        0     8199 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/oidc.py
+-rw-r--r--   0        0        0    11402 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/okta.py
+-rw-r--r--   0        0        0     8448 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/radius.py
+-rw-r--r--   0        0        0    25441 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/token.py
+-rw-r--r--   0        0        0     5582 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/auth_methods/userpass.py
+-rw-r--r--   0        0        0     1639 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/secrets_engines/__init__.py
+-rw-r--r--   0        0        0     7150 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/secrets_engines/active_directory.py
+-rw-r--r--   0        0        0    17328 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/secrets_engines/aws.py
+-rw-r--r--   0        0        0     7356 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/secrets_engines/azure.py
+-rw-r--r--   0        0        0     6728 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/secrets_engines/consul.py
+-rw-r--r--   0        0        0    13590 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/secrets_engines/database.py
+-rw-r--r--   0        0        0    13115 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/secrets_engines/gcp.py
+-rw-r--r--   0        0        0    59390 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/secrets_engines/identity.py
+-rw-r--r--   0        0        0     2901 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/secrets_engines/kv.py
+-rw-r--r--   0        0        0     5811 2023-06-17 20:06:13.190544 hvac-1.1.1/hvac/api/secrets_engines/kv_v1.py
+-rw-r--r--   0        0        0    20340 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/secrets_engines/kv_v2.py
+-rw-r--r--   0        0        0    24600 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/secrets_engines/pki.py
+-rw-r--r--   0        0        0     5823 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/secrets_engines/rabbitmq.py
+-rw-r--r--   0        0        0    21208 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/secrets_engines/ssh.py
+-rw-r--r--   0        0        0    45095 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/secrets_engines/transform.py
+-rw-r--r--   0        0        0    50198 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/secrets_engines/transit.py
+-rw-r--r--   0        0        0     1699 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/__init__.py
+-rw-r--r--   0        0        0     3741 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/audit.py
+-rw-r--r--   0        0        0     9289 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/auth.py
+-rw-r--r--   0        0        0     1668 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/capabilities.py
+-rw-r--r--   0        0        0     3310 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/health.py
+-rw-r--r--   0        0        0     4952 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/init.py
+-rw-r--r--   0        0        0    15889 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/key.py
+-rw-r--r--   0        0        0     1161 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/leader.py
+-rw-r--r--   0        0        0     4326 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/lease.py
+-rw-r--r--   0        0        0    10108 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/mount.py
+-rw-r--r--   0        0        0     1393 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/namespace.py
+-rw-r--r--   0        0        0     2794 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/policy.py
+-rw-r--r--   0        0        0     5646 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/raft.py
+-rw-r--r--   0        0        0     3471 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/seal.py
+-rw-r--r--   0        0        0      265 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/system_backend_mixin.py
+-rw-r--r--   0        0        0     1146 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/system_backend/wrapping.py
+-rw-r--r--   0        0        0      479 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/vault_api_base.py
+-rw-r--r--   0        0        0     3599 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/api/vault_api_category.py
+-rw-r--r--   0        0        0     3607 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/aws_utils.py
+-rw-r--r--   0        0        0        0 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/constants/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/constants/approle.py
+-rw-r--r--   0        0        0      363 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/constants/aws.py
+-rw-r--r--   0        0        0      221 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/constants/azure.py
+-rw-r--r--   0        0        0      731 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/constants/client.py
+-rw-r--r--   0        0        0      515 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/constants/gcp.py
+-rw-r--r--   0        0        0      137 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/constants/identity.py
+-rw-r--r--   0        0        0      900 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/constants/transit.py
+-rw-r--r--   0        0        0     1450 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/exceptions.py
+-rw-r--r--   0        0        0    13097 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/utils.py
+-rw-r--r--   0        0        0    13974 2023-06-17 20:06:13.194544 hvac-1.1.1/hvac/v1/__init__.py
+-rw-r--r--   0        0        0     1638 2023-06-17 20:06:13.194544 hvac-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3373 1970-01-01 00:00:00.000000 hvac-1.1.1/PKG-INFO
```

### Comparing `hvac-1.1.0/LICENSE.txt` & `hvac-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/README.md` & `hvac-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/adapters.py` & `hvac-1.1.1/hvac/adapters.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/__init__.py` & `hvac-1.1.1/hvac/api/auth_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/approle.py` & `hvac-1.1.1/hvac/api/auth_methods/approle.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/aws.py` & `hvac-1.1.1/hvac/api/auth_methods/aws.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/azure.py` & `hvac-1.1.1/hvac/api/auth_methods/azure.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/cert.py` & `hvac-1.1.1/hvac/api/auth_methods/cert.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/gcp.py` & `hvac-1.1.1/hvac/api/auth_methods/gcp.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/github.py` & `hvac-1.1.1/hvac/api/auth_methods/github.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/jwt.py` & `hvac-1.1.1/hvac/api/auth_methods/jwt.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/kubernetes.py` & `hvac-1.1.1/hvac/api/auth_methods/kubernetes.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/ldap.py` & `hvac-1.1.1/hvac/api/auth_methods/ldap.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/legacy_mfa.py` & `hvac-1.1.1/hvac/api/auth_methods/legacy_mfa.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/mfa.py` & `hvac-1.1.1/hvac/api/auth_methods/mfa.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/oidc.py` & `hvac-1.1.1/hvac/api/auth_methods/oidc.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/okta.py` & `hvac-1.1.1/hvac/api/auth_methods/okta.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/radius.py` & `hvac-1.1.1/hvac/api/auth_methods/radius.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/auth_methods/token.py` & `hvac-1.1.1/hvac/api/auth_methods/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,25 +107,19 @@
                 "display_name": display_name,
                 "num_uses": num_uses,
                 "period": period,
                 "entity_alias": entity_alias,
             }
         )
 
+        api_path = f"/v1/auth/{mount_point}/create"
+
         if role_name is not None:
-            api_path = "/v1/auth/{mount_point}/create/{role_name}".format(
-                mount_point=mount_point,
-                role_name=role_name,
-            )
-            return self._adapter.post(
-                url=api_path,
-                json=params,
-            )
+            api_path = f"{api_path}/{role_name}"
 
-        api_path = f"/v1/auth/{mount_point}/create"
         return self._adapter.post(
             url=api_path,
             json=params,
             wrap_ttl=wrap_ttl,
         )
 
     def create_orphan(
```

### Comparing `hvac-1.1.0/hvac/api/auth_methods/userpass.py` & `hvac-1.1.1/hvac/api/auth_methods/userpass.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/__init__.py` & `hvac-1.1.1/hvac/api/secrets_engines/__init__.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/active_directory.py` & `hvac-1.1.1/hvac/api/secrets_engines/active_directory.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/aws.py` & `hvac-1.1.1/hvac/api/secrets_engines/aws.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/azure.py` & `hvac-1.1.1/hvac/api/secrets_engines/azure.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/consul.py` & `hvac-1.1.1/hvac/api/secrets_engines/consul.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/database.py` & `hvac-1.1.1/hvac/api/secrets_engines/database.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/gcp.py` & `hvac-1.1.1/hvac/api/secrets_engines/gcp.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/identity.py` & `hvac-1.1.1/hvac/api/secrets_engines/identity.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/kv.py` & `hvac-1.1.1/hvac/api/secrets_engines/kv.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/kv_v1.py` & `hvac-1.1.1/hvac/api/secrets_engines/kv_v1.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/kv_v2.py` & `hvac-1.1.1/hvac/api/secrets_engines/kv_v2.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/pki.py` & `hvac-1.1.1/hvac/api/secrets_engines/pki.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/rabbitmq.py` & `hvac-1.1.1/hvac/api/secrets_engines/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/ssh.py` & `hvac-1.1.1/hvac/api/secrets_engines/ssh.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/transform.py` & `hvac-1.1.1/hvac/api/secrets_engines/transform.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/secrets_engines/transit.py` & `hvac-1.1.1/hvac/api/secrets_engines/transit.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/__init__.py` & `hvac-1.1.1/hvac/api/system_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/audit.py` & `hvac-1.1.1/hvac/api/system_backend/audit.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/auth.py` & `hvac-1.1.1/hvac/api/system_backend/auth.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/capabilities.py` & `hvac-1.1.1/hvac/api/system_backend/capabilities.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/health.py` & `hvac-1.1.1/hvac/api/system_backend/health.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/init.py` & `hvac-1.1.1/hvac/api/system_backend/init.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/key.py` & `hvac-1.1.1/hvac/api/system_backend/key.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/leader.py` & `hvac-1.1.1/hvac/api/system_backend/leader.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/lease.py` & `hvac-1.1.1/hvac/api/system_backend/lease.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/mount.py` & `hvac-1.1.1/hvac/api/system_backend/mount.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/namespace.py` & `hvac-1.1.1/hvac/api/system_backend/namespace.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/policy.py` & `hvac-1.1.1/hvac/api/system_backend/policy.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/raft.py` & `hvac-1.1.1/hvac/api/system_backend/raft.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/seal.py` & `hvac-1.1.1/hvac/api/system_backend/seal.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/system_backend/wrapping.py` & `hvac-1.1.1/hvac/api/system_backend/wrapping.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/api/vault_api_category.py` & `hvac-1.1.1/hvac/api/vault_api_category.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/aws_utils.py` & `hvac-1.1.1/hvac/aws_utils.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/constants/client.py` & `hvac-1.1.1/hvac/constants/client.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/constants/gcp.py` & `hvac-1.1.1/hvac/constants/gcp.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/constants/transit.py` & `hvac-1.1.1/hvac/constants/transit.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/exceptions.py` & `hvac-1.1.1/hvac/exceptions.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/utils.py` & `hvac-1.1.1/hvac/utils.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/hvac/v1/__init__.py` & `hvac-1.1.1/hvac/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hvac-1.1.0/pyproject.toml` & `hvac-1.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hvac"
-version = "1.1.0"
+version = "1.1.1"
 description = "HashiCorp Vault API client"
 readme = "README.md"
 authors = [
     "Ian Unruh <ianunruh@gmail.com>",
     "Jeffrey Hogan <jeff.hogan1@gmail.com>",
 ]
 maintainers = [
@@ -36,15 +36,14 @@
 [tool.poetry.dev-dependencies]
 Werkzeug = "2.0.3"
 Authlib = "^1.0.1"
 black = "22.6.0"
 Flask = "2.0.3"
 Flask-SQLAlchemy = "^2.5.1"
 flake8 = "4.0.1"
-codecov = "^2.1.12"
 coverage = "6.2"
 ipaddress = "^1.0.23"
 mock = "^4.0.3"
 nose = "^1.3.7"
 parameterized = "^0.8.1"
 pytest = "7.0.1"
 pytest-cov = "^3.0.0"
```

### Comparing `hvac-1.1.0/PKG-INFO` & `hvac-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: hvac
-Version: 1.1.0
+Version: 1.1.1
 Summary: HashiCorp Vault API client
 Home-page: https://github.com/hvac/hvac
 License: Apache-2.0
 Keywords: hashicorp,vault
 Author: Ian Unruh
 Author-email: ianunruh@gmail.com
 Maintainer: Brian Scholer
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: pyhcl (>=0.4.4,<0.5.0)
```

