# Comparing `tmp/gitz-1.4.1.tar.gz` & `tmp/gitz-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitz-1.4.1.tar", max compression
+gzip compressed data, was "gitz-1.5.0.tar", max compression
```

## Comparing `gitz-1.4.1.tar` & `gitz-1.5.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0     1067 2022-08-16 10:24:05.068671 gitz-1.4.1/LICENSE
--rw-r--r--   0        0        0     5030 2022-11-24 13:59:56.505841 gitz-1.4.1/README.rst
--rwxr-xr-x   0        0        0     3362 2022-08-16 10:24:05.096284 gitz-1.4.1/git-adjust
--rwxr-xr-x   0        0        0      152 2022-08-16 10:24:05.096355 gitz-1.4.1/git-copy
--rwxr-xr-x   0        0        0     2169 2022-08-16 10:24:05.096423 gitz-1.4.1/git-delete
--rwxr-xr-x   0        0        0     3721 2022-08-16 10:24:05.096513 gitz-1.4.1/git-for-each
--rwxr-xr-x   0        0        0     2937 2022-08-16 10:24:05.096590 gitz-1.4.1/git-gitz
--rwxr-xr-x   0        0        0     6641 2022-11-24 13:59:56.510170 gitz-1.4.1/git-go
--rwxr-xr-x   0        0        0     2911 2022-08-16 10:24:05.096758 gitz-1.4.1/git-infer
--rwxr-xr-x   0        0        0     1179 2022-08-16 10:24:05.096830 gitz-1.4.1/git-multi-pick
--rwxr-xr-x   0        0        0     4925 2022-12-02 11:24:16.355909 gitz-1.4.1/git-new
--rwxr-xr-x   0        0        0     2535 2022-08-16 10:24:05.096974 gitz-1.4.1/git-permute
--rwxr-xr-x   0        0        0      161 2022-08-16 10:24:05.097035 gitz-1.4.1/git-rename
--rwxr-xr-x   0        0        0     2105 2022-08-16 10:24:05.097099 gitz-1.4.1/git-rot
--rwxr-xr-x   0        0        0     2167 2022-08-16 10:24:05.097170 gitz-1.4.1/git-save
--rwxr-xr-x   0        0        0     2958 2022-08-16 10:24:05.097240 gitz-1.4.1/git-split
--rwxr-xr-x   0        0        0     1258 2022-08-16 10:24:05.097309 gitz-1.4.1/git-st
--rwxr-xr-x   0        0        0     5260 2022-08-16 10:24:05.097417 gitz-1.4.1/git-stripe
--rwxr-xr-x   0        0        0     3606 2022-08-16 10:24:05.097499 gitz-1.4.1/git-update
--rwxr-xr-x   0        0        0     1643 2022-08-16 10:24:05.097568 gitz-1.4.1/git-when
--rw-r--r--   0        0        0        0 2022-08-16 10:24:05.097626 gitz-1.4.1/gitz/__init__.py
--rw-r--r--   0        0        0      856 2022-11-23 12:51:30.259842 gitz-1.4.1/gitz/config.py
--rw-r--r--   0        0        0       40 2022-08-16 10:24:05.097802 gitz-1.4.1/gitz/git/__init__.py
--rw-r--r--   0        0        0     1759 2022-08-16 10:24:05.097882 gitz-1.4.1/gitz/git/combine.py
--rw-r--r--   0        0        0     2035 2022-08-16 10:24:05.097955 gitz-1.4.1/gitz/git/delete.py
--rw-r--r--   0        0        0     2590 2022-11-23 12:51:30.164905 gitz-1.4.1/gitz/git/functions.py
--rw-r--r--   0        0        0      526 2022-08-16 10:24:05.098089 gitz-1.4.1/gitz/git/guess_origin.py
--rw-r--r--   0        0        0     5808 2022-08-16 10:24:05.098185 gitz-1.4.1/gitz/git/mover.py
--rw-r--r--   0        0        0     1267 2022-08-16 10:24:05.098255 gitz-1.4.1/gitz/git/reference_branch.py
--rw-r--r--   0        0        0     3685 2022-08-16 10:24:05.098333 gitz-1.4.1/gitz/git/repo.py
--rw-r--r--   0        0        0     1281 2022-11-23 13:24:34.806280 gitz-1.4.1/gitz/git/root.py
--rw-r--r--   0        0        0     1576 2022-08-16 10:24:05.098473 gitz-1.4.1/gitz/git/save.py
--rw-r--r--   0        0        0      160 2022-08-16 10:24:05.098571 gitz-1.4.1/gitz/program/__init__.py
--rw-r--r--   0        0        0      959 2022-08-16 10:24:05.098637 gitz-1.4.1/gitz/program/env.py
--rw-r--r--   0        0        0      984 2022-08-16 10:24:05.098704 gitz-1.4.1/gitz/program/log.py
--rw-r--r--   0        0        0      875 2022-08-16 10:24:05.098766 gitz-1.4.1/gitz/program/parser.py
--rw-r--r--   0        0        0     1302 2022-08-16 10:24:05.098842 gitz-1.4.1/gitz/program/print_help.py
--rw-r--r--   0        0        0     2052 2022-08-16 10:24:05.098922 gitz-1.4.1/gitz/program/program.py
--rw-r--r--   0        0        0     1146 2022-08-16 10:24:05.098987 gitz-1.4.1/gitz/program/run_proc.py
--rw-r--r--   0        0        0     1532 2022-08-16 10:24:05.099079 gitz-1.4.1/gitz/program/runner.py
--rw-r--r--   0        0        0     1042 2022-08-16 10:24:05.099156 gitz-1.4.1/gitz/program/summaries.py
--rw-r--r--   0        0        0     1507 2022-12-05 16:58:17.666759 gitz-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     6067 1970-01-01 00:00:00.000000 gitz-1.4.1/setup.py
--rw-r--r--   0        0        0     5563 1970-01-01 00:00:00.000000 gitz-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-08-16 10:24:05.068671 gitz-1.5.0/LICENSE
+-rw-r--r--   0        0        0     5030 2023-02-04 14:05:52.187315 gitz-1.5.0/README.rst
+-rwxr-xr-x   0        0        0     3362 2022-08-16 10:24:05.096284 gitz-1.5.0/git-adjust
+-rwxr-xr-x   0        0        0      152 2022-08-16 10:24:05.096355 gitz-1.5.0/git-copy
+-rwxr-xr-x   0        0        0     2169 2022-08-16 10:24:05.096423 gitz-1.5.0/git-delete
+-rwxr-xr-x   0        0        0     3721 2022-08-16 10:24:05.096513 gitz-1.5.0/git-for-each
+-rwxr-xr-x   0        0        0     2937 2022-08-16 10:24:05.096590 gitz-1.5.0/git-gitz
+-rwxr-xr-x   0        0        0     6657 2023-02-25 17:43:28.412077 gitz-1.5.0/git-go
+-rwxr-xr-x   0        0        0     2911 2022-08-16 10:24:05.096758 gitz-1.5.0/git-infer
+-rwxr-xr-x   0        0        0     1179 2022-08-16 10:24:05.096830 gitz-1.5.0/git-multi-pick
+-rwxr-xr-x   0        0        0     5132 2023-06-17 12:32:09.707879 gitz-1.5.0/git-new
+-rwxr-xr-x   0        0        0     2535 2022-08-16 10:24:05.096974 gitz-1.5.0/git-permute
+-rwxr-xr-x   0        0        0      161 2022-08-16 10:24:05.097035 gitz-1.5.0/git-rename
+-rwxr-xr-x   0        0        0     2105 2022-08-16 10:24:05.097099 gitz-1.5.0/git-rot
+-rwxr-xr-x   0        0        0     2167 2022-08-16 10:24:05.097170 gitz-1.5.0/git-save
+-rwxr-xr-x   0        0        0     2958 2022-08-16 10:24:05.097240 gitz-1.5.0/git-split
+-rwxr-xr-x   0        0        0     1258 2022-08-16 10:24:05.097309 gitz-1.5.0/git-st
+-rwxr-xr-x   0        0        0     5260 2022-08-16 10:24:05.097417 gitz-1.5.0/git-stripe
+-rwxr-xr-x   0        0        0     3676 2023-02-08 17:44:13.003570 gitz-1.5.0/git-update
+-rwxr-xr-x   0        0        0     1643 2022-08-16 10:24:05.097568 gitz-1.5.0/git-when
+-rw-r--r--   0        0        0        0 2022-08-16 10:24:05.097626 gitz-1.5.0/gitz/__init__.py
+-rw-r--r--   0        0        0      834 2023-02-13 16:39:18.863607 gitz-1.5.0/gitz/config.py
+-rw-r--r--   0        0        0       40 2022-08-16 10:24:05.097802 gitz-1.5.0/gitz/git/__init__.py
+-rw-r--r--   0        0        0     1759 2022-08-16 10:24:05.097882 gitz-1.5.0/gitz/git/combine.py
+-rw-r--r--   0        0        0     2035 2022-08-16 10:24:05.097955 gitz-1.5.0/gitz/git/delete.py
+-rw-r--r--   0        0        0     2617 2023-03-22 10:49:48.248659 gitz-1.5.0/gitz/git/functions.py
+-rw-r--r--   0        0        0      526 2022-08-16 10:24:05.098089 gitz-1.5.0/gitz/git/guess_origin.py
+-rw-r--r--   0        0        0     5808 2022-08-16 10:24:05.098185 gitz-1.5.0/gitz/git/mover.py
+-rw-r--r--   0        0        0     1267 2022-08-16 10:24:05.098255 gitz-1.5.0/gitz/git/reference_branch.py
+-rw-r--r--   0        0        0     3685 2022-08-16 10:24:05.098333 gitz-1.5.0/gitz/git/repo.py
+-rw-r--r--   0        0        0     1281 2023-01-31 16:56:44.017958 gitz-1.5.0/gitz/git/root.py
+-rw-r--r--   0        0        0     1576 2022-08-16 10:24:05.098473 gitz-1.5.0/gitz/git/save.py
+-rw-r--r--   0        0        0      160 2022-08-16 10:24:05.098571 gitz-1.5.0/gitz/program/__init__.py
+-rw-r--r--   0        0        0      968 2023-02-08 17:43:12.978890 gitz-1.5.0/gitz/program/env.py
+-rw-r--r--   0        0        0      984 2022-08-16 10:24:05.098704 gitz-1.5.0/gitz/program/log.py
+-rw-r--r--   0        0        0      875 2022-08-16 10:24:05.098766 gitz-1.5.0/gitz/program/parser.py
+-rw-r--r--   0        0        0     1302 2022-08-16 10:24:05.098842 gitz-1.5.0/gitz/program/print_help.py
+-rw-r--r--   0        0        0     2052 2022-08-16 10:24:05.098922 gitz-1.5.0/gitz/program/program.py
+-rw-r--r--   0        0        0     1146 2022-08-16 10:24:05.098987 gitz-1.5.0/gitz/program/run_proc.py
+-rw-r--r--   0        0        0     1532 2022-08-16 10:24:05.099079 gitz-1.5.0/gitz/program/runner.py
+-rw-r--r--   0        0        0     1042 2022-08-16 10:24:05.099156 gitz-1.5.0/gitz/program/summaries.py
+-rw-r--r--   0        0        0     1500 2023-06-17 12:38:01.823648 gitz-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 gitz-1.5.0/PKG-INFO
```

### Comparing `gitz-1.4.1/LICENSE` & `gitz-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/README.rst` & `gitz-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-adjust` & `gitz-1.5.0/git-adjust`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-delete` & `gitz-1.5.0/git-delete`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-for-each` & `gitz-1.5.0/git-for-each`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-gitz` & `gitz-1.5.0/git-gitz`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-go` & `gitz-1.5.0/git-go`

 * *Files 2% similar despite different names*

```diff
@@ -222,16 +222,16 @@
     if not origin:
         return
 
     prefix = next(p for p in ('git@', 'https://') if origin.startswith(p))
     origin = origin[len(prefix) :]
     host, user, project_git = origin.replace(':', '/').split('/')
     host_name, *_ = host.split('.')
