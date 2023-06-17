# Comparing `tmp/fix8-0.1.5.tar.gz` & `tmp/fix8-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fix8-0.1.5.tar", last modified: Sun Sep 18 14:35:30 2022, max compression
+gzip compressed data, was "fix8-0.1.6.tar", last modified: Sat Jun 17 18:20:28 2023, max compression
```

## Comparing `fix8-0.1.5.tar` & `fix8-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-18 14:35:30.183326 fix8-0.1.5/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2621 2022-09-18 14:35:30.183326 fix8-0.1.5/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1536 2022-09-18 14:35:21.000000 fix8-0.1.5/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-18 14:35:30.183326 fix8-0.1.5/fix8.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2621 2022-09-18 14:35:30.000000 fix8-0.1.5/fix8.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      229 2022-09-18 14:35:30.000000 fix8-0.1.5/fix8.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-09-18 14:35:30.000000 fix8-0.1.5/fix8.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       36 2022-09-18 14:35:30.000000 fix8-0.1.5/fix8.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2022-09-18 14:35:30.000000 fix8-0.1.5/fix8.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-09-18 14:35:30.000000 fix8-0.1.5/fix8.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-09-18 14:35:30.000000 fix8-0.1.5/fix8.egg-info/zip-safe
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    13932 2022-09-18 14:35:21.000000 fix8-0.1.5/fix8.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      986 2022-09-18 14:35:30.183326 fix8-0.1.5/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1493 2022-09-18 14:35:21.000000 fix8-0.1.5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-17 18:20:28.369139 fix8-0.1.6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2669 2023-06-17 18:20:28.369139 fix8-0.1.6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-17 18:20:19.000000 fix8-0.1.6/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-17 18:20:28.369139 fix8-0.1.6/fix8.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2669 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      229 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       36 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/zip-safe
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    14750 2023-06-17 18:20:19.000000 fix8-0.1.6/fix8.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      986 2023-06-17 18:20:28.369139 fix8-0.1.6/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1493 2023-06-17 18:20:19.000000 fix8-0.1.6/setup.py
```

### Comparing `fix8-0.1.5/PKG-INFO` & `fix8-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fix8
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automatic fix for Python linting issues found by Flake8
 Home-page: https://github.com/PeterJCLaw/fix8
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/PeterJCLaw/fix8/blob/master/README.md
 Project-URL: Code, https://github.com/PeterJCLaw/fix8
