# Comparing `tmp/pydiverse_pipedag-0.4.0.tar.gz` & `tmp/pydiverse_pipedag-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse_pipedag-0.4.0.tar", max compression
+gzip compressed data, was "pydiverse_pipedag-0.4.1.tar", max compression
```

## Comparing `pydiverse_pipedag-0.4.0.tar` & `pydiverse_pipedag-0.4.1.tar`

### file list

```diff
@@ -1,50 +1,57 @@
--rw-r--r--   0        0        0     1517 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/LICENSE
--rw-r--r--   0        0        0     7260 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/docs/package/README.md
--rw-r--r--   0        0        0     3059 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       13 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      313 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      749 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       88 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     5334 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0    10562 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/lock.py
--rw-r--r--   0        0        0      177 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    20296 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0     7267 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0    82994 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/sql.py
--rw-r--r--   0        0        0       45 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     1274 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py
--rw-r--r--   0        0        0      456 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/util/pandas.py
--rw-r--r--   0        0        0    40457 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/util/sql_ddl.py
--rw-r--r--   0        0        0    12122 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table_cache.py
--rw-r--r--   0        0        0      342 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0     8079 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    25913 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      219 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0    13470 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/config.py
--rw-r--r--   0        0        0     9204 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     2544 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     5665 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     6360 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      285 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      648 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     6516 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1380 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1079 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0      124 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     8908 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0     5422 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0     7855 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     2039 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    17644 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0       37 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/util/__init__.py
--rw-r--r--   0        0        0     1104 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/util/cache.py
--rw-r--r--   0        0        0     4231 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/util/json.py
--rw-r--r--   0        0        0      177 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0     2061 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1435 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      880 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     2927 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     9283 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0     1553 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     2811 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/structlog.py
--rw-r--r--   0        0        0     8747 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-06-17 05:57:06.114336 pydiverse_pipedag-0.4.1/LICENSE
+-rw-r--r--   0        0        0     7229 2023-06-17 05:57:06.114336 pydiverse_pipedag-0.4.1/docs/package/README.md
+-rw-r--r--   0        0        0     3037 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      355 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      749 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       88 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     5334 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0      357 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/lock/__init__.py
+-rw-r--r--   0        0        0     6097 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/lock/base.py
+-rw-r--r--   0        0        0    11773 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/lock/database.py
+-rw-r--r--   0        0        0     2541 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/lock/filelock.py
+-rw-r--r--   0        0        0      768 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/lock/nolock.py
+-rw-r--r--   0        0        0     3671 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/lock/zookeeper.py
+-rw-r--r--   0        0        0        0 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/lock.py
+-rw-r--r--   0        0        0      177 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    20296 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0     7267 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0    83022 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/sql.py
+-rw-r--r--   0        0        0       45 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     1274 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py
+-rw-r--r--   0        0        0      456 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/util/pandas.py
+-rw-r--r--   0        0        0    40457 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/util/sql_ddl.py
+-rw-r--r--   0        0        0    12122 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table_cache.py
+-rw-r--r--   0        0        0      342 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0     8231 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    25913 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      219 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0    13669 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/core/config.py
+-rw-r--r--   0        0        0     9325 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     2551 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     5626 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     6568 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      332 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      648 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     2818 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/engine/dask.py
+-rw-r--r--   0        0        0     6516 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1380 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1079 2023-06-17 05:57:06.118336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     8908 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0     5422 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0     7855 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     2039 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    17644 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0       37 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/util/__init__.py
+-rw-r--r--   0        0        0     1104 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/util/cache.py
+-rw-r--r--   0        0        0     4222 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/util/json.py
+-rw-r--r--   0        0        0      177 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0     2061 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1435 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      880 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     2927 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     7992 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0     1553 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     2811 2023-06-17 05:57:06.122336 pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/structlog.py
+-rw-r--r--   0        0        0     8788 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.4.1/PKG-INFO
```

### Comparing `pydiverse_pipedag-0.4.0/LICENSE` & `pydiverse_pipedag-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/docs/package/README.md` & `pydiverse_pipedag-0.4.1/docs/package/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pydiverse.pipedag
 
-[![CI](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml/badge.svg)](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml)
+[![CI](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/tests.yml/badge.svg)](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/tests.yml)
 
 A pipeline orchestration library executing tasks within one python session. It takes care of SQL table
 (de)materialization, caching and cache invalidation. Blob storage is supported as well for example
 for storing model files.
 
 This is an early stage version 0.x which lacks documentation. Please contact
 https://github.com/orgs/pydiverse/teams/code-owners if you like to become an early adopter
