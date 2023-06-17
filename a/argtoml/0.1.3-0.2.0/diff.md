# Comparing `tmp/argtoml-0.1.3.tar.gz` & `tmp/argtoml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argtoml-0.1.3.tar", last modified: Thu Jun 15 22:16:30 2023, max compression
+gzip compressed data, was "argtoml-0.2.0.tar", last modified: Sat Jun 17 20:45:46 2023, max compression
```

## Comparing `argtoml-0.1.3.tar` & `argtoml-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:16:30.603556 argtoml-0.1.3/
--rw-r--r--   0 gum       (1000) gum       (1000)     1069 2023-06-10 10:02:47.000000 argtoml-0.1.3/LICENSE
--rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-15 22:16:30.603556 argtoml-0.1.3/PKG-INFO
--rw-r--r--   0 gum       (1000) gum       (1000)     1522 2023-06-07 09:20:09.000000 argtoml-0.1.3/README.md
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:16:30.600223 argtoml-0.1.3/argtoml/
--rw-r--r--   0 gum       (1000) gum       (1000)       92 2023-06-05 13:46:56.000000 argtoml-0.1.3/argtoml/__init__.py
--rw-r--r--   0 gum       (1000) gum       (1000)     7832 2023-06-15 22:16:08.000000 argtoml-0.1.3/argtoml/main.py
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:16:30.603556 argtoml-0.1.3/argtoml/tests/
--rw-r--r--   0 gum       (1000) gum       (1000)       25 2023-06-09 12:19:14.000000 argtoml-0.1.3/argtoml/tests/__init__.py
--rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.3/argtoml/tests/test_main.py
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:16:30.603556 argtoml-0.1.3/argtoml.egg-info/
--rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-15 22:16:30.000000 argtoml-0.1.3/argtoml.egg-info/PKG-INFO
--rw-r--r--   0 gum       (1000) gum       (1000)      273 2023-06-15 22:16:30.000000 argtoml-0.1.3/argtoml.egg-info/SOURCES.txt
--rw-r--r--   0 gum       (1000) gum       (1000)        1 2023-06-15 22:16:30.000000 argtoml-0.1.3/argtoml.egg-info/dependency_links.txt
--rw-r--r--   0 gum       (1000) gum       (1000)        8 2023-06-15 22:16:30.000000 argtoml-0.1.3/argtoml.egg-info/top_level.txt
--rw-r--r--   0 gum       (1000) gum       (1000)      939 2023-06-15 22:16:20.000000 argtoml-0.1.3/pyproject.toml
--rw-r--r--   0 gum       (1000) gum       (1000)       38 2023-06-15 22:16:30.603556 argtoml-0.1.3/setup.cfg
--rw-r--r--   0 gum       (1000) gum       (1000)       61 2023-06-07 07:31:31.000000 argtoml-0.1.3/setup.py
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:16:30.603556 argtoml-0.1.3/tests/
--rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.3/tests/test_main.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-17 20:45:46.706484 argtoml-0.2.0/
+-rw-r--r--   0 gum       (1000) gum       (1000)     1069 2023-06-10 10:02:47.000000 argtoml-0.2.0/LICENSE
+-rw-r--r--   0 gum       (1000) gum       (1000)     2518 2023-06-17 20:45:46.703151 argtoml-0.2.0/PKG-INFO
+-rw-r--r--   0 gum       (1000) gum       (1000)     2005 2023-06-17 20:45:18.000000 argtoml-0.2.0/README.md
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-17 20:45:46.699818 argtoml-0.2.0/argtoml/
+-rw-r--r--   0 gum       (1000) gum       (1000)       92 2023-06-05 13:46:56.000000 argtoml-0.2.0/argtoml/__init__.py
+-rw-r--r--   0 gum       (1000) gum       (1000)     8126 2023-06-17 20:00:08.000000 argtoml-0.2.0/argtoml/main.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-17 20:45:46.703151 argtoml-0.2.0/argtoml/tests/
+-rw-r--r--   0 gum       (1000) gum       (1000)       25 2023-06-09 12:19:14.000000 argtoml-0.2.0/argtoml/tests/__init__.py
+-rw-r--r--   0 gum       (1000) gum       (1000)      218 2023-06-17 20:40:27.000000 argtoml-0.2.0/argtoml/tests/test_main.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-17 20:45:46.703151 argtoml-0.2.0/argtoml.egg-info/
+-rw-r--r--   0 gum       (1000) gum       (1000)     2518 2023-06-17 20:45:46.000000 argtoml-0.2.0/argtoml.egg-info/PKG-INFO
+-rw-r--r--   0 gum       (1000) gum       (1000)      273 2023-06-17 20:45:46.000000 argtoml-0.2.0/argtoml.egg-info/SOURCES.txt
+-rw-r--r--   0 gum       (1000) gum       (1000)        1 2023-06-17 20:45:46.000000 argtoml-0.2.0/argtoml.egg-info/dependency_links.txt
+-rw-r--r--   0 gum       (1000) gum       (1000)        8 2023-06-17 20:45:46.000000 argtoml-0.2.0/argtoml.egg-info/top_level.txt
+-rw-r--r--   0 gum       (1000) gum       (1000)      922 2023-06-17 20:44:32.000000 argtoml-0.2.0/pyproject.toml
+-rw-r--r--   0 gum       (1000) gum       (1000)       38 2023-06-17 20:45:46.706484 argtoml-0.2.0/setup.cfg
+-rw-r--r--   0 gum       (1000) gum       (1000)       61 2023-06-07 07:31:31.000000 argtoml-0.2.0/setup.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-17 20:45:46.703151 argtoml-0.2.0/tests/
+-rw-r--r--   0 gum       (1000) gum       (1000)      218 2023-06-17 20:40:27.000000 argtoml-0.2.0/tests/test_main.py
```

### Comparing `argtoml-0.1.3/LICENSE` & `argtoml-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `argtoml-0.1.3/PKG-INFO` & `argtoml-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,91 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.1.3
+Version: 0.2.0
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
-Author-email: Jochem Hölscher <jono-dev.6psuo@simplelogin.com>
+Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
----
-created_datetime: 2023-06-05T21:51:00
----
-
 # README
 
 The `argtoml` package wraps around `argparse`.
 It adds the content of a toml file to the cli options.
 After parsing, it creates a `types.SimpleNameSpace` object.
 
-## usage
-
-Use `argtoml` the same as you would use `argparse`.
-If you don't provide the location for the toml file, it will search for one in the current directory or any parent directory of the main file (in)directly importing `argtoml`.
-
-```python
-from argtoml import ArgumentParser, arg_parse
+## install
 
