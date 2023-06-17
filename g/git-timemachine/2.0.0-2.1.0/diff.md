# Comparing `tmp/git_timemachine-2.0.0.tar.gz` & `tmp/git_timemachine-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_timemachine-2.0.0.tar", max compression
+gzip compressed data, was "git_timemachine-2.1.0.tar", max compression
```

## Comparing `git_timemachine-2.0.0.tar` & `git_timemachine-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rwxr-xr-x   0        0        0      280 2023-06-16 16:24:50.513758 git_timemachine-2.0.0/README.md
--rwxr-xr-x   0        0        0     1042 2023-06-17 09:42:08.737421 git_timemachine-2.0.0/pyproject.toml
--rwxr-xr-x   0        0        0       87 2023-06-16 16:25:38.438695 git_timemachine-2.0.0/src/git_timemachine/__init__.py
--rwxr-xr-x   0        0        0     1723 2023-06-17 09:40:33.004403 git_timemachine-2.0.0/src/git_timemachine/__main__.py
--rwxr-xr-x   0        0        0      336 2023-06-17 09:12:10.537199 git_timemachine-2.0.0/src/git_timemachine/command/__init__.py
--rwxr-xr-x   0        0        0     3897 2023-06-17 08:51:15.374491 git_timemachine-2.0.0/src/git_timemachine/command/commit.py
--rwxr-xr-x   0        0        0      894 2023-06-17 08:13:19.376189 git_timemachine-2.0.0/src/git_timemachine/command/config.py
--rwxr-xr-x   0        0        0     1215 2023-06-16 17:46:11.169634 git_timemachine-2.0.0/src/git_timemachine/command/log.py
--rwxr-xr-x   0        0        0     2593 2023-06-17 06:31:17.237148 git_timemachine-2.0.0/src/git_timemachine/command/migrate.py
--rwxr-xr-x   0        0        0      682 2023-06-17 09:18:16.347728 git_timemachine-2.0.0/src/git_timemachine/command/session.py
--rwxr-xr-x   0        0        0      661 2023-06-17 06:06:10.094026 git_timemachine-2.0.0/src/git_timemachine/command/switch_date.py
--rwxr-xr-x   0        0        0     1026 2023-06-17 06:27:50.485505 git_timemachine-2.0.0/src/git_timemachine/git.py
--rwxr-xr-x   0        0        0      423 2023-06-17 09:39:44.699950 git_timemachine-2.0.0/src/git_timemachine/session.py
--rwxr-xr-x   0        0        0     1209 2023-06-17 08:19:16.406434 git_timemachine-2.0.0/src/git_timemachine/utils.py
--rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 git_timemachine-2.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0      280 2023-06-16 16:24:50.513758 git_timemachine-2.1.0/README.md
+-rwxr-xr-x   0        0        0     1042 2023-06-17 09:55:06.054017 git_timemachine-2.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0       87 2023-06-16 16:25:38.438695 git_timemachine-2.1.0/src/git_timemachine/__init__.py
+-rwxr-xr-x   0        0        0     1723 2023-06-17 09:40:33.004403 git_timemachine-2.1.0/src/git_timemachine/__main__.py
+-rwxr-xr-x   0        0        0      387 2023-06-17 09:53:52.453256 git_timemachine-2.1.0/src/git_timemachine/command/__init__.py
+-rwxr-xr-x   0        0        0     3897 2023-06-17 08:51:15.374491 git_timemachine-2.1.0/src/git_timemachine/command/commit.py
+-rwxr-xr-x   0        0        0      894 2023-06-17 08:13:19.376189 git_timemachine-2.1.0/src/git_timemachine/command/config.py
+-rwxr-xr-x   0        0        0     1215 2023-06-16 17:46:11.169634 git_timemachine-2.1.0/src/git_timemachine/command/log.py
+-rwxr-xr-x   0        0        0     2593 2023-06-17 06:31:17.237148 git_timemachine-2.1.0/src/git_timemachine/command/migrate.py
+-rwxr-xr-x   0        0        0      857 2023-06-17 09:54:34.902269 git_timemachine-2.1.0/src/git_timemachine/command/review.py
+-rwxr-xr-x   0        0        0      682 2023-06-17 09:18:16.347728 git_timemachine-2.1.0/src/git_timemachine/command/session.py
+-rwxr-xr-x   0        0        0      661 2023-06-17 06:06:10.094026 git_timemachine-2.1.0/src/git_timemachine/command/switch_date.py
+-rwxr-xr-x   0        0        0     1026 2023-06-17 06:27:50.485505 git_timemachine-2.1.0/src/git_timemachine/git.py
+-rwxr-xr-x   0        0        0      423 2023-06-17 09:39:44.699950 git_timemachine-2.1.0/src/git_timemachine/session.py
+-rwxr-xr-x   0        0        0     1209 2023-06-17 08:19:16.406434 git_timemachine-2.1.0/src/git_timemachine/utils.py
+-rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 git_timemachine-2.1.0/PKG-INFO
```

### Comparing `git_timemachine-2.0.0/pyproject.toml` & `git_timemachine-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-timemachine"
-version = "2.0.0"
+version = "2.1.0"
 description = "A command-line tool that helps you record commits on Git repositories at any time node."
 authors = ["HE Yaowen <he.yaowen@hotmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/he-yaowen/git-timemachine"
 packages = [{include = "git_timemachine", from = "src"}]
```

### Comparing `git_timemachine-2.0.0/src/git_timemachine/__main__.py` & `git_timemachine-2.1.0/src/git_timemachine/__main__.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-2.0.0/src/git_timemachine/command/commit.py` & `git_timemachine-2.1.0/src/git_timemachine/command/commit.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-2.0.0/src/git_timemachine/command/config.py` & `git_timemachine-2.1.0/src/git_timemachine/command/config.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-2.0.0/src/git_timemachine/command/log.py` & `git_timemachine-2.1.0/src/git_timemachine/command/log.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-2.0.0/src/git_timemachine/command/migrate.py` & `git_timemachine-2.1.0/src/git_timemachine/command/migrate.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-2.0.0/src/git_timemachine/command/session.py` & `git_timemachine-2.1.0/src/git_timemachine/command/session.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-2.0.0/src/git_timemachine/command/switch_date.py` & `git_timemachine-2.1.0/src/git_timemachine/command/switch_date.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-2.0.0/src/git_timemachine/git.py` & `git_timemachine-2.1.0/src/git_timemachine/git.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-2.0.0/src/git_timemachine/utils.py` & `git_timemachine-2.1.0/src/git_timemachine/utils.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-2.0.0/PKG-INFO` & `git_timemachine-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-timemachine
-Version: 2.0.0
+Version: 2.1.0
 Summary: A command-line tool that helps you record commits on Git repositories at any time node.
 Home-page: https://github.com/he-yaowen/git-timemachine
 License: GPL-3.0
 Author: HE Yaowen
 Author-email: he.yaowen@hotmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

