# Comparing `tmp/wwpdb.utils.wf-0.34.tar.gz` & `tmp/wwpdb.utils.wf-0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.wf-0.34.tar", last modified: Tue Jun 13 02:58:17 2023, max compression
+gzip compressed data, was "wwpdb.utils.wf-0.35.tar", last modified: Sat Jun 17 11:34:49 2023, max compression
```

## Comparing `wwpdb.utils.wf-0.34.tar` & `wwpdb.utils.wf-0.35.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.305676 wwpdb.utils.wf-0.34/
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-06-13 02:58:17.305676 wwpdb.utils.wf-0.34/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      485 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-13 02:58:17.305676 wwpdb.utils.wf-0.34/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2105 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.293676 wwpdb.utils.wf-0.34/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.297676 wwpdb.utils.wf-0.34/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.297676 wwpdb.utils.wf-0.34/wwpdb/utils/wf/
--rw-r--r--   0 vsts      (1001) docker     (123)     3229 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/DataSelector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4658 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/DataValueContainer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3661 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/WfDataObject.py
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.297676 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/
--rw-r--r--   0 vsts      (1001) docker     (123)     6846 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/DbApiUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16002 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/DbCommand.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4025 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/DbConnection.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1946 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/LocalDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3018 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/StatusDbApi.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1281 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/WFEtime.py
--rw-r--r--   0 vsts      (1001) docker     (123)    47456 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/WfDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4251 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/WfTracking.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11637 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/dbAPI.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.305676 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/
--rw-r--r--   0 vsts      (1001) docker     (123)    65750 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/AnnotationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11876 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/ChemCompUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3611 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/DictUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3595 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/DpUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17700 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/EmUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6275 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/FileUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13301 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/FormatUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    50817 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/NmrUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13901 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/PdbxUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3840 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/PrdSearchUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3427 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/ReportUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5580 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/SFConvert.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5698 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/SeqStatsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11212 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/SeqdbUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1456 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/UtilsBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)    24022 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/ValidationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.305676 wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/
--rw-r--r--   0 vsts      (1001) docker     (123)    15843 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/ActionRegistry.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7456 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/ActionRegistryIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11325 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/ProcessRunner.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.305676 wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/
--rw-r--r--   0 vsts      (1001) docker     (123)    12006 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/WfSchemaMap.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11697 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/database_descriptions.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/mandatory_items.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.293676 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-06-13 02:58:17.000000 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1724 2023-06-13 02:58:17.000000 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 02:58:17.000000 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 02:58:03.000000 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-06-13 02:58:17.000000 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-13 02:58:17.000000 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:34:49.147414 wwpdb.utils.wf-0.35/
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-06-17 11:34:49.147414 wwpdb.utils.wf-0.35/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      485 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-17 11:34:49.147414 wwpdb.utils.wf-0.35/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2105 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:34:49.143414 wwpdb.utils.wf-0.35/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:34:49.143414 wwpdb.utils.wf-0.35/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:34:49.143414 wwpdb.utils.wf-0.35/wwpdb/utils/wf/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3229 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/DataSelector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4658 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/DataValueContainer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3661 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/WfDataObject.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:34:49.143414 wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6846 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/DbApiUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16002 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/DbCommand.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4025 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/DbConnection.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1946 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/LocalDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3018 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/StatusDbApi.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1281 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/WFEtime.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    47456 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/WfDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4251 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/WfTracking.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11637 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/dbAPI.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:34:49.147414 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/
+-rw-r--r--   0 vsts      (1001) docker     (123)    65750 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/AnnotationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11876 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/ChemCompUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3611 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/DictUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3595 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/DpUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17700 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/EmUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6275 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/FileUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13301 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/FormatUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    50817 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/NmrUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13901 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/PdbxUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3840 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/PrdSearchUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3427 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/ReportUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5580 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/SFConvert.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5698 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/SeqStatsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11212 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/SeqdbUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1456 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/UtilsBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    24022 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/ValidationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:34:49.147414 wwpdb.utils.wf-0.35/wwpdb/utils/wf/process/
+-rw-r--r--   0 vsts      (1001) docker     (123)    15843 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/process/ActionRegistry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7456 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/process/ActionRegistryIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11325 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/process/ProcessRunner.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/process/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:34:49.147414 wwpdb.utils.wf-0.35/wwpdb/utils/wf/schema/
+-rw-r--r--   0 vsts      (1001) docker     (123)    12006 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/schema/WfSchemaMap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/schema/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11697 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/schema/database_descriptions.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-06-17 11:33:58.000000 wwpdb.utils.wf-0.35/wwpdb/utils/wf/schema/mandatory_items.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:34:49.143414 wwpdb.utils.wf-0.35/wwpdb.utils.wf.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-06-17 11:34:49.000000 wwpdb.utils.wf-0.35/wwpdb.utils.wf.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1724 2023-06-17 11:34:49.000000 wwpdb.utils.wf-0.35/wwpdb.utils.wf.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-17 11:34:49.000000 wwpdb.utils.wf-0.35/wwpdb.utils.wf.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-17 11:34:38.000000 wwpdb.utils.wf-0.35/wwpdb.utils.wf.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-06-17 11:34:49.000000 wwpdb.utils.wf-0.35/wwpdb.utils.wf.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-17 11:34:49.000000 wwpdb.utils.wf-0.35/wwpdb.utils.wf.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.wf-0.34/LICENSE` & `wwpdb.utils.wf-0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/PKG-INFO` & `wwpdb.utils.wf-0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.wf
-Version: 0.34
+Version: 0.35
 Summary: OneDep WF status DB access utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_wf
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.wf-0.34/setup.py` & `wwpdb.utils.wf-0.35/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     #
-    install_requires=["mysqlclient", "wwpdb.utils.config >= 0.22.2", "wwpdb.io", "mmcif", "wwpdb.utils.dp ~= 0.40", "wwpdb.utils.session"],
+    install_requires=["mysqlclient", "wwpdb.utils.config >= 0.22.2", "wwpdb.io", "mmcif", "wwpdb.utils.dp ~= 0.47", "wwpdb.utils.session"],
     packages=find_packages(exclude=["wwpdb.utils.tests_wf", "mock-data", "tests.*"]),
     package_data={
         # If any package contains *.md or *.rst ...  files, include them:
         "": ["*.md", "*.rst", "*.txt", "*.cfg"],
     },
     #
     # These basic tests require no database services -