-parser = ArgumentParser()
-parser.add_argument("--path", default="./")
-parser.add_argument("--project.name", default="argtoml")
-args = arg_parse(parser)
+```sh
+pip install argtoml
 ```
 
-If we, for example have the following config.toml in the same directory as the above script
+## usage
+
+If there's a `src/config.toml`
 
 ```toml
+debug = true
+home = "~"
+
 [project]
 author = "Jono"
 name = "argconfig"
+pyproject = "./pyproject.toml"
 ```
 
-then args is an object with the following entries.
+and a `src/__main__.py`
 
 ```python
-assert args.path == "./"
-assert args.project.author == "Jono"
-assert args.project.name == "argtoml"
+from argtoml import parse_args  # , ArgumentParser
+
+args = parse_args(path=True)
+print(args.debug)
+print(args.home)
+print(args.project.author)
+print(args.project.name)
+print(args.project.pyproject)
 ```
 
+then the shell can look like
+
+```sh
+$ pwd
+/home/jono/project
+$ python src/__main__.py --project.name argtoml --no-debug
+False
+/home/jono
+Jono
+argtoml
+/home/jono/project/pyproject.toml
+```
+
+## packaging
+
+`argtoml` works with a packaged toml file. You can provide it's path like this.
+
+```python
+arg_parse(toml="my_config.toml")
+```
+
+If you provide a relative path, `argtoml` will look for `my_config.toml` in the package directory if the main file using `argtoml` is from a package, otherwise `argtoml` will look for `my_config.toml` in the same directory as the main file.
+If you want to ship a toml file with your package, make sure to [add the toml file to your package](https://setuptools.pypa.io/en/latest/userguide/datafiles.html).
+
 ## notes
 
 This is a personal tool thus far, some idiosyncrasies remain:
 
 - Adding dotted arguments not present in the toml might break everything I didn't even test this.
 - I didn't test any arrays, they should work?
 - I don't feel like adding other formats but toml.
-- I don't know if, in the above example, the user can do something like `main.py --project {author=jo3} --project.author jjj`, but it should crash if they do this.
+- I don't know if, in the above example, the user can do something like `python __main__.py --project {author="jo3"} --project.author jjj`, but it should crash if they do this.
+- Interpreting strings as paths _probably_ only works with unix style paths.
 
 ## todos
 
 - Add toml comments as argument descriptions.
 - Pretty-print the output of parse_args.
-
+- Load and merge multiple toml files
```

### Comparing `argtoml-0.1.3/argtoml/main.py` & `argtoml-0.2.0/argtoml/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,88 +2,84 @@
 # vim:fenc=utf-8
 
 """
 Create an argument parser from a toml file.
 """
 
 import builtins
-import os
 import tomllib
 from argparse import ArgumentParser
 from ast import literal_eval
+from importlib.resources import as_file, files
 from pathlib import Path
 from types import SimpleNamespace
 from typing import Optional, Union
 
 import __main__
 
-TOML_PATH = ""
+TOML_PATH: Path
+
 
 class Struct:
     def __init__(self, **entries):
         self.__dict__.update(entries)
 
     def __repr__(self):
         return "<%s>" % str(
             "\n ".join("%s : %s" % (k, repr(v)) for (k, v) in self.__dict__.items())
         )
 
-def string_to_path(string: str, prefix: Path = Path.cwd()):
+
+def string_to_path(string: str, prefix: Path) -> Union[Path, str]:
     """
     Convert a string to a Path object.
     """
     if string == "~":
         return Path.home()
+
     elif string == ".":
         return prefix
+
     elif string == "..":
         return prefix.parent
+
     elif len(string) > 0 and string[0] == "/":
         return Path(string)
+
     elif len(string) > 1 and string[0:2] == "~/":
         return Path.home() / string[2:]
+
     elif len(string) > 1 and string[0:2] == "./":
         return prefix / string[2:]
+
     elif len(string) > 2 and string[0:3] == "../":
         return prefix.parent / string[3:]
+
     else:
         return string
 
 
-def locate_toml():
+def locate_toml(base: Path, relative: Union[str, Path]):
     """
     Locate the toml file in the current directory.
     """
-    # The toml file can be named config.toml or have the same name as the main file..
-    main_file = Path(__main__.__file__)
-    toml_file_names = ["config.toml"]
-    if main_file.name != "main.py":
-        toml_file_names.append(main_file.stem + ".toml")
-
-    # The toml file can also be named after the project directory.
-    dir = main_file.parent
-    if dir.name != "":
-        if dir.name == "src":
-            toml_file_names.append(dir.parent.name + ".toml")
-        else:
-            toml_file_names.append(dir.name + ".toml")
+    path: Path
+    if type(relative) == str:
+        relative = string_to_path(relative, base)
+    if not Path(relative).is_absolute():
+        path = base / relative
+    else:
+        path = Path(relative)
 
-    # Search for the toml file in the current directory.
-    for file in os.listdir("."):
-        if file in toml_file_names:
-            return str(Path.cwd() / file)
-
-    # Search for the toml file in the project directory or its parents.
-    while dir.name != "":
-        for file in os.listdir(dir):
-            if file in toml_file_names:
-                return os.path.join(dir, file)
-        dir = dir.parent
+    if path.is_file():
+        return path
 
-    raise FileNotFoundError("No toml config file found current, or project directory")
+    raise FileNotFoundError(
+        f"No toml config file found at {path}, or project directory"
+    )
 
 
 def add_toml_args(parser, toml, prefix=""):
     """
     Add the content of a toml file as argument with default values
     to an ArgumentParser object.
     """
@@ -110,15 +106,15 @@
                 f"--{prefix}{key}",
                 required=False,
                 type=type_,
                 help=f"defaults to {value}",
             )
 
 
