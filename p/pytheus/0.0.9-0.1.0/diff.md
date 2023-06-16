# Comparing `tmp/pytheus-0.0.9.tar.gz` & `tmp/pytheus-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytheus-0.0.9.tar", last modified: Sat Apr 15 09:54:15 2023, max compression
+gzip compressed data, was "pytheus-0.1.0.tar", last modified: Fri Jun 16 22:09:15 2023, max compression
```

## Comparing `pytheus-0.0.9.tar` & `pytheus-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-15 09:54:15.198875 pytheus-0.0.9/
--rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.0.9/LICENSE
--rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-15 09:54:15.198684 pytheus-0.0.9/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)    12050 2023-04-12 19:36:26.000000 pytheus-0.0.9/README.md
--rw-r--r--   0 llandy     (501) staff       (20)     1089 2023-04-15 09:53:06.000000 pytheus-0.0.9/pyproject.toml
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-15 09:54:15.184860 pytheus-0.0.9/pytheus/
--rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.0.9/pytheus/__init__.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-15 09:54:15.186201 pytheus-0.0.9/pytheus/backends/
--rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.0.9/pytheus/backends/__init__.py
--rw-r--r--   0 llandy     (501) staff       (20)     4148 2023-04-04 00:38:41.000000 pytheus-0.0.9/pytheus/backends/base.py
--rw-r--r--   0 llandy     (501) staff       (20)     3142 2023-04-15 09:52:20.000000 pytheus-0.0.9/pytheus/backends/redis.py
--rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.0.9/pytheus/exceptions.py
--rw-r--r--   0 llandy     (501) staff       (20)     2058 2023-04-12 22:30:13.000000 pytheus-0.0.9/pytheus/exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    18841 2023-04-13 22:40:07.000000 pytheus-0.0.9/pytheus/metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     3051 2023-04-03 00:08:23.000000 pytheus-0.0.9/pytheus/registry.py
--rw-r--r--   0 llandy     (501) staff       (20)      568 2023-04-13 22:40:07.000000 pytheus-0.0.9/pytheus/utils.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-15 09:54:15.185633 pytheus-0.0.9/pytheus.egg-info/
--rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-15 09:54:15.000000 pytheus-0.0.9/pytheus.egg-info/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)      485 2023-04-15 09:54:15.000000 pytheus-0.0.9/pytheus.egg-info/SOURCES.txt
--rw-r--r--   0 llandy     (501) staff       (20)        1 2023-04-15 09:54:15.000000 pytheus-0.0.9/pytheus.egg-info/dependency_links.txt
--rw-r--r--   0 llandy     (501) staff       (20)      176 2023-04-15 09:54:15.000000 pytheus-0.0.9/pytheus.egg-info/requires.txt
--rw-r--r--   0 llandy     (501) staff       (20)        8 2023-04-15 09:54:15.000000 pytheus-0.0.9/pytheus.egg-info/top_level.txt
--rw-r--r--   0 llandy     (501) staff       (20)       38 2023-04-15 09:54:15.198913 pytheus-0.0.9/setup.cfg
--rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.0.9/setup.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-15 09:54:15.198292 pytheus-0.0.9/tests/
--rw-r--r--   0 llandy     (501) staff       (20)     5857 2023-04-13 22:30:11.000000 pytheus-0.0.9/tests/test_exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    23523 2023-04-13 22:40:07.000000 pytheus-0.0.9/tests/test_metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.0.9/tests/test_registry.py
--rw-r--r--   0 llandy     (501) staff       (20)      349 2023-04-13 22:40:07.000000 pytheus-0.0.9/tests/test_utils.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-06-16 22:09:15.494112 pytheus-0.1.0/
+-rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.1.0/LICENSE
+-rw-r--r--   0 llandy     (501) staff       (20)    13832 2023-06-16 22:09:15.493921 pytheus-0.1.0/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)    13187 2023-06-11 21:57:42.000000 pytheus-0.1.0/README.md
+-rw-r--r--   0 llandy     (501) staff       (20)     1325 2023-06-16 22:08:06.000000 pytheus-0.1.0/pyproject.toml
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-06-16 22:09:15.490759 pytheus-0.1.0/pytheus/
+-rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.1.0/pytheus/__init__.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-06-16 22:09:15.492094 pytheus-0.1.0/pytheus/backends/
+-rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.1.0/pytheus/backends/__init__.py
+-rw-r--r--   0 llandy     (501) staff       (20)     4254 2023-06-10 22:34:13.000000 pytheus-0.1.0/pytheus/backends/base.py
+-rw-r--r--   0 llandy     (501) staff       (20)     6255 2023-06-03 01:35:21.000000 pytheus-0.1.0/pytheus/backends/redis.py
+-rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.1.0/pytheus/exceptions.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3282 2023-06-03 01:35:21.000000 pytheus-0.1.0/pytheus/exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    22725 2023-06-16 22:06:24.000000 pytheus-0.1.0/pytheus/metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     4391 2023-06-16 22:06:24.000000 pytheus-0.1.0/pytheus/middleware.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3076 2023-06-03 01:35:21.000000 pytheus-0.1.0/pytheus/registry.py
+-rw-r--r--   0 llandy     (501) staff       (20)      568 2023-05-14 22:26:37.000000 pytheus-0.1.0/pytheus/utils.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-06-16 22:09:15.491515 pytheus-0.1.0/pytheus.egg-info/
+-rw-r--r--   0 llandy     (501) staff       (20)    13832 2023-06-16 22:09:15.000000 pytheus-0.1.0/pytheus.egg-info/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)      507 2023-06-16 22:09:15.000000 pytheus-0.1.0/pytheus.egg-info/SOURCES.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        1 2023-06-16 22:09:15.000000 pytheus-0.1.0/pytheus.egg-info/dependency_links.txt
+-rw-r--r--   0 llandy     (501) staff       (20)      217 2023-06-16 22:09:15.000000 pytheus-0.1.0/pytheus.egg-info/requires.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        8 2023-06-16 22:09:15.000000 pytheus-0.1.0/pytheus.egg-info/top_level.txt
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2023-06-16 22:09:15.494146 pytheus-0.1.0/setup.cfg
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.1.0/setup.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-06-16 22:09:15.493529 pytheus-0.1.0/tests/
+-rw-r--r--   0 llandy     (501) staff       (20)     7264 2023-06-02 00:02:13.000000 pytheus-0.1.0/tests/test_exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    29297 2023-06-11 21:57:42.000000 pytheus-0.1.0/tests/test_metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.1.0/tests/test_registry.py
+-rw-r--r--   0 llandy     (501) staff       (20)      349 2023-04-13 22:40:07.000000 pytheus-0.1.0/tests/test_utils.py
```

### Comparing `pytheus-0.0.9/LICENSE` & `pytheus-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.9/PKG-INFO` & `pytheus-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-Metadata-Version: 2.1
-Name: pytheus
-Version: 0.0.9
-Summary: playing with metrics
-Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
-Project-URL: Homepage, https://github.com/Llandy3d/pytheus
-Project-URL: Documentation, https://pythe.us
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: redis
-Provides-Extra: docs
-License-File: LICENSE
-
 <img src="https://user-images.githubusercontent.com/16627175/185823115-b33905c3-f389-40e1-b830-2197889a936a.png" height="400">
 
 # pytheus
 
 *playing with metrics*
 
