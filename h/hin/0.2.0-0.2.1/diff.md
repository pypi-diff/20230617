# Comparing `tmp/hin-0.2.0.tar.gz` & `tmp/hin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hin-0.2.0.tar", max compression
+gzip compressed data, was "hin-0.2.1.tar", max compression
```

## Comparing `hin-0.2.0.tar` & `hin-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1073 2023-06-17 03:57:03.677212 hin-0.2.0/LICENSE
--rw-r--r--   0        0        0     2960 2023-06-17 03:57:03.864803 hin-0.2.0/README.rst
--rw-r--r--   0        0        0      123 2023-06-17 03:57:03.871219 hin-0.2.0/hin/__init__.py
--rw-r--r--   0        0        0      146 2023-06-17 03:57:03.871315 hin-0.2.0/hin/__main__.py
--rw-r--r--   0        0        0     3398 2023-06-17 03:57:03.871394 hin-0.2.0/hin/_actions.py
--rw-r--r--   0        0        0     3591 2023-06-17 06:51:43.454460 hin-0.2.0/hin/_add.py
--rw-r--r--   0        0        0      763 2023-06-17 03:57:03.871556 hin-0.2.0/hin/_clone.py
--rw-r--r--   0        0        0     1305 2023-06-17 03:57:03.871667 hin-0.2.0/hin/_commit.py
--rw-r--r--   0        0        0     2077 2023-06-17 07:07:46.755998 hin-0.2.0/hin/_config.py
--rw-r--r--   0        0        0     7741 2023-06-17 07:06:42.033989 hin-0.2.0/hin/_decorators.py
--rw-r--r--   0        0        0     5602 2023-06-17 08:36:51.724316 hin-0.2.0/hin/_file.py
--rw-r--r--   0        0        0     1647 2023-06-17 03:57:03.872023 hin-0.2.0/hin/_gitignore.py
--rw-r--r--   0        0        0     1913 2023-06-17 03:57:03.872093 hin-0.2.0/hin/_link.py
--rw-r--r--   0        0        0      673 2023-06-17 03:57:03.872153 hin-0.2.0/hin/_list.py
--rw-r--r--   0        0        0     5357 2023-06-17 03:57:03.872238 hin-0.2.0/hin/_main.py
--rw-r--r--   0        0        0     1129 2023-06-17 08:57:48.466032 hin-0.2.0/hin/_push.py
--rw-r--r--   0        0        0     1160 2023-06-17 03:57:03.872399 hin-0.2.0/hin/_remove.py
--rw-r--r--   0        0        0     2524 2023-06-17 06:53:40.877969 hin-0.2.0/hin/_status.py
--rw-r--r--   0        0        0     1265 2023-06-17 03:57:03.872581 hin-0.2.0/hin/_undo.py
--rw-r--r--   0        0        0      204 2023-06-17 08:38:55.452865 hin-0.2.0/hin/_version.py
--rw-r--r--   0        0        0        0 2023-06-17 03:57:03.872710 hin-0.2.0/hin/py.typed
--rw-r--r--   0        0        0     2231 2023-06-17 08:38:55.453451 hin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 hin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-17 10:41:25.428222 hin-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2960 2023-06-17 10:41:25.428380 hin-0.2.1/README.rst
+-rw-r--r--   0        0        0      123 2023-06-17 10:41:25.428911 hin-0.2.1/hin/__init__.py
+-rw-r--r--   0        0        0      146 2023-06-17 10:41:29.391036 hin-0.2.1/hin/__main__.py
+-rw-r--r--   0        0        0     3398 2023-06-17 10:41:29.391149 hin-0.2.1/hin/_actions.py
+-rw-r--r--   0        0        0     3591 2023-06-17 10:41:34.551029 hin-0.2.1/hin/_add.py
+-rw-r--r--   0        0        0      763 2023-06-17 10:41:29.391354 hin-0.2.1/hin/_clone.py
+-rw-r--r--   0        0        0     1305 2023-06-17 10:41:33.826978 hin-0.2.1/hin/_commit.py
+-rw-r--r--   0        0        0     2077 2023-06-17 10:41:29.391549 hin-0.2.1/hin/_config.py
+-rw-r--r--   0        0        0     7741 2023-06-17 10:41:29.391662 hin-0.2.1/hin/_decorators.py
+-rw-r--r--   0        0        0     5602 2023-06-17 10:41:34.733957 hin-0.2.1/hin/_file.py
+-rw-r--r--   0        0        0     1647 2023-06-17 10:41:29.391856 hin-0.2.1/hin/_gitignore.py
+-rw-r--r--   0        0        0     1913 2023-06-17 10:41:29.391949 hin-0.2.1/hin/_link.py
+-rw-r--r--   0        0        0      673 2023-06-17 10:41:29.392046 hin-0.2.1/hin/_list.py
+-rw-r--r--   0        0        0     5357 2023-06-17 10:41:29.392189 hin-0.2.1/hin/_main.py
+-rw-r--r--   0        0        0     2016 2023-06-17 10:41:35.470188 hin-0.2.1/hin/_push.py
+-rw-r--r--   0        0        0     1160 2023-06-17 10:41:31.973772 hin-0.2.1/hin/_remove.py
+-rw-r--r--   0        0        0     2524 2023-06-17 10:41:33.258176 hin-0.2.1/hin/_status.py
+-rw-r--r--   0        0        0     1265 2023-06-17 10:41:29.392606 hin-0.2.1/hin/_undo.py
+-rw-r--r--   0        0        0      204 2023-06-17 10:41:35.656208 hin-0.2.1/hin/_version.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:41:25.430368 hin-0.2.1/hin/py.typed
+-rw-r--r--   0        0        0     2231 2023-06-17 10:41:35.657155 hin-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 hin-0.2.1/PKG-INFO
```

### Comparing `hin-0.2.0/LICENSE` & `hin-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/README.rst` & `hin-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_actions.py` & `hin-0.2.1/hin/_actions.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_add.py` & `hin-0.2.1/hin/_add.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_clone.py` & `hin-0.2.1/hin/_clone.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_commit.py` & `hin-0.2.1/hin/_commit.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_config.py` & `hin-0.2.1/hin/_config.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_decorators.py` & `hin-0.2.1/hin/_decorators.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_file.py` & `hin-0.2.1/hin/_file.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_gitignore.py` & `hin-0.2.1/hin/_gitignore.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_link.py` & `hin-0.2.1/hin/_link.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_list.py` & `hin-0.2.1/hin/_list.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_main.py` & `hin-0.2.1/hin/_main.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_push.py` & `hin-0.2.1/hin/_push.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,24 +20,48 @@
     \f
 
     :param out: Console object.
     :param remote: Remote URL.
     :param repo: Git repository type.
     """
     if remote is not None:
-        try:
-            repo.git.remote("remove", _ORIGIN)
-        except _git.GitCommandError:
-            pass
+        # only add if no remote has been added yet
+        # if you re-add the remote you get the following:
+        #
+        #     $ git status
+        #     On branch master
+        #     nothing to commit, working tree clean
+        #
+        # instead of:
+        #
+        #     $ git status
+        #     On branch master
+        #     Your branch is up to date with 'origin/master'
+        #
+        #     nothing to commit, working tree clean
+        #
+        # "Your branch is up to date with" is the unambiguous string to
+        # look for to confirm that there is nothing to push
+        if not (
+            repo.git.remote() == _ORIGIN
+            and repo.git.remote("get-url", _ORIGIN) == remote
+        ):
+            try:
+                repo.git.remote("remove", _ORIGIN)
+            except _git.GitCommandError:
+                pass
 
-        repo.git.remote("add", _ORIGIN, remote)
+            repo.git.remote("add", _ORIGIN, remote)
 
     try:
-        repo.git.push(_ORIGIN, "master", set_upstream=True)
-        out.print("[green bold]changes pushed to remote[/green bold]")
+        if "Your branch is up to date with" in repo.git.status():
+            out.print("no changes to push to remote")
+        else:
+            repo.git.push(_ORIGIN, "master", set_upstream=True)
+            out.print("[green bold]changes pushed to remote[/green bold]")
     except _git.GitCommandError as err:
         if "'origin' does not appear to be a git repository" in str(err):
             raise RuntimeError(
                 "'origin' does not appear to be a git repository\n"
                 "try running `hin push --remote=<REMOTE>` to set origin"
                 " upstream"
             ) from err
```

### Comparing `hin-0.2.0/hin/_remove.py` & `hin-0.2.1/hin/_remove.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_status.py` & `hin-0.2.1/hin/_status.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/hin/_undo.py` & `hin-0.2.1/hin/_undo.py`

 * *Files identical despite different names*

### Comparing `hin-0.2.0/pyproject.toml` & `hin-0.2.1/pyproject.toml`

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
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.poetry.dependencies]
 appdirs = "^1.4.4"
 click = "^8.1.3"
 click-help-colors = "^0.9.1"
 configobj = "^5.0.8"
 gitpython = "^3.1.31"
```

### Comparing `hin-0.2.0/PKG-INFO` & `hin-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hin
-Version: 0.2.0
+Version: 0.2.1
 Summary: Dotfile manager
 Home-page: https://pypi.org/project/hin/
 License: MIT
 Keywords: config,dot,dotfile,file,hin
 Author: jshwi
 Author-email: stephen@jshwisolutions.com
 Maintainer: jshwi
```