@@ -31,14 +31,15 @@
 Automatic fix for Python linting issues found by [Flake8](https://flake8.pycqa.org/).
 
 ## Fixes
 
 * `F401`: Unused imports are removed. (If doing so would create a blank line at
   the start of the file then the next line is also removed).
 * `C812`, `C813`, `C814`, `C815`, `C816`: Trailing commas are added
+* `FA100`: Future annotation imports are added.
 * `LBL001`: Leading blank lines are removed.
 
 ## Install
 
 ``` bash
 pip install fix8
 ```
```

### Comparing `fix8-0.1.5/README.md` & `fix8-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Automatic fix for Python linting issues found by [Flake8](https://flake8.pycqa.org/).
 
 ## Fixes
 
 * `F401`: Unused imports are removed. (If doing so would create a blank line at
   the start of the file then the next line is also removed).
 * `C812`, `C813`, `C814`, `C815`, `C816`: Trailing commas are added
+* `FA100`: Future annotation imports are added.
 * `LBL001`: Leading blank lines are removed.
 
 ## Install
 
 ``` bash
 pip install fix8
 ```
```

### Comparing `fix8-0.1.5/fix8.egg-info/PKG-INFO` & `fix8-0.1.6/fix8.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fix8
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automatic fix for Python linting issues found by Flake8
 Home-page: https://github.com/PeterJCLaw/fix8
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/PeterJCLaw/fix8/blob/master/README.md
 Project-URL: Code, https://github.com/PeterJCLaw/fix8
@@ -31,14 +31,15 @@
 Automatic fix for Python linting issues found by [Flake8](https://flake8.pycqa.org/).
 
 ## Fixes
 
 * `F401`: Unused imports are removed. (If doing so would create a blank line at
   the start of the file then the next line is also removed).
 * `C812`, `C813`, `C814`, `C815`, `C816`: Trailing commas are added
+* `FA100`: Future annotation imports are added.
 * `LBL001`: Leading blank lines are removed.
 
 ## Install
 
 ``` bash
 pip install fix8
 ```
```

### Comparing `fix8-0.1.5/fix8.py` & `fix8-0.1.6/fix8.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #!/usr/bin/env python3
 
+from __future__ import annotations
+
 import argparse
 import contextlib
 import io
 import itertools
 import re
 import sys
+import token
+import tokenize
+from collections.abc import Collection
 from pathlib import Path
 from typing import (
     Callable,
-    Dict,
     Iterable,
     Iterator,
-    List,
     NamedTuple,
-    Optional,
     Sequence,
     Tuple,
     TYPE_CHECKING,
     TypeVar,
-    Union,
 )
 
 import parso
 from flake8.main.application import (  # type: ignore[import]
     Application as Flake8,
 )
 from flake8.style_guide import Decision  # type: ignore[import]
@@ -61,19 +62,19 @@
 # a description of the edit.
 LineFixer = Callable[[CodeLine], str]
 TLineFixer = TypeVar('TLineFixer', bound=LineFixer)
 
 FileFixer = Callable[[Sequence[ErrorDetail], str], str]
 TFileFixer = TypeVar('TFileFixer', bound=FileFixer)
 
-LINE_FIXERS: Dict[str, LineFixer] = {}
-FILE_FIXERS: Dict[str, FileFixer] = {}
+LINE_FIXERS: dict[str, LineFixer] = {}
+FILE_FIXERS: dict[str, FileFixer] = {}
 
 
-def merge_overlapping_spans(spans: Sequence[Span]) -> List[Span]:
+def merge_overlapping_spans(spans: Sequence[Span]) -> list[Span]:
     if not spans:
         return []
 
     spans = sorted(spans)
 
     output_spans = [spans[0]]
 
@@ -160,18 +161,18 @@
     def get_start_pos(node_or_leaf: parso.tree.NodeOrLeaf) -> Position:
         leaf = node_or_leaf.get_first_leaf()
         if leaf.prefix.isspace():
             return leaf.get_start_pos_of_prefix()  # type: ignore[no-any-return]
         return leaf.start_pos  # type: ignore[no-any-return]
 
     def find_path(
-        node: Union[tree.ImportFrom, tree.ImportName],
-        import_name: List[str],
-        import_as_name: Optional[str],
-    ) -> List[tree.Name]:
+        node: tree.ImportFrom | tree.ImportName,
+        import_name: list[str],
+        import_as_name: str | None,
+    ) -> list[tree.Name]:
         for path, as_name in zip(node.get_paths(), node.get_defined_names()):
             if import_as_name is None:
                 # Not expecting a rename
                 if as_name not in path:
                     # But was a rename
                     continue
             else:
@@ -182,25 +183,25 @@
 
             if all(
                 name_str == name_node.get_code(include_prefix=False)
                 for name_node, name_str in zip(path, import_name)
             ):
                 return path  # type: ignore[no-any-return]
 
-        raise ValueError("Failed to find matching path for {}".format(import_name))
+        raise ValueError(f"Failed to find matching path for {import_name}")
 
     def on_same_line(a: parso.tree.NodeOrLeaf, b: parso.tree.NodeOrLeaf) -> bool:
         return a.start_pos[0] == b.start_pos[0]
 
     message_regex = re.compile(r"^'([\w\.]+)(\s+as\s+([\w\.]+))?'")
 
     def get_part_to_remove(
         detail: ErrorDetail,
-        node: Union[tree.ImportFrom, tree.ImportName],
-    ) -> Tuple[tree.Name, str]:
+        node: tree.ImportFrom | tree.ImportName,
+    ) -> tuple[tree.Name, str]:
         match = message_regex.search(detail.message)
         if match is None:
             raise ValueError("Unable to extract import name from message {!r}".format(
                 detail.message,
             ))
 
         import_name = match.group(1).split('.')
@@ -215,30 +216,30 @@
         import_name = import_name[node.level:]
 
         found_path = find_path(node, import_name, import_as_name)
         return found_path[-1], import_as_name
 
     def get_node_to_remove(
         name: tree.Name,
-        import_as_name: Optional[str],
-        node: Union[tree.ImportFrom, tree.ImportName],
-    ) -> Union[parso.tree.BaseNode, parso.tree.Leaf]:
+        import_as_name: str | None,
+        node: tree.ImportFrom | tree.ImportName,
+    ) -> parso.tree.BaseNode | parso.tree.Leaf:
         assert name.parent is not None  # placate mypy
         if name.parent.parent == node:
             # We're removing something like `bar as spam` from
             #   from foo import bar as spam, quox
             assert not import_as_name, "Expected renamed import, but didn't find it"
             return name
 
         # We're removing something like `quox` from
         #   from foo import bar as spam, quox
         assert import_as_name, "Did not expect renamed import, but found one"
         return name.parent
 
-    def is_operator(node: parso.tree.NodeOrLeaf, char: str) -> 'TypeGuard[tree.Operator]':
+    def is_operator(node: parso.tree.NodeOrLeaf, char: str) -> TypeGuard[tree.Operator]:
         return isinstance(node, tree.Operator) and node == char
 
     def operators_to_remove(
         elements: Iterable[parso.tree.NodeOrLeaf],
     ) -> Iterator[tree.Operator]:
         last_was_operator = True
         for element in elements:
@@ -249,16 +250,16 @@
             if last_was_operator:
                 yield element
 
             last_was_operator = True
 
     def get_parts_to_remove(
         line_messages: Sequence[ErrorDetail],
-        node: Union[tree.ImportFrom, tree.ImportName],
-    ) -> List[Span]:
+        node: tree.ImportFrom | tree.ImportName,
+    ) -> list[Span]:
         nodes_to_remove = set(
             get_node_to_remove(
                 *get_part_to_remove(message, node),
                 node,
             )
             for message in line_messages
         )
