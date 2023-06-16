# Comparing `tmp/deduplicationdict-1.0.1.tar.gz` & `tmp/deduplicationdict-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deduplicationdict-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deduplicationdict-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deduplicationdict-1.0.1.tar` & `deduplicationdict-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    17190 2023-05-27 06:10:01.043229 deduplicationdict-1.0.1/LICENSE
--rw-r--r--   0        0        0     4095 2023-06-02 01:57:49.631690 deduplicationdict-1.0.1/README.md
--rw-r--r--   0        0        0    10826 2023-05-27 23:42:44.735005 deduplicationdict-1.0.1/deduplicationdict/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 20:16:38.579244 deduplicationdict-1.0.1/deduplicationdict/py.typed
--rw-r--r--   0        0        0     4026 2023-05-27 23:51:47.853909 deduplicationdict-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     7150 1970-01-01 00:00:00.000000 deduplicationdict-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    17190 2023-05-27 06:10:01.043229 deduplicationdict-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4095 2023-06-16 22:18:05.371028 deduplicationdict-1.0.2/README.md
+-rw-r--r--   0        0        0    11503 2023-06-16 22:05:40.683130 deduplicationdict-1.0.2/deduplicationdict/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 20:16:38.579244 deduplicationdict-1.0.2/deduplicationdict/py.typed
+-rw-r--r--   0        0        0     4026 2023-06-16 19:06:36.445758 deduplicationdict-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7150 1970-01-01 00:00:00.000000 deduplicationdict-1.0.2/PKG-INFO
```

### Comparing `deduplicationdict-1.0.1/LICENSE` & `deduplicationdict-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deduplicationdict-1.0.1/README.md` & `deduplicationdict-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 assert dedup_dict["b"] == 2
 assert dedup_dict["c"] == [5, 6, 7]
 assert dedup_dict["d"] == [1, 2, 3]
 assert dedup_dict["e"] == [1, 2, 3]
 assert DeDuplicationDict.from_json_save_dict(dedup_dict.to_json_save_dict()).to_dict() == dedup_dict.to_dict()
 ```
 
-Usage
-with [SqliteDict](https://github.com/RaRe-Technologies/sqlitedict): [SqliteDeDuplicationDict.py](https://gist.github.com/Vivswan/6fca547b2927e0bf11743869058d4b10)
+Usage with [SqliteDict](https://github.com/RaRe-Technologies/sqlitedict):
+[SqliteDeDuplicationDict.py](https://gist.github.com/Vivswan/6fca547b2927e0bf11743869058d4b10)
 
 ## Results from Testing
 
 | Method              | JSON Memory (MB) | In-Memory (MB) |
 |:--------------------|:----------------:|:--------------:|
 | `dict`              |    14.089 MB     |   27.542 MB    |
 | `DeDuplicationDict` |    1.7906 MB     |    3.806 MB    |
```

### Comparing `deduplicationdict-1.0.1/deduplicationdict/__init__.py` & `deduplicationdict-1.0.2/deduplicationdict/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     Attributes:
         hash_length (int): The length of the hash value used for deduplication.
         auto_clean_up (bool): Whether to automatically clean up unused hash values when deleting items.
     """
 
     hash_length: int = 8
     auto_clean_up: bool = True
+    skip_update_on_setitem: bool = True
 
     def __init__(self, *args, _value_dict: dict = None, **kwargs):
         """Initialize a DeDuplicationDict instance.
 
         Args:
             *args: Positional arguments passed to the dict constructor.
             _value_dict (dict, optional): An existing value dictionary to use for deduplication.
@@ -67,31 +68,33 @@
 
         self.key_dict: Dict[str, Union[str, DeDuplicationDict]] = {}
         self.value_dict: Dict[str, Any] = {} if _value_dict is None else _value_dict
 
         for k, v in dict(*args, **kwargs).items():
             self[k] = v
 
-    def _set_value_dict(self, value_dict: dict) -> DeDuplicationDict:
+    def _set_value_dict(self, value_dict: dict, skip_update: bool = False) -> DeDuplicationDict:
         """Update the value dictionary and propagate the changes to nested DeDuplicationDict instances.
 
         Args:
             value_dict (dict): The new value dictionary to use for deduplication.
+            skip_update (bool): Whether to skip updating the value dictionary of nested
 
         Return:
             DeDuplicationDict: self
         """
 
