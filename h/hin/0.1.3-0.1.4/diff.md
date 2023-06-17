# Comparing `tmp/hin-0.1.3.tar.gz` & `tmp/hin-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hin-0.1.3.tar", max compression
+gzip compressed data, was "hin-0.1.4.tar", max compression
```

## Comparing `hin-0.1.3.tar` & `hin-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1073 2023-06-16 09:11:05.379377 hin-0.1.3/LICENSE
--rw-r--r--   0        0        0     2960 2023-06-16 09:11:05.379527 hin-0.1.3/README.rst
--rw-r--r--   0        0        0      123 2023-06-16 09:11:05.379992 hin-0.1.3/hin/__init__.py
--rw-r--r--   0        0        0      146 2023-06-16 09:11:07.768110 hin-0.1.3/hin/__main__.py
--rw-r--r--   0        0        0     3398 2023-06-16 09:11:07.768217 hin-0.1.3/hin/_actions.py
--rw-r--r--   0        0        0     3535 2023-06-16 09:11:07.768329 hin-0.1.3/hin/_add.py
--rw-r--r--   0        0        0      763 2023-06-16 09:11:07.768427 hin-0.1.3/hin/_clone.py
--rw-r--r--   0        0        0     1321 2023-06-16 09:11:07.768518 hin-0.1.3/hin/_commit.py
--rw-r--r--   0        0        0     2077 2023-06-16 09:11:07.768622 hin-0.1.3/hin/_config.py
--rw-r--r--   0        0        0     7741 2023-06-16 09:11:07.768747 hin-0.1.3/hin/_decorators.py
--rw-r--r--   0        0        0     5854 2023-06-16 09:11:10.863789 hin-0.1.3/hin/_file.py
--rw-r--r--   0        0        0     1647 2023-06-16 09:11:07.768948 hin-0.1.3/hin/_gitignore.py
--rw-r--r--   0        0        0     1913 2023-06-16 09:11:07.769042 hin-0.1.3/hin/_link.py
--rw-r--r--   0        0        0      673 2023-06-16 09:11:07.769199 hin-0.1.3/hin/_list.py
--rw-r--r--   0        0        0     5357 2023-06-16 09:11:07.769318 hin-0.1.3/hin/_main.py
--rw-r--r--   0        0        0     1129 2023-06-16 09:11:07.769423 hin-0.1.3/hin/_push.py
--rw-r--r--   0        0        0     1160 2023-06-16 09:11:10.307656 hin-0.1.3/hin/_remove.py
--rw-r--r--   0        0        0     2496 2023-06-16 09:11:09.393260 hin-0.1.3/hin/_status.py
--rw-r--r--   0        0        0     1265 2023-06-16 09:11:07.769752 hin-0.1.3/hin/_undo.py
--rw-r--r--   0        0        0      204 2023-06-16 09:11:11.050889 hin-0.1.3/hin/_version.py
--rw-r--r--   0        0        0        0 2023-06-16 09:11:05.381342 hin-0.1.3/hin/py.typed
--rw-r--r--   0        0        0     2231 2023-06-16 09:11:11.051715 hin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 hin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-17 01:37:09.329976 hin-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2960 2023-06-17 01:37:09.330162 hin-0.1.4/README.rst
+-rw-r--r--   0        0        0      123 2023-06-17 01:37:09.330737 hin-0.1.4/hin/__init__.py
+-rw-r--r--   0        0        0      146 2023-06-17 01:37:12.105716 hin-0.1.4/hin/__main__.py
+-rw-r--r--   0        0        0     3398 2023-06-17 01:37:12.105828 hin-0.1.4/hin/_actions.py
+-rw-r--r--   0        0        0     3535 2023-06-17 01:37:12.105931 hin-0.1.4/hin/_add.py
+-rw-r--r--   0        0        0      763 2023-06-17 01:37:12.106030 hin-0.1.4/hin/_clone.py
+-rw-r--r--   0        0        0     1321 2023-06-17 01:37:12.106123 hin-0.1.4/hin/_commit.py
+-rw-r--r--   0        0        0     2077 2023-06-17 01:37:12.106239 hin-0.1.4/hin/_config.py
+-rw-r--r--   0        0        0     7741 2023-06-17 01:37:12.106369 hin-0.1.4/hin/_decorators.py
+-rw-r--r--   0        0        0     5598 2023-06-17 01:37:15.940368 hin-0.1.4/hin/_file.py
+-rw-r--r--   0        0        0     1647 2023-06-17 01:37:12.106576 hin-0.1.4/hin/_gitignore.py
+-rw-r--r--   0        0        0     1913 2023-06-17 01:37:12.106699 hin-0.1.4/hin/_link.py
+-rw-r--r--   0        0        0      673 2023-06-17 01:37:12.106809 hin-0.1.4/hin/_list.py
+-rw-r--r--   0        0        0     5357 2023-06-17 01:37:12.106930 hin-0.1.4/hin/_main.py
+-rw-r--r--   0        0        0     1129 2023-06-17 01:37:12.107036 hin-0.1.4/hin/_push.py
+-rw-r--r--   0        0        0     1160 2023-06-17 01:37:14.660330 hin-0.1.4/hin/_remove.py
+-rw-r--r--   0        0        0     2524 2023-06-17 01:37:15.940767 hin-0.1.4/hin/_status.py
+-rw-r--r--   0        0        0     1265 2023-06-17 01:37:12.107317 hin-0.1.4/hin/_undo.py
+-rw-r--r--   0        0        0      204 2023-06-17 01:37:29.728183 hin-0.1.4/hin/_version.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:37:09.332033 hin-0.1.4/hin/py.typed
+-rw-r--r--   0        0        0     2231 2023-06-17 01:37:29.729221 hin-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 hin-0.1.4/PKG-INFO
```

### Comparing `hin-0.1.3/LICENSE` & `hin-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/README.rst` & `hin-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_actions.py` & `hin-0.1.4/hin/_actions.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_add.py` & `hin-0.1.4/hin/_add.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_clone.py` & `hin-0.1.4/hin/_clone.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_commit.py` & `hin-0.1.4/hin/_commit.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_config.py` & `hin-0.1.4/hin/_config.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_decorators.py` & `hin-0.1.4/hin/_decorators.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_file.py` & `hin-0.1.4/hin/_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,23 +93,14 @@
         return self._key
 
     @property
     def value(self) -> _File:
         """Path to the actual file or directory."""
         return self._value
 
