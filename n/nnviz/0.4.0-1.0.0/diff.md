# Comparing `tmp/nnviz-0.4.0.tar.gz` & `tmp/nnviz-1.0.0.tar.gz`

## Comparing `nnviz-0.4.0.tar` & `nnviz-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/__init__.py
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/dataspec.py
--rw-r--r--   0        0        0    11104 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/cli/__init__.py
--rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/cli/main.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/colors/__init__.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/colors/base.py
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/colors/bubble.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/colors/hashcolor.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/drawing/__init__.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/drawing/base.py
--rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/drawing/graphviz.py
--rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/inspection/__init__.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/inspection/base.py
--rw-r--r--   0        0        0    17686 2020-02-02 00:00:00.000000 nnviz-0.4.0/nnviz/inspection/torchfx.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 nnviz-0.4.0/.gitignore
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 nnviz-0.4.0/LICENSE
--rw-r--r--   0        0        0    15083 2020-02-02 00:00:00.000000 nnviz-0.4.0/README.md
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 nnviz-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    16809 2020-02-02 00:00:00.000000 nnviz-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/__init__.py
+-rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/dataspec.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/cli/__init__.py
+-rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/cli/main.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/colors/__init__.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/colors/base.py
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/colors/bubble.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/colors/hashcolor.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/drawing/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/drawing/base.py
+-rw-r--r--   0        0        0    15065 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/drawing/graphviz.py
+-rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/inspection/__init__.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/inspection/base.py
+-rw-r--r--   0        0        0    18035 2020-02-02 00:00:00.000000 nnviz-1.0.0/nnviz/inspection/torchfx.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nnviz-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 nnviz-1.0.0/LICENSE
+-rw-r--r--   0        0        0    15083 2020-02-02 00:00:00.000000 nnviz-1.0.0/README.md
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 nnviz-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    16808 2020-02-02 00:00:00.000000 nnviz-1.0.0/PKG-INFO
```

### Comparing `nnviz-0.4.0/nnviz/dataspec.py` & `nnviz-1.0.0/nnviz/dataspec.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,26 +41,34 @@
         pass
 
 
 class PrettyDataSpecVisitor(DataSpecVisitor):
     """Visitor for the `DataSpec` class that produces a pretty string representation."""
 
     def __init__(self):
+        """Constructor. Accepts no arguments and returns an initialized visitor."""
         self._indent = 0
         self._key = ""
         self._template = "{indent}{key}{entry}\n"
 
         self._result = ""
 
     @property
     def has_control(self) -> bool:
         return True
 
     @property
     def result(self) -> str:
+        """The result of the visitation. This property is only valid after the
+        `visit` method has been called, or after the `accept` method has been
+        called on a `DataSpec` instance, passin this visitor as an argument.
+
+        Returns:
+            str: A string representation of the visited `DataSpec` instance.
+        """
         return self._result
 
     def _entry(self, body: str) -> str:
         key_fmt = self._key + ": " if self._key else ""
         indent = " " * 4 * self._indent
         return self._template.format(indent=indent, key=key_fmt, entry=body)
 
@@ -97,85 +105,109 @@
         self._end_composite("}", _old_key)
 
     def visit_unknown_spec(self, spec: UnknownSpec) -> None:
         self._result += self._entry("???")
 
 
 class DataSpec(pyd.BaseModel, ABC):
-    """Specification of the data that is passed through the graph."""
+    """Models a synthetic representation of the data type passing through the graph.
+    Currently, this hierarchy can model tensors, builtin types, lists and maps. All
+    other types are represented as `UnknownSpec`.
+    """
 
     class Config:
         frozen = True
 
     spec_type: t.Literal[""] = ""
+    """DataSpec type discriminator. Do not set this field manually."""
 
     @abstractmethod
     def accept(self, visitor: DataSpecVisitor) -> None:
         """Accepts an incoming visitor."""
         pass
 
     @classmethod
     def build(cls, data: t.Any) -> DataSpec:
+        """Creates a `DataSpec` instance from a given data object.
+
+        Args:
+            data (t.Any): The data object to build the `DataSpec` from. Can be anything.
+
+        Returns:
+            DataSpec: The `DataSpec` instance that models the given data object.
+        """
         if isinstance(data, torch.Tensor):
             return TensorSpec(shape=data.shape, dtype=str(data.dtype))
         elif isinstance(data, (list, tuple)):
             return ListSpec(elements=[cls.build(x) for x in data])
         elif isinstance(data, dict):
             return MapSpec(elements={k: cls.build(v) for k, v in data.items()})
         elif isinstance(data, (int, float, str, bool, type(None), type(...), bytes)):
             return BuiltInSpec(name=data.__class__.__name__)
         else:
             return UnknownSpec()
 
     def pretty(self) -> str:
