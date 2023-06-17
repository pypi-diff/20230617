# Comparing `tmp/atlassian-python-api-3.9.0.tar.gz` & `tmp/atlassian-python-api-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/atlassian-python-api-3.9.0.tar", last modified: Mon May  3 17:00:08 2021, max compression
+gzip compressed data, was "dist/atlassian-python-api-3.9.1.tar", last modified: Wed May  5 06:03:01 2021, max compression
```

## Comparing `atlassian-python-api-3.9.0.tar` & `atlassian-python-api-3.9.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     8264 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/PKG-INFO
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    11315 2020-03-02 18:07:51.000000 atlassian-python-api-3.9.0/LICENSE
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)       69 2021-01-21 22:13:28.000000 atlassian-python-api-3.9.0/requirements.txt
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    19184 2021-02-13 18:36:23.000000 atlassian-python-api-3.9.0/pyproject.toml
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/tests/
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     3686 2021-01-03 19:44:37.000000 atlassian-python-api-3.9.0/tests/test_servicedesk.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    13362 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/tests/test_bitbucket_server.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     4062 2021-01-08 06:09:56.000000 atlassian-python-api-3.9.0/tests/test_confluence_advanced_mode.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2020-03-02 18:07:51.000000 atlassian-python-api-3.9.0/tests/__init__.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     2777 2021-03-13 12:38:52.000000 atlassian-python-api-3.9.0/tests/mockup.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    12866 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/tests/test_bitbucket_cloud.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     5799 2020-11-17 08:17:35.000000 atlassian-python-api-3.9.0/tests/test_confluence_attach.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     1791 2020-11-17 08:17:35.000000 atlassian-python-api-3.9.0/tests/test_base.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)      101 2020-03-02 18:07:51.000000 atlassian-python-api-3.9.0/MANIFEST.in
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     2425 2021-01-21 22:13:28.000000 atlassian-python-api-3.9.0/setup.py
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/atlassian/
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    28693 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/service_desk.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    98203 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/confluence.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     1125 2020-11-02 13:01:12.000000 atlassian-python-api-3.9.0/atlassian/request_utils.py
--rwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)    38544 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/bamboo.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     2179 2020-11-17 08:17:35.000000 atlassian-python-api-3.9.0/atlassian/crowd.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)      485 2020-11-02 13:01:12.000000 atlassian-python-api-3.9.0/atlassian/__init__.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)        6 2021-05-03 16:59:22.000000 atlassian-python-api-3.9.0/atlassian/VERSION
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    11009 2021-01-14 06:35:38.000000 atlassian-python-api-3.9.0/atlassian/utils.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     2590 2020-11-02 13:01:12.000000 atlassian-python-api-3.9.0/atlassian/marketplace.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)   141909 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/jira.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)      353 2020-06-16 14:23:03.000000 atlassian-python-api-3.9.0/atlassian/errors.py
--rwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)    18935 2021-03-15 17:43:12.000000 atlassian-python-api-3.9.0/atlassian/xray.py
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)   105307 2021-04-14 18:41:30.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/__init__.py
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/server/
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/server/projects/
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/server/projects/repos/
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     8696 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/server/projects/repos/__init__.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     7503 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/server/projects/__init__.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     1613 2021-01-03 17:40:41.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/server/__init__.py
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/server/common/
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)       40 2021-01-03 21:44:42.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/server/common/__init__.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     7321 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/server/common/permissions.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     5978 2021-01-03 19:44:37.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/server/globalPermissions.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     1775 2021-01-03 19:44:37.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/server/base.py
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)      821 2021-01-08 06:09:56.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/__init__.py
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     5065 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/issues.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     6539 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/branchRestrictions.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    11566 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/__init__.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     3510 2021-01-03 19:44:37.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/defaultReviewers.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    14118 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/pullRequests.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     8950 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/pipelines.py
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/workspaces/
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     4458 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/workspaces/__init__.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     7133 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/workspaces/projects.py
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/common/
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)      543 2020-12-31 15:12:32.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/common/users.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)       39 2020-12-31 15:12:32.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/common/__init__.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     2894 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/base.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     5927 2021-01-03 19:44:37.000000 atlassian-python-api-3.9.0/atlassian/bitbucket/base.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     3807 2020-11-17 08:17:35.000000 atlassian-python-api-3.9.0/atlassian/portfolio.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    11757 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.0/atlassian/rest_client.py
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     1015 2021-01-20 09:04:52.000000 atlassian-python-api-3.9.0/tox.ini
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)      244 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/setup.cfg
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     5084 2021-01-05 07:17:54.000000 atlassian-python-api-3.9.0/README.rst
-drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/atlassian_python_api.egg-info/
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     8264 2021-05-03 17:00:07.000000 atlassian-python-api-3.9.0/atlassian_python_api.egg-info/PKG-INFO
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)        1 2020-03-02 19:19:00.000000 atlassian-python-api-3.9.0/atlassian_python_api.egg-info/not-zip-safe
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     1829 2021-05-03 17:00:08.000000 atlassian-python-api-3.9.0/atlassian_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)       81 2021-05-03 17:00:07.000000 atlassian-python-api-3.9.0/atlassian_python_api.egg-info/requires.txt
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)       16 2021-05-03 17:00:07.000000 atlassian-python-api-3.9.0/atlassian_python_api.egg-info/top_level.txt
--rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)        1 2021-05-03 17:00:07.000000 atlassian-python-api-3.9.0/atlassian_python_api.egg-info/dependency_links.txt
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     8264 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/PKG-INFO
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    11315 2020-03-02 18:07:51.000000 atlassian-python-api-3.9.1/LICENSE
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)       69 2021-01-21 22:13:28.000000 atlassian-python-api-3.9.1/requirements.txt
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    19184 2021-02-13 18:36:23.000000 atlassian-python-api-3.9.1/pyproject.toml
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/tests/
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     3686 2021-01-03 19:44:37.000000 atlassian-python-api-3.9.1/tests/test_servicedesk.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    13362 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/tests/test_bitbucket_server.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     4062 2021-01-08 06:09:56.000000 atlassian-python-api-3.9.1/tests/test_confluence_advanced_mode.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2020-03-02 18:07:51.000000 atlassian-python-api-3.9.1/tests/__init__.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     2777 2021-03-13 12:38:52.000000 atlassian-python-api-3.9.1/tests/mockup.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    12866 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/tests/test_bitbucket_cloud.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     5799 2020-11-17 08:17:35.000000 atlassian-python-api-3.9.1/tests/test_confluence_attach.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     1791 2020-11-17 08:17:35.000000 atlassian-python-api-3.9.1/tests/test_base.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)      101 2020-03-02 18:07:51.000000 atlassian-python-api-3.9.1/MANIFEST.in
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     2425 2021-01-21 22:13:28.000000 atlassian-python-api-3.9.1/setup.py
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian/
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    28693 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/service_desk.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    98203 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/confluence.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     1125 2020-11-02 13:01:12.000000 atlassian-python-api-3.9.1/atlassian/request_utils.py
+-rwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)    38544 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/bamboo.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     2179 2020-11-17 08:17:35.000000 atlassian-python-api-3.9.1/atlassian/crowd.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)      485 2020-11-02 13:01:12.000000 atlassian-python-api-3.9.1/atlassian/__init__.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)        6 2021-05-05 06:02:20.000000 atlassian-python-api-3.9.1/atlassian/VERSION
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    11009 2021-01-14 06:35:38.000000 atlassian-python-api-3.9.1/atlassian/utils.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     2590 2020-11-02 13:01:12.000000 atlassian-python-api-3.9.1/atlassian/marketplace.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)   141909 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/jira.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)      353 2020-06-16 14:23:03.000000 atlassian-python-api-3.9.1/atlassian/errors.py
+-rwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)    18935 2021-03-15 17:43:12.000000 atlassian-python-api-3.9.1/atlassian/xray.py
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)   105309 2021-05-05 06:02:09.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/__init__.py
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/server/
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/server/projects/
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/server/projects/repos/
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     8696 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/server/projects/repos/__init__.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     7503 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/server/projects/__init__.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     1613 2021-01-03 17:40:41.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/server/__init__.py
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/server/common/
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)       40 2021-01-03 21:44:42.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/server/common/__init__.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     7321 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/server/common/permissions.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     5978 2021-01-03 19:44:37.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/server/globalPermissions.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     1775 2021-01-03 19:44:37.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/server/base.py
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)      821 2021-01-08 06:09:56.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/__init__.py
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     5065 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/issues.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     6539 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/branchRestrictions.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    11566 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/__init__.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     3510 2021-01-03 19:44:37.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/defaultReviewers.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    14118 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/pullRequests.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     8950 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/pipelines.py
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/workspaces/
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     4458 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/workspaces/__init__.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     7133 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/workspaces/projects.py
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/common/
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)      543 2020-12-31 15:12:32.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/common/users.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)       39 2020-12-31 15:12:32.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/common/__init__.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     2894 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/base.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     5927 2021-01-03 19:44:37.000000 atlassian-python-api-3.9.1/atlassian/bitbucket/base.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     3807 2020-11-17 08:17:35.000000 atlassian-python-api-3.9.1/atlassian/portfolio.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)    11757 2021-05-03 11:26:40.000000 atlassian-python-api-3.9.1/atlassian/rest_client.py
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     1015 2021-01-20 09:04:52.000000 atlassian-python-api-3.9.1/tox.ini
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)      244 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/setup.cfg
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     5084 2021-01-05 07:17:54.000000 atlassian-python-api-3.9.1/README.rst
+drwxr-xr-x   0 gonchik.tsymzhitov (36748) orcgroup   (410)        0 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian_python_api.egg-info/
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     8264 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)        1 2020-03-02 19:19:00.000000 atlassian-python-api-3.9.1/atlassian_python_api.egg-info/not-zip-safe
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)     1829 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)       81 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian_python_api.egg-info/requires.txt
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)       16 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian_python_api.egg-info/top_level.txt
+-rw-r--r--   0 gonchik.tsymzhitov (36748) orcgroup   (410)        1 2021-05-05 06:03:01.000000 atlassian-python-api-3.9.1/atlassian_python_api.egg-info/dependency_links.txt
```

### Comparing `atlassian-python-api-3.9.0/PKG-INFO` & `atlassian-python-api-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlassian-python-api
-Version: 3.9.0
+Version: 3.9.1
 Summary: Python Atlassian REST API Wrapper
 Home-page: https://github.com/atlassian-api/atlassian-python-api
 Author: Matt Harasymczuk
 Author-email: matt@astrotech.io
 Maintainer: Gonchik Tsymzhitov
 Maintainer-email: gonchik.tsymzhitov@gmail.com
 License: Apache License 2.0