-    project, g = project_git.split('.')
-    assert g == 'git'
+    project, g = project_git.rsplit('.', maxsplit=1)
+    assert g == 'git', g
 
     return host, host_name, user, project
 
 
 def add_arguments(parser):
     parser.add_argument('cmd', nargs='?', default='commits', help=_HELP_CMD)
     parser.add_argument('files', nargs='*', default=(), help=_HELP_FILE)
```

### Comparing `gitz-1.4.1/git-infer` & `gitz-1.5.0/git-infer`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-multi-pick` & `gitz-1.5.0/git-multi-pick`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-new` & `gitz-1.5.0/git-new`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,26 @@
 
     if ARGS.duplicate:
         if ARGS.reference_branch:
             PROGRAM.exit('Cannot set --duplicate and --reference-branch')
         if len(ARGS.branches) > 1:
             PROGRAM.exit('Cannot --duplicate multiple branches')
         ARGS.reference_branch = ARGS.branches[0]
-        _, _, ARGS.branches[0] = ARGS.reference_branch.partition('/')
-        if not ARGS.branches[0]:
-            _, _, ARGS.branches[0] = ARGS.reference_branch.partition(':')
+
+        remote, _, rest = ARGS.reference_branch.partition(':')
+        if rest:
+            ARGS.branches[0] = rest
+            ARGS.reference_branch = f'{remote}/{rest}'
+
+        else:
+            _, _, ARGS.branches[0] = ARGS.reference_branch.partition('/')
             if not ARGS.branches[0]:
-                PROGRAM.exit('--duplicate requires a branch with a slash')
+                _, _, ARGS.branches[0] = ARGS.reference_branch.partition(':')
+                if not ARGS.branches[0]:
+                    PROGRAM.exit('--duplicate requires a branch with a slash')
 
     branches = functions.branches()
     remote_branches = functions.remote_branches()
     origin = guess_origin.guess_origin(ARGS.origin)
     origin_branches = remote_branches[origin]
     overwrites = (set(branches) | set(origin)) & set(ARGS.branches)
     if overwrites:
```