@@ -281,15 +282,15 @@
             nodes_to_remove.add(last_remaining_sibling)
 
         return [
             (get_start_pos(x), x.end_pos)
             for x in nodes_to_remove
         ]
 
-    spans_to_remove: List[Span] = []
+    spans_to_remove: list[Span] = []
 
     for lineno, grouped in itertools.groupby(messages, lambda x: x.line):
         line_messages = list(grouped)
 
         col = min(x.col for x in line_messages)
         node = module.get_leaf_for_position((lineno, col)).parent
 
@@ -332,19 +333,47 @@
 
         lines = before + interim + after
 
     return ''.join(lines)
 
 
 @file_fixer
+def fix_FA100(messages: Sequence[ErrorDetail], content: str) -> str:
+    tokens = tokenize.generate_tokens(io.StringIO(content).readline)
+
+    skip_types: Collection[int] = (token.COMMENT, token.NL, token.NEWLINE, token.STRING)
+    for tok in tokens:
+        if tok.type in skip_types:
+            if tok.type == token.STRING:
+                # Only the first string is a docstring
+                skip_types = tuple(x for x in skip_types if x != token.STRING)
+
+            continue
+        break
+
+    lineno, _ = tok.start
+    lineno -= 1  # convert to 0-indexed
+
+    lines = content.splitlines(keepends=True)
+
+    text = 'from __future__ import annotations\n\n'
+    if lineno > 0 and lines[lineno - 1].strip():
+        text = '\n' + text
+
+    lines.insert(lineno, text)
+
+    return ''.join(lines)
+
+
+@file_fixer
 def fix_LBL001(messages: Sequence[ErrorDetail], content: str) -> str:
     return content.lstrip('\n')
 
 
-def parse_flake8_output(flake8_output: str) -> Dict[Path, List[ErrorDetail]]:
+def parse_flake8_output(flake8_output: str) -> dict[Path, list[ErrorDetail]]:
     """
     Parse output from Flake8 formatted using FLAKE8_FORMAT into a useful form.
     """
     lines = [
         x.split(':', maxsplit=4)
         for x in sorted(flake8_output.splitlines())
     ]
@@ -357,15 +386,15 @@
             ErrorDetail(line=int(line), col=int(col), code=code, message=message)
             for (_, line, col, code, message) in messages
         )
 
     return error_details
 
 
-def run_flake8(args: List[str]) -> Dict[Path, List[ErrorDetail]]:
+def run_flake8(args: list[str]) -> dict[Path, list[ErrorDetail]]:
     # Flake8 v4 assumes stdout is a buffered output and sometimes writes
     # directly to the buffer.
     buffer = io.BytesIO()
     with contextlib.redirect_stdout(io.TextIOWrapper(buffer)) as wrapper:
         flake8 = Flake8()
         flake8.initialize(args + ['--format', FLAKE8_FORMAT])
 
@@ -385,15 +414,15 @@
         # Note: the wrapper will close our buffer when it gets closed, so need to
         # get the value while it's still alive.
         output = buffer.getvalue().decode()
 
     return parse_flake8_output(output)
 
 
-def process_errors(messages: List[ErrorDetail], content: str) -> str:
+def process_errors(messages: list[ErrorDetail], content: str) -> str:
     lines = content.splitlines()
     modified = False
 
     for message in sorted(messages, reverse=True):
         line_fixer_fn = LINE_FIXERS.get(message.code)
         if not line_fixer_fn:
             continue
@@ -428,25 +457,25 @@
             continue
 
         with filepath.open(mode='r+') as f:
             content = f.read()
             new_content = process_errors(error_details, content)
 
             if new_content != content:
-                print("Fixing {}".format(filepath))
+                print(f"Fixing {filepath}")
                 f.seek(0)
                 f.write(new_content)
                 f.truncate()
 
 
-def parse_args(argv: List[str]) -> argparse.Namespace:
+def parse_args(argv: list[str]) -> argparse.Namespace:
     parser = argparse.ArgumentParser()
     parser.add_argument('flake8_args', metavar='FLAKE8_ARG', nargs='*')
     return parser.parse_args(argv)
 
 
-def main(argv: List[str] = sys.argv[1:]) -> None:
+def main(argv: list[str] = sys.argv[1:]) -> None:
     return run(parse_args(argv))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `fix8-0.1.5/setup.cfg` & `fix8-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `fix8-0.1.5/setup.py` & `fix8-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup  # type: ignore[import]
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name='fix8',
-    version='0.1.5',
+    version='0.1.6',
     url='https://github.com/PeterJCLaw/fix8',
     project_urls={
         'Documentation': 'https://github.com/PeterJCLaw/fix8/blob/master/README.md',
         'Code': 'https://github.com/PeterJCLaw/fix8',
         'Issue tracker': 'https://github.com/PeterJCLaw/fix8/issues',
     },
     description="Automatic fix for Python linting issues found by Flake8",
```

