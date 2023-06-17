# Comparing `tmp/Architectural Lens-0.0.4.tar.gz` & `tmp/Architectural Lens-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Architectural Lens-0.0.4.tar", last modified: Fri Apr 14 10:24:16 2023, max compression
+gzip compressed data, was "Architectural Lens-0.0.5.tar", last modified: Sat Jun 17 10:20:57 2023, max compression
```

## Comparing `Architectural Lens-0.0.4.tar` & `Architectural Lens-0.0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/Architectural_Lens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 10:24:16.000000 Architectural Lens-0.0.4/Architectural_Lens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-14 10:24:16.000000 Architectural Lens-0.0.4/Architectural_Lens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:24:16.000000 Architectural Lens-0.0.4/Architectural_Lens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 10:24:16.000000 Architectural Lens-0.0.4/Architectural_Lens.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 10:24:16.000000 Architectural Lens-0.0.4/Architectural_Lens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 10:24:16.000000 Architectural Lens-0.0.4/Architectural_Lens.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 10:24:16.945555 Architectural Lens-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/cli_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/core/bt_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/core/bt_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/core/bt_module.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/src/plantuml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantuml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantuml/fetch_git.py
--rw-r--r--   0 runner    (1001) docker     (123)    19854 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantuml/plantuml_file_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/src/plantumlv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantumlv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantumlv2/pu_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantumlv2/pu_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantumlv2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/utils/config_manager_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/utils/path_manager_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:20:57.863391 Architectural Lens-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:20:57.859391 Architectural Lens-0.0.5/Architectural_Lens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-17 10:20:57.000000 Architectural Lens-0.0.5/Architectural_Lens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-17 10:20:57.000000 Architectural Lens-0.0.5/Architectural_Lens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 10:20:57.000000 Architectural Lens-0.0.5/Architectural_Lens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-17 10:20:57.000000 Architectural Lens-0.0.5/Architectural_Lens.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-17 10:20:57.000000 Architectural Lens-0.0.5/Architectural_Lens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-17 10:20:57.000000 Architectural Lens-0.0.5/Architectural_Lens.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-17 10:20:57.863391 Architectural Lens-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-17 10:20:57.863391 Architectural Lens-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:20:57.859391 Architectural Lens-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/cli_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:20:57.859391 Architectural Lens-0.0.5/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/core/bt_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/core/bt_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/core/bt_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:20:57.859391 Architectural Lens-0.0.5/src/plantuml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/plantuml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/plantuml/fetch_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19854 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/plantuml/plantuml_file_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:20:57.863391 Architectural Lens-0.0.5/src/plantumlv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/plantumlv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/plantumlv2/pu_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/plantumlv2/pu_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/plantumlv2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:20:57.863391 Architectural Lens-0.0.5/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/utils/config_manager_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-17 10:20:47.000000 Architectural Lens-0.0.5/src/utils/path_manager_singleton.py
```

### Comparing `Architectural Lens-0.0.4/Architectural_Lens.egg-info/SOURCES.txt` & `Architectural Lens-0.0.5/Architectural_Lens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.4/README.md` & `Architectural Lens-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.4/setup.py` & `Architectural Lens-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Architectural Lens",
-    version="0.0.4",
+    version="0.0.5",
     description="Thesis project",
     author="Nikolai Perlt",
     author_email="npe@itu.dk",
     url="https://github.com/Perlten/MT-diagrams",
     packages=find_packages(),
     long_description="This is the long description",
     install_requires=[
```

### Comparing `Architectural Lens-0.0.4/src/cli_interface.py` & `Architectural Lens-0.0.5/src/cli_interface.py`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.4/src/core/bt_file.py` & `Architectural Lens-0.0.5/src/core/bt_file.py`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.4/src/core/bt_graph.py` & `Architectural Lens-0.0.5/src/core/bt_graph.py`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.4/src/core/bt_module.py` & `Architectural Lens-0.0.5/src/core/bt_module.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,16 @@
         files = [
             element
             for element in os.listdir(self.path)
             if element.endswith(".py")
         ]
 
         for file in files:
+            if file == "testing.py":
+                continue
             bt_file = BTFile(
                 label=file.split("/")[-1], module=self, am=self.am
             )
             bt_file.ast = self.am.ast_from_file(os.path.join(self.path, file))
             self.file_list.append(bt_file)
 
     def get_files_recursive(self) -> list[BTFile]:
```

### Comparing `Architectural Lens-0.0.4/src/plantuml/plantuml_file_creator.py` & `Architectural Lens-0.0.5/src/plantuml/plantuml_file_creator.py`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.4/src/plantumlv2/pu_entities.py` & `Architectural Lens-0.0.5/src/plantumlv2/pu_entities.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,22 @@
                         self.bt_package,
                         bt_package_dependency,
                     )
                 )
             except Exception:
                 pass
 
+    def get_parent_list(self):
+        res = []
+        if self.parent is None:
+            return res
+        res.append(self.parent)
+        res.extend(self.parent.get_parent_list())
+        return res
+
     def render_package(self) -> str:
         config_manager = ConfigManagerSingleton()
         state_str = self.state.value
         if self.state == EntityState.NEUTRAL:
             state_str = config_manager.package_color
 
         return f'package "{self.name}" {state_str}'
@@ -84,14 +92,27 @@
         self, used_packages: set["PuPackage"]
     ):
         for sub_module in self.sub_modules:
             if sub_module not in used_packages:
                 sub_module.filter_excess_packages_dependencies(used_packages)
                 self.pu_dependency_list.extend(sub_module.pu_dependency_list)
 
+        for dependency in self.pu_dependency_list:
+            l = dependency.to_package.get_parent_list()
+            for p in l:
+                if p in used_packages:
+                    dep = PuDependency(
+                        self,
+                        p,
+                        dependency.from_bt_package,
+                        dependency.to_bt_package,
+                    )
+                    self.pu_dependency_list.append(dep)
+                    break
+
         # change all from package to self
         for dependency in self.pu_dependency_list:
             dependency.from_package = self
 
         # filter all dependencies pointing to self
         self.pu_dependency_list = [
             dependency
```

### Comparing `Architectural Lens-0.0.4/src/plantumlv2/pu_manager.py` & `Architectural Lens-0.0.5/src/plantumlv2/pu_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,24 @@
 from src.plantumlv2.utils import get_pu_package_path_from_bt_package
 import os
 
 
 def render_pu(graph: BTGraph, config: dict):
     views = _create_pu_graph(graph, config)
     for view_name, pu_package_map in views.items():
+        if os.getenv("MT_DEBUG"):
+            dep_count = sum(
+                len(package.pu_dependency_list)
+                for package in pu_package_map.values()
+            )
+            package_count = len(list(pu_package_map.values()))
+            print("View name:", view_name)
+            print("Package count:", package_count)
+            print("Dependency count:", dep_count)
+
         plant_uml_str = _render_pu_graph(
             list(pu_package_map.values()), view_name, config
         )
         project_name = config["name"]
         save_location = os.path.join(
             config["saveLocation"], f"{project_name}-{view_name}"
         )
```

### Comparing `Architectural Lens-0.0.4/src/utils/functions.py` & `Architectural Lens-0.0.5/src/utils/functions.py`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.4/src/utils/path_manager_singleton.py` & `Architectural Lens-0.0.5/src/utils/path_manager_singleton.py`

 * *Files identical despite different names*

