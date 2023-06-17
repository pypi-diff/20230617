# Comparing `tmp/pymolecule_parser-0.0.0.tar.gz` & `tmp/pymolecule_parser-0.0.1.tar.gz`

## Comparing `pymolecule_parser-0.0.0.tar` & `pymolecule_parser-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/main.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/src/pymolecule_parser/__about__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/src/pymolecule_parser/__init__.py
--rwxr-xr-x   0        0        0     7017 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/src/pymolecule_parser/pymolecule_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/tests/unit_test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/LICENSE
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/README.md
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/main.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/src/pymolecule_parser/__about__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/src/pymolecule_parser/__init__.py
+-rwxr-xr-x   0        0        0     7017 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/src/pymolecule_parser/pymolecule_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/tests/unit_test.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/LICENSE
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/README.md
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 pymolecule_parser-0.0.1/PKG-INFO
```

### Comparing `pymolecule_parser-0.0.0/.github/workflows/build.yml` & `pymolecule_parser-0.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pymolecule_parser-0.0.0/.github/workflows/test.yml` & `pymolecule_parser-0.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pymolecule_parser-0.0.0/src/pymolecule_parser/pymolecule_parser.py` & `pymolecule_parser-0.0.1/src/pymolecule_parser/pymolecule_parser.py`

 * *Files identical despite different names*

### Comparing `pymolecule_parser-0.0.0/.gitignore` & `pymolecule_parser-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pymolecule_parser-0.0.0/LICENSE` & `pymolecule_parser-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymolecule_parser-0.0.0/README.md` & `pymolecule_parser-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pymolecule_parser-0.0.0/pyproject.toml` & `pymolecule_parser-0.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymolecule_parser-0.0.0/PKG-INFO` & `pymolecule_parser-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymolecule-parser
-Version: 0.0.0
+Version: 0.0.1
 Summary: A parser for molecule formula. Nested brackets are supported.
 Project-URL: Documentation, https://github.com/kohei-noda-qcrg/pymolecule-parser#readme
 Project-URL: Issues, https://github.com/kohei-noda-qcrg/pymolecule-parser/issues
 Project-URL: Source, https://github.com/kohei-noda-qcrg/pymolecule-parser
 Author-email: Kohei Noda <kohei-noda@hiroshima-u.ac.jp>
 License-Expression: MIT
 License-File: LICENSE
```