+        """Pretty string representation for terminal output.
+
+        Returns:
+            str: A pretty string representation of the `DataSpec` instance.
+        """
         visitor = PrettyDataSpecVisitor()
         self.accept(visitor)
         return visitor.result
 
 
 class TensorSpec(DataSpec):
     """Specification of the data that is passed through the graph."""
 
     spec_type: t.Literal["tensor"] = "tensor"
-    shape: t.Sequence[int] = pyd.Field(
-        default_factory=list, description="Shape of the tensor."
-    )
-    dtype: str = pyd.Field("", description="Data type of the tensor.")
+    """DataSpec type discriminator. Do not set this field manually."""
+
+    shape: t.Sequence[int] = pyd.Field(default_factory=list)
+    """Shape of the tensor."""
+
+    dtype: str = ""
+    """Data type of the tensor."""
 
     def accept(self, visitor: DataSpecVisitor) -> None:
         visitor.visit_tensor_spec(self)
 
 
 class BuiltInSpec(DataSpec):
     """Specification of the data that is passed through the graph."""
 
     spec_type: t.Literal["builtin"] = "builtin"
-    name: str = pyd.Field("", description="Name of the builtin type.")
+    """DataSpec type discriminator. Do not set this field manually."""
+
+    name: str = ""
+    """Name of the builtin type."""
 
     def accept(self, visitor: DataSpecVisitor) -> None:
         visitor.visit_builtin_spec(self)
 
 
 class UnknownSpec(DataSpec):
     """Specification of the data that is passed through the graph."""
 
     spec_type: t.Literal["unknown"] = "unknown"
+    """DataSpec type discriminator. Do not set this field manually."""
 
     def accept(self, visitor: DataSpecVisitor) -> None:
         visitor.visit_unknown_spec(self)
 
 
 class ListSpec(DataSpec):
     """Specification of the data that is passed through the graph."""
 
     spec_type: t.Literal["list"] = "list"
+    """DataSpec type discriminator. Do not set this field manually."""
 
-    elements: t.Sequence[t_any_spec] = pyd.Field(
-        default_factory=list, description="List of elements in the list."
-    )
+    elements: t.Sequence[t_any_spec] = pyd.Field(default_factory=list)
+    """List of elements in the list."""
 
     @pyd.validator("elements")
     def validate_elements(cls, v):
         return [pyd.parse_obj_as(t_any_spec, v) for v in v]
 
     def accept(self, visitor: DataSpecVisitor) -> None:
         visitor.visit_list_spec(self)
@@ -184,18 +216,18 @@
                 element.accept(visitor)
 
 
 class MapSpec(DataSpec):
     """Specification of the data that is passed through the graph."""
 
     spec_type: t.Literal["map"] = "map"
+    """DataSpec type discriminator. Do not set this field manually."""
 
-    elements: t.Mapping[str, t_any_spec] = pyd.Field(
-        default_factory=dict, description="Mapping of keys to elements in the map."
-    )
+    elements: t.Mapping[str, t_any_spec] = pyd.Field(default_factory=dict)
+    """Mapping of keys to elements in the map."""
 
     @pyd.validator("elements")
     def validate_elements(cls, v):
         return {k: pyd.parse_obj_as(t_any_spec, v) for k, v in v.items()}
 
     def accept(self, visitor: DataSpecVisitor) -> None:
         visitor.visit_map_spec(self)
```

### Comparing `nnviz-0.4.0/nnviz/entities.py` & `nnviz-1.0.0/nnviz/entities.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,100 +9,114 @@
 from nnviz import dataspec
 
 
 class NodeModel(pyd.BaseModel):
     """Pydantic model for a node in the graph. Contains some information about a layer
     of a neural network."""
 
-    type_: t.Literal[""] = ""
+    node_type: t.Literal[""] = ""
+    """NodeModel type discriminator. Do not set this field manually."""
 
