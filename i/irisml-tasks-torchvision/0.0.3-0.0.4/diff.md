# Comparing `tmp/irisml-tasks-torchvision-0.0.3.tar.gz` & `tmp/irisml-tasks-torchvision-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-torchvision-0.0.3.tar", last modified: Fri Dec  2 01:45:45 2022, max compression
+gzip compressed data, was "irisml-tasks-torchvision-0.0.4.tar", last modified: Fri Jun 16 22:30:22 2023, max compression
```

## Comparing `irisml-tasks-torchvision-0.0.3.tar` & `irisml-tasks-torchvision-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 01:45:45.103771 irisml-tasks-torchvision-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2022-12-02 01:43:50.000000 irisml-tasks-torchvision-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      679 2022-12-02 01:45:45.103771 irisml-tasks-torchvision-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      450 2022-12-02 01:43:50.000000 irisml-tasks-torchvision-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 01:45:45.099771 irisml-tasks-torchvision-0.0.3/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 01:45:45.103771 irisml-tasks-torchvision-0.0.3/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)     6971 2022-12-02 01:43:50.000000 irisml-tasks-torchvision-0.0.3/irisml/tasks/create_torchvision_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3165 2022-12-02 01:43:50.000000 irisml-tasks-torchvision-0.0.3/irisml/tasks/create_torchvision_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     1644 2022-12-02 01:43:50.000000 irisml-tasks-torchvision-0.0.3/irisml/tasks/load_torchvision_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 01:45:45.103771 irisml-tasks-torchvision-0.0.3/irisml_tasks_torchvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      679 2022-12-02 01:45:45.000000 irisml-tasks-torchvision-0.0.3/irisml_tasks_torchvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      526 2022-12-02 01:45:45.000000 irisml-tasks-torchvision-0.0.3/irisml_tasks_torchvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 01:45:45.000000 irisml-tasks-torchvision-0.0.3/irisml_tasks_torchvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-12-02 01:45:45.000000 irisml-tasks-torchvision-0.0.3/irisml_tasks_torchvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2022-12-02 01:45:45.000000 irisml-tasks-torchvision-0.0.3/irisml_tasks_torchvision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-12-02 01:43:50.000000 irisml-tasks-torchvision-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      454 2022-12-02 01:45:45.103771 irisml-tasks-torchvision-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 01:45:45.103771 irisml-tasks-torchvision-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2022-12-02 01:43:50.000000 irisml-tasks-torchvision-0.0.3/test/test_create_torchvision_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      639 2022-12-02 01:43:50.000000 irisml-tasks-torchvision-0.0.3/test/test_create_torchvision_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)      356 2022-12-02 01:43:50.000000 irisml-tasks-torchvision-0.0.3/test/test_load_torchvision_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:22.268285 irisml-tasks-torchvision-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 22:27:36.000000 irisml-tasks-torchvision-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-16 22:30:22.268285 irisml-tasks-torchvision-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-16 22:27:36.000000 irisml-tasks-torchvision-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:22.264285 irisml-tasks-torchvision-0.0.4/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:22.268285 irisml-tasks-torchvision-0.0.4/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-06-16 22:27:36.000000 irisml-tasks-torchvision-0.0.4/irisml/tasks/create_torchvision_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-16 22:27:36.000000 irisml-tasks-torchvision-0.0.4/irisml/tasks/create_torchvision_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-16 22:27:36.000000 irisml-tasks-torchvision-0.0.4/irisml/tasks/load_torchvision_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:22.268285 irisml-tasks-torchvision-0.0.4/irisml_tasks_torchvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-16 22:30:22.000000 irisml-tasks-torchvision-0.0.4/irisml_tasks_torchvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-16 22:30:22.000000 irisml-tasks-torchvision-0.0.4/irisml_tasks_torchvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 22:30:22.000000 irisml-tasks-torchvision-0.0.4/irisml_tasks_torchvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-16 22:30:22.000000 irisml-tasks-torchvision-0.0.4/irisml_tasks_torchvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 22:30:22.000000 irisml-tasks-torchvision-0.0.4/irisml_tasks_torchvision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-16 22:27:36.000000 irisml-tasks-torchvision-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-16 22:30:22.268285 irisml-tasks-torchvision-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:22.268285 irisml-tasks-torchvision-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-16 22:27:36.000000 irisml-tasks-torchvision-0.0.4/test/test_create_torchvision_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-16 22:27:36.000000 irisml-tasks-torchvision-0.0.4/test/test_create_torchvision_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-16 22:27:36.000000 irisml-tasks-torchvision-0.0.4/test/test_load_torchvision_dataset.py
```

### Comparing `irisml-tasks-torchvision-0.0.3/LICENSE` & `irisml-tasks-torchvision-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-torchvision-0.0.3/PKG-INFO` & `irisml-tasks-torchvision-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-torchvision
-Version: 0.0.3
+Version: 0.0.4
 Summary: Torchvision-related tasks for IrisML
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-torchvision-0.0.3/irisml/tasks/create_torchvision_model.py` & `irisml-tasks-torchvision-0.0.4/irisml/tasks/create_torchvision_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-torchvision-0.0.3/irisml/tasks/create_torchvision_transform.py` & `irisml-tasks-torchvision-0.0.4/irisml/tasks/create_torchvision_transform.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,24 +3,33 @@
 from typing import Callable, List
 import torch.nn
 import torchvision.transforms
 import irisml.core
 
 
 class Task(irisml.core.TaskBase):