### Comparing `gitz-1.4.1/git-permute` & `gitz-1.5.0/git-permute`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-rot` & `gitz-1.5.0/git-rot`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-save` & `gitz-1.5.0/git-save`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-split` & `gitz-1.5.0/git-split`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-st` & `gitz-1.5.0/git-st`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-stripe` & `gitz-1.5.0/git-stripe`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/git-update` & `gitz-1.5.0/git-update`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,22 @@
         protected_branches = ENV.protected_branches()
         protected = set(ARGS.branches).intersection(protected_branches)
         if PROGRAM.error_if(protected, 'Protected'):
             PROGRAM.exit()
 
         branches = [b for b in branches if b not in protected_branches]
 
-        if not branches:
-            PROGRAM.message('No branches to update')
-            return
+    try:
+        branches.remove('gh-pages')
+    except ValueError:
+        pass
+
+    if not branches:
+        PROGRAM.message('No branches to update')
+        return
 
     starting_branch = functions.branch_name()
     failed = []
 
     ref_branch = reference_branch.reference_branch()
     fetched = set()
```

### Comparing `gitz-1.4.1/git-when` & `gitz-1.5.0/git-when`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/config.py` & `gitz-1.5.0/gitz/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pathlib import Path
 import sys
 
-__version__ = '1.3.0'
 HOME_PAGE = 'https://github.com/rec/gitz/blob/master/README.rst'
 
 # In development and when running tests, LIBRARY_DIRECTORY and
 # EXECUTABLE_DIRECTORY will be the same but in a pip installation
 # they will be different!
 LIBRARY_DIRECTORY = Path(__file__).absolute().parent.parent
 EXECUTABLE_DIRECTORY = Path(sys.argv[0]).absolute().parent
```