-    @property
-    def isdotfile(self) -> bool:
-        """Boolean for whether file begins with a dot.
-
-        Some hidden files, such as ~/Library for OSX do not begin with a
-        dot.
-        """
-        return str(self._key.relpath).startswith(".")
-
     def is_child_of(self, other: Matrix) -> bool:
         """Check whether this is a child of a file matrix.
 
         :param other: Matrix to check against.
         :return: Boolean for whether this is the child of a matrix.
         """
         return (str(self.key.path).startswith(str(other.key.path))) or (
```

### Comparing `hin-0.1.3/hin/_gitignore.py` & `hin-0.1.4/hin/_gitignore.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_link.py` & `hin-0.1.4/hin/_link.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_list.py` & `hin-0.1.4/hin/_list.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_main.py` & `hin-0.1.4/hin/_main.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_push.py` & `hin-0.1.4/hin/_push.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_remove.py` & `hin-0.1.4/hin/_remove.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/hin/_status.py` & `hin-0.1.4/hin/_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,29 +26,29 @@
 
     @property
     def kind(self) -> str:
         """Type of change."""
         return self._kind
 
     @property
-    def path(self) -> str:
+    def path(self) -> _Path:
         """Changed path."""
-        return self._path
+        return _Path(self._path)
 
 
 def _print_paths(line: str, config: _Config) -> None:
     if line.startswith("\t"):
         path_ref = _PathRef(_re.sub(" +", " ", line).strip())
         for existing in config.values():
-            if path_ref.path.startswith(str(existing.value.relpath)):
-                path = str(path_ref.path)
-                if existing.isdotfile:
-                    path = f".{path}"
-
-                print(path_ref.kind, path)
+            if str(path_ref.path).startswith(str(existing.value.relpath)):
+                print(
+                    path_ref.kind,
+                    existing.key.relpath
+                    / str(_Path(*path_ref.path.parts[1:])),
+                )
 
 
 def _print_status(out: _Console, output: str, config: _Config) -> None:
     for line in output.splitlines():
         if _re.match(r"((\w+(?: \w+)*):)", line):
             out.print(f"[green bold]{line}[/green bold]")
```

### Comparing `hin-0.1.3/hin/_undo.py` & `hin-0.1.4/hin/_undo.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.3/pyproject.toml` & `hin-0.1.4/pyproject.toml`

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
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 appdirs = "^1.4.4"
 click = "^8.1.3"
 click-help-colors = "^0.9.1"
 configobj = "^5.0.8"
 gitpython = "^3.1.31"
```

### Comparing `hin-0.1.3/PKG-INFO` & `hin-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hin
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dotfile manager
 Home-page: https://pypi.org/project/hin/
 License: MIT
 Keywords: config,dot,dotfile,file,hin
 Author: jshwi
 Author-email: stephen@jshwisolutions.com
 Maintainer: jshwi
```

