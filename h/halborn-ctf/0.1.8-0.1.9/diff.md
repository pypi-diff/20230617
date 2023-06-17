# Comparing `tmp/halborn_ctf-0.1.8.tar.gz` & `tmp/halborn_ctf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halborn_ctf-0.1.8.tar", last modified: Tue May 30 08:59:26 2023, max compression
+gzip compressed data, was "halborn_ctf-0.1.9.tar", last modified: Wed May 31 22:40:33 2023, max compression
```

## Comparing `halborn_ctf-0.1.8.tar` & `halborn_ctf-0.1.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.874366 halborn_ctf-0.1.8/
--rw-r--r--   0 fr0zn      (501) staff       (20)      594 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/.coveragerc
--rw-r--r--   0 fr0zn      (501) staff       (20)      566 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/.gitignore
--rw-r--r--   0 fr0zn      (501) staff       (20)      530 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/.readthedocs.yml
--rw-r--r--   0 fr0zn      (501) staff       (20)       86 2023-05-02 06:37:24.000000 halborn_ctf-0.1.8/AUTHORS.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      128 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/CHANGELOG.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)    13866 2023-04-29 17:50:20.000000 halborn_ctf-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     1081 2023-05-02 06:37:24.000000 halborn_ctf-0.1.8/LICENSE.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-30 08:59:26.874448 halborn_ctf-0.1.8/PKG-INFO
--rw-r--r--   0 fr0zn      (501) staff       (20)     1687 2023-05-02 13:57:33.000000 halborn_ctf-0.1.8/README.rst
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.867830 halborn_ctf-0.1.8/docs/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1154 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/docs/Makefile
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.868040 halborn_ctf-0.1.8/docs/_static/
--rw-r--r--   0 fr0zn      (501) staff       (20)       18 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/docs/_static/.gitignore
--rw-r--r--   0 fr0zn      (501) staff       (20)       41 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/docs/authors.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       43 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/docs/changelog.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     9819 2023-05-03 09:08:19.000000 halborn_ctf-0.1.8/docs/conf.py
--rw-r--r--   0 fr0zn      (501) staff       (20)       33 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/docs/contributing.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     1646 2023-05-03 08:57:14.000000 halborn_ctf-0.1.8/docs/index.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       67 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/docs/license.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      231 2023-05-02 07:06:55.000000 halborn_ctf-0.1.8/docs/requirements.txt
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.851966 halborn_ctf-0.1.8/docs/src/
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.868880 halborn_ctf-0.1.8/docs/src/getting_started/
--rw-r--r--   0 fr0zn      (501) staff       (20)     2292 2023-05-03 09:12:11.000000 halborn_ctf-0.1.8/docs/src/getting_started/examples.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     1325 2023-05-02 14:03:18.000000 halborn_ctf-0.1.8/docs/src/getting_started/installation.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     8582 2023-05-03 08:43:10.000000 halborn_ctf-0.1.8/docs/src/getting_started/quick_start.rst
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.869217 halborn_ctf-0.1.8/docs/src/user_guide/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1706 2023-05-03 09:31:00.000000 halborn_ctf-0.1.8/docs/src/user_guide/faq.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      346 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/pyproject.toml
--rw-r--r--   0 fr0zn      (501) staff       (20)     1323 2023-05-30 08:59:26.874851 halborn_ctf-0.1.8/setup.cfg
--rw-r--r--   0 fr0zn      (501) staff       (20)      708 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/setup.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.852106 halborn_ctf-0.1.8/src/
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.870802 halborn_ctf-0.1.8/src/halborn_ctf/
--rw-r--r--   0 fr0zn      (501) staff       (20)      643 2023-04-30 11:37:15.000000 halborn_ctf-0.1.8/src/halborn_ctf/__init__.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     4492 2023-05-02 09:22:23.000000 halborn_ctf-0.1.8/src/halborn_ctf/cli.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1338 2023-05-02 18:37:52.000000 halborn_ctf-0.1.8/src/halborn_ctf/functions.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.872297 halborn_ctf-0.1.8/src/halborn_ctf/network/
--rw-r--r--   0 fr0zn      (501) staff       (20)      131 2023-05-02 18:10:52.000000 halborn_ctf-0.1.8/src/halborn_ctf/network/__init__.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1409 2023-05-02 18:10:43.000000 halborn_ctf-0.1.8/src/halborn_ctf/network/_generic.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.873166 halborn_ctf-0.1.8/src/halborn_ctf/network/filters/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1918 2023-05-01 07:37:02.000000 halborn_ctf-0.1.8/src/halborn_ctf/network/filters/__init__.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.873659 halborn_ctf-0.1.8/src/halborn_ctf/network/filters/_json_rpc/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1314 2023-05-02 17:51:03.000000 halborn_ctf-0.1.8/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1333 2023-05-02 17:51:12.000000 halborn_ctf-0.1.8/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1611 2023-05-01 07:37:55.000000 halborn_ctf-0.1.8/src/halborn_ctf/network/filters/_utils.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     2968 2023-05-01 07:15:21.000000 halborn_ctf-0.1.8/src/halborn_ctf/network/filters/json_rpc.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     4159 2023-04-30 06:56:04.000000 halborn_ctf-0.1.8/src/halborn_ctf/shell.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     3675 2023-05-03 08:37:30.000000 halborn_ctf-0.1.8/src/halborn_ctf/state.py
--rw-r--r--   0 fr0zn      (501) staff       (20)    22586 2023-05-30 08:58:57.000000 halborn_ctf-0.1.8/src/halborn_ctf/templates.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.871955 halborn_ctf-0.1.8/src/halborn_ctf.egg-info/
--rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-30 08:59:26.000000 halborn_ctf-0.1.8/src/halborn_ctf.egg-info/PKG-INFO
--rw-r--r--   0 fr0zn      (501) staff       (20)     1274 2023-05-30 08:59:26.000000 halborn_ctf-0.1.8/src/halborn_ctf.egg-info/SOURCES.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-05-30 08:59:26.000000 halborn_ctf-0.1.8/src/halborn_ctf.egg-info/dependency_links.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)       52 2023-05-30 08:59:26.000000 halborn_ctf-0.1.8/src/halborn_ctf.egg-info/entry_points.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-04-28 12:47:06.000000 halborn_ctf-0.1.8/src/halborn_ctf.egg-info/not-zip-safe
--rw-r--r--   0 fr0zn      (501) staff       (20)      160 2023-05-30 08:59:26.000000 halborn_ctf-0.1.8/src/halborn_ctf.egg-info/requires.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)       12 2023-05-30 08:59:26.000000 halborn_ctf-0.1.8/src/halborn_ctf.egg-info/top_level.txt
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 08:59:26.874137 halborn_ctf-0.1.8/tests/
--rw-r--r--   0 fr0zn      (501) staff       (20)      279 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/tests/conftest.py
--rw-r--r--   0 fr0zn      (501) staff       (20)      592 2023-05-02 06:37:24.000000 halborn_ctf-0.1.8/tests/test_skeleton.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     2851 2023-04-28 12:46:11.000000 halborn_ctf-0.1.8/tox.ini
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.270630 halborn_ctf-0.1.9/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      594 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/.coveragerc
+-rw-r--r--   0 fr0zn      (501) staff       (20)      566 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/.gitignore
+-rw-r--r--   0 fr0zn      (501) staff       (20)      530 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/.readthedocs.yml
+-rw-r--r--   0 fr0zn      (501) staff       (20)       86 2023-05-02 06:37:24.000000 halborn_ctf-0.1.9/AUTHORS.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      128 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/CHANGELOG.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)    13866 2023-04-29 17:50:20.000000 halborn_ctf-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1081 2023-05-02 06:37:24.000000 halborn_ctf-0.1.9/LICENSE.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-31 22:40:33.270695 halborn_ctf-0.1.9/PKG-INFO
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1687 2023-05-02 13:57:33.000000 halborn_ctf-0.1.9/README.rst
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.267907 halborn_ctf-0.1.9/docs/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1154 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/docs/Makefile
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.268005 halborn_ctf-0.1.9/docs/_static/
+-rw-r--r--   0 fr0zn      (501) staff       (20)       18 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/docs/_static/.gitignore
+-rw-r--r--   0 fr0zn      (501) staff       (20)       41 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/docs/authors.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)       43 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/docs/changelog.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     9819 2023-05-03 09:08:19.000000 halborn_ctf-0.1.9/docs/conf.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)       33 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/docs/contributing.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1646 2023-05-03 08:57:14.000000 halborn_ctf-0.1.9/docs/index.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)       67 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/docs/license.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      231 2023-05-02 07:06:55.000000 halborn_ctf-0.1.9/docs/requirements.txt
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.265315 halborn_ctf-0.1.9/docs/src/
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.268283 halborn_ctf-0.1.9/docs/src/getting_started/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1541 2023-05-31 22:29:27.000000 halborn_ctf-0.1.9/docs/src/getting_started/examples.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1325 2023-05-02 14:03:18.000000 halborn_ctf-0.1.9/docs/src/getting_started/installation.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     8582 2023-05-03 08:43:10.000000 halborn_ctf-0.1.9/docs/src/getting_started/quick_start.rst
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.268381 halborn_ctf-0.1.9/docs/src/user_guide/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1706 2023-05-31 22:26:20.000000 halborn_ctf-0.1.9/docs/src/user_guide/faq.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      346 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/pyproject.toml
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1323 2023-05-31 22:40:33.271036 halborn_ctf-0.1.9/setup.cfg
+-rw-r--r--   0 fr0zn      (501) staff       (20)      708 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/setup.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.265456 halborn_ctf-0.1.9/src/
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.268936 halborn_ctf-0.1.9/src/halborn_ctf/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      643 2023-04-30 11:37:15.000000 halborn_ctf-0.1.9/src/halborn_ctf/__init__.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     4492 2023-05-02 09:22:23.000000 halborn_ctf-0.1.9/src/halborn_ctf/cli.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1338 2023-05-02 18:37:52.000000 halborn_ctf-0.1.9/src/halborn_ctf/functions.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.269796 halborn_ctf-0.1.9/src/halborn_ctf/network/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      131 2023-05-31 21:58:02.000000 halborn_ctf-0.1.9/src/halborn_ctf/network/__init__.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1409 2023-05-02 18:10:43.000000 halborn_ctf-0.1.9/src/halborn_ctf/network/_generic.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.270088 halborn_ctf-0.1.9/src/halborn_ctf/network/filters/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1915 2023-05-31 22:32:23.000000 halborn_ctf-0.1.9/src/halborn_ctf/network/filters/__init__.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.270301 halborn_ctf-0.1.9/src/halborn_ctf/network/filters/_json_rpc/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1269 2023-05-31 22:31:23.000000 halborn_ctf-0.1.9/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1288 2023-05-31 22:31:34.000000 halborn_ctf-0.1.9/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2022 2023-05-31 22:32:55.000000 halborn_ctf-0.1.9/src/halborn_ctf/network/filters/_utils.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2060 2023-05-31 22:20:31.000000 halborn_ctf-0.1.9/src/halborn_ctf/network/filters/json_rpc.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     4159 2023-04-30 06:56:04.000000 halborn_ctf-0.1.9/src/halborn_ctf/shell.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     3675 2023-05-03 08:37:30.000000 halborn_ctf-0.1.9/src/halborn_ctf/state.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)    22239 2023-05-31 22:34:37.000000 halborn_ctf-0.1.9/src/halborn_ctf/templates.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.269607 halborn_ctf-0.1.9/src/halborn_ctf.egg-info/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-31 22:40:33.000000 halborn_ctf-0.1.9/src/halborn_ctf.egg-info/PKG-INFO
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1274 2023-05-31 22:40:33.000000 halborn_ctf-0.1.9/src/halborn_ctf.egg-info/SOURCES.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-05-31 22:40:33.000000 halborn_ctf-0.1.9/src/halborn_ctf.egg-info/dependency_links.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)       52 2023-05-31 22:40:33.000000 halborn_ctf-0.1.9/src/halborn_ctf.egg-info/entry_points.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-04-28 12:47:06.000000 halborn_ctf-0.1.9/src/halborn_ctf.egg-info/not-zip-safe
+-rw-r--r--   0 fr0zn      (501) staff       (20)      160 2023-05-31 22:40:33.000000 halborn_ctf-0.1.9/src/halborn_ctf.egg-info/requires.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)       12 2023-05-31 22:40:33.000000 halborn_ctf-0.1.9/src/halborn_ctf.egg-info/top_level.txt
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-31 22:40:33.270532 halborn_ctf-0.1.9/tests/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      279 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/tests/conftest.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)      592 2023-05-02 06:37:24.000000 halborn_ctf-0.1.9/tests/test_skeleton.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2851 2023-04-28 12:46:11.000000 halborn_ctf-0.1.9/tox.ini
```

### Comparing `halborn_ctf-0.1.8/.coveragerc` & `halborn_ctf-0.1.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/.gitignore` & `halborn_ctf-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/.readthedocs.yml` & `halborn_ctf-0.1.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/CONTRIBUTING.rst` & `halborn_ctf-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/LICENSE.txt` & `halborn_ctf-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/PKG-INFO` & `halborn_ctf-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halborn_ctf
-Version: 0.1.8
+Version: 0.1.9
 Summary: Add a short description here!
 Home-page: https://github.com/HalbornAcademy/halborn_ctf
 Author: ferran.celades
 Author-email: ferran.celades@halborn.com
 License: MIT
 Project-URL: Documentation, https://halborn-ctf.readthedocs.io/
 Platform: any