@@ -16,42 +16,47 @@
 with `conda install pydiverse-pipedag -c conda-forge`.
 
 ## Example
 
 A flow can look like this (i.e. put this in a file named `run_pipeline.py`):
 
 ```python
-from pydiverse.pipedag import materialize, Table, Flow, Stage
-import sqlalchemy as sa
 import pandas as pd
+import sqlalchemy as sa
 
-from pydiverse.pipedag.context import StageLockContext, RunContext
+from pydiverse.pipedag import Flow, Stage, Table, materialize
+from pydiverse.pipedag.context import StageLockContext
 
 
 @materialize(lazy=True)
 def lazy_task_1():
-    return sa.select([sa.literal(1).label("x"), sa.literal(2).label("y")])
+    return sa.select(
+        sa.literal(1).label("x"),
+        sa.literal(2).label("y"),
+    )
 
 
 @materialize(lazy=True, input_type=sa.Table)
 def lazy_task_2(input1: sa.Table, input2: sa.Table):
-    query = sa.select([(input1.c.x * 5).label("x5"), input2.c.a]).select_from(
-        input1.outerjoin(input2, input2.c.x == input1.c.x)
-    )
+    query = sa.select(
+        (input1.c.x * 5).label("x5"),
+        input2.c.a,
+    ).select_from(input1.outerjoin(input2, input2.c.x == input1.c.x))
+
     return Table(query, name="task_2_out", primary_key=["a"])
 
 
 @materialize(lazy=True, input_type=sa.Table)
-def lazy_task_3(input: sa.Table, my_stage: Stage):
-    return sa.text(f"SELECT * FROM {my_stage.transaction_name}.{input.name}")
+def lazy_task_3(input1: sa.Table):
+    return sa.text(f"SELECT * FROM {input1.original.schema}.{input1.name}")
 
 
 @materialize(lazy=True, input_type=sa.Table)
-def lazy_task_4(input: sa.Table, prev_stage: Stage):
-    return sa.text(f"SELECT * FROM {prev_stage.name}.{input.name}")
+def lazy_task_4(input1: sa.Table):
+    return sa.text(f"SELECT * FROM {input1.original.schema}.{input1.name}")
 
 
 @materialize(nout=2, version="1.0.0")
 def eager_inputs():
     dfA = pd.DataFrame(
         {
             "a": [0, 1, 2, 4],
@@ -74,21 +79,21 @@
 
 def main():
     with Flow() as f:
         with Stage("stage_1"):
             lazy_1 = lazy_task_1()
             a, b = eager_inputs()
 
-        with Stage("stage_2") as stage2:
+        with Stage("stage_2"):
             lazy_2 = lazy_task_2(lazy_1, b)
-            lazy_3 = lazy_task_3(lazy_2, stage2)
+            lazy_3 = lazy_task_3(lazy_2)
             eager = eager_task(lazy_1, b)
 
         with Stage("stage_3"):
-            lazy_4 = lazy_task_4(lazy_2, stage2)
+            lazy_4 = lazy_task_4(lazy_2)
         _ = lazy_3, lazy_4, eager  # unused terminal output tables
 
     # Run flow
     result = f.run()
     assert result.successful
 
     # Run in a different way for testing
```

### Comparing `pydiverse_pipedag-0.4.0/pyproject.toml` & `pydiverse_pipedag-0.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-pipedag"
-version = "0.4.0"
+version = "0.4.1"
 description = "A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files."
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
@@ -34,50 +34,51 @@
 python-box = ">=6.1.0"
 PyYAML = ">=6.0"
 pyarrow = ">=11.0.0"
 cryptography = ">=41.0.1"
 
 filelock = { version = ">=3.7.1", optional = true }
 kazoo = { version = ">=2.8.0", optional = true }
+dask = { version = ">=2022.1.0", optional = true }
+
 
 [tool.poetry.extras]
 filelock = ["filelock"]
 zookeeper = ["kazoo"]
