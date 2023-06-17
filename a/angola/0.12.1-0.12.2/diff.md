# Comparing `tmp/angola-0.12.1.tar.gz` & `tmp/angola-0.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.12.1.tar", last modified: Fri Jun  9 05:24:09 2023, max compression
+gzip compressed data, was "angola-0.12.2.tar", last modified: Sat Jun 17 18:39:25 2023, max compression
```

## Comparing `angola-0.12.1.tar` & `angola-0.12.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:24:09.205971 angola-0.12.1/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.12.1/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.12.1/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-09 05:24:09.206033 angola-0.12.1/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.12.1/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-09 05:24:09.206255 angola-0.12.1/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-09 05:24:04.000000 angola-0.12.1/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:24:09.200431 angola-0.12.1/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:24:09.203756 angola-0.12.1/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.12.1/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    48688 2023-06-09 05:23:54.000000 angola-0.12.1/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.12.1/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.12.1/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.12.1/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    19447 2023-06-09 03:27:14.000000 angola-0.12.1/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:24:09.204713 angola-0.12.1/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-09 05:24:09.000000 angola-0.12.1/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-09 05:24:09.000000 angola-0.12.1/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-09 05:24:09.000000 angola-0.12.1/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-09 05:24:09.000000 angola-0.12.1/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-09 05:24:09.000000 angola-0.12.1/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-09 05:24:09.205874 angola-0.12.1/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.12.1/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.12.1/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.12.1/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.12.1/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.12.1/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-17 18:39:25.698866 angola-0.12.2/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.12.2/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.12.2/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-17 18:39:25.698929 angola-0.12.2/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.12.2/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-17 18:39:25.699155 angola-0.12.2/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-17 18:39:15.000000 angola-0.12.2/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-17 18:39:25.692696 angola-0.12.2/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-17 18:39:25.696280 angola-0.12.2/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.12.2/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    50794 2023-06-11 22:47:22.000000 angola-0.12.2/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.12.2/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.12.2/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.12.2/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    19447 2023-06-09 03:27:14.000000 angola-0.12.2/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-17 18:39:25.697226 angola-0.12.2/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-17 18:39:25.000000 angola-0.12.2/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-17 18:39:25.000000 angola-0.12.2/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-17 18:39:25.000000 angola-0.12.2/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-17 18:39:25.000000 angola-0.12.2/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-17 18:39:25.000000 angola-0.12.2/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-17 18:39:25.698772 angola-0.12.2/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.12.2/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.12.2/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.12.2/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.12.2/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.12.2/tests/test_query.py
```

### Comparing `angola-0.12.1/LICENSE` & `angola-0.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.12.1/PKG-INFO` & `angola-0.12.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.12.1
+Version: 0.12.2
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.12.1/README.md` & `angola-0.12.2/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.12.1/setup.py` & `angola-0.12.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.12.1"
+VERSION = "0.12.2"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.12.1/src/angola/database.py` & `angola-0.12.2/src/angola/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -742,14 +742,19 @@
         if self._collection_prefix:
             if isinstance(self._collection_prefix, str):
                 collection_name = "%s%s" % (self._collection_prefix, collection_name)
             elif callable(self._collection_prefix):
                 collection_name = self._collection_prefix(collection_name)
         return collection_name
 
+    def unprefix_collection_name(self, collection_name:str) -> str:
+        if self._collection_prefix:
+            return collection_name.replace(self._collection_prefix, "")
+        return collection_name
+        
     def has_db(self, dbname:str=None) -> bool:
         """
         Check if the system has a database
 
         Params:
             dbname:str|None - The dbname to check or the current self.dbname
 
@@ -791,76 +796,82 @@
                         username=self.username, 
                         password=self.password, 
                         collection_prefix=collection_prefix or self._collection_prefix, 
                         custom_ops=self._custom_ops, 
                         default_indexes=default_indexes or self.default_indexes,
                         query_max_limit=self.query_max_limit)
 
-    def has_collection(self, collection_name) -> bool:
+    def has_collection(self, collection_name, use_prefix=True) -> bool:
         """
         Test if collection exists in the current db. 
 
         Params:
             collection_name:str - the collection name 
 
         Returns:
             bool
         """
-        collection_name = self.prefix_collection_name(collection_name)
+        if use_prefix:
+            collection_name = self.prefix_collection_name(collection_name)
         return self.db.has_collection(collection_name)
 
-    def create_collection(self, collection_name:str, indexes:list=[]) -> bool:
+    def create_collection(self, collection_name:str, indexes:list=[], use_prefix=True) -> bool:
         """
         Create a collection if not exists
         Returns: bool
         """
         if not self.has_collection(collection_name):
-            collection_name = self.prefix_collection_name(collection_name)
+            if use_prefix:
+                collection_name = self.prefix_collection_name(collection_name)
             col = self.db.create_collection(collection_name)
 
             # indexes
             if _indexes := {l.get("name"):l for l in [*DEFAULT_INDEXES, *(self.default_indexes or []), *(indexes or [])]}.values():
                 for index in _indexes:
                     col._add_index(index) 
                     
             return True 
         return False
 
-    def select_collection(self, collection_name:str, indexes:list=[], immut_keys:list=[], item_class=None, auto_create:bool=True) -> "Collection":
+    def select_collection(self, collection_name:str, indexes:list=[], immut_keys:list=[], item_class=None, auto_create:bool=True, use_prefix=True) -> "Collection":
         """
         To select a collection
 
         Params:
             collection_name:str - collectioin name 
             indexes:List[dict] - the indexes to use
             immut_keys:list - immutable keys. Keys that can't be updated once created
             auto_create:bool - To auto create the collection if doesn't exist