```

### Comparing `halborn_ctf-0.1.8/README.rst` & `halborn_ctf-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/docs/Makefile` & `halborn_ctf-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/docs/conf.py` & `halborn_ctf-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/docs/index.rst` & `halborn_ctf-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/docs/src/getting_started/examples.rst` & `halborn_ctf-0.1.9/docs/src/getting_started/examples.rst`

 * *Files 10% similar despite different names*

```diff
@@ -52,77 +52,41 @@
 
     ...
 
 
 Filtering
 ======================
 
-Inline:
-
-.. code::
-
-
-    import halborn_ctf.network as network
-
-    ...
-
-        PATH_MAPPING = {
-            '/': {
-                    'port': 8545,
-                    'path': '/',
-                    'methods': ['POST']
-            },
-        }
-
-        ...
-
-        def run(self):
-            network.filters.json_rpc.filter_methods([], listen_port=8545, to_port=8546)
-
-
 On the ``PATH_MAPPING``:
 
 
 .. code::
 
-    import halborn_ctf.network as network
+    import halborn_ctf.network.filters as filters
 
     ...
 
         PATH_MAPPING = {
             '/': {
                     'port': 8545,
                     'path': '/',
                     'methods': ['POST'],
-                    'filter': {
-                        'method': network.filters.json_rpc.filter_methods,
-                        'args': [
-                            ['evm_.*']
-                        ],
-                    }
+                    'filter': filters.json_rpc.whitelist_methods(['evm_.*']),
             },
         }
 
 With custom filter on the ``PATH_MAPPING``:
 
 .. code::
 
