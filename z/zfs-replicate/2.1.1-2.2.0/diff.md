# Comparing `tmp/zfs_replicate-2.1.1.tar.gz` & `tmp/zfs_replicate-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zfs_replicate-2.1.1.tar", max compression
+gzip compressed data, was "zfs_replicate-2.2.0.tar", max compression
```

## Comparing `zfs_replicate-2.1.1.tar` & `zfs_replicate-2.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1290 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/LICENSE
--rw-r--r--   0        0        0     3385 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/README.md
--rw-r--r--   0        0        0     1640 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/__init__.pyi
--rw-r--r--   0        0        0       33 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/__init__.py
--rw-r--r--   0        0        0       35 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/cli/__init__.py
--rw-r--r--   0        0        0      912 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/cli/click.py
--rw-r--r--   0        0        0     4164 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/cli/main.py
--rw-r--r--   0        0        0      203 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/compress/__init__.py
--rw-r--r--   0        0        0      484 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/compress/command.py
--rw-r--r--   0        0        0      170 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/compress/type.py
--rw-r--r--   0        0        0      327 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/error.py
--rw-r--r--   0        0        0      711 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/filesystem/__init__.py
--rw-r--r--   0        0        0     1546 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/filesystem/create.py
--rw-r--r--   0        0        0      660 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/filesystem/destroy.py
--rw-r--r--   0        0        0     1524 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/filesystem/list.py
--rw-r--r--   0        0        0      412 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/filesystem/type.py
--rw-r--r--   0        0        0      952 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/list.py
--rw-r--r--   0        0        0      273 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/optional.py
--rw-r--r--   0        0        0      330 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/snapshot/__init__.py
--rw-r--r--   0        0        0      692 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/snapshot/destroy.py
--rw-r--r--   0        0        0     2369 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/snapshot/list.py
--rw-r--r--   0        0        0     2094 2023-06-13 20:07:47.182983 zfs_replicate-2.1.1/zfs/replicate/snapshot/send.py
--rw-r--r--   0        0        0      799 2023-06-13 20:07:47.186983 zfs_replicate-2.1.1/zfs/replicate/snapshot/type.py
--rw-r--r--   0        0        0      183 2023-06-13 20:07:47.186983 zfs_replicate-2.1.1/zfs/replicate/ssh/__init__.py
--rw-r--r--   0        0        0      158 2023-06-13 20:07:47.186983 zfs_replicate-2.1.1/zfs/replicate/ssh/cipher.py
--rw-r--r--   0        0        0      815 2023-06-13 20:07:47.186983 zfs_replicate-2.1.1/zfs/replicate/ssh/command.py
--rw-r--r--   0        0        0      598 2023-06-13 20:07:47.186983 zfs_replicate-2.1.1/zfs/replicate/subprocess.py
--rw-r--r--   0        0        0      256 2023-06-13 20:07:47.186983 zfs_replicate-2.1.1/zfs/replicate/task/__init__.py
--rw-r--r--   0        0        0     2160 2023-06-13 20:07:47.186983 zfs_replicate-2.1.1/zfs/replicate/task/execute.py
--rw-r--r--   0        0        0     3220 2023-06-13 20:07:47.186983 zfs_replicate-2.1.1/zfs/replicate/task/generate.py
--rw-r--r--   0        0        0     2560 2023-06-13 20:07:47.186983 zfs_replicate-2.1.1/zfs/replicate/task/report.py
--rw-r--r--   0        0        0      413 2023-06-13 20:07:47.186983 zfs_replicate-2.1.1/zfs/replicate/task/type.py
--rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 zfs_replicate-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1290 2023-06-17 10:54:24.635549 zfs_replicate-2.2.0/LICENSE
+-rw-r--r--   0        0        0     3385 2023-06-17 10:54:24.635549 zfs_replicate-2.2.0/README.md
+-rw-r--r--   0        0        0     1640 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/__init__.pyi
+-rw-r--r--   0        0        0       33 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/__init__.py
+-rw-r--r--   0        0        0       35 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/cli/__init__.py
+-rw-r--r--   0        0        0      912 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/cli/click.py
+-rw-r--r--   0        0        0     4164 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/cli/main.py
+-rw-r--r--   0        0        0      203 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/compress/__init__.py
+-rw-r--r--   0        0        0      484 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/compress/command.py
+-rw-r--r--   0        0        0      170 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/compress/type.py
+-rw-r--r--   0        0        0      327 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/error.py
+-rw-r--r--   0        0        0      711 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/filesystem/__init__.py
+-rw-r--r--   0        0        0     1546 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/filesystem/create.py
+-rw-r--r--   0        0        0      660 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/filesystem/destroy.py
+-rw-r--r--   0        0        0     1524 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/filesystem/list.py
+-rw-r--r--   0        0        0      412 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/filesystem/type.py
+-rw-r--r--   0        0        0      952 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/list.py
+-rw-r--r--   0        0        0      273 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/optional.py
+-rw-r--r--   0        0        0      330 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/snapshot/__init__.py
+-rw-r--r--   0        0        0      692 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/snapshot/destroy.py
+-rw-r--r--   0        0        0     2369 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/snapshot/list.py
+-rw-r--r--   0        0        0     2094 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/snapshot/send.py
+-rw-r--r--   0        0        0      799 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/snapshot/type.py
+-rw-r--r--   0        0        0      183 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/ssh/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/ssh/cipher.py
+-rw-r--r--   0        0        0      815 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/ssh/command.py
+-rw-r--r--   0        0        0      598 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/subprocess.py
+-rw-r--r--   0        0        0      256 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/task/__init__.py
+-rw-r--r--   0        0        0     2160 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/task/execute.py
+-rw-r--r--   0        0        0     3220 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/task/generate.py
+-rw-r--r--   0        0        0     2560 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/task/report.py
+-rw-r--r--   0        0        0      413 2023-06-17 10:54:24.639549 zfs_replicate-2.2.0/zfs/replicate/task/type.py
+-rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 zfs_replicate-2.2.0/PKG-INFO
```

### Comparing `zfs_replicate-2.1.1/LICENSE` & `zfs_replicate-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/README.md` & `zfs_replicate-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/pyproject.toml` & `zfs_replicate-2.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 license = "BSD-2-Clause"
 name = "zfs-replicate"
 packages = [
   {include = "zfs"}
 ]
 readme = "README.md"
 repository = "https://github.com/alunduil/zfs-replicate"
