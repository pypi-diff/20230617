# Comparing `tmp/kast_flow_api_python-1.0.3.tar.gz` & `tmp/kast_flow_api_python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kast_flow_api_python-1.0.3.tar", max compression
+gzip compressed data, was "kast_flow_api_python-1.0.4.tar", max compression
```

## Comparing `kast_flow_api_python-1.0.3.tar` & `kast_flow_api_python-1.0.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-15 11:14:06.166894 kast_flow_api_python-1.0.3/kast_flow_api/__init__.py
--rw-r--r--   0        0        0     8864 2023-06-15 11:14:05.927894 kast_flow_api_python-1.0.3/kast_flow_api/v1.py
--rw-r--r--   0        0        0      528 2023-06-15 11:14:26.053940 kast_flow_api_python-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-17 13:00:30.531251 kast_flow_api_python-1.0.4/kast_flow_api/__init__.py
+-rw-r--r--   0        0        0     8058 2023-06-17 13:00:30.504251 kast_flow_api_python-1.0.4/kast_flow_api/v1.py
+-rw-r--r--   0        0        0      528 2023-06-17 13:00:50.763301 kast_flow_api_python-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.4/PKG-INFO
```

### Comparing `kast_flow_api_python-1.0.3/kast_flow_api/v1.py` & `kast_flow_api_python-1.0.4/kast_flow_api/v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from dataclasses import asdict, dataclass, field, fields
-from enum import Enum, StrEnum
+from enum import StrEnum
 from functools import wraps
 from typing import Any, Callable, Protocol, Self, Tuple, Type, TypeVar, cast
 
 from dacite import Config, from_dict
 
 
 class KastFormat(StrEnum):
@@ -22,33 +22,14 @@
                 message=[
                     ["KastFormat", f"shoud be one of {list(map(str, KastFormat))}"],
                 ],
                 errors=e,
             )
 
 
-class KastDataFrameBackend(Enum):
-    NOTSET = "notset"
-    PANDAS = "pandas"
-    PYSPARK = "pyspark"
-
-    @staticmethod
-    def from_string(s: str) -> "KastDataFrameBackend":
-        try:
-            return KastDataFrameBackend(s)
-        except KeyError:
-            raise KastInvalidDataFrameBackend(
-                message=[
-                    ["Error", "Unsupported DataFrame backend"],
-                    ["Given", s],
-                ],
-                errors=None,
-            )
-
-
 T = TypeVar("T")
 
 
 def kast_unmarshal(clazz: T) -> T:
     """Type ignore is necessary due to typechecker not supporting alias of dataclass
     see: https://github.com/python/mypy/issues/9875
     """
@@ -61,18 +42,14 @@
         ...
 
     @property
     def id(self: Self) -> str:
         ...
 
     @property
-    def backend(self: Self) -> KastDataFrameBackend:
-        ...
-
-    @property
     def schema(self: Self) -> Any:
         ...
 
     def createOrReplaceTempView(self: Self, name: str = "") -> "KastDataFrame":
         ...
 
     def map(self: Self, fn: Any, schema: str | dict[str, Any]) -> "KastDataFrame":
@@ -134,15 +111,14 @@
     def emptyKastDataFrame(self: Self) -> KastDataFrame:
         ...
 
 
 @dataclass(frozen=True, slots=True, kw_only=True, eq=True)
 class KastFunction(Protocol):
     id: str
-    backend: KastDataFrameBackend = KastDataFrameBackend.NOTSET
     outs: KastOuts = field(default_factory=make_outs)
 
     def compute(
         self: Self,
         tool: KastTool,
         tables: list[KastDataFrame],
     ) -> KastDataFrame:
@@ -256,27 +232,22 @@
         return result
 
     return cast(Fn, duration)
 
 
 class KastManifest:
     __nodes: KastNodeList
-    __backend: KastDataFrameBackend
 
-    def __init__(
-        self: Self, nodes: KastNodeList, backend: KastDataFrameBackend
-    ) -> None:
+    def __init__(self: Self, nodes: KastNodeList) -> None:
         self.__nodes = nodes
-        self.__backend = backend
 
     def deser(self: Self, *add_modules: str) -> KastNodeList:
         nodesRaw: list[KastNode] = []
         for node in self.__nodes:
             node_dict: dict[str, Any] = cast(dict[str, Any], node)
-            node_dict["backend"] = self.__backend
             nodesRaw.append(
                 KastNode.from_dict(
                     modules={__name__, *add_modules},
                     **node_dict,
                 )
             )
         return cast(KastNodeList, nodesRaw)
```

### Comparing `kast_flow_api_python-1.0.3/pyproject.toml` & `kast_flow_api_python-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kast-flow-api-python"
-version = "1.0.3"
+version = "1.0.4"
 description = "kast python api unified processing engine"
 authors = ["kast"]
 packages = [
     { include = "kast_flow_api" }
 ]
 
 [tool.poetry.dependencies]
```