-#mssql = ["pyodbc", "pytsql"]
-#ibm_db2 = ["ibm-db", "ibm-db-sa"]
-#pdtransform = ["pydiverse-transform"]
-#ibis = ["ibis", "ibis-framework"]
-#polars = ["tidypolars", "polars", "connectorx"]
-#prefect = ["prefect", "docker-compose"]
+dask = ["dask"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.2.0"
 pytest-mock = ">=3.10.0"
 pytest-timeout = ">=2.1.0"
 
 black = { version = "23.3.0", extras = ["d"] }
 isort = "^5.10.1"
 ruff = "^0.0.270"
 pre-commit = ">=2.20.0"
 
 kazoo = ">=2.8.0"
+dask = ">=2022.1.0"
 psycopg2 = ">=2.9.3"
 pydot = ">=1.4.2"
 
-[tool.poetry.group.test]
+[tool.poetry.group.tests]
 optional = true
 
-[tool.poetry.group.test.dependencies]
+[tool.poetry.group.tests.dependencies]
 # Table Hooks
 pydiverse-transform = "^0.1.0"
 ibis = ">=3.2.0"
 ibis-framework = { version = ">=5.1.0", extras = ["mssql", "postgres"] }
 polars = ">=0.16.18"
 tidypolars = { version = "^0.2.19", python = "<3.11" }
-connectorx = { version = ">=0.3.1", python = "<3.11" }
+connectorx = [
+    { version = ">=0.3.1", python = "<3.11" },
+    { version = "0.3.2a5", python = "==3.11" }  # Latest full release is broken - unpin when 0.3.2 released
+]
 # Engines
 prefect = "^1.3"
 # MSSQL
 pyodbc = ">=4.0.35"
 pytsql = ">=1.1.4"
 # IBM DB2
 ibm-db = { version = ">=3.1.4", markers="platform_machine == 'x86_64'" }
```

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/_typing.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/_typing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/blob.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/blob.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/sql.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     Uses schema swapping for transactions:
     Creates a schema for each stage and a temporary schema for each
     transaction. If all tasks inside a stage succeed, swaps the schemas by
     renaming them.
     """
 
     METADATA_SCHEMA = "pipedag_metadata"
+    LOCK_SCHEMA = "pipedag_locks"
 
     @classmethod
     def _init_conf_(cls, config: dict[str, Any]):
         config = config.copy()
         engine_url = config.pop("url")
         return cls(engine_url, **config)
 
@@ -122,16 +123,15 @@
         self.pytsql_isolate_top_level_statements = pytsql_isolate_top_level_statements
         self.print_materialize = print_materialize
         self.print_sql = print_sql
         self.no_db_locking = no_db_locking
         self.metadata_schema = self.get_schema(self.METADATA_SCHEMA)
 
         self._init_database(engine_url, create_database_if_not_exists)
-        self.engine_url_obj = sa.engine.make_url(engine_url)
-        self.engine_url_no_pw = repr(self.engine_url_obj)
+        self.engine_url = sa.engine.make_url(engine_url)
         self.engine = self._connect(engine_url, self.schema_prefix, self.schema_suffix)
         self.engines_other = dict()  # i.e. for IBIS connection
 
         # Set up metadata tables and schema
         from sqlalchemy import CLOB, BigInteger, Boolean, Column, DateTime, String
 
         if self.engine.dialect.name == "ibm_db_sa":
@@ -206,15 +206,15 @@
             Column("task_hash", String(32)),
             Column("in_transaction_schema", Boolean),
             schema=self.metadata_schema.get(),
         )
 
         self.logger.info(
             "Initialized SQL Table Store",
-            engine_url=self.engine_url_no_pw,
+            engine_url=self.engine_url.render_as_string(hide_password=True),
             schema_prefix=self.schema_prefix,
             schema_suffix=self.schema_suffix,
         )
 
     @staticmethod
     def _init_database(engine_url: str, create_database_if_not_exists: bool):
         if not create_database_if_not_exists:
@@ -792,14 +792,15 @@
         # Call schema swap function with updated transaction name
         self._init_stage_schema_swap(stage)
 
     def commit_stage(self, stage: Stage):
         # If the stage is 100% cache valid, then we just need to update the
         # "in_transaction_schema" column of the metadata tables.
         if not RunContext.get().has_stage_changed(stage):
+            self.logger.info("Stage is cache valid", stage=stage)
             with self.engine_connect() as conn:
                 self._commit_stage_update_metadata(stage, conn)
             return
 
         # Commit normally
         stage_commit_technique = ConfigContext.get().stage_commit_technique
         if stage_commit_technique == StageCommitTechnique.SCHEMA_SWAP:
@@ -1480,14 +1481,22 @@
                 .where(self.tasks_table.c.stage == stage.name)
                 .where(self.tasks_table.c.in_transaction_schema.in_([False]))
                 .order_by(self.tasks_table.c.output_json)
             ).all()
             result = [row[0] for row in result]
         return compute_cache_key(*result)
 
+    # DatabaseLockManager
+
+    def get_engine_for_locking(self) -> sa.Engine:
+        return self._connect(self.engine_url, self.schema_prefix, self.schema_suffix)
+
+    def get_lock_schema(self) -> Schema:
+        return self.get_schema(self.LOCK_SCHEMA)
+
 
 @SQLTableStore.register_table()
 class SQLAlchemyTableHook(TableHook[SQLTableStore]):
     @classmethod
     def can_materialize(cls, type_) -> bool:
         return issubclass(
             type_, (sa.sql.elements.TextClause, sa.sql.selectable.Selectable)
@@ -1584,15 +1593,15 @@
 
     # we need to resolve aliases since pandas.read_sql_table does not work for them
     # and sa.Table does not auto-reflect columns
     table_name = ibm_db_sa_fix_name(table_name)
     schema = ibm_db_sa_fix_name(schema)
     tbl = sa.Table("SYSTABLES", sa.MetaData(), schema="SYSIBM", autoload_with=conn)
     query = (
-        sa_select([tbl.c.base_name, tbl.c.base_schema])
+        sa.select(tbl.c.base_name, tbl.c.base_schema)
         .select_from(tbl)
         .where(
             (tbl.c.creator == schema) & (tbl.c.name == table_name) & (tbl.c.TYPE == "A")
         )
     )
     for retry_iteration in range(4):
         # retry operation since it might have been terminated as a deadlock victim
@@ -1799,15 +1808,15 @@
                         autoload_with=store.engine,
                     ).alias("tbl")
                     dtype_map = {c.name: cls._pandas_type(c.type) for c in sql_table.c}
                     cols, year_cols = cls._fix_cols(
                         {c.name: c for c in sql_table.c}, store.engine.dialect.name
                     )
                     dtype_map.update({col: pd.Int16Dtype() for col in year_cols})
-                    query = sa_select(cols.values()).select_from(sql_table)
+                    query = sa.select(*cols.values()).select_from(sql_table)
                     try:
                         # works only from pandas 2.0.0 on
                         df = pd.read_sql(
                             query,
                             con=conn,
                             dtype=dtype_map,
                         )
@@ -1857,15 +1866,16 @@
         table: Table[polars.dataframe.DataFrame],
         stage_name,
         task_info: TaskInfo | None,
     ):
         schema = store.get_schema(stage_name)
         if store.print_materialize:
             store.logger.info(
-                f"Writing table '{schema.get()}.{table.name}':\n{table.obj}"
+                f"Writing table '{schema.get()}.{table.name}'",
+                table_obj=table.obj,
             )
         table_name = table.name
         # TODO:
         # dtype_map = {}
         # if store.engine.dialect.name == "ibm_db_sa":
         #     # Default string target is CLOB which can't be used for indexing.
         #     # We could use VARCHAR(32000), but if we change this to VARCHAR(256)
@@ -1888,16 +1898,18 @@
         stage_name: str,
         as_type: type[polars.dataframe.DataFrame],
         namer: NameDisambiguator | None = None,
     ) -> polars.dataframe.DataFrame:
         schema = store.get_schema(stage_name).get()
         table_name = table.name
         table_name, schema = store.resolve_aliases(table_name, schema)
-        conn = str(store.engine_url_obj)
-        df = polars.read_database(f'SELECT * FROM {schema}."{table_name}"', conn)
+        connection_uri = store.engine_url.render_as_string(hide_password=False)
+        df = polars.read_database(
+            f'SELECT * FROM {schema}."{table_name}"', connection_uri
+        )
         return df
 
     @classmethod
     def auto_table(cls, obj: polars.dataframe.DataFrame):
         # currently, we don't know how to store a table name inside polars dataframe
         return super().auto_table(obj)
 
@@ -1926,16 +1938,16 @@
         store,
         table: Table[tidypolars.Tibble],
         stage_name,
         task_info: TaskInfo | None,
     ):
         t = table.obj
         table = table.copy_without_obj()
-        table.obj = t.obj.to_polars()
-        PolarsTableHook.materialize(store, t, stage_name, task_info)
+        table.obj = t.to_polars()
+        PolarsTableHook.materialize(store, table, stage_name, task_info)
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
@@ -2030,29 +2042,27 @@
             return str(query)
         return super().lazy_query_str(store, obj)
 
 
 try:
     # optional dependency to ibis
     import ibis
-    import ibis.expr.types as ibis_types
 except ImportError as e:
     warnings.warn(str(e), ImportWarning)
     ibis = None
-    ibis_types = None
 
 
 @SQLTableStore.register_table(ibis)
 class IbisTableHook(TableHook[SQLTableStore]):
     @staticmethod
     def get_con(store):
         # TODO: move this function to a better ibis specific place
         con = store.engines_other.get("ibis")
         if con is None:
-            url = store.engine_url_obj
+            url = store.engine_url
             dialect = store.engine.dialect.name
             if dialect == "postgresql":
                 con = ibis.postgres.connect(
                     host=url.host,
                     user=url.username,
                     password=url.password,
                     port=url.port,
@@ -2073,42 +2083,42 @@
                 )
             store.engines_other["ibis"] = con
         return con
 
     @classmethod
     def can_materialize(cls, type_) -> bool:
         # Operations on a table like mutate() or join() don't change the type
-        return issubclass(type_, ibis_types.Table)
+        return issubclass(type_, ibis.expr.types.Table)
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
-        return issubclass(type_, ibis_types.Table)
+        return issubclass(type_, ibis.expr.types.Table)
 
     @classmethod
     def materialize(
         cls,
         store,
-        table: Table[ibis_types.Table],
+        table: Table[ibis.expr.types.Table],
         stage_name,
         task_info: TaskInfo | None,
     ):
         t = table.obj
         table = table.copy_without_obj()
         table.obj = sa.text(cls.lazy_query_str(store, t))
         return SQLAlchemyTableHook.materialize(store, table, stage_name, task_info)
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
-        as_type: type[ibis_types.Table],
+        as_type: type[ibis.expr.types.Table],
         namer: NameDisambiguator | None = None,
-    ) -> ibis_types.Table:
+    ) -> ibis.expr.types.Table:
         con = cls.get_con(store)
         table_name = table.name
         schema = store.get_schema(stage_name).get()
         table_name, schema = store.resolve_aliases(table_name, schema)
         for retry_iteration in range(4):
             # retry operation since it might have been terminated as a deadlock victim
             try:
@@ -2117,31 +2127,21 @@
                     schema=schema,
                 )
                 break
             except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
                 if retry_iteration == 3:
                     raise
                 time.sleep(retry_iteration * retry_iteration * 1.2)
+        else:
+            raise Exception
         return tbl
 
     @classmethod
-    def auto_table(cls, obj: ibis_types.Table):
+    def auto_table(cls, obj: ibis.expr.types.Table):
         if obj.has_name():
             return Table(obj, obj.get_name())
         else:
             return super().auto_table(obj)
 
     @classmethod
-    def lazy_query_str(cls, store, obj: ibis_types.Table) -> str:
+    def lazy_query_str(cls, store, obj: ibis.expr.types.Table) -> str:
         return str(ibis.to_sql(obj, cls.get_con(store).name))
-
-
-def sa_select(*args, **kwargs):
-    """Run sa.select in 'old' way compatible with sqlalchemy>=2.0."""
-    try:
-        return sa.select(*args, **kwargs)
-    except sa.exc.ArgumentError:
-        if len(args) == 1 and isinstance(args[0], Iterable) and len(kwargs) == 0:
-            # for sqlalchemy 2.0, we need to unpack columns
-            return sa.select(*args[0])
-        else:
-            raise
```

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/util/sql_ddl.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table/util/sql_ddl.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table_cache.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/backend/table_cache.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/context/context.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/context/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,14 +131,18 @@
     stage_commit_technique: StageCommitTechnique
     network_interface: str
     attrs: dict[str, Any]
 
     # other configuration options
     ignore_fresh_input: bool = False
 
+    # INTERNAL FLAGS - ONLY FOR PIPEDAG USE
+    # When set to True, exceptions raised in a flow don't get logged
+    _swallow_exceptions: bool = False
+
     @cached_property
     def auto_table(self) -> tuple[type, ...]:
         return tuple(map(import_object, self.config_dict.get("auto_table", ())))
 
     @cached_property
     def auto_blob(self) -> tuple[type, ...]:
         return tuple(map(import_object, self.config_dict.get("auto_blob", ())))
```

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/context/run_context.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/context/run_context.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/config.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,29 +172,31 @@
             instance_id=config["instance_id"],
             stage_commit_technique=stage_commit_technique,
             fail_fast=config["fail_fast"],
             network_interface=config["network_interface"],
             attrs=Box(config["attrs"], frozen_box=True),
         )
 
-        try:
-            # Make sure @cached_property store is set up and loaded
-            # and throw config errors early.
-            with config_context:
-                _ = config_context.store
-                _ = config_context.auto_table
-                _ = config_context.auto_blob
+        if "PYDIVERSE_PIPEDAG_PYTEST" not in os.environ:
+            # If we're running test cases, this can be skipped to improve performance
+            try:
+                # Make sure @cached_property store is set up and loaded
+                # and throw config errors early.
+                with config_context:
+                    _ = config_context.store
+                    _ = config_context.auto_table
+                    _ = config_context.auto_blob
 
-                config_context.create_orchestration_engine().dispose()
-                config_context.create_lock_manager().dispose()
-        except Exception as e:
-            raise RuntimeError(
-                "Error while creating backend objects from pipedag config "
-                f"(instance={instance}, flow={flow}): {self.path}"
-            ) from e
+                    config_context.create_orchestration_engine().dispose()
+                    config_context.create_lock_manager().dispose()
+            except Exception as e:
+                raise RuntimeError(
+                    "Error while creating backend objects from pipedag config "
+                    f"(instance={instance}, flow={flow}): {self.path}"
+                ) from e
 
         return config_context
 
     def __get_merged_config_dict(self, instance, flow, default=None):
         search_paths = [
             ("instances", "__any__"),
             ("instances", instance),
```

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/flow.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/core/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import warnings
 from collections import defaultdict
 from typing import TYPE_CHECKING
 
 import networkx as nx
 import structlog
 
 from pydiverse.pipedag.context import ConfigContext, DAGContext, RunContextServer
@@ -232,15 +233,17 @@
             check for fresh input into pipe-DAG
         :param kwargs: Other keyword arguments. They get passed on directly to the
             orchestration engine's `.run` method and thus are engine dependant.
         :return:
             Result object that gives information whether run was successful
         """
 
-        # TODO: implement running only a subset of stages (see parameter stages)
+        if stages is not None:
+            # TODO: implement running only a subset of stages (see parameter stages)
+            warnings.warn("flow.run(stages=...) isn't yet supported")
 
         # Get the ConfigContext to use
         if config_context is None:
             try:
                 config_context = ConfigContext.get()
             except LookupError:
                 config_context = PipedagConfig.default.get()
```

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/result.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/core/result.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 @frozen
 class Result:
     underlying: Any
     successful: bool
     config_context: ConfigContext | None
 
     task_values: dict[Task, Any]
-    exception: Exception = None
+    exception: Exception | None = None
 
     def get(self, task: Task | TaskGetItem, as_type: type = None) -> Materializable:
         """Load the results of a task from the database.
 
         :param task: The task
         :param as_type: The type as which tables produced by this task should
             be dematerialized. If no type is specified, the input type of
```

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/stage.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/core/stage.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,15 +149,14 @@
             outer = outer.outer_stage
         return False
 
     def __getstate__(self):
         state = self.__dict__.copy()
         state.pop("tasks", None)
         state.pop("commit_task", None)
-        state.pop("outer_stage", None)
         state.pop("logger", None)
         return state
 
 
 class CommitStageTask(Task):
     def __init__(self, stage: Stage, flow: Flow):
         super().__init__(
```

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/task.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/core/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,19 @@
         if config_context is None:
             config_context = ConfigContext.get()
 
         with run_context, config_context:
             try:
                 result = self._run(inputs)
             except Exception as e:
-                self.logger.exception("Task failed (raised an exception)")
+                if config_context._swallow_exceptions:
+                    # PIPEDAG INTERNAL
+                    self.logger.info("Task failed (raised an exception)", cause=str(e))
+                else:
+                    self.logger.exception("Task failed (raised an exception)")
                 self.did_finish(FinalTaskState.FAILED)
                 raise e
             else:
                 self.did_finish(FinalTaskState.COMPLETED)
                 return result
 
     def _run(self, inputs: [int, Any]):
```

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/base.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/sequential.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/engine/sequential.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/cache.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/cache.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/container.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/container.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/core.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/core.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/store.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/store.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/util/cache.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/util/cache.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/util/json.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/materialize/util/json.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         }
     if isinstance(o, dt.datetime):
         return {
             PIPEDAG_TYPE: PIPEDAG_TYPE_DATETIME,
             "datetime": o.isoformat(),
         }
 
-    raise TypeError(f"Object of type {type(o).__name__} is not JSON serializable")
+    raise TypeError(f"Object of type {type(o)} is not JSON serializable")
 
 
 def json_object_hook(d: dict):
     """Decode json with `Table` and `Blob` objects"""
     pipedag_type = d.get(PIPEDAG_TYPE)
     if pipedag_type:
         run_context = RunContext.get()
```

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/disposable.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/disposable.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/import_.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/import_.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/ipc.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/ipc.py`

 * *Files 22% similar despite different names*

```diff
@@ -38,132 +38,119 @@
 
         self.socket = pynng.Rep0(listen=listen, recv_timeout=recv_timeout)
         self.nonces = set()
 
         self._fernet = Fernet(Fernet.generate_key())
 
         self.__stop_flag = False
-        self.__thread = None
-        self.logger = structlog.get_logger(logger_name=type(self).__name__)
+        self.logger = structlog.get_logger(
+            logger_name=type(self).__name__, address=self.address
+        )
 
         self.msg_default = msg_default
         self.msg_ext_hook = msg_ext_hook
 
-    def _get_id(self, ctx_id=0):
-        return dict(
-            address=self.address,
-            thread=threading.get_ident(),
-            ctx_id=ctx_id,
-        )
-
     def run(self):
-        self.logger.info("Starting IPCServer", **self._get_id())
+        self.logger.info("Starting IPCServer")
         self.run_loop()
 
     def stop(self):
         self.__stop_flag = True
-        self.logger.debug("Request IPCServer to stop", **self._get_id())
+        self.logger.debug("Request IPCServer to stop")
 
     def __enter__(self):
-        self.__thread = self
-        self.__thread.start()
-        self.logger.debug("Started IPCServer thread", thread=self.__thread.ident)
+        self.start()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stop()
-        if self.__thread is not None:
-            self.logger.debug("Stop IPCServer thread", thread=self.__thread.ident)
-            self.__thread.join()
+        self.join()
 
     def run_loop(self):
-        """
-        Run main loop for responding to client requests to this server process.
+        context = None
+        context_id = 0
+
+        threads = set()
+        active_threads = 0
 
-        We rely on a fixed request-response pattern of pynng library (Req0/Rep0)
-        which requires us to open a context for every request-response pair.
-        We create threads for determining and sending responses and we keep 10
-        such threads in-flight. At the end we join all 10 threads even though
-        some threads might actually already have completed and may even share the
-        same ident number. We log thread IDs as hash(thread.ident) % 100 for
-        receiving human processable numbers.
-        """
-        max_threads_in_flight = 10  # keep up to 10 threads in flight
-
-        socket = None
-        ctx_id = 0
-        threads = []
         try:
-            socket = self.socket.new_context()
-            ctx_id += 1
-            self.logger.debug("New socket context", **self._get_id(ctx_id))
+            context = self.socket.new_context()
+            context_id += 1
+
             while not self.__stop_flag:
-                # noinspection PyBroadException
                 try:
-                    data = socket.recv()
+                    data = context.recv()
                     data = self._fernet.decrypt(data)
                     unpacker = msgpack.Unpacker(
                         use_list=False, ext_hook=self.msg_ext_hook
                     )
                     unpacker.feed(data)
 
                     # Expected: (NONCE, PAYLOAD)
                     if unpacker.read_array_header() != 2:
                         raise IPCError(
                             "Expected request to contain exactly two fields:"
                             " nonce and payload."
                         )
+
                     nonce = unpacker.unpack()
                     nonce_hex = nonce.hex()
 
                     if nonce in self.nonces:
                         # Already processing this request
                         self.logger.warning(
                             "Already processing request",
                             nonce=nonce_hex,
-                            **self._get_id(ctx_id),
                         )
-                        socket = self.socket.new_context()
-                        ctx_id += 1
-                        self.logger.debug("Next socket context", **self._get_id(ctx_id))
-                        continue
 
-                    self.nonces.add(nonce)
+                        context = self.socket.new_context()
+                        context_id += 1
+                        continue
 
-                    if len(threads) >= max_threads_in_flight:
-                        self.logger.debug("Joining thread", thread=threads[0].ident)
-                        threads[0].join()
-                        del threads[0]
                     thread_logger = structlog.get_logger(
-                        logger_name="IPC Worker", nonce=nonce_hex, ctx_id=ctx_id
+                        logger_name="IPC Worker", nonce=nonce_hex, id=context_id
                     )
                     thread = threading.Thread(
                         name="IPC Worker",
                         target=self._serve,
-                        args=[thread_logger, socket, unpacker],
+                        args=[thread_logger, context, unpacker],
                         daemon=True,
                     )
-                    socket = self.socket.new_context()
-                    ctx_id += 1
-                    self.logger.debug("next socket context", **self._get_id(ctx_id))
-                    threads.append(thread)
+
                     thread.start()
+                    threads.add(thread)
+
+                    context = self.socket.new_context()
+                    context_id += 1
                 except pynng.Timeout:
                     pass
                 except Exception:
                     self.logger.exception("Exception occurred in run_loop")
+
+                # Clear list of active threads
+                if len(threads) >= active_threads + 25:
+                    active_threads = 0
+                    for thread in list(threads):
+                        if thread.is_alive():
+                            active_threads += 1
+                        else:
+                            self.logger.debug("Joining thread", thread=thread.ident)
+                            thread.join()
+                            threads.remove(thread)
+
         finally:
+            if context is not None:
+                context.close()  # close the open request-response context
+
             for thread in threads:
                 self.logger.debug("Joining thread", thread=thread.ident)
                 thread.join()
-            self.logger.debug("Closing socket", **self._get_id())
-            if socket is not None:
-                socket.close()  # close the open request-response context
+
             self.socket.close()
-            self.logger.info("Stopped IPCServer", **self._get_id())
+            self.logger.info("Stopped IPCServer")
 
     def _serve(self, thread_logger, socket: pynng.Socket, unpacker):
         try:
             msg = unpacker.unpack()
             thread_logger.debug(
                 "IPCServer Received",
                 message=msg,
@@ -179,14 +166,15 @@
             reply = self._fernet.encrypt(reply)
         except Exception as e:
             thread_logger.critical("Uncaught exception in _serve", exc_info=e)
             reply = b""
 
         try:
             socket.send(reply)
+            socket.close()
         except Exception:
             thread_logger.exception("Failed to send reply")
 
     def handle_request(self, request: dict[str, Any]):
         return None
 
     @cached_property
@@ -214,43 +202,40 @@
             msg_default=self.msg_default,
             msg_ext_hook=self.msg_ext_hook,
         )
 
 
 class IPCClient:
     def __init__(self, addr: str, fernet: Fernet, msg_default=None, msg_ext_hook=None):
-        self.logger = structlog.get_logger(
-            logger_name=type(self).__name__,
-            thread=threading.get_ident(),
-        )
+        self.logger = structlog.get_logger(logger_name=type(self).__name__)
         self.addr = addr
         self._fernet = fernet
         self.msg_default = msg_default
         self.msg_ext_hook = msg_ext_hook
 
         self.socket = self._connect()
 
     def _connect(self):
         self.logger.debug("Opening client connection", addr=self.addr)
         return pynng.Req0(dial=self.addr, resend_time=30_000)
 
     def request(self, payload: Any) -> Any:
         with self.socket.new_context() as socket:
-            self.logger.debug("Client request")
+            self.logger.debug("Client request", payload=payload)
             nonce = uuid.uuid4().bytes[:16]
             msg = msgpack.packb((nonce, payload), default=self.msg_default)
             msg = self._fernet.encrypt(msg)
             socket.send(msg)
 
             response = socket.recv()
-            self.logger.debug("Client got response")
             response = self._fernet.decrypt(response)
             response = msgpack.unpackb(
                 response, use_list=False, ext_hook=self.msg_ext_hook
             )
+            self.logger.debug("Client got response", response=response)
             return response
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state["socket"]
         return state
```

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/naming.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/naming.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/structlog.py` & `pydiverse_pipedag-0.4.1/src/pydiverse/pipedag/util/structlog.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.4.0/PKG-INFO` & `pydiverse_pipedag-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.4.0
+Version: 0.4.1
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
+Provides-Extra: dask
 Provides-Extra: filelock
 Provides-Extra: zookeeper
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: SQLAlchemy (>=1.4.39)
 Requires-Dist: attrs (>=22.1.0)
 Requires-Dist: cryptography (>=41.0.1)
+Requires-Dist: dask (>=2022.1.0) ; extra == "dask"
 Requires-Dist: filelock (>=3.7.1) ; extra == "filelock"
 Requires-Dist: kazoo (>=2.8.0) ; extra == "zookeeper"
 Requires-Dist: msgpack (>=1.0.4)
 Requires-Dist: networkx (>=2.8)
 Requires-Dist: packaging (>=21.3)
 Requires-Dist: pandas (>=1.4.3)
 Requires-Dist: pyarrow (>=11.0.0)
@@ -32,15 +34,15 @@
 Requires-Dist: python-box (>=6.1.0)
 Requires-Dist: structlog (>=22.1.0)
 Requires-Dist: typing-extensions (>=4.1.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # pydiverse.pipedag
 
-[![CI](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml/badge.svg)](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml)
+[![CI](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/tests.yml/badge.svg)](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/tests.yml)
 
 A pipeline orchestration library executing tasks within one python session. It takes care of SQL table
 (de)materialization, caching and cache invalidation. Blob storage is supported as well for example
 for storing model files.
 
 This is an early stage version 0.x which lacks documentation. Please contact
 https://github.com/orgs/pydiverse/teams/code-owners if you like to become an early adopter
@@ -52,42 +54,47 @@
 with `conda install pydiverse-pipedag -c conda-forge`.
 
 ## Example
 
 A flow can look like this (i.e. put this in a file named `run_pipeline.py`):
 
 ```python
-from pydiverse.pipedag import materialize, Table, Flow, Stage
-import sqlalchemy as sa
 import pandas as pd
+import sqlalchemy as sa
 
-from pydiverse.pipedag.context import StageLockContext, RunContext
+from pydiverse.pipedag import Flow, Stage, Table, materialize
+from pydiverse.pipedag.context import StageLockContext
 
 
 @materialize(lazy=True)
 def lazy_task_1():
-    return sa.select([sa.literal(1).label("x"), sa.literal(2).label("y")])
+    return sa.select(
+        sa.literal(1).label("x"),
+        sa.literal(2).label("y"),
+    )
 
 
 @materialize(lazy=True, input_type=sa.Table)
 def lazy_task_2(input1: sa.Table, input2: sa.Table):
-    query = sa.select([(input1.c.x * 5).label("x5"), input2.c.a]).select_from(
-        input1.outerjoin(input2, input2.c.x == input1.c.x)
-    )
+    query = sa.select(
+        (input1.c.x * 5).label("x5"),
+        input2.c.a,
+    ).select_from(input1.outerjoin(input2, input2.c.x == input1.c.x))
+
     return Table(query, name="task_2_out", primary_key=["a"])
 
 
 @materialize(lazy=True, input_type=sa.Table)
-def lazy_task_3(input: sa.Table, my_stage: Stage):
-    return sa.text(f"SELECT * FROM {my_stage.transaction_name}.{input.name}")
+def lazy_task_3(input1: sa.Table):
+    return sa.text(f"SELECT * FROM {input1.original.schema}.{input1.name}")
 
 
 @materialize(lazy=True, input_type=sa.Table)
-def lazy_task_4(input: sa.Table, prev_stage: Stage):
-    return sa.text(f"SELECT * FROM {prev_stage.name}.{input.name}")
+def lazy_task_4(input1: sa.Table):
+    return sa.text(f"SELECT * FROM {input1.original.schema}.{input1.name}")
 
 
 @materialize(nout=2, version="1.0.0")
 def eager_inputs():
     dfA = pd.DataFrame(
         {
             "a": [0, 1, 2, 4],
@@ -110,21 +117,21 @@
 
 def main():
     with Flow() as f:
         with Stage("stage_1"):
             lazy_1 = lazy_task_1()
             a, b = eager_inputs()
 
-        with Stage("stage_2") as stage2:
+        with Stage("stage_2"):
             lazy_2 = lazy_task_2(lazy_1, b)
-            lazy_3 = lazy_task_3(lazy_2, stage2)
+            lazy_3 = lazy_task_3(lazy_2)
             eager = eager_task(lazy_1, b)
 
         with Stage("stage_3"):
-            lazy_4 = lazy_task_4(lazy_2, stage2)
+            lazy_4 = lazy_task_4(lazy_2)
         _ = lazy_3, lazy_4, eager  # unused terminal output tables
 
     # Run flow
     result = f.run()
     assert result.successful
 
     # Run in a different way for testing
```