-    name: str = pyd.Field(..., description="Qualified name of the node.")
-    path: t.Sequence[str] = pyd.Field(
-        default_factory=list,
-        description="Path of the node. E.g. ['features', '0', 'conv1']",
-    )
+    name: str = pyd.Field(...)
+    """Qualified name of the node."""
+
+    path: t.Sequence[str] = pyd.Field(default_factory=list)
+    """Path of the node. E.g. ['features', '0', 'conv1']"""
 
 
 class OpNodeModel(NodeModel):
     """`NodeModel` specialized for an operation node."""
 
-    type_: t.Literal["op"] = "op"
+    node_type: t.Literal["op"] = "op"
+    """NodeModel type discriminator. Do not set this field manually."""
+
+    op: str = ""
+    """Name of the operation. E.g. 'Conv2d'."""
+
+    full_op: str = ""
+    """Full name of the operation. E.g. 'torch.nn.modules.conv.Conv2d'."""
+
+    const_args: t.Sequence[t.Any] = pyd.Field(default_factory=list)
+    """Constant positional arguments of the operation."""
 
-    op: str = pyd.Field("", description="Name of the operation. E.g. 'Conv2d'.")
-    full_op: str = pyd.Field(
-        "",
-        description="Full name of the operation. E.g. 'torch.nn.modules.conv.Conv2d'.",
-    )
-    const_args: t.Sequence[t.Any] = pyd.Field(
-        default_factory=list,
-        description="Constant positional arguments of the operation.",
-    )
-    const_kwargs: t.Mapping[str, t.Any] = pyd.Field(
-        default_factory=dict, description="Constant keyword arguments of the operation."
-    )
-    n_parameters: int = pyd.Field(0, description="Number of parameters.")
-    perc_parameters: float = pyd.Field(0.0, description="Percentage of parameters.")
+    const_kwargs: t.Mapping[str, t.Any] = pyd.Field(default_factory=dict)
+    """Constant keyword arguments of the operation."""
+
+    n_parameters: int = 0
+    """Number of parameters of the operation."""
+
+    perc_parameters: float = 0.0
+    """Percentage of parameters of the operation."""
 
 
 class CollapsedNodeModel(NodeModel):
     """`NodeModel` specialized for a collapsed node."""
 
-    type_: t.Literal["collapsed"] = "collapsed"
+    node_type: t.Literal["collapsed"] = "collapsed"
+    """NodeModel type discriminator. Do not set this field manually."""
 
-    n_parameters: int = pyd.Field(0, description="Number of parameters.")
-    perc_parameters: float = pyd.Field(0.0, description="Percentage of parameters.")
+    n_parameters: int = 0
+    """Number of parameters of the collapsed node."""
+
+    perc_parameters: float = 0.0
+    """Percentage of parameters of the collapsed node."""
 
 
 class InputNodeModel(NodeModel):
     """`NodeModel` specialized for an input node."""
 
-    type_: t.Literal["input"] = "input"
+    node_type: t.Literal["input"] = "input"
+    """NodeModel type discriminator. Do not set this field manually."""
 
 
 class OutputNodeModel(NodeModel):
     """`NodeModel` specialized for an output node."""
 
-    type_: t.Literal["output"] = "output"
+    node_type: t.Literal["output"] = "output"
+    """NodeModel type discriminator. Do not set this field manually."""
 
 
 t_any_node = t.Union[
     NodeModel, OpNodeModel, CollapsedNodeModel, InputNodeModel, OutputNodeModel
 ]
 
 
 class GraphMeta(pyd.BaseModel):
     """Pydantic model for the metadata associated with the graph."""
 
-    title: str = pyd.Field("", description="Title of the graph.")
-    source: str = pyd.Field("", description="Where the graph comes from.")
-    source_version: str = pyd.Field("", description="Graph source version.")
-    nnviz_version: str = pyd.Field(
-        nnviz.__version__, description="Version of nnviz used to generate the graph."
-    )
+    title: str = ""
+    """Title of the graph."""
+
+    source: str = ""
+    """Where the graph comes from."""
+
+    source_version: str = ""
+    """Graph source library version."""
+
+    nnviz_version: str = pyd.Field(nnviz.__version__)
+    """Version of nnviz used to generate the graph."""
 
 
 class GraphData(pyd.BaseModel):
     """Pydantic model for the data associated with the graph. It consists of an anemic
     representation of the graph, i.e. a mapping of nodes and a list of edges.
     This is done to make it easier to serialize and deserialize the graph, without
     having to deal with the networkx graph representation.
     """
 
