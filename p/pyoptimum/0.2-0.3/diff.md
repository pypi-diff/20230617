# Comparing `tmp/pyoptimum-0.2.tar.gz` & `tmp/pyoptimum-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoptimum-0.2.tar", last modified: Sun May  8 15:31:24 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pyoptimum-0.2.tar` & `pyoptimum-0.3.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxr-x   0 mauricio  (1000) mauricio  (1000)        0 2022-05-08 15:31:24.337634 pyoptimum-0.2/
--rw-rw-r--   0 mauricio  (1000) mauricio  (1000)     1077 2020-02-29 16:38:32.000000 pyoptimum-0.2/LICENSE
--rw-rw-r--   0 mauricio  (1000) mauricio  (1000)      675 2022-05-08 15:31:24.337634 pyoptimum-0.2/PKG-INFO
--rw-rw-r--   0 mauricio  (1000) mauricio  (1000)      100 2020-02-29 16:38:32.000000 pyoptimum-0.2/README.md
-drwxrwxr-x   0 mauricio  (1000) mauricio  (1000)        0 2022-05-08 15:31:24.337634 pyoptimum-0.2/pyoptimum/
--rw-rw-r--   0 mauricio  (1000) mauricio  (1000)     2096 2022-05-08 14:06:35.000000 pyoptimum-0.2/pyoptimum/__init__.py
-drwxrwxr-x   0 mauricio  (1000) mauricio  (1000)        0 2022-05-08 15:31:24.337634 pyoptimum-0.2/pyoptimum.egg-info/
--rw-rw-r--   0 mauricio  (1000) mauricio  (1000)      675 2022-05-08 15:31:23.000000 pyoptimum-0.2/pyoptimum.egg-info/PKG-INFO
--rw-rw-r--   0 mauricio  (1000) mauricio  (1000)      222 2022-05-08 15:31:24.000000 pyoptimum-0.2/pyoptimum.egg-info/SOURCES.txt
--rw-rw-r--   0 mauricio  (1000) mauricio  (1000)        1 2022-05-08 15:31:24.000000 pyoptimum-0.2/pyoptimum.egg-info/dependency_links.txt
--rw-rw-r--   0 mauricio  (1000) mauricio  (1000)        9 2022-05-08 15:31:24.000000 pyoptimum-0.2/pyoptimum.egg-info/requires.txt
--rw-rw-r--   0 mauricio  (1000) mauricio  (1000)       10 2022-05-08 15:31:24.000000 pyoptimum-0.2/pyoptimum.egg-info/top_level.txt
--rw-rw-r--   0 mauricio  (1000) mauricio  (1000)       79 2022-05-08 15:31:24.337634 pyoptimum-0.2/setup.cfg
--rw-rw-r--   0 mauricio  (1000) mauricio  (1000)      829 2022-05-08 15:30:58.000000 pyoptimum-0.2/setup.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pyoptimum-0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyoptimum-0.3/requirements.txt
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 pyoptimum-0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 pyoptimum-0.3/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/Makefile
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/conf.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/make.bat
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/requirements.txt
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/src/modules.rst
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/src/quickstart.rst
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 pyoptimum-0.3/src/pyoptimum/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyoptimum-0.3/tests/__init__.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 pyoptimum-0.3/tests/test_basic.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pyoptimum-0.3/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyoptimum-0.3/LICENSE
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 pyoptimum-0.3/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pyoptimum-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyoptimum-0.3/PKG-INFO
```

### Comparing `pyoptimum-0.2/LICENSE` & `pyoptimum-0.3/LICENSE`

 * *Files identical despite different names*