### Comparing `gitz-1.4.1/gitz/git/combine.py` & `gitz-1.5.0/gitz/git/combine.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/git/delete.py` & `gitz-1.5.0/gitz/git/delete.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/git/functions.py` & `gitz-1.5.0/gitz/git/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,16 +62,17 @@
 
     if must_fetch:
         for remote in remotes:
             fetch(remote)
 
     result = {}
     for rb in branches('-r'):
-        remote, branch = rb.split('/', maxsplit=1)
-        result.setdefault(remote, []).append(branch)
+        remote, *branch = rb.split('/', maxsplit=1)
+        if branch:
+            result.setdefault(remote, []).append(branch[0])
     return result
 
 
 def is_ancestor(parent, child='HEAD'):
     try:
         GIT.merge_base('--is-ancestor', parent, child)
         return True
```

### Comparing `gitz-1.4.1/gitz/git/guess_origin.py` & `gitz-1.5.0/gitz/git/guess_origin.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/git/mover.py` & `gitz-1.5.0/gitz/git/mover.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/git/reference_branch.py` & `gitz-1.5.0/gitz/git/reference_branch.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/git/repo.py` & `gitz-1.5.0/gitz/git/repo.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/git/root.py` & `gitz-1.5.0/gitz/git/root.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/git/save.py` & `gitz-1.5.0/gitz/git/save.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/program/env.py` & `gitz-1.5.0/gitz/program/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 PREFIX = 'GITZ_'
 CONFIG_FILE = '.gitz.json'
 
 
 class Env:
     DEFAULTS = {
-        'PROTECTED_BRANCHES': 'develop:main:master',
+        'PROTECTED_BRANCHES': 'develop:main:master:gh-pages',
         'REFERENCE_BRANCHES': 'develop:main:master',
         'ORIGIN': 'origin',
         'UPSTREAM': 'upstream:origin',
     }
 
     def __getattr__(self, key):
         return lambda: self.get(key)
