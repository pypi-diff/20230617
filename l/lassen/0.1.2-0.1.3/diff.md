# Comparing `tmp/lassen-0.1.2.tar.gz` & `tmp/lassen-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lassen-0.1.2.tar", max compression
+gzip compressed data, was "lassen-0.1.3.tar", max compression
```

## Comparing `lassen-0.1.2.tar` & `lassen-0.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1071 2023-06-06 18:13:43.336753 lassen-0.1.2/LICENSE
--rw-r--r--   0        0        0     2781 2023-06-15 21:16:27.733755 lassen-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986429 lassen-0.1.2/lassen/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986933 lassen-0.1.2/lassen/alembic/__init__.py
--rw-r--r--   0        0        0     3685 2023-06-06 23:14:20.987092 lassen-0.1.2/lassen/alembic/cli.py
--rw-r--r--   0        0        0     3601 2023-06-06 23:14:20.987203 lassen-0.1.2/lassen/alembic/io.py
--rw-r--r--   0        0        0     1043 2023-06-06 23:14:20.987305 lassen-0.1.2/lassen/alembic/runner.py
--rw-r--r--   0        0        0      174 2023-06-06 23:14:20.987414 lassen-0.1.2/lassen/assets/__init__.py
--rw-r--r--   0        0        0     1592 2023-06-06 23:14:20.987525 lassen-0.1.2/lassen/assets/alembic.ini
--rw-r--r--   0        0        0      494 2023-06-06 23:14:20.987634 lassen-0.1.2/lassen/assets/script.py.mako
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.987697 lassen-0.1.2/lassen/core/__init__.py
--rw-r--r--   0        0        0      153 2023-06-15 21:16:27.734730 lassen-0.1.2/lassen/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2487 2023-06-15 21:16:27.734981 lassen-0.1.2/lassen/core/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     1862 2023-06-06 23:14:20.988497 lassen-0.1.2/lassen/core/config.py
--rw-r--r--   0        0        0        0 2023-06-15 21:16:27.735020 lassen-0.1.2/lassen/datasets/__init__.py
--rw-r--r--   0        0        0     2368 2023-06-15 22:39:22.170659 lassen-0.1.2/lassen/datasets/dataset_helpers.py
--rw-r--r--   0        0        0     3024 2023-06-15 22:26:02.922940 lassen-0.1.2/lassen/datasets/pyarrow_schemas.py
--rw-r--r--   0        0        0      240 2023-06-06 23:14:20.988685 lassen-0.1.2/lassen/db/__init__.py
--rw-r--r--   0        0        0      396 2023-06-15 21:16:27.735607 lassen-0.1.2/lassen/db/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      139 2023-06-06 23:14:20.989157 lassen-0.1.2/lassen/db/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      147 2023-06-06 23:14:20.989285 lassen-0.1.2/lassen/db/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      293 2023-06-06 23:14:20.989436 lassen-0.1.2/lassen/db/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1931 2023-06-15 21:16:27.735885 lassen-0.1.2/lassen/db/__pycache__/base_class.cpython-310.pyc
--rw-r--r--   0        0        0     2727 2023-06-06 23:14:20.989823 lassen-0.1.2/lassen/db/__pycache__/base_class.cpython-311.pyc
--rw-r--r--   0        0        0      839 2023-06-15 21:16:27.736092 lassen-0.1.2/lassen/db/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0     1271 2023-06-06 23:14:20.990178 lassen-0.1.2/lassen/db/__pycache__/session.cpython-311.pyc
--rw-r--r--   0        0        0     1909 2023-06-06 23:14:20.990303 lassen-0.1.2/lassen/db/base_class.py
--rw-r--r--   0        0        0      627 2023-06-06 23:14:20.990409 lassen-0.1.2/lassen/db/session.py
--rw-r--r--   0        0        0      210 2023-06-06 23:14:20.990522 lassen-0.1.2/lassen/schema.py
--rw-r--r--   0        0        0      227 2023-06-15 21:16:27.736193 lassen-0.1.2/lassen/shared.py
--rw-r--r--   0        0        0     9983 2023-06-06 23:14:20.990676 lassen-0.1.2/lassen/store.py
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.990727 lassen-0.1.2/lassen/tests/__init__.py
--rw-r--r--   0        0        0      154 2023-06-15 21:16:27.736415 lassen-0.1.2/lassen/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1973 2023-06-15 21:31:07.938752 lassen-0.1.2/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1220 2023-06-06 23:14:20.991368 lassen-0.1.2/lassen/tests/__pycache__/fixtures.cpython-310.pyc
--rw-r--r--   0        0        0     5734 2023-06-15 21:16:27.736953 lassen-0.1.2/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1901 2023-06-15 21:16:27.737091 lassen-0.1.2/lassen/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-15 21:16:27.737128 lassen-0.1.2/lassen/tests/datasets/__init__.py
--rw-r--r--   0        0        0     2243 2023-06-15 22:42:38.547093 lassen-0.1.2/lassen/tests/datasets/test_dataset_helpers.py
--rw-r--r--   0        0        0     1645 2023-06-15 22:26:02.923228 lassen-0.1.2/lassen/tests/datasets/test_pyarrow_schemas.py
--rw-r--r--   0        0        0      176 2023-06-06 23:14:20.991801 lassen-0.1.2/lassen/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      463 2023-06-06 23:14:20.991923 lassen-0.1.2/lassen/tests/fixtures/test_harness/README.md
--rw-r--r--   0        0        0      311 2023-06-06 23:14:20.992056 lassen-0.1.2/lassen/tests/fixtures/test_harness/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.992112 lassen-0.1.2/lassen/tests/fixtures/test_harness/test_harness/__init__.py
--rw-r--r--   0        0        0      691 2023-06-06 23:14:20.992321 lassen-0.1.2/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py
--rw-r--r--   0        0        0      653 2023-06-06 23:14:20.992456 lassen-0.1.2/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py
--rw-r--r--   0        0        0      217 2023-06-06 23:14:20.992593 lassen-0.1.2/lassen/tests/fixtures/test_harness/test_harness/models.py
--rw-r--r--   0        0        0      461 2023-06-06 23:14:20.992727 lassen-0.1.2/lassen/tests/model_fixtures.py
--rw-r--r--   0        0        0     2252 2023-06-06 23:14:20.992858 lassen-0.1.2/lassen/tests/test_alembic.py
--rw-r--r--   0        0        0     2799 2023-06-06 23:14:20.992986 lassen-0.1.2/lassen/tests/test_store.py
--rw-r--r--   0        0        0     1224 2023-06-15 22:43:13.240473 lassen-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 lassen-0.1.2/setup.py
--rw-r--r--   0        0        0     3696 1970-01-01 00:00:00.000000 lassen-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 18:13:43.336753 lassen-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2781 2023-06-15 21:16:27.733755 lassen-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986429 lassen-0.1.3/lassen/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986933 lassen-0.1.3/lassen/alembic/__init__.py
+-rw-r--r--   0        0        0     3685 2023-06-06 23:14:20.987092 lassen-0.1.3/lassen/alembic/cli.py
+-rw-r--r--   0        0        0     3601 2023-06-06 23:14:20.987203 lassen-0.1.3/lassen/alembic/io.py
+-rw-r--r--   0        0        0     1043 2023-06-06 23:14:20.987305 lassen-0.1.3/lassen/alembic/runner.py
+-rw-r--r--   0        0        0      174 2023-06-06 23:14:20.987414 lassen-0.1.3/lassen/assets/__init__.py
+-rw-r--r--   0        0        0     1592 2023-06-06 23:14:20.987525 lassen-0.1.3/lassen/assets/alembic.ini
+-rw-r--r--   0        0        0      494 2023-06-06 23:14:20.987634 lassen-0.1.3/lassen/assets/script.py.mako
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.987697 lassen-0.1.3/lassen/core/__init__.py
+-rw-r--r--   0        0        0      153 2023-06-15 21:16:27.734730 lassen-0.1.3/lassen/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2487 2023-06-15 21:16:27.734981 lassen-0.1.3/lassen/core/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     1862 2023-06-06 23:14:20.988497 lassen-0.1.3/lassen/core/config.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:16:27.735020 lassen-0.1.3/lassen/datasets/__init__.py
+-rw-r--r--   0        0        0     2368 2023-06-15 22:39:22.170659 lassen-0.1.3/lassen/datasets/dataset_helpers.py
+-rw-r--r--   0        0        0     3024 2023-06-15 22:26:02.922940 lassen-0.1.3/lassen/datasets/pyarrow_schemas.py
+-rw-r--r--   0        0        0      240 2023-06-06 23:14:20.988685 lassen-0.1.3/lassen/db/__init__.py
+-rw-r--r--   0        0        0      396 2023-06-15 21:16:27.735607 lassen-0.1.3/lassen/db/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      139 2023-06-06 23:14:20.989157 lassen-0.1.3/lassen/db/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      147 2023-06-06 23:14:20.989285 lassen-0.1.3/lassen/db/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      293 2023-06-06 23:14:20.989436 lassen-0.1.3/lassen/db/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1931 2023-06-15 21:16:27.735885 lassen-0.1.3/lassen/db/__pycache__/base_class.cpython-310.pyc
+-rw-r--r--   0        0        0     2727 2023-06-06 23:14:20.989823 lassen-0.1.3/lassen/db/__pycache__/base_class.cpython-311.pyc
+-rw-r--r--   0        0        0      839 2023-06-15 21:16:27.736092 lassen-0.1.3/lassen/db/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0     1271 2023-06-06 23:14:20.990178 lassen-0.1.3/lassen/db/__pycache__/session.cpython-311.pyc
+-rw-r--r--   0        0        0     1909 2023-06-06 23:14:20.990303 lassen-0.1.3/lassen/db/base_class.py
+-rw-r--r--   0        0        0      627 2023-06-06 23:14:20.990409 lassen-0.1.3/lassen/db/session.py
+-rw-r--r--   0        0        0      210 2023-06-06 23:14:20.990522 lassen-0.1.3/lassen/schema.py
+-rw-r--r--   0        0        0      227 2023-06-15 21:16:27.736193 lassen-0.1.3/lassen/shared.py
+-rw-r--r--   0        0        0     9983 2023-06-06 23:14:20.990676 lassen-0.1.3/lassen/store.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.990727 lassen-0.1.3/lassen/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-15 21:16:27.736415 lassen-0.1.3/lassen/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1973 2023-06-15 21:31:07.938752 lassen-0.1.3/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1220 2023-06-06 23:14:20.991368 lassen-0.1.3/lassen/tests/__pycache__/fixtures.cpython-310.pyc
+-rw-r--r--   0        0        0     5734 2023-06-15 21:16:27.736953 lassen-0.1.3/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1901 2023-06-15 21:16:27.737091 lassen-0.1.3/lassen/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:16:27.737128 lassen-0.1.3/lassen/tests/datasets/__init__.py
+-rw-r--r--   0        0        0     2243 2023-06-15 22:42:38.547093 lassen-0.1.3/lassen/tests/datasets/test_dataset_helpers.py
+-rw-r--r--   0        0        0     1645 2023-06-15 22:26:02.923228 lassen-0.1.3/lassen/tests/datasets/test_pyarrow_schemas.py
+-rw-r--r--   0        0        0      176 2023-06-06 23:14:20.991801 lassen-0.1.3/lassen/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-06 23:14:20.991923 lassen-0.1.3/lassen/tests/fixtures/test_harness/README.md
+-rw-r--r--   0        0        0      311 2023-06-06 23:14:20.992056 lassen-0.1.3/lassen/tests/fixtures/test_harness/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.992112 lassen-0.1.3/lassen/tests/fixtures/test_harness/test_harness/__init__.py
+-rw-r--r--   0        0        0      691 2023-06-06 23:14:20.992321 lassen-0.1.3/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py
+-rw-r--r--   0        0        0      653 2023-06-06 23:14:20.992456 lassen-0.1.3/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py
+-rw-r--r--   0        0        0      217 2023-06-06 23:14:20.992593 lassen-0.1.3/lassen/tests/fixtures/test_harness/test_harness/models.py
+-rw-r--r--   0        0        0      461 2023-06-06 23:14:20.992727 lassen-0.1.3/lassen/tests/model_fixtures.py
+-rw-r--r--   0        0        0     2252 2023-06-06 23:14:20.992858 lassen-0.1.3/lassen/tests/test_alembic.py
+-rw-r--r--   0        0        0     2799 2023-06-06 23:14:20.992986 lassen-0.1.3/lassen/tests/test_store.py
+-rw-r--r--   0        0        0     1325 2023-06-17 18:38:20.916738 lassen-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4347 1970-01-01 00:00:00.000000 lassen-0.1.3/setup.py
+-rw-r--r--   0        0        0     3763 1970-01-01 00:00:00.000000 lassen-0.1.3/PKG-INFO
```

### Comparing `lassen-0.1.2/LICENSE` & `lassen-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/README.md` & `lassen-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/alembic/cli.py` & `lassen-0.1.3/lassen/alembic/cli.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/alembic/io.py` & `lassen-0.1.3/lassen/alembic/io.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/alembic/runner.py` & `lassen-0.1.3/lassen/alembic/runner.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/assets/alembic.ini` & `lassen-0.1.3/lassen/assets/alembic.ini`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/core/__pycache__/config.cpython-310.pyc` & `lassen-0.1.3/lassen/core/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/core/config.py` & `lassen-0.1.3/lassen/core/config.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/datasets/dataset_helpers.py` & `lassen-0.1.3/lassen/datasets/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/datasets/pyarrow_schemas.py` & `lassen-0.1.3/lassen/datasets/pyarrow_schemas.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/db/__pycache__/base_class.cpython-310.pyc` & `lassen-0.1.3/lassen/db/__pycache__/base_class.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/db/__pycache__/base_class.cpython-311.pyc` & `lassen-0.1.3/lassen/db/__pycache__/base_class.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/db/__pycache__/session.cpython-310.pyc` & `lassen-0.1.3/lassen/db/__pycache__/session.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/db/__pycache__/session.cpython-311.pyc` & `lassen-0.1.3/lassen/db/__pycache__/session.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/db/base_class.py` & `lassen-0.1.3/lassen/db/base_class.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/db/session.py` & `lassen-0.1.3/lassen/db/session.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/store.py` & `lassen-0.1.3/lassen/store.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc` & `lassen-0.1.3/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/tests/__pycache__/fixtures.cpython-310.pyc` & `lassen-0.1.3/lassen/tests/__pycache__/fixtures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc` & `lassen-0.1.3/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/tests/conftest.py` & `lassen-0.1.3/lassen/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/tests/datasets/test_dataset_helpers.py` & `lassen-0.1.3/lassen/tests/datasets/test_dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/tests/datasets/test_pyarrow_schemas.py` & `lassen-0.1.3/lassen/tests/datasets/test_pyarrow_schemas.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py` & `lassen-0.1.3/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py` & `lassen-0.1.3/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/tests/test_alembic.py` & `lassen-0.1.3/lassen/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/lassen/tests/test_store.py` & `lassen-0.1.3/lassen/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.2/pyproject.toml` & `lassen-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "lassen"
-version = "0.1.2"
+version = "0.1.3"
 description = "Common webapp scaffolding."
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = "^0.96.0"
 pydantic = "^1.10.8"
-SQLAlchemy = "^2.0.15"
 inflection = "^0.5.1"
-psycopg2 = "^2.9.6"
 click = "^8.1.3"
 alembic = "^1.11.1"
 alembic-autogenerate-enums = "^0.1.1"
 python-dotenv = "^1.0.0"
 
 datasets = { version = "^2.13.0", optional = true }
 numpy = { version = "^1.24.3", optional = true }
 pandas = { version = "^2.0.2", optional = true }
 
+SQLAlchemy = { version = "^2.0.15", optional = true }
+psycopg2 = { version = "^2.9.6", optional = true }
+
 [tool.poetry.extras]
 datasets = ["datasets", "numpy", "pandas"]
+database = ["SQLAlchemy", "psycopg2"]
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 black = "^23.3.0"
 mypy = "^1.3.0"
```

