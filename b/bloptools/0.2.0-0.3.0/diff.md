# Comparing `tmp/bloptools-0.2.0.tar.gz` & `tmp/bloptools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloptools-0.2.0.tar", last modified: Tue Apr 25 16:05:18 2023, max compression
+gzip compressed data, was "bloptools-0.3.0.tar", last modified: Sat Jun 17 19:09:39 2023, max compression
```

## Comparing `bloptools-0.2.0.tar` & `bloptools-0.3.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.037809 bloptools-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-25 16:05:06.000000 bloptools-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-25 16:05:06.000000 bloptools-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-25 16:05:06.000000 bloptools-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-25 16:05:06.000000 bloptools-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-25 16:05:18.037809 bloptools-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-25 16:05:06.000000 bloptools-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.037809 bloptools-0.2.0/bloptools/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 16:05:18.037809 bloptools-0.2.0/bloptools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.029809 bloptools-0.2.0/bloptools/bo/
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/bo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/bo/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/bo/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/bo/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.029809 bloptools-0.2.0/bloptools/de/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/de/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/de/de_opt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26559 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/de/de_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/de/hardware_flyer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.029809 bloptools-0.2.0/bloptools/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.033809 bloptools-0.2.0/bloptools/experiments/atf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/atf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/atf/atf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.033809 bloptools-0.2.0/bloptools/experiments/nsls2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/nsls2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/nsls2/iss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/nsls2/tes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.033809 bloptools-0.2.0/bloptools/experiments/shadow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/shadow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/shadow/chx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/shadow/tes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.033809 bloptools-0.2.0/bloptools/experiments/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.033809 bloptools-0.2.0/bloptools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/tests/test_bayesian_himmelblau.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/tests/test_bayesian_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.029809 bloptools-0.2.0/bloptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-25 16:05:17.000000 bloptools-0.2.0/bloptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-25 16:05:17.000000 bloptools-0.2.0/bloptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:05:17.000000 bloptools-0.2.0/bloptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 16:05:17.000000 bloptools-0.2.0/bloptools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 16:05:17.000000 bloptools-0.2.0/bloptools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.033809 bloptools-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.037809 bloptools-0.2.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/min_versions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/release-history.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-25 16:05:06.000000 bloptools-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 16:05:06.000000 bloptools-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-25 16:05:18.037809 bloptools-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-25 16:05:06.000000 bloptools-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68503 2023-04-25 16:05:06.000000 bloptools-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.014958 bloptools-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-17 19:09:34.000000 bloptools-0.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-17 19:09:34.000000 bloptools-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-17 19:09:34.000000 bloptools-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-17 19:09:34.000000 bloptools-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-17 19:09:39.014958 bloptools-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-17 19:09:34.000000 bloptools-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.014958 bloptools-0.3.0/bloptools/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-17 19:09:39.014958 bloptools-0.3.0/bloptools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.010958 bloptools-0.3.0/bloptools/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)    23788 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/bayesian/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/bayesian/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/bayesian/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.010958 bloptools-0.3.0/bloptools/de/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/de/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/de/de_opt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26559 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/de/de_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/de/hardware_flyer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.010958 bloptools-0.3.0/bloptools/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.010958 bloptools-0.3.0/bloptools/experiments/atf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/experiments/atf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/experiments/atf/atf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.010958 bloptools-0.3.0/bloptools/experiments/nsls2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/experiments/nsls2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/experiments/nsls2/iss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/experiments/nsls2/tes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.010958 bloptools-0.3.0/bloptools/experiments/sirepo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/experiments/sirepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/experiments/sirepo/tes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.010958 bloptools-0.3.0/bloptools/experiments/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/experiments/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.010958 bloptools-0.3.0/bloptools/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.010958 bloptools-0.3.0/bloptools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/tests/test_bayesian_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/tests/test_bayesian_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-17 19:09:34.000000 bloptools-0.3.0/bloptools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.010958 bloptools-0.3.0/bloptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-17 19:09:38.000000 bloptools-0.3.0/bloptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-17 19:09:38.000000 bloptools-0.3.0/bloptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 19:09:38.000000 bloptools-0.3.0/bloptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 19:09:38.000000 bloptools-0.3.0/bloptools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-17 19:09:38.000000 bloptools-0.3.0/bloptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.010958 bloptools-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 19:09:34.000000 bloptools-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-17 19:09:34.000000 bloptools-0.3.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:09:39.014958 bloptools-0.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-06-17 19:09:34.000000 bloptools-0.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-17 19:09:34.000000 bloptools-0.3.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-17 19:09:34.000000 bloptools-0.3.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-17 19:09:34.000000 bloptools-0.3.0/docs/source/min_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-17 19:09:34.000000 bloptools-0.3.0/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-17 19:09:34.000000 bloptools-0.3.0/docs/source/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 19:09:34.000000 bloptools-0.3.0/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-17 19:09:34.000000 bloptools-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 19:09:34.000000 bloptools-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-17 19:09:39.014958 bloptools-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-17 19:09:34.000000 bloptools-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68503 2023-06-17 19:09:34.000000 bloptools-0.3.0/versioneer.py
```

### Comparing `bloptools-0.2.0/CONTRIBUTING.rst` & `bloptools-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bloptools-0.2.0/LICENSE` & `bloptools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bloptools-0.2.0/PKG-INFO` & `bloptools-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloptools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Beamline Optimization Tools
 Home-page: https://github.com/NSLS-II/bloptools
 Author: Brookhaven National Laboratory
 Author-email: mrakitin@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `bloptools-0.2.0/bloptools/bo/kernels.py` & `bloptools-0.3.0/bloptools/bayesian/kernels.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,46 +2,55 @@
 import numpy as np
 import torch
 
 
 class LatentMaternKernel(gpytorch.kernels.Kernel):
     def __init__(
         self,
-        n_dof,
-        off_diag=True,
+        n_dim,
+        off_diag=False,
+        diagonal_prior=False,
         **kwargs,
     ):
         super(LatentMaternKernel, self).__init__()
 
-        self.n_dof = n_dof
-        self.n_off_diag = int(n_dof * (n_dof - 1) / 2)
+        self.n_dim = n_dim
+        self.n_off_diag = int(n_dim * (n_dim - 1) / 2)
         self.off_diag = off_diag
 
         # output_scale_constraint = gpytorch.constraints.Positive()
-        trans_diagonal_constraint = gpytorch.constraints.Interval(2e0, 2e1)
+        trans_diagonal_constraint = gpytorch.constraints.Interval(1e0, 1e2)
         trans_off_diag_constraint = gpytorch.constraints.Interval(-1e0, 1e0)
 
         trans_diagonal_initial = np.sqrt(
             trans_diagonal_constraint.lower_bound * trans_diagonal_constraint.upper_bound
         )
         raw_trans_diagonal_initial = trans_diagonal_constraint.inverse_transform(trans_diagonal_initial)
 
         # self.register_parameter(
         #    name="raw_output_scale", parameter=torch.nn.Parameter(torch.ones(*self.batch_shape, 1).double())
         # )
         self.register_parameter(
             name="raw_trans_diagonal",
             parameter=torch.nn.Parameter(
-                raw_trans_diagonal_initial * torch.ones(*self.batch_shape, self.n_dof).double()
+                raw_trans_diagonal_initial * torch.ones(*self.batch_shape, self.n_dim).double()
             ),
         )
 
         # self.register_constraint("raw_output_scale", output_scale_constraint)
         self.register_constraint("raw_trans_diagonal", trans_diagonal_constraint)
 
+        if diagonal_prior:
+            self.register_prior(
+                name="trans_diagonal_prior",
+                prior=gpytorch.priors.GammaPrior(concentration=1, rate=0.2),
+                param_or_closure=lambda m: m.trans_diagonal,
+                setting_closure=lambda m, v: m._set_trans_diagonal(v),
+            )
+
         if self.off_diag:
             self.register_parameter(
                 name="raw_trans_off_diag",
                 parameter=torch.nn.Parameter(torch.zeros(*self.batch_shape, self.n_off_diag).double()),
             )
             self.register_constraint("raw_trans_off_diag", trans_off_diag_constraint)
 
@@ -84,20 +93,20 @@
             value = torch.as_tensor(value).to(self.raw_trans_diagonal)
         self.initialize(raw_trans_diagonal=self.raw_trans_diagonal_constraint.inverse_transform(value))
 
     @property
     def trans_matrix(self):
         # no rotations
         if not self.off_diag:
-            T = torch.eye(self.n_dof).double()
+            T = torch.eye(self.n_dim).double()
 
         # construct an orthogonal matrix. fun fact: exp(skew(N)) is the generator of SO(N)
         else:
-            A = torch.zeros((self.n_dof, self.n_dof)).double()
-            A[np.triu_indices(self.n_dof, k=1)] = self.trans_off_diag
+            A = torch.zeros((self.n_dim, self.n_dim)).double()
+            A[np.triu_indices(self.n_dim, k=1)] = self.trans_off_diag
             A += -A.T
             T = torch.linalg.matrix_exp(A)
 
         T = torch.matmul(torch.diag(self.trans_diagonal), T)
 
         return T
 
@@ -107,30 +116,36 @@
             # return torch.square(self.output_scale[0]) * torch.ones((*self.batch_shape, *x1.shape[:-1]))
             return torch.ones((*self.batch_shape, *x1.shape[:-1]))
 
         # computes the autocovariance of the process at the parameters
         if auto:
             x2 = x1
 
-        # x1 and x2 are arrays of shape (..., n_1, n_dof) and (..., n_2, n_dof)
+        # print(x1, x2)
+
+        # x1 and x2 are arrays of shape (..., n_1, n_dim) and (..., n_2, n_dim)
         _x1, _x2 = torch.as_tensor(x1).double(), torch.as_tensor(x2).double()
 
-        # dx has shape (..., n_1, n_2, n_dof)
+        # dx has shape (..., n_1, n_2, n_dim)
         dx = _x1.unsqueeze(-2) - _x2.unsqueeze(-3)
 
         # transform coordinates with hyperparameters (this applies lengthscale and rotations)
         trans_dx = torch.matmul(self.trans_matrix, dx.unsqueeze(-1))
 
         # total transformed distance. D has shape (..., n_1, n_2)
         d_eff = torch.sqrt(torch.matmul(trans_dx.transpose(-1, -2), trans_dx).sum((-1, -2)) + 1e-12)
 
         # Matern covariance of effective order nu=3/2.
         # nu=3/2 is a special case and has a concise closed-form expression
         # In general, this is something between an exponential (n=1/2) and a Gaussian (n=infinity)
         # https://en.wikipedia.org/wiki/Matern_covariance_function
-        C = (1 + d_eff) * torch.exp(-d_eff)
+
+        # C = torch.exp(-d_eff) # Matern_0.5 (exponential)
+        C = (1 + d_eff) * torch.exp(-d_eff)  # Matern_1.5
+        # C = (1 + d_eff + 1 / 3 * torch.square(d_eff)) * torch.exp(-d_eff)  # Matern_2.5
+        # C = torch.exp(-0.5 * np.square(d_eff)) # Matern_infinity (RBF)
 
         # C = torch.square(self.output_scale[0]) * torch.exp(-torch.square(d_eff))
 
         # print(f'{diag = } {C.shape = }')
 
         return C
```