-
+            use_prefix:bool - To use the prefix or not
         Return: Collection
 
         """
 
         if self.has_collection(collection_name):
-            collection_name = self.prefix_collection_name(collection_name)
+            if use_prefix:
+                collection_name = self.prefix_collection_name(collection_name)
             col = self.db.collection(collection_name)
         elif auto_create is True:
             self.create_collection(collection_name=collection_name, indexes=indexes)
-            collection_name = self.prefix_collection_name(collection_name)
+            if use_prefix:
+                collection_name = self.prefix_collection_name(collection_name)
             col = self.db.collection(collection_name)
         else:
             raise CollectionNotFoundError()
 
         return Collection(db=self, collection=col, immut_keys=immut_keys, custom_ops=self._custom_ops, item_class=item_class)
 
-    def select_edge_collection(self, collection_name:str):
+    def select_edge_collection(self, collection_name:str, use_prefix=True):
         if self.db.has_collection(collection_name):
-            collection_name = self.prefix_collection_name(collection_name)
+            if use_prefix:
+                collection_name = self.prefix_collection_name(collection_name)
             return self.db.collection(collection_name)
         else:
-            collection_name = self.prefix_collection_name(collection_name)
+            if use_prefix:
+                collection_name = self.prefix_collection_name(collection_name)
             return self.db.create_collection(name=collection_name, edge=True)
 
     def get_item(self, path:str) -> CollectionItem:
         """
         To get an item via path.
 
         - Item Path: [COLLECTION_NAME/KEY] -> articles/1234568
