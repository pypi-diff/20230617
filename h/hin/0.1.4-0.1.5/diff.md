# Comparing `tmp/hin-0.1.4.tar.gz` & `tmp/hin-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hin-0.1.4.tar", max compression
+gzip compressed data, was "hin-0.1.5.tar", max compression
```

## Comparing `hin-0.1.4.tar` & `hin-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1073 2023-06-17 01:37:09.329976 hin-0.1.4/LICENSE
--rw-r--r--   0        0        0     2960 2023-06-17 01:37:09.330162 hin-0.1.4/README.rst
--rw-r--r--   0        0        0      123 2023-06-17 01:37:09.330737 hin-0.1.4/hin/__init__.py
--rw-r--r--   0        0        0      146 2023-06-17 01:37:12.105716 hin-0.1.4/hin/__main__.py
--rw-r--r--   0        0        0     3398 2023-06-17 01:37:12.105828 hin-0.1.4/hin/_actions.py
--rw-r--r--   0        0        0     3535 2023-06-17 01:37:12.105931 hin-0.1.4/hin/_add.py
--rw-r--r--   0        0        0      763 2023-06-17 01:37:12.106030 hin-0.1.4/hin/_clone.py
--rw-r--r--   0        0        0     1321 2023-06-17 01:37:12.106123 hin-0.1.4/hin/_commit.py
--rw-r--r--   0        0        0     2077 2023-06-17 01:37:12.106239 hin-0.1.4/hin/_config.py
--rw-r--r--   0        0        0     7741 2023-06-17 01:37:12.106369 hin-0.1.4/hin/_decorators.py
--rw-r--r--   0        0        0     5598 2023-06-17 01:37:15.940368 hin-0.1.4/hin/_file.py
--rw-r--r--   0        0        0     1647 2023-06-17 01:37:12.106576 hin-0.1.4/hin/_gitignore.py
--rw-r--r--   0        0        0     1913 2023-06-17 01:37:12.106699 hin-0.1.4/hin/_link.py
--rw-r--r--   0        0        0      673 2023-06-17 01:37:12.106809 hin-0.1.4/hin/_list.py
--rw-r--r--   0        0        0     5357 2023-06-17 01:37:12.106930 hin-0.1.4/hin/_main.py
--rw-r--r--   0        0        0     1129 2023-06-17 01:37:12.107036 hin-0.1.4/hin/_push.py
--rw-r--r--   0        0        0     1160 2023-06-17 01:37:14.660330 hin-0.1.4/hin/_remove.py
--rw-r--r--   0        0        0     2524 2023-06-17 01:37:15.940767 hin-0.1.4/hin/_status.py
--rw-r--r--   0        0        0     1265 2023-06-17 01:37:12.107317 hin-0.1.4/hin/_undo.py
--rw-r--r--   0        0        0      204 2023-06-17 01:37:29.728183 hin-0.1.4/hin/_version.py
--rw-r--r--   0        0        0        0 2023-06-17 01:37:09.332033 hin-0.1.4/hin/py.typed
--rw-r--r--   0        0        0     2231 2023-06-17 01:37:29.729221 hin-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 hin-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-17 03:20:22.685361 hin-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2960 2023-06-17 03:20:22.685512 hin-0.1.5/README.rst
+-rw-r--r--   0        0        0      123 2023-06-17 03:20:22.686035 hin-0.1.5/hin/__init__.py
+-rw-r--r--   0        0        0      146 2023-06-17 03:20:28.162166 hin-0.1.5/hin/__main__.py
+-rw-r--r--   0        0        0     3398 2023-06-17 03:20:28.162279 hin-0.1.5/hin/_actions.py
+-rw-r--r--   0        0        0     3535 2023-06-17 03:20:28.162381 hin-0.1.5/hin/_add.py
+-rw-r--r--   0        0        0      763 2023-06-17 03:20:28.162472 hin-0.1.5/hin/_clone.py
+-rw-r--r--   0        0        0     1305 2023-06-17 03:20:32.538373 hin-0.1.5/hin/_commit.py
+-rw-r--r--   0        0        0     2077 2023-06-17 03:20:28.162672 hin-0.1.5/hin/_config.py
+-rw-r--r--   0        0        0     7741 2023-06-17 03:20:28.162789 hin-0.1.5/hin/_decorators.py
+-rw-r--r--   0        0        0     5598 2023-06-17 03:20:31.993245 hin-0.1.5/hin/_file.py
+-rw-r--r--   0        0        0     1647 2023-06-17 03:20:28.162987 hin-0.1.5/hin/_gitignore.py
+-rw-r--r--   0        0        0     1913 2023-06-17 03:20:28.163082 hin-0.1.5/hin/_link.py
+-rw-r--r--   0        0        0      673 2023-06-17 03:20:28.163179 hin-0.1.5/hin/_list.py
+-rw-r--r--   0        0        0     5357 2023-06-17 03:20:28.163290 hin-0.1.5/hin/_main.py
+-rw-r--r--   0        0        0     1129 2023-06-17 03:20:28.163389 hin-0.1.5/hin/_push.py
+-rw-r--r--   0        0        0     1160 2023-06-17 03:20:30.724742 hin-0.1.5/hin/_remove.py
+-rw-r--r--   0        0        0     2524 2023-06-17 03:20:31.993873 hin-0.1.5/hin/_status.py
+-rw-r--r--   0        0        0     1265 2023-06-17 03:20:28.163680 hin-0.1.5/hin/_undo.py
+-rw-r--r--   0        0        0      204 2023-06-17 03:20:32.722981 hin-0.1.5/hin/_version.py
+-rw-r--r--   0        0        0        0 2023-06-17 03:20:22.687372 hin-0.1.5/hin/py.typed
+-rw-r--r--   0        0        0     2231 2023-06-17 03:20:32.724007 hin-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 hin-0.1.5/PKG-INFO
```

### Comparing `hin-0.1.4/LICENSE` & `hin-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/README.rst` & `hin-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_actions.py` & `hin-0.1.5/hin/_actions.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_add.py` & `hin-0.1.5/hin/_add.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_clone.py` & `hin-0.1.5/hin/_clone.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_commit.py` & `hin-0.1.5/hin/_commit.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     """
     try:
         entry = _Entry.new(file)
         for existing in config.values():
             if entry.is_child_of(existing):
                 entry = existing.child(existing)
 
-            repo.git.restore("--source", "stash@{0}", "--", entry.value.path)
-            if repo.git.diff("HEAD", "--", entry.value.path):
-                repo.git.add(entry.value.path)
-                return f"update {entry.value.relpath}"
+        repo.git.restore("--source", "stash@{0}", "--", entry.value.path)
+        if repo.git.diff("HEAD", "--", entry.value.path):
+            repo.git.add(entry.value.path)
+            return f"update {entry.value.relpath}"
 
     except _git.GitCommandError:
         pass
 
     out.print("nothing to commit")
     return None
```

### Comparing `hin-0.1.4/hin/_config.py` & `hin-0.1.5/hin/_config.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_decorators.py` & `hin-0.1.5/hin/_decorators.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_file.py` & `hin-0.1.5/hin/_file.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_gitignore.py` & `hin-0.1.5/hin/_gitignore.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_link.py` & `hin-0.1.5/hin/_link.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_list.py` & `hin-0.1.5/hin/_list.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_main.py` & `hin-0.1.5/hin/_main.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_push.py` & `hin-0.1.5/hin/_push.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_remove.py` & `hin-0.1.5/hin/_remove.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_status.py` & `hin-0.1.5/hin/_status.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/hin/_undo.py` & `hin-0.1.5/hin/_undo.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.4/pyproject.toml` & `hin-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 license = "MIT"
 maintainers = [
   "jshwi <stephen@jshwisolutions.com>"
 ]
 name = "hin"
 readme = "README.rst"
 repository = "https://github.com/jshwi/hin"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 appdirs = "^1.4.4"
 click = "^8.1.3"
 click-help-colors = "^0.9.1"
 configobj = "^5.0.8"
 gitpython = "^3.1.31"
```

### Comparing `hin-0.1.4/PKG-INFO` & `hin-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hin
-Version: 0.1.4
+Version: 0.1.5
 Summary: Dotfile manager
 Home-page: https://pypi.org/project/hin/
 License: MIT
 Keywords: config,dot,dotfile,file,hin
 Author: jshwi
 Author-email: stephen@jshwisolutions.com
 Maintainer: jshwi
```

