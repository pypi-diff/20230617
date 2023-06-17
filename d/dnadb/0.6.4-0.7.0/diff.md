# Comparing `tmp/dnadb-0.6.4.tar.gz` & `tmp/dnadb-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.6.4.tar", last modified: Sat Jun  3 17:04:12 2023, max compression
+gzip compressed data, was "dnadb-0.7.0.tar", last modified: Sat Jun 17 20:11:48 2023, max compression
```

## Comparing `dnadb-0.6.4.tar` & `dnadb-0.7.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.6.4/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-06-03 17:04:12.466433 dnadb-0.6.4/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.6.4/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-06-03 17:02:06.000000 dnadb-0.6.4/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-06-03 17:04:12.466433 dnadb-0.6.4/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-06-03 17:02:15.000000 dnadb-0.6.4/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.6.4/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.6.4/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.6.4/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.6.4/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.6.4/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     2252 2023-05-21 14:19:04.000000 dnadb-0.6.4/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4958 2023-05-23 07:14:31.000000 dnadb-0.6.4/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     8047 2023-05-23 07:16:22.000000 dnadb-0.6.4/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6218 2023-05-31 17:48:30.000000 dnadb-0.6.4/src/dnadb/fastq.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/dnadb/integration/
--rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-05-23 06:13:30.000000 dnadb-0.6.4/src/dnadb/integration/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/dnadb/integration/tf/
--rw-r--r--   0 dwl2x     (1000) users      (100)       18 2023-05-23 06:20:23.000000 dnadb-0.6.4/src/dnadb/integration/tf/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     3266 2023-05-24 04:25:25.000000 dnadb-0.6.4/src/dnadb/integration/tf/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    11296 2023-06-03 16:57:18.000000 dnadb-0.6.4/src/dnadb/sample.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    20938 2023-06-03 16:59:30.000000 dnadb-0.6.4/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)       84 2023-05-21 14:17:53.000000 dnadb-0.6.4/src/dnadb/types.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.6.4/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-06-03 17:04:12.000000 dnadb-0.6.4/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      644 2023-06-03 17:04:12.000000 dnadb-0.6.4/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-06-03 17:04:12.000000 dnadb-0.6.4/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-06-03 17:04:12.000000 dnadb-0.6.4/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-06-03 17:04:12.000000 dnadb-0.6.4/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-17 20:11:48.768631 dnadb-0.7.0/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.7.0/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-06-17 20:11:48.768631 dnadb-0.7.0/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.7.0/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-06-17 20:09:05.000000 dnadb-0.7.0/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-06-17 20:11:48.768631 dnadb-0.7.0/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-17 20:11:48.768631 dnadb-0.7.0/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-17 20:11:48.768631 dnadb-0.7.0/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-06-17 20:09:18.000000 dnadb-0.7.0/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-17 20:11:48.768631 dnadb-0.7.0/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.7.0/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.7.0/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.7.0/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-17 20:11:48.768631 dnadb-0.7.0/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.7.0/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.7.0/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     2252 2023-05-21 14:19:04.000000 dnadb-0.7.0/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4958 2023-05-23 07:14:31.000000 dnadb-0.7.0/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     8047 2023-05-23 07:16:22.000000 dnadb-0.7.0/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6218 2023-05-31 17:48:30.000000 dnadb-0.7.0/src/dnadb/fastq.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-17 20:11:48.768631 dnadb-0.7.0/src/dnadb/integration/
+-rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-05-23 06:13:30.000000 dnadb-0.7.0/src/dnadb/integration/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-17 20:11:48.768631 dnadb-0.7.0/src/dnadb/integration/tf/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       18 2023-05-23 06:20:23.000000 dnadb-0.7.0/src/dnadb/integration/tf/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     3266 2023-05-24 04:25:25.000000 dnadb-0.7.0/src/dnadb/integration/tf/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    11445 2023-06-17 19:04:52.000000 dnadb-0.7.0/src/dnadb/sample.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    21086 2023-06-17 20:08:45.000000 dnadb-0.7.0/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)       84 2023-05-21 14:17:53.000000 dnadb-0.7.0/src/dnadb/types.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.7.0/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-17 20:11:48.768631 dnadb-0.7.0/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-06-17 20:11:48.000000 dnadb-0.7.0/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      644 2023-06-17 20:11:48.000000 dnadb-0.7.0/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-06-17 20:11:48.000000 dnadb-0.7.0/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-06-17 20:11:48.000000 dnadb-0.7.0/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-06-17 20:11:48.000000 dnadb-0.7.0/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.6.4/LICENSE` & `dnadb-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.4/PKG-INFO` & `dnadb-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.6.4
+Version: 0.7.0
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.6.4/pyproject.toml` & `dnadb-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.6.4"
+version = "0.7.0"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.6.4/src/dnadb/datasets/dataset.py` & `dnadb-0.7.0/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.4/src/dnadb/datasets/greengenes.py` & `dnadb-0.7.0/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.4/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.7.0/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.4/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.7.0/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.4/src/dnadb/db.py` & `dnadb-0.7.0/src/dnadb/db.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.4/src/dnadb/dna.py` & `dnadb-0.7.0/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.4/src/dnadb/fasta.py` & `dnadb-0.7.0/src/dnadb/fasta.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.4/src/dnadb/fastq.py` & `dnadb-0.7.0/src/dnadb/fastq.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.4/src/dnadb/integration/tf/dna.py` & `dnadb-0.7.0/src/dnadb/integration/tf/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.4/src/dnadb/sample.py` & `dnadb-0.7.0/src/dnadb/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,21 +63,24 @@
 
 class SampleMappingEntryFactory:
     def __init__(self, name: str, fasta_index_db: FastaIndexDb):
         self.name = name
         self.fasta_index_db = fasta_index_db
         self.abundance_map: dict[int, int] = {}
 