-    nodes: t.Mapping[str, t_any_node] = pyd.Field(
-        default_factory=dict, description="Mapping (node -> node model)."
-    )
+    nodes: t.Mapping[str, t_any_node] = pyd.Field(default_factory=dict)
+    """Mapping of nodes names to their models."""
+
     edges: t.Sequence[
         t.Tuple[str, str, str, t.Optional[dataspec.t_any_spec]]
-    ] = pyd.Field(
-        default_factory=list,
-        description="List of edges. As tuples (src, tgt, key, [spec]).",
-    )
-    metadata: GraphMeta = pyd.Field(
-        GraphMeta(), description="Metadata associated with the graph."  # type: ignore
-    )
+    ] = pyd.Field(default_factory=list)
+    """List of edges. As tuples (src, tgt, key, [spec])."""
+
+    metadata: GraphMeta = GraphMeta()  # type: ignore
+    """Metadata associated with the graph."""
 
 
 class NNGraph:
     """Graph representation of a neural network."""
 
     MODEL_KEY = "model"
     """Key used to store the `NodeModel` in the graph nodes."""
@@ -139,17 +153,21 @@
             graph (nx.MultiDiGraph): NetworkX graph wrapped by this class.
             metadata (GraphMeta): Metadata associated with the graph.
         """
         self._graph = graph
         self._metadata = metadata
 
     def __getitem__(self, name: str) -> NodeModel:
+        """Returns the model associated with the node name."""
         return self._graph.nodes[name][self.MODEL_KEY]
 
     def __setitem__(self, name: str, model: NodeModel) -> None:
+        """Sets the model associated with the node name. And, if the node does not
+        exist, it is created.
+        """
         if name in self._graph.nodes:
             self._graph.nodes[name][self.MODEL_KEY] = model
         else:
             self._graph.add_node(name, model=model)
 
     @property
     def nodes(self) -> t.Iterable[str]:
@@ -210,14 +228,20 @@
 
         Returns:
             t.Optional[DataSpec]: The data spec associated with the edge.
         """
         return self._graph.edges[source, target, key].get(self.SPEC_KEY, None)
 
     def collapse(self, path: t.Sequence[str]) -> None:
+        """Garther all nodes sharing the same path prefix and collapse them into a
+        single collapsed node. This operation is done in place and is not reversible.
+
+        Args:
+            path (t.Sequence[str]): The path prefix to collapse.
+        """
         # Find all nodes sharing the same path prefix
         to_coll = [n for n in self.nodes if tuple(self[n].path[: len(path)]) == path]
 
         # Gather their models
         models = [self[n] for n in to_coll]
 
         # [Get number of parameters for each node]
```

### Comparing `nnviz-0.4.0/nnviz/cli/main.py` & `nnviz-1.0.0/nnviz/cli/main.py`

 * *Files identical despite different names*

### Comparing `nnviz-0.4.0/nnviz/colors/bubble.py` & `nnviz-1.0.0/nnviz/colors/bubble.py`

 * *Files 24% similar despite different names*

```diff
@@ -173,70 +173,7 @@
             sub_tree.spawn(args[0])
 
         # Recurse on the sub-tree with the first argument removed
         return self._pick_recur(sub_tree[args[0]], *args[1:])
 
     def pick(self, *args: t.Hashable) -> colors.RGBColor:
         return self._pick_recur(self._color_tree, *args)