-    """Create transform objects in torchvision library."""
-    VERSION = '0.1.0'
+    """Create transform objects in torchvision library.
+
+    This task creates a transform object in torchvision library from string expressions.
+    The expression can be a simple method name such as "RandomCrop" or a method call such as "RandomCrop((32, 32))".
+
+    ToTensor is always appended to the end of the transform object.
+
+    Config:
+        transforms ([str]): A list of transform descriptions.
+    """
+    VERSION = '0.1.1'
 
     @dataclasses.dataclass
     class Config:
-        transforms: List[str]
+        transforms: List[str] = dataclasses.field(default_factory=list)
 
     @dataclasses.dataclass
     class Outputs:
-        transform: Callable = None
+        transform: Callable
 
     class Transform:
         def __init__(self, transform_configs: List):
             transform_instances = []
             for method_name, args in transform_configs:
                 transform_class = getattr(torchvision.transforms, method_name)
                 transform_instances.append(transform_class(*args))
@@ -50,15 +59,15 @@
 
             transform_configs.append((method_name, args))
 
         transform = Task.Transform(transform_configs)
         return self.Outputs(transform)
 
     def dry_run(self, inputs):
-        return self.Outputs(torchvision.transforms.ToTensor())
+        return self.execute(inputs)
 
     @staticmethod
     def _parse_transform(expr):
         parsed = ast.parse(expr)
         if len(parsed.body) != 1:
             raise ValueError(f"Transform description cannot have multiple expressions: {expr}")
```

### Comparing `irisml-tasks-torchvision-0.0.3/irisml/tasks/load_torchvision_dataset.py` & `irisml-tasks-torchvision-0.0.4/irisml/tasks/load_torchvision_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-torchvision-0.0.3/irisml_tasks_torchvision.egg-info/PKG-INFO` & `irisml-tasks-torchvision-0.0.4/irisml_tasks_torchvision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-torchvision
-Version: 0.0.3
+Version: 0.0.4
 Summary: Torchvision-related tasks for IrisML
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-torchvision-0.0.3/irisml_tasks_torchvision.egg-info/SOURCES.txt` & `irisml-tasks-torchvision-0.0.4/irisml_tasks_torchvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irisml-tasks-torchvision-0.0.3/test/test_create_torchvision_model.py` & `irisml-tasks-torchvision-0.0.4/test/test_create_torchvision_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-torchvision-0.0.3/test/test_create_torchvision_transform.py` & `irisml-tasks-torchvision-0.0.4/test/test_create_torchvision_transform.py`

 * *Files identical despite different names*