-    def add_entry(self, entry: FastaEntry, abundance: int = 1) -> 'SampleMappingEntryFactory':
-        index = self.fasta_index_db.fasta_id_to_index(entry.identifier)
+    def add_fasta_id(self, fasta_id: str, abundance: int = 1) -> 'SampleMappingEntryFactory':
+        index = self.fasta_index_db.fasta_id_to_index(fasta_id)
         if index not in self.abundance_map:
             self.abundance_map[index] = 0
         self.abundance_map[index] += abundance
         return self
 
+    def add_entry(self, entry: FastaEntry, abundance: int = 1) -> 'SampleMappingEntryFactory':
+        return self.add_fasta_id(entry.identifier, abundance)
+
     def add_entries(self, entries: Iterable[FastaEntry]) -> 'SampleMappingEntryFactory':
         for entry in entries:
             self.add_entry(entry)
         return self
 
     def build(self) -> SampleMappingEntry:
         indices = np.array(sorted(self.abundance_map.keys()))
```

### Comparing `dnadb-0.6.4/src/dnadb/taxonomy.py` & `dnadb-0.7.0/src/dnadb/taxonomy.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,28 +13,29 @@
 from .utils import open_file
 
 RANKS = ("Kingdom", "Phylum", "Class", "Order", "Family", "Genus", "Species")
 RANK_PREFIXES = ''.join(rank[0] for rank in RANKS).lower()
 
 # Utility Functions --------------------------------------------------------------------------------
 
-def split_taxonomy(taxonomy: str) -> Tuple[str, ...]:
+def split_taxonomy(taxonomy: str, keep_empty: bool = False) -> Tuple[str, ...]:
     """
     Split taxonomy label into a tuple
     """
-    return tuple(re.findall(r"\w__([^;]+)", taxonomy))
+    return tuple(re.findall(r"\w__([^;]*)" if keep_empty else r"\w__([^;]+)", taxonomy))
 
 
-def join_taxonomy(taxonomy: Union[Tuple[str, ...], List[str]]) -> str:
+def join_taxonomy(taxonomy: Union[Tuple[str, ...], List[str]], depth: Optional[int] = None) -> str:
     """
     Merge a taxonomy tuple into a string format
     """
-    depth = len(taxonomy)
+    if depth is None:
+        depth = len(taxonomy)
     assert depth >= 1 and depth <= len(RANKS), "Invalid taxonomy"
-    taxonomy = tuple(taxonomy) + ("",) * (len(RANKS) - depth)
+    taxonomy = tuple(taxonomy) + ("",)*(depth - len(taxonomy))
     return "; ".join([f"{RANK_PREFIXES[i]}__{taxon}" for i, taxon in enumerate(taxonomy)])
 
 # Taxonomy TSV Utilities ---------------------------------------------------------------------------
 
 @dataclass(frozen=True, order=True)
 class TaxonomyEntry:
     __slots__ = ("identifier", "label")
@@ -295,15 +296,15 @@
                 recursive_insert(merged.taxon_tree_head, child)
         return merged
 
     def __init__(self, depth: int = 6):
         self.depth = depth
         self.taxon_tree_head = Taxon(-1, "_root_")
         self._taxon_to_id_map: Optional[Tuple[Dict[Taxon, int], ...]] = None