@@ -971,30 +982,41 @@
         All collections in the db
 
         Returns:
             list
         """
         return self.db.collections()
     
-    def rename_collection(self, collection_name:str, new_name:str):
+    def rename_collection(self, collection_name:str, new_name:str, use_prefix=True):
         """
         Rename collection
         """
-        if self.has(collection_name) and not self.has(new_name):
-            collection_name = self.prefix_collection_name(collection_name)
-            new_name = self.prefix_collection_name(new_name)
-            coll = self.select(collection_name)
-            coll.rename(new_name)
-            return self.select(new_name)
+        if self.has(collection_name, use_prefix=use_prefix) and not self.has(new_name, use_prefix=use_prefix):
+            if use_prefix:
+                collection_name = self.prefix_collection_name(collection_name)
+            if use_prefix:
+                new_name = self.prefix_collection_name(new_name)
+            coll = self.select_collection(collection_name, use_prefix=use_prefix)
+            coll.collection.rename(new_name)
+            return self.select_collection(new_name, use_prefix=use_prefix)
     
-    def drop_collection(self, collection_name:str):
-        if self.has_collection(collection_name):
-            collection_name = self.prefix_collection_name(collection_name)
+    def delete_collection(self, collection_name:str, use_prefix=True):
+        if self.has_collection(collection_name, use_prefix=use_prefix):
+            if use_prefix:
+                collection_name = self.prefix_collection_name(collection_name)
             self.db.delete_collection(collection_name)
 
+    def truncate_collection(self, collection_name:str, use_prefix=True):
+        if self.has_collection(collection_name, use_prefix=use_prefix):
+            if use_prefix:
+                collection_name = self.prefix_collection_name(collection_name)
+            coll = self.select_collection(collection_name, use_prefix=use_prefix)
+            coll.collection.truncate()
+
+
     def add_index(self, collection_name, data:dict):
         """
         Args:
             - collection, the collection name
             - data: dict of 
                     {
                         "type": "persistent",
@@ -1017,34 +1039,37 @@
             - collection, the collection name
             - id: the index id
         """
         collection_name = self.prefix_collection_name(collection_name)
         col = self.db.collection(collection_name)
         col.delete_index(id, ignore_missing=True)
 
-    def link_edges(self, from_item:"CollectionItem", to_item:"CollectionItem", data:dict={}, edge_collection_name:str=None):
+    def link_edges(self, from_item:"CollectionItem", to_item:"CollectionItem", data:dict={}, edge_collection_name:str=None, use_prefix=True):
         """
         GRAPH
         Link edges of 2 collections from:to
 
         Params:
             - from_item:CollectionItem
             - to_item:CollectionItem
             - data:dict
             - edge_collection_name:str
         """
         from_coll_name = from_item._collection.name
         to_coll_name = to_item._collection.name
+        from_cname = self.unprefix_collection_name(from_coll_name)
+        to_cname = self.unprefix_collection_name(to_coll_name)
+
+        if not edge_collection_name and from_cname and to_cname:
+            edge_collection_name = _create_edge_name(from_cname, to_cname)
 
-        if not edge_collection_name and from_coll_name and to_coll_name:
-            edge_collection_name = "edges__%s--%s" % (from_coll_name, to_coll_name)
         if not edge_collection_name:
             raise Exception("MISSING EDGE COLLECTION NAME")
 
-        coll = self.select_edge_collection(edge_collection_name)
+        coll = self.select_edge_collection(edge_collection_name, use_prefix=use_prefix)
 
         # ensuring _id and _key are not included
         if data:
             for k in ["_id", "_key"]:
                 if k in data:
                     data.pop(k)
         doc = {
@@ -1144,15 +1169,27 @@
                                     edge_uniqueness='global',
                                     vertex_uniqueness='global',
                                     min_depth=min_depth, 
                                     )["paths"]:
                 
                 yield tuple(self._load_item(item) for item in trav["vertices"])
 
+    def get_collection_stats(self, collection_name:str, use_prefix=True) -> dict:
+        coll = self.select_collection(collection_name=collection_name, use_prefix=use_prefix)
+        koll = coll.collection
+        count = koll.count()
+        statistics = koll.statistics() or {"documents_size": 0, "indexes": {"count": 0, "size": 0}}
+        return {
+            "documents_count": count, 
+            "documents_size": statistics.get("documents_size"),
+            "indexes_count": statistics.get("indexes").get("count"),
+            "indexes_size": statistics.get("indexes").get("size"),
+        }
 
+    
 class Collection(object):
 
     def __init__(self, db:Database, collection,  immut_keys:list=[], custom_ops:dict={}, item_class=None):
         self.db = db
         self.collection = collection
         self._immut_keys = immut_keys
         self._custom_ops = custom_ops
@@ -1351,28 +1388,33 @@
         Returns
             CollectionItem
         """
         if data := list(self.find(filters=filters, limit=1, sort=None)):
             return data[0]
         return None
 
-    def edges_with(self, collection:"Collection") -> tuple:
+    def edges_with(self, collection:"Collection", use_prefix=True) -> tuple:
         """
         ::GRAPH::
 
         Create an Edge Collection Definition, especially when building a traversal
 
         ie:
         relations = [CollectionA.edges_with(CollectionB)]
 
         Returns
             tuple(name, edge_name, from_collection_name, to_collection_name)
         """
-        edge_name = _create_edge_name(from_name=self.collection_name, to_name=collection.collection_name)
-        name = "%s--%s" % (self.collection_name, collection.collection_name)
+        from_coll_name = self.collection_name
+        to_coll_name = collection.collection_name
+        from_cname = self.db.unprefix_collection_name(from_coll_name)
+        to_cname = self.db.unprefix_collection_name(to_coll_name)
+
+        edge_name = _create_edge_name(from_cname, to_cname)
+        name = "%s--%s" % (from_cname, to_cname)
         return (name, edge_name, self.collection_name, collection.collection_name)
 
 
 class SubCollection(object):
     _data = []
     _constraints = []
     _item = None
@@ -1537,15 +1579,15 @@
         data = dict_query.query(data=self._data, filters=filters)
         return dict_query.Cursor([_SubCollectionItem(self, d) for d in data])
 
 
 #------------------------------------------------------------------------------
 
 def _create_edge_name(from_name, to_name):
-    return "edges__%s--%s" % (from_name, to_name)
+    return "edge--%s-%s" % (from_name, to_name)
 
 def _create_document_item(data:dict={}) -> dict:
     _key = data["_key"] if "_key" in data else lib.gen_key()
 
     return {
         "_key": _key,
         "_created_at:$datetime": True,
```

### Comparing `angola-0.12.1/src/angola/dict_mutator.py` & `angola-0.12.2/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.1/src/angola/dict_query.py` & `angola-0.12.2/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.1/src/angola/lib.py` & `angola-0.12.2/src/angola/lib.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.1/src/angola/lib_xql.py` & `angola-0.12.2/src/angola/lib_xql.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.1/src/angola.egg-info/PKG-INFO` & `angola-0.12.2/src/angola.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.12.1
+Version: 0.12.2
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.12.1/tests/test_database.py` & `angola-0.12.2/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.1/tests/test_dict_mutator.py` & `angola-0.12.2/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.1/tests/test_lib.py` & `angola-0.12.2/tests/test_lib.py`

 * *Files identical despite different names*