```

### Comparing `atlassian-python-api-3.9.0/LICENSE` & `atlassian-python-api-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/pyproject.toml` & `atlassian-python-api-3.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/tests/test_servicedesk.py` & `atlassian-python-api-3.9.1/tests/test_servicedesk.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/tests/test_bitbucket_server.py` & `atlassian-python-api-3.9.1/tests/test_bitbucket_server.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/tests/test_confluence_advanced_mode.py` & `atlassian-python-api-3.9.1/tests/test_confluence_advanced_mode.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/tests/mockup.py` & `atlassian-python-api-3.9.1/tests/mockup.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/tests/test_bitbucket_cloud.py` & `atlassian-python-api-3.9.1/tests/test_bitbucket_cloud.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/tests/test_confluence_attach.py` & `atlassian-python-api-3.9.1/tests/test_confluence_attach.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/tests/test_base.py` & `atlassian-python-api-3.9.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/setup.py` & `atlassian-python-api-3.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/service_desk.py` & `atlassian-python-api-3.9.1/atlassian/service_desk.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/confluence.py` & `atlassian-python-api-3.9.1/atlassian/confluence.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/request_utils.py` & `atlassian-python-api-3.9.1/atlassian/request_utils.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bamboo.py` & `atlassian-python-api-3.9.1/atlassian/bamboo.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/crowd.py` & `atlassian-python-api-3.9.1/atlassian/crowd.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/utils.py` & `atlassian-python-api-3.9.1/atlassian/utils.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/marketplace.py` & `atlassian-python-api-3.9.1/atlassian/marketplace.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/jira.py` & `atlassian-python-api-3.9.1/atlassian/jira.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/xray.py` & `atlassian-python-api-3.9.1/atlassian/xray.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/__init__.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         Get group of members
         :param group: The group name to query
         :param start:
         :param limit:
         :return: A list of group members
         """
 
-        url = "{}/groups/more-members".format(self._url_admin)
+        url = "{}/groups/more-members".format(self._url_admin())
         params = {}
         if start:
             params["start"] = start
         if limit:
             params["limit"] = limit
         if group:
             params["context"] = group
```

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/server/projects/repos/__init__.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/server/projects/repos/__init__.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/server/projects/__init__.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/server/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/server/__init__.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/server/__init__.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/server/common/permissions.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/server/common/permissions.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/server/globalPermissions.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/server/globalPermissions.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/server/base.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/server/base.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/__init__.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/issues.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/issues.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/branchRestrictions.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/branchRestrictions.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/__init__.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/defaultReviewers.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/defaultReviewers.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/pullRequests.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/pullRequests.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/repositories/pipelines.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/repositories/pipelines.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/workspaces/__init__.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/workspaces/projects.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/workspaces/projects.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/common/users.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/common/users.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/cloud/base.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/cloud/base.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/bitbucket/base.py` & `atlassian-python-api-3.9.1/atlassian/bitbucket/base.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/portfolio.py` & `atlassian-python-api-3.9.1/atlassian/portfolio.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian/rest_client.py` & `atlassian-python-api-3.9.1/atlassian/rest_client.py`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/tox.ini` & `atlassian-python-api-3.9.1/tox.ini`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/README.rst` & `atlassian-python-api-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `atlassian-python-api-3.9.0/atlassian_python_api.egg-info/PKG-INFO` & `atlassian-python-api-3.9.1/atlassian_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlassian-python-api
-Version: 3.9.0
+Version: 3.9.1
 Summary: Python Atlassian REST API Wrapper
 Home-page: https://github.com/atlassian-api/atlassian-python-api
 Author: Matt Harasymczuk
 Author-email: matt@astrotech.io
 Maintainer: Gonchik Tsymzhitov
 Maintainer-email: gonchik.tsymzhitov@gmail.com
 License: Apache License 2.0
```

### Comparing `atlassian-python-api-3.9.0/atlassian_python_api.egg-info/SOURCES.txt` & `atlassian-python-api-3.9.1/atlassian_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