```

### Comparing `gitz-1.4.1/gitz/program/log.py` & `gitz-1.5.0/gitz/program/log.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/program/parser.py` & `gitz-1.5.0/gitz/program/parser.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/program/print_help.py` & `gitz-1.5.0/gitz/program/print_help.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/program/program.py` & `gitz-1.5.0/gitz/program/program.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/program/run_proc.py` & `gitz-1.5.0/gitz/program/run_proc.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/program/runner.py` & `gitz-1.5.0/gitz/program/runner.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/gitz/program/summaries.py` & `gitz-1.5.0/gitz/program/summaries.py`

 * *Files identical despite different names*

### Comparing `gitz-1.4.1/pyproject.toml` & `gitz-1.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.black]
 line-length = 79
 skip-string-normalization = true
 target-version = ['py37']
 
 [tool.poetry]
 name = "gitz"
-version = "1.4.1"
-description = "🗜 gitz - tiny useful git commands, some dangerous 🗜"
+version = "1.5.0"
+description = "🗜 Tiny useful git commands, some dangerous 🗜"
 authors = ["Tom Ritchford <tom@swirly.com>"]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.scripts]
```

### Comparing `gitz-1.4.1/setup.py` & `gitz-1.5.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,190 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gitz
+Version: 1.5.0
+Summary: 🗜 Tiny useful git commands, some dangerous 🗜
+Author: Tom Ritchford
+Author-email: tom@swirly.com
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/x-rst
 