+
+[![ci](https://github.com/Llandy3d/pytheus/workflows/ci/badge.svg?event=push)](https://github.com/Llandy3d/pytheus/actions?query=event%3Apush+branch%3Amain+workflow%3Aci)
+[![pypi](https://img.shields.io/pypi/v/pytheus.svg)](https://pypi.python.org/pypi/pytheus)
+[![versions](https://img.shields.io/pypi/pyversions/pytheus.svg)](https://github.com/Llandy3d/pytheus)
+[![license](https://img.shields.io/github/license/Llandy3d/pytheus.svg)](https://github.com/Llandy3d/pytheus/blob/main/LICENSE)
+[![downloads](https://pepy.tech/badge/pytheus/month)](https://pepy.tech/project/pytheus)
+
 ---
 
 **Documentation**: https://pythe.us
 
 ---
 
 pytheus is a modern python library for collecting [prometheus](https://prometheus.io/docs/introduction/overview/) metrics built with multiprocessing in mind.
@@ -47,15 +39,15 @@
 - What you see is what you get.
 - No differences between `singleprocess` & `multiprocess`, the only change is loading a different backend and everything will work out of the box.
 - High flexibility with an high degree of `labels` control and customization.
 
 ---
 ## Requirements
 
-- Python 3.10+
+- Python 3.8+
 - redis >= 4.0.0 (**optional**: for multiprocessing)
 
 ---
 
 **Architecture**
 
 A small piece of the architecture is described in the [ARCHITECTURE.md file](ARCHITECTURE.md)
@@ -286,14 +278,36 @@
 
 # tracking time can also be done as a decorator
 @histogram
 def do_something():
     ...
 ```
 
+## Summary
+
+A Summary is a metric that captures individual observations and tracks the total size & number of events observed. It can be useful to track latencies for example.
+
+```python
+from pytheus.metrics import Summary
+
+summary = Summary(name="my_summary", description="My description")
+
+# observe a value
+summary.observe(0.4)
+
+# you can also time a piece of code, will set the duration in seconds to value when exited
+with summary.time():
+    do_something()
+
+# tracking time can also be done as a decorator
+@summary
+def do_something():
+    ...
+```
+
 ## Custom Collectors
 
 It is possible to use a custom collector in cases you can't directly instrument the code.
 You will need to inherit from `CustomCollector` and define the `collect` method.
 Also be sure to disable the automatic registering of a newly created metric into the default registry.
 
 ```python
```

### Comparing `pytheus-0.0.9/README.md` & `pytheus-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,39 @@
+Metadata-Version: 2.1
+Name: pytheus
+Version: 0.1.0
+Summary: playing with metrics
+Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
+Project-URL: Homepage, https://github.com/Llandy3d/pytheus
+Project-URL: Documentation, https://pythe.us
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: redis
+Provides-Extra: docs
+License-File: LICENSE
+
 <img src="https://user-images.githubusercontent.com/16627175/185823115-b33905c3-f389-40e1-b830-2197889a936a.png" height="400">
 
 # pytheus
 
 *playing with metrics*
 
+
+[![ci](https://github.com/Llandy3d/pytheus/workflows/ci/badge.svg?event=push)](https://github.com/Llandy3d/pytheus/actions?query=event%3Apush+branch%3Amain+workflow%3Aci)
+[![pypi](https://img.shields.io/pypi/v/pytheus.svg)](https://pypi.python.org/pypi/pytheus)
+[![versions](https://img.shields.io/pypi/pyversions/pytheus.svg)](https://github.com/Llandy3d/pytheus)
+[![license](https://img.shields.io/github/license/Llandy3d/pytheus.svg)](https://github.com/Llandy3d/pytheus/blob/main/LICENSE)
+[![downloads](https://pepy.tech/badge/pytheus/month)](https://pepy.tech/project/pytheus)
+
 ---
 
 **Documentation**: https://pythe.us
 
 ---
 
 pytheus is a modern python library for collecting [prometheus](https://prometheus.io/docs/introduction/overview/) metrics built with multiprocessing in mind.
@@ -32,15 +58,15 @@
 - What you see is what you get.
 - No differences between `singleprocess` & `multiprocess`, the only change is loading a different backend and everything will work out of the box.
 - High flexibility with an high degree of `labels` control and customization.
 
 ---
 ## Requirements
 
-- Python 3.10+
+- Python 3.8+
 - redis >= 4.0.0 (**optional**: for multiprocessing)
 
 ---
 
 **Architecture**
 
 A small piece of the architecture is described in the [ARCHITECTURE.md file](ARCHITECTURE.md)
@@ -271,14 +297,36 @@
 
 # tracking time can also be done as a decorator
 @histogram
 def do_something():
     ...
 ```
 
+## Summary
+
+A Summary is a metric that captures individual observations and tracks the total size & number of events observed. It can be useful to track latencies for example.
+
+```python
+from pytheus.metrics import Summary
+
+summary = Summary(name="my_summary", description="My description")
+
+# observe a value
+summary.observe(0.4)
+
+# you can also time a piece of code, will set the duration in seconds to value when exited
+with summary.time():
+    do_something()
+
+# tracking time can also be done as a decorator
+@summary
+def do_something():
+    ...
+```
+
 ## Custom Collectors
 
 It is possible to use a custom collector in cases you can't directly instrument the code.
 You will need to inherit from `CustomCollector` and define the `collect` method.
 Also be sure to disable the automatic registering of a newly created metric into the default registry.
 
 ```python
```

### Comparing `pytheus-0.0.9/pyproject.toml` & `pytheus-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 [project]
 name = "pytheus"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Llandy Riveron Del Risco", email="llandy3d@gmail.com" },
 ]
 description = "playing with metrics"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Llandy3d/pytheus"
 Documentation = "https://pythe.us"
 
 [project.optional-dependencies]
 test = [
   "pytest >= 7.0.0",
+  "pytest-asyncio >= 0.21.0",
   "mypy == 1.1.1",
   "ruff == 0.0.260",
   "black == 23.3.0",
   "isort == 5.12.0",
   "tox == 4.4.11",
+  "fakeredis == 2.10.3",
 
   # mypy types
   "types-redis == 4.5.4.0",
 ]
 
 redis = [
   "redis >= 4.0.0",
```

### Comparing `pytheus-0.0.9/pytheus/backends/base.py` & `pytheus-0.1.0/pytheus/backends/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import importlib
 import json
 import os
 from threading import Lock
-from typing import TYPE_CHECKING, Any, Protocol, runtime_checkable
+from typing import TYPE_CHECKING, Any, Dict, Optional, Protocol, Type, runtime_checkable
 
 from pytheus.exceptions import InvalidBackendClassException, InvalidBackendConfigException
 
 if TYPE_CHECKING:
     from pytheus.metrics import _Metric
 
 
-BackendConfig = dict[str, Any]
+BackendConfig = Dict[str, Any]
 
 
 @runtime_checkable
 class Backend(Protocol):
     """
     Describes how to implement a Backend that can be used as a metric value backend.
     It must take the values indicated in the `__init__` method.
     """
 
     def __init__(
         # optional config ?
         self,
         config: BackendConfig,
         metric: "_Metric",
-        histogram_bucket: str | None = None,
+        histogram_bucket: Optional[str] = None,
     ) -> None:
         ...
 
     def inc(self, value: float) -> None:
         ...
 
     def dec(self, value: float) -> None:
@@ -38,40 +38,40 @@
     def set(self, value: float) -> None:
         ...
 
     def get(self) -> float:
         ...
 
 
-def _import_backend_class(full_import_path: str) -> type[Backend]:
+def _import_backend_class(full_import_path: str) -> Type[Backend]:
     try:
         module_path, class_name = full_import_path.rsplit(".", 1)
     except ValueError:  # Empty string or not full path to the class
         raise InvalidBackendClassException(
             "Backend class could not be imported. Full import path needs to be provided, e.g. "
             "my_package.my_module.MyClass"
         )
     try:
         module = importlib.import_module(module_path)
     except ImportError as e:
         raise InvalidBackendClassException(f"Module '{module_path}' could not be imported: {e}")
     try:
-        cls: type[Backend] = getattr(module, class_name)
+        cls: Type[Backend] = getattr(module, class_name)
         if not issubclass(cls, Backend):
             raise InvalidBackendClassException(f"Class '{class_name}' is not a Backend subclass")
         return cls
     except AttributeError:
         raise InvalidBackendClassException(
             f"Class '{class_name}' could not be found in module '{module_path}'"
         )
 
 
 def load_backend(
-    backend_class: type[Backend] | None = None,
-    backend_config: BackendConfig | None = None,
+    backend_class: Optional[Type[Backend]] = None,
+    backend_config: Optional[BackendConfig] = None,
 ) -> None:
     # Load default backend class
     global BACKEND_CLASS
     backend_class_env_var: str = "PYTHEUS_BACKEND_CLASS"
     if backend_class is not None:  # Explicit
         BACKEND_CLASS = backend_class
     elif backend_class_env_var in os.environ:  # Environment
@@ -94,27 +94,31 @@
         BACKEND_CONFIG = {}  # Default
 
     # initialization hook
     if hasattr(BACKEND_CLASS, "_initialize"):
         BACKEND_CLASS._initialize(BACKEND_CONFIG)
 
 
-def get_backend(metric: "_Metric", histogram_bucket: str | None = None) -> Backend:
+def get_backend(metric: "_Metric", histogram_bucket: Optional[str] = None) -> Backend:
     # Probably ok not to cache this and allow each metric to keep its own
     return BACKEND_CLASS(BACKEND_CONFIG, metric, histogram_bucket=histogram_bucket)
 
 
+def get_backend_class() -> Type[Backend]:
+    return BACKEND_CLASS
+
+
 class SingleProcessBackend:
     """Provides a single-process backend that uses a thread-safe, in-memory approach."""
 
     def __init__(
         self,
         config: BackendConfig,
         metric: "_Metric",
-        histogram_bucket: str | None = None,
+        histogram_bucket: Optional[str] = None,
     ) -> None:
         self._value = 0.0
         self._lock = Lock()
 
     def inc(self, value: float) -> None:
         with self._lock:
             self._value += value
@@ -128,9 +132,9 @@
             self._value = value
 
     def get(self) -> float:
         with self._lock:
             return self._value
 
 
-BACKEND_CLASS: type[Backend]
+BACKEND_CLASS: Type[Backend]
 BACKEND_CONFIG: BackendConfig
```

### Comparing `pytheus-0.0.9/pytheus/metrics.py` & `pytheus-0.1.0/pytheus/metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
+import asyncio
 import functools
 import itertools
 import re
 import time
-from collections.abc import Generator
 from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import Callable, Iterable, Sequence
+from typing import Callable, Dict, Generator, Iterable, Optional, Sequence, Tuple, Type, Union
 
 from pytheus.backends import get_backend
 from pytheus.exceptions import (
     BucketException,
     LabelValidationException,
     UnobservableMetricException,
 )
 from pytheus.registry import REGISTRY, Collector, Registry
 from pytheus.utils import InfFloat, MetricType
 
-Labels = dict[str, str]
+Labels = Dict[str, str]
 
 
 metric_name_re = re.compile(r"[a-zA-Z_:][a-zA-Z0-9_:]*")
 label_name_re = re.compile(r"[a-zA-Z_][a-zA-Z0-9_]*")
 
 
 @dataclass
 class Sample:
     suffix: str
-    labels: dict[str, str] | None
+    labels: Optional[Dict[str, str]]
     value: float
 
 
 class CustomCollector(Collector):
     """
     Inheriting from this protocol is the current way to create a custom collector.
     The property `name` will return the lowercased class name so that it can be
@@ -59,52 +59,53 @@
     """
 
     def __init__(
         self,
         name: str,
         description: str,
         metric: "_Metric",
-        required_labels: Sequence[str] | None = None,
-        default_labels: Labels | None = None,
-        registry: Registry | None = REGISTRY,
+        required_labels: Optional[Sequence[str]] = None,
+        default_labels: Optional[Labels] = None,
+        registry: Optional[Registry] = REGISTRY,
     ) -> None:
         if metric_name_re.fullmatch(name) is None:
             raise ValueError(f"Invalid metric name: {name}")
 
         if required_labels:
-            is_histogram = isinstance(metric, Histogram)
-            self._validate_required_labels(required_labels, is_histogram)
+            self._validate_required_labels(required_labels, metric.type_)
 
         self._required_labels = set(required_labels) if required_labels else None
 
         if default_labels:
             self._validate_labels(default_labels)
 
         self.name = name
         self.description = description
         self.type_ = metric.type_
         self._default_labels = default_labels
         self._default_labels_count = len(default_labels) if default_labels else 0
         self._metric = metric
-        self._labeled_metrics: dict[tuple[str, ...], _Metric] = {}
+        self._labeled_metrics: Dict[Tuple[str, ...], _Metric] = {}
         self._registry = registry
 
         if registry:
             registry.register(self)
 
-    def _validate_required_labels(self, labels: Sequence[str], is_histogram: bool = False) -> None:
+    def _validate_required_labels(self, labels: Sequence[str], metric_type: MetricType) -> None:
         """
         Validates label names according to the regex.
         Labels starting with `__` are reserved for internal use by Prometheus.
         """
         for label in labels:
             if label.startswith("__") or label_name_re.fullmatch(label) is None:
                 raise LabelValidationException(f"Invalid label name: {label}")
-            if is_histogram and label == "le":
+            if metric_type == MetricType.HISTOGRAM and label == "le":
                 raise LabelValidationException(f"Invalid label name for Histogram: {label}")
+            elif metric_type == MetricType.SUMMARY and label == "quantile":
+                raise LabelValidationException(f"Invalid label name for Summary: {label}")
 
     def _validate_labels(self, labels: Labels) -> None:
         """
         Validates labels.
         If no `required_labels` is set raises an error.
         `labels` will be also validated to be a subset of `required_labels`.
         """
@@ -123,32 +124,33 @@
         """
         labeled_metrics: Iterable[Sample]
         if self._required_labels:
             labeled_metrics = (
                 sample for metric in self._labeled_metrics.values() for sample in metric.collect()
             )
             if self._default_labels and self._metric._can_observe:
-                labeled_metrics = itertools.chain(labeled_metrics, self._metric.collect())
+                # note: this chaining order is important for correct matching with redis pipeline
+                labeled_metrics = itertools.chain(self._metric.collect(), labeled_metrics)
             return labeled_metrics
         else:
             return self._metric.collect()
 
 
 class _Metric:
     type_: MetricType = MetricType.UNTYPED
 
     def __init__(
         self,
         name: str,
         description: str,
-        required_labels: Sequence[str] | None = None,
-        labels: Labels | None = None,
-        default_labels: Labels | None = None,
-        registry: Registry | None = REGISTRY,
-        collector: _MetricCollector | None = None,
+        required_labels: Optional[Sequence[str]] = None,
+        labels: Optional[Labels] = None,
+        default_labels: Optional[Labels] = None,
+        registry: Optional[Registry] = REGISTRY,
+        collector: Optional[_MetricCollector] = None,
     ) -> None:
         self.name = name
         self.description = description
         self._labels = labels
         self._registry = registry
         self._metric_value_backend = None
         self._collector = (
@@ -162,15 +164,15 @@
 
         if not collector and labels:
             raise LabelValidationException(
                 "Setting labels when creating a metric is not allowed. "
                 "You might be looking for default_labels."
             )
 
-        if self._can_observe and not isinstance(self, Histogram):
+        if self._can_observe and self.type_ not in [MetricType.HISTOGRAM, MetricType.SUMMARY]:
             self._metric_value_backend = get_backend(self)
 
     def _check_can_observe(self) -> bool:
         if not self._collector._required_labels:
             return True
 
         required_labels_count = len(self._collector._required_labels)
@@ -203,15 +205,14 @@
     def labels(self, labels_: Labels) -> "_Metric":
         """
         If no labels is passed to the call returns itself.
         If there are already present labels, they will be updated with the passed labels_ and if
         it's not observable will just return the new child instance. Otherwise it will also add
         the instance to the labeled_metrics on the collector.
         """
-        # if not labels_ or self._collector._required_labels is None:
         if not labels_:
             return self
 
         self._collector._validate_labels(labels_)
 
         if self._labels:
             new_labels = self._labels.copy()
@@ -289,15 +290,15 @@
             raise ValueError(f"Counter increase value ({value}) must be >= 0")
 
         assert self._metric_value_backend is not None
         self._metric_value_backend.inc(value)
 
     @contextmanager
     def count_exceptions(
-        self, exceptions: type[Exception] | tuple[Exception] | None = None
+        self, exceptions: Union[Type[Exception], Tuple[Exception], None] = None
     ) -> Generator[None, None, None]:
         """
         Will count and reraise raised exceptions.
         It is possibly to specify which exceptions to track.
         """
         self._raise_if_cannot_observe()
         if exceptions is None:
@@ -307,27 +308,36 @@
             yield
         except exceptions:  # type: ignore
             self.inc()
             raise
 
     def __call__(
         self,
-        func: Callable | None = None,
-        exceptions: type[Exception] | tuple[Exception] | None = None,
+        func: Optional[Callable] = None,
+        exceptions: Union[Type[Exception], Tuple[Exception], None] = None,
     ) -> Callable:
         """
         When called acts as a decorator counting exceptions raised.
         """
         if func is None:
             return functools.partial(self.__call__, exceptions=exceptions)
 
-        @functools.wraps(func)
-        def wrapper(*args, **kwargs):  # type: ignore
-            with self.count_exceptions(exceptions):
-                return func(*args, **kwargs)
+        if asyncio.iscoroutinefunction(func):
+
+            @functools.wraps(func)
+            async def wrapper(*args, **kwargs):  # type: ignore
+                with self.count_exceptions(exceptions):
+                    return await func(*args, **kwargs)
+
+        else:
+
+            @functools.wraps(func)
+            def wrapper(*args, **kwargs):  # type: ignore
+                with self.count_exceptions(exceptions):
+                    return func(*args, **kwargs)
 
         return wrapper
 
     def collect(self) -> Iterable[Sample]:
         self._raise_if_cannot_observe()
         assert self._metric_value_backend is not None
         sample = Sample("", self._labels, self._metric_value_backend.get())
@@ -375,33 +385,46 @@
         Will increase the gauge value when entered and decrease it when exited.
         """
         self._raise_if_cannot_observe()
         self.inc()
         yield
         self.dec()
 
-    def __call__(self, func: Callable | None = None, track_inprogress: bool = False) -> Callable:
+    def __call__(self, func: Optional[Callable] = None, track_inprogress: bool = False) -> Callable:
         """
         When called acts as a decorator tracking the time taken by
         the wrapped function.
 
         If passing the parameter `track_inprogress` as `True` it will instead increase while the
         function is running and will decrease when it's finished.
         """
         if func is None:
             return functools.partial(self.__call__, track_inprogress=track_inprogress)
 
-        @functools.wraps(func)
-        def wrapper(*args, **kwargs):  # type: ignore
-            if track_inprogress:
-                with self.track_inprogress():
-                    return func(*args, **kwargs)
-            else:
-                with self.time():
-                    return func(*args, **kwargs)
+        if asyncio.iscoroutinefunction(func):
+
+            @functools.wraps(func)
+            async def wrapper(*args, **kwargs):  # type: ignore
+                if track_inprogress:
+                    with self.track_inprogress():
+                        return await func(*args, **kwargs)
+                else:
+                    with self.time():
+                        return await func(*args, **kwargs)
+
+        else:
+
+            @functools.wraps(func)
+            def wrapper(*args, **kwargs):  # type: ignore
+                if track_inprogress:
+                    with self.track_inprogress():
+                        return func(*args, **kwargs)
+                else:
+                    with self.time():
+                        return func(*args, **kwargs)
 
         return wrapper
 
     @contextmanager
     def time(self) -> Generator[None, None, None]:
         """
         Times the duration inside of it and sets the value.
@@ -425,19 +448,19 @@
     # Values taken from the golang/rust client.
     DEFAULT_BUCKETS = (0.005, 0.01, 0.025, 0.05, 0.1, 0.25, 0.5, 1, 2.5, 5, 10)
 
     def __init__(
         self,
         name: str,
         description: str,
-        required_labels: Sequence[str] | None = None,
-        labels: Labels | None = None,
-        default_labels: Labels | None = None,
-        registry: Registry | None = REGISTRY,
-        collector: _MetricCollector | None = None,
+        required_labels: Optional[Sequence[str]] = None,
+        labels: Optional[Labels] = None,
+        default_labels: Optional[Labels] = None,
+        registry: Optional[Registry] = REGISTRY,
+        collector: Optional[_MetricCollector] = None,
         buckets: Sequence[float] = DEFAULT_BUCKETS,
     ) -> None:
         super().__init__(
             name,
             description,
             required_labels,
             labels,
@@ -514,19 +537,27 @@
         self.observe(time.perf_counter() - start)
 
     def __call__(self, func: Callable) -> Callable:
         """
         When called acts as a decorator tracking the time taken by
         the wrapped function.
         """
+        if asyncio.iscoroutinefunction(func):
+
+            @functools.wraps(func)
+            async def wrapper(*args, **kwargs):  # type: ignore
+                with self.time():
+                    return await func(*args, **kwargs)
 
-        @functools.wraps(func)
-        def wrapper(*args, **kwargs):  # type: ignore
-            with self.time():
-                return func(*args, **kwargs)
+        else:
+
+            @functools.wraps(func)
+            def wrapper(*args, **kwargs):  # type: ignore
+                with self.time():
+                    return func(*args, **kwargs)
 
         return wrapper
 
     def collect(self) -> Iterable[Sample]:
         self._raise_if_cannot_observe()
         samples = []
         for i, bound in enumerate(self._upper_bounds):
@@ -538,13 +569,96 @@
         assert self._sum is not None
         assert self._count is not None
         samples.append(Sample("_sum", self._labels, self._sum.get()))
         samples.append(Sample("_count", self._labels, self._count.get()))
 
         return (self._add_default_labels_to_sample(sample) for sample in samples)
 
+
+class Summary(_Metric):
+    type_: MetricType = MetricType.SUMMARY
+
+    def __init__(
+        self,
+        name: str,
+        description: str,
+        required_labels: Optional[Sequence[str]] = None,
+        labels: Optional[Labels] = None,
+        default_labels: Optional[Labels] = None,
+        registry: Optional[Registry] = REGISTRY,
+        collector: Optional[_MetricCollector] = None,
+    ) -> None:
+        super().__init__(
+            name,
+            description,
+            required_labels,
+            labels,
+            default_labels,
+            registry,
+            collector,
+        )
+
+        self._sum = None
+        self._count = None
+        if self._can_observe:
+            # as always `histogram_bucket` might not be the best name for it
+            self._sum = get_backend(self, histogram_bucket="sum")
+            self._count = get_backend(self, histogram_bucket="count")
+
+    def observe(self, value: float) -> None:
+        """
+        Observe the given value.
+        Value can be negative, in that case prometheus might not detect counter resets.
+        """
+        self._raise_if_cannot_observe()
+        assert self._sum is not None
+        assert self._count is not None
+        self._sum.inc(value)
+        self._count.inc(1)
+
+    @contextmanager
+    def time(self) -> Generator[None, None, None]:
+        """
+        Times the duration inside of it and sets the value.
+        """
+        self._raise_if_cannot_observe()
+        start = time.perf_counter()
+        yield
+        self.observe(time.perf_counter() - start)
+
+    def __call__(self, func: Callable) -> Callable:
+        """
+        When called acts as a decorator tracking the time taken by
+        the wrapped function.
+        """
+        if asyncio.iscoroutinefunction(func):
+
+            @functools.wraps(func)
+            async def wrapper(*args, **kwargs):  # type: ignore
+                with self.time():
+                    return await func(*args, **kwargs)
+
+        else:
+
+            @functools.wraps(func)
+            def wrapper(*args, **kwargs):  # type: ignore
+                with self.time():
+                    return func(*args, **kwargs)
+
+        return wrapper
+
+    def collect(self) -> Iterable[Sample]:
+        self._raise_if_cannot_observe()
+        samples = []
+        assert self._sum is not None
+        assert self._count is not None
+        samples.append(Sample("_sum", self._labels, self._sum.get()))
+        samples.append(Sample("_count", self._labels, self._count.get()))
+
+        return (self._add_default_labels_to_sample(sample) for sample in samples)
+
 
 # maybe just go with the typing alias
 @dataclass
 class Label:
     name: str
     value: str
```

### Comparing `pytheus-0.0.9/pytheus/registry.py` & `pytheus-0.1.0/pytheus/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from logging import getLogger
 from threading import Lock
-from typing import Iterable, Protocol
+from typing import Dict, Iterable, Optional, Protocol
 
 from pytheus.utils import MetricType
 
 logger = getLogger(__name__)
 
 
 class Collector(Protocol):
@@ -13,31 +13,31 @@
     type_: MetricType
 
     def collect(self) -> Iterable:
         ...
 
 
 class Registry(Protocol):
-    prefix: str | None
+    prefix: Optional[str]
 
     def register(self, collector: Collector) -> None:
         ...
 
     def unregister(self, collector: Collector) -> None:
         ...
 
     def collect(self) -> Iterable:
         ...
 
 
 class CollectorRegistry:
-    def __init__(self, prefix: str | None = None) -> None:
+    def __init__(self, prefix: Optional[str] = None) -> None:
         self._lock = Lock()
         self.prefix = prefix
-        self._collectors: dict[str, Collector] = {}
+        self._collectors: Dict[str, Collector] = {}
 
     def register(self, collector: Collector) -> None:
         with self._lock:
             if collector.name in self._collectors:
                 logger.warning(
                     f"collector with name '{collector.name}' already registered."
                     " Keeping previous entry"
@@ -69,15 +69,15 @@
             del self._collectors[collector.name]
 
     def collect(self) -> Iterable[Collector]:
         yield from self._collectors.values()
 
 
 class CollectorRegistryProxy:
-    def __init__(self, registry: Registry | None = None) -> None:
+    def __init__(self, registry: Optional[Registry] = None) -> None:
         self._registry = registry or CollectorRegistry()
         self.prefix = self._registry.prefix
 
     def set_registry(self, registry: Registry) -> None:
         self._registry = registry
         self.prefix = self._registry.prefix
```

### Comparing `pytheus-0.0.9/pytheus/utils.py` & `pytheus-0.1.0/pytheus/utils.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.9/pytheus.egg-info/PKG-INFO` & `pytheus-0.1.0/pytheus.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 Metadata-Version: 2.1
 Name: pytheus
-Version: 0.0.9
+Version: 0.1.0
 Summary: playing with metrics
 Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
 Project-URL: Homepage, https://github.com/Llandy3d/pytheus
 Project-URL: Documentation, https://pythe.us
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: redis
 Provides-Extra: docs
 License-File: LICENSE
 
 <img src="https://user-images.githubusercontent.com/16627175/185823115-b33905c3-f389-40e1-b830-2197889a936a.png" height="400">
 
 # pytheus
 
 *playing with metrics*
 
+
+[![ci](https://github.com/Llandy3d/pytheus/workflows/ci/badge.svg?event=push)](https://github.com/Llandy3d/pytheus/actions?query=event%3Apush+branch%3Amain+workflow%3Aci)
+[![pypi](https://img.shields.io/pypi/v/pytheus.svg)](https://pypi.python.org/pypi/pytheus)
+[![versions](https://img.shields.io/pypi/pyversions/pytheus.svg)](https://github.com/Llandy3d/pytheus)
+[![license](https://img.shields.io/github/license/Llandy3d/pytheus.svg)](https://github.com/Llandy3d/pytheus/blob/main/LICENSE)
+[![downloads](https://pepy.tech/badge/pytheus/month)](https://pepy.tech/project/pytheus)
+
 ---
 
 **Documentation**: https://pythe.us
 
 ---
 
 pytheus is a modern python library for collecting [prometheus](https://prometheus.io/docs/introduction/overview/) metrics built with multiprocessing in mind.
@@ -47,15 +58,15 @@
 - What you see is what you get.
 - No differences between `singleprocess` & `multiprocess`, the only change is loading a different backend and everything will work out of the box.
 - High flexibility with an high degree of `labels` control and customization.
 
 ---
 ## Requirements
 
-- Python 3.10+
+- Python 3.8+
 - redis >= 4.0.0 (**optional**: for multiprocessing)
 
 ---
 
 **Architecture**
 
 A small piece of the architecture is described in the [ARCHITECTURE.md file](ARCHITECTURE.md)
@@ -286,14 +297,36 @@
 
 # tracking time can also be done as a decorator
 @histogram
 def do_something():
     ...
 ```
 
+## Summary
+
+A Summary is a metric that captures individual observations and tracks the total size & number of events observed. It can be useful to track latencies for example.
+
+```python
+from pytheus.metrics import Summary
+
+summary = Summary(name="my_summary", description="My description")
+
+# observe a value
+summary.observe(0.4)
+
+# you can also time a piece of code, will set the duration in seconds to value when exited
+with summary.time():
+    do_something()
+
+# tracking time can also be done as a decorator
+@summary
+def do_something():
+    ...
+```
+
 ## Custom Collectors
 
 It is possible to use a custom collector in cases you can't directly instrument the code.
 You will need to inherit from `CustomCollector` and define the `collect` method.
 Also be sure to disable the automatic registering of a newly created metric into the default registry.
 
 ```python
```

### Comparing `pytheus-0.0.9/tests/test_exposition.py` & `pytheus-0.1.0/tests/test_exposition.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pytheus.exposition import generate_metrics
+from unittest import mock
+
+from pytheus.exposition import _escape_help, format_labels, generate_metrics
 from pytheus.metrics import Counter, Histogram
 from pytheus.registry import REGISTRY, CollectorRegistry
 
 
 class TestExposition:
     def setup_counters(self):
         c = Counter("http_req_total", "metric desc", required_labels=["p", "m"])
@@ -81,9 +83,46 @@
         histogram = Histogram(
             "hello", "world", required_labels=["bob"], default_labels={"bob": "default"}
         )
         histogram = histogram.labels({"bob": "a"})
         histogram.observe(0.4)
         metrics_text = generate_metrics()
         assert metrics_text == (
-            '# HELP hello world\n# TYPE hello histogram\nhello_bucket{bob="a",le="0.005"} 0.0\nhello_bucket{bob="a",le="0.01"} 0.0\nhello_bucket{bob="a",le="0.025"} 0.0\nhello_bucket{bob="a",le="0.05"} 0.0\nhello_bucket{bob="a",le="0.1"} 0.0\nhello_bucket{bob="a",le="0.25"} 0.0\nhello_bucket{bob="a",le="0.5"} 1.0\nhello_bucket{bob="a",le="1"} 1.0\nhello_bucket{bob="a",le="2.5"} 1.0\nhello_bucket{bob="a",le="5"} 1.0\nhello_bucket{bob="a",le="10"} 1.0\nhello_bucket{bob="a",le="+Inf"} 1.0\nhello_sum{bob="a"} 0.4\nhello_count{bob="a"} 1.0\nhello_bucket{bob="default",le="0.005"} 0.0\nhello_bucket{bob="default",le="0.01"} 0.0\nhello_bucket{bob="default",le="0.025"} 0.0\nhello_bucket{bob="default",le="0.05"} 0.0\nhello_bucket{bob="default",le="0.1"} 0.0\nhello_bucket{bob="default",le="0.25"} 0.0\nhello_bucket{bob="default",le="0.5"} 0.0\nhello_bucket{bob="default",le="1"} 0.0\nhello_bucket{bob="default",le="2.5"} 0.0\nhello_bucket{bob="default",le="5"} 0.0\nhello_bucket{bob="default",le="10"} 0.0\nhello_bucket{bob="default",le="+Inf"} 0.0\nhello_sum{bob="default"} 0.0\nhello_count{bob="default"} 0.0\n'
+            '# HELP hello world\n# TYPE hello histogram\nhello_bucket{bob="default",le="0.005"} 0.0\nhello_bucket{bob="default",le="0.01"} 0.0\nhello_bucket{bob="default",le="0.025"} 0.0\nhello_bucket{bob="default",le="0.05"} 0.0\nhello_bucket{bob="default",le="0.1"} 0.0\nhello_bucket{bob="default",le="0.25"} 0.0\nhello_bucket{bob="default",le="0.5"} 0.0\nhello_bucket{bob="default",le="1"} 0.0\nhello_bucket{bob="default",le="2.5"} 0.0\nhello_bucket{bob="default",le="5"} 0.0\nhello_bucket{bob="default",le="10"} 0.0\nhello_bucket{bob="default",le="+Inf"} 0.0\nhello_sum{bob="default"} 0.0\nhello_count{bob="default"} 0.0\nhello_bucket{bob="a",le="0.005"} 0.0\nhello_bucket{bob="a",le="0.01"} 0.0\nhello_bucket{bob="a",le="0.025"} 0.0\nhello_bucket{bob="a",le="0.05"} 0.0\nhello_bucket{bob="a",le="0.1"} 0.0\nhello_bucket{bob="a",le="0.25"} 0.0\nhello_bucket{bob="a",le="0.5"} 1.0\nhello_bucket{bob="a",le="1"} 1.0\nhello_bucket{bob="a",le="2.5"} 1.0\nhello_bucket{bob="a",le="5"} 1.0\nhello_bucket{bob="a",le="10"} 1.0\nhello_bucket{bob="a",le="+Inf"} 1.0\nhello_sum{bob="a"} 0.4\nhello_count{bob="a"} 1.0\n'
+        )
+
+    def test_generate_metrics_respects_escaping(self):
+        registry = CollectorRegistry()
+        counter = Counter(
+            "http_req_total", 'slash\\quote"newline\n', required_labels=["bob"], registry=registry
+        )
+        counter.labels({"bob": 'slash\\quote"newline\n'})
+        metrics_text = generate_metrics(registry)
+        assert metrics_text == (
+            '# HELP http_req_total slash\\\\quote"newline\\n\n'
+            "# TYPE http_req_total counter\n"
+            'http_req_total{bob="slash\\\\quote\\"newline\\n"} 0.0\n'
+            ""
         )
+
+    @mock.patch("pytheus.exposition.get_backend_class")
+    def test_generate_metrics_calls_generate_samples(self, get_backend_mock):
+        generate_metrics()
+        assert get_backend_mock()._generate_samples.called
+
+    def test_format_labels_escapes_characters(self):
+        # \ -> \\
+        # " -> \"
+        # \n -> \n (escaped)
+        labels = {"bob": 'slash\\ quote" newline\n'}
+        expected = '{bob="slash\\\\ quote\\" newline\\n"}'
+        formatted_string = format_labels(labels)
+
+        assert formatted_string == expected
+
+    def test_escape_help(self):
+        # \ -> \\
+        # \n -> \n (escaped)
+        help_text = 'slash\\ quote" newline\n'
+        expected = 'slash\\\\ quote" newline\\n'
+
+        assert _escape_help(help_text) == expected
```

### Comparing `pytheus-0.0.9/tests/test_metrics.py` & `pytheus-0.1.0/tests/test_metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,23 @@
 import pytest
 
 from pytheus.exceptions import (
     BucketException,
     LabelValidationException,
     UnobservableMetricException,
 )
-from pytheus.metrics import Counter, CustomCollector, Gauge, Histogram, _Metric, _MetricCollector
+from pytheus.metrics import (
+    Counter,
+    CustomCollector,
+    Gauge,
+    Histogram,
+    Summary,
+    _Metric,
+    _MetricCollector,
+)
 from pytheus.registry import REGISTRY, CollectorRegistry
 from pytheus.utils import InfFloat, MetricType
 
 
 @pytest.fixture
 def set_empty_registry():
     """
@@ -50,28 +58,28 @@
     def test_name_with_incorrect_values(self, name):
         with pytest.raises(ValueError):
             _MetricCollector(name, "desc", _Metric)
 
     def test_validate_required_labels_with_correct_values(self):
         labels = ["action", "method", "_type"]
         collector = _MetricCollector("name", "desc", _Metric)
-        collector._validate_required_labels(labels)
+        collector._validate_required_labels(labels, MetricType.COUNTER)
 
     @pytest.mark.parametrize(
         "label",
         [
             "__private",
             "microµ",
             "@type",
         ],
     )
     def test_validate_required_labels_with_incorrect_values(self, label):
         collector = _MetricCollector("name", "desc", _Metric)
         with pytest.raises(LabelValidationException):
-            collector._validate_required_labels([label])
+            collector._validate_required_labels([label], MetricType.COUNTER)
 
     def test_collect_without_labels(self):
         counter = Counter("name", "desc")
         samples = counter._collector.collect()
         assert len(list(samples)) == 1
 
     def test_collect_with_labels(self):
@@ -333,14 +341,25 @@
             raise ValueError
 
         with pytest.raises(ValueError):
             test()
 
         assert counter._metric_value_backend.get() == 1
 
+    @pytest.mark.asyncio
+    async def test_count_exception_with_decorator_async(self, counter):
+        @counter
+        async def test():
+            raise ValueError
+
+        with pytest.raises(ValueError):
+            await test()
+
+        assert counter._metric_value_backend.get() == 1
+
     def test_count_exception_with_decorator_multiple(self, counter):
         @counter
         def test():
             raise ValueError
 
         @counter
         def test_2():
@@ -349,34 +368,73 @@
         with pytest.raises(ValueError):
             test()
         with pytest.raises(ValueError):
             test_2()
 
         assert counter._metric_value_backend.get() == 2
 
+    @pytest.mark.asyncio
+    async def test_count_exception_with_decorator_multiple_async(self, counter):
+        @counter
+        async def test():
+            raise ValueError
+
+        @counter
+        async def test_2():
+            raise ValueError
+
+        with pytest.raises(ValueError):
+            await test()
+        with pytest.raises(ValueError):
+            await test_2()
+
+        assert counter._metric_value_backend.get() == 2
+
     def test_count_exception_with_specified_as_decorator(self, counter):
         @counter(exceptions=(IndexError, ValueError))
         def test():
             raise ValueError
 
         with pytest.raises(ValueError):
             test()
 
         assert counter._metric_value_backend.get() == 1
 
+    @pytest.mark.asyncio
+    async def test_count_exception_with_specified_as_decorator_async(self, counter):
+        @counter(exceptions=(IndexError, ValueError))
+        async def test():
+            raise ValueError
+
+        with pytest.raises(ValueError):
+            await test()
+
+        assert counter._metric_value_backend.get() == 1
+
     def test_count_exception_with_specified_is_ignored_as_decorator(self, counter):
         @counter(exceptions=IndexError)
         def test():
             raise ValueError
 
         with pytest.raises(ValueError):
             test()
 
         assert counter._metric_value_backend.get() == 0
 
+    @pytest.mark.asyncio
+    async def test_count_exception_with_specified_is_ignored_as_decorator_async(self, counter):
+        @counter(exceptions=IndexError)
+        async def test():
+            raise ValueError
+
+        with pytest.raises(ValueError):
+            await test()
+
+        assert counter._metric_value_backend.get() == 0
+
 
 class TestGauge:
     @pytest.fixture
     def gauge(self):
         return Gauge("name", "desc")
 
     def test_metric_type(self, gauge):
@@ -445,34 +503,65 @@
         @gauge
         def test():
             pass
 
         test()
         assert gauge._metric_value_backend.get() != 0
 
+    @pytest.mark.asyncio
+    async def test_as_decorator_async(self, gauge):
+        @gauge
+        async def test():
+            pass
+
+        await test()
+        assert gauge._metric_value_backend.get() != 0
+
     def test_as_decorator_with_track_inprogress(self, gauge):
         backend_mock = mock.Mock()
         gauge._metric_value_backend = backend_mock
 
         @gauge(track_inprogress=True)
         def test():
             pass
 
         test()
         backend_mock.inc.assert_called()
         backend_mock.dec.assert_called()
 
+    @pytest.mark.asyncio
+    async def test_as_decorator_with_track_inprogress_async(self, gauge):
+        backend_mock = mock.Mock()
+        gauge._metric_value_backend = backend_mock
+
+        @gauge(track_inprogress=True)
+        async def test():
+            pass
+
+        await test()
+        backend_mock.inc.assert_called()
+        backend_mock.dec.assert_called()
+
     def test_as_decorator_with_track_inprogress_as_false(self, gauge):
         @gauge(track_inprogress=False)
         def test():
             pass
 
         test()
         assert gauge._metric_value_backend.get() != 0
 
+    @pytest.mark.asyncio
+    async def test_as_decorator_with_track_inprogress_as_false_async(self, gauge):
+        @gauge(track_inprogress=False)
+        async def test():
+            pass
+
+        await test()
+        assert gauge._metric_value_backend.get() != 0
+
 
 class TestHistogram:
     @pytest.fixture
     def histogram(self):
         return Histogram("name", "desc")
 
     def test_metric_type(self, histogram):
@@ -568,38 +657,166 @@
         assert histogram._buckets[1].get() == 1
         assert histogram._buckets[2].get() == 1
 
     def test_time(self, histogram):
         with histogram.time():
             pass
         assert histogram._count.get() == 1
-        assert histogram._count.get() != 0
+        assert histogram._sum.get() != 0
 
     def test_as_decorator(self, histogram):
         @histogram
         def test():
             pass
 
         test()
         assert histogram._count.get() == 1
-        assert histogram._count.get() != 0
+        assert histogram._sum.get() != 0
 
     def test_as_decorator_multiple(self, histogram):
         @histogram
         def test():
             pass
 
         @histogram
         def test_2():
             pass
 
         test()
         test_2()
         assert histogram._count.get() == 2
-        assert histogram._count.get() != 0
+        assert histogram._sum.get() != 0
+
+    @pytest.mark.asyncio
+    async def test_as_decorator_async(self, histogram):
+        @histogram
+        async def test():
+            pass
+
+        await test()
+        assert histogram._count.get() == 1
+        assert histogram._sum.get() != 0
+
+    @pytest.mark.asyncio
+    async def test_as_decorator_multiple_async(self, histogram):
+        @histogram
+        async def test():
+            pass
+
+        @histogram
+        async def test_2():
+            pass
+
+        await test()
+        await test_2()
+        assert histogram._count.get() == 2
+        assert histogram._sum.get() != 0
+
+
+class TestSummary:
+    @pytest.fixture
+    def summary(self):
+        return Summary("name", "desc")
+
+    def test_metric_type(self, summary):
+        assert summary.type_ == MetricType.SUMMARY
+
+    def test_create_summary_with_default_labels(self):
+        Summary("name", "desc", required_labels=["bob", "cat"])
+
+    def test_summary_fails_with_quantile_label(self):
+        with pytest.raises(LabelValidationException):
+            Summary("name", "desc", required_labels=["bob", "quantile"])
+
+    def test_does_not_have_metric_value_backend(self, summary):
+        assert summary._metric_value_backend is None
+
+    def test_unobservable_does_not_create_buckets(self):
+        summary = Summary("name", "desc", required_labels=["bob"])
+        assert summary._sum is None
+        assert summary._count is None
+
+    def test_observable_creates_buckets(self):
+        summary = Summary("name", "desc", required_labels=["bob"])
+        summary = summary.labels({"bob": "cat"})
+        assert summary._sum is not None
+        assert summary._count is not None
+
+    def test_collect(self):
+        summary = Summary("name", "desc")
+        samples = summary.collect()
+        samples = list(samples)
+
+        assert len(samples) == 2
+
+    def test_osberve_unobservable_raises(self):
+        summary = Summary("name", "desc", required_labels=["bob"])
+        with pytest.raises(UnobservableMetricException):
+            summary.observe(2)
+
+    def test_observe(self):
+        summary = Summary("name", "desc")
+        summary.observe(0.4)
+
+        assert summary._sum.get() == 0.4
+        assert summary._count.get() == 1
+
+    def test_time(self, summary):
+        with summary.time():
+            pass
+        assert summary._count.get() == 1
+        assert summary._sum.get() != 0
+
+    def test_as_decorator(self, summary):
+        @summary
+        def test():
+            pass
+
+        test()
+        assert summary._count.get() == 1
+        assert summary._sum.get() != 0
+
+    def test_as_decorator_multiple(self, summary):
+        @summary
+        def test():
+            pass
+
+        @summary
+        def test_2():
+            pass
+
+        test()
+        test_2()
+        assert summary._count.get() == 2
+        assert summary._sum.get() != 0
+
+    @pytest.mark.asyncio
+    async def test_as_decorator_async(self, summary):
+        @summary
+        async def test():
+            pass
+
+        await test()
+        assert summary._count.get() == 1
+        assert summary._sum.get() != 0
+
+    @pytest.mark.asyncio
+    async def test_as_decorator_multiple_async(self, summary):
+        @summary
+        async def test():
+            pass
+
+        @summary
+        async def test_2():
+            pass
+
+        await test()
+        await test_2()
+        assert summary._count.get() == 2
+        assert summary._sum.get() != 0
 
 
 class _TestCollector(CustomCollector):
     def collect(self):
         counter = Counter("name", "desc", registry=None)
         counter.inc()
         yield counter
```

### Comparing `pytheus-0.0.9/tests/test_registry.py` & `pytheus-0.1.0/tests/test_registry.py`

 * *Files identical despite different names*

