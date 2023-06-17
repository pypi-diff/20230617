# Comparing `tmp/unasyncd-0.2.1.tar.gz` & `tmp/unasyncd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unasyncd-0.2.1.tar", max compression
+gzip compressed data, was "unasyncd-0.3.0.tar", max compression
```

## Comparing `unasyncd-0.2.1.tar` & `unasyncd-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-06-10 12:20:34.638068 unasyncd-0.2.1/LICENSE
--rw-r--r--   0        0        0    15986 2023-06-10 12:20:34.638068 unasyncd-0.2.1/README.md
--rw-r--r--   0        0        0      908 2023-06-10 12:20:34.638068 unasyncd-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-10 12:20:34.638068 unasyncd-0.2.1/unasyncd/__init__.py
--rw-r--r--   0        0        0     3836 2023-06-10 12:20:34.638068 unasyncd-0.2.1/unasyncd/cli.py
--rw-r--r--   0        0        0     2482 2023-06-10 12:20:34.638068 unasyncd-0.2.1/unasyncd/config.py
--rw-r--r--   0        0        0    10306 2023-06-10 12:20:34.638068 unasyncd-0.2.1/unasyncd/main.py
--rw-r--r--   0        0        0    36834 2023-06-10 12:20:34.638068 unasyncd-0.2.1/unasyncd/transformers.py
--rw-r--r--   0        0        0    16696 1970-01-01 00:00:00.000000 unasyncd-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-17 09:23:10.690536 unasyncd-0.3.0/LICENSE
+-rw-r--r--   0        0        0    17755 2023-06-17 09:23:10.690536 unasyncd-0.3.0/README.md
+-rw-r--r--   0        0        0      995 2023-06-17 09:23:10.690536 unasyncd-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-17 09:23:10.690536 unasyncd-0.3.0/unasyncd/__init__.py
+-rw-r--r--   0        0        0     4089 2023-06-17 09:23:10.690536 unasyncd-0.3.0/unasyncd/cli.py
+-rw-r--r--   0        0        0     2553 2023-06-17 09:23:10.690536 unasyncd-0.3.0/unasyncd/config.py
+-rw-r--r--   0        0        0    10349 2023-06-17 09:23:10.690536 unasyncd-0.3.0/unasyncd/main.py
+-rw-r--r--   0        0        0    37540 2023-06-17 09:23:10.690536 unasyncd-0.3.0/unasyncd/transformers.py
+-rw-r--r--   0        0        0    18624 1970-01-01 00:00:00.000000 unasyncd-0.3.0/PKG-INFO
```

### Comparing `unasyncd-0.2.1/LICENSE` & `unasyncd-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unasyncd-0.2.1/README.md` & `unasyncd-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     * [As a pre-commit hook](#as-a-pre-commit-hook)
     * [Configuration](#configuration)
       * [File](#file)
       * [CLI options](#cli-options)
       * [Exclusions](#exclusions)
       * [Extending name replacements](#extending-name-replacements)
     * [Handling of imports](#handling-of-imports)
+    * [Integration with linters](#integration-with-linters)
     * [Limitations](#limitations)
     * [Disclaimer](#disclaimer)
 <!-- TOC -->
 
 ## What can be transformed?
 
 Unasyncd supports a wide variety of transformation, ranging from simple name
@@ -393,15 +394,15 @@
 
 ### As a pre-commit hook
 
 Unasyncd is available as a pre-commit hook:
 
 ```yaml
 - repo: https://github.com/provinzkraut/unasyncd
-  rev: v0.2.0
+  rev: v0.2.1
   hooks:
     - id: unasyncd
 ```
 
 ### Configuration
 
 Unasyncd can be configured via a `pyproject.toml` file, a dedicated `.unasyncd.toml`
@@ -417,14 +418,15 @@
 | `add_replacements`            | table | -       | A table of additional name replacements                                            |
 | `per_file_add_replacements`   | table | -       | A table mapping file names to tables of additional replacements                    |
 | `transform_docstrings`        | bool  | false   | Enable transformation of docstrings                                                |
 | `add_editors_note`            | bool  | false   | Add a note on top of the generated files                                           |
 | `infer_type_checking_imports` | bool  | true    | Infer if new imports should be added to an 'if TYPE_CHECKING' block                |
 | `cache`                       | bool  | true    | Cache transformation results                                                       |
 | `force_regen`                 | bool  | false   | Always regenerate files, regardless if their content has changed                   |
+| `ruff_fix`                    | bool  | false   | Run `ruff --fix` on the generated code                                             |
 
 **Example**
 
 ```toml
 [tool.unasyncd]
 files = { "async_thing.py" = "sync_thing.py", "foo.py" = "bar.py" }
 exclude = ["Something", "SomethingElse.within"]
@@ -436,26 +438,29 @@
 no_cache = false
 no_cache = false
 force_regen = false
 ```
 
 #### CLI options
 
-*Feature flags corresponding to configuration values*
+*Feature flags corresponding to configuration values. These will override the
+configuration file values*
 
 | option                             | description                                                         |
 |------------------------------------|---------------------------------------------------------------------|
 | `--cache`                          | Cache transformation results                                        |
 | `--no-cache `                      | Don't cache transformation results                                  |
 | `--transform-docstrings`           | Enable transformation of docstrings                                 |
 | `--no-transform-docstrings`        | Inverse of `--transform-docstrings`                                 |
 | `--infer-type-checking-imports`    | Infer if new imports should be added to an 'if TYPE_CHECKING' block |
 | `--no-infer-type-checking-imports` | Inverse of `infer-type-checking-imports`                            |
 | `--add-editors-note`               | Add a note on top of each generated file                            |
 | `--no-add-editors-note`            | Inverse of `--add-editors-note`                                     |
+| `--ruff-fix`                       | Run `ruff --fix` on the generated code                              |
+| `--no-ruff-fix`                    | Inverse of `--ruff-fix`                                             |
 | `--force`                          | Always regenerate files, regardless if their content has changed    |
 | `--no-force`                       | Inverse of `--force`                                                |
 | `--check`                          | Don't write changes back to files                                   |
 | `--write`                          | Inverse of `--check`                                                |
 
 
 *Additional CLI options*
@@ -525,16 +530,44 @@
    comment
 
 Unasyncd will not remove imports that have become unused as a result of the applied
 transformations. This is because tracking of usages is a complex task and best left to
 tools made specifically for this job like [ruff](https://beta.ruff.rs/docs) or
 [autoflake](https://github.com/PyCQA/autoflake).
 
-Not doing this work twice - e.g. employing a tool to automatically remove unused
-imports alongside unasyncd - can also be a significant performance improvement.
+
+### Integration with linters
+
+Using unasyncd in conjunction with linters offering autofixing behaviour can lead to an
+edit-loop, where unasyncd generates a new file which the other tool then changes in a
+non-AST-equivalent way - for example by removing an import that has become unused as a
+result of the transformation applied by unasyncd -, in turn causing unasyncd to
+regenerate the file the next time it is invoked, since the target file is no longer
+AST-equivalent to what unasyncd thinks it should be.
+
+To alleviate this, unasyncd offers a [ruff](https://beta.ruff.rs/docs) integration,
+which can automatically run `ruff --fix` on the generated code before writing it back.
+It will use the existing ruff configuration for this to ensure the fixes applied to
+adhere to the rules used throughout the project.
+
+If this option is used, the transformed code will never be altered by ruff, therefore
+breaking the cycle.
+
+This option can be enabled with the `ruff_fix = true` feature flag, or by using the
+`--ruff-fix` CLI flag.
+
+Usage of this option requires an installation of `ruff`. If not independently installed,
+it can be installed as an extra of unasyncd: `pip install unasyncd[ruff]`.
+
+**Why is only ruff supported?**
+
+Ruff was chosen for its speed, having a negligible impact on the overall performance of
+unasyncd, and because it can replace most of the common linters / tools with autofixing
+capabilities, removing the need for separate integrations.
+
 
 ### Limitations
 
 Transformations for `contextlib.AsyncContextManager`, `asyncio.TaskGroup` and
 `anyio.create_task_group` only work when they're being called in a `with` statement
 directly. This is due to the fact that unasyncd does not track assignments or support
 type inference. Support for these usages might be added in a future version.
```

### Comparing `unasyncd-0.2.1/pyproject.toml` & `unasyncd-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 [tool.poetry]
 name = "unasyncd"
-version = "0.2.1"
+version = "0.3.0"
 description = "A tool to transform asynchronous Python code to synchronous Python code."
 authors = ["Janek Nouvertné <j.a.nouvertne@posteo.de>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 libcst = "^1.0.0"
 click = "^8.1.3"
 rich = "^13.4.1"
 anyio = "^3.7.0"
-msgspec = "^0.15.1"
+msgspec = "^0.16.0"
 tomli-w = "^1.0.0"
 rich-click = "^1.6.1"
+ruff = {version = "*", optional = true}
+
+[tool.poetry.extras]
+ruff = ["ruff"]
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pre-commit = "^3.3.2"
 pytest-mock = "^3.10.0"
+ruff = "*"
 
 
 [tool.poetry.scripts]
 unasyncd = "unasyncd.cli:main"
 
 
 [tool.ruff]
@@ -33,15 +38,15 @@
     "F",  # pyflakes
     "ERA", # eradicate
     "I",   # isort
     "RUF", # Ruff-specific rules
     "TCH", # flake8-type-checking
     "UP",  # pyupgrade
 ]
-target-version = "py311"
+target-version = "py39"
 
 [tool.mypy]
 strict = true
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `unasyncd-0.2.1/unasyncd/cli.py` & `unasyncd-0.3.0/unasyncd/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 import time
 from pathlib import Path
 
 import rich
 import rich_click as click
 
@@ -68,14 +70,20 @@
 @click.option(
     "--add-editors-note/--no-add-editors-note",
     is_flag=True,
     default=None,
     help="Add an editors note to the generated files",
 )
 @click.option(
+    "--ruff-fix/--no-ruff-fix",
+    is_flag=True,
+    default=None,
+    help="Run 'ruff --fix' on the transformed output before writing it back",
+)
+@click.option(
     "--check/--write",
     "check_only",
     is_flag=True,
     default=None,
     help="Write changes back",
 )
 @click.option(
@@ -99,14 +107,15 @@
 @click.option("-q", "--quiet", is_flag=True, help="Suppress all console output")
 @click.argument("files", nargs=-1)
 def main(
     files: tuple[str, ...],
     cache: bool | None,
     transform_docstrings: bool | None,
     infer_type_checking_imports: bool | None,
+    ruff_fix: bool | None,
     check_only: bool,
     add_editors_note: bool | None,
     config_file: Path | None,
     force_regen: bool | None,
     verbose: bool,
     quiet: bool,
 ) -> None:
@@ -127,14 +136,15 @@
         cache=cache,
         transform_docstrings=transform_docstrings,
         add_editors_note=add_editors_note,
         files=dict(f.split(":", 1) for f in files) if files else None,
         check_only=check_only,
         force_regen=force_regen,
         infer_type_checking_imports=infer_type_checking_imports,
+        ruff_fix=ruff_fix,
     )
 
     if not config.files:
         console.print("[red]No files selected. Quitting")
     else:
         quit(
             int(
```

### Comparing `unasyncd-0.2.1/unasyncd/config.py` & `unasyncd-0.3.0/unasyncd/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     cache: bool
     extra_replacements: dict[str, dict[str, str]]
     exclude: dict[str, list[str]]
     files: dict[str, str]
     force_regen: bool
     check_only: bool
     infer_type_checking_imports: bool
+    ruff_fix: bool
 
     def key(self) -> str:
         return hashlib.sha1(msgspec.json.encode(self)).hexdigest()
 
 
 def _collect_paths(file_names: dict[str, str]) -> dict[str, str]:
     files = {}
@@ -70,8 +71,9 @@
         },
         add_editors_note=raw_config.get("add_editors_note", False),
         transform_docstrings=raw_config.get("transform_docstrings", False),
         cache=raw_config.get("cache", True),
         check_only=raw_config.get("check_only", False),
         force_regen=raw_config.get("force_regen", False),
         infer_type_checking_imports=raw_config.get("infer_type_checking_imports", True),
+        ruff_fix=raw_config.get("ruff_fix", False),
     )
```

### Comparing `unasyncd-0.2.1/unasyncd/main.py` & `unasyncd-0.3.0/unasyncd/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,15 @@
         from .transformers import TreeTransformer
 
         transformer = TreeTransformer(
             exclude=self.config.exclude.get(str(file), set()),
             transform_docstrings=self.config.transform_docstrings,
             extra_name_replacements=self.config.extra_replacements.get(str(file), {}),
             infer_type_checking_imports=self.config.infer_type_checking_imports,
+            ruff_fix=self.config.ruff_fix,
         )
 
         content = await file.get_content()
         loop = asyncio.get_running_loop()
         transformed = await loop.run_in_executor(self._executor, transformer, content)
         if self.config.add_editors_note:
             note = (
```

### Comparing `unasyncd-0.2.1/unasyncd/transformers.py` & `unasyncd-0.3.0/unasyncd/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from __future__ import annotations
 
 import dataclasses
 import itertools
 import re
+import subprocess
+import sys
 from collections import defaultdict
 from collections.abc import Iterable, Sequence
-from typing import Any, TypeVar
+from typing import Any, Callable, TypeVar, Union
 
 import libcst as cst
 import libcst.matchers as m
 from libcst import MetadataWrapper
 from libcst.metadata import QualifiedName, ScopeProvider
 from libcst.native import parse_module
 
-AnyImport = cst.ImportFrom | cst.Import
-ScopedNodeT = TypeVar("ScopedNodeT", bound=cst.Module | cst.FunctionDef | cst.ClassDef)
+AnyImport = Union[cst.ImportFrom, cst.Import]
+ScopedNodeT = TypeVar(
+    "ScopedNodeT", bound=Union[cst.Module, cst.FunctionDef, cst.ClassDef]
+)
 AnyImportT = TypeVar("AnyImportT", bound=AnyImport)
 
 
 NAME_REPLACEMENTS = {
     "__aenter__": "__enter__",
     "__aexit__": "__exit__",
     "__anext__": "__next__",
@@ -110,24 +114,24 @@
         if body:
             expr = body[0]
         else:
             return None
     else:
         expr = body
 
-    while isinstance(expr, cst.BaseSuite | cst.SimpleStatementLine):
+    while isinstance(expr, (cst.BaseSuite, cst.SimpleStatementLine)):
         if len(expr.body) == 0:
             return None
 
         expr = expr.body[0]
     if not isinstance(expr, cst.Expr):
         return None
 
     val = expr.value
-    if isinstance(val, cst.SimpleString | cst.ConcatenatedString):
+    if isinstance(val, (cst.SimpleString, cst.ConcatenatedString)):
         return val
 
     return None
 
 
 def _get_full_name_for_import_from(node: cst.ImportFrom) -> str:
     return (
@@ -149,22 +153,44 @@
 
     def __init__(
         self,
         exclude: Iterable[str] | None = None,
         transform_docstrings: bool = True,
         extra_name_replacements: dict[str, str] | None = None,
         infer_type_checking_imports: bool = True,
+        ruff_fix: bool = False,
     ) -> None:
         self.exclude = exclude
         self.transform_docstrings = transform_docstrings
         self.name_replacements = {
             **NAME_REPLACEMENTS,
             **(extra_name_replacements or {}),
         }
         self.infer_type_checking_imports = infer_type_checking_imports
+        self._post_transforms: list[Callable[[str, str, cst.Module], str]] = []
+        if ruff_fix:
+            self._post_transforms.append(self._run_ruff)
+
+    def _run_ruff(self, source: str, output: str, tree: cst.Module) -> str:
+        with subprocess.Popen(
+            [
+                sys.executable,
+                "-m",
+                "ruff",
+                "--no-cache",
+                "--fix",
+                "--quiet",
+                "-",
+            ],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            stdin=subprocess.PIPE,
+            encoding="utf-8",
+        ) as process:
+            return process.communicate(input=output)[0]
 
     def __call__(self, source: str) -> str:
         if not source:
             return ""
 
         wrapper = MetadataWrapper(parse_module(source), unsafe_skip_copy=True)
         result = wrapper.visit(
@@ -172,18 +198,17 @@
                 exclude=self.exclude,
                 name_replacements=self.name_replacements,
                 transform_docstrings=self.transform_docstrings,
                 infer_type_checking_imports=self.infer_type_checking_imports,
             )
         )
         output = result.code
+        for post_transform in self._post_transforms:
+            output = post_transform(source, output, result)
 
-        # newlines at the end can get lost so ensure we have one
-        if source[-1] == result.default_newline and not result.has_trailing_newline:
-            output += result.default_newline
         return output
 
 
 class _ReplaceAttributesMixin:
     """
     ``CSTTransformer`` mixin that replaces attributes by their fully qualified name
     """
```

### Comparing `unasyncd-0.2.1/PKG-INFO` & `unasyncd-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: unasyncd
-Version: 0.2.1
+Version: 0.3.0
 Summary: A tool to transform asynchronous Python code to synchronous Python code.
 License: MIT
 Author: Janek Nouvertné
 Author-email: j.a.nouvertne@posteo.de
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: ruff
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: libcst (>=1.0.0,<2.0.0)
-Requires-Dist: msgspec (>=0.15.1,<0.16.0)
+Requires-Dist: msgspec (>=0.16.0,<0.17.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
+Requires-Dist: ruff ; extra == "ruff"
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Unasync
 
 A tool to transform asynchronous Python code to synchronous Python code.
 
@@ -88,14 +92,15 @@
     * [As a pre-commit hook](#as-a-pre-commit-hook)
     * [Configuration](#configuration)
       * [File](#file)
       * [CLI options](#cli-options)
       * [Exclusions](#exclusions)
       * [Extending name replacements](#extending-name-replacements)
     * [Handling of imports](#handling-of-imports)
+    * [Integration with linters](#integration-with-linters)
     * [Limitations](#limitations)
     * [Disclaimer](#disclaimer)
 <!-- TOC -->
 
 ## What can be transformed?
 
 Unasyncd supports a wide variety of transformation, ranging from simple name
@@ -413,15 +418,15 @@
 
 ### As a pre-commit hook
 
 Unasyncd is available as a pre-commit hook:
 
 ```yaml
 - repo: https://github.com/provinzkraut/unasyncd
-  rev: v0.2.0
+  rev: v0.2.1
   hooks:
     - id: unasyncd
 ```
 
 ### Configuration
 
 Unasyncd can be configured via a `pyproject.toml` file, a dedicated `.unasyncd.toml`
@@ -437,14 +442,15 @@
 | `add_replacements`            | table | -       | A table of additional name replacements                                            |
 | `per_file_add_replacements`   | table | -       | A table mapping file names to tables of additional replacements                    |
 | `transform_docstrings`        | bool  | false   | Enable transformation of docstrings                                                |
 | `add_editors_note`            | bool  | false   | Add a note on top of the generated files                                           |
 | `infer_type_checking_imports` | bool  | true    | Infer if new imports should be added to an 'if TYPE_CHECKING' block                |
 | `cache`                       | bool  | true    | Cache transformation results                                                       |
 | `force_regen`                 | bool  | false   | Always regenerate files, regardless if their content has changed                   |
+| `ruff_fix`                    | bool  | false   | Run `ruff --fix` on the generated code                                             |
 
 **Example**
 
 ```toml
 [tool.unasyncd]
 files = { "async_thing.py" = "sync_thing.py", "foo.py" = "bar.py" }
 exclude = ["Something", "SomethingElse.within"]
@@ -456,26 +462,29 @@
 no_cache = false
 no_cache = false
 force_regen = false
 ```
 
 #### CLI options
 
-*Feature flags corresponding to configuration values*
+*Feature flags corresponding to configuration values. These will override the
+configuration file values*
 
 | option                             | description                                                         |
 |------------------------------------|---------------------------------------------------------------------|
 | `--cache`                          | Cache transformation results                                        |
 | `--no-cache `                      | Don't cache transformation results                                  |
 | `--transform-docstrings`           | Enable transformation of docstrings                                 |
 | `--no-transform-docstrings`        | Inverse of `--transform-docstrings`                                 |
 | `--infer-type-checking-imports`    | Infer if new imports should be added to an 'if TYPE_CHECKING' block |
 | `--no-infer-type-checking-imports` | Inverse of `infer-type-checking-imports`                            |
 | `--add-editors-note`               | Add a note on top of each generated file                            |
 | `--no-add-editors-note`            | Inverse of `--add-editors-note`                                     |
+| `--ruff-fix`                       | Run `ruff --fix` on the generated code                              |
+| `--no-ruff-fix`                    | Inverse of `--ruff-fix`                                             |
 | `--force`                          | Always regenerate files, regardless if their content has changed    |
 | `--no-force`                       | Inverse of `--force`                                                |
 | `--check`                          | Don't write changes back to files                                   |
 | `--write`                          | Inverse of `--check`                                                |
 
 
 *Additional CLI options*
@@ -545,16 +554,44 @@
    comment
 
 Unasyncd will not remove imports that have become unused as a result of the applied
 transformations. This is because tracking of usages is a complex task and best left to
 tools made specifically for this job like [ruff](https://beta.ruff.rs/docs) or
 [autoflake](https://github.com/PyCQA/autoflake).
 
-Not doing this work twice - e.g. employing a tool to automatically remove unused
-imports alongside unasyncd - can also be a significant performance improvement.
+
+### Integration with linters
+
+Using unasyncd in conjunction with linters offering autofixing behaviour can lead to an
+edit-loop, where unasyncd generates a new file which the other tool then changes in a
+non-AST-equivalent way - for example by removing an import that has become unused as a
+result of the transformation applied by unasyncd -, in turn causing unasyncd to
+regenerate the file the next time it is invoked, since the target file is no longer
+AST-equivalent to what unasyncd thinks it should be.
+
+To alleviate this, unasyncd offers a [ruff](https://beta.ruff.rs/docs) integration,
+which can automatically run `ruff --fix` on the generated code before writing it back.
+It will use the existing ruff configuration for this to ensure the fixes applied to
+adhere to the rules used throughout the project.
+
+If this option is used, the transformed code will never be altered by ruff, therefore
+breaking the cycle.
+
+This option can be enabled with the `ruff_fix = true` feature flag, or by using the
+`--ruff-fix` CLI flag.
+
+Usage of this option requires an installation of `ruff`. If not independently installed,
+it can be installed as an extra of unasyncd: `pip install unasyncd[ruff]`.
+
+**Why is only ruff supported?**
+
+Ruff was chosen for its speed, having a negligible impact on the overall performance of
+unasyncd, and because it can replace most of the common linters / tools with autofixing
+capabilities, removing the need for separate integrations.
+
 
 ### Limitations
 
 Transformations for `contextlib.AsyncContextManager`, `asyncio.TaskGroup` and
 `anyio.create_task_group` only work when they're being called in a `with` statement
 directly. This is due to the fact that unasyncd does not track assignments or support
 type inference. Support for these usages might be added in a future version.
```