-packages = \
-['gitz', 'gitz.git', 'gitz.program']
+🗜 gitz - git commands for rapid development 🗜
+------------------------------------------------------
 
-package_data = \
-{'': ['*']}
+This is a collection of seventeen git utilities aimed at people doing rapid
+development using Git.
 
-scripts = \
-['git-adjust',
- 'git-copy',
- 'git-delete',
- 'git-for-each',
- 'git-gitz',
- 'git-go',
- 'git-infer',
- 'git-multi-pick',
- 'git-new',
- 'git-permute',
- 'git-rename',
- 'git-rot',
- 'git-save',
- 'git-split',
- 'git-st',
- 'git-stripe',
- 'git-update',
- 'git-when']
-
-setup_kwargs = {
-    'name': 'gitz',
-    'version': '1.4.1',
-    'description': '🗜 gitz - tiny useful git commands, some dangerous 🗜',
-    'long_description': "🗜 gitz - git commands for rapid development 🗜\n------------------------------------------------------\n\nThis is a collection of seventeen git utilities aimed at people doing rapid\ndevelopment using Git.\n\nGitz is for two types of users - quality-obsessed individuals who relentlessly\nmanicure their pull requests until every byte is in the right place; and\nultra-rapid developers who want to generate large features quickly while taking\nadvantage of continuous integration.\n\nMost of these utilities only exist here, one came from a chat on Reddit and\nI don't know where one of them came from.\n\nFour of them are written in Bash, the rest use Python 3.  They have been tested\non Mac OS/X (Darwin) and on Ubuntu, and will likely work on any Unix-like\noperating system.\n\nHow to install\n==============\n\nUse `pip <https://pypi.org/project/pip/>`_:\n\n.. code-block:: bash\n\n    pip3 install gitz\n\nOr simply download\n`this directory <https://github.com/rec/gitz/zipball/master/>`_\nand make sure it's in your shell's ``PATH`` - gitz has no\nexternal dependencies.\n\n\nGetting help\n============\n\nThis page contains a summary and a link to a manual page for each command.  From\nthe terminal, use ``-h`` flag like this: ``git new -h`` or use ``man`` like\nthis: ``man git-new``.\n\n\nWhen to use gitz\n=================\n\n1. At the start of a session\n\n   - ``git new`` safely creates fresh branches from upstream\n\n   - ``git update`` for each branch, rebases from upstream and force-pushes\n\n2. During development\n\n   - ``git st`` is a more compact and prettier ``git status``\n\n   - ``git when`` shows you when documents were last changed\n\n3. During rapid development\n\n   - ``git infer`` commits files with an automatically generated message -\n     great for committing tiny changes for later rebasing down\n\n4. While cleaning up a branch for review\n\n   - ``git permute`` permutes, squashes or removes commits in the current branch\n\n   - ``git split`` split one or more commits, perhaps with the staging area,\n     into many small individual commits, one per file\n\n5. During repository maintenance\n\n   - ``git rotate`` rotates through all branches\n\n   - ``git copy``, ``git delete``,  and ``git rename`` work on both local\n     and upstream branches\n\n6. Working with continuous integration\n\n   - ``git stripe`` pushes a sequence of commits to individual remote branches\n     where CI can find and test them\n\nThe movie\n==========\n\n.. figure:: https://asciinema.org/a/XwakAaMsMzKg4hIAJa18iiNac.png\n    :target: https://asciinema.org/a/XwakAaMsMzKg4hIAJa18iiNac?autoplay=1&theme=solarized-light&loop=1\n    :align: center\n    :alt: The whole gitz movie\n    :width: 430\n    :height: 402\n\nThe gitz commands\n-----------------\n\n\nSafe commands\n=============\n\nInformational commands that don't change your repository\n\n`git gitz <doc/git-gitz.rst>`_\n  Print information about the gitz git commands\n\n`git go <doc/git-go.rst>`_\n  Open a browser page for the current repo\n\n`git infer <doc/git-infer.rst>`_\n  Commit changes with an automatically generated message\n  \n  (from https://github.com/moondewio/git-infer)\n\n`git multi-pick <doc/git-multi-pick.rst>`_\n  Cherry-pick multiple commits, with an optional squash\n\n`git new <doc/git-new.rst>`_\n  Create and push new branches\n\n`git rot <doc/git-rot.rst>`_\n  Rotate through branches in a Git repository\n\n`git st <doc/git-st.rst>`_\n  Colorful, compact git status\n\n`git stripe <doc/git-stripe.rst>`_\n  Push a sequence of commit IDs to a remote repository\n\n`git when <doc/git-when.rst>`_\n  For each file, show the most recent commit that changed it.\n  \n  Dotfiles are ignored by default.\n\nDangerous commands that delete, rename or overwrite branches\n============================================================\n\n`git copy <doc/git-copy.rst>`_\n  Copy a git branch locally and remotely\n\n`git delete <doc/git-delete.rst>`_\n  Delete one or more branches locally and remotely\n\n`git rename <doc/git-rename.rst>`_\n  Rename a git branch locally and remotely\n\nBy default, the branches ``develop`` and ``master`` are protected -\nthey are not allowed to be copied to, renamed, or deleted.\n\nYou can configure this in three ways:\n\n- setting the ``--all/-a`` flag ignore protected branches entirely\n\n- setting the environment variable ``GITZ_PROTECTED_BRANCHES`` overrides these\n  defaults\n\n- setting a value for the keys ``PROTECTED_BRANCHES`` in the file\n  .gitz.json in the top directory of your Git project has the same effect\n\nDangerous commands that rewrite history\n=======================================\n\nSlice, dice, shuffle and split your commits.\n\nThese commands are not intended for use on a shared or production branch, but\ncan significantly speed up rapid development on private branches.\n\n`git adjust <doc/git-adjust.rst>`_\n  Amend any commit, not just the last\n\n`git permute <doc/git-permute.rst>`_\n  Reorder and delete commits in the current branch\n\n`git split <doc/git-split.rst>`_\n  Split a range of commits into many single-file commits\n\n`git update <doc/git-update.rst>`_\n  Update branches from a reference branch\n",
-    'author': 'Tom Ritchford',
-    'author_email': 'tom@swirly.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'scripts': scripts,
-    'python_requires': '>=3.7,<4.0',
-}
+Gitz is for two types of users - quality-obsessed individuals who relentlessly
+manicure their pull requests until every byte is in the right place; and
+ultra-rapid developers who want to generate large features quickly while taking
+advantage of continuous integration.
 