-        value_dict.update(self.value_dict)
+        if not skip_update:
+            value_dict.update(self.value_dict)
         self.value_dict = value_dict
         for v in self.key_dict.values():
             if isinstance(v, str):
                 continue
 
-            v._set_value_dict(value_dict)
+            v._set_value_dict(value_dict, skip_update=skip_update)
 
         return self
 
     def __setitem__(self, key: KT, value: VT) -> None:
         """Set the value for the given key, deduplicating the value if necessary.
 
         Args:
@@ -102,15 +105,16 @@
         if key in self.key_dict:
             del self[key]
 
         if isinstance(value, dict):
             self.key_dict[key] = DeDuplicationDict(value, _value_dict=self.value_dict)
         elif isinstance(value, DeDuplicationDict):
             self.key_dict[key] = value
-            value._set_value_dict(self.value_dict)
+            self.value_dict.update(value.value_dict)
+            value._set_value_dict(self.value_dict, skip_update=self.skip_update_on_setitem)
         else:
             hash_id = sha256(pickle.dumps(value)).hexdigest()[:self.hash_length]
             self.key_dict[key] = hash_id
 
             if hash_id not in self.value_dict:
                 self.value_dict[hash_id] = value
 
@@ -175,14 +179,26 @@
 
         Returns:
             DeDuplicationDict: A new DeDuplicationDict instance with its own value dictionary.
         """
 
         return self.from_json_save_dict(self.to_json_save_dict())
 
+    def __deepcopy__(self, memo: dict) -> DeDuplicationDict:
+        """Create a deep copy of the DeDuplicationDict instance.
+
+        Args:
+            memo (dict): A dictionary of memoized values.
+
+        Returns:
+            DeDuplicationDict: A new DeDuplicationDict instance with its own value dictionary.
+        """
+
+        return self.detach()
+
     def _del_detach(self) -> DeDuplicationDict:
         """Detach the DeDuplicationDict instance from its value dictionary and clean up unused hash values.
 
         Return:
             DeDuplicationDict: self
         """
```

### Comparing `deduplicationdict-1.0.1/pyproject.toml` & `deduplicationdict-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [tool.setuptools.packages.find]
 where = ["deduplicationdict"]
 
 [project]
 # $ pip install deduplicationdict
 name = "deduplicationdict"
-version = "1.0.1"
+version = "1.0.2"
 description = "A dictionary that de-duplicates values."
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["python", "dict", "deduplication", "optimization", ]
 authors = [
     { name = "Vivswan Shah", email = "vivswanshah@pitt.edu" }
```

### Comparing `deduplicationdict-1.0.1/PKG-INFO` & `deduplicationdict-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deduplicationdict
-Version: 1.0.1
+Version: 1.0.2
 Summary: A dictionary that de-duplicates values.
 Keywords: python,dict,deduplication,optimization
 Author-email: Vivswan Shah <vivswanshah@pitt.edu>
 Maintainer-email: Vivswan Shah <vivswanshah@pitt.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -124,16 +124,16 @@
 assert dedup_dict["b"] == 2
 assert dedup_dict["c"] == [5, 6, 7]
 assert dedup_dict["d"] == [1, 2, 3]
 assert dedup_dict["e"] == [1, 2, 3]
 assert DeDuplicationDict.from_json_save_dict(dedup_dict.to_json_save_dict()).to_dict() == dedup_dict.to_dict()
 ```
 
-Usage
-with [SqliteDict](https://github.com/RaRe-Technologies/sqlitedict): [SqliteDeDuplicationDict.py](https://gist.github.com/Vivswan/6fca547b2927e0bf11743869058d4b10)
+Usage with [SqliteDict](https://github.com/RaRe-Technologies/sqlitedict):
+[SqliteDeDuplicationDict.py](https://gist.github.com/Vivswan/6fca547b2927e0bf11743869058d4b10)
 
 ## Results from Testing
 
 | Method              | JSON Memory (MB) | In-Memory (MB) |
 |:--------------------|:----------------:|:--------------:|
 | `dict`              |    14.089 MB     |   27.542 MB    |
 | `DeDuplicationDict` |    1.7906 MB     |    3.806 MB    |
```

