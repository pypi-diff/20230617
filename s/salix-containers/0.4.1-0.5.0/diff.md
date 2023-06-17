# Comparing `tmp/salix-containers-0.4.1.tar.gz` & `tmp/salix_containers-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salix-containers-0.4.1.tar", max compression
+gzip compressed data, was "salix_containers-0.5.0.tar", max compression
```

## Comparing `salix-containers-0.4.1.tar` & `salix_containers-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      331 2023-04-22 15:43:41.633649 salix-containers-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      182 2023-04-22 15:41:04.593649 salix-containers-0.4.1/salix_containers/__init__.py
--rw-r--r--   0        0        0     1039 2023-04-15 17:31:03.289609 salix-containers-0.4.1/salix_containers/caselessmapping.py
--rw-r--r--   0        0        0     1617 2022-04-16 20:28:31.676860 salix-containers-0.4.1/salix_containers/casttypes.py
--rw-r--r--   0        0        0      452 2023-04-22 14:46:09.483649 salix-containers-0.4.1/salix_containers/empty.py
--rw-r--r--   0        0        0        0 2023-04-15 16:49:10.619609 salix-containers-0.4.1/salix_containers/tests/__init__.py
--rw-r--r--   0        0        0     3591 2023-04-22 14:54:07.813649 salix-containers-0.4.1/salix_containers/tests/test_caselessmappings.py
--rw-r--r--   0        0        0     2669 2023-04-22 14:54:39.073649 salix-containers-0.4.1/salix_containers/tests/test_casttypes.py
--rw-r--r--   0        0        0     1370 2023-04-22 15:17:50.143649 salix-containers-0.4.1/salix_containers/tests/test_empty.py
--rw-r--r--   0        0        0      561 2023-04-22 15:44:45.880620 salix-containers-0.4.1/setup.py
--rw-r--r--   0        0        0      489 2023-04-22 15:44:45.880833 salix-containers-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      331 2023-06-17 16:42:22.753414 salix_containers-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      182 2023-04-22 15:41:04.593649 salix_containers-0.5.0/salix_containers/__init__.py
+-rw-r--r--   0        0        0     1039 2023-04-15 17:31:03.289609 salix_containers-0.5.0/salix_containers/caselessmapping.py
+-rw-r--r--   0        0        0     2048 2023-06-17 16:40:30.673414 salix_containers-0.5.0/salix_containers/casttypes.py
+-rw-r--r--   0        0        0      452 2023-04-22 14:46:09.483649 salix_containers-0.5.0/salix_containers/empty.py
+-rw-r--r--   0        0        0        0 2023-04-15 16:49:10.619609 salix_containers-0.5.0/salix_containers/tests/__init__.py
+-rw-r--r--   0        0        0     3591 2023-04-22 14:54:07.813649 salix_containers-0.5.0/salix_containers/tests/test_caselessmappings.py
+-rw-r--r--   0        0        0     3053 2023-06-17 16:38:14.583414 salix_containers-0.5.0/salix_containers/tests/test_casttypes.py
+-rw-r--r--   0        0        0     1370 2023-04-22 15:17:50.143649 salix_containers-0.5.0/salix_containers/tests/test_empty.py
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 salix_containers-0.5.0/PKG-INFO
```

### Comparing `salix-containers-0.4.1/salix_containers/caselessmapping.py` & `salix_containers-0.5.0/salix_containers/caselessmapping.py`

 * *Files identical despite different names*

### Comparing `salix-containers-0.4.1/salix_containers/casttypes.py` & `salix_containers-0.5.0/salix_containers/casttypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,41 +3,49 @@
 class CastBase:
     """
     Identical to regular dict/list except on instantiation it performs a
     one-off recursive recasting of all contained items that have a type listed
     in cast_map to the mapped target type.
 
     Also automatically recasts any list or dict instances to CastList and
-    CastDict respectively.
+    CastDict respectively and recurses them.
+
+    Will only recurse lists and dicts, so if you want to recurse into tuples
+    or sets, make sure to include a conversion for these into lists.
 
     Useful if you have stubborn objects that won't pickle or export to json for
     example.
 
     cast_map is a dict of conversion types and their recast targets, e.g.:
 
         {int: str, float: Decimal}
 
     Conversion types can be a tuple of types:
 
         {(int, float): str}
 
+
     """
     def __init__(self, *args, cast_map, **kwargs):
+        # recast keys of cast_map to always be tuples
+        cast_map = {(tuple([key]) if not isinstance(key, tuple) else key): value for key, value in cast_map.items()}
         self.cast_map = cast_map
         super().__init__(*args, **kwargs)
         self._recast()
 
     def _recast(self):
         raise NotImplemented()
 
     def _recast_item(self, item):
         # Try to recast it first, then recurse
-        for src, dst in self.cast_map.items():
-            if isinstance(item, src):
-                item = dst(item)
+        for src_types, dst_type in self.cast_map.items():
+            for src_type in src_types:
+                if isinstance(item, src_type):
+                    item = dst_type(item)
+                    break
         if isinstance(item, list):
             return CastList(item, cast_map=self.cast_map)
         elif isinstance(item, dict):
             return CastDict(item, cast_map=self.cast_map)
         else:
             return item
```

### Comparing `salix-containers-0.4.1/salix_containers/tests/test_caselessmappings.py` & `salix_containers-0.5.0/salix_containers/tests/test_caselessmappings.py`

 * *Files identical despite different names*

### Comparing `salix-containers-0.4.1/salix_containers/tests/test_casttypes.py` & `salix_containers-0.5.0/salix_containers/tests/test_casttypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,7 +87,18 @@
         self.assertDictEqual(cd, {1: 6})
 
     def test_cast10(self):
         d = {1: ('a', 'b', 'c'), 2: ('1', '2', '3')}
         cd = CastDict(d, cast_map={tuple: lambda x: ':'.join(x)})
         self.assertDictEqual(cd, {1: 'a:b:c', 2: '1:2:3'})
 
+    def test_cast_map_tuple_src_type1(self):
+        d = {1: ['10', '11']}
+        cd = CastDict(d, cast_map={(str, set): int})
+        self.assertDictEqual(cd, {1: [10, 11]})
+
+    def test_cast_map_tuple_src_type2(self):
+        d = {1: ('10', '11'), 2: [7, 9]}
+        cd = CastDict(d, cast_map={(tuple, list): set})
+        self.assertDictEqual(cd, {1: {'10', '11'}, 2: {7, 9}})
+
+
```

### Comparing `salix-containers-0.4.1/salix_containers/tests/test_empty.py` & `salix_containers-0.5.0/salix_containers/tests/test_empty.py`

 * *Files identical despite different names*

