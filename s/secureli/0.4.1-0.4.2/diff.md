# Comparing `tmp/secureli-0.4.1.tar.gz` & `tmp/secureli-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.4.1.tar", max compression
+gzip compressed data, was "secureli-0.4.2.tar", max compression
```

## Comparing `secureli-0.4.1.tar` & `secureli-0.4.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    11343 2023-06-16 21:37:18.997710 secureli-0.4.1/LICENSE
--rw-r--r--   0        0        0    11614 2023-06-16 21:37:18.997710 secureli-0.4.1/README.md
--rw-r--r--   0        0        0     2043 2023-06-16 21:37:19.001710 secureli-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0    34252 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/actions/__init__.py
--rw-r--r--   0        0        0    10730 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/actions/action.py
--rw-r--r--   0        0        0      761 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/actions/build.py
--rw-r--r--   0        0        0     1160 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10628 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/actions/scan.py
--rw-r--r--   0        0        0      791 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/actions/setup.py
--rw-r--r--   0        0        0     2087 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/actions/update.py
--rw-r--r--   0        0        0     6165 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/container.py
--rw-r--r--   0        0        0     2807 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/main.py
--rw-r--r--   0        0        0        0 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     1752 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3926 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/__init__.py
--rw-r--r--   0        0        0     4883 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/files/build.txt
--rw-r--r--   0        0        0       93 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/files/configs/javascript.config.yaml
--rw-r--r--   0        0        0      161 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/files/configs/typescript.config.yaml
--rw-r--r--   0        0        0     1271 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      461 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      619 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0     1363 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/files/javascript-pre-commit.yaml
--rw-r--r--   0        0        0     1151 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      409 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      433 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0     1349 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0     2225 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/services/language_support.py
--rw-r--r--   0        0        0     4413 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3074 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1080 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0     1372 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0     1028 2023-06-16 21:37:19.001710 secureli-0.4.1/secureli/utilities/usage_stats.py
--rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 secureli-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-06-16 22:35:29.401878 secureli-0.4.2/LICENSE
+-rw-r--r--   0        0        0    11614 2023-06-16 22:35:29.401878 secureli-0.4.2/README.md
+-rw-r--r--   0        0        0     2043 2023-06-16 22:35:29.401878 secureli-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 22:35:29.401878 secureli-0.4.2/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 22:35:29.401878 secureli-0.4.2/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-16 22:35:29.401878 secureli-0.4.2/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-06-16 22:35:29.401878 secureli-0.4.2/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0    34252 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    10730 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/actions/build.py
+-rw-r--r--   0        0        0     1160 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10628 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/actions/scan.py
+-rw-r--r--   0        0        0      791 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/actions/update.py
+-rw-r--r--   0        0        0     6165 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     1752 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3926 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/__init__.py
+-rw-r--r--   0        0        0     4883 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0       93 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/files/configs/javascript.config.yaml
+-rw-r--r--   0        0        0      161 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/files/configs/typescript.config.yaml
+-rw-r--r--   0        0        0     1271 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      461 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      619 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0     1363 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/files/javascript-pre-commit.yaml
+-rw-r--r--   0        0        0     1151 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      409 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      433 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0     1349 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0     2225 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4413 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3074 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0     1372 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0     1028 2023-06-16 22:35:29.405878 secureli-0.4.2/secureli/utilities/usage_stats.py
+-rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 secureli-0.4.2/PKG-INFO
```

### Comparing `secureli-0.4.1/LICENSE` & `secureli-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/README.md` & `secureli-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/pyproject.toml` & `secureli-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secureli"
-version = "0.4.1"
+version = "0.4.2"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
```

### Comparing `secureli-0.4.1/secureli/abstractions/echo.py` & `secureli-0.4.2/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/abstractions/lexer_guesser.py` & `secureli-0.4.2/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/abstractions/pre_commit.py` & `secureli-0.4.2/secureli/abstractions/pre_commit.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/actions/action.py` & `secureli-0.4.2/secureli/actions/action.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/actions/build.py` & `secureli-0.4.2/secureli/actions/build.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/actions/initializer.py` & `secureli-0.4.2/secureli/actions/initializer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/actions/scan.py` & `secureli-0.4.2/secureli/actions/scan.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/actions/setup.py` & `secureli-0.4.2/secureli/actions/setup.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/actions/update.py` & `secureli-0.4.2/secureli/actions/update.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/container.py` & `secureli-0.4.2/secureli/container.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/main.py` & `secureli-0.4.2/secureli/main.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/repositories/repo_files.py` & `secureli-0.4.2/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/repositories/secureli_config.py` & `secureli-0.4.2/secureli/repositories/secureli_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/repositories/settings.py` & `secureli-0.4.2/secureli/repositories/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/resources/files/build.txt` & `secureli-0.4.2/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/resources/files/csharp-pre-commit.yaml` & `secureli-0.4.2/secureli/resources/files/csharp-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/resources/files/java-pre-commit.yaml` & `secureli-0.4.2/secureli/resources/files/java-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/resources/files/javascript-pre-commit.yaml` & `secureli-0.4.2/secureli/resources/files/javascript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/resources/files/python-pre-commit.yaml` & `secureli-0.4.2/secureli/resources/files/python-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.4.2/secureli/resources/files/typescript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/resources/read_resource.py` & `secureli-0.4.2/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/resources/slugify.py` & `secureli-0.4.2/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/services/git_ignore.py` & `secureli-0.4.2/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/services/language_analyzer.py` & `secureli-0.4.2/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/services/language_support.py` & `secureli-0.4.2/secureli/services/language_support.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/services/logging.py` & `secureli-0.4.2/secureli/services/logging.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/services/scanner.py` & `secureli-0.4.2/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/services/secureli_ignore.py` & `secureli-0.4.2/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/services/updater.py` & `secureli-0.4.2/secureli/services/updater.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/settings.py` & `secureli-0.4.2/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/utilities/git_meta.py` & `secureli-0.4.2/secureli/utilities/git_meta.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/utilities/patterns.py` & `secureli-0.4.2/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/secureli/utilities/usage_stats.py` & `secureli-0.4.2/secureli/utilities/usage_stats.py`

 * *Files identical despite different names*

### Comparing `secureli-0.4.1/PKG-INFO` & `secureli-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.4.1
+Version: 0.4.2
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