-def fill_toml_args(args, toml, prefix="", filled=False, path: Optional[Path]=None):
+def fill_toml_args(args, toml, prefix="", filled=False, path: Optional[Path] = None):
     namespace = SimpleNamespace()
     for raw_key, value in toml.items():
         # Check if the user provided the same key but with dashes instead of underscores.
         key = raw_key.replace("-", "_")
         key_str = prefix + "." + key if prefix else key
         # Boolean variables have 2 arguments.
         alt_key_str = prefix + ".no_" + key if prefix else "no_" + key
@@ -129,26 +125,28 @@
             )
 
         arg_value = args[key_str] if key_str in args else None
 
         # Fill in the default value from the toml file.
         if arg_value is None:
             if type(value) == dict:
-                setattr(namespace, key, fill_toml_args(args, value, key, filled, path=path))
+                setattr(
+                    namespace, key, fill_toml_args(args, value, key, filled, path=path)
+                )
             # Check whether both boolean arguments are empty before filling in the default.
             elif type(value) == bool:
                 if args[alt_key_str] is None:
                     setattr(namespace, key, value)  # Fill in the default.
                 else:
                     setattr(namespace, key, False)  # The anti-argument was called.
                     del args[alt_key_str]
 
             elif path is not None and type(value) == str:
                 setattr(namespace, key, string_to_path(value, path))