-        self._id_to_taxon_map: Optional[Tuple[Dict[int, Taxon], ...]] = None
+        self._id_to_taxon_map: Optional[Tuple[List[Taxon], ...]] = None
 
     def add_entries(self, entries: Iterable[TaxonomyEntry]):
         """
         Add taxonomy entries to the hierarchy.
 
         Args:
             entries (Iterable[TaxonomyEntry]): The taxonomy entries to add.
@@ -418,15 +419,15 @@
 
         Args:
             taxonomy (str): The taxonomy label to reduce (e.g. "k__Bacteria; ...").
 
         Returns:
             str: The reduced taxonomy label.
         """
-        return join_taxonomy(self.reduce_taxons(split_taxonomy(taxonomy)))
+        return join_taxonomy(self.reduce_taxons(split_taxonomy(taxonomy)), depth=self.depth)
 
     def reduce_taxons(self, taxons: Tuple[str, ...]) -> Tuple[str, ...]:
         """
         Reduce the taxonomy tuple to a valid known taxonomy in the hierarchy.
 
         Args:
             taxons (Tuple[str, ...]): The taxonomy tuple to reduce.
@@ -496,15 +497,15 @@
         Args:
             taxon_tokens (npt.NDArray[np.int64]): The taxonomy tokens.
             include_missing (bool): Assign missing taxons in the tokenized taxonomy to 0. Defaults to False.
 
         Returns:
             str: The detokenized taxonomy label.
         """
-        return join_taxonomy(self.detokenize_taxons(taxon_tokens, include_missing))
+        return join_taxonomy(self.detokenize_taxons(taxon_tokens, include_missing), depth=self.depth)
 
     def detokenize_taxons(
         self,
         taxon_tokens: npt.NDArray[np.int32],
         include_missing: bool = False
     ) -> Tuple[str, ...]:
         """
@@ -566,23 +567,24 @@
         if self._taxon_to_id_map is None:
             self._taxon_to_id_map = tuple({} for _ in range(self.depth))
             for taxon in self:
                 self._taxon_to_id_map[taxon.rank][taxon] = len(self._taxon_to_id_map[taxon.rank])
         return self._taxon_to_id_map
 
     @property
-    def id_to_taxon_map(self) -> Tuple[Dict[int, Taxon], ...]:
+    def id_to_taxon_map(self) -> Tuple[List[Taxon], ...]:
         """
         A mapping of taxon IDs to Taxon instances.
         """
         if self._id_to_taxon_map is None:
-            self._id_to_taxon_map = tuple({} for _ in range(self.depth))
+            self._id_to_taxon_map = tuple([] for _ in range(self.depth))
             for taxon in self:
-                taxon_id = self.taxon_to_id_map[taxon.rank][taxon]
-                self._id_to_taxon_map[taxon.rank][taxon_id] = taxon
+                # taxon_id = self.taxon_to_id_map[taxon.rank][taxon]
+                # assert len(self._id_to_taxon_map[taxon.rank]) == taxon_id
+                self._id_to_taxon_map[taxon.rank].append(taxon)
         return self._id_to_taxon_map
 
     def __eq__(self, other: "TaxonomyHierarchy"):
         """
         Check if two taxonomy hierarchies are equal.
         """
         for taxon, other_taxon in zip(self, other):
@@ -590,22 +592,19 @@
                 return False
         return True
 
     def __iter__(self) -> Generator[Taxon, None, None]:
         """
         Breadth-first sorted iteration over the taxonomy hierarchy.
         """
-        q: list[Taxon] = []
-        for child in self.taxon_tree_head:
-            heapq.heappush(q, child)
+        q: list[Taxon] = sorted(self.taxon_tree_head.children.values())
         while len(q) > 0:
-            taxon = heapq.heappop(q)
+            taxon = q.pop(0)
             yield taxon
-            for child in taxon:
-                heapq.heappush(q, child)
+            q += sorted(taxon.children.values())
 
 def entries(
     taxonomy: Union[io.TextIOBase, Iterable[TaxonomyEntry], str, Path]
 ) -> Iterable[TaxonomyEntry]:
     """
     Create an iterator over a taxonomy file or iterable of taxonomy entries.
     """
```

### Comparing `dnadb-0.6.4/src/dnadb/utils.py` & `dnadb-0.7.0/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.4/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.7.0/src/dnadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.6.4
+Version: 0.7.0
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.6.4/src/dnadb.egg-info/SOURCES.txt` & `dnadb-0.7.0/src/dnadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

