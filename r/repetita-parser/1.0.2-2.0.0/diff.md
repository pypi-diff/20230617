# Comparing `tmp/repetita_parser-1.0.2.tar.gz` & `tmp/repetita_parser-2.0.0.tar.gz`

## Comparing `repetita_parser-1.0.2.tar` & `repetita_parser-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,32 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/src/repetita_parser/__init__.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/src/repetita_parser/demands.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/src/repetita_parser/errors.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/src/repetita_parser/instance.py
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/src/repetita_parser/topology.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/paths.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/test_demands.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/test_errors.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/test_instance.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/test_topology.py
--rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/DeutscheTelekom.0000.demands
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/DeutscheTelekom.graph
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_edge_fields.graph
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_edge_header.graph
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_edge_memo.graph
--rw-r--r--   0        0        0    18701 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_fields.demands
--rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_header.demands
--rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_memo.demands
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_node_fields.graph
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_node_header.graph
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_node_memo.graph
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/LICENSE
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/README.md
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/src/repetita_parser/__init__.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/src/repetita_parser/demands.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/src/repetita_parser/errors.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/src/repetita_parser/instance.py
+-rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/src/repetita_parser/topology.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/src/repetita_parser/types.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/paths.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/test_demands.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/test_errors.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/test_instance.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/test_topology.py
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/parsing/bad/bad_edge_fields.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/parsing/bad/bad_edge_header.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/parsing/bad/bad_edge_memo.graph
+-rw-r--r--   0        0        0    18701 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/parsing/bad/bad_fields.demands
+-rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/parsing/bad/bad_header.demands
+-rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/parsing/bad/bad_memo.demands
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/parsing/bad/bad_node_fields.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/parsing/bad/bad_node_header.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/parsing/bad/bad_node_memo.graph
+-rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/shared/DeutscheTelekom.0000.demands
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/shared/DeutscheTelekom.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/validation/bad/DeutscheTelekom.graph
+-rw-r--r--   0        0        0    18713 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/validation/bad/both_bad.demands
+-rw-r--r--   0        0        0    18710 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/validation/bad/dest_bad.demands
+-rw-r--r--   0        0        0    18709 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/tests/data/validation/bad/src_bad.demands
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/README.md
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 repetita_parser-2.0.0/PKG-INFO
```

### Comparing `repetita_parser-1.0.2/src/repetita_parser/topology.py` & `repetita_parser-2.0.0/src/repetita_parser/topology.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 from dataclasses import dataclass
-from os import PathLike
 from typing import List, NamedTuple
 
 from repetita_parser.errors import ParseError
+from repetita_parser.types import PathLike
 
 try:
     import networkx as nx
 except ImportError:
     _has_networkx = False
 else:
     _has_networkx = True
@@ -25,18 +25,20 @@
     dest: int
     weight: float
     bandwidth: float
     delay: float
 
 
 class Topology:
-    def __init__(self, nodes: List[Node], edges: List[Edge]) -> None:
+    def __init__(self, nodes: List[Node], edges: List[Edge], source_file: PathLike) -> None:
         self.nodes: List[Node] = nodes
         self.edges: List[Edge] = edges
 