-                
+
             else:
                 setattr(namespace, key, value)
 
         # Fill in the value from the command line.
         else:
             if filled:
                 raise Exception(
@@ -159,30 +157,40 @@
                 match type(value):
                     case builtins.list:
                         arg_value = literal_eval(arg_value)
                         assert type(arg_value) == list
                         for i, arg in enumerate(arg_value):
                             if type(arg) == dict:
                                 # TODO; I might need to check for whether any values are filled twice.
-                                arg_value[i] = fill_toml_args(args, arg, key, filled, path=path)
+                                arg_value[i] = fill_toml_args(
+                                    args, arg, key, filled, path=path
+                                )
 
                     case builtins.dict:
                         # Check if values are not filled twice.
                         fill_toml_args(args, value, key, True, path=path)
                         arg_value = literal_eval(arg_value)
                         assert type(arg_value) == dict
-                        arg_value = fill_toml_args(args, arg_value, key, filled, path=path)
+                        arg_value = fill_toml_args(
+                            args, arg_value, key, filled, path=path
+                        )
 
                     case builtins.bool:
                         assert type(arg_value) == bool
                         if args[alt_key_str] is not None:
-                            raise ValueError(f"Do not call --{key_str} and --{alt_key_str} simultaneously.")
+                            raise ValueError(
+                                f"Do not call --{key_str} and --{alt_key_str} simultaneously."
+                            )
                     case builtins.str:
                         assert type(arg_value) == str
-                        arg_value = string_to_path(arg_value, path) if path is not None else arg_value
+                        arg_value = (
+                            string_to_path(arg_value, path)
+                            if path is not None
+                            else arg_value
+                        )
 
                     case _:
                         assert type(value) == type(arg_value)
 
             except AssertionError:
                 raise TypeError(
                     f"Type mismatch for {key_str}: the type from {TOML_PATH} is {type(value)}, but the CLI got a {type(arg_value)}"
@@ -190,34 +198,50 @@
 
             setattr(namespace, key, arg_value)
             del args[key_str]
 
     return namespace
 
 
-def parse_args(parser=ArgumentParser(), toml=None, path: Union[Path, bool]=False):
+def parse_args(
+    parser=None,
+    description="",
+    toml: Union[Path, str] = "config.toml",
+    path: Union[Path, bool] = False,
+):
     """
     Add the content of a toml file as argument with default values
     to an ArgumentParser object.
     """
 
-    # Locate the toml file.
+    # Locate and read the toml file.
+    package = __main__.__package__
     global TOML_PATH
-    if toml is None:
-        toml = locate_toml()
-        TOML_PATH = toml
-
-    if path == True:
-        path = Path(toml).parent
+    if package:
+        with as_file(files(package)) as package_path:
+            TOML_PATH = locate_toml(package_path, toml)
+    else:
+        TOML_PATH = locate_toml(Path(__main__.__file__).parent, toml)
+    with open(TOML_PATH, "rb") as f:
+        toml_doc = tomllib.load(f)
 
     # Add the keys from the toml file as arguments.
-    with open(toml, "rb") as f:
-        toml = tomllib.load(f)
-    add_toml_args(parser, toml)
+    if parser is None:
+        parser = ArgumentParser(
+            description=description
+            + f"\nCLI arguments are constructed from {TOML_PATH}. View that file for more documentation"
+        )
+    add_toml_args(parser, toml_doc)
     args = vars(parser.parse_args())
 
-    namespace = fill_toml_args(args, toml, path=path if path else None)
+    if path == True:
+        namespace = fill_toml_args(args, toml_doc, path=TOML_PATH.parent)
+    elif path == False:
+        namespace = fill_toml_args(args, toml_doc)
+    else:
+        namespace = fill_toml_args(args, toml_doc, path=path)
+
     for key, value in args.items():
         if value is not None:
             setattr(namespace, key, value)
 
     return namespace
```

### Comparing `argtoml-0.1.3/argtoml.egg-info/PKG-INFO` & `argtoml-0.2.0/argtoml.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,91 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.1.3
+Version: 0.2.0
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
-Author-email: Jochem Hölscher <jono-dev.6psuo@simplelogin.com>
+Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
----
-created_datetime: 2023-06-05T21:51:00
----
-
 # README
 
 The `argtoml` package wraps around `argparse`.
 It adds the content of a toml file to the cli options.
 After parsing, it creates a `types.SimpleNameSpace` object.
 
-## usage
-
-Use `argtoml` the same as you would use `argparse`.
-If you don't provide the location for the toml file, it will search for one in the current directory or any parent directory of the main file (in)directly importing `argtoml`.
-
-```python
-from argtoml import ArgumentParser, arg_parse
+## install
 
-parser = ArgumentParser()
-parser.add_argument("--path", default="./")
-parser.add_argument("--project.name", default="argtoml")
-args = arg_parse(parser)
+```sh
+pip install argtoml
 ```
 
-If we, for example have the following config.toml in the same directory as the above script
+## usage
+
+If there's a `src/config.toml`
 
 ```toml
+debug = true
+home = "~"
+
 [project]
 author = "Jono"
 name = "argconfig"
+pyproject = "./pyproject.toml"
 ```
 
-then args is an object with the following entries.
+and a `src/__main__.py`
 
 ```python
-assert args.path == "./"
-assert args.project.author == "Jono"
-assert args.project.name == "argtoml"
+from argtoml import parse_args  # , ArgumentParser
+
+args = parse_args(path=True)
+print(args.debug)
+print(args.home)
+print(args.project.author)
+print(args.project.name)
+print(args.project.pyproject)
 ```
 
+then the shell can look like
+
+```sh
+$ pwd
+/home/jono/project
+$ python src/__main__.py --project.name argtoml --no-debug
+False
+/home/jono
+Jono
+argtoml
+/home/jono/project/pyproject.toml
+```
+
+## packaging
+
+`argtoml` works with a packaged toml file. You can provide it's path like this.
+
+```python
+arg_parse(toml="my_config.toml")
+```
+
+If you provide a relative path, `argtoml` will look for `my_config.toml` in the package directory if the main file using `argtoml` is from a package, otherwise `argtoml` will look for `my_config.toml` in the same directory as the main file.
+If you want to ship a toml file with your package, make sure to [add the toml file to your package](https://setuptools.pypa.io/en/latest/userguide/datafiles.html).
+
 ## notes
 
 This is a personal tool thus far, some idiosyncrasies remain:
 
 - Adding dotted arguments not present in the toml might break everything I didn't even test this.
 - I didn't test any arrays, they should work?
 - I don't feel like adding other formats but toml.
-- I don't know if, in the above example, the user can do something like `main.py --project {author=jo3} --project.author jjj`, but it should crash if they do this.
+- I don't know if, in the above example, the user can do something like `python __main__.py --project {author="jo3"} --project.author jjj`, but it should crash if they do this.
+- Interpreting strings as paths _probably_ only works with unix style paths.
 
 ## todos
 
 - Add toml comments as argument descriptions.
 - Pretty-print the output of parse_args.
-
+- Load and merge multiple toml files
```

### Comparing `argtoml-0.1.3/pyproject.toml` & `argtoml-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "argtoml"
-version = "0.1.3"
+version = "0.2.0"
 description = "Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file."
 dynamic = ["readme"]
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -15,15 +15,15 @@
 github = "https://github.com/JJJHolscher/argtoml"
 
 [project.urls]
 homepage = "https://github.com/JJJHolscher/argtoml"
 
 [[project.authors]]
 name = "Jochem Hölscher"
-email = "jono-dev.6psuo@simplelogin.com"
+email = "a.fake@e.mail"
 
 [build-system]
 requires = [
     "setuptools>=61.0",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
```