### Comparing `bloptools-0.2.0/bloptools/de/de_opt_utils.py` & `bloptools-0.3.0/bloptools/de/de_opt_utils.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.2.0/bloptools/de/de_optimization.py` & `bloptools-0.3.0/bloptools/de/de_optimization.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.2.0/bloptools/de/hardware_flyer.py` & `bloptools-0.3.0/bloptools/de/hardware_flyer.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.2.0/bloptools/experiments/nsls2/tes.py` & `bloptools-0.3.0/bloptools/experiments/nsls2/tes.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.2.0/bloptools/tests/conftest.py` & `bloptools-0.3.0/bloptools/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.2.0/bloptools/utils.py` & `bloptools-0.3.0/bloptools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,24 @@
 
 def get_routing(origin, points):
     """
     Finds an efficient routing between $n$ points, after normalizing each dimension.
     Returns $n-1$ indices, ignoring the zeroeth index (the origin).
     """
 
+    if not len(points) > 1:
+        return np.array([0]), 1.0
+
     _points = np.r_[np.atleast_2d(origin), points]
 
-    rel_points = _points / _points.std(axis=0)
+    rel_points = _points / np.array([std if std > 0 else 1.0 for std in points.std(axis=0)])
 
     # delay_matrix = gpo.delay_estimate(rel_points[:,None,:] - rel_points[None,:,:])
     delay_matrix = np.sqrt(np.square(rel_points[:, None, :] - rel_points[None, :, :]).sum(axis=-1))