+Most of these utilities only exist here, one came from a chat on Reddit and
+I don't know where one of them came from.
+
+Four of them are written in Bash, the rest use Python 3.  They have been tested
+on Mac OS/X (Darwin) and on Ubuntu, and will likely work on any Unix-like
+operating system.
+
+How to install
+==============
+
+Use `pip <https://pypi.org/project/pip/>`_:
+
+.. code-block:: bash
+
+    pip3 install gitz
+
+Or simply download
+`this directory <https://github.com/rec/gitz/zipball/master/>`_
+and make sure it's in your shell's ``PATH`` - gitz has no
+external dependencies.
+
+
+Getting help
+============
+
+This page contains a summary and a link to a manual page for each command.  From
+the terminal, use ``-h`` flag like this: ``git new -h`` or use ``man`` like
+this: ``man git-new``.
+
+
+When to use gitz
+=================
+
+1. At the start of a session
+
+   - ``git new`` safely creates fresh branches from upstream
+
+   - ``git update`` for each branch, rebases from upstream and force-pushes
+
+2. During development
+
+   - ``git st`` is a more compact and prettier ``git status``
+
+   - ``git when`` shows you when documents were last changed
+
+3. During rapid development
+
+   - ``git infer`` commits files with an automatically generated message -
+     great for committing tiny changes for later rebasing down
+
+4. While cleaning up a branch for review
+
+   - ``git permute`` permutes, squashes or removes commits in the current branch
+
+   - ``git split`` split one or more commits, perhaps with the staging area,
+     into many small individual commits, one per file
+
+5. During repository maintenance
+
+   - ``git rotate`` rotates through all branches
+
+   - ``git copy``, ``git delete``,  and ``git rename`` work on both local
+     and upstream branches
+
+6. Working with continuous integration
+
+   - ``git stripe`` pushes a sequence of commits to individual remote branches
+     where CI can find and test them
+
+The movie
+==========
+
+.. figure:: https://asciinema.org/a/XwakAaMsMzKg4hIAJa18iiNac.png
+    :target: https://asciinema.org/a/XwakAaMsMzKg4hIAJa18iiNac?autoplay=1&theme=solarized-light&loop=1
+    :align: center
+    :alt: The whole gitz movie
+    :width: 430
+    :height: 402
+
+The gitz commands
+-----------------
+
+
+Safe commands
+=============
+
+Informational commands that don't change your repository
+
+`git gitz <doc/git-gitz.rst>`_
+  Print information about the gitz git commands
+
+`git go <doc/git-go.rst>`_
+  Open a browser page for the current repo
+
+`git infer <doc/git-infer.rst>`_
+  Commit changes with an automatically generated message
+  
+  (from https://github.com/moondewio/git-infer)
+
+`git multi-pick <doc/git-multi-pick.rst>`_
+  Cherry-pick multiple commits, with an optional squash
+
+`git new <doc/git-new.rst>`_
+  Create and push new branches
+
+`git rot <doc/git-rot.rst>`_
+  Rotate through branches in a Git repository
+
+`git st <doc/git-st.rst>`_
+  Colorful, compact git status
+
+`git stripe <doc/git-stripe.rst>`_
+  Push a sequence of commit IDs to a remote repository
+
+`git when <doc/git-when.rst>`_
+  For each file, show the most recent commit that changed it.
+  
+  Dotfiles are ignored by default.
+
+Dangerous commands that delete, rename or overwrite branches
+============================================================
+
+`git copy <doc/git-copy.rst>`_
+  Copy a git branch locally and remotely
+
+`git delete <doc/git-delete.rst>`_
+  Delete one or more branches locally and remotely
+
+`git rename <doc/git-rename.rst>`_
+  Rename a git branch locally and remotely
+
+By default, the branches ``develop`` and ``master`` are protected -
+they are not allowed to be copied to, renamed, or deleted.
+
+You can configure this in three ways:
+
+- setting the ``--all/-a`` flag ignore protected branches entirely
+
+- setting the environment variable ``GITZ_PROTECTED_BRANCHES`` overrides these
+  defaults
+
+- setting a value for the keys ``PROTECTED_BRANCHES`` in the file
+  .gitz.json in the top directory of your Git project has the same effect
+
+Dangerous commands that rewrite history
+=======================================
+
+Slice, dice, shuffle and split your commits.
+
+These commands are not intended for use on a shared or production branch, but
+can significantly speed up rapid development on private branches.
+
+`git adjust <doc/git-adjust.rst>`_
+  Amend any commit, not just the last
+
+`git permute <doc/git-permute.rst>`_
+  Reorder and delete commits in the current branch
+
+`git split <doc/git-split.rst>`_
+  Split a range of commits into many single-file commits
+
+`git update <doc/git-update.rst>`_
+  Update branches from a reference branch
 
-setup(**setup_kwargs)
```