```

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/DataSelector.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/DataSelector.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/DataValueContainer.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/DataValueContainer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/WfDataObject.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/WfDataObject.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/DbApiUtil.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/DbApiUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/DbCommand.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/DbCommand.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/DbConnection.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/DbConnection.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/LocalDbApi.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/LocalDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/StatusDbApi.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/StatusDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/WFEtime.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/WFEtime.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/WfDbApi.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/WfDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/WfTracking.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/WfTracking.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/dbAPI.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/dbapi/dbAPI.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/AnnotationUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/AnnotationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/ChemCompUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/ChemCompUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/DictUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/DictUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/DpUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/DpUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/EmUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/EmUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/FileUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/FileUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/FormatUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/FormatUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/NmrUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/NmrUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/PdbxUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/PdbxUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/PrdSearchUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/PrdSearchUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/ReportUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/ReportUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/SFConvert.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/SFConvert.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/SeqStatsUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/SeqStatsUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/SeqdbUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/SeqdbUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/UtilsBase.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/UtilsBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/ValidationUtils.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/plugins/ValidationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/ActionRegistry.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/process/ActionRegistry.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/ActionRegistryIo.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/process/ActionRegistryIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/ProcessRunner.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/process/ProcessRunner.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/WfSchemaMap.py` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/schema/WfSchemaMap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/database_descriptions.txt` & `wwpdb.utils.wf-0.35/wwpdb/utils/wf/schema/database_descriptions.txt`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/PKG-INFO` & `wwpdb.utils.wf-0.35/wwpdb.utils.wf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.wf
-Version: 0.34
+Version: 0.35
 Summary: OneDep WF status DB access utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_wf
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/SOURCES.txt` & `wwpdb.utils.wf-0.35/wwpdb.utils.wf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