### Comparing `lassen-0.1.2/setup.py` & `lassen-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,35 +14,34 @@
  'lassen.tests.fixtures.test_harness.test_harness',
  'lassen.tests.fixtures.test_harness.test_harness.migrations']
 
 package_data = \
 {'': ['*'], 'lassen.tests.fixtures': ['test_harness/*']}
 
 install_requires = \
-['SQLAlchemy>=2.0.15,<3.0.0',
- 'alembic-autogenerate-enums>=0.1.1,<0.2.0',
+['alembic-autogenerate-enums>=0.1.1,<0.2.0',
  'alembic>=1.11.1,<2.0.0',
  'click>=8.1.3,<9.0.0',
  'fastapi>=0.96.0,<0.97.0',
  'inflection>=0.5.1,<0.6.0',
- 'psycopg2>=2.9.6,<3.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'python-dotenv>=1.0.0,<2.0.0']
 
 extras_require = \
-{'datasets': ['datasets>=2.13.0,<3.0.0',
+{'database': ['SQLAlchemy>=2.0.15,<3.0.0', 'psycopg2>=2.9.6,<3.0.0'],
+ 'datasets': ['datasets>=2.13.0,<3.0.0',
               'numpy>=1.24.3,<2.0.0',
               'pandas>=2.0.2,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['migrate = lassen.alembic.cli:main']}
 
 setup_kwargs = {
     'name': 'lassen',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Common webapp scaffolding.',
     'long_description': '# lassen\n\n**40.4881° N, 121.5049° W**\n\nCore utilities for MonkeySee web applications.\n\nNot guaranteed to be backwards compatible, use at your own risk.\n\n## Structure\n\n**Stores:** Each model is expected to have its own store. Base classes that provide standard logic are provided by `lassen.store`\n- StoreBase: Base class for all stores\n- StoreFilterMixin: Mixin for filtering stores that specify an additional schema to use to filter\n\n**Datasets:** Optional huggingface `datasets` processing utilities. Only installed under the `lassen[datasets]` extra. These provide support for:\n\n- batch_to_examples: Iterate and manipulate each example separately, versus over nested key-based lists.\n- examples_to_batch: Takes the output of a typehinted element-wise batch and converts into the format needed for dataset insertion. If datasets can\'t automatically interpret the type of the fields, also provide automatic casting based on the typehinted dataclass.\n\n```python\nfrom lassen.datasets import batch_to_examples, examples_to_batch\nimport pandas as pd\n\n@dataclass\nclass BatchInsertion:\n    texts: list[str]\n\ndef batch_process(examples):\n    new_examples : list[BatchInsertion] = []\n    for example in batch_to_examples(examples):\n        new_examples.append(\n            BatchInsertion(\n                example["raw_text"].split()\n            )\n        )\n\n    # datasets won\'t be able to typehint a dataset that starts with an empty example, so we use our explicit schema to cast the data\n    return examples_to_batch(new_examples, BatchInsertion, explicit_schema=True)\n\ndf = pd.DataFrame(\n    [\n        {"raw_text": ""},\n        {"raw_text": "This is a test"},\n        {"raw_text": "This is another test"},\n    ]\n)\n\ndataset = Dataset.from_pandas(df)\n\ndataset = dataset.map(\n    batch_process,\n    batched=True,\n    batch_size=1,\n    num_proc=1,\n    remove_columns=dataset.column_names,\n)\n```\n\n**Migrations:** Lassen includes a templated alembic.init and env.py file. Client applications just need to have a `migrations` folder within their project root. After this you can swap `poetry run alembic` with `poetry run migrate`.\n\n```sh\npoetry run migrate upgrade head\n```\n\n**Settings:** Application settings should subclass our core settings. This provides a standard way to load settings from environment variables and includes common database keys.\n\n```python\nfrom lassen.core.config import CoreSettings, register_settings\n\n@register_settings\nclass ClientSettings(CoreSettings):\n    pass\n```\n\n**Schemas:** For helper schemas when returning results via API, see [lassen.schema](./lassen/schema.py).\n\n## Development\n\n```sh\npoetry install --extras "datasets"\n\ncreateuser lassen\ncreatedb -O lassen lassen_db\ncreatedb -O lassen lassen_test_db\n```\n\nUnit Tests:\n\n```sh\npoetry run pytest\n```\n',
     'author': 'Pierce Freeman',
     'author_email': 'pierce@freeman.vc',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `lassen-0.1.2/PKG-INFO` & `lassen-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: lassen
-Version: 0.1.2
+Version: 0.1.3
 Summary: Common webapp scaffolding.
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: database
 Provides-Extra: datasets
-Requires-Dist: SQLAlchemy (>=2.0.15,<3.0.0)
+Requires-Dist: SQLAlchemy (>=2.0.15,<3.0.0); extra == "database"
 Requires-Dist: alembic (>=1.11.1,<2.0.0)
 Requires-Dist: alembic-autogenerate-enums (>=0.1.1,<0.2.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: datasets (>=2.13.0,<3.0.0); extra == "datasets"
 Requires-Dist: fastapi (>=0.96.0,<0.97.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0); extra == "datasets"
 Requires-Dist: pandas (>=2.0.2,<3.0.0); extra == "datasets"
-Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
+Requires-Dist: psycopg2 (>=2.9.6,<3.0.0); extra == "database"
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # lassen
 
 **40.4881° N, 121.5049° W**
```

