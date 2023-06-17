# Comparing `tmp/kedro_ibis_dataset-0.0.6a3.tar.gz` & `tmp/kedro_ibis_dataset-0.0.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_ibis_dataset-0.0.6a3.tar", last modified: Sat Jun 17 00:59:47 2023, max compression
+gzip compressed data, was "kedro_ibis_dataset-0.0.6b1.tar", last modified: Sat Jun 17 10:42:53 2023, max compression
```

## Comparing `kedro_ibis_dataset-0.0.6a3.tar` & `kedro_ibis_dataset-0.0.6b1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       55 2023-06-16 19:34:49.301187 kedro_ibis_dataset-0.0.6a3/README.md
--rw-r--r--   0        0        0      683 2023-06-17 00:59:47.794857 kedro_ibis_dataset-0.0.6a3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 23:01:44.746383 kedro_ibis_dataset-0.0.6a3/src/kedro_ibis_dataset/__init__.py
--rw-r--r--   0        0        0     2448 2023-06-16 23:07:41.966063 kedro_ibis_dataset-0.0.6a3/src/kedro_ibis_dataset/kedro_ibis_dataset.py
--rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 kedro_ibis_dataset-0.0.6a3/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-06-16 19:34:49.301187 kedro_ibis_dataset-0.0.6b1/README.md
+-rw-r--r--   0        0        0      795 2023-06-17 10:42:53.716990 kedro_ibis_dataset-0.0.6b1/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-06-17 09:51:15.984286 kedro_ibis_dataset-0.0.6b1/src/kedro_ibis_dataset/__init__.py
+-rw-r--r--   0        0        0     2846 2023-06-17 10:40:13.135984 kedro_ibis_dataset-0.0.6b1/src/kedro_ibis_dataset/kedro_ibis_dataset.py
+-rw-r--r--   0        0        0     1238 2023-06-17 10:38:51.997409 kedro_ibis_dataset-0.0.6b1/tests/test_ibis_dataset.py
+-rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 kedro_ibis_dataset-0.0.6b1/PKG-INFO
```

### Comparing `kedro_ibis_dataset-0.0.6a3/pyproject.toml` & `kedro_ibis_dataset-0.0.6b1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kedro-ibis-dataset"
-version = "0.0.6a3"
+version = "0.0.6b1"
 description = "Ibis connector for kedro catalog"
 authors = [
     { name = "Iñigo Hidalgo Rey", email = "inigohrey@gmail.com" },
 ]
 dependencies = [
     "kedro>=0.17.1",
     "ibis-framework>=5.1.0",
@@ -31,7 +31,14 @@
 shell = "./tasks/tag-release.sh"
 
 [tool.pdm.scripts.release]
 composite = [
     "build",
     "tag",
 ]
+
+[tool.pdm.dev-dependencies]
+test = [
+    "pytest>=7.3.2",
+    "ibis-framework[duckdb]",
+    "duckdb>=0.8.1",
+]
```

### Comparing `kedro_ibis_dataset-0.0.6a3/src/kedro_ibis_dataset/kedro_ibis_dataset.py` & `kedro_ibis_dataset-0.0.6b1/src/kedro_ibis_dataset/kedro_ibis_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,24 +43,39 @@
         Returns:
             None
         """
         if connection_string not in cls.connections:
             cls.connections[connection_string] = ibis.connect(connection_string)
         return
 
-    # TODO: check table exists when instantiating connection?
-    # would this be desirable behavior?
-    # def _exists(self):
+
 
     def _load(self):
-        con = self.connections[self.connection_string]
-        return con.table(self.table_name)
+        return self._table
+
+    def _save(self, data, **kwargs):
+        if self._table_exists:
+            self._table.insert(data, **kwargs)
+        else:
+            self._connection.create_table(self.table_name, data)
 
-    def _save(self, data):
-        # TODO: implement save method
-        raise DataSetError("Saving to IbisDataSet is not supported.")
-    
     def _describe(self):
         return dict(
             table_name=self.table_name,
             credentials=self.credentials
         )
+    @property
+    def _table(self):
+        if not self._table_exists:
+            raise DataSetError(f"Table '{self.table_name}' does not exist in DB.")
+        return self._connection.table(self.table_name)
+
+    # TODO: extend _exists for kedro funcionality?
+    # is there a functional benefit with kedro?
+    # def _exists(self):
+    @property
+    def _table_exists(self):
+        return self.table_name in self._connection.list_tables()
+
+    @property
+    def _connection(self):
+        return self.connections[self.connection_string]
```