-
-
-if __name__ == "__main__":  # pragma: no cover
-    import random
-
-    import cv2 as cv
-
-    cv.namedWindow("sasso", cv.WINDOW_NORMAL)
-    H = W = 512
-    cv.resizeWindow("sasso", H, W)
-
-    bubble = _BubbleTree(np.array([0, 0]), 1.0, {})
-
-    depth = 3
-    possible_keys = [chr(i) for i in range(ord("a"), ord("a") + 21)]
-
-    while True:
-        canvas = np.zeros((H, W, 3))
-
-        # Sample with replacement from the possible keys
-        args = [random.choice(possible_keys) for _ in range(depth)]
-        # Add some other random arguments
-        args += [random.random() for _ in range(2)]
-
-        def add_args(tree: _BubbleTree, args: t.List[t.Hashable]) -> None:
-            if len(args) == 0:
-                return
-
-            if args[0] not in tree:
-                tree.spawn(args[0])
-
-            add_args(tree[args[0]], args[1:])
-
-        add_args(bubble, args)  # type: ignore
-
-        def visit(tree: _BubbleTree, d: int) -> None:
-            row, col = int(tree.origin[0] * H // 2 + H // 2), int(
-                tree.origin[1] * H // 2 + H // 2
-            )
-            if len(tree.children) == 0:
-                canvas[row, col, :] = 255
-
-            if d <= depth and d > 0:
-                # Draw a circle around the origin of the tree
-                cv.circle(
-                    canvas,
-                    (col, row),
-                    int(tree.radius * H // 2),
-                    (0, 0, 255 // d),
-                    thickness=1,
-                )
-
-            for child in tree.children.values():
-                visit(child, d + 1)
-
-        visit(bubble, 0)
-
-        canvas = (canvas / np.max(canvas) * 255).astype(np.uint8)
-        cv.imshow("sasso", cv.cvtColor(canvas, cv.COLOR_RGB2BGR))
-        key = cv.waitKey(1)
-
-        if key == ord("q"):
-            break
```

### Comparing `nnviz-0.4.0/nnviz/drawing/base.py` & `nnviz-1.0.0/nnviz/drawing/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from abc import ABC, abstractmethod
 
 from nnviz import entities as ent
 
 
 class GraphDrawer(ABC):
-    """An abstract class for drawing a neural network graph. All nnviz graph drawers
+    """NNViz interface for drawing a neural network graph. All nnviz graph drawers
     should inherit from this class.
     """
 
     @abstractmethod
     def draw(self, nngraph: ent.NNGraph) -> None:
         """Draw a neural network graph. This method returns nothing, to avoid making
         decisions about where to save/display/return the graph. The implementation of
-        this interface can add custom logic to save/display/return the graph separately.
+        this interface can add custom logic to save/display/store the graph separately.
 
         Args:
             nngraph (NNGraph): The neural network graph to draw.
         """
         pass
```

### Comparing `nnviz-0.4.0/nnviz/drawing/graphviz.py` & `nnviz-1.0.0/nnviz/drawing/graphviz.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from nnviz import entities as ent
 
 
 class HTMLSpecVisitor(dataspec.DataSpecVisitor):
     """Visitor for the `DataSpec` class that produces an HTML table nesting."""
 
     def __init__(self) -> None:
+        """Constructor. Accepts no arguments. and initializes the visitor."""
         super().__init__()
         self._code = ""
         self._name_stack: t.List[t.List[str]] = []
         self._code_stack: t.List[str] = []
 
     def _end_visit(self, code: str) -> None:
         if len(self._name_stack) > 0:
@@ -162,26 +163,38 @@
 
 
 class GraphvizDrawer(drawing.GraphDrawer):
     """A graph drawer that uses Graphviz to draw a neural network graph."""
 
     def __init__(
         self,
-        path: Path,
+        path: t.Union[str, Path],
         color_picker: t.Optional[colors.ColorPicker] = None,
         style: t.Optional[GraphvizDrawerStyle] = None,
     ) -> None:
-        self._path = path
+        """Constructor.
+
+        Args:
+            path (t.Union[str, Path]): The path to save the graph to. Can be
+             a .png, .pdf, .svg file.
+            color_picker (t.Optional[colors.ColorPicker], optional): The color picker to
+             use for this drawer. If left to none, a color picker will be chosen
+             automatically. Defaults to None.
+            style (t.Optional[GraphvizDrawerStyle], optional): The style object to use
+            see `GraphvizDrawerStyle` for details. If left to none, a default style
+            will be chosen automatically. Defaults to None.
+        """
+        self._path = Path(path)
         self._color_picker = color_picker or colors.BubbleColorPicker()
         self._style = style or GraphvizDrawerStyle()
         self._ignore_prefixes = ["torch.nn."]
 
     def _text_color(self, color: colors.RGBColor) -> str:
         not_filled = "filled" not in self._style.node_style
-        return "black" if color.is_bright() or not_filled else "white"
+        return "black" if color.brightness > 128 or not_filled else "white"
 
     def _multi_line(self, *lines: str) -> str:
         multi_line = "<BR/>".join(lines)
         return f"<{multi_line}>"
 
     def _pick_color_for_op_node(self, node: ent.OpNodeModel) -> colors.RGBColor:
         filtered_op = node.full_op
@@ -203,15 +216,15 @@
             n_params_fmt = _human_format(node.n_parameters)
             perc_params_fmt = _human_format(node.perc_parameters * 100) + "%"
             lines.append(f"<B>params</B>: {n_params_fmt} ({perc_params_fmt})")
         return lines
 
     def _op_params(self, node: ent.OpNodeModel) -> t.Dict[str, t.Any]:
         rgb = self._pick_color_for_op_node(node)
-        color = rgb.to_hex()
+        color = rgb.hex
         font_c = self._text_color(rgb)
 
         title_fsize = self._style.node_title_font_size
         lines = [f'<B><FONT POINT-SIZE="{title_fsize}">{node.op}</FONT></B>']
 
         if self._style.show_node_name:
             lines.append(f"<I>{node.name}</I>")
@@ -237,15 +250,15 @@
         label = self._multi_line(*lines)
         return {"label": label, "color": color, "fillcolor": color, "fontcolor": font_c}
 
     def _input_output_params(
         self, node: ent.NodeModel, title: str
     ) -> t.Dict[str, t.Any]:
         rgb = colors.RGBColor(0, 0, 0)
-        color = rgb.to_hex()
+        color = rgb.hex
         font_c = self._text_color(rgb)
 
         fsize = self._style.node_title_font_size
         lines = [f'<B><FONT POINT-SIZE="{fsize}">{title}</FONT></B>']
         if self._style.show_node_name:
             lines.append(f"<I>{node.name}</I>")
 
@@ -256,15 +269,15 @@
         return self._input_output_params(node, "Input")
 
     def _output_params(self, node: ent.OutputNodeModel) -> t.Dict[str, t.Any]:
         return self._input_output_params(node, "Output")
 
     def _collapsed_params(self, node: ent.CollapsedNodeModel) -> t.Dict[str, t.Any]:
         rgb = self._color_picker.pick(*node.path[:-1])
-        color = rgb.to_hex()
+        color = rgb.hex
         font_c = self._text_color(rgb)
 
         joined_path = ".".join(node.path)
         joined_path = joined_path if len(joined_path) > 0 else "root"
         fsize = self._style.node_title_font_size
         lines = [f'<B><FONT POINT-SIZE="{fsize}">{joined_path}</FONT></B>']
 
@@ -278,21 +291,21 @@
     def _node_params(self, node: ent.NodeModel) -> t.Dict[str, t.Any]:
         type_map = {
             "op": self._op_params,
             "input": self._input_params,
             "output": self._output_params,
             "collapsed": self._collapsed_params,
         }
-        params = type_map[node.type_](node)
+        params = type_map[node.node_type](node)
         return {**self._style.default_node_params(), **params}
 
     def _subgraph_params(self, name: str, depth: int) -> t.Dict[str, t.Any]:
         # Bg color is a function of depth
         gray_level = int(255 * (1 / (depth / 10 + 1.1)))
-        bgcolor = colors.RGBColor(gray_level, gray_level, gray_level).to_hex()
+        bgcolor = colors.RGBColor(gray_level, gray_level, gray_level).hex
 
         # Label is the name of the subgraph
         body = name.partition("cluster_")[2]
         fsize = self._style.cluster_title_font_size
         label = f'<<B><FONT POINT-SIZE="{fsize}">{body}</FONT></B>>'
 
         params = {"label": label, "bgcolor": bgcolor, "labeljust": "l"}
@@ -332,15 +345,15 @@
         lines = []
         if nngraph.metadata.title:
             body = nngraph.metadata.title
             fsize = self._style.graph_title_font_size
             lines.append(f'<B><FONT POINT-SIZE="{fsize}">{body}</FONT></B>')
 
         if nngraph.metadata.source:
-            body = f"<B>Source:</B> {nngraph.metadata.source}"
+            body = f"<B>Source: </B> {nngraph.metadata.source}"
             if nngraph.metadata.source_version:
                 body += f" v{nngraph.metadata.source_version}"
             lines.append(body)
 
         lines.append(f"<B>NNViz </B>v{nngraph.metadata.nnviz_version}")
         lines.append(" ")
 
@@ -349,23 +362,27 @@
 
     def _convert(self, nngraph: ent.NNGraph) -> pgv.AGraph:
         # Initialize a pygraphviz graph
         graph_params = self._graph_params(nngraph)
         pgvgraph = pgv.AGraph(directed=True, strict=False, **graph_params)
 
         # Populate nodes
-        for node in nngraph.nodes:
+        for node in sorted(nngraph.nodes):
             model = nngraph[node]
             target_graph = self._get_tgt_graph_by_path(pgvgraph, model.path)
             target_graph.add_node(node, **self._node_params(model))
 
         # Populate edges
         for source, target, key in nngraph.edges:
             spec = nngraph.get_spec(source, target, key)
             pgvgraph.add_edge(source, target, **self._edge_params(spec))
 
         return pgvgraph
 
     def draw(self, nngraph: ent.NNGraph) -> None:
-        converted = self._convert(nngraph)
+        # Hardcoded to dot, because the other options suck ass.
         prog = "dot"
+
+        # Convert and draw to file
+        converted = self._convert(nngraph)
+        self._path.parent.mkdir(parents=True, exist_ok=True)
         converted.draw(self._path, prog=prog)
```

### Comparing `nnviz-0.4.0/nnviz/inspection/__init__.py` & `nnviz-1.0.0/nnviz/inspection/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,70 +50,97 @@
 
 def load_from_dynamic_import(model: str) -> t.Any:
     """Import a symbol from a python file or module. The file or module can be anywhere
     in the file system, it will be added to the python path.
 
     Args:
         model (str): The path to the python file or module, followed by a colon and the
+            name of the symbol to import.
 
     Returns:
         t.Any: The imported symbol.
     """
     path, _, symbol_name = model.rpartition(":")
     if path.endswith(".py"):
         return load_from_file_import(path, symbol_name)
     else:
         return load_from_module_import(path, symbol_name)
 
 
+def _parse_argstr(argstr: str) -> t.Tuple[t.Tuple, t.Dict]:
+    args = []
+    kwargs = {}
+    for arg in argstr.split(";"):
+        if not arg:
+            continue
+        if "=" in arg:
+            key, _, value = arg.partition("=")
+            kwargs[key] = eval(value)
+        else:
+            args.append(eval(arg))
+
+    return tuple(args), kwargs
+
+
 def load_from_string(model: str) -> nn.Module:
-    """Load a model from a string. The string can be either the name of a model in
+    """Load a model from a string.
 
     Args:
-        model (str): The name of the model to load.
+        model (str): The name of the model to load. The string must have the following
+            format:
+
+            - <module>:<symbol>;[args][kwargs] -> load a model from a module/file
+            - <symbol>;[args][kwargs] -> load a model from `torchvision.models`
+
+            Args and kwargs are ; separated and currently only support strings and
+            numbers. Kwargs are passed as <key>=<value> pairs.
 
     Raises:
         ValueError: If the model could not be loaded.
 
     Returns:
         nn.Module: The loaded model.
     """
-    if ":" not in model:
-        smb = load_from_torchvision(model)
+    symbol, _, argstr = model.partition(";")
+    args, kwargs = _parse_argstr(argstr)
+
+    if ":" not in symbol:
+        smb = load_from_torchvision(symbol)
     else:
-        smb = load_from_dynamic_import(model)
+        smb = load_from_dynamic_import(symbol)
 
     if isinstance(smb, nn.Module):
         return smb
 
     if callable(smb):
-        return smb()
+        return smb(*args, **kwargs)
 
     raise ValueError(f"Could not load model {model}")
 
 
 DEFAULT_KEY = "x"
-"""The default key to use when the input is a single tensor."""
+"""The default key to use when the input is a single tensor.
+"""
 
 
 def parse_input_str(in_str: t.Optional[str]) -> t.Optional[t.Dict]:
     """Parse an input string to a dictionary of tensors.
 
     Args:
         in_str (t.Optional[str]): The input string, can be:
 
             - None -> None
             - default -> float32 BCHW tensor of shape (1, 3, 224, 224) (commonly used)
             - image<side> (e.g. image224, image256, ...) -> float32 BCHH tensor
             - image<height>x<width> (e.g. image224x224, image256x512, ...) -> float32
-            BCHW tensor
+              BCHW tensor
             - tensor<s0>x<s1>x<s2>x... (e.g. tensor1x3x224x224, tensor1x3x256x512, ...)
-            -> float32 generic tensors
-            - <key1>:<value1>;<key2>:<value2>;... (e.g. x:tensor1x30;y:tensor1x40,
-            ...) -> dictionary of tensors
+              -> float32 generic tensors
+            - <key1>:<value1>;<key2>:<value2>;... (e.g. x:tensor1x30;y:tensor1x40;...)
+              -> dictionary of tensors
 
     Returns:
         t.Optional[t.Dict]: A dictionary of tensors to use as input for the model.
     """
     # If the input is None, exit early returning None
     if in_str is None:
         return None
```

### Comparing `nnviz-0.4.0/nnviz/inspection/base.py` & `nnviz-1.0.0/nnviz/inspection/base.py`

 * *Files identical despite different names*

### Comparing `nnviz-0.4.0/nnviz/inspection/torchfx.py` & `nnviz-1.0.0/nnviz/inspection/torchfx.py`

 * *Files 3% similar despite different names*

```diff
@@ -296,14 +296,20 @@
             )
             warnings.warn(msg)
             return None
 
         return specs
 
     def call_module(self, m: nn.Module, forward: t.Callable, args, kwargs):
+        """Override the call_module method to keep track of the current module qualname.
+
+        I have to override this docstring because the original one sucks so much that
+        it cannot even be rendered by Sphinx. I'm not even kidding. For the brave, refer
+        to the original pytorch source code, I have had enough of this.
+        """
         old_qualname = self.current_module_qualname
         try:
             module_qualname = self.path_of_module(m)
             self._qualname_to_callable[module_qualname] = m
             self.current_module_qualname = module_qualname
             if not self.is_leaf_module(m, module_qualname):
                 return forward(*args, **kwargs)
```

### Comparing `nnviz-0.4.0/.gitignore` & `nnviz-1.0.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -128,14 +128,17 @@
 # Pyre type checker
 .pyre/
 
 # NNViz outputs
 *.pdf
 *.svg
 *.json
-!examples/*.pdf
-!examples/*.svg
-!examples/*.json
+!docs/**/*.pdf
+!docs/**/*.svg
+!docs/**/*.json
+!examples/**/*.pdf
+!examples/**/*.svg
+!examples/**/*.json
 
 # VSCode
 .vscode/
 .vs/
```

### Comparing `nnviz-0.4.0/LICENSE` & `nnviz-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nnviz-0.4.0/README.md` & `nnviz-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nnviz-0.4.0/pyproject.toml` & `nnviz-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -39,27 +39,27 @@
 
 [project.optional-dependencies]
 tests = [
     "pytest",
     "pytest-cov",
 ]
 dev = [
-    "pylama",
     "black",
     "flake8",
+    "ruff",
 ]
 build = [
     "hatch",
     "build",
 ]
 docs = [
-    "Sphinx==5.1.1",
-    "sphinx-material==0.0.35",
-    "myst-parser==0.18.0",
-    "sphinxcontrib-mermaid==0.7.1",
+    "Sphinx==6.1.3",
+    "sphinx-immaterial==0.11.3",
+    "myst-parser==1.0.0",
+    "sphinxcontrib-mermaid==0.8.1",
 ]
 
 [project.urls]
 "Source" = "https://github.com/lucabonfiglioli/nnviz"
 "Issues" = "https://github.com/lucabonfiglioli/nnviz/issues"
 
 [project.scripts]
```

### Comparing `nnviz-0.4.0/PKG-INFO` & `nnviz-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnviz
-Version: 0.4.0
+Version: 1.0.0
 Summary: Neural models visualization.
 Project-URL: Source, https://github.com/lucabonfiglioli/nnviz
 Project-URL: Issues, https://github.com/lucabonfiglioli/nnviz/issues
 Author-email: LucaBonfiglioli <luca.bonfiglioli@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 License-File: LICENSE
 Keywords: deeplearning,graph,neural,nnviz,visualization
@@ -28,20 +28,20 @@
 Requires-Dist: typer>=0.6.0
 Provides-Extra: build
 Requires-Dist: build; extra == 'build'
 Requires-Dist: hatch; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
-Requires-Dist: pylama; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: myst-parser==0.18.0; extra == 'docs'
-Requires-Dist: sphinx-material==0.0.35; extra == 'docs'
-Requires-Dist: sphinx==5.1.1; extra == 'docs'
-Requires-Dist: sphinxcontrib-mermaid==0.7.1; extra == 'docs'
+Requires-Dist: myst-parser==1.0.0; extra == 'docs'
+Requires-Dist: sphinx-immaterial==0.11.3; extra == 'docs'
+Requires-Dist: sphinx==6.1.3; extra == 'docs'
+Requires-Dist: sphinxcontrib-mermaid==0.8.1; extra == 'docs'
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # 📊 NNViz
```