-version = "2.1.1"
+version = "2.2.0"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 python = "^3.7.2"
 stringcase = "^1.2.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `zfs_replicate-2.1.1/zfs/replicate/cli/click.py` & `zfs_replicate-2.2.0/zfs/replicate/cli/click.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/cli/main.py` & `zfs_replicate-2.2.0/zfs/replicate/cli/main.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/filesystem/__init__.py` & `zfs_replicate-2.2.0/zfs/replicate/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/filesystem/create.py` & `zfs_replicate-2.2.0/zfs/replicate/filesystem/create.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/filesystem/destroy.py` & `zfs_replicate-2.2.0/zfs/replicate/filesystem/destroy.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/filesystem/list.py` & `zfs_replicate-2.2.0/zfs/replicate/filesystem/list.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/list.py` & `zfs_replicate-2.2.0/zfs/replicate/list.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/snapshot/destroy.py` & `zfs_replicate-2.2.0/zfs/replicate/snapshot/destroy.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/snapshot/list.py` & `zfs_replicate-2.2.0/zfs/replicate/snapshot/list.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/snapshot/send.py` & `zfs_replicate-2.2.0/zfs/replicate/snapshot/send.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/snapshot/type.py` & `zfs_replicate-2.2.0/zfs/replicate/snapshot/type.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/ssh/command.py` & `zfs_replicate-2.2.0/zfs/replicate/ssh/command.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/subprocess.py` & `zfs_replicate-2.2.0/zfs/replicate/subprocess.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/task/execute.py` & `zfs_replicate-2.2.0/zfs/replicate/task/execute.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/task/generate.py` & `zfs_replicate-2.2.0/zfs/replicate/task/generate.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/zfs/replicate/task/report.py` & `zfs_replicate-2.2.0/zfs/replicate/task/report.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-2.1.1/PKG-INFO` & `zfs_replicate-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zfs-replicate
-Version: 2.1.1
+Version: 2.2.0
 Summary: ZFS Snapshot Replicator
 Home-page: https://github.com/alunduil/zfs-replicate
 License: BSD-2-Clause
 Keywords: zfs,replication,backup,remote
 Author: Alex Brandt
 Author-email: alunduil@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
```

