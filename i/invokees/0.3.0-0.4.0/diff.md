# Comparing `tmp/invokees-0.3.0.tar.gz` & `tmp/invokees-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invokees-0.3.0.tar", max compression
+gzip compressed data, was "invokees-0.4.0.tar", max compression
```

## Comparing `invokees-0.3.0.tar` & `invokees-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-03-05 18:06:21.861428 invokees-0.3.0/README.md
--rw-r--r--   0        0        0     1901 2023-06-17 12:09:11.683251 invokees-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-05 18:06:21.862947 invokees-0.3.0/src/invokees/__init__.py
--rw-r--r--   0        0        0      659 2023-03-05 18:06:21.863452 invokees-0.3.0/src/invokees/files.py
--rw-r--r--   0        0        0      278 2023-03-05 18:06:21.863910 invokees-0.3.0/src/invokees/tasks/__init__.py
--rw-r--r--   0        0        0     2501 2023-03-05 18:06:21.864204 invokees-0.3.0/src/invokees/tasks/code.py
--rw-r--r--   0        0        0        0 2023-06-17 12:04:18.930264 invokees-0.3.0/src/invokees/tasks/docs.py
--rw-r--r--   0        0        0        0 2023-06-17 12:04:18.930669 invokees-0.3.0/src/invokees/tasks/release.py
--rw-r--r--   0        0        0      647 2023-06-17 12:04:18.930955 invokees-0.3.0/src/invokees/tasks/self.py
--rw-r--r--   0        0        0     1999 2023-06-17 12:04:18.931126 invokees-0.3.0/src/invokees/tasks/test.py
--rw-r--r--   0        0        0        0 2023-03-05 18:06:21.864310 invokees-0.3.0/src/invokees/tools/__init__.py
--rw-r--r--   0        0        0     1188 1970-01-01 00:00:00.000000 invokees-0.3.0/setup.py
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 invokees-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-05 18:06:21.861428 invokees-0.4.0/README.md
+-rw-r--r--   0        0        0     1902 2023-06-17 12:14:39.467413 invokees-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-05 18:06:21.862947 invokees-0.4.0/src/invokees/__init__.py
+-rw-r--r--   0        0        0      659 2023-03-05 18:06:21.863452 invokees-0.4.0/src/invokees/files.py
+-rw-r--r--   0        0        0      278 2023-03-05 18:06:21.863910 invokees-0.4.0/src/invokees/tasks/__init__.py
+-rw-r--r--   0        0        0     2501 2023-03-05 18:06:21.864204 invokees-0.4.0/src/invokees/tasks/code.py
+-rw-r--r--   0        0        0        0 2023-06-17 12:04:18.930264 invokees-0.4.0/src/invokees/tasks/docs.py
+-rw-r--r--   0        0        0        0 2023-06-17 12:04:18.930669 invokees-0.4.0/src/invokees/tasks/release.py
+-rw-r--r--   0        0        0      647 2023-06-17 12:04:18.930955 invokees-0.4.0/src/invokees/tasks/self.py
+-rw-r--r--   0        0        0     1999 2023-06-17 12:04:18.931126 invokees-0.4.0/src/invokees/tasks/test.py
+-rw-r--r--   0        0        0        0 2023-03-05 18:06:21.864310 invokees-0.4.0/src/invokees/tools/__init__.py
+-rw-r--r--   0        0        0     1180 1970-01-01 00:00:00.000000 invokees-0.4.0/setup.py
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 invokees-0.4.0/PKG-INFO
```

### Comparing `invokees-0.3.0/pyproject.toml` & `invokees-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "invokees"
 packages = [{include = "invokees", from = "src"}]
 
-version = "0.3.0"
+version = "0.4.0"
 description = "Common python project tasks"
 authors = ["Nicola Coretti <nico.coretti@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 invoke = "^2.0.0"
 rich = "^13.3.1"
 pytest = "^7.2.1"
-prysk = {extras = ["pytest-plugin"], version = "^0.13.1"}
+prysk = {extras = ["pytest-plugin"], version = ">=0.13.1"}
 coverage = "^7.1.0"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.2.0"
 ruff = ">=0.0.247"
 mypy = "^1.0.1"
 black = "^23.1.0"
 tomlkit = "^0.11.6"
```

### Comparing `invokees-0.3.0/src/invokees/files.py` & `invokees-0.4.0/src/invokees/files.py`

 * *Files identical despite different names*

### Comparing `invokees-0.3.0/src/invokees/tasks/code.py` & `invokees-0.4.0/src/invokees/tasks/code.py`

 * *Files identical despite different names*

### Comparing `invokees-0.3.0/src/invokees/tasks/self.py` & `invokees-0.4.0/src/invokees/tasks/self.py`

 * *Files identical despite different names*

### Comparing `invokees-0.3.0/src/invokees/tasks/test.py` & `invokees-0.4.0/src/invokees/tasks/test.py`

 * *Files identical despite different names*

### Comparing `invokees-0.3.0/setup.py` & `invokees-0.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 install_requires = \
 ['black>=23.1.0,<24.0.0',
  'coverage>=7.1.0,<8.0.0',
  'invoke>=2.0.0,<3.0.0',
  'isort>=5.12.0,<6.0.0',
  'mypy>=1.0.1,<2.0.0',
  'pre-commit>=3.1.1,<4.0.0',
- 'prysk[pytest-plugin]>=0.13.1,<0.14.0',
+ 'prysk[pytest-plugin]>=0.13.1',
  'pytest-cov>=4.0.0,<5.0.0',
  'pytest-xdist>=3.2.0,<4.0.0',
  'pytest>=7.2.1,<8.0.0',
  'rich>=13.3.1,<14.0.0',
  'ruff>=0.0.247',
  'tomlkit>=0.11.6,<0.12.0',
  'types-docutils>=0.19.1.6',
  'types-invoke>=2.0.0.5,<3.0.0.0',
  'types-pygments>=2.14.0.5,<3.0.0.0',
  'types-setuptools>=67.4.0.3,<68.0.0.0']
 
 setup_kwargs = {
     'name': 'invokees',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Common python project tasks',
     'long_description': '',
     'author': 'Nicola Coretti',
     'author_email': 'nico.coretti@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `invokees-0.3.0/PKG-INFO` & `invokees-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invokees
-Version: 0.3.0
+Version: 0.4.0
 Summary: Common python project tasks
 License: MIT
 Author: Nicola Coretti
 Author-email: nico.coretti@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.1.0,<24.0.0)
 Requires-Dist: coverage (>=7.1.0,<8.0.0)
 Requires-Dist: invoke (>=2.0.0,<3.0.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: mypy (>=1.0.1,<2.0.0)
 Requires-Dist: pre-commit (>=3.1.1,<4.0.0)
-Requires-Dist: prysk[pytest-plugin] (>=0.13.1,<0.14.0)
+Requires-Dist: prysk[pytest-plugin] (>=0.13.1)
 Requires-Dist: pytest (>=7.2.1,<8.0.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: pytest-xdist (>=3.2.0,<4.0.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
 Requires-Dist: ruff (>=0.0.247)
 Requires-Dist: tomlkit (>=0.11.6,<0.12.0)
 Requires-Dist: types-docutils (>=0.19.1.6)
```