-    delay_matrix = (1e6 * delay_matrix).astype(int)  # it likes integers idk
+    delay_matrix = (1e3 * delay_matrix).astype(int)  # it likes integers idk
 
     manager = pywrapcp.RoutingIndexManager(
         len(_points), 1, 0
     )  # number of depots, number of salesmen, starting index
     routing = pywrapcp.RoutingModel(manager)
 
     def delay_callback(from_index, to_index):
```

### Comparing `bloptools-0.2.0/bloptools.egg-info/PKG-INFO` & `bloptools-0.3.0/bloptools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloptools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Beamline Optimization Tools
 Home-page: https://github.com/NSLS-II/bloptools
 Author: Brookhaven National Laboratory
 Author-email: mrakitin@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `bloptools-0.2.0/docs/Makefile` & `bloptools-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bloptools-0.2.0/docs/make.bat` & `bloptools-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bloptools-0.2.0/docs/source/conf.py` & `bloptools-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.2.0/docs/source/min_versions.rst` & `bloptools-0.3.0/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `bloptools-0.2.0/docs/source/release-history.rst` & `bloptools-0.3.0/docs/source/release-history.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 ===============
 Release History
 ===============
 
+v0.3.0 (2023-06-17)
+-------------------
+
+- Implemented multi-task optimization
+- Simplified the syntax on initializing the agent
+- Resolved issues discovered at ISS
+
 
 v0.2.0 (2023-04-25)
 -------------------
 
 - Rebased the Bayesian optimization models to be compatible with ``botorch`` code.
 - Optimization objectives can be customized with ``experiment`` modules.
 - Added optimization test functions for quicker testing and development.
```

### Comparing `bloptools-0.2.0/setup.py` & `bloptools-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.2.0/versioneer.py` & `bloptools-0.3.0/versioneer.py`

 * *Files identical despite different names*