+        self.source_file = source_file
+
     def as_nx_graph(self):
         """
         Convert the topology to a `networkx.MultiDiGraph`. In the graph, nodes
         are represented by their index into `self.nodes`. Node and edge objects
         carry their respective `Node` and `Edge` objects in their attributes
         under the `obj` key.
 
@@ -130,15 +132,15 @@
 
         state.line_idx += 1
 
     state.line_idx += 1
     return edges
 
 
-def parse(file_path: PathLike):
+def parse(file_path: PathLike) -> Topology:
     nodes_id = "NODES"
     edges_id = "EDGES"
 
     with open(file_path) as f:
         cur_line_idx = 0
         line = f.readline()
         fields = line.strip("\n").split()
@@ -157,8 +159,8 @@
 
         if fields[0] != edges_id:
             msg = "expected edges header line"
             raise ParseError(msg, file_path, cur_line_idx + 1)
 
         edges = _parse_edges(state)
 
-        return Topology(nodes, edges)
+        return Topology(nodes, edges, file_path)
```

### Comparing `repetita_parser-1.0.2/tests/test_topology.py` & `repetita_parser-2.0.0/tests/test_topology.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 
 import pytest
 from paths import TOPOLOGY_FILE_PATH
 
-from repetita_parser import topology
-from repetita_parser.errors import ParseError
+from repetita_parser import errors, topology
 
 
 def test_parse():
     topo = topology.parse(TOPOLOGY_FILE_PATH)
     assert len(topo.nodes) == 30
     assert len(topo.edges) == 110
 
@@ -28,27 +27,27 @@
 
     with pytest.raises(ImportError, match="NetworkX is required to call this function"):
         topo.as_nx_graph()
 
     topology._has_networkx = True
 
 
-def test_parse_errors():
-    root = Path("tests/data/bad")
+bad_root = Path("tests/data/parsing/bad")
 
-    with pytest.raises(ParseError, match="expected nodes header line"):
-        topology.parse(root / "bad_node_header.graph")
 
-    with pytest.raises(ParseError, match="expected nodes memo line"):
-        topology.parse(root / "bad_node_memo.graph")
-
-    with pytest.raises(ParseError, match="not all node fields present"):
-        topology.parse(root / "bad_node_fields.graph")
-
-    with pytest.raises(ParseError, match="expected edges header line"):
-        topology.parse(root / "bad_edge_header.graph")
-
-    with pytest.raises(ParseError, match="expected edges memo line"):
-        topology.parse(root / "bad_edge_memo.graph")
-
-    with pytest.raises(ParseError, match="not all edge fields present"):
-        topology.parse(root / "bad_edge_fields.graph")
+@pytest.mark.parametrize(
+    "topo_file, expectation",
+    [
+        (
+            bad_root / "bad_node_header.graph",
+            pytest.raises(errors.ParseError, match="expected nodes header line"),
+        ),
+        (bad_root / "bad_node_memo.graph", pytest.raises(errors.ParseError, match="expected nodes memo line")),
+        (bad_root / "bad_node_fields.graph", pytest.raises(errors.ParseError, match="not all node fields present")),
+        (bad_root / "bad_edge_header.graph", pytest.raises(errors.ParseError, match="expected edges header line")),
+        (bad_root / "bad_edge_memo.graph", pytest.raises(errors.ParseError, match="expected edges memo line")),
+        (bad_root / "bad_edge_fields.graph", pytest.raises(errors.ParseError, match="not all edge fields present")),
+    ],
+)
+def test_parse_errors(topo_file, expectation):
+    with expectation:
+        topology.parse(topo_file)
```

### Comparing `repetita_parser-1.0.2/tests/data/DeutscheTelekom.0000.demands` & `repetita_parser-2.0.0/tests/data/shared/DeutscheTelekom.0000.demands`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/tests/data/DeutscheTelekom.graph` & `repetita_parser-2.0.0/tests/data/shared/DeutscheTelekom.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/tests/data/bad/bad_edge_fields.graph` & `repetita_parser-2.0.0/tests/data/parsing/bad/bad_edge_fields.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/tests/data/bad/bad_edge_header.graph` & `repetita_parser-2.0.0/tests/data/parsing/bad/bad_edge_header.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/tests/data/bad/bad_edge_memo.graph` & `repetita_parser-2.0.0/tests/data/parsing/bad/bad_edge_memo.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/tests/data/bad/bad_fields.demands` & `repetita_parser-2.0.0/tests/data/parsing/bad/bad_fields.demands`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/tests/data/bad/bad_header.demands` & `repetita_parser-2.0.0/tests/data/parsing/bad/bad_header.demands`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/tests/data/bad/bad_memo.demands` & `repetita_parser-2.0.0/tests/data/parsing/bad/bad_memo.demands`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/tests/data/bad/bad_node_fields.graph` & `repetita_parser-2.0.0/tests/data/parsing/bad/bad_node_fields.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/tests/data/bad/bad_node_header.graph` & `repetita_parser-2.0.0/tests/data/parsing/bad/bad_node_header.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/tests/data/bad/bad_node_memo.graph` & `repetita_parser-2.0.0/tests/data/parsing/bad/bad_node_memo.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/.gitignore` & `repetita_parser-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/LICENSE` & `repetita_parser-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.2/README.md` & `repetita_parser-2.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,11 +18,13 @@
 
 ## Installation
 Via pip:
 ```bash
 pip install repetita-parser
 ```
 
+An AUR package under the name of [`python-repetita-parser`](https://aur.archlinux.org/packages/python-repetita-parser) is available as well.
+
 
 ## Data Format
 REPETITA defines two file formats, one for topology files and another for demand files.
 These formats are defined in the [REPETITA wiki](https://github.com/svissicchio/Repetita/wiki/Adding-Problem-Instances).
```

### Comparing `repetita_parser-1.0.2/pyproject.toml` & `repetita_parser-2.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "repetita-parser"
-version = "1.0.2"
+version = "2.0.0"
 description = "A parser for the REPETITA format"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 authors = [
   { name="Leon Richardt", email="pip@leon.dev" },
 ]
-classifiers = [
-  "Development Status :: 4 - Beta",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
-]
 dependencies = ["numpy"]
 
 [project.optional-dependencies]
 networkx = ["networkx"]
 
 [project.urls]
 Documentation = "https://github.com/leon-richardt/python-repetita-parser#readme"
```

