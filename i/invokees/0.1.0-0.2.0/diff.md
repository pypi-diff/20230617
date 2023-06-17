# Comparing `tmp/invokees-0.1.0.tar.gz` & `tmp/invokees-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invokees-0.1.0.tar", max compression
+gzip compressed data, was "invokees-0.2.0.tar", max compression
```

## Comparing `invokees-0.1.0.tar` & `invokees-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,10 @@
--rw-r--r--   0        0        0        0 2023-02-17 21:35:43.133555 invokees-0.1.0/README.md
--rw-r--r--   0        0        0     1872 2023-03-05 20:59:32.722947 invokees-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-05 19:00:16.595850 invokees-0.1.0/src/invokees/__init__.py
--rw-r--r--   0        0        0      659 2023-03-05 19:00:16.595850 invokees-0.1.0/src/invokees/files.py
--rw-r--r--   0        0        0      278 2023-03-05 19:00:16.596850 invokees-0.1.0/src/invokees/tasks/__init__.py
--rw-r--r--   0        0        0     2501 2023-03-05 19:00:16.596850 invokees-0.1.0/src/invokees/tasks/code.py
--rw-r--r--   0        0        0        0 2023-03-05 20:01:32.235882 invokees-0.1.0/src/invokees/tasks/docs.py
--rw-r--r--   0        0        0        0 2023-03-05 20:00:27.928023 invokees-0.1.0/src/invokees/tasks/release.py
--rw-r--r--   0        0        0      647 2023-03-05 20:54:00.506478 invokees-0.1.0/src/invokees/tasks/self.py
--rw-r--r--   0        0        0     1999 2023-03-05 20:23:57.144957 invokees-0.1.0/src/invokees/tasks/test.py
--rw-r--r--   0        0        0        0 2023-03-05 19:00:16.597850 invokees-0.1.0/src/invokees/tools/__init__.py
--rw-r--r--   0        0        0     1174 2023-03-05 21:28:12.422524 invokees-0.1.0/setup.py
--rw-r--r--   0        0        0     1207 2023-03-05 21:28:12.422749 invokees-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-05 18:06:21.861428 invokees-0.2.0/README.md
+-rw-r--r--   0        0        0     1833 2023-06-17 11:48:33.529946 invokees-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-05 18:06:21.862947 invokees-0.2.0/src/invokees/__init__.py
+-rw-r--r--   0        0        0      659 2023-03-05 18:06:21.863452 invokees-0.2.0/src/invokees/files.py
+-rw-r--r--   0        0        0      278 2023-03-05 18:06:21.863910 invokees-0.2.0/src/invokees/tasks/__init__.py
+-rw-r--r--   0        0        0     2501 2023-03-05 18:06:21.864204 invokees-0.2.0/src/invokees/tasks/code.py
+-rw-r--r--   0        0        0      837 2023-03-05 18:06:21.868636 invokees-0.2.0/src/invokees/tasks/self.py
+-rw-r--r--   0        0        0        0 2023-03-05 18:06:21.864310 invokees-0.2.0/src/invokees/tools/__init__.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 invokees-0.2.0/setup.py
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 invokees-0.2.0/PKG-INFO
```

### Comparing `invokees-0.1.0/pyproject.toml` & `invokees-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "invokees"
 packages = [{include = "invokees", from = "src"}]
 
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Nicola Coretti <nico.coretti@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 invoke = "^2.0.0"
 rich = "^13.3.1"
 pytest = "^7.2.1"
-prysk = {extras = ["pytest-plugin"], version = "^0.13.1"}
+prysk = ">=0.13.0"
 coverage = "^7.1.0"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.2.0"
 ruff = "^0.0.247"
 mypy = "^1.0.1"
 black = "^23.1.0"
 tomlkit = "^0.11.6"
```

### Comparing `invokees-0.1.0/src/invokees/files.py` & `invokees-0.2.0/src/invokees/files.py`

 * *Files identical despite different names*

### Comparing `invokees-0.1.0/src/invokees/tasks/code.py` & `invokees-0.2.0/src/invokees/tasks/code.py`

 * *Files identical despite different names*

### Comparing `invokees-0.1.0/setup.py` & `invokees-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,36 +13,36 @@
 install_requires = \
 ['black>=23.1.0,<24.0.0',
  'coverage>=7.1.0,<8.0.0',
  'invoke>=2.0.0,<3.0.0',
  'isort>=5.12.0,<6.0.0',
  'mypy>=1.0.1,<2.0.0',
  'pre-commit>=3.1.1,<4.0.0',
- 'prysk[pytest-plugin]>=0.13.1,<0.14.0',
+ 'prysk>=0.13.0',
  'pytest-cov>=4.0.0,<5.0.0',
  'pytest-xdist>=3.2.0,<4.0.0',
  'pytest>=7.2.1,<8.0.0',
  'rich>=13.3.1,<14.0.0',
  'ruff>=0.0.247,<0.0.248',
  'tomlkit>=0.11.6,<0.12.0',
  'types-docutils>=0.19.1.6,<0.20.0.0',
  'types-invoke>=2.0.0.5,<3.0.0.0',
  'types-pygments>=2.14.0.5,<3.0.0.0',
  'types-setuptools>=67.4.0.3,<68.0.0.0']
 
 setup_kwargs = {
     'name': 'invokees',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': '',
     'author': 'Nicola Coretti',
     'author_email': 'nico.coretti@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `invokees-0.1.0/PKG-INFO` & `invokees-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: invokees
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Nicola Coretti
 Author-email: nico.coretti@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.1.0,<24.0.0)
 Requires-Dist: coverage (>=7.1.0,<8.0.0)
 Requires-Dist: invoke (>=2.0.0,<3.0.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: mypy (>=1.0.1,<2.0.0)
 Requires-Dist: pre-commit (>=3.1.1,<4.0.0)
-Requires-Dist: prysk[pytest-plugin] (>=0.13.1,<0.14.0)
+Requires-Dist: prysk (>=0.13.0)
 Requires-Dist: pytest (>=7.2.1,<8.0.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: pytest-xdist (>=3.2.0,<4.0.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
 Requires-Dist: ruff (>=0.0.247,<0.0.248)
 Requires-Dist: tomlkit (>=0.11.6,<0.12.0)
 Requires-Dist: types-docutils (>=0.19.1.6,<0.20.0.0)
```

