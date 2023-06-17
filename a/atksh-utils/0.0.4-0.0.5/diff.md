# Comparing `tmp/atksh-utils-0.0.4.tar.gz` & `tmp/atksh-utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.0.4.tar", last modified: Sat Jun 17 06:30:49 2023, max compression
+gzip compressed data, was "atksh-utils-0.0.5.tar", last modified: Sat Jun 17 08:54:43 2023, max compression
```

## Comparing `atksh-utils-0.0.4.tar` & `atksh-utils-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.673572 atksh-utils-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.665572 atksh-utils-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.669572 atksh-utils-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 06:30:49.673572 atksh-utils-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 06:30:49.673572 atksh-utils-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.665572 atksh-utils-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.669572 atksh-utils-0.0.4/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.673572 atksh-utils-0.0.4/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-17 06:30:49.000000 atksh-utils-0.0.4/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.673572 atksh-utils-0.0.4/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 06:30:49.000000 atksh-utils-0.0.4/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-17 06:30:49.000000 atksh-utils-0.0.4/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 06:30:49.000000 atksh-utils-0.0.4/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-17 06:30:49.000000 atksh-utils-0.0.4/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 06:30:49.000000 atksh-utils-0.0.4/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.669572 atksh-utils-0.0.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.673572 atksh-utils-0.0.4/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:54:43.658689 atksh-utils-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:54:43.646689 atksh-utils-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:54:43.650689 atksh-utils-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 08:54:43.658689 atksh-utils-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 08:54:43.658689 atksh-utils-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:54:43.650689 atksh-utils-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:54:43.654689 atksh-utils-0.0.5/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:54:43.658689 atksh-utils-0.0.5/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-17 08:54:43.000000 atksh-utils-0.0.5/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:54:43.654689 atksh-utils-0.0.5/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 08:54:43.000000 atksh-utils-0.0.5/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-17 08:54:43.000000 atksh-utils-0.0.5/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 08:54:43.000000 atksh-utils-0.0.5/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-17 08:54:43.000000 atksh-utils-0.0.5/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 08:54:43.000000 atksh-utils-0.0.5/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:54:43.650689 atksh-utils-0.0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:54:43.658689 atksh-utils-0.0.5/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-17 08:54:30.000000 atksh-utils-0.0.5/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.0.4/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.0.5/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.4/.gitignore` & `atksh-utils-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.4/LICENSE` & `atksh-utils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.4/PKG-INFO` & `atksh-utils-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.0.4/README.md` & `atksh-utils-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.4/pyproject.toml` & `atksh-utils-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.4/src/atksh_utils/openai/api.py` & `atksh-utils-0.0.5/src/atksh_utils/openai/api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.4/src/atksh_utils/openai/functional.py` & `atksh-utils-0.0.5/src/atksh_utils/openai/functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,24 +59,31 @@
             for arg in args.args:
                 argument_name = arg.arg
                 argument_type = self.extract_parameter_type(argument_name, self.func.__doc__)
                 argument_type = str(argument_type).replace(" ", "").replace("\n", "")
                 parameter_description = self.extract_parameter_description(
                     argument_name, self.func.__doc__
                 )
+                argument_type_ = argument_type
+                if "list" in argument_type:
+                    argument_type = "list"
                 if "optional" not in argument_type:
                     required.append(argument_name)
                 elif "," in argument_type:
                     argument_type = argument_type.split(",")[0]
                 elif " " in argument_type:
                     argument_type = argument_type.split(" ")[0]
                 parameters["properties"][argument_name] = {
                     "type": self.type_maps.get(argument_type, argument_type),
                     "description": parameter_description,
                 }
+                if argument_type == "list":
+                    item_type = argument_type_.split("[")[-1].split("]")[0]
+                    item_type = self.type_maps.get(item_type, item_type)
+                    parameters["properties"][argument_name]["items"] = dict(type=item_type)
 
         # Extract function return type
         return_type = None
         if isinstance(tree.body[0], ast.FunctionDef) and tree.body[0].returns:
             return_type = ast.get_source_segment(source, tree.body[0].returns)
             return_type = self.type_maps.get(return_type, return_type)
```

### Comparing `atksh-utils-0.0.4/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.0.5/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.4/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.0.5/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.0.4/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.0.5/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.4/tests/openai/test_api.py` & `atksh-utils-0.0.5/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.4/tests/openai/test_functional.py` & `atksh-utils-0.0.5/tests/openai/test_functional.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from atksh_utils.openai import function_info
 
 
-def my_function(x: int, y: str, flag: bool = False) -> float:
+def my_function(x: int, y: str, z: "list[str]", flag: bool = False) -> float:
     """
     This is a test function.
 
     :param x: An integer.
     :type x: int
     :param y: A string.
     :type y: str
+    :param z: A list of strings.
+    :type z: list[str]
     :param flag: A boolean. Defaults to False.
     :type flag: bool, optional
     :return: A float.
     :rtype: float
     """
     return 3.14
 
@@ -24,13 +26,15 @@
     assert info["name"] == "my_function"
     assert info["description"] == "This is a test function."
     assert info["parameters"]["type"] == "object"
     assert info["parameters"]["properties"]["x"]["type"] == "integer"
     assert info["parameters"]["properties"]["x"]["description"] == "An integer."
     assert info["parameters"]["properties"]["y"]["type"] == "string"
     assert info["parameters"]["properties"]["y"]["description"] == "A string."
+    assert info["parameters"]["properties"]["z"]["type"] == "array"
+    assert info["parameters"]["properties"]["z"]["items"]["type"] == "string"
     assert info["parameters"]["properties"]["flag"]["type"] == "boolean"
     assert (
         info["parameters"]["properties"]["flag"]["description"] == "A boolean. Defaults to False."
     )
-    assert info["parameters"]["required"] == ["x", "y"]
+    assert info["parameters"]["required"] == ["x", "y", "z"]
     assert info["return_type"] == "number"
```