-    import halborn_ctf.network as network
+    import halborn_ctf.network.filters as filters
 
     ...
 
         PATH_MAPPING = {
             '/': {
                     'port': 8545,
                     'path': '/',
                     'methods': ['POST'],
-                    'filter': {
-                        'method': network.filters.run_script,
-                        'args': [
-                            ['filter.py']
-                        ],
-                        'kwargs': {
-                            'context_argument': 0x1337
-                        },
-                    }
+                    'filter': filters.generic_filter('filter_file.py', my_arg=[], extra='more'),
             },
         }
```

### Comparing `halborn_ctf-0.1.8/docs/src/getting_started/installation.rst` & `halborn_ctf-0.1.9/docs/src/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/docs/src/getting_started/quick_start.rst` & `halborn_ctf-0.1.9/docs/src/getting_started/quick_start.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/docs/src/user_guide/faq.rst` & `halborn_ctf-0.1.9/docs/src/user_guide/faq.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/setup.cfg` & `halborn_ctf-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/setup.py` & `halborn_ctf-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf/__init__.py` & `halborn_ctf-0.1.9/src/halborn_ctf/__init__.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf/cli.py` & `halborn_ctf-0.1.9/src/halborn_ctf/cli.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf/functions.py` & `halborn_ctf-0.1.9/src/halborn_ctf/functions.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf/network/_generic.py` & `halborn_ctf-0.1.9/src/halborn_ctf/network/_generic.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf/network/filters/__init__.py` & `halborn_ctf-0.1.9/src/halborn_ctf/network/filters/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,21 +28,21 @@
         # We can also use the whitelist variant to only allow those methods
         # network.filters.json_rpc.whitelist_methods(['net_*', 'eth_*'...], listen_port=8545, to_port=9999)
 
 It is possible to also define your own filters (which can later be exposed to the player for reference) by either referencing the current 
 implementations or the official documentation (https://2qwesgdhjuiytyrjhtgdbf.readthedocs.io/en/latest/scripting/inlinescripts.html).
 
 Example:
-    Once the script is created it can be executed using :class:`run_script`::
+    Once the script is created it can be executed using :class:`generic_filter`::
 
-        run_script('./filter.py', listen_port=8545, to_port=9999, custom='More data')
+        generic_filter('./filter.py', my_args=[], extra_custom='more')
         ...
         # The script can access the extra **kwargs using ``ctx.options.[kwargname]`` and JSON decoding it
         custom_data = json.loads(ctx.options.custom)
 
 """
 from . import json_rpc
-from ._utils import run_script
+from ._utils import generic_filter
 
 __all__ = [
-    'run_script'
+    'generic_filter'
 ]
```

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py` & `halborn_ctf-0.1.9/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from mitmproxy import ctx
 from mitmproxy import http
 import re
 import json
 
 class FilterJSONRPCMethod:
-    def __init__(self):
-        self.num = 0
 
     def load(self, loader):
         loader.add_option(
             name="methods",
             typespec=str,
             default="",
             help="Methods to whitelist",
```

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py` & `halborn_ctf-0.1.9/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from mitmproxy import ctx
 from mitmproxy import http
 import re
 import json
 
 class WhitelistJSONRPCMethod:
-    def __init__(self):
-        self.num = 0
 
     def load(self, loader):
         loader.add_option(
             name="methods",
             typespec=str,
             default="",
             help="Methods to whitelist",
```

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf/network/filters/_utils.py` & `halborn_ctf-0.1.9/src/halborn_ctf/network/filters/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 from ...shell import run as _run
 import json
 
-def run_script(script, listen_port, to_port, to_host='127.0.0.1', **kwargs):
+def generic_filter(filter_file, **kwargs):
     """Allows running an arbitrary ``mitmdump`` script as a background shell process.
 
     The ``mitmdump`` will be used in ``upstream`` mode against ``http://{to_host}:{to_port}`` 
-    and listen under ``listen_port``. Any extra arguments provided to the ``run_script`` will be 
+    and listen under ``listen_port``. Any extra arguments provided to the ``generic_filter`` will be
     transfered to the ``script`` using the ``--set`` command flag on the command line of mitmdump 
     as JSON encoded string which can be accessed on the script using ``mitmproxy.ctx.options.[varname]``.
 
     Example:
-        Once the script is created it can be executed using :class:`run_script`::
+        Once the script is created it can be executed using :class:`generic_filter`::
 
-            run_script('./filter.py', listen_port=8545, to_port=9999, custom='More data')
+            generic_filter('./filter.py', listen_port=8545, to_port=9999, custom='More data')
             ...
             # The script can access the extra **kwargs using ``ctx.options.[kwargname]`` and JSON decoding it
             custom_data = json.loads(ctx.options.custom)
 
     Args:
         script (str): Path of the script to execute
         listen_port (int): Port that mitmdump will listen on
         to_port (int): The upstream port to proxy traffic to
         to_host (str): The upstream host to proxy traffic to. Defaults to '127.0.0.1'.
     """
+    def _wrapper(listen_port, to_port, to_host='127.0.0.1'):
+        set_args = ' '.join(['--set {0}={1}'.format(k, json.dumps(json.dumps(v))) for k,v in kwargs.items()])
 
-    # The double escape is for the cli to handle it as part as the --set definition (ex method="[\"data\"]")
-    set_args = ' '.join(['--set {0}={1}'.format(k, json.dumps(json.dumps(v))) for k,v in kwargs.items()])
+        cmd = f'mitmdump -s {filter_file} --mode upstream:http://{to_host}:{to_port} -p {listen_port} {set_args}'
+        _run(cmd, background=True)
 
-    cmd = f'mitmdump -s {script} --mode upstream:http://{to_host}:{to_port} -p {listen_port} {set_args}'
-    _run(cmd, background=True)
+    return _wrapper
+
+# def generic_filter(script, listen_port, to_port, to_host='127.0.0.1', **kwargs):
+
+#     # The double escape is for the cli to handle it as part as the --set definition (ex method="[\"data\"]")
+#     set_args = ' '.join(['--set {0}={1}'.format(k, json.dumps(json.dumps(v))) for k,v in kwargs.items()])
+
+#     cmd = f'mitmdump -s {script} --mode upstream:http://{to_host}:{to_port} -p {listen_port} {set_args}'
+#     _run(cmd, background=True)
```

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf/network/filters/json_rpc.py` & `halborn_ctf-0.1.9/src/halborn_ctf/network/filters/json_rpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from ._json_rpc import whitelist_json_rpc_method
 from ._json_rpc import filter_json_rpc_method
 
-from  ._utils import run_script
+from  ._utils import generic_filter
 
-def whitelist_methods(methods=[], *, listen_port, to_port, to_host='127.0.0.1'):
+def whitelist_methods(methods=[]):
     """Proxy filter that allows whitelisting JSON RPC methods
 
-    The proxy will expose a service that will be listening on ``listen_port`` and redirect
-    all traffic to ``to_host:to_port``.
-
     Each request will be checked for a valid method and if the method is not whitelisted 
     the following data will be send::
 
         {
             "jsonrpc": "2.0",
             "id": json_dump['id'],
             "error": {
@@ -22,31 +19,25 @@
         }
 
     Example:
 
         The ``methods`` parameter does support regex on each of the elements::
 
             # Allowing all methods starting with `eth_` and `net_`
-            whitelist_methods(["eth_.*", "net_.*"], listen_port=8545, to_port=8546)
+            whitelist_methods(["eth_.*", "net_.*"])
 
     Args:
         methods (list, optional): A list of methods to whitelist. Each element of the 
             list does support regex expressions to match multiple patterns. Example: ``["eth_.*"]``. Defaults to [].
-        listen_port (int): The port that will expose the proxy filter server 
-        to_port (int): The port that all traffic will be redirected to 
-        to_host (str, optional): The host that all traffic will be redirected to. Defaults to '127.0.0.1'.
     """
-    run_script(whitelist_json_rpc_method.__file__, **locals())
+    return generic_filter(whitelist_json_rpc_method.__file__, **locals())
 
-def filter_methods(methods=[], *, listen_port, to_port, to_host='127.0.0.1'):
+def filter_methods(methods=[]):
     """Proxy filter that allows filtering JSON RPC method
 
-    The proxy will expose a service that will be listening on ``listen_port`` and redirect
-    all traffic to ``to_host:to_port``.
-
     Each request will be checked for a valid method and if the method is on the filter list 
     the following data will be send::
 
         {
             "jsonrpc": "2.0",
             "id": json_dump['id'],
             "error": {
@@ -56,22 +47,19 @@
         }
 
     Example:
 
         The ``methods`` parameter does support regex on each of the elements::
 
             # Disable all methods starting with `anvil_` and `evm_`
-            filter_methods(["anvil_.*", "evm_.*"], listen_port=8545, to_port=8546)
+            filter_methods(["anvil_.*", "evm_.*"])
 
     Args:
         methods (list, optional): A list of methods to filter. Each element of the 
             list does support regex expressions to match multiple patterns. Example: ``["evm_.*"]``. Defaults to [].
-        listen_port (int): The port that will expose the proxy filter server 
-        to_port (int): The port that all traffic will be redirected to 
-        to_host (str, optional): The host that all traffic will be redirected to. Defaults to '127.0.0.1'.
     """
-    run_script(filter_json_rpc_method.__file__, **locals())
+    return generic_filter(filter_json_rpc_method.__file__, **locals())
 
 __all__ = [
     'whitelist_methods',
     'filter_methods'
 ]
```

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf/shell.py` & `halborn_ctf-0.1.9/src/halborn_ctf/shell.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf/state.py` & `halborn_ctf-0.1.9/src/halborn_ctf/state.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf/templates.py` & `halborn_ctf-0.1.9/src/halborn_ctf/templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,28 +66,14 @@
       os.killpg(0, signal.SIGINT) # kill all processes in my group
     except KeyboardInterrupt:
       # SIGINT is delievered to this process as well as the child processes.
       # Ignore it so that the existing exception, if any, is returned. This
       # leaves us with a clean exit code if there was no exception.
       pass
 
-class MappingInfoFilter(TypedDict):
-    """Dictionary data type to store the details for a filter used on a mapping.
-    """
-
-    method: Callable
-    """ (Callable): The function that runs the filter.
-    """
-    args: NotRequired[list]
-    """ (list, optional): The list of arguments for the filter function.
-    """
-    kwargs: NotRequired[str]
-    """ (dict, optional): The kwargs for the filter function, only used by default on custom filters and will be passed on the script inside ``ctx.options.[HERE]``.
-    """
-
 class MappingInfo(TypedDict):
     """Dictionary data type to store the details for a path mapping
     """
 
     port: int
     """ (int): The port to redirect to.
     """
@@ -96,16 +82,16 @@
     """
     path: NotRequired[str]
     """ (str, optional): The path to redirect to. Defaults to ``'/'``.
     """
     methods: list[str]
     """ (list[str], optional): The allowed methods. Defaults to ``["GET"]``.
     """
-    filter: NotRequired[MappingInfoFilter]
-    """ (MappingInfoFilter, optional): Information containing a filter to execute.
+    filter: Callable
+    """ (Callable, optional): One of the valid built-in filters or a generic_filter function. 
     """
 
 class FlagType(Enum):
     NONE = 0
     """If no flag is present
     """
     STATIC = 1
@@ -249,15 +235,15 @@
                 }
             )
 
     Note:
         This function will be executed each time the user requests the ``/info`` route.
     """
 
-    PATH_MAPPING = {}
+    PATH_MAPPING: dict[str, MappingInfo] = {}
     """
     (dict[str, MappingInfo]): Mapping used internally to register the challenge URL's paths.
     It does contain a mapping of ``path`` to ``MappingInfo`` dictionary details.
 
     Example:
         Have the challenge ``/`` path expose the anvil service which is running internally on port ``8545``::
 
@@ -287,44 +273,39 @@
         It allows to use filters::
 
             PATH_MAPPING = {
                 '/': {
                         'port': 8545,
                         'path': '/',
                         'methods': ['POST'],
-                        'filter': {
-                            'method': network.filters.json_rpc.filter_methods,
-                            'args': [],
-
-                            # Custom filter
-                            # 'method': network.filters.run_script,
-                            # 'args': ['filter.py'],
-                            # 'kwargs': {}
-                        }
+                        'filter': network.filters.json_rpc.whitelist_methods(['evm_.*']),
                 }
             }
 
     Note:
         There is no need to specify any of the required field for the filter such as ``listen_port``, ``to_port``, ``to_host`` as those will
         be extracted from the mapping itself and a random listening port used and remapped.
     """
 
     def _check_feature_enabled(self, feature_name, required_function):
         if getattr(self, feature_name):
             try:
                 getattr(self, required_function)
             except:
                 raise NotImplementedError(f'Missing function "{required_function}" ({feature_name} == True)')
+
+            self._challenge_config[feature_name] = True
         else:
             try:
                 getattr(self, required_function)
                 raise NotImplementedError(f'Remove "{required_function}" function ({feature_name} == False)')
             except:
                 pass
 
+            self._challenge_config[feature_name] = False
 
 
     def __init__(self) -> None:
         super().__init__()
 
         self._app = flask.Flask('Challenge')
         self.log = logging.getLogger(self.CHALLENGE_NAME)
@@ -333,33 +314,30 @@
 
         self._ready = False
         self._state_set = False
         self._state = State({})
         self._state_public_set = False
         self._state_public = State({})
 
-        #     'public': State({}),
-        #     'ready': False,
-        # })
+        self._challenge_config = {}
+        self._challenge_config['FLAG_TYPE'] = self.FLAG_TYPE.name
 
         if self.HAS_SOLVER:
             self._solved = False
             self._solved_msg = None
             # self._state._setattr('solved', False)
             # self._state._setattr('solved_msg', None)
 
         self._check_feature_enabled('HAS_FILES', 'files')
         self._check_feature_enabled('HAS_SOLVER', 'solver')
         self._check_feature_enabled('HAS_DETAILS', 'details')
 
         if not self.HAS_SOLVER and self.FLAG_TYPE == FlagType.NONE:
             raise ValueError("HAS_SOLVER == False and FLAG_TYPE == NONE")
 
-        self._path_mapping: dict[str, MappingInfo] = {}
-
     # @property
     # def ready(self):
     #     """(bool): Allows setting the challenge as ready to be played.
 
     #         Example::
 
     #             def run(self):
@@ -471,17 +449,29 @@
         # self._state_public_set = State(value)
         self._state_public_set = True
 
     def _app_info_handler(self):
         # if not self._ready:
         #     return Response("Challenge not ready", status=503)
 
+        _mapping: dict[str, MappingInfo] = {}
+        for k,v in self.PATH_MAPPING.items():
+            _mapping[k] = {
+                'port': v.get('port'),
+                'host': v.get('host', '127.0.0.1'),
+                'path': v.get('path', '/'),
+                'methods': v.get('methods', ['GET']),
+                # 'filter': _filter
+            }
+
         _return = {
             'ready': self._ready,
             'state': self._state_public,
+            'config': self._challenge_config,
+            'mapping': _mapping
         }
 
         if self.HAS_DETAILS:
             _return['details'] = dedent(self.details()).strip()
         else:
             _return['details'] = None
 
@@ -573,22 +563,19 @@
         for i, values in enumerate(self.PATH_MAPPING.items()):
             path, path_data = values
             methods = path_data.get('methods', ['GET'])
             host = path_data.get('host', '127.0.0.1')
             port = path_data['port']
             # TODO: Verify methods and path_data
             _filter = path_data.get('filter', None)
-            if _filter and _filter['method']:
-                _filter_args = _filter.get('args', [])
-                _filter_kwargs = _filter.get('kwargs', {})
+            if _filter:
 
                 random_port = find_free_port()
 
-                # The filter should listen on random port and redirect to host:port
-                _filter['method'](*_filter_args, **_filter_kwargs, listen_port=random_port, to_port=port, to_host=host)
+                _filter(listen_port=random_port, to_port=port, to_host=host)
 
                 # The path mapping should redirect to 127.0.0.1:random_port
                 self._app.add_url_rule(path, 'mapping-{}'.format(i), self._generic_path_handler(port=random_port, host='127.0.0.1', path=path), methods=methods)
             else:
                 self._app.add_url_rule(path, 'mapping-{}'.format(i), self._generic_path_handler(port=port, host=host, path=path), methods=methods)
 
     def _flask_run(self):
@@ -632,14 +619,16 @@
 
             self.run()
 
             self._register_challenge_paths()
 
             self._ready = True
 
+            # TODO: Try to run in on a thread and start it before the self.run function. This will allow to notify the ready state
+            # in case a backgroun process is not specified as background.
             self._flask_run()
 
 
     @abstractmethod
     def build(self):
         """All the static funtionality that should be executed during the build phase of the challenge container. The running container will
         have everything executed here pre-bundled as this funcionality is only executed once for all running instances.
```

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf.egg-info/PKG-INFO` & `halborn_ctf-0.1.9/src/halborn_ctf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halborn-ctf
-Version: 0.1.8
+Version: 0.1.9
 Summary: Add a short description here!
 Home-page: https://github.com/HalbornAcademy/halborn_ctf
 Author: ferran.celades
 Author-email: ferran.celades@halborn.com
 License: MIT
 Project-URL: Documentation, https://halborn-ctf.readthedocs.io/
 Platform: any
```

### Comparing `halborn_ctf-0.1.8/src/halborn_ctf.egg-info/SOURCES.txt` & `halborn_ctf-0.1.9/src/halborn_ctf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/tests/test_skeleton.py` & `halborn_ctf-0.1.9/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.8/tox.ini` & `halborn_ctf-0.1.9/tox.ini`

 * *Files identical despite different names*

