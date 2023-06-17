# Comparing `tmp/minijinja-0.32.0.tar.gz` & `tmp/minijinja-1.0.0.tar.gz`

## Comparing `minijinja-0.32.0.tar` & `minijinja-1.0.0.tar`

### file list

```diff
@@ -1,65 +1,62 @@
--rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 minijinja-0.32.0/local_dependencies/minijinja/Cargo.toml
--rw-r--r--   0     1001      123    10847 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/LICENSE
--rw-r--r--   0     1001      123     5593 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/README.md
--rw-r--r--   0     1001      123      598 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/doc-header.html
--rw-r--r--   0     1001      123    17588 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/ast.rs
--rw-r--r--   0     1001      123    30962 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/codegen.rs
--rw-r--r--   0     1001      123    11867 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/instructions.rs
--rw-r--r--   0     1001      123    23650 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/lexer.rs
--rw-r--r--   0     1001      123     7038 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/meta.rs
--rw-r--r--   0     1001      123      220 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/mod.rs
--rw-r--r--   0     1001      123    40725 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/parser.rs
--rw-r--r--   0     1001      123     4099 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/compiler/tokens.rs
--rw-r--r--   0     1001      123     5460 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/custom_syntax.rs
--rw-r--r--   0     1001      123     2722 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/debug.rs
--rw-r--r--   0     1001      123     7292 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/defaults.rs
--rw-r--r--   0     1001      123    23025 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/environment.rs
--rw-r--r--   0     1001      123    10801 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/error.rs
--rw-r--r--   0     1001      123     2337 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/expression.rs
--rw-r--r--   0     1001      123    44682 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/filters.rs
--rw-r--r--   0     1001      123    10177 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/functions.rs
--rw-r--r--   0     1001      123     1822 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/key/deserialize.rs
--rw-r--r--   0     1001      123     9223 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/key/mod.rs
--rw-r--r--   0     1001      123     5980 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/key/serialize.rs
--rw-r--r--   0     1001      123    10489 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/lib.rs
--rw-r--r--   0     1001      123     5689 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/macros.rs
--rw-r--r--   0     1001      123     4186 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/output.rs
--rw-r--r--   0     1001      123    10960 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/source.rs
--rw-r--r--   0     1001      123    25393 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/syntax.rs
--rw-r--r--   0     1001      123     7921 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/template.rs
--rw-r--r--   0     1001      123    13306 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/tests.rs
--rw-r--r--   0     1001      123     3809 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/testutils.rs
--rw-r--r--   0     1001      123    11730 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/utils.rs
--rw-r--r--   0     1001      123    26412 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/value/argtypes.rs
--rw-r--r--   0     1001      123     2864 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/value/deserialize.rs
--rw-r--r--   0     1001      123    44887 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/value/mod.rs
--rw-r--r--   0     1001      123    18349 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/value/object.rs
--rw-r--r--   0     1001      123    11170 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/value/ops.rs
--rw-r--r--   0     1001      123    11516 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/value/serialize.rs
--rw-r--r--   0     1001      123     1685 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/closure_object.rs
--rw-r--r--   0     1001      123     9844 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/context.rs
--rw-r--r--   0     1001      123     1862 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/fuel.rs
--rw-r--r--   0     1001      123     4433 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/loop_object.rs
--rw-r--r--   0     1001      123     5550 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/macro_object.rs
--rw-r--r--   0     1001      123    39339 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/mod.rs
--rw-r--r--   0     1001      123     6127 2023-04-20 15:36:15.000000 minijinja-0.32.0/local_dependencies/minijinja/src/vm/state.rs
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 minijinja-0.32.0/Cargo.toml
--rw-r--r--   0     1001      123       47 2023-04-20 15:36:15.000000 minijinja-0.32.0/.gitignore
--rw-r--r--   0     1001      123       45 2023-04-20 15:36:15.000000 minijinja-0.32.0/.vscode/settings.json
--rw-r--r--   0     1001      123    10847 2023-04-20 15:36:15.000000 minijinja-0.32.0/LICENSE
--rw-r--r--   0     1001      123      415 2023-04-20 15:36:15.000000 minijinja-0.32.0/Makefile
--rw-r--r--   0     1001      123     7544 2023-04-20 15:36:15.000000 minijinja-0.32.0/README.md
--rw-r--r--   0     1001      123      571 2023-04-20 15:36:15.000000 minijinja-0.32.0/hello.py
--rw-r--r--   0     1001      123     1110 2023-04-20 15:36:15.000000 minijinja-0.32.0/pyproject.toml
--rw-r--r--   0     1001      123     4284 2023-04-20 15:36:15.000000 minijinja-0.32.0/python/minijinja/__init__.py
--rw-r--r--   0     1001      123      558 2023-04-20 15:36:15.000000 minijinja-0.32.0/python/minijinja/_internal.py
--rw-r--r--   0     1001      123    20491 2023-04-20 15:36:15.000000 minijinja-0.32.0/src/environment.rs
--rw-r--r--   0     1001      123     2406 2023-04-20 15:36:15.000000 minijinja-0.32.0/src/error_support.rs
--rw-r--r--   0     1001      123      303 2023-04-20 15:36:15.000000 minijinja-0.32.0/src/lib.rs
--rw-r--r--   0     1001      123     2935 2023-04-20 15:36:15.000000 minijinja-0.32.0/src/state.rs
--rw-r--r--   0     1001      123    11218 2023-04-20 15:36:15.000000 minijinja-0.32.0/src/typeconv.rs
--rw-r--r--   0     1001      123     6798 2023-04-20 15:36:15.000000 minijinja-0.32.0/tests/test_basic.py
--rw-r--r--   0     1001      123      541 2023-04-20 15:36:15.000000 minijinja-0.32.0/tests/test_security.py
--rw-r--r--   0     1001      123     2492 2023-04-20 15:36:15.000000 minijinja-0.32.0/tests/test_state.py
--rw-r--r--   0     1001      123    66922 2023-04-20 15:37:05.000000 minijinja-0.32.0/Cargo.lock
--rw-r--r--   0        0        0     8547 1970-01-01 00:00:00.000000 minijinja-0.32.0/PKG-INFO
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 minijinja-1.0.0/local_dependencies/minijinja/Cargo.toml
+-rw-r--r--   0     1001      123    10847 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/LICENSE
+-rw-r--r--   0     1001      123     5348 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/README.md
+-rw-r--r--   0     1001      123      598 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/doc-header.html
+-rw-r--r--   0     1001      123    17406 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/compiler/ast.rs
+-rw-r--r--   0     1001      123    30568 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/compiler/codegen.rs
+-rw-r--r--   0     1001      123    12009 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/compiler/instructions.rs
+-rw-r--r--   0     1001      123    24210 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/compiler/lexer.rs
+-rw-r--r--   0     1001      123     9285 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/compiler/meta.rs
+-rw-r--r--   0     1001      123      193 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/compiler/mod.rs
+-rw-r--r--   0     1001      123    41052 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/compiler/parser.rs
+-rw-r--r--   0     1001      123     4221 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/compiler/tokens.rs
+-rw-r--r--   0     1001      123     4336 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/custom_syntax.rs
+-rw-r--r--   0     1001      123     2724 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/debug.rs
+-rw-r--r--   0     1001      123     7733 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/defaults.rs
+-rw-r--r--   0     1001      123    24349 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/environment.rs
+-rw-r--r--   0     1001      123    12780 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/error.rs
+-rw-r--r--   0     1001      123     3152 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/expression.rs
+-rw-r--r--   0     1001      123    42829 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/filters.rs
+-rw-r--r--   0     1001      123    10204 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/functions.rs
+-rw-r--r--   0     1001      123    10529 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/lib.rs
+-rw-r--r--   0     1001      123     6558 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/loader.rs
+-rw-r--r--   0     1001      123     5033 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/macros.rs
+-rw-r--r--   0     1001      123     5073 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/output.rs
+-rw-r--r--   0     1001      123    25393 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/syntax.rs
+-rw-r--r--   0     1001      123    13525 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/template.rs
+-rw-r--r--   0     1001      123    14232 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/tests.rs
+-rw-r--r--   0     1001      123    12149 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/utils.rs
+-rw-r--r--   0     1001      123    30115 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/value/argtypes.rs
+-rw-r--r--   0     1001      123     2887 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/value/deserialize.rs
+-rw-r--r--   0     1001      123     4129 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/value/keyref.rs
+-rw-r--r--   0     1001      123    50061 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/value/mod.rs
+-rw-r--r--   0     1001      123    18234 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/value/object.rs
+-rw-r--r--   0     1001      123    11000 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/value/ops.rs
+-rw-r--r--   0     1001      123    11674 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/value/serialize.rs
+-rw-r--r--   0     1001      123     1468 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/vm/closure_object.rs
+-rw-r--r--   0     1001      123    10451 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/vm/context.rs
+-rw-r--r--   0     1001      123     2236 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/vm/fuel.rs
+-rw-r--r--   0     1001      123     4433 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/vm/loop_object.rs
+-rw-r--r--   0     1001      123     5544 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/vm/macro_object.rs
+-rw-r--r--   0     1001      123    38221 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/vm/mod.rs
+-rw-r--r--   0     1001      123    12006 2023-06-16 08:49:54.000000 minijinja-1.0.0/local_dependencies/minijinja/src/vm/state.rs
+-rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 minijinja-1.0.0/Cargo.toml
+-rw-r--r--   0     1001      123       47 2023-06-16 08:49:54.000000 minijinja-1.0.0/.gitignore
+-rw-r--r--   0     1001      123       45 2023-06-16 08:49:54.000000 minijinja-1.0.0/.vscode/settings.json
+-rw-r--r--   0     1001      123    10847 2023-06-16 08:49:54.000000 minijinja-1.0.0/LICENSE
+-rw-r--r--   0     1001      123      399 2023-06-16 08:49:54.000000 minijinja-1.0.0/Makefile
+-rw-r--r--   0     1001      123     7495 2023-06-16 08:49:54.000000 minijinja-1.0.0/README.md
+-rw-r--r--   0     1001      123      571 2023-06-16 08:49:54.000000 minijinja-1.0.0/hello.py
+-rw-r--r--   0     1001      123     1145 2023-06-16 08:49:54.000000 minijinja-1.0.0/pyproject.toml
+-rw-r--r--   0     1001      123     4284 2023-06-16 08:49:54.000000 minijinja-1.0.0/python/minijinja/__init__.py
+-rw-r--r--   0     1001      123      558 2023-06-16 08:49:54.000000 minijinja-1.0.0/python/minijinja/_internal.py
+-rw-r--r--   0     1001      123    20209 2023-06-16 08:49:54.000000 minijinja-1.0.0/src/environment.rs
+-rw-r--r--   0     1001      123     2406 2023-06-16 08:49:54.000000 minijinja-1.0.0/src/error_support.rs
+-rw-r--r--   0     1001      123      303 2023-06-16 08:49:54.000000 minijinja-1.0.0/src/lib.rs
+-rw-r--r--   0     1001      123     2745 2023-06-16 08:49:54.000000 minijinja-1.0.0/src/state.rs
+-rw-r--r--   0     1001      123    10976 2023-06-16 08:49:54.000000 minijinja-1.0.0/src/typeconv.rs
+-rw-r--r--   0     1001      123     6772 2023-06-16 08:49:54.000000 minijinja-1.0.0/tests/test_basic.py
+-rw-r--r--   0     1001      123      541 2023-06-16 08:49:54.000000 minijinja-1.0.0/tests/test_security.py
+-rw-r--r--   0     1001      123     2304 2023-06-16 08:49:54.000000 minijinja-1.0.0/tests/test_state.py
+-rw-r--r--   0     1001      123    64176 2023-06-16 08:50:00.000000 minijinja-1.0.0/Cargo.lock
+-rw-r--r--   0        0        0     8497 1970-01-01 00:00:00.000000 minijinja-1.0.0/PKG-INFO
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/Cargo.toml` & `minijinja-1.0.0/local_dependencies/minijinja/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [package]
 name = "minijinja"
-version = "0.32.0"
+version = "1.0.0"
 edition = "2021"
 license = "Apache-2.0"
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 description = "a powerful template engine for Rust with minimal dependencies"
 homepage = "https://github.com/mitsuhiko/minijinja"
 repository = "https://github.com/mitsuhiko/minijinja"
 keywords = ["jinja", "jinja2", "templates"]
 readme = "README.md"
 rust-version = "1.61"
 exclude = ["tests"]
 
 [package.metadata.docs.rs]
-features = ["source", "json", "urlencode", "testutils", "custom_syntax"]
+features = ["loader", "json", "urlencode", "custom_syntax"]
 rustdoc-args = ["--cfg", "docsrs", "--html-in-header", "doc-header.html"]
 
 [features]
 default = ["builtins", "debug", "deserialization", "macros", "multi_template", "adjacent_loop_items"]
 
 # API features
 preserve_order = ["indexmap"]
 deserialization = []
 debug = []
-source = ["self_cell", "memo-map"]
-unicode = ["unicode-ident"]
-testutils = []
+loader = ["self_cell", "memo-map"]
+unicode = ["unicode-ident", "unicase"]
 custom_syntax = ["dep:aho-corasick"]
 
 # Speedups
 key_interning = []
 speedups = ["v_htmlescape"]
 
 # Engine Features
@@ -44,21 +43,18 @@
 urlencode = ["percent-encoding"]
 
 # Internal Features that should not be used
 internal_debug = []
 unstable_machinery = ["internal_debug"]
 unstable_machinery_serde = ["unstable_machinery", "serde/derive"]
 
-# Incorrectly named features to be removed in 1.x
-multi-template = ["multi_template"]
-adjacent-loop-items = ["adjacent_loop_items"]
-
 [dependencies]
 aho-corasick = { version = "1.0", default-features = false, optional = true }
 serde = "1.0.130"
 v_htmlescape = { version = "0.15.8", optional = true }
-self_cell = { version = "0.10.1", optional = true }
+self_cell = { version = "1.0.0", optional = true }
 serde_json = { version = "1.0.68", optional = true }
-percent-encoding = { version = "2.1.0", optional = true }
+percent-encoding = { version = "2.2.0", optional = true }
 indexmap = { version = "1.9.0", optional = true }
 memo-map = { version = "0.3.1", optional = true }
 unicode-ident = { version = "1.0.5", optional = true }
+unicase = { version = "2.6.0", optional = true }
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/LICENSE` & `minijinja-1.0.0/local_dependencies/minijinja/LICENSE`

 * *Files identical despite different names*

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/README.md` & `minijinja-1.0.0/local_dependencies/minijinja/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,27 +21,28 @@
 dependencies for a small problem.  Additionally it tries not to re-invent
 something but stay in line with prior art to leverage an already existing
 ecosystem of editor integrations.
 
 ```
 $ cargo tree
 minimal v0.1.0 (examples/minimal)
-└── minijinja v0.32.0 (minijinja)
+└── minijinja v1.0.0 (minijinja)
     └── serde v1.0.144
 ```
 
 You can play with MiniJinja online [in the browser playground](https://mitsuhiko.github.io/minijinja-playground/)
 powered by a WASM build of MiniJinja.
 
 **Goals:**
 
 * [Well documented](https://docs.rs/minijinja), compact API
 * Minimal dependencies, reasonable compile times and [decent runtime performance](https://github.com/mitsuhiko/minijinja/tree/main/benchmarks#comparison-results)
 * [Stay close as possible](https://github.com/mitsuhiko/minijinja/blob/main/COMPATIBILITY.md) to Jinja2
-* Support for [expression evaluation](https://docs.rs/minijinja/latest/minijinja/struct.Expression.html)
+* Support for [expression evaluation](https://docs.rs/minijinja/latest/minijinja/struct.Expression.html) which
+  allows the use [as a DSL](https://github.com/mitsuhiko/minijinja/tree/main/examples/dsl)
 * Support for all [`serde`](https://serde.rs) compatible types
 * [Well tested](https://github.com/mitsuhiko/minijinja/tree/main/minijinja/tests)
 * Support for [dynamic runtime objects](https://docs.rs/minijinja/latest/minijinja/value/trait.Object.html) with methods and dynamic attributes
 * [Descriptive errors](https://github.com/mitsuhiko/minijinja/tree/main/examples/error)
 * [Compiles to WebAssembly](https://github.com/mitsuhiko/minijinja-playground/blob/main/src/lib.rs)
 * [Works with Python](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-py)
 
@@ -68,23 +69,14 @@
 ```
 
 ## Getting Help
 
 If you are stuck with `MiniJinja`, have suggestions or need help, you can use the
 [GitHub Discussions](https://github.com/mitsuhiko/minijinja/discussions).
 
-## Minimum Rust Version
-
-MiniJinja's development version requires Rust 1.61 due to limitations with
-HRTBs in older Rust versions.
-
-MiniJinja 0.20 supports Rust versions down to 1.45.  It is possible to write
-code that is compatible with both 0.20 and newer versions of MiniJinja which
-should make it possible to defer the upgrade to later.
-
 ## Related Crates
 
 * [minijinja-autoreload](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-autoreload): provides
   auto reloading functionality of environments
 * [minijinja-contrib](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-contrib): provides
   additional utilities too specific for the core
 * [minijinja-stack-ref](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-stack-ref): provides
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/doc-header.html` & `minijinja-1.0.0/local_dependencies/minijinja/doc-header.html`

 * *Files identical despite different names*

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/compiler/ast.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/compiler/ast.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 use std::ops::Deref;
 
 #[cfg(feature = "internal_debug")]
 use std::fmt;
 
 use crate::compiler::tokens::Span;
-use crate::key::Key;
-use crate::value::{value_map_with_capacity, MapType, Value, ValueRepr};
+use crate::value::{value_map_with_capacity, KeyRef, MapType, Value, ValueRepr};
 
 /// Container for nodes with location info.
 ///
 /// This container fulfills two purposes: it adds location information
 /// to nodes, but it also ensures the nodes is heap allocated.  The
 /// latter is useful to ensure that enum variants do not cause the enum
 /// to become too large.
@@ -496,15 +495,15 @@
         if !self.pairs.iter().all(|x| matches!(x.1, Expr::Const(_))) {
             return None;
         }
 
         let mut rv = value_map_with_capacity(self.pairs.len());
         for (key, value) in &self.pairs {
             if let Expr::Const(value) = value {
-                rv.insert(Key::make_string_key(key), value.value.clone());
+                rv.insert(KeyRef::Value(Value::from(*key)), value.value.clone());
             }
         }
 
         Some(Value(ValueRepr::Map(rv.into(), MapType::Kwargs)))
     }
 }
 
@@ -523,21 +522,15 @@
         {
             return None;
         }
 
         let mut rv = value_map_with_capacity(self.keys.len());
         for (key, value) in self.keys.iter().zip(self.values.iter()) {
             if let (Expr::Const(maybe_key), Expr::Const(value)) = (key, value) {
-                rv.insert(
-                    match maybe_key.value.clone().try_into_key() {
-                        Ok(key) => key,
-                        Err(_) => return None,
-                    },
-                    value.value.clone(),
-                );
+                rv.insert(KeyRef::Value(maybe_key.value.clone()), value.value.clone());
             }
         }
 
         Some(Value(ValueRepr::Map(rv.into(), MapType::Normal)))
     }
 }
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/compiler/codegen.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/compiler/codegen.rs`

 * *Files 1% similar despite different names*

```diff
@@ -44,32 +44,28 @@
     blocks: BTreeMap<&'source str, Instructions<'source>>,
     pending_block: Vec<PendingBlock>,
     current_line: u32,
     span_stack: Vec<Span>,
     filter_local_ids: BTreeMap<&'source str, LocalId>,
     test_local_ids: BTreeMap<&'source str, LocalId>,
     raw_template_bytes: usize,
-    #[cfg(feature = "multi_template")]
-    has_extends: bool,
 }
 
 impl<'source> CodeGenerator<'source> {
     /// Creates a new code generator.
     pub fn new(file: &'source str, source: &'source str) -> CodeGenerator<'source> {
         CodeGenerator {
             instructions: Instructions::new(file, source),
             blocks: BTreeMap::new(),
             pending_block: Vec::with_capacity(32),
             current_line: 0,
             span_stack: Vec::with_capacity(32),
             filter_local_ids: BTreeMap::new(),
             test_local_ids: BTreeMap::new(),
             raw_template_bytes: 0,
-            #[cfg(feature = "multi_template")]
-            has_extends: false,
         }
     }
 
     /// Sets the current location's line.
     pub fn set_line(&mut self, lineno: u32) {
         self.current_line = lineno;
     }
@@ -233,20 +229,14 @@
     pub fn compile_stmt(&mut self, stmt: &ast::Stmt<'source>) {
         match stmt {
             ast::Stmt::Template(t) => {
                 self.set_line_from_span(t.span());
                 for node in &t.children {
                     self.compile_stmt(node);
                 }
-                #[cfg(feature = "multi_template")]
-                {
-                    if self.has_extends {
-                        self.add(Instruction::RenderParent);
-                    }
-                }
             }
             ast::Stmt::EmitExpr(expr) => {
                 self.compile_emit_expr(expr);
             }
             ast::Stmt::EmitRaw(raw) => {
                 self.set_line_from_span(raw.span());
                 self.add(Instruction::EmitRaw(raw.raw));
@@ -337,15 +327,14 @@
                 self.add(Instruction::EndCapture);
             }
             #[cfg(feature = "multi_template")]
             ast::Stmt::Extends(extends) => {
                 self.set_line_from_span(extends.span());
                 self.compile_expr(&extends.name);
                 self.add_with_span(Instruction::LoadBlocks, extends.span());
-                self.has_extends = true;
             }
             #[cfg(feature = "multi_template")]
             ast::Stmt::Include(include) => {
                 self.set_line_from_span(include.span());
                 self.compile_expr(&include.name);
                 self.add_with_span(Instruction::Include(include.ignore_missing), include.span());
             }
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/compiler/instructions.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/compiler/instructions.rs`

 * *Files 3% similar despite different names*

```diff
@@ -199,18 +199,14 @@
     #[cfg(feature = "multi_template")]
     CallBlock(&'source str),
 
     /// Loads block from a template with name on stack ("extends")
     #[cfg(feature = "multi_template")]
     LoadBlocks,
 
-    /// Renders the parent template
-    #[cfg(feature = "multi_template")]
-    RenderParent,
-
     /// Includes another template.
     #[cfg(feature = "multi_template")]
     Include(bool),
 
     /// Builds a module
     #[cfg(feature = "multi_template")]
     ExportLocals,
@@ -255,14 +251,23 @@
     line_infos: Vec<LineInfo>,
     #[cfg(feature = "debug")]
     span_infos: Vec<SpanInfo>,
     name: &'source str,
     source: &'source str,
 }
 
+pub(crate) static EMPTY_INSTRUCTIONS: Instructions<'static> = Instructions {
+    instructions: Vec::new(),
+    line_infos: Vec::new(),
+    #[cfg(feature = "debug")]
+    span_infos: Vec::new(),
+    name: "<unknown>",
+    source: "",
+};
+
 impl<'source> Instructions<'source> {
     /// Creates a new instructions object.
     pub fn new(name: &'source str, source: &'source str) -> Instructions<'source> {
         Instructions {
             instructions: Vec::with_capacity(128),
             line_infos: Vec::with_capacity(128),
             #[cfg(feature = "debug")]
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/compiler/lexer.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/compiler/lexer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 use crate::compiler::tokens::{Span, Token};
 use crate::error::{Error, ErrorKind};
 use crate::utils::{memchr, memstr, unescape};
 
-#[cfg(test)]
-use similar_asserts::assert_eq;
-
 #[cfg(feature = "custom_syntax")]
 pub use crate::custom_syntax::SyntaxConfig;
 
 /// Non configurable syntax config
 #[cfg(not(feature = "custom_syntax"))]
-#[derive(Debug, Copy, Clone, Default)]
+#[derive(Debug, Clone, Default)]
 pub struct SyntaxConfig;
 
 enum LexerState {
     Template,
     InVariable,
     InBlock,
 }
@@ -29,14 +26,15 @@
 
 struct TokenizerState<'s> {
     stack: Vec<LexerState>,
     rest: &'s str,
     failed: bool,
     current_line: u32,
     current_col: u32,
+    current_offset: u32,
 }
 
 fn find_start_marker_memchr(a: &str) -> Option<(usize, bool)> {
     let bytes = a.as_bytes();
     let mut offset = 0;
     loop {
         let idx = match memchr(&bytes[offset..], b'{') {
@@ -76,15 +74,15 @@
     find_start_marker_memchr(a)
 }
 
 fn match_start_marker(rest: &str, syntax_config: &SyntaxConfig) -> Option<(StartMarker, usize)> {
     #[cfg(not(feature = "custom_syntax"))]
     {
         let _ = syntax_config;
-        return match_start_marker_default(rest);
+        match_start_marker_default(rest)
     }
 
     #[cfg(feature = "custom_syntax")]
     {
         if syntax_config.aho_corasick.is_none() {
             return match_start_marker_default(rest);
         }
@@ -186,30 +184,33 @@
                 '\n' => {
                     self.current_line += 1;
                     self.current_col = 0;
                 }
                 _ => self.current_col += 1,
             }
         }
+        self.current_offset += bytes as u32;
         self.rest = new_rest;
         skipped
     }
 
     #[inline(always)]
-    fn loc(&self) -> (u32, u32) {
-        (self.current_line, self.current_col)
+    fn loc(&self) -> (u32, u32, u32) {
+        (self.current_line, self.current_col, self.current_offset)
     }
 
-    fn span(&self, start: (u32, u32)) -> Span {
-        let (start_line, start_col) = start;
+    fn span(&self, start: (u32, u32, u32)) -> Span {
+        let (start_line, start_col, start_offset) = start;
         Span {
             start_line,
             start_col,
+            start_offset,
             end_line: self.current_line,
             end_col: self.current_col,
+            end_offset: self.current_offset,
         }
     }
 
     fn syntax_error(&mut self, msg: &'static str) -> Error {
         self.failed = true;
         Error::new(ErrorKind::SyntaxError, msg)
     }
@@ -333,14 +334,15 @@
             LexerState::InVariable
         } else {
             LexerState::Template
         }],
         failed: false,
         current_line: 1,
         current_col: 0,
+        current_offset: 0,
     };
     let mut trim_leading_whitespace = false;
 
     std::iter::from_fn(move || {
         let (variable_end, block_start, block_end, comment_end) = {
             #[cfg(feature = "custom_syntax")]
             {
@@ -564,97 +566,104 @@
                 }
                 None => panic!("empty lexer state"),
             }
         }
     })
 }
 
-#[test]
-fn test_find_marker() {
-    let syntax = SyntaxConfig::default();
-    assert!(find_start_marker("{", &syntax).is_none());
-    assert!(find_start_marker("foo", &syntax).is_none());
-    assert!(find_start_marker("foo {", &syntax).is_none());
-    assert_eq!(find_start_marker("foo {{", &syntax), Some((4, false)));
-    assert_eq!(find_start_marker("foo {{-", &syntax), Some((4, true)));
-}
+#[cfg(test)]
+mod tests {
+    use super::*;
 
-#[test]
-#[cfg(feature = "custom_syntax")]
-fn test_find_marker_custom_syntax() {
-    use crate::Syntax;
+    use similar_asserts::assert_eq;
 
-    let syntax = Syntax {
-        block_start: "%{".into(),
-        block_end: "}%".into(),
-        variable_start: "[[".into(),
-        variable_end: "]]".into(),
-        comment_start: "/*".into(),
-        comment_end: "*/".into(),
-    };
+    #[test]
+    fn test_find_marker() {
+        let syntax = SyntaxConfig::default();
+        assert!(find_start_marker("{", &syntax).is_none());
+        assert!(find_start_marker("foo", &syntax).is_none());
+        assert!(find_start_marker("foo {", &syntax).is_none());
+        assert_eq!(find_start_marker("foo {{", &syntax), Some((4, false)));
+        assert_eq!(find_start_marker("foo {{-", &syntax), Some((4, true)));
+    }
 
-    let syntax_config = syntax.compile().expect("failed to create syntax config");
+    #[test]
+    #[cfg(feature = "custom_syntax")]
+    fn test_find_marker_custom_syntax() {
+        use crate::Syntax;
 
-    assert_eq!(find_start_marker("%{", &syntax_config), Some((0, false)));
-    assert!(find_start_marker("/", &syntax_config).is_none());
-    assert!(find_start_marker("foo [", &syntax_config).is_none());
-    assert_eq!(
-        find_start_marker("foo /*", &syntax_config),
-        Some((4, false))
-    );
-    assert_eq!(
-        find_start_marker("foo [[-", &syntax_config),
-        Some((4, true))
-    );
-}
-
-#[test]
-fn test_is_basic_tag() {
-    assert_eq!(skip_basic_tag(" raw %}", "raw", "%}"), Some((7, false)));
-    assert_eq!(skip_basic_tag(" raw %}", "endraw", "%}"), None);
-    assert_eq!(skip_basic_tag("  raw  %}", "raw", "%}"), Some((9, false)));
-    assert_eq!(skip_basic_tag("-  raw  -%}", "raw", "%}"), Some((11, true)));
-}
-
-#[test]
-fn test_basic_identifiers() {
-    fn assert_ident(s: &str) {
-        match tokenize(s, true, Default::default()).next() {
-            Some(Ok((Token::Ident(ident), _))) if ident == s => {}
-            _ => panic!("did not get a matching token result: {s:?}"),
-        }
-    }
+        let syntax = Syntax {
+            block_start: "%{".into(),
+            block_end: "}%".into(),
+            variable_start: "[[".into(),
+            variable_end: "]]".into(),
+            comment_start: "/*".into(),
+            comment_end: "*/".into(),
+        };
+
+        let syntax_config = syntax.compile().expect("failed to create syntax config");
 
-    fn assert_not_ident(s: &str) {
-        let res = tokenize(s, true, Default::default()).collect::<Result<Vec<_>, _>>();
-        if let Ok(tokens) = res {
-            if let &[(Token::Ident(_), _)] = &tokens[..] {
-                panic!("got a single ident for {s:?}")
+        assert_eq!(find_start_marker("%{", &syntax_config), Some((0, false)));
+        assert!(find_start_marker("/", &syntax_config).is_none());
+        assert!(find_start_marker("foo [", &syntax_config).is_none());
+        assert_eq!(
+            find_start_marker("foo /*", &syntax_config),
+            Some((4, false))
+        );
+        assert_eq!(
+            find_start_marker("foo [[-", &syntax_config),
+            Some((4, true))
+        );
+    }
+
+    #[test]
+    fn test_is_basic_tag() {
+        assert_eq!(skip_basic_tag(" raw %}", "raw", "%}"), Some((7, false)));
+        assert_eq!(skip_basic_tag(" raw %}", "endraw", "%}"), None);
+        assert_eq!(skip_basic_tag("  raw  %}", "raw", "%}"), Some((9, false)));
+        assert_eq!(skip_basic_tag("-  raw  -%}", "raw", "%}"), Some((11, true)));
+    }
+
+    #[test]
+    fn test_basic_identifiers() {
+        fn assert_ident(s: &str) {
+            match tokenize(s, true, Default::default()).next() {
+                Some(Ok((Token::Ident(ident), _))) if ident == s => {}
+                _ => panic!("did not get a matching token result: {s:?}"),
             }
         }
-    }
 
-    assert_ident("foo_bar_baz");
-    assert_ident("_foo_bar_baz");
-    assert_ident("_42world");
-    assert_ident("_world42");
-    assert_ident("world42");
-    assert_not_ident("42world");
+        fn assert_not_ident(s: &str) {
+            let res = tokenize(s, true, Default::default()).collect::<Result<Vec<_>, _>>();
+            if let Ok(tokens) = res {
+                if let &[(Token::Ident(_), _)] = &tokens[..] {
+                    panic!("got a single ident for {s:?}")
+                }
+            }
+        }
 
-    #[cfg(feature = "unicode")]
-    {
-        assert_ident("foo");
-        assert_ident("föö");
-        assert_ident("き");
-        assert_ident("_");
-        assert_not_ident("1a");
-        assert_not_ident("a-");
-        assert_not_ident("🐍a");
-        assert_not_ident("a🐍🐍");
-        assert_ident("ᢅ");
-        assert_ident("ᢆ");
-        assert_ident("℘");
-        assert_ident("℮");
-        assert_not_ident("·");
-        assert_ident("a·");
+        assert_ident("foo_bar_baz");
+        assert_ident("_foo_bar_baz");
+        assert_ident("_42world");
+        assert_ident("_world42");
+        assert_ident("world42");
+        assert_not_ident("42world");
+
+        #[cfg(feature = "unicode")]
+        {
+            assert_ident("foo");
+            assert_ident("föö");
+            assert_ident("き");
+            assert_ident("_");
+            assert_not_ident("1a");
+            assert_not_ident("a-");
+            assert_not_ident("🐍a");
+            assert_not_ident("a🐍🐍");
+            assert_ident("ᢅ");
+            assert_ident("ᢆ");
+            assert_ident("℘");
+            assert_ident("℮");
+            assert_not_ident("·");
+            assert_ident("a·");
+        }
     }
 }
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/compiler/parser.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/compiler/parser.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,22 @@
+use std::borrow::Cow;
 use std::collections::BTreeSet;
 use std::fmt;
 
 use crate::compiler::ast::{self, Spanned};
 use crate::compiler::lexer::{tokenize, SyntaxConfig};
 use crate::compiler::tokens::{Span, Token};
 use crate::error::{Error, ErrorKind};
 use crate::value::Value;
 
 const MAX_RECURSION: usize = 150;
 const RESERVED_NAMES: [&str; 8] = [
     "true", "True", "false", "False", "none", "None", "loop", "self",
 ];
 
-macro_rules! syntax_error {
-    ($msg:expr) => {{
-        return Err(Error::new(ErrorKind::SyntaxError, $msg));
-    }};
-    ($msg:expr, $($tt:tt)*) => {{
-        return Err(Error::new(ErrorKind::SyntaxError, format!($msg, $($tt)*)));
-    }};
-}
-
 fn unexpected<D: fmt::Display>(unexpected: D, expected: &str) -> Error {
     Error::new(
         ErrorKind::SyntaxError,
         format!("unexpected {unexpected}, expected {expected}"),
     )
 }
 
@@ -32,14 +24,27 @@
     unexpected("end of input", expected)
 }
 
 fn make_const(value: Value, span: Span) -> ast::Expr<'static> {
     ast::Expr::Const(Spanned::new(ast::Const { value }, span))
 }
 
+fn syntax_error(msg: Cow<'static, str>) -> Error {
+    Error::new(ErrorKind::SyntaxError, msg)
+}
+
+macro_rules! syntax_error {
+    ($msg:expr) => {{
+        return Err(syntax_error(Cow::Borrowed($msg)));
+    }};
+    ($msg:expr, $($tt:tt)*) => {{
+        return Err(syntax_error(Cow::Owned(format!($msg, $($tt)*))));
+    }};
+}
+
 macro_rules! expect_token {
     ($parser:expr, $expectation:expr) => {{
         match ok!($parser.stream.next()) {
             Some(rv) => rv,
             None => return Err(unexpected_eof($expectation)),
         }
     }};
@@ -67,21 +72,21 @@
             _ => false,
         }
     };
 }
 
 macro_rules! skip_token {
     ($p:expr, $match:pat) => {
-        if matches_token!($p, $match) {
-            // we can ignore the error as matches_token! would already
-            // have created it.
-            let _ = $p.stream.next();
-            true
-        } else {
-            false
+        match $p.stream.current() {
+            Err(err) => return Err(err),
+            Ok(Some(($match, _))) => {
+                let _ = $p.stream.next();
+                true
+            }
+            _ => false,
         }
     };
 }
 
 enum SetParseResult<'a> {
     Set(ast::Set<'a>),
     SetBlock(ast::SetBlock<'a>),
@@ -125,14 +130,15 @@
     }
 
     /// Expands the span
     #[inline(always)]
     pub fn expand_span(&self, mut span: Span) -> Span {
         span.end_line = self.last_span.end_line;
         span.end_col = self.last_span.end_col;
+        span.end_offset = self.last_span.end_offset;
         span
     }
 
     /// Returns the current span.
     #[inline(always)]
     pub fn current_span(&self) -> Span {
         if let Some(Ok((_, span))) = self.current {
@@ -200,18 +206,17 @@
     };
 }
 
 macro_rules! with_recursion_guard {
     ($parser:expr, $expr:expr) => {{
         $parser.depth += 1;
         if $parser.depth > MAX_RECURSION {
-            return Err(Error::new(
-                ErrorKind::SyntaxError,
+            return Err(syntax_error(Cow::Borrowed(
                 "template exceeds maximum recursion limits",
-            ));
+            )));
         }
         let rv = $expr;
         $parser.depth -= 1;
         rv
     }};
 }
 
@@ -377,15 +382,15 @@
                     expect_token!(self, Token::BracketClose, "`]`");
 
                     if !is_slice {
                         expr = ast::Expr::GetItem(Spanned::new(
                             ast::GetItem {
                                 expr,
                                 subscript_expr: ok!(start.ok_or_else(|| {
-                                    Error::new(ErrorKind::SyntaxError, "empty subscript")
+                                    syntax_error(Cow::Borrowed("empty subscript"))
                                 })),
                             },
                             self.stream.expand_span(span),
                         ));
                     } else {
                         expr = ast::Expr::Slice(Spanned::new(
                             ast::Slice {
@@ -487,18 +492,17 @@
                 ast::Expr::Var(ref var) if skip_token!(self, Token::Assign) => {
                     if first_span.is_none() {
                         first_span = Some(var.span());
                     }
                     kwargs.push((var.id, ok!(self.parse_expr_noif())));
                 }
                 _ if !kwargs.is_empty() => {
-                    return Err(Error::new(
-                        ErrorKind::SyntaxError,
+                    return Err(syntax_error(Cow::Borrowed(
                         "non-keyword arg after keyword arg",
-                    ));
+                    )));
                 }
                 _ => {
                     args.push(expr);
                 }
             }
         }
 
@@ -632,45 +636,45 @@
 
         macro_rules! respan {
             ($expr:expr) => {
                 Spanned::new($expr, self.stream.expand_span(span))
             };
         }
 
-        Ok(match token {
-            Token::Ident("for") => ast::Stmt::ForLoop(respan!(ok!(self.parse_for_stmt()))),
-            Token::Ident("if") => ast::Stmt::IfCond(respan!(ok!(self.parse_if_cond()))),
-            Token::Ident("with") => ast::Stmt::WithBlock(respan!(ok!(self.parse_with_block()))),
-            Token::Ident("set") => match ok!(self.parse_set()) {
+        let ident = match token {
+            Token::Ident(ident) => ident,
+            token => syntax_error!("unknown {}, expected statement", token),
+        };
+
+        Ok(match ident {
+            "for" => ast::Stmt::ForLoop(respan!(ok!(self.parse_for_stmt()))),
+            "if" => ast::Stmt::IfCond(respan!(ok!(self.parse_if_cond()))),
+            "with" => ast::Stmt::WithBlock(respan!(ok!(self.parse_with_block()))),
+            "set" => match ok!(self.parse_set()) {
                 SetParseResult::Set(rv) => ast::Stmt::Set(respan!(rv)),
                 SetParseResult::SetBlock(rv) => ast::Stmt::SetBlock(respan!(rv)),
             },
-            Token::Ident("autoescape") => {
-                ast::Stmt::AutoEscape(respan!(ok!(self.parse_auto_escape())))
-            }
-            Token::Ident("filter") => {
-                ast::Stmt::FilterBlock(respan!(ok!(self.parse_filter_block())))
-            }
+            "autoescape" => ast::Stmt::AutoEscape(respan!(ok!(self.parse_auto_escape()))),
+            "filter" => ast::Stmt::FilterBlock(respan!(ok!(self.parse_filter_block()))),
             #[cfg(feature = "multi_template")]
-            Token::Ident("block") => ast::Stmt::Block(respan!(ok!(self.parse_block()))),
+            "block" => ast::Stmt::Block(respan!(ok!(self.parse_block()))),
             #[cfg(feature = "multi_template")]
-            Token::Ident("extends") => ast::Stmt::Extends(respan!(ok!(self.parse_extends()))),
+            "extends" => ast::Stmt::Extends(respan!(ok!(self.parse_extends()))),
             #[cfg(feature = "multi_template")]
-            Token::Ident("include") => ast::Stmt::Include(respan!(ok!(self.parse_include()))),
+            "include" => ast::Stmt::Include(respan!(ok!(self.parse_include()))),
             #[cfg(feature = "multi_template")]
-            Token::Ident("import") => ast::Stmt::Import(respan!(ok!(self.parse_import()))),
+            "import" => ast::Stmt::Import(respan!(ok!(self.parse_import()))),
             #[cfg(feature = "multi_template")]
-            Token::Ident("from") => ast::Stmt::FromImport(respan!(ok!(self.parse_from_import()))),
+            "from" => ast::Stmt::FromImport(respan!(ok!(self.parse_from_import()))),
             #[cfg(feature = "macros")]
-            Token::Ident("macro") => ast::Stmt::Macro(respan!(ok!(self.parse_macro()))),
+            "macro" => ast::Stmt::Macro(respan!(ok!(self.parse_macro()))),
             #[cfg(feature = "macros")]
-            Token::Ident("call") => ast::Stmt::CallBlock(respan!(ok!(self.parse_call_block()))),
-            Token::Ident("do") => ast::Stmt::Do(respan!(ok!(self.parse_do()))),
-            Token::Ident(name) => syntax_error!("unknown statement {}", name),
-            token => syntax_error!("unknown {}, expected statement", token),
+            "call" => ast::Stmt::CallBlock(respan!(ok!(self.parse_call_block()))),
+            "do" => ast::Stmt::Do(respan!(ok!(self.parse_do()))),
+            name => syntax_error!("unknown statement {}", name),
         })
     }
 
     fn parse_assign_name(&mut self) -> Result<ast::Expr<'a>, Error> {
         let (id, span) = expect_token!(self, Token::Ident(name) => name, "identifier");
         if RESERVED_NAMES.contains(&id) {
             syntax_error!("cannot assign to reserved variable name {}", id);
@@ -881,15 +885,15 @@
                     expr: filter,
                     args,
                 },
                 self.stream.expand_span(span),
             )));
         }
 
-        filter.ok_or_else(|| Error::new(ErrorKind::SyntaxError, "expected a filter"))
+        filter.ok_or_else(|| syntax_error(Cow::Borrowed("expected a filter")))
     }
 
     fn parse_filter_block(&mut self) -> Result<ast::FilterBlock<'a>, Error> {
         let filter = ok!(self.parse_filter_chain());
         expect_token!(self, Token::BlockEnd, "end of block");
         let body = ok!(self.subparse(&|tok| matches!(tok, Token::Ident("endfilter"))));
         ok!(self.stream.next());
@@ -901,16 +905,26 @@
         let name = ok!(self.parse_expr());
         Ok(ast::Extends { name })
     }
 
     #[cfg(feature = "multi_template")]
     fn parse_include(&mut self) -> Result<ast::Include<'a>, Error> {
         let name = ok!(self.parse_expr());
+
+        // with/without context is without meaning in MiniJinja, but for syntax
+        // compatibility it's supported.
+        if skip_token!(self, Token::Ident("without" | "with")) {
+            expect_token!(self, Token::Ident("context"), "missing keyword");
+        }
+
         let ignore_missing = if skip_token!(self, Token::Ident("ignore")) {
             expect_token!(self, Token::Ident("missing"), "missing keyword");
+            if skip_token!(self, Token::Ident("without" | "with")) {
+                expect_token!(self, Token::Ident("context"), "missing keyword");
+            }
             true
         } else {
             false
         };
         Ok(ast::Include {
             name,
             ignore_missing,
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/compiler/tokens.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/compiler/tokens.rs`

 * *Files 21% similar despite different names*

```diff
@@ -81,61 +81,63 @@
     /// Close Brace
     BraceClose,
 }
 
 impl<'a> fmt::Display for Token<'a> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         match self {
-            Token::TemplateData(_) => write!(f, "template-data"),
-            Token::VariableStart => write!(f, "start of variable block"),
-            Token::VariableEnd => write!(f, "end of variable block"),
-            Token::BlockStart => write!(f, "start of block"),
-            Token::BlockEnd => write!(f, "end of block"),
-            Token::Ident(_) => write!(f, "identifier"),
-            Token::Str(_) | Token::String(_) => write!(f, "string"),
-            Token::Int(_) => write!(f, "integer"),
-            Token::Float(_) => write!(f, "float"),
-            Token::Plus => write!(f, "`+`"),
-            Token::Minus => write!(f, "`-`"),
-            Token::Mul => write!(f, "`*`"),
-            Token::Div => write!(f, "`/`"),
-            Token::FloorDiv => write!(f, "`//`"),
-            Token::Pow => write!(f, "`**`"),
-            Token::Mod => write!(f, "`%`"),
-            Token::Bang => write!(f, "`!`"),
-            Token::Dot => write!(f, "`.`"),
-            Token::Comma => write!(f, "`,`"),
-            Token::Colon => write!(f, "`:`"),
-            Token::Tilde => write!(f, "`~`"),
-            Token::Assign => write!(f, "`=`"),
-            Token::Pipe => write!(f, "`|`"),
-            Token::Eq => write!(f, "`==`"),
-            Token::Ne => write!(f, "`!=`"),
-            Token::Gt => write!(f, "`>`"),
-            Token::Gte => write!(f, "`>=`"),
-            Token::Lt => write!(f, "`<`"),
-            Token::Lte => write!(f, "`<=`"),
-            Token::BracketOpen => write!(f, "`[`"),
-            Token::BracketClose => write!(f, "`]`"),
-            Token::ParenOpen => write!(f, "`(`"),
-            Token::ParenClose => write!(f, "`)`"),
-            Token::BraceOpen => write!(f, "`{{`"),
-            Token::BraceClose => write!(f, "`}}`"),
+            Token::TemplateData(_) => f.write_str("template-data"),
+            Token::VariableStart => f.write_str("start of variable block"),
+            Token::VariableEnd => f.write_str("end of variable block"),
+            Token::BlockStart => f.write_str("start of block"),
+            Token::BlockEnd => f.write_str("end of block"),
+            Token::Ident(_) => f.write_str("identifier"),
+            Token::Str(_) | Token::String(_) => f.write_str("string"),
+            Token::Int(_) => f.write_str("integer"),
+            Token::Float(_) => f.write_str("float"),
+            Token::Plus => f.write_str("`+`"),
+            Token::Minus => f.write_str("`-`"),
+            Token::Mul => f.write_str("`*`"),
+            Token::Div => f.write_str("`/`"),
+            Token::FloorDiv => f.write_str("`//`"),
+            Token::Pow => f.write_str("`**`"),
+            Token::Mod => f.write_str("`%`"),
+            Token::Bang => f.write_str("`!`"),
+            Token::Dot => f.write_str("`.`"),
+            Token::Comma => f.write_str("`,`"),
+            Token::Colon => f.write_str("`:`"),
+            Token::Tilde => f.write_str("`~`"),
+            Token::Assign => f.write_str("`=`"),
+            Token::Pipe => f.write_str("`|`"),
+            Token::Eq => f.write_str("`==`"),
+            Token::Ne => f.write_str("`!=`"),
+            Token::Gt => f.write_str("`>`"),
+            Token::Gte => f.write_str("`>=`"),
+            Token::Lt => f.write_str("`<`"),
+            Token::Lte => f.write_str("`<=`"),
+            Token::BracketOpen => f.write_str("`[`"),
+            Token::BracketClose => f.write_str("`]`"),
+            Token::ParenOpen => f.write_str("`(`"),
+            Token::ParenClose => f.write_str("`)`"),
+            Token::BraceOpen => f.write_str("`{{`"),
+            Token::BraceClose => f.write_str("`}}`"),
         }
     }
 }
 
 /// Token span information
 #[derive(Clone, Copy, Default, PartialEq, Eq)]
 #[cfg_attr(feature = "unstable_machinery_serde", derive(serde::Serialize))]
 pub struct Span {
     pub start_line: u32,
     pub start_col: u32,
+    pub start_offset: u32,
     pub end_line: u32,
     pub end_col: u32,
+    pub end_offset: u32,
 }
 
 impl fmt::Debug for Span {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         write!(
             f,
             " @ {}:{}-{}:{}",
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/debug.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/debug.rs`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 }
 
 struct VarPrinter<'x>(&'x BTreeMap<String, Value>);
 
 impl<'x> fmt::Debug for VarPrinter<'x> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         if self.0.is_empty() {
-            return write!(f, "No referenced variables");
+            return f.write_str("No referenced variables");
         }
         let mut m = f.debug_struct("Referenced variables:");
         let mut vars = self.0.iter().collect::<Vec<_>>();
         vars.sort_by_key(|x| x.0);
         for (key, value) in vars {
             m.field(key, value);
         }
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/defaults.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/defaults.rs`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 }
 
 /// The default logic for auto escaping based on file extension.
 ///
 /// * [`Html`](AutoEscape::Html): `.html`, `.htm`, `.xml`
 #[cfg_attr(
     feature = "json",
-    doc = r" * [`Json`](AutoEscape::Json): `.json`, `.js`, `.yml`"
+    doc = r" * [`Json`](AutoEscape::Json): `.json`, `.json5`, `.js`, `.yaml`, `.yml`"
 )]
 /// * [`None`](AutoEscape::None): _all others_
 pub fn default_auto_escape_callback(name: &str) -> AutoEscape {
     match name.rsplit('.').next() {
         Some("html" | "htm" | "xml") => AutoEscape::Html,
         #[cfg(feature = "json")]
-        Some("json" | "js" | "yaml" | "yml") => AutoEscape::Json,
+        Some("json" | "json5" | "js" | "yaml" | "yml") => AutoEscape::Json,
         _ => AutoEscape::None,
     }
 }
 
 /// The default formatter.
 ///
 /// This formatter takes a value and directly writes it into the output format
@@ -85,14 +85,16 @@
         rv.insert("slice".into(), BoxedFilter::new(filters::slice));
         rv.insert("indent".into(), BoxedFilter::new(filters::indent));
         rv.insert("select".into(), BoxedFilter::new(filters::select));
         rv.insert("reject".into(), BoxedFilter::new(filters::reject));
         rv.insert("selectattr".into(), BoxedFilter::new(filters::selectattr));
         rv.insert("rejectattr".into(), BoxedFilter::new(filters::rejectattr));
         rv.insert("map".into(), BoxedFilter::new(filters::map));
+        rv.insert("unique".into(), BoxedFilter::new(filters::unique));
+        rv.insert("pprint".into(), BoxedFilter::new(filters::pprint));
 
         #[cfg(feature = "json")]
         {
             rv.insert("tojson".into(), BoxedFilter::new(filters::tojson));
         }
         #[cfg(feature = "urlencode")]
         {
@@ -144,14 +146,18 @@
         rv.insert("gt".into(), is_gt.clone());
         rv.insert("greaterthan".into(), is_gt.clone());
         rv.insert(">".into(), is_gt);
         let is_ge = BoxedTest::new(tests::is_ge);
         rv.insert("ge".into(), is_ge.clone());
         rv.insert(">=".into(), is_ge);
         rv.insert("in".into(), BoxedTest::new(tests::is_in));
+        rv.insert("true".into(), BoxedTest::new(tests::is_true));
+        rv.insert("false".into(), BoxedTest::new(tests::is_false));
+        rv.insert("filter".into(), BoxedTest::new(tests::is_filter));
+        rv.insert("test".into(), BoxedTest::new(tests::is_test));
     }
     rv
 }
 
 pub(crate) fn get_globals() -> BTreeMap<Cow<'static, str>, Value> {
     #[allow(unused_mut)]
     let mut rv = BTreeMap::new();
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/environment.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/environment.rs`

 * *Files 12% similar despite different names*

```diff
@@ -7,70 +7,44 @@
 
 use crate::compiler::codegen::CodeGenerator;
 use crate::compiler::lexer::SyntaxConfig;
 use crate::compiler::parser::parse_expr;
 use crate::error::{attach_basic_debug_info, Error, ErrorKind};
 use crate::expression::Expression;
 use crate::output::Output;
-use crate::template::{CompiledTemplate, Template};
+use crate::template::{CompiledTemplate, CompiledTemplateRef, Template};
 use crate::utils::{AutoEscape, BTreeMapKeysDebug, UndefinedBehavior};
 use crate::value::{FunctionArgs, FunctionResult, Value};
-use crate::vm::{State, Vm};
+use crate::vm::State;
 use crate::{defaults, filters, functions, tests};
 
-type TemplateMap<'source> = BTreeMap<&'source str, Arc<CompiledTemplate<'source>>>;
-
-#[derive(Clone)]
-enum Source<'source> {
-    Borrowed(TemplateMap<'source>, SyntaxConfig),
-    #[cfg(feature = "source")]
-    Owned(crate::source::Source),
-}
-
-impl<'source> fmt::Debug for Source<'source> {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        match self {
-            Self::Borrowed(tmpls, _) => fmt::Debug::fmt(&BTreeMapKeysDebug(tmpls), f),
-            #[cfg(feature = "source")]
-            Self::Owned(arg0) => fmt::Debug::fmt(arg0, f),
-        }
-    }
-}
-
 type AutoEscapeFunc = dyn Fn(&str) -> AutoEscape + Sync + Send;
 type FormatterFunc = dyn Fn(&mut Output, &State, &Value) -> Result<(), Error> + Sync + Send;
 
 /// An abstraction that holds the engine configuration.
 ///
 /// This object holds the central configuration state for templates.  It is also
 /// the container for all loaded templates.
 ///
 /// The environment holds references to the source the templates were created from.
 /// This makes it very inconvenient to pass around unless the templates are static
 /// strings.
-#[cfg_attr(
-    feature = "source",
-    doc = "
-For situations where you want to load dynamic templates and share the
-environment it's recommended to turn on the `source` feature and to use the
-[`Source`](crate::source::Source) type with the environment."
-)]
 ///
 /// There are generally two ways to construct an environment:
 ///
 /// * [`Environment::new`] creates an environment preconfigured with sensible
 ///   defaults.  It will contain all built-in filters, tests and globals as well
 ///   as a callback for auto escaping based on file extension.
 /// * [`Environment::empty`] creates a completely blank environment.
 #[derive(Clone)]
 pub struct Environment<'source> {
-    templates: Source<'source>,
+    templates: TemplateStore<'source>,
     filters: BTreeMap<Cow<'source, str>, filters::BoxedFilter>,
     tests: BTreeMap<Cow<'source, str>, tests::BoxedTest>,
-    pub(crate) globals: BTreeMap<Cow<'source, str>, Value>,
+    globals: BTreeMap<Cow<'source, str>, Value>,
     default_auto_escape: Arc<AutoEscapeFunc>,
     undefined_behavior: UndefinedBehavior,
     formatter: Arc<FormatterFunc>,
     #[cfg(feature = "debug")]
     debug: bool,
     #[cfg(feature = "fuel")]
     fuel: Option<u64>,
@@ -98,15 +72,15 @@
     ///
     /// This environment does not yet contain any templates but it will have all
     /// the default filters, tests and globals loaded.  If you do not want any
     /// default configuration you can use the alternative
     /// [`empty`](Environment::empty) method.
     pub fn new() -> Environment<'source> {
         Environment {
-            templates: Source::Borrowed(Default::default(), Default::default()),
+            templates: TemplateStore::default(),
             filters: defaults::get_builtin_filters(),
             tests: defaults::get_builtin_tests(),
             globals: defaults::get_globals(),
             default_auto_escape: Arc::new(defaults::default_auto_escape_callback),
             undefined_behavior: UndefinedBehavior::default(),
             formatter: Arc::new(defaults::escape_formatter),
             #[cfg(feature = "debug")]
@@ -118,163 +92,227 @@
 
     /// Creates a completely empty environment.
     ///
     /// This environment has no filters, no templates, no globals and no default
     /// logic for auto escaping configured.
     pub fn empty() -> Environment<'source> {
         Environment {
-            templates: Source::Borrowed(Default::default(), Default::default()),
+            templates: TemplateStore::default(),
             filters: Default::default(),
             tests: Default::default(),
             globals: Default::default(),
             default_auto_escape: Arc::new(defaults::no_auto_escape),
             undefined_behavior: UndefinedBehavior::default(),
             formatter: Arc::new(defaults::escape_formatter),
             #[cfg(feature = "debug")]
             debug: cfg!(debug_assertions),
             #[cfg(feature = "fuel")]
             fuel: None,
         }
     }
 
-    /// Loads a template from a string.
+    /// Loads a template from a string into the environment.
     ///
     /// The `name` parameter defines the name of the template which identifies
     /// it.  To look up a loaded template use the [`get_template`](Self::get_template)
     /// method.
     ///
+    /// ```
+    /// # use minijinja::Environment;
+    /// let mut env = Environment::new();
+    /// env.add_template("index.html", "Hello {{ name }}!").unwrap();
+    /// ```
+    ///
     /// Note that there are situations where the interface of this method is
-    /// too restrictive.  For instance the environment itself does not permit
-    /// any form of sensible dynamic template loading.
+    /// too restrictive as you need to hold on to the strings for the lifetime
+    /// of the environment.
     #[cfg_attr(
-        feature = "source",
-        doc = "To address this restriction use [`set_source`](Self::set_source)."
+        feature = "loader",
+        doc = "To address this restriction use [`add_template_owned`](Self::add_template_owned)."
     )]
     pub fn add_template(&mut self, name: &'source str, source: &'source str) -> Result<(), Error> {
-        match self.templates {
-            Source::Borrowed(ref mut map, ref syntax) => {
-                let compiled_template = ok!(CompiledTemplate::from_name_and_source_with_syntax(
-                    name,
-                    source,
-                    syntax.clone()
-                ));
-                map.insert(name, Arc::new(compiled_template));
-                Ok(())
-            }
-            #[cfg(feature = "source")]
-            Source::Owned(ref mut src) => src.add_template(name, source),
-        }
+        self.templates.insert(name, source)
+    }
+
+    /// Adds a template without without borrowing.
+    ///
+    /// This lets you place an owned [`String`] in the environment rather than the
+    /// borrowed `&str` without having to worry about lifetimes.
+    ///
+    /// ```
+    /// # use minijinja::Environment;
+    /// let mut env = Environment::new();
+    /// env.add_template_owned("index.html".to_string(), "Hello {{ name }}!".to_string()).unwrap();
+    /// ```
+    ///
+    /// **Note**: the name is a bit of a misnomer as this API also allows to borrow too as
+    /// the parameters are actually [`Cow`].
+    #[cfg(feature = "loader")]
+    #[cfg_attr(docsrs, doc(cfg(feature = "loader")))]
+    pub fn add_template_owned<N, S>(&mut self, name: N, source: S) -> Result<(), Error>
+    where
+        N: Into<Cow<'source, str>>,
+        S: Into<Cow<'source, str>>,
+    {
+        self.templates.insert_cow(name.into(), source.into())
+    }
+
+    /// Register a template loader as source of templates.
+    ///
+    /// When a template loader is registered, the environment gains the ability
+    /// to dynamically load templates.  The loader is invoked with the name of
+    /// the template.  If this template exists `Ok(Some(template_source))` has
+    /// to be returned, otherwise `Ok(None)`.  Once a template has been loaded
+    /// it's stored on the environment.  This means the loader is only invoked
+    /// once per template name.
+    ///
+    /// For loading templates from the file system, you can use the
+    /// [`path_loader`](crate::path_loader) function.
+    ///
+    /// # Example
+    ///
+    /// ```rust
+    /// # use minijinja::Environment;
+    /// fn create_env() -> Environment<'static> {
+    ///     let mut env = Environment::new();
+    ///     env.set_loader(|name| {
+    ///         if name == "layout.html" {
+    ///             Ok(Some("...".into()))
+    ///         } else {
+    ///             Ok(None)
+    ///         }
+    ///     });
+    ///     env
+    /// }
+    /// ```
+    #[cfg(feature = "loader")]
+    #[cfg_attr(docsrs, doc(cfg(feature = "loader")))]
+    pub fn set_loader<F>(&mut self, f: F)
+    where
+        F: Fn(&str) -> Result<Option<String>, Error> + Send + Sync + 'static,
+    {
+        self.templates.set_loader(f);
     }
 
     /// Removes a template by name.
     pub fn remove_template(&mut self, name: &str) {
-        match self.templates {
-            Source::Borrowed(ref mut map, _) => {
-                map.remove(name);
-            }
-            #[cfg(feature = "source")]
-            Source::Owned(ref mut source) => {
-                source.remove_template(name);
-            }
-        }
+        self.templates.remove(name);
+    }
+
+    /// Removes all stored templates.
+    ///
+    /// This method is mainly useful when combined with a loader as it causes
+    /// the loader to "reload" templates.  By calling this method one can trigger
+    /// a reload.
+    pub fn clear_templates(&mut self) {
+        self.templates.clear();
     }
 
     /// Fetches a template by name.
     ///
     /// This requires that the template has been loaded with
     /// [`add_template`](Environment::add_template) beforehand.  If the template was
-    /// not loaded an error of kind `TemplateNotFound` is returned.
+    /// not loaded an error of kind `TemplateNotFound` is returned.  If a loaded was
+    /// added to the engine this can also dynamically load templates.
     ///
     /// ```
     /// # use minijinja::{Environment, context};
     /// let mut env = Environment::new();
     /// env.add_template("hello.txt", "Hello {{ name }}!").unwrap();
     /// let tmpl = env.get_template("hello.txt").unwrap();
     /// println!("{}", tmpl.render(context!{ name => "World" }).unwrap());
     /// ```
-    pub fn get_template(&self, name: &str) -> Result<Template<'_>, Error> {
-        let compiled = match &self.templates {
-            Source::Borrowed(ref map, _) => {
-                ok!(map.get(name).ok_or_else(|| Error::new_not_found(name)))
-            }
-            #[cfg(feature = "source")]
-            Source::Owned(source) => ok!(source.get_compiled_template(name)),
-        };
+    pub fn get_template(&self, name: &str) -> Result<Template<'_, '_>, Error> {
+        let compiled = ok!(self.templates.get(name));
         Ok(Template::new(
             self,
-            compiled,
+            CompiledTemplateRef::Borrowed(compiled),
             self.initial_auto_escape(name),
         ))
     }
 
-    /// Parses and renders a template from a string in one go.
+    /// Loads a template from a string.
     ///
-    /// In some cases you really only need a template to be rendered once from
-    /// a string and returned.  The internal name of the template is `<string>`.
+    /// In some cases you really only need to work with (eg: render) a template to be
+    /// rendered once only.
     ///
     /// ```
     /// # use minijinja::{Environment, context};
     /// let env = Environment::new();
-    /// let rv = env.render_str("Hello {{ name }}", context! { name => "World" });
+    /// let tmpl = env.template_from_named_str("template_name", "Hello {{ name }}").unwrap();
+    /// let rv = tmpl.render(context! { name => "World" });
     /// println!("{}", rv.unwrap());
     /// ```
+    pub fn template_from_named_str(
+        &self,
+        name: &'source str,
+        source: &'source str,
+    ) -> Result<Template<'_, 'source>, Error> {
+        Ok(Template::new(
+            self,
+            CompiledTemplateRef::Owned(Arc::new(ok!(CompiledTemplate::new(
+                name,
+                source,
+                self._syntax_config().clone(),
+            )))),
+            self.initial_auto_escape(name),
+        ))
+    }
+
+    /// Loads a template from a string, with name `<string>`.
     ///
-    /// **Note on values:** The [`Value`] type implements `Serialize` and can be
-    /// efficiently passed to render.  It does not undergo actual serialization.
-    pub fn render_str<S: Serialize>(&self, source: &str, ctx: S) -> Result<String, Error> {
-        // reduce total amount of code faling under mono morphization into
-        // this function, and share the rest in _eval.
-        self._render_str("<string>", source, Value::from_serializable(&ctx))
+    /// This is a shortcut to [`template_from_named_str`](Self::template_from_named_str)
+    /// with name set to `<string>`.
+    pub fn template_from_str(&self, source: &'source str) -> Result<Template<'_, 'source>, Error> {
+        self.template_from_named_str("<string>", source)
     }
 
     /// Parses and renders a template from a string in one go with name.
     ///
     /// Like [`render_str`](Self::render_str), but provide a name for the
-    /// template to be used instead of the default `<string>`.
+    /// template to be used instead of the default `<string>`.  This is an
+    /// alias for [`template_from_named_str`](Self::template_from_named_str) paired with
+    /// [`render`](Template::render).
     ///
     /// ```
     /// # use minijinja::{Environment, context};
     /// let env = Environment::new();
     /// let rv = env.render_named_str(
     ///     "template_name",
     ///     "Hello {{ name }}",
-    ///     context! { name => "World" }
+    ///     context!{ name => "World" }
     /// );
     /// println!("{}", rv.unwrap());
     /// ```
     ///
     /// **Note on values:** The [`Value`] type implements `Serialize` and can be
     /// efficiently passed to render.  It does not undergo actual serialization.
     pub fn render_named_str<S: Serialize>(
         &self,
         name: &str,
         source: &str,
         ctx: S,
     ) -> Result<String, Error> {
-        // reduce total amount of code faling under mono morphization into
-        // this function, and share the rest in _eval.
-        self._render_str(name, source, Value::from_serializable(&ctx))
+        ok!(self.template_from_named_str(name, source)).render(ctx)
     }
 
-    fn _render_str(&self, name: &str, source: &str, root: Value) -> Result<String, Error> {
-        let compiled = ok!(CompiledTemplate::from_name_and_source_with_syntax(
-            name,
-            source,
-            self._syntax_config().clone()
-        ));
-        let mut rv = String::with_capacity(compiled.buffer_size_hint);
-        Vm::new(self)
-            .eval(
-                &compiled.instructions,
-                root,
-                &compiled.blocks,
-                &mut Output::with_string(&mut rv),
-                self.initial_auto_escape(name),
-            )
-            .map(|_| rv)
+    /// Parses and renders a template from a string in one go.
+    ///
+    /// In some cases you really only need a template to be rendered once from
+    /// a string and returned.  The internal name of the template is `<string>`.
+    ///
+    /// This is an alias for [`template_from_str`](Self::template_from_str) paired with
+    /// [`render`](Template::render).
+    ///
+    /// **Note on values:** The [`Value`] type implements `Serialize` and can be
+    /// efficiently passed to render.  It does not undergo actual serialization.
+    pub fn render_str<S: Serialize>(&self, source: &str, ctx: S) -> Result<String, Error> {
+        // reduce total amount of code faling under mono morphization into
+        // this function, and share the rest in _eval.
+        ok!(self.template_from_str(source)).render(ctx)
     }
 
     /// Sets a new function to select the default auto escaping.
     ///
     /// This function is invoked when templates are loaded from the environment
     /// to determine the default auto escaping behavior.  The function is
     /// invoked with the name of the template and can make an initial auto
@@ -387,14 +425,17 @@
     ///
     /// When MiniJinja is compiled with the `fuel` feature then every
     /// instruction consumes a certain amount of fuel.  Usually `1`, some will
     /// consume no fuel.  By default the engine has the fuel feature disabled
     /// (`None`).  To turn on fuel set something like `Some(50000)` which will
     /// allow 50.000 instructions to execute before running out of fuel.
     ///
+    /// To find out how much fuel is consumed, you can access the fuel levels
+    /// from the [`State`](crate::State).
+    ///
     /// Fuel consumed per-render.
     #[cfg(feature = "fuel")]
     #[cfg_attr(docsrs, doc(cfg(feature = "fuel")))]
     pub fn set_fuel(&mut self, fuel: Option<u64>) {
         self.fuel = fuel;
     }
 
@@ -410,73 +451,27 @@
     /// Note that when `source` is used, the syntax is held on the underlying source
     /// which means that the actual source needs to have it's syntax changed.
     ///
     /// See [`Syntax`](crate::Syntax) for more information.
     #[cfg(feature = "custom_syntax")]
     #[cfg_attr(docsrs, doc(cfg(feature = "custom_syntax")))]
     pub fn set_syntax(&mut self, syntax: crate::custom_syntax::Syntax) -> Result<(), Error> {
-        match self.templates {
-            Source::Borrowed(_, ref mut syn) => *syn = ok!(syntax.compile()),
-            #[cfg(feature = "source")]
-            Source::Owned(ref mut source) => ok!(source.set_syntax(syntax)),
-        };
+        self.templates.syntax_config = ok!(syntax.compile());
         Ok(())
     }
 
     /// Returns the current syntax.
     #[cfg(feature = "custom_syntax")]
     #[cfg_attr(docsrs, doc(cfg(feature = "custom_syntax")))]
     pub fn syntax(&self) -> &crate::custom_syntax::Syntax {
         &self._syntax_config().syntax
     }
 
     fn _syntax_config(&self) -> &SyntaxConfig {
-        match self.templates {
-            Source::Borrowed(_, ref syn) => syn,
-            #[cfg(feature = "source")]
-            Source::Owned(ref source) => source._syntax_config(),
-        }
-    }
-
-    /// Sets the template source for the environment.
-    ///
-    /// This helps when working with dynamically loaded templates.  The
-    /// [`Source`](crate::source::Source) is consulted by the environment to
-    /// look up templates that are requested.  The source has the capabilities
-    /// to load templates with fewer lifetime restrictions and can also
-    /// load templates dynamically at runtime as requested.
-    ///
-    /// When a source is set already loaded templates in the environment are
-    /// discarded and replaced with the templates from the source.
-    ///
-    /// For more information see [`Source`](crate::source::Source).
-    #[cfg(feature = "source")]
-    #[cfg_attr(docsrs, doc(cfg(feature = "source")))]
-    pub fn set_source(&mut self, source: crate::source::Source) {
-        self.templates = Source::Owned(source);
-    }
-
-    /// Returns the currently set source.
-    #[cfg(feature = "source")]
-    #[cfg_attr(docsrs, doc(cfg(feature = "source")))]
-    pub fn source(&self) -> Option<&crate::source::Source> {
-        match self.templates {
-            Source::Borrowed(..) => None,
-            Source::Owned(ref source) => Some(source),
-        }
-    }
-
-    /// Returns the currently set source as mutable reference.
-    #[cfg(feature = "source")]
-    #[cfg_attr(docsrs, doc(cfg(feature = "source")))]
-    pub fn source_mut(&mut self) -> Option<&mut crate::source::Source> {
-        match self.templates {
-            Source::Borrowed(..) => None,
-            Source::Owned(ref mut source) => Some(source),
-        }
+        &self.templates.syntax_config
     }
 
     /// Compiles an expression.
     ///
     /// This lets one compile an expression in the template language and
     /// receive the output.  This lets one use the expressions of the language
     /// be used as a minimal scripting language.  For more information and an
@@ -565,14 +560,19 @@
     }
 
     /// Removes a global function or variable by name.
     pub fn remove_global(&mut self, name: &str) {
         self.globals.remove(name);
     }
 
+    /// Returns an empty [`State`] for testing purposes and similar.
+    pub fn empty_state(&self) -> State<'_, '_> {
+        State::new_for_env(self)
+    }
+
     /// Looks up a function.
     pub(crate) fn get_global(&self, name: &str) -> Option<Value> {
         self.globals.get(name).cloned()
     }
 
     /// Looks up a filter.
     pub(crate) fn get_filter(&self, name: &str) -> Option<&filters::BoxedFilter> {
@@ -602,7 +602,59 @@
         if value.is_undefined() && matches!(self.undefined_behavior, UndefinedBehavior::Strict) {
             Err(Error::from(ErrorKind::UndefinedError))
         } else {
             (self.formatter)(out, state, value)
         }
     }
 }
+
+#[cfg(not(feature = "loader"))]
+mod basic_store {
+    use super::*;
+
+    #[derive(Clone, Default)]
+    pub struct BasicStore<'source> {
+        pub syntax_config: SyntaxConfig,
+        map: BTreeMap<&'source str, Arc<CompiledTemplate<'source>>>,
+    }
+
+    impl<'source> fmt::Debug for BasicStore<'source> {
+        fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+            BTreeMapKeysDebug(&self.map).fmt(f)
+        }
+    }
+
+    impl<'source> BasicStore<'source> {
+        pub fn insert(&mut self, name: &'source str, source: &'source str) -> Result<(), Error> {
+            self.map.insert(
+                name,
+                Arc::new(ok!(CompiledTemplate::new(
+                    name,
+                    source,
+                    self.syntax_config.clone()
+                ))),
+            );
+            Ok(())
+        }
+
+        pub fn remove(&mut self, name: &str) {
+            self.map.remove(name);
+        }
+
+        pub fn clear(&mut self) {
+            self.map.clear();
+        }
+
+        pub fn get(&self, name: &str) -> Result<&CompiledTemplate<'source>, Error> {
+            self.map
+                .get(name)
+                .map(|x| &**x)
+                .ok_or_else(|| Error::new_not_found(name))
+        }
+    }
+}
+
+#[cfg(not(feature = "loader"))]
+use self::basic_store::BasicStore as TemplateStore;
+
+#[cfg(feature = "loader")]
+use crate::loader::LoaderStore as TemplateStore;
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/error.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/error.rs`

 * *Files 21% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 
         Ok(())
     }
 }
 
 /// An enum describing the error kind.
 #[derive(Debug, Copy, Clone, PartialEq, Eq)]
+#[non_exhaustive]
 pub enum ErrorKind {
     /// A non primitive value was encountered where one was expected.
     NonPrimitive,
     /// A value is not valid for a key in a map.
     NonKey,
     /// An invalid operation was attempted.
     InvalidOperation,
@@ -136,14 +137,17 @@
     WriteFailure,
     /// Engine ran out of fuel
     #[cfg(feature = "fuel")]
     OutOfFuel,
     #[cfg(feature = "custom_syntax")]
     /// Error creating aho-corasick delimiters
     InvalidDelimiter,
+    /// An unknown block was called
+    #[cfg(feature = "multi_template")]
+    UnknownBlock,
 }
 
 impl ErrorKind {
     fn description(self) -> &'static str {
         match self {
             ErrorKind::NonPrimitive => "not a primitive",
             ErrorKind::NonKey => "not a key type",
@@ -163,14 +167,16 @@
             ErrorKind::EvalBlock => "could not render block",
             ErrorKind::CannotUnpack => "cannot unpack",
             ErrorKind::WriteFailure => "failed to write output",
             #[cfg(feature = "fuel")]
             ErrorKind::OutOfFuel => "engine ran out of fuel",
             #[cfg(feature = "custom_syntax")]
             ErrorKind::InvalidDelimiter => "invalid custom delimiters",
+            #[cfg(feature = "multi_template")]
+            ErrorKind::UnknownBlock => "unknown block",
         }
     }
 }
 
 impl fmt::Display for ErrorKind {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         write!(f, "{}", self.description())
@@ -249,41 +255,83 @@
     }
 
     /// Returns the error kind
     pub fn kind(&self) -> ErrorKind {
         self.repr.kind
     }
 
+    /// Returns the error detail
+    ///
+    /// The detail is an error message that provides further details about
+    /// the error kind.
+    pub fn detail(&self) -> Option<&str> {
+        self.repr.detail.as_deref()
+    }
+
     /// Returns the filename of the template that caused the error.
     pub fn name(&self) -> Option<&str> {
         self.repr.name.as_deref()
     }
 
     /// Returns the line number where the error occurred.
     pub fn line(&self) -> Option<usize> {
         if self.repr.lineno > 0 {
             Some(self.repr.lineno)
         } else {
             None
         }
     }
 
+    /// Returns the byte range of where the error occurred if available.
+    ///
+    /// In combination with [`template_source`](Self::template_source) this can be
+    /// used to better visualize where the error is coming from.  By indexing into
+    /// the template source one ends up with the source of the failing expression.
+    ///
+    /// Note that debug mode ([`Environment::set_debug`](crate::Environment::set_debug))
+    /// needs to be enabled, and the `debug` feature must be turned on.  The engine
+    /// usually keeps track of spans in all cases, but there is no absolute guarantee
+    /// that it is able to provide a range in all error cases.
+    ///
+    /// ```
+    /// # use minijinja::{Error, Environment, context};
+    /// # let mut env = Environment::new();
+    /// # env.set_debug(true);
+    /// let tmpl = env.template_from_str("Hello {{ foo + bar }}!").unwrap();
+    /// let err = tmpl.render(context!(foo => "a string", bar => 0)).unwrap_err();
+    /// let src = err.template_source().unwrap();
+    /// assert_eq!(&src[err.range().unwrap()], "foo + bar");
+    /// ```
+    #[cfg(feature = "debug")]
+    #[cfg_attr(docsrs, doc(cfg(feature = "debug")))]
+    pub fn range(&self) -> Option<std::ops::Range<usize>> {
+        self.repr
+            .span
+            .map(|x| x.start_offset as usize..x.end_offset as usize)
+    }
+
+    /// Returns the template source if available.
+    #[cfg(feature = "debug")]
+    #[cfg_attr(docsrs, doc(cfg(feature = "debug")))]
+    pub fn template_source(&self) -> Option<&str> {
+        self.debug_info().and_then(|x| x.source())
+    }
+
     /// Returns the line number where the error occurred.
     #[cfg(feature = "debug")]
     pub(crate) fn span(&self) -> Option<Span> {
         self.repr.span
     }
 
     /// Returns the template debug information is available.
     ///
     /// The debug info snapshot is only embedded into the error if the debug
     /// mode is enabled on the environment
     /// ([`Environment::set_debug`](crate::Environment::set_debug)).
     #[cfg(feature = "debug")]
-    #[cfg_attr(docsrs, doc(cfg(feature = "debug")))]
     pub(crate) fn debug_info(&self) -> Option<&crate::debug::DebugInfo> {
         self.repr.debug_info.as_ref()
     }
 
     #[cfg(feature = "debug")]
     #[cfg_attr(docsrs, doc(cfg(feature = "debug")))]
     pub(crate) fn attach_debug_info(&mut self, value: crate::debug::DebugInfo) {
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/filters.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/filters.rs`

 * *Files 4% similar despite different names*

```diff
@@ -249,24 +249,20 @@
 }
 
 #[cfg(feature = "builtins")]
 mod builtins {
     use super::*;
 
     use crate::error::ErrorKind;
-    use crate::key::Key;
     use crate::value::{Kwargs, ValueKind, ValueRepr};
     use std::borrow::Cow;
     use std::cmp::Ordering;
     use std::fmt::Write;
     use std::mem;
 
-    #[cfg(test)]
-    use {crate::testutils::apply_filter, similar_asserts::assert_eq};
-
     /// Converts a value to uppercase.
     ///
     /// ```jinja
     /// <h1>{{ chapter.title|upper }}</h1>
     /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn upper(v: Cow<'_, str>) -> String {
@@ -353,31 +349,38 @@
                 ErrorKind::InvalidOperation,
                 format!("cannot calculate length of value of type {}", v.kind()),
             )
         })
     }
 
     fn sort_helper(a: &Value, b: &Value, case_sensitive: bool) -> Ordering {
-        if !case_sensitive && (a.kind() == ValueKind::String || b.kind() == ValueKind::String) {
-            // TODO: optional unicode support
-            return a
-                .to_string()
-                .to_ascii_lowercase()
-                .cmp(&b.to_string().to_ascii_lowercase());
-        }
-        match (Key::from_borrowed_value(a), Key::from_borrowed_value(b)) {
-            (Ok(a), Ok(b)) => a.partial_cmp(&b),
-            _ => a.partial_cmp(b),
+        if !case_sensitive {
+            if let (Some(a), Some(b)) = (a.as_str(), b.as_str()) {
+                #[cfg(feature = "unicode")]
+                {
+                    return unicase::UniCase::new(a).cmp(&unicase::UniCase::new(b));
+                }
+                #[cfg(not(feature = "unicode"))]
+                {
+                    return a.to_ascii_lowercase().cmp(&b.to_ascii_lowercase());
+                }
+            }
         }
-        .unwrap_or(Ordering::Less)
+        a.cmp(b)
     }
 
     /// Dict sorting functionality.
     ///
     /// This filter works like `|items` but sorts the pairs by key first.
+    ///
+    /// The filter accepts a few keyword arguments:
+    ///
+    /// * `case_sensitive`: set to `true` to make the sorting of strings case sensitive.
+    /// * `by`: set to `"value"` to sort by value. Defaults to `"key"`.
+    /// * `reverse`: set to `true` to sort in reverse.
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn dictsort(v: Value, kwargs: Kwargs) -> Result<Value, Error> {
         if v.kind() == ValueKind::Map {
             let mut rv = Vec::with_capacity(v.len().unwrap_or(0));
             let iter = ok!(v.try_iter());
             for key in iter {
                 let value = v.get_item(&key).unwrap_or(Value::UNDEFINED);
@@ -649,31 +652,34 @@
 
     /// Returns the smallest item from the list.
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn min(state: &State, value: Value) -> Result<Value, Error> {
         let iter = ok!(state.undefined_behavior().try_iter(value).map_err(|err| {
             Error::new(ErrorKind::InvalidOperation, "cannot convert value to list").with_source(err)
         }));
-        Ok(iter
-            .min_by(|a, b| a.partial_cmp(b).unwrap_or(Ordering::Less))
-            .unwrap_or(Value::UNDEFINED))
+        Ok(iter.min().unwrap_or(Value::UNDEFINED))
     }
 
     /// Returns the largest item from the list.
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn max(state: &State, value: Value) -> Result<Value, Error> {
         let iter = ok!(state.undefined_behavior().try_iter(value).map_err(|err| {
             Error::new(ErrorKind::InvalidOperation, "cannot convert value to list").with_source(err)
         }));
-        Ok(iter
-            .max_by(|a, b| a.partial_cmp(b).unwrap_or(Ordering::Less))
-            .unwrap_or(Value::UNDEFINED))
+        Ok(iter.max().unwrap_or(Value::UNDEFINED))
     }
 
     /// Returns the sorted version of the given list.
+    ///
+    /// The filter accepts a few keyword arguments:
+    ///
+    /// * `case_sensitive`: set to `true` to make the sorting of strings case sensitive.
+    /// * `attribute`: can be set to an attribute or dotted path to sort by that attribute
+    /// * `reverse`: set to `true` to sort in reverse.
+    ///
     /// ```jinja
     /// {{ [1, 3, 2, 4]|sort }} -> [4, 3, 2, 1]
     /// {{ [1, 3, 2, 4]|sort(reverse=true) }} -> [1, 2, 3, 4]
     /// # Sort users by age attribute in descending order.
     /// {{ users|sort(attribute="age") }}
     /// # Sort users by age attribute in ascending order.
     /// {{ users|sort(attribute="age", reverse=true) }}
@@ -1125,15 +1131,16 @@
         state: &State,
         value: Value,
         args: crate::value::Rest<Value>,
     ) -> Result<Vec<Value>, Error> {
         let mut rv = Vec::with_capacity(value.len().unwrap_or(0));
 
         // attribute mapping
-        let (args, kwargs) = Kwargs::from_args(&args);
+        let (args, kwargs): (&[Value], Kwargs) = crate::value::from_args(&args)?;
+
         if let Some(attr) = ok!(kwargs.get::<Option<Value>>("attribute")) {
             if !args.is_empty() {
                 return Err(Error::from(ErrorKind::TooManyArguments));
             }
             let default = ok!(kwargs.get::<Option<Value>>("default"));
             for value in ok!(state.undefined_behavior().try_iter(value)) {
                 let sub_val = match attr.as_str() {
@@ -1178,139 +1185,49 @@
                 .chain(args.iter().skip(1).cloned())
                 .collect::<Vec<_>>();
             rv.push(ok!(filter.apply_to(state, &new_args)));
         }
         Ok(rv)
     }
 
-    #[test]
-    fn test_basics() {
-        fn test(a: u32, b: u32) -> Result<u32, Error> {
-            Ok(a + b)
-        }
-
-        let mut env = crate::Environment::new();
-        env.add_filter("test", test);
-        assert_eq!(
-            apply_filter(&env, "test", &[Value::from(23), Value::from(42)]).unwrap(),
-            Value::from(65)
-        );
-    }
-
-    #[test]
-    fn test_rest_args() {
-        fn sum(val: u32, rest: crate::value::Rest<u32>) -> u32 {
-            rest.iter().fold(val, |a, b| a + b)
-        }
-
-        let mut env = crate::Environment::new();
-        env.add_filter("sum", sum);
-        assert_eq!(
-            apply_filter(
-                &env,
-                "sum",
-                &[
-                    Value::from(1),
-                    Value::from(2),
-                    Value::from(3),
-                    Value::from(4)
-                ][..]
-            )
-            .unwrap(),
-            Value::from(1 + 2 + 3 + 4)
-        );
-    }
-
-    #[test]
-    fn test_optional_args() {
-        fn add(val: u32, a: u32, b: Option<u32>) -> Result<u32, Error> {
-            // ensure we really get our value as first argument
-            assert_eq!(val, 23);
-            let mut sum = val + a;
-            if let Some(b) = b {
-                sum += b;
-            }
-            Ok(sum)
-        }
-
-        let mut env = crate::Environment::new();
-        env.add_filter("add", add);
-        assert_eq!(
-            apply_filter(&env, "add", &[Value::from(23), Value::from(42)][..]).unwrap(),
-            Value::from(65)
-        );
-        assert_eq!(
-            apply_filter(
-                &env,
-                "add",
-                &[Value::from(23), Value::from(42), Value::UNDEFINED][..]
-            )
-            .unwrap(),
-            Value::from(65)
-        );
-        assert_eq!(
-            apply_filter(
-                &env,
-                "add",
-                &[Value::from(23), Value::from(42), Value::from(1)][..]
-            )
-            .unwrap(),
-            Value::from(66)
-        );
-    }
+    /// Returns a list of unique items from the given iterable.
+    ///
+    /// Returns a list of unique items from the given iterable.
+    ///
+    /// ```jinja
+    /// {{ ['foo', 'bar', 'foobar', 'FooBar']|unique|list }}
+    ///   -> ['foo', 'bar', 'foobar']
+    /// ```
+    ///
+    /// The unique items are yielded in the same order as their first occurrence
+    /// in the iterable passed to the filter.  The filter will not detect
+    /// duplicate objects or arrays, only primitives such as strings or numbers.
+    #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
+    #[cfg(feature = "builtins")]
+    pub fn unique(values: Vec<Value>) -> Value {
+        use std::collections::BTreeSet;
 
-    #[test]
-    fn test_values_in_vec() {
-        fn upper(value: &str) -> String {
-            value.to_uppercase()
-        }
+        let mut rv = Vec::new();
+        let mut seen = BTreeSet::new();
 
-        fn sum(value: Vec<i64>) -> i64 {
-            value.into_iter().sum::<i64>()
+        for item in values {
+            if !seen.contains(&item) {
+                rv.push(item.clone());
+                seen.insert(item);
+            }
         }
 
-        let mut env = crate::Environment::new();
-        env.add_filter("upper", upper);
-        env.add_filter("sum", sum);
-
-        assert_eq!(
-            apply_filter(&env, "upper", &[Value::from("Hello World!")]).unwrap(),
-            Value::from("HELLO WORLD!")
-        );
-
-        assert_eq!(
-            apply_filter(
-                &env,
-                "sum",
-                &[Value::from(vec![Value::from(1), Value::from(2)])]
-            )
-            .unwrap(),
-            Value::from(3)
-        );
+        Value::from(rv)
     }
 
-    #[test]
-    fn test_seq_object_borrow() {
-        fn connect(values: &dyn crate::value::SeqObject) -> String {
-            let mut rv = String::new();
-            for item in values.iter() {
-                rv.push_str(&item.to_string())
-            }
-            rv
-        }
-
-        let mut env = crate::Environment::new();
-        env.add_filter("connect", connect);
-        assert_eq!(
-            apply_filter(
-                &env,
-                "connect",
-                &[Value::from(vec![Value::from("HELLO"), Value::from(42)])]
-            )
-            .unwrap(),
-            Value::from("HELLO42")
-        );
+    /// Pretty print a variable.
+    ///
+    /// This is useful for debugging as it better shows what's inside an object.
+    #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
+    #[cfg(feature = "builtins")]
+    pub fn pprint(value: &Value) -> String {
+        format!("{:#?}", value)
     }
 }
 
 #[cfg(feature = "builtins")]
 pub use self::builtins::*;
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/functions.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/functions.rs`

 * *Files 2% similar despite different names*

```diff
@@ -198,18 +198,18 @@
 }
 
 impl fmt::Debug for BoxedFunction {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         #[cfg(feature = "debug")]
         {
             if !self.1.is_empty() {
-                return write!(f, "{}", self.1);
+                return f.write_str(self.1);
             }
         }
-        write!(f, "function")
+        f.write_str("function")
     }
 }
 
 impl fmt::Display for BoxedFunction {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         write!(f, "{self:?}")
     }
@@ -224,15 +224,15 @@
 #[cfg(feature = "builtins")]
 mod builtins {
     use super::*;
 
     use std::collections::BTreeMap;
 
     use crate::error::ErrorKind;
-    use crate::value::ValueKind;
+    use crate::value::{MapType, ValueRepr};
 
     /// Returns a range.
     ///
     /// Return a list containing an arithmetic progression of integers. `range(i,
     /// j)` returns `[i, i+1, i+2, ..., j-1]`. `lower` defaults to 0. When `step` is
     /// given, it specifies the increment (or decrement). For example, `range(4)`
     /// and `range(0, 4, 1)` return `[0, 1, 2, 3]`. The end point is omitted.
@@ -286,20 +286,18 @@
     /// <script>const CONFIG = {{ dict(
     ///   DEBUG=true,
     ///   API_URL_PREFIX="/api"
     /// )|tojson }};</script>
     /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn dict(value: Value) -> Result<Value, Error> {
-        if value.is_undefined() {
-            Ok(Value::from(BTreeMap::<bool, Value>::new()))
-        } else if value.kind() != ValueKind::Map {
-            Err(Error::from(ErrorKind::InvalidOperation))
-        } else {
-            Ok(value)
+        match value.0 {
+            ValueRepr::Undefined => Ok(Value::from(BTreeMap::<bool, Value>::new())),
+            ValueRepr::Map(map, _) => Ok(Value(ValueRepr::Map(map, MapType::Normal))),
+            _ => Err(Error::from(ErrorKind::InvalidOperation)),
         }
     }
 
     /// Outputs the current context stringified.
     ///
     /// This is a useful function to quickly figure out the state of affairs
     /// in a template.  It emits a stringified debug dump of the current
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/lib.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -141,44 +141,49 @@
 //!   - `macros`: when removed the `{% macro %}` tag is not included.
 //!   - `multi_template`: when removed the templates related to imports and extends
 //!     are removed (`{% from %}`, `{% import %}`, `{% include %}`, and `{% extends %}`
 //!     as well as `{% block %}`).
 //!   - `adjacent_loop_items`: when removed the `previtem` and `nextitem` attributes of
 //!     the `loop` object no longer exist.  Removing this feature can provide faster
 //!     template execution when a lot of loops are involved.
-//!   - `unicode`: when added unicode identifiers are supported.  Without this features
-//!     only ASCII identifiers can be used for variable names and attributes.
+//!   - `unicode`: when added unicode identifiers are supported and the `sort`
+//!     filter's case insensitive comparising changes to using unicode and not
+//!     ASCII rules.  Without this features only ASCII identifiers can be used
+//!     for variable names and attributes.
 //!
 //! - **Rust Functionality:**
 //!
 //!   - `debug`: if this feature is removed some debug functionality of the engine is
 //!     removed as well.  This mainly affects the quality of error reporting.
 //!   - `deserialization`: when removed this disables deserialization support for
 //!     the [`Value`](crate::value::Value) type.
 //!
-//! There are some additional features that can be enabled:
+//! There are some additional features that provide extra functionality:
 //!
 //! - `fuel`: enables the `fuel` feature which makes the engine track fuel consumption which
 //!   can be used to better protect against expensive templates.
-//! - `source`: enables the `Source` type which helps with dynamic loading of templates.
-//! - `speedups`: enables all speedups, in particular it turns on the `v_htmlescape` dependency
-//!   for faster HTML escapling.
+//! - `loader`: enables owned and dynamic template loading of templates.
+//! - `custom_syntax`: when this feature is enabled, custom delimiters are supported by
+//!   the parser.
+//! - `preserve_order`: When enable the internal value implementation uses an indexmap
+//!   which preserves the original order of maps and structs.
 //! - `json`: When enabled the `tojson` filter is added as builtin filter as well as
 //!   the ability to auto escape via `AutoEscape::Json`.
 //! - `urlencode`: When enabled the `urlencode` filter is added as builtin filter.
-//! - `preserve_order`: When enable the internal value implementation uses an indexmap
-//!   which preserves the original order of maps and structs.
+//!
+//! Performance and memory related features:
+//!
+//! - `speedups`: enables all speedups, in particular it turns on the `v_htmlescape` dependency
+//!   for faster HTML escapling.
 //! - `key_interning`: if this feature is enabled the automatic string interning in
 //!   the value type is enabled.  This feature used to be turned on by default but
 //!   has negative performance effects in newer versions of MiniJinja since a lot of
 //!   the previous uses of key interning are no longer needed.  Enabling it however
 //!   cuts down on memory usage slightly in certain scenarios by interning all string
 //!   keys used in dynamic map values.
-//! - `custom_syntax`: when this feature is enabled, custom delimiters are supported by
-//!   the parser.
 //!
 //! </details>
 #![allow(clippy::cognitive_complexity)]
 #![allow(clippy::get_first)]
 #![cfg_attr(docsrs, feature(doc_cfg))]
 #![deny(missing_docs)]
 #![doc(html_logo_url = "https://github.com/mitsuhiko/minijinja/raw/main/artwork/logo-square.png")]
@@ -187,32 +192,30 @@
 mod macros;
 
 mod compiler;
 mod defaults;
 mod environment;
 mod error;
 mod expression;
-mod key;
 mod output;
 mod template;
 mod utils;
 mod vm;
 
 pub mod filters;
 pub mod functions;
 pub mod syntax;
 pub mod tests;
 pub mod value;
 
-#[cfg(any(test, feature = "testutils"))]
-#[cfg_attr(docsrs, doc(cfg(feature = "testutils")))]
-pub mod testutils;
+#[cfg(feature = "loader")]
+mod loader;
 
-#[cfg(feature = "source")]
-mod source;
+#[cfg(feature = "loader")]
+pub use loader::path_loader;
 
 #[cfg(feature = "custom_syntax")]
 mod custom_syntax;
 
 #[cfg(feature = "debug")]
 mod debug;
 
@@ -223,17 +226,14 @@
 pub use self::output::Output;
 pub use self::template::Template;
 pub use self::utils::{AutoEscape, HtmlEscape, UndefinedBehavior};
 
 #[cfg(feature = "custom_syntax")]
 pub use self::custom_syntax::Syntax;
 
-#[cfg(feature = "source")]
-pub use self::source::Source;
-
 pub use self::macros::__context;
 pub use self::vm::State;
 
 /// This module gives access to the low level machinery.
 ///
 /// This module is only provided by the `unstable_machinery` feature and does not
 /// have a stable interface.  It mostly exists for internal testing purposes and
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/macros.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/macros.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#[cfg(test)]
-use similar_asserts::assert_eq;
-
 // `ok!` and `some!` are less bloaty alternatives to the standard library's try operator (`?`).
 // Since we do not need type conversions in this crate we can fall back to much easier match
 // patterns that compile faster and produce less bloaty code.
 
 macro_rules! ok {
     ($expr:expr) => {
         match $expr {
@@ -22,16 +19,15 @@
         }
     };
 }
 
 /// Hidden utility module for the [`context!`](crate::context!) macro.
 #[doc(hidden)]
 pub mod __context {
-    use crate::key::Key;
-    use crate::value::{MapType, Value, ValueMap, ValueRepr};
+    use crate::value::{KeyRef, MapType, Value, ValueMap, ValueRepr};
     use crate::Environment;
     use std::rc::Rc;
     use std::sync::Arc;
 
     #[inline(always)]
     pub fn value_optimization() -> impl Drop {
         crate::value::value_optimization()
@@ -40,15 +36,15 @@
     #[inline(always)]
     pub fn make() -> ValueMap {
         ValueMap::default()
     }
 
     #[inline(always)]
     pub fn add(ctx: &mut ValueMap, key: &'static str, value: Value) {
-        ctx.insert(Key::Str(key), value);
+        ctx.insert(KeyRef::Str(key), value);
     }
 
     #[inline(always)]
     pub fn build(ctx: ValueMap) -> Value {
         ValueRepr::Map(Arc::new(ctx), MapType::Normal).into()
     }
 
@@ -182,29 +178,7 @@
     (
         $tmpl:expr
         $(, $key:ident $(=> $value:expr)?)* $(,)?
     ) => {
         $crate::render!(in $crate::__context::thread_local_env(), $tmpl, $($key $(=> $value)? ,)*)
     }
 }
-
-#[test]
-fn test_context() {
-    use crate::value::Value;
-    let var1 = 23;
-    let ctx = context!(var1, var2 => 42);
-    assert_eq!(ctx.get_attr("var1").unwrap(), Value::from(23));
-    assert_eq!(ctx.get_attr("var2").unwrap(), Value::from(42));
-}
-
-#[test]
-fn test_render() {
-    let env = crate::Environment::new();
-    let rv = render!(in env, "Hello {{ name }}!", name => "World");
-    assert_eq!(rv, "Hello World!");
-
-    let rv = render!("Hello {{ name }}!", name => "World");
-    assert_eq!(rv, "Hello World!");
-
-    let rv = render!("Hello World!");
-    assert_eq!(rv, "Hello World!");
-}
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/output.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/output.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 use std::{fmt, io};
 
+use crate::error::{Error, ErrorKind};
 use crate::utils::AutoEscape;
 use crate::value::Value;
 
 /// How should output be captured?
-#[derive(Debug, Clone, Copy)]
+#[derive(Debug, Clone, Copy, Eq, PartialEq)]
 #[cfg_attr(feature = "unstable_machinery_serde", derive(serde::Serialize))]
 pub enum CaptureMode {
     Capture,
     #[allow(unused)]
     Discard,
 }
 
-/// An abstraction over [`Write`](std::fmt::Write) for the rendering.
+/// An abstraction over [`fmt::Write`](std::fmt::Write) for the rendering.
 ///
 /// This is a utility type used in the engine which can be written into like one
 /// can write into an [`std::fmt::Write`] value.  It's primarily used internally
 /// in the engine but it's also passed to the custom formatter function.
 pub struct Output<'a> {
     w: &'a mut (dyn fmt::Write + 'a),
     capture_stack: Vec<Option<String>>,
@@ -36,17 +37,20 @@
             w,
             capture_stack: Vec::new(),
         }
     }
 
     /// Creates a null output that writes nowhere.
     pub(crate) fn null() -> Self {
+        // The null writer also has a single entry on the discarding capture
+        // stack.  In fact, `w` is more or less useless here as we always
+        // shadow it.  This is done so that `is_discarding` returns true.
         Self {
             w: NullWriter::get_mut(),
-            capture_stack: Vec::new(),
+            capture_stack: vec![None],
         }
     }
 
     /// Begins capturing into a string or discard.
     pub(crate) fn begin_capture(&mut self, mode: CaptureMode) {
         self.capture_stack.push(match mode {
             CaptureMode::Capture => Some(String::new()),
@@ -72,14 +76,21 @@
         match self.capture_stack.last_mut() {
             Some(Some(stream)) => stream as _,
             Some(None) => NullWriter::get_mut(),
             None => self.w,
         }
     }
 
+    /// Returns `true` if the output is discarding.
+    #[inline(always)]
+    #[allow(unused)]
+    pub(crate) fn is_discarding(&self) -> bool {
+        matches!(self.capture_stack.last(), Some(None))
+    }
+
     /// Writes some data to the underlying buffer contained within this output.
     #[inline]
     pub fn write_str(&mut self, s: &str) -> fmt::Result {
         self.target().write_str(s)
     }
 
     /// Writes some formatted information into this instance.
@@ -130,14 +141,27 @@
 }
 
 pub struct WriteWrapper<W> {
     pub w: W,
     pub err: Option<io::Error>,
 }
 
+impl<W> WriteWrapper<W> {
+    /// Replaces the given error with the held error if available.
+    pub fn take_err(&mut self, original: Error) -> Error {
+        self.err
+            .take()
+            .map(|io_err| {
+                Error::new(ErrorKind::WriteFailure, "I/O error during rendering")
+                    .with_source(io_err)
+            })
+            .unwrap_or(original)
+    }
+}
+
 impl<W: io::Write> fmt::Write for WriteWrapper<W> {
     #[inline]
     fn write_str(&mut self, s: &str) -> fmt::Result {
         self.w.write_all(s.as_bytes()).map_err(|e| {
             self.err = Some(e);
             fmt::Error
         })
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/syntax.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/syntax.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/tests.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/tests.rs`

 * *Files 6% similar despite different names*

```diff
@@ -438,27 +438,54 @@
     #[cfg(feature = "builtins")]
     pub fn is_in(value: &Value, other: &Value) -> bool {
         crate::value::ops::contains(other, value)
             .map(|value| value.is_true())
             .unwrap_or(false)
     }
 
-    #[test]
-    fn test_basics() {
-        fn test(_: &State, a: u32, b: u32) -> bool {
-            assert_eq!(a, 23);
-            a == b
-        }
+    /// Checks if a value is `true`.
+    ///
+    /// ```jinja
+    /// {% if value is true %}...{% endif %}
+    /// ```
+    #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
+    #[cfg(feature = "builtins")]
+    pub fn is_true(value: &Value) -> bool {
+        matches!(value.0, crate::value::ValueRepr::Bool(true))
+    }
+
+    /// Checks if a value is `false`.
+    ///
+    /// ```jinja
+    /// {% if value is false %}...{% endif %}
+    /// ```
+    #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
+    #[cfg(feature = "builtins")]
+    pub fn is_false(value: &Value) -> bool {
+        matches!(value.0, crate::value::ValueRepr::Bool(false))
+    }
 
-        let mut env = crate::Environment::new();
-        env.add_test("test", test);
-        assert!(crate::testutils::perform_test(
-            &env,
-            "test",
-            &[Value::from(23), Value::from(23)][..]
-        )
-        .unwrap());
+    /// Checks if a filter with a given name is available.
+    ///
+    /// ```jinja
+    /// {% if 'tojson' is filter %}...{% endif %}
+    /// ```
+    #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
+    #[cfg(feature = "builtins")]
+    pub fn is_filter(state: &State, name: &str) -> bool {
+        state.env.get_filter(name).is_some()
+    }
+
+    /// Checks if a test with a given name is available.
+    ///
+    /// ```jinja
+    /// {% if 'greaterthan' is test %}...{% endif %}
+    /// ```
+    #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
+    #[cfg(feature = "builtins")]
+    pub fn is_test(state: &State, name: &str) -> bool {
+        state.env.get_test(name).is_some()
     }
 }
 
 #[cfg(feature = "builtins")]
 pub use self::builtins::*;
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/utils.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/utils.rs`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 use std::iter::{once, repeat};
 use std::str::Chars;
 
 use crate::error::{Error, ErrorKind};
 use crate::value::{OwnedValueIterator, StringType, Value, ValueKind, ValueRepr};
 use crate::Output;
 
-#[cfg(test)]
-use similar_asserts::assert_eq;
-
 /// internal marker to seal up some trait methods
 pub struct SealedMarker;
 
 pub fn memchr(haystack: &[u8], needle: u8) -> Option<usize> {
     haystack.iter().position(|&x| x == needle)
 }
 
 pub fn memstr(haystack: &[u8], needle: &[u8]) -> Option<usize> {
     haystack
         .windows(needle.len())
         .position(|window| window == needle)
 }
 
+/// Helper for dealing with untrusted size hints.
+#[inline(always)]
+pub(crate) fn untrusted_size_hint(value: usize) -> usize {
+    value.min(1024)
+}
+
 fn write_with_html_escaping(out: &mut Output, value: &Value) -> fmt::Result {
     if matches!(
         value.kind(),
         ValueKind::Undefined | ValueKind::None | ValueKind::Bool | ValueKind::Number
     ) {
         write!(out, "{value}")
     } else if let Some(s) = value.as_str() {
@@ -188,14 +191,15 @@
             let bytes = self.0.as_bytes();
             let mut start = 0;
 
             for (i, b) in bytes.iter().enumerate() {
                 macro_rules! escaping_body {
                     ($quote:expr) => {{
                         if start < i {
+                            // SAFETY: this is safe because we only push valid utf-8 bytes over
                             ok!(f.write_str(unsafe {
                                 std::str::from_utf8_unchecked(&bytes[start..i])
                             }));
                         }
                         ok!(f.write_str($quote));
                         start = i + 1;
                     }};
@@ -210,14 +214,15 @@
                         b'/' => escaping_body!("&#x2f;"),
                         _ => (),
                     }
                 }
             }
 
             if start < bytes.len() {
+                // SAFETY: this is safe because we only push valid utf-8 bytes over
                 f.write_str(unsafe { std::str::from_utf8_unchecked(&bytes[start..]) })
             } else {
                 Ok(())
             }
         }
     }
 }
@@ -322,21 +327,28 @@
 
 impl<F: FnOnce()> Drop for OnDrop<F> {
     fn drop(&mut self) {
         self.0.take().unwrap()();
     }
 }
 
-#[test]
-fn test_html_escape() {
-    let input = "<>&\"'/";
-    let output = HtmlEscape(input).to_string();
-    assert_eq!(output, "&lt;&gt;&amp;&quot;&#x27;&#x2f;");
-}
+#[cfg(test)]
+mod tests {
+    use super::*;
 
-#[test]
-fn test_unescape() {
-    assert_eq!(unescape(r"foo\u2603bar").unwrap(), "foo\u{2603}bar");
-    assert_eq!(unescape(r"\t\b\f\r\n\\\/").unwrap(), "\t\x08\x0c\r\n\\/");
-    assert_eq!(unescape("foobarbaz").unwrap(), "foobarbaz");
-    assert_eq!(unescape(r"\ud83d\udca9").unwrap(), "💩");
+    use similar_asserts::assert_eq;
+
+    #[test]
+    fn test_html_escape() {
+        let input = "<>&\"'/";
+        let output = HtmlEscape(input).to_string();
+        assert_eq!(output, "&lt;&gt;&amp;&quot;&#x27;&#x2f;");
+    }
+
+    #[test]
+    fn test_unescape() {
+        assert_eq!(unescape(r"foo\u2603bar").unwrap(), "foo\u{2603}bar");
+        assert_eq!(unescape(r"\t\b\f\r\n\\\/").unwrap(), "\t\x08\x0c\r\n\\/");
+        assert_eq!(unescape("foobarbaz").unwrap(), "foobarbaz");
+        assert_eq!(unescape(r"\ud83d\udca9").unwrap(), "💩");
+    }
 }
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/value/argtypes.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/value/argtypes.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 use std::borrow::Cow;
 use std::cell::RefCell;
 use std::collections::{BTreeMap, HashMap, HashSet};
 use std::convert::TryFrom;
 use std::ops::{Deref, DerefMut};
 
 use crate::error::{Error, ErrorKind};
-use crate::key::{Key, StaticKey};
 use crate::utils::UndefinedBehavior;
 use crate::value::{
-    Arc, MapType, Object, Packed, SeqObject, StringType, Value, ValueKind, ValueMap, ValueRepr,
+    Arc, KeyRef, MapType, Object, Packed, SeqObject, StringType, Value, ValueKind, ValueMap,
+    ValueRepr,
 };
 use crate::vm::State;
 
 /// A utility trait that represents the return value of functions and filters.
 ///
 /// It's implemented for the following types:
 ///
@@ -59,26 +59,38 @@
 /// Utility function to convert a slice of values into arguments.
 ///
 /// This performs the same conversion that [`Function`](crate::functions::Function)
 /// performs.  It exists so that you one can leverage the same functionality when
 /// implementing [`Object::call_method`](crate::value::Object::call_method).
 ///
 /// ```
-/// use minijinja::value::from_args;
+/// # use minijinja::value::from_args;
 /// # use minijinja::value::Value;
 /// # fn foo() -> Result<(), minijinja::Error> {
 /// # let args = vec![Value::from("foo"), Value::from(42i64)]; let args = &args[..];
-///
 /// // args is &[Value]
 /// let (string, num): (&str, i64) = from_args(args)?;
 /// # Ok(()) } fn main() { foo().unwrap(); }
 /// ```
 ///
 /// Note that only value conversions are supported which means that `&State` is not
 /// a valid conversion type.
+///
+/// You can also use this function to split positional and keyword arguments ([`Kwargs`]):
+///
+/// ```
+/// # use minijinja::value::{Value, Rest, Kwargs, from_args};
+/// # use minijinja::Error;
+/// # fn foo() -> Result<(), minijinja::Error> {
+/// # let args = vec![Value::from("foo"), Value::from(42i64)]; let args = &args[..];
+/// // args is &[Value], kwargs is Kwargs
+/// let (args, kwargs): (&[Value], Kwargs) = from_args(args)?;
+/// # Ok(())
+/// # } fn main() { foo().unwrap(); }
+/// ```
 #[inline(always)]
 pub fn from_args<'a, Args>(values: &'a [Value]) -> Result<Args, Error>
 where
     Args: FunctionArgs<'a, Output = Args>,
 {
     Args::from_values(None, values)
 }
@@ -161,36 +173,63 @@
     fn from_state_and_values(
         state: Option<&'a State>,
         values: &'a [Value],
         offset: usize,
     ) -> Result<(Self::Output, usize), Error> {
         Self::from_state_and_value(state, values.get(offset))
     }
+
+    #[doc(hidden)]
+    #[inline(always)]
+    fn is_trailing() -> bool {
+        false
+    }
 }
 
 macro_rules! tuple_impls {
     ( $( $name:ident )* * $rest_name:ident ) => {
         impl<'a, $($name,)* $rest_name> FunctionArgs<'a> for ($($name,)* $rest_name,)
             where $($name: ArgType<'a>,)* $rest_name: ArgType<'a>
         {
             type Output = ($($name::Output,)* $rest_name::Output ,);
 
-            fn from_values(state: Option<&'a State>, values: &'a [Value]) -> Result<Self::Output, Error> {
+            fn from_values(state: Option<&'a State>, mut values: &'a [Value]) -> Result<Self::Output, Error> {
                 #![allow(non_snake_case, unused)]
+                $( let $name; )*
+                let mut $rest_name = None;
                 let mut idx = 0;
+
+                // special case: the last type is marked trailing (eg: for Kwargs) and we have at
+                // least one value.  In that case we need to read it first before going to the rest
+                // of the arguments.  This is needed to support from_args::<(&[Value], Kwargs)>
+                // or similar.
+                let rest_first = $rest_name::is_trailing() && !values.is_empty();
+                if rest_first {
+                    let (val, offset) = ok!($rest_name::from_state_and_values(state, values, values.len() - 1));
+                    $rest_name = Some(val);
+                    values = &values[..values.len() - offset];
+                }
                 $(
-                    let ($name, offset) = ok!($name::from_state_and_value(state, values.get(idx)));
+                    let (val, offset) = ok!($name::from_state_and_values(state, values, idx));
+                    $name = val;
                     idx += offset;
                 )*
-                let ($rest_name, offset) = ok!($rest_name::from_state_and_values(state, values, idx));
-                idx += offset;
+
+                if !rest_first {
+                    let (val, offset) = ok!($rest_name::from_state_and_values(state, values, idx));
+                    $rest_name = Some(val);
+                    idx += offset;
+                }
+
                 if values.get(idx).is_some() {
                     Err(Error::from(ErrorKind::TooManyArguments))
                 } else {
-                    Ok(( $($name,)* $rest_name,))
+                    // SAFETY: this is safe because both no batter what `rest_first` is set to
+                    // either way the variable is set.
+                    Ok(($($name,)* unsafe { $rest_name.unwrap_unchecked() },))
                 }
             }
         }
     };
 }
 
 impl<'a> FunctionArgs<'a> for () {
@@ -224,22 +263,22 @@
         ValueRepr::Bytes(Arc::new(val.into())).into()
     }
 }
 
 impl<'a> From<&'a str> for Value {
     #[inline(always)]
     fn from(val: &'a str) -> Self {
-        ValueRepr::String(Arc::new(val.into()), StringType::Normal).into()
+        ValueRepr::String(Arc::from(val.to_string()), StringType::Normal).into()
     }
 }
 
 impl From<String> for Value {
     #[inline(always)]
     fn from(val: String) -> Self {
-        ValueRepr::String(Arc::new(val), StringType::Normal).into()
+        ValueRepr::String(Arc::from(val), StringType::Normal).into()
     }
 }
 
 impl<'a> From<Cow<'a, str>> for Value {
     #[inline(always)]
     fn from(val: Cow<'a, str>) -> Self {
         match val {
@@ -252,52 +291,37 @@
 impl From<()> for Value {
     #[inline(always)]
     fn from(_: ()) -> Self {
         ValueRepr::None.into()
     }
 }
 
-impl<'a> From<Key<'a>> for Value {
-    fn from(val: Key) -> Self {
-        match val {
-            Key::Bool(val) => val.into(),
-            Key::I64(val) => val.into(),
-            Key::Char(val) => val.into(),
-            Key::String(val) => ValueRepr::String(val, StringType::Normal).into(),
-            Key::Str(val) => val.into(),
-        }
-    }
-}
-
 impl<V: Into<Value>> FromIterator<V> for Value {
     fn from_iter<T: IntoIterator<Item = V>>(iter: T) -> Self {
-        let vec = iter.into_iter().map(|v| v.into()).collect();
-
-        ValueRepr::Seq(Arc::new(vec)).into()
+        ValueRepr::Seq(Arc::new(iter.into_iter().map(Into::into).collect())).into()
     }
 }
 
-impl<K: Into<StaticKey>, V: Into<Value>> FromIterator<(K, V)> for Value {
+impl<K: Into<Value>, V: Into<Value>> FromIterator<(K, V)> for Value {
     fn from_iter<T: IntoIterator<Item = (K, V)>>(iter: T) -> Self {
         let map = iter
             .into_iter()
-            .map(|(k, v)| (k.into(), v.into()))
+            .map(|(k, v)| (KeyRef::Value(k.into()), v.into()))
             .collect();
-
         ValueRepr::Map(Arc::new(map), MapType::Normal).into()
     }
 }
 
-impl<K: Into<StaticKey>, V: Into<Value>> From<BTreeMap<K, V>> for Value {
+impl<K: Into<Value>, V: Into<Value>> From<BTreeMap<K, V>> for Value {
     fn from(val: BTreeMap<K, V>) -> Self {
         val.into_iter().map(|(k, v)| (k.into(), v.into())).collect()
     }
 }
 
-impl<K: Into<StaticKey>, V: Into<Value>> From<HashMap<K, V>> for Value {
+impl<K: Into<Value>, V: Into<Value>> From<HashMap<K, V>> for Value {
     fn from(val: HashMap<K, V>) -> Self {
         val.into_iter().map(|(k, v)| (k.into(), v.into())).collect()
     }
 }
 
 impl<T: Into<Value>> From<Vec<T>> for Value {
     fn from(val: Vec<T>) -> Self {
@@ -307,16 +331,16 @@
 
 impl<T: Object> From<Arc<T>> for Value {
     fn from(object: Arc<T>) -> Self {
         Value::from(object as Arc<dyn Object>)
     }
 }
 
-impl From<Arc<String>> for Value {
-    fn from(value: Arc<String>) -> Self {
+impl From<Arc<str>> for Value {
+    fn from(value: Arc<str>) -> Self {
         Value(ValueRepr::String(value, StringType::Normal))
     }
 }
 
 macro_rules! value_from {
     ($src:ty, $dst:ident) => {
         impl From<$src> for Value {
@@ -338,26 +362,32 @@
 impl From<u128> for Value {
     #[inline(always)]
     fn from(val: u128) -> Self {
         ValueRepr::U128(Packed(val)).into()
     }
 }
 
+impl From<char> for Value {
+    #[inline(always)]
+    fn from(val: char) -> Self {
+        ValueRepr::String(Arc::from(val.to_string()), StringType::Normal).into()
+    }
+}
+
 value_from!(bool, Bool);
 value_from!(u8, U64);
 value_from!(u16, U64);
 value_from!(u32, U64);
 value_from!(u64, U64);
 value_from!(i8, I64);
 value_from!(i16, I64);
 value_from!(i32, I64);
 value_from!(i64, I64);
 value_from!(f32, F64);
 value_from!(f64, F64);
-value_from!(char, Char);
 value_from!(Arc<Vec<u8>>, Bytes);
 value_from!(Arc<Vec<Value>>, Seq);
 value_from!(Arc<dyn Object>, Dynamic);
 
 fn unsupported_conversion(kind: ValueKind, target: &str) -> Error {
     Error::new(
         ErrorKind::InvalidOperation,
@@ -422,15 +452,20 @@
 primitive_int_try_from!(i128);
 primitive_int_try_from!(usize);
 
 primitive_try_from!(bool, {
     ValueRepr::Bool(val) => val,
 });
 primitive_try_from!(char, {
-    ValueRepr::Char(val) => val,
+    ValueRepr::String(ref val, _) => {
+        let mut char_iter = val.chars();
+        ok!(char_iter.next().filter(|_| char_iter.next().is_none()).ok_or_else(|| {
+            unsupported_conversion(ValueKind::String, "non single character string")
+        }))
+    },
 });
 primitive_try_from!(f32, {
     ValueRepr::U64(val) => val as f32,
     ValueRepr::I64(val) => val as f32,
     ValueRepr::U128(val) => val.0 as f32,
     ValueRepr::I128(val) => val.0 as f32,
     ValueRepr::F64(val) => val as f32,
@@ -510,15 +545,15 @@
 impl<'a> ArgType<'a> for Cow<'_, str> {
     type Output = Cow<'a, str>;
 
     #[inline(always)]
     fn from_value(value: Option<&'a Value>) -> Result<Cow<'a, str>, Error> {
         match value {
             Some(value) => Ok(match value.0 {
-                ValueRepr::String(ref s, _) => Cow::Borrowed(s.as_str()),
+                ValueRepr::String(ref s, _) => Cow::Borrowed(s as &str),
                 _ => Cow::Owned(value.to_string()),
             }),
             None => Err(Error::from(ErrorKind::MissingArgument)),
         }
     }
 }
 
@@ -530,14 +565,35 @@
         match value {
             Some(value) => Ok(value),
             None => Err(Error::from(ErrorKind::MissingArgument)),
         }
     }
 }
 
+impl<'a> ArgType<'a> for &[Value] {
+    type Output = &'a [Value];
+
+    #[inline(always)]
+    fn from_value(value: Option<&'a Value>) -> Result<&'a [Value], Error> {
+        match value {
+            Some(value) => Ok(std::slice::from_ref(value)),
+            None => Err(Error::from(ErrorKind::MissingArgument)),
+        }
+    }
+
+    fn from_state_and_values(
+        _state: Option<&'a State>,
+        values: &'a [Value],
+        offset: usize,
+    ) -> Result<(&'a [Value], usize), Error> {
+        let args = values.get(offset..).unwrap_or_default();
+        Ok((args, args.len()))
+    }
+}
+
 /// Utility type to capture remaining arguments.
 ///
 /// In some cases you might want to have a variadic function.  In that case
 /// you can define the last argument to a [`Filter`](crate::filters::Filter),
 /// [`Test`](crate::tests::Test) or [`Function`](crate::functions::Function)
 /// this way.  The `Rest<T>` type will collect all the remaining arguments
 /// here.  It's implemented for all [`ArgType`]s.  The type itself deref's
@@ -621,15 +677,40 @@
 ///     }
 ///     options.assert_all_used()?;
 ///     Ok(values)
 /// }
 /// ```
 ///
 /// If for whatever reason you need a value again you can use [`Into`] to
-/// convert it back into a [`Value`].
+/// convert it back into a [`Value`].  This is particularly useful when performing
+/// calls into values.  To create a [`Kwargs`] object from scratch you can use
+/// [`FromIterator`]:
+///
+/// ```
+/// use minijinja::value::{Value, Kwargs};
+/// let kwargs = Kwargs::from_iter([
+///     ("foo", Value::from(true)),
+///     ("bar", Value::from(42)),
+/// ]);
+/// let value = Value::from(kwargs);
+/// assert!(value.is_kwargs());
+/// ```
+///
+/// When working with [`Rest`] you can use [`from_args`] to split all arguments into
+/// positional arguments and keyword arguments:
+///
+/// ```
+/// # use minijinja::value::{Value, Rest, Kwargs, from_args};
+/// # use minijinja::Error;
+/// fn my_func(args: Rest<Value>) -> Result<Value, Error> {
+///     let (args, kwargs) = from_args::<(&[Value], Kwargs)>(&args)?;
+///     // do something with args and kwargs
+/// # todo!()
+/// }
+/// ```
 #[derive(Debug, Clone)]
 pub struct Kwargs {
     values: Arc<ValueMap>,
     used: RefCell<HashSet<String>>,
 }
 
 impl<'a> ArgType<'a> for Kwargs {
@@ -656,51 +737,34 @@
         if let Some(value) = values.get(offset) {
             if let ValueRepr::Map(ref map, MapType::Kwargs) = value.0 {
                 return Ok((Kwargs::new(map.clone()), 1));
             }
         }
         Ok((Kwargs::new(Default::default()), 0))
     }
+
+    fn is_trailing() -> bool {
+        true
+    }
 }
 
 impl Kwargs {
     fn new(map: Arc<ValueMap>) -> Kwargs {
         Kwargs {
             values: map,
             used: RefCell::new(HashSet::new()),
         }
     }
 
-    /// Split off kwargs from args.
-    ///
-    /// This is useful when [`Rest`] is used to consume all arguments:
-    ///
-    /// ```rust
-    /// # use minijinja::value::{Value, Rest, Kwargs};
-    /// fn my_func(args: Rest<Value>) -> Value {
-    ///     let (args, kwargs) = Kwargs::from_args(&args);
-    ///     // do something with args and kwargs
-    /// # todo!()
-    /// }
-    /// ```
-    pub fn from_args(args: &[Value]) -> (&[Value], Kwargs) {
-        if let Some(value) = args.last() {
-            if let ValueRepr::Map(ref map, MapType::Kwargs) = value.0 {
-                return (&args[..args.len() - 1], Kwargs::new(map.clone()));
-            }
-        }
-        (args, Kwargs::new(Default::default()))
-    }
-
     /// Get a single argument from the kwargs but don't mark it as used.
     pub fn peek<'a, T>(&'a self, key: &'a str) -> Result<T, Error>
     where
         T: ArgType<'a, Output = T>,
     {
-        T::from_value(self.values.get(&Key::Str(key)))
+        T::from_value(self.values.get(&KeyRef::Str(key)))
     }
 
     /// Gets a single argument from the kwargs and marks it as used.
     ///
     /// This method works pretty much like [`from_args`] and marks any parameter
     /// used internally.  For optional arguments you would typically use
     /// `Option<T>` and for non optional ones directly `T`.
@@ -727,15 +791,15 @@
         let rv = ok!(self.peek::<T>(key));
         self.used.borrow_mut().insert(key.to_string());
         Ok(rv)
     }
 
     /// Checks if a keyword argument exists.
     pub fn has(&self, key: &str) -> bool {
-        self.values.contains_key(&Key::Str(key))
+        self.values.contains_key(&KeyRef::Str(key))
     }
 
     /// Iterates over all passed keyword arguments.
     pub fn args(&self) -> impl Iterator<Item = &str> {
         self.values.iter().filter_map(|x| x.0.as_str())
     }
 
@@ -757,14 +821,40 @@
                 ));
             }
         }
         Ok(())
     }
 }
 
+impl FromIterator<(String, Value)> for Kwargs {
+    fn from_iter<T>(iter: T) -> Self
+    where
+        T: IntoIterator<Item = (String, Value)>,
+    {
+        Kwargs::new(Arc::new(
+            iter.into_iter()
+                .map(|(k, v)| (KeyRef::Value(Value::from(k)), v))
+                .collect(),
+        ))
+    }
+}
+
+impl<'a> FromIterator<(&'a str, Value)> for Kwargs {
+    fn from_iter<T>(iter: T) -> Self
+    where
+        T: IntoIterator<Item = (&'a str, Value)>,
+    {
+        Kwargs::new(Arc::new(
+            iter.into_iter()
+                .map(|(k, v)| (KeyRef::Value(Value::from(k)), v))
+                .collect(),
+        ))
+    }
+}
+
 impl From<Kwargs> for Value {
     fn from(value: Kwargs) -> Self {
         Value(ValueRepr::Map(value.values, MapType::Kwargs))
     }
 }
 
 impl TryFrom<Value> for Kwargs {
@@ -855,16 +945,37 @@
 
 impl From<usize> for Value {
     fn from(val: usize) -> Self {
         Value::from(val as u64)
     }
 }
 
-#[test]
-fn test_as_f64() {
-    let v = Value::from(42u32);
-    let f: f64 = v.try_into().unwrap();
-    assert_eq!(f, 42.0);
-    let v = Value::from(42.5);
-    let f: f64 = v.try_into().unwrap();
-    assert_eq!(f, 42.5);
+#[cfg(test)]
+mod tests {
+    use super::*;
+
+    #[test]
+    fn test_as_f64() {
+        let v = Value::from(42u32);
+        let f: f64 = v.try_into().unwrap();
+        assert_eq!(f, 42.0);
+        let v = Value::from(42.5);
+        let f: f64 = v.try_into().unwrap();
+        assert_eq!(f, 42.5);
+    }
+
+    #[test]
+    fn test_split_kwargs() {
+        let args = [
+            Value::from(42),
+            Value::from(true),
+            Value::from(Kwargs::from_iter([
+                ("foo", Value::from(1)),
+                ("bar", Value::from(2)),
+            ])),
+        ];
+        let (args, kwargs) = from_args::<(&[Value], Kwargs)>(&args).unwrap();
+        assert_eq!(args, &[Value::from(42), Value::from(true)]);
+        assert_eq!(kwargs.get::<Value>("foo").unwrap(), Value::from(1));
+        assert_eq!(kwargs.get::<Value>("bar").unwrap(), Value::from(2));
+    }
 }
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/value/deserialize.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/value/deserialize.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use serde::de::{self, MapAccess, SeqAccess, Visitor};
 use serde::Deserialize;
 
-use crate::value::{MapType, Value, ValueMap, ValueRepr};
+use crate::value::{KeyRef, MapType, Value, ValueMap, ValueRepr};
 
 impl<'de> Deserialize<'de> for Value {
     fn deserialize<D>(deserializer: D) -> Result<Self, D::Error>
     where
         D: serde::Deserializer<'de>,
     {
         let visitor = ValueVisitor;
@@ -92,12 +92,12 @@
 
     fn visit_map<A>(self, mut map: A) -> Result<Self::Value, A::Error>
     where
         A: MapAccess<'de>,
     {
         let mut rv = ValueMap::default();
         while let Some((k, v)) = ok!(map.next_entry()) {
-            rv.insert(k, v);
+            rv.insert(KeyRef::Value(k), v);
         }
         Ok(Value(ValueRepr::Map(rv.into(), MapType::Normal)))
     }
 }
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/value/mod.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/value/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,34 @@
 //!
 //! # Converting Values
 //!
 //! Values are typically created via the [`From`] trait:
 //!
 //! ```
 //! # use minijinja::value::Value;
-//! let value = Value::from(42);
+//! let int_value = Value::from(42);
+//! let none_value = Value::from(());
+//! let true_value = Value::from(true);
 //! ```
 //!
 //! Or via the [`FromIterator`] trait:
 //!
 //! ```
 //! # use minijinja::value::Value;
 //! // collection into a sequence
 //! let value: Value = (1..10).into_iter().collect();
 //!
 //! // collection into a map
 //! let value: Value = [("key", "value")].into_iter().collect();
 //! ```
 //!
+//! The special [`Undefined`](Value::UNDEFINED) value also exists but does not
+//! have a rust equivalent.  It can be created via the [`UNDEFINED`](Value::UNDEFINED)
+//! constant.
+//!
 //! MiniJinja will however create values via an indirection via [`serde`] when
 //! a template is rendered or an expression is evaluated.  This can also be
 //! triggered manually by using the [`Value::from_serializable`] method:
 //!
 //! ```
 //! # use minijinja::value::Value;
 //! let value = Value::from_serializable(&[1, 2, 3]);
@@ -102,60 +108,61 @@
 // on the content module in serde::private::ser.
 
 use std::cell::{Cell, RefCell};
 use std::cmp::Ordering;
 use std::collections::BTreeMap;
 use std::convert::TryFrom;
 use std::fmt;
+use std::hash::{Hash, Hasher};
 use std::marker::PhantomData;
 use std::sync::Arc;
 
 use serde::ser::{Serialize, Serializer};
 
 use crate::error::{Error, ErrorKind};
 use crate::functions;
-use crate::key::{Key, StaticKey};
 use crate::utils::OnDrop;
 use crate::value::object::{SimpleSeqObject, SimpleStructObject};
+use crate::value::ops::as_f64;
 use crate::value::serialize::transform;
 use crate::vm::State;
 
 pub use crate::value::argtypes::{from_args, ArgType, FunctionArgs, FunctionResult, Kwargs, Rest};
 pub use crate::value::object::{Object, ObjectKind, SeqObject, SeqObjectIter, StructObject};
 
 mod argtypes;
 #[cfg(feature = "deserialization")]
 mod deserialize;
+mod keyref;
 mod object;
 pub(crate) mod ops;
 mod serialize;
 
-#[cfg(test)]
-use similar_asserts::assert_eq;
+pub(crate) use crate::value::keyref::KeyRef;
 
 // We use in-band signalling to roundtrip some internal values.  This is
 // not ideal but unfortunately there is no better system in serde today.
 const VALUE_HANDLE_MARKER: &str = "\x01__minijinja_ValueHandle";
 
 #[cfg(feature = "preserve_order")]
-pub(crate) type ValueMap = indexmap::IndexMap<StaticKey, Value>;
+pub(crate) type ValueMap = indexmap::IndexMap<KeyRef<'static>, Value>;
 
 #[cfg(not(feature = "preserve_order"))]
-pub(crate) type ValueMap = std::collections::BTreeMap<StaticKey, Value>;
+pub(crate) type ValueMap = std::collections::BTreeMap<KeyRef<'static>, Value>;
 
 #[inline(always)]
 pub(crate) fn value_map_with_capacity(capacity: usize) -> ValueMap {
     #[cfg(not(feature = "preserve_order"))]
     {
         let _ = capacity;
         ValueMap::new()
     }
     #[cfg(feature = "preserve_order")]
     {
-        ValueMap::with_capacity(capacity)
+        ValueMap::with_capacity(crate::utils::untrusted_size_hint(capacity))
     }
 }
 
 thread_local! {
     static INTERNAL_SERIALIZATION: Cell<bool> = Cell::new(false);
 
     // This should be an AtomicU64 but sadly 32bit targets do not necessarily have
@@ -180,24 +187,28 @@
 /// support deserialization.  So it becomes possible to completely change what
 /// gets sent there, even at the cost of serializing something that cannot be
 /// deserialized.
 pub fn serializing_for_value() -> bool {
     INTERNAL_SERIALIZATION.with(|flag| flag.get())
 }
 
-/// When key interning is enabled while the returned token is held keys are
-/// interned in a map, freed at the end of the section.
-#[cfg(feature = "key_interning")]
-pub(crate) use crate::key::key_interning::use_string_cache as value_optimization;
-
-/// Without key interning this is a dummy drop.
-#[cfg(not(feature = "key_interning"))]
+/// Enables value optimizations.
+///
+/// If `key_interning` is enabled, this turns on that feature, otherwise
+/// it becomes a noop.
 #[inline(always)]
 pub(crate) fn value_optimization() -> impl Drop {
-    OnDrop::new(|| {})
+    #[cfg(feature = "key_interning")]
+    {
+        crate::value::keyref::key_interning::use_string_cache()
+    }
+    #[cfg(not(feature = "key_interning"))]
+    {
+        OnDrop::new(|| {})
+    }
 }
 
 fn mark_internal_serialization() -> impl Drop {
     let old = INTERNAL_SERIALIZATION.with(|flag| {
         let old = flag.get();
         flag.set(true);
         old
@@ -216,40 +227,36 @@
     Undefined,
     /// The value is the none singleton ([`()`])
     None,
     /// The value is a [`bool`]
     Bool,
     /// The value is a number of a supported type.
     Number,
-    /// The value is a character.
-    Char,
     /// The value is a string.
     String,
     /// The value is a byte array.
     Bytes,
     /// The value is an array of other values.
     Seq,
     /// The value is a key/value mapping.
     Map,
 }
 
 impl fmt::Display for ValueKind {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        let ty = match *self {
+        f.write_str(match *self {
             ValueKind::Undefined => "undefined",
             ValueKind::None => "none",
             ValueKind::Bool => "bool",
             ValueKind::Number => "number",
-            ValueKind::Char => "char",
             ValueKind::String => "string",
             ValueKind::Bytes => "bytes",
             ValueKind::Seq => "sequence",
             ValueKind::Map => "map",
-        };
-        write!(f, "{ty}")
+        })
     }
 }
 
 /// The type of map
 #[derive(Copy, Clone, Debug)]
 pub(crate) enum MapType {
     /// A regular map
@@ -282,48 +289,91 @@
 #[derive(Clone)]
 pub(crate) enum ValueRepr {
     Undefined,
     Bool(bool),
     U64(u64),
     I64(i64),
     F64(f64),
-    Char(char),
     None,
-    Invalid(Arc<String>),
+    Invalid(Arc<str>),
     U128(Packed<u128>),
     I128(Packed<i128>),
-    String(Arc<String>, StringType),
+    String(Arc<str>, StringType),
     Bytes(Arc<Vec<u8>>),
     Seq(Arc<Vec<Value>>),
     Map(Arc<ValueMap>, MapType),
     Dynamic(Arc<dyn Object>),
 }
 
 impl fmt::Debug for ValueRepr {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         match self {
-            ValueRepr::Undefined => write!(f, "Undefined"),
+            ValueRepr::Undefined => f.write_str("Undefined"),
             ValueRepr::Bool(val) => fmt::Debug::fmt(val, f),
             ValueRepr::U64(val) => fmt::Debug::fmt(val, f),
             ValueRepr::I64(val) => fmt::Debug::fmt(val, f),
             ValueRepr::F64(val) => fmt::Debug::fmt(val, f),
-            ValueRepr::Char(val) => fmt::Debug::fmt(val, f),
-            ValueRepr::None => write!(f, "None"),
+            ValueRepr::None => f.write_str("None"),
             ValueRepr::Invalid(ref val) => write!(f, "<invalid value: {}>", val),
             ValueRepr::U128(val) => fmt::Debug::fmt(&{ val.0 }, f),
             ValueRepr::I128(val) => fmt::Debug::fmt(&{ val.0 }, f),
             ValueRepr::String(val, _) => fmt::Debug::fmt(val, f),
             ValueRepr::Bytes(val) => fmt::Debug::fmt(val, f),
             ValueRepr::Seq(val) => fmt::Debug::fmt(val, f),
             ValueRepr::Map(val, _) => fmt::Debug::fmt(val, f),
             ValueRepr::Dynamic(val) => fmt::Debug::fmt(val, f),
         }
     }
 }
 
+impl Hash for Value {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        match &self.0 {
+            ValueRepr::None | ValueRepr::Undefined => 0u8.hash(state),
+            ValueRepr::String(ref s, _) => s.hash(state),
+            ValueRepr::Bool(b) => b.hash(state),
+            ValueRepr::Invalid(s) => s.hash(state),
+            ValueRepr::Bytes(b) => b.hash(state),
+            ValueRepr::Seq(b) => b.hash(state),
+            ValueRepr::Map(m, _) => m.iter().for_each(|(k, v)| {
+                k.hash(state);
+                v.hash(state);
+            }),
+            ValueRepr::Dynamic(d) => match d.kind() {
+                ObjectKind::Plain => 0u8.hash(state),
+                ObjectKind::Seq(s) => s.iter().for_each(|x| x.hash(state)),
+                ObjectKind::Struct(s) => {
+                    if let Some(fields) = s.static_fields() {
+                        fields.iter().for_each(|k| {
+                            k.hash(state);
+                            s.get_field(k).hash(state);
+                        });
+                    } else {
+                        s.fields().iter().for_each(|k| {
+                            k.hash(state);
+                            s.get_field(k).hash(state);
+                        });
+                    }
+                }
+            },
+            ValueRepr::U64(_)
+            | ValueRepr::I64(_)
+            | ValueRepr::F64(_)
+            | ValueRepr::U128(_)
+            | ValueRepr::I128(_) => {
+                if let Ok(val) = i64::try_from(self.clone()) {
+                    val.hash(state)
+                } else {
+                    as_f64(self).map(|x| x.to_bits()).hash(state)
+                }
+            }
+        }
+    }
+}
+
 /// Represents a dynamically typed value in the template engine.
 #[derive(Clone)]
 pub struct Value(pub(crate) ValueRepr);
 
 impl PartialEq for Value {
     fn eq(&self, other: &Self) -> bool {
         match (&self.0, &other.0) {
@@ -334,92 +384,130 @@
             _ => match ops::coerce(self, other) {
                 Some(ops::CoerceResult::F64(a, b)) => a == b,
                 Some(ops::CoerceResult::I128(a, b)) => a == b,
                 Some(ops::CoerceResult::Str(a, b)) => a == b,
                 None => {
                     if let (Some(a), Some(b)) = (self.as_seq(), other.as_seq()) {
                         a.iter().eq(b.iter())
+                    } else if self.kind() == ValueKind::Map && other.kind() == ValueKind::Map {
+                        if self.len() != other.len() {
+                            return false;
+                        }
+                        if let Ok(mut iter) = self.try_iter() {
+                            iter.all(|x| self.get_item_opt(&x) == other.get_item_opt(&x))
+                        } else {
+                            false
+                        }
                     } else {
                         false
                     }
                 }
             },
         }
     }
 }
 
 impl Eq for Value {}
 
 impl PartialOrd for Value {
     fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
-        match (&self.0, &other.0) {
-            (ValueRepr::None, ValueRepr::None) => Some(Ordering::Equal),
-            (ValueRepr::Undefined, ValueRepr::Undefined) => Some(Ordering::Equal),
-            (ValueRepr::Bytes(a), ValueRepr::Bytes(b)) => a.partial_cmp(b),
+        Some(self.cmp(other))
+    }
+}
+
+fn f64_total_cmp(left: f64, right: f64) -> Ordering {
+    // this is taken from f64::total_cmp on newer rust versions
+    let mut left = left.to_bits() as i64;
+    let mut right = right.to_bits() as i64;
+    left ^= (((left >> 63) as u64) >> 1) as i64;
+    right ^= (((right >> 63) as u64) >> 1) as i64;
+    left.cmp(&right)
+}
+
+impl Ord for Value {
+    fn cmp(&self, other: &Self) -> Ordering {
+        let value_ordering = match (&self.0, &other.0) {
+            (ValueRepr::None, ValueRepr::None) => Ordering::Equal,
+            (ValueRepr::Undefined, ValueRepr::Undefined) => Ordering::Equal,
+            (ValueRepr::String(ref a, _), ValueRepr::String(ref b, _)) => a.cmp(b),
+            (ValueRepr::Bytes(a), ValueRepr::Bytes(b)) => a.cmp(b),
             _ => match ops::coerce(self, other) {
-                Some(ops::CoerceResult::F64(a, b)) => a.partial_cmp(&b),
-                Some(ops::CoerceResult::I128(a, b)) => a.partial_cmp(&b),
-                Some(ops::CoerceResult::Str(a, b)) => a.partial_cmp(b),
-                None => None,
+                Some(ops::CoerceResult::F64(a, b)) => f64_total_cmp(a, b),
+                Some(ops::CoerceResult::I128(a, b)) => a.cmp(&b),
+                Some(ops::CoerceResult::Str(a, b)) => a.cmp(b),
+                None => {
+                    if let (Some(a), Some(b)) = (self.as_seq(), other.as_seq()) {
+                        a.iter().cmp(b.iter())
+                    } else if self.kind() == ValueKind::Map && other.kind() == ValueKind::Map {
+                        if let (Ok(a), Ok(b)) = (self.try_iter(), other.try_iter()) {
+                            a.map(|k| (k.clone(), self.get_item_opt(&k)))
+                                .cmp(b.map(|k| (k.clone(), other.get_item_opt(&k))))
+                        } else {
+                            Ordering::Equal
+                        }
+                    } else {
+                        Ordering::Equal
+                    }
+                }
             },
-        }
+        };
+        value_ordering.then((self.kind() as usize).cmp(&(other.kind() as usize)))
     }
 }
 
 impl fmt::Debug for Value {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> Result<(), std::fmt::Error> {
         fmt::Debug::fmt(&self.0, f)
     }
 }
 
 impl fmt::Display for Value {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         match &self.0 {
             ValueRepr::Undefined => Ok(()),
-            ValueRepr::Bool(val) => write!(f, "{val}"),
-            ValueRepr::U64(val) => write!(f, "{val}"),
-            ValueRepr::I64(val) => write!(f, "{val}"),
+            ValueRepr::Bool(val) => val.fmt(f),
+            ValueRepr::U64(val) => val.fmt(f),
+            ValueRepr::I64(val) => val.fmt(f),
             ValueRepr::F64(val) => {
                 if val.is_nan() {
-                    write!(f, "NaN")
+                    f.write_str("NaN")
                 } else if val.is_infinite() {
                     write!(f, "{}inf", if val.is_sign_negative() { "-" } else { "" })
                 } else {
                     let mut num = val.to_string();
                     if !num.contains('.') {
                         num.push_str(".0");
                     }
                     write!(f, "{num}")
                 }
             }
-            ValueRepr::Char(val) => write!(f, "{val}"),
-            ValueRepr::None => write!(f, "none"),
+            ValueRepr::None => f.write_str("none"),
             ValueRepr::Invalid(ref val) => write!(f, "<invalid value: {}>", val),
             ValueRepr::I128(val) => write!(f, "{}", { val.0 }),
             ValueRepr::String(val, _) => write!(f, "{val}"),
             ValueRepr::Bytes(val) => write!(f, "{}", String::from_utf8_lossy(val)),
             ValueRepr::Seq(values) => {
-                ok!(write!(f, "["));
+                ok!(f.write_str("["));
                 for (idx, val) in values.iter().enumerate() {
                     if idx > 0 {
-                        ok!(write!(f, ", "));
+                        ok!(f.write_str(", "));
                     }
                     ok!(write!(f, "{val:?}"));
                 }
-                write!(f, "]")
+                f.write_str("]")
             }
             ValueRepr::Map(m, _) => {
-                ok!(write!(f, "{{"));
+                ok!(f.write_str("{"));
                 for (idx, (key, val)) in m.iter().enumerate() {
                     if idx > 0 {
-                        ok!(write!(f, ", "));
+                        ok!(f.write_str(", "));
                     }
                     ok!(write!(f, "{key:?}: {val:?}"));
                 }
-                write!(f, "}}")
+                f.write_str("}")
             }
             ValueRepr::U128(val) => write!(f, "{}", { val.0 }),
             ValueRepr::Dynamic(x) => write!(f, "{x}"),
         }
     }
 }
 
@@ -432,30 +520,31 @@
 /// Intern a string.
 ///
 /// When the `key_interning` feature is in used, then MiniJinja will attempt to
 /// reuse strings in certain cases.  This function can be used to utilize the
 /// same functionality.  There is no guarantee that a string will be interned
 /// as there are heuristics involved for it.  Additionally the string interning
 /// will only work during the template engine execution (eg: within filters etc.).
-///
-/// ```
-/// use minijinja::value::{intern, Value};
-/// let val = Value::from(intern("my_key"));
-/// ```
-pub fn intern(s: &str) -> Arc<String> {
-    if let Key::String(ref s) = Key::make_string_key(s) {
-        s.clone()
-    } else {
-        unreachable!()
+pub fn intern(s: &str) -> Arc<str> {
+    #[cfg(feature = "key_interning")]
+    {
+        crate::value::keyref::key_interning::try_intern(s)
+    }
+    #[cfg(not(feature = "key_interning"))]
+    {
+        Arc::from(s.to_string())
     }
 }
 
 #[allow(clippy::len_without_is_empty)]
 impl Value {
-    /// The undefined value
+    /// The undefined value.
+    ///
+    /// This constant exists because the undefined type does not exist in Rust
+    /// and this is the only way to construct it.
     pub const UNDEFINED: Value = Value(ValueRepr::Undefined);
 
     /// Creates a value from something that can be serialized.
     ///
     /// This is the method that MiniJinja will generally use whenever a serializable
     /// object is passed to one of the APIs that internally want to create a value.
     /// For instance this is what [`context!`](crate::context) and
@@ -490,15 +579,15 @@
     /// supply the `|safe` filter, you can use a value of this type instead.
     ///
     /// ```
     /// # use minijinja::value::Value;
     /// let val = Value::from_safe_string("<em>note</em>".into());
     /// ```
     pub fn from_safe_string(value: String) -> Value {
-        ValueRepr::String(Arc::new(value), StringType::Safe).into()
+        ValueRepr::String(Arc::from(value), StringType::Safe).into()
     }
 
     /// Creates a value from a dynamic object.
     ///
     /// For more information see [`Object`].
     ///
     /// ```rust
@@ -585,15 +674,14 @@
     /// This can be used to determine what's in the value before trying to
     /// perform operations on it.
     pub fn kind(&self) -> ValueKind {
         match self.0 {
             ValueRepr::Undefined => ValueKind::Undefined,
             ValueRepr::Bool(_) => ValueKind::Bool,
             ValueRepr::U64(_) | ValueRepr::I64(_) | ValueRepr::F64(_) => ValueKind::Number,
-            ValueRepr::Char(_) => ValueKind::Char,
             ValueRepr::None => ValueKind::None,
             ValueRepr::I128(_) => ValueKind::Number,
             ValueRepr::String(..) => ValueKind::String,
             ValueRepr::Bytes(_) => ValueKind::Bytes,
             ValueRepr::U128(_) => ValueKind::Number,
             ValueRepr::Seq(_) => ValueKind::Seq,
             ValueRepr::Map(..) => ValueKind::Map,
@@ -632,15 +720,14 @@
         match self.0 {
             ValueRepr::Bool(val) => val,
             ValueRepr::U64(x) => x != 0,
             ValueRepr::U128(x) => x.0 != 0,
             ValueRepr::I64(x) => x != 0,
             ValueRepr::I128(x) => x.0 != 0,
             ValueRepr::F64(x) => x != 0.0,
-            ValueRepr::Char(x) => x != '\x00',
             ValueRepr::String(ref x, _) => !x.is_empty(),
             ValueRepr::Bytes(ref x) => !x.is_empty(),
             ValueRepr::None | ValueRepr::Undefined | ValueRepr::Invalid(_) => false,
             ValueRepr::Seq(ref x) => !x.is_empty(),
             ValueRepr::Map(ref x, _) => !x.is_empty(),
             ValueRepr::Dynamic(ref x) => match x.kind() {
                 ObjectKind::Plain => true,
@@ -664,15 +751,15 @@
     pub fn is_none(&self) -> bool {
         matches!(&self.0, ValueRepr::None)
     }
 
     /// If the value is a string, return it.
     pub fn as_str(&self) -> Option<&str> {
         match &self.0 {
-            ValueRepr::String(ref s, _) => Some(s.as_str()),
+            ValueRepr::String(ref s, _) => Some(s as &str),
             _ => None,
         }
     }
 
     /// Returns the bytes of this value if they exist.
     pub fn as_bytes(&self) -> Option<&[u8]> {
         match &self.0 {
@@ -752,15 +839,15 @@
     /// let value = ctx.get_attr("foo")?;
     /// assert_eq!(value.to_string(), "Foo");
     /// # Ok(()) }
     /// ```
     pub fn get_attr(&self, key: &str) -> Result<Value, Error> {
         Ok(match self.0 {
             ValueRepr::Undefined => return Err(Error::from(ErrorKind::UndefinedError)),
-            ValueRepr::Map(ref items, _) => items.get(&Key::Str(key)).cloned(),
+            ValueRepr::Map(ref items, _) => items.get(&KeyRef::Str(key)).cloned(),
             ValueRepr::Dynamic(ref dy) => match dy.kind() {
                 ObjectKind::Struct(s) => s.get_field(key),
                 ObjectKind::Plain | ObjectKind::Seq(_) => None,
             },
             _ => None,
         }
         .unwrap_or(Value::UNDEFINED))
@@ -770,15 +857,15 @@
     /// resolution.
     ///
     /// The main difference is that the return value will be `None` if the value is
     /// unable to look up the key rather than returning `Undefined` and errors will
     /// also not be created.
     pub(crate) fn get_attr_fast(&self, key: &str) -> Option<Value> {
         match self.0 {
-            ValueRepr::Map(ref items, _) => items.get(&Key::Str(key)).cloned(),
+            ValueRepr::Map(ref items, _) => items.get(&KeyRef::Str(key)).cloned(),
             ValueRepr::Dynamic(ref dy) => match dy.kind() {
                 ObjectKind::Struct(s) => s.get_field(key),
                 ObjectKind::Plain | ObjectKind::Seq(_) => None,
             },
             _ => None,
         }
     }
@@ -881,97 +968,122 @@
     /// assert_eq!(thing.id, 42);
     /// ```
     pub fn downcast_object_ref<T: Object>(&self) -> Option<&T> {
         self.as_object().and_then(|x| x.downcast_ref())
     }
 
     pub(crate) fn get_item_opt(&self, key: &Value) -> Option<Value> {
-        let key = some!(Key::from_borrowed_value(key).ok());
+        let key = KeyRef::Value(key.clone());
 
         let seq = match self.0 {
             ValueRepr::Map(ref items, _) => return items.get(&key).cloned(),
             ValueRepr::Seq(ref items) => &**items as &dyn SeqObject,
             ValueRepr::Dynamic(ref dy) => match dy.kind() {
                 ObjectKind::Plain => return None,
                 ObjectKind::Seq(s) => s,
-                ObjectKind::Struct(s) => match key {
-                    Key::String(ref key) => return s.get_field(key),
-                    Key::Str(key) => return s.get_field(key),
-                    _ => return None,
-                },
+                ObjectKind::Struct(s) => {
+                    return if let Some(key) = key.as_str() {
+                        s.get_field(key)
+                    } else {
+                        None
+                    };
+                }
             },
+            ValueRepr::String(ref s, _) => {
+                if let Some(idx) = key.as_i64() {
+                    let idx = some!(isize::try_from(idx).ok());
+                    let idx = if idx < 0 {
+                        some!(s.chars().count().checked_sub(-idx as usize))
+                    } else {
+                        idx as usize
+                    };
+                    return s.chars().nth(idx).map(Value::from);
+                } else {
+                    return None;
+                }
+            }
             _ => return None,
         };
 
-        if let Key::I64(idx) = key {
+        if let Some(idx) = key.as_i64() {
             let idx = some!(isize::try_from(idx).ok());
             let idx = if idx < 0 {
                 some!(seq.item_count().checked_sub(-idx as usize))
             } else {
                 idx as usize
             };
             seq.get_item(idx)
         } else {
             None
         }
     }
 
     /// Calls the value directly.
-    pub(crate) fn call(&self, state: &State, args: &[Value]) -> Result<Value, Error> {
+    ///
+    /// If the value holds a function or macro, this invokes it.  Note that in
+    /// MiniJinja there is a separate namespace for methods on objects and callable
+    /// items.  To call methods (which should be a rather rare occurrence) you
+    /// have to use [`call_method`](Self::call_method).
+    ///
+    /// The `args` slice is for the arguments of the function call.  To pass
+    /// keyword arguments use the [`Kwargs`](crate::value::Kwargs) type.
+    ///
+    /// Usually the state is already available when it's useful to call this method,
+    /// but when it's not available you can get a fresh template state straight
+    /// from the [`Template`](crate::Template) via [`new_state`](crate::Template::new_state).
+    ///
+    /// ```
+    /// # use minijinja::{Environment, value::{Value, Kwargs}};
+    /// # let mut env = Environment::new();
+    /// # env.add_template("foo", "").unwrap();
+    /// # let tmpl = env.get_template("foo").unwrap();
+    /// # let state = tmpl.new_state(); let state = &state;
+    /// let func = Value::from_function(|v: i64, kwargs: Kwargs| {
+    ///     v * kwargs.get::<i64>("mult").unwrap_or(1)
+    /// });
+    /// let rv = func.call(
+    ///     state,
+    ///     &[
+    ///         Value::from(42),
+    ///         Value::from(Kwargs::from_iter([("mult", Value::from(2))])),
+    ///     ],
+    /// ).unwrap();
+    /// assert_eq!(rv, Value::from(84));
+    /// ```
+    pub fn call(&self, state: &State, args: &[Value]) -> Result<Value, Error> {
         if let ValueRepr::Dynamic(ref dy) = self.0 {
             dy.call(state, args)
         } else {
             Err(Error::new(
                 ErrorKind::InvalidOperation,
                 format!("value of type {} is not callable", self.kind()),
             ))
         }
     }
 
     /// Calls a method on the value.
-    pub(crate) fn call_method(
-        &self,
-        state: &State,
-        name: &str,
-        args: &[Value],
-    ) -> Result<Value, Error> {
+    ///
+    /// The name of the method is `name`, the arguments passed are in the `args`
+    /// slice.
+    pub fn call_method(&self, state: &State, name: &str, args: &[Value]) -> Result<Value, Error> {
         match self.0 {
             ValueRepr::Dynamic(ref dy) => return dy.call_method(state, name, args),
             ValueRepr::Map(ref map, _) => {
-                if let Some(value) = map.get(&Key::Str(name)) {
+                if let Some(value) = map.get(&KeyRef::Str(name)) {
                     return value.call(state, args);
                 }
             }
             _ => {}
         }
         Err(Error::new(
             ErrorKind::InvalidOperation,
             format!("object has no method named {name}"),
         ))
     }
 
-    pub(crate) fn try_into_key(self) -> Result<StaticKey, Error> {
-        match self.0 {
-            ValueRepr::Bool(val) => Ok(Key::Bool(val)),
-            ValueRepr::U64(v) => TryFrom::try_from(v)
-                .map(Key::I64)
-                .map_err(|_| ErrorKind::NonKey.into()),
-            ValueRepr::U128(v) => TryFrom::try_from(v.0)
-                .map(Key::I64)
-                .map_err(|_| ErrorKind::NonKey.into()),
-            ValueRepr::I64(v) => Ok(Key::I64(v)),
-            ValueRepr::I128(v) => TryFrom::try_from(v.0)
-                .map(Key::I64)
-                .map_err(|_| ErrorKind::NonKey.into()),
-            ValueRepr::Char(c) => Ok(Key::Char(c)),
-            ValueRepr::String(ref s, _) => Ok(Key::String(s.clone())),
-            _ => Err(ErrorKind::NonKey.into()),
-        }
-    }
-
     /// Iterates over the value without holding a reference.
     pub(crate) fn try_iter_owned(&self) -> Result<OwnedValueIterator, Error> {
         let (iter_state, len) = match self.0 {
             ValueRepr::None | ValueRepr::Undefined => (ValueIteratorState::Empty, 0),
             ValueRepr::String(ref s, _) => (
                 ValueIteratorState::Chars(0, Arc::clone(s)),
                 s.chars().count(),
@@ -1059,15 +1171,14 @@
         }
 
         match self.0 {
             ValueRepr::Bool(b) => serializer.serialize_bool(b),
             ValueRepr::U64(u) => serializer.serialize_u64(u),
             ValueRepr::I64(i) => serializer.serialize_i64(i),
             ValueRepr::F64(f) => serializer.serialize_f64(f),
-            ValueRepr::Char(c) => serializer.serialize_char(c),
             ValueRepr::None | ValueRepr::Undefined | ValueRepr::Invalid(_) => {
                 serializer.serialize_unit()
             }
             ValueRepr::U128(u) => serializer.serialize_u128(u.0),
             ValueRepr::I128(i) => serializer.serialize_i128(i.0),
             ValueRepr::String(ref s, _) => serializer.serialize_str(s),
             ValueRepr::Bytes(ref b) => serializer.serialize_bytes(b),
@@ -1097,15 +1208,15 @@
                         for k in fields {
                             let v = s.get_field(k).unwrap_or(Value::UNDEFINED);
                             ok!(map.serialize_entry(k, &v));
                         }
                     } else {
                         for k in s.fields() {
                             let v = s.get_field(&k).unwrap_or(Value::UNDEFINED);
-                            ok!(map.serialize_entry(k.as_str(), &v));
+                            ok!(map.serialize_entry(&*k as &str, &v));
                         }
                     }
                     map.end()
                 }
             },
         }
     }
@@ -1152,31 +1263,31 @@
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         f.debug_struct("ValueIterator").finish()
     }
 }
 
 enum ValueIteratorState {
     Empty,
-    Chars(usize, Arc<String>),
+    Chars(usize, Arc<str>),
     Seq(usize, Arc<Vec<Value>>),
     StaticStr(usize, &'static [&'static str]),
-    ArcStr(usize, Vec<Arc<String>>),
+    ArcStr(usize, Vec<Arc<str>>),
     DynSeq(usize, Arc<dyn Object>),
     #[cfg(not(feature = "preserve_order"))]
-    Map(Option<StaticKey>, Arc<ValueMap>),
+    Map(Option<KeyRef<'static>>, Arc<ValueMap>),
     #[cfg(feature = "preserve_order")]
     Map(usize, Arc<ValueMap>),
 }
 
 impl ValueIteratorState {
     fn advance_state(&mut self) -> Option<Value> {
         match self {
             ValueIteratorState::Empty => None,
             ValueIteratorState::Chars(offset, ref s) => {
-                s.as_str()[*offset..].chars().next().map(|c| {
+                (s as &str)[*offset..].chars().next().map(|c| {
                     *offset += c.len_utf8();
                     Value::from(c)
                 })
             }
             ValueIteratorState::Seq(idx, items) => items
                 .get(*idx)
                 .map(|x| {
@@ -1201,71 +1312,88 @@
                 } else {
                     unreachable!()
                 }
             }
             #[cfg(feature = "preserve_order")]
             ValueIteratorState::Map(idx, map) => map.get_index(*idx).map(|x| {
                 *idx += 1;
-                Value::from(x.0.clone())
+                x.0.as_value()
             }),
             #[cfg(not(feature = "preserve_order"))]
             ValueIteratorState::Map(ptr, map) => {
                 if let Some(current) = ptr.take() {
                     let next = map.range(&current..).nth(1).map(|x| x.0.clone());
-                    let rv = Value::from(current);
+                    let rv = current.as_value();
                     *ptr = next;
                     Some(rv)
                 } else {
                     None
                 }
             }
         }
     }
 }
 
-#[test]
-fn test_dynamic_object_roundtrip() {
-    use std::sync::atomic::{self, AtomicUsize};
+#[cfg(test)]
+mod tests {
+    use super::*;
 
-    #[derive(Debug)]
-    struct X(AtomicUsize);
+    use similar_asserts::assert_eq;
 
-    impl fmt::Display for X {
-        fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-            write!(f, "{}", self.0.load(atomic::Ordering::Relaxed))
-        }
-    }
+    #[test]
+    fn test_dynamic_object_roundtrip() {
+        use std::sync::atomic::{self, AtomicUsize};
 
-    impl Object for X {
-        fn kind(&self) -> ObjectKind<'_> {
-            ObjectKind::Struct(self)
-        }
-    }
+        #[derive(Debug)]
+        struct X(AtomicUsize);
 
-    impl crate::value::object::StructObject for X {
-        fn get_field(&self, name: &str) -> Option<Value> {
-            match name {
-                "value" => Some(Value::from(self.0.load(atomic::Ordering::Relaxed))),
-                _ => None,
+        impl fmt::Display for X {
+            fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+                write!(f, "{}", self.0.load(atomic::Ordering::Relaxed))
             }
         }
 
-        fn static_fields(&self) -> Option<&'static [&'static str]> {
-            Some(&["value"][..])
+        impl Object for X {
+            fn kind(&self) -> ObjectKind<'_> {
+                ObjectKind::Struct(self)
+            }
         }
-    }
 
-    let x = Arc::new(X(Default::default()));
-    let x_value = Value::from(x.clone());
-    x.0.fetch_add(42, atomic::Ordering::Relaxed);
-    let x_clone = Value::from_serializable(&x_value);
-    x.0.fetch_add(23, atomic::Ordering::Relaxed);
+        impl crate::value::object::StructObject for X {
+            fn get_field(&self, name: &str) -> Option<Value> {
+                match name {
+                    "value" => Some(Value::from(self.0.load(atomic::Ordering::Relaxed))),
+                    _ => None,
+                }
+            }
 
-    assert_eq!(x_value.to_string(), "65");
-    assert_eq!(x_clone.to_string(), "65");
-}
+            fn static_fields(&self) -> Option<&'static [&'static str]> {
+                Some(&["value"][..])
+            }
+        }
 
-#[test]
-#[cfg(target_pointer_width = "64")]
-fn test_sizes() {
-    assert_eq!(std::mem::size_of::<Value>(), 24);
+        let x = Arc::new(X(Default::default()));
+        let x_value = Value::from(x.clone());
+        x.0.fetch_add(42, atomic::Ordering::Relaxed);
+        let x_clone = Value::from_serializable(&x_value);
+        x.0.fetch_add(23, atomic::Ordering::Relaxed);
+
+        assert_eq!(x_value.to_string(), "65");
+        assert_eq!(x_clone.to_string(), "65");
+    }
+
+    #[test]
+    fn test_string_char() {
+        let val = Value::from('a');
+        assert_eq!(char::try_from(val).unwrap(), 'a');
+        let val = Value::from("a");
+        assert_eq!(char::try_from(val).unwrap(), 'a');
+        let val = Value::from("wat");
+        assert!(char::try_from(val).is_err());
+    }
+
+    #[test]
+    #[cfg(target_pointer_width = "64")]
+    fn test_sizes() {
+        assert_eq!(std::mem::size_of::<Value>(), 24);
+    }
 }
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/value/object.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/value/object.rs`

 * *Files 2% similar despite different names*

```diff
@@ -453,19 +453,18 @@
     fn static_fields(&self) -> Option<&'static [&'static str]> {
         None
     }
 
     /// Returns a vector of field names.
     ///
     /// This should be implemented if [`static_fields`](Self::static_fields) cannot
-    /// be implemented due to lifetime restrictions.  To avoid unnecessary
-    /// allocations of the fields themselves it's recommended to use the
-    /// [`intern`] function.  The default implementation converts the return value
-    /// of [`static_fields`](Self::static_fields) into a compatible format automatically.
-    fn fields(&self) -> Vec<Arc<String>> {
+    /// be implemented due to lifetime restrictions.  The default implementation
+    /// converts the return value of [`static_fields`](Self::static_fields) into
+    /// a compatible format automatically.
+    fn fields(&self) -> Vec<Arc<str>> {
         self.static_fields()
             .into_iter()
             .flat_map(|fields| fields.iter().copied().map(intern))
             .collect()
     }
 
     /// Returns the number of fields.
@@ -489,15 +488,15 @@
 
     #[inline]
     fn static_fields(&self) -> Option<&'static [&'static str]> {
         T::static_fields(self)
     }
 
     #[inline]
-    fn fields(&self) -> Vec<Arc<String>> {
+    fn fields(&self) -> Vec<Arc<str>> {
         T::fields(self)
     }
 
     #[inline]
     fn field_count(&self) -> usize {
         T::field_count(self)
     }
@@ -511,37 +510,37 @@
 
     #[inline]
     fn static_fields(&self) -> Option<&'static [&'static str]> {
         T::static_fields(self)
     }
 
     #[inline]
-    fn fields(&self) -> Vec<Arc<String>> {
+    fn fields(&self) -> Vec<Arc<str>> {
         T::fields(self)
     }
 
     #[inline]
     fn field_count(&self) -> usize {
         T::field_count(self)
     }
 }
 
 #[repr(transparent)]
 pub struct SimpleSeqObject<T>(pub T);
 
 impl<T: SeqObject + 'static> fmt::Display for SimpleSeqObject<T> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        ok!(write!(f, "["));
+        ok!(f.write_str("["));
         for (idx, val) in (&self.0 as &dyn SeqObject).iter().enumerate() {
             if idx > 0 {
-                ok!(write!(f, ", "));
+                ok!(f.write_str(", "));
             }
             ok!(write!(f, "{val:?}"));
         }
-        write!(f, "]")
+        f.write_str("]")
     }
 }
 
 impl<T: SeqObject + 'static> fmt::Debug for SimpleSeqObject<T> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         f.debug_list()
             .entries((&self.0 as &dyn SeqObject).iter())
@@ -556,23 +555,23 @@
 }
 
 #[repr(transparent)]
 pub struct SimpleStructObject<T>(pub T);
 
 impl<T: StructObject + 'static> fmt::Display for SimpleStructObject<T> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        ok!(write!(f, "{{"));
+        ok!(f.write_str("{"));
         for (idx, field) in self.0.fields().iter().enumerate() {
             if idx > 0 {
-                ok!(write!(f, ", "));
+                ok!(f.write_str(", "));
             }
             let val = self.0.get_field(field).unwrap_or(Value::UNDEFINED);
             ok!(write!(f, "{field:?}: {val:?}"));
         }
-        write!(f, "}}")
+        f.write_str("}")
     }
 }
 
 impl<T: StructObject + 'static> fmt::Debug for SimpleStructObject<T> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         let mut m = f.debug_map();
         for field in self.0.fields() {
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/value/ops.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/value/ops.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 use std::convert::{TryFrom, TryInto};
-use std::fmt::Write;
 
 use crate::error::{Error, ErrorKind};
-use crate::value::{Arc, ObjectKind, SeqObject, Value, ValueKind, ValueRepr};
+use crate::value::{KeyRef, ObjectKind, SeqObject, Value, ValueKind, ValueRepr};
 
 pub enum CoerceResult<'a> {
     I128(i128, i128),
     F64(f64, f64),
     Str(&'a str, &'a str),
 }
 
-fn as_f64(value: &Value) -> Option<f64> {
+pub(crate) fn as_f64(value: &Value) -> Option<f64> {
     Some(match value.0 {
         ValueRepr::Bool(x) => x as i64 as f64,
         ValueRepr::U64(x) => x as f64,
         ValueRepr::U128(x) => x.0 as f64,
         ValueRepr::I64(x) => x as f64,
         ValueRepr::I128(x) => x.0 as f64,
         ValueRepr::F64(x) => x,
@@ -244,25 +243,16 @@
         }
     } else {
         Err(Error::from(ErrorKind::InvalidOperation))
     }
 }
 
 /// Attempts a string concatenation.
-pub fn string_concat(mut left: Value, right: &Value) -> Value {
-    match left.0 {
-        // if we're a string and we have a single reference to it, we can
-        // directly append into ourselves and reconstruct the value
-        ValueRepr::String(ref mut s, _) => {
-            write!(Arc::make_mut(s), "{right}").ok();
-            left
-        }
-        // otherwise we use format! to concat the two values
-        _ => Value::from(format!("{left}{right}")),
-    }
+pub fn string_concat(left: Value, right: &Value) -> Value {
+    Value::from(format!("{left}{right}"))
 }
 
 /// Implements a containment operation on values.
 pub fn contains(container: &Value, value: &Value) -> Result<Value, Error> {
     // Special case where if the container is undefined, it cannot hold
     // values.  For strict containment checks the vm has a special case.
     if container.is_undefined() {
@@ -273,90 +263,93 @@
             s.contains(s2)
         } else {
             s.contains(&value.to_string())
         }
     } else if let Some(seq) = container.as_seq() {
         seq.iter().any(|item| &item == value)
     } else if let ValueRepr::Map(ref map, _) = container.0 {
-        let key = match value.clone().try_into_key() {
-            Ok(key) => key,
-            Err(_) => return Ok(Value::from(false)),
-        };
-        map.get(&key).is_some()
+        map.get(&KeyRef::Value(value.clone())).is_some()
     } else {
         return Err(Error::new(
             ErrorKind::InvalidOperation,
             "cannot perform a containment check on this value",
         ));
     };
     Ok(Value::from(rv))
 }
 
-#[test]
-fn test_adding() {
-    let err = add(&Value::from("a"), &Value::from(42)).unwrap_err();
-    assert_eq!(
-        err.to_string(),
-        "invalid operation: tried to use + operator on unsupported types string and number"
-    );
-
-    assert_eq!(
-        add(&Value::from(1), &Value::from(2)).unwrap(),
-        Value::from(3)
-    );
-    assert_eq!(
-        add(&Value::from("foo"), &Value::from("bar")).unwrap(),
-        Value::from("foobar")
-    );
-}
-
-#[test]
-fn test_subtracting() {
-    let err = sub(&Value::from("a"), &Value::from(42)).unwrap_err();
-    assert_eq!(
-        err.to_string(),
-        "invalid operation: tried to use - operator on unsupported types string and number"
-    );
-
-    let err = sub(&Value::from("foo"), &Value::from("bar")).unwrap_err();
-    assert_eq!(
-        err.to_string(),
-        "invalid operation: tried to use - operator on unsupported types string and string"
-    );
-
-    assert_eq!(
-        sub(&Value::from(2), &Value::from(1)).unwrap(),
-        Value::from(1)
-    );
-}
-
-#[test]
-fn test_dividing() {
-    let err = div(&Value::from("a"), &Value::from(42)).unwrap_err();
-    assert_eq!(
-        err.to_string(),
-        "invalid operation: tried to use / operator on unsupported types string and number"
-    );
-
-    let err = div(&Value::from("foo"), &Value::from("bar")).unwrap_err();
-    assert_eq!(
-        err.to_string(),
-        "invalid operation: tried to use / operator on unsupported types string and string"
-    );
-
-    assert_eq!(
-        div(&Value::from(100), &Value::from(2)).unwrap(),
-        Value::from(50.0)
-    );
-}
-
-#[test]
-fn test_concat() {
-    assert_eq!(
-        string_concat(Value::from("foo"), &Value::from(42)),
-        Value::from("foo42")
-    );
-    assert_eq!(
-        string_concat(Value::from(23), &Value::from(42)),
-        Value::from("2342")
-    );
+#[cfg(test)]
+mod tests {
+    use super::*;
+
+    use similar_asserts::assert_eq;
+
+    #[test]
+    fn test_adding() {
+        let err = add(&Value::from("a"), &Value::from(42)).unwrap_err();
+        assert_eq!(
+            err.to_string(),
+            "invalid operation: tried to use + operator on unsupported types string and number"
+        );
+
+        assert_eq!(
+            add(&Value::from(1), &Value::from(2)).unwrap(),
+            Value::from(3)
+        );
+        assert_eq!(
+            add(&Value::from("foo"), &Value::from("bar")).unwrap(),
+            Value::from("foobar")
+        );
+    }
+
+    #[test]
+    fn test_subtracting() {
+        let err = sub(&Value::from("a"), &Value::from(42)).unwrap_err();
+        assert_eq!(
+            err.to_string(),
+            "invalid operation: tried to use - operator on unsupported types string and number"
+        );
+
+        let err = sub(&Value::from("foo"), &Value::from("bar")).unwrap_err();
+        assert_eq!(
+            err.to_string(),
+            "invalid operation: tried to use - operator on unsupported types string and string"
+        );
+
+        assert_eq!(
+            sub(&Value::from(2), &Value::from(1)).unwrap(),
+            Value::from(1)
+        );
+    }
+
+    #[test]
+    fn test_dividing() {
+        let err = div(&Value::from("a"), &Value::from(42)).unwrap_err();
+        assert_eq!(
+            err.to_string(),
+            "invalid operation: tried to use / operator on unsupported types string and number"
+        );
+
+        let err = div(&Value::from("foo"), &Value::from("bar")).unwrap_err();
+        assert_eq!(
+            err.to_string(),
+            "invalid operation: tried to use / operator on unsupported types string and string"
+        );
+
+        assert_eq!(
+            div(&Value::from(100), &Value::from(2)).unwrap(),
+            Value::from(50.0)
+        );
+    }
+
+    #[test]
+    fn test_concat() {
+        assert_eq!(
+            string_concat(Value::from("foo"), &Value::from(42)),
+            Value::from("foo42")
+        );
+        assert_eq!(
+            string_concat(Value::from(23), &Value::from(42)),
+            Value::from("2342")
+        );
+    }
 }
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/value/serialize.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/value/serialize.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 use std::collections::BTreeMap;
 use std::fmt;
 
 use serde::{ser, Serialize, Serializer};
 
-use crate::key::{Key, KeySerializer, StaticKey};
+use crate::utils::untrusted_size_hint;
 use crate::value::{
-    value_map_with_capacity, Arc, MapType, Packed, StringType, Value, ValueMap, ValueRepr,
+    value_map_with_capacity, Arc, KeyRef, MapType, Packed, StringType, Value, ValueMap, ValueRepr,
     VALUE_HANDLES, VALUE_HANDLE_MARKER,
 };
 
 #[derive(Debug)]
-pub struct InvalidValue(Arc<String>);
+pub struct InvalidValue(Arc<str>);
 
 impl std::error::Error for InvalidValue {}
 
 impl fmt::Display for InvalidValue {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        write!(f, "{}", self.0)
+        self.0.fmt(f)
     }
 }
 
 impl serde::ser::Error for InvalidValue {
     fn custom<T>(msg: T) -> Self
     where
         T: fmt::Display,
     {
-        InvalidValue(Arc::new(msg.to_string()))
+        InvalidValue(Arc::from(msg.to_string()))
     }
 }
 
 /// Transforms a serializable value to a value object.
 ///
 /// This neither fails nor panics.  For objects that cannot be represented
 /// the value might be represented as a half broken error object.
@@ -103,19 +103,19 @@
     }
 
     fn serialize_f64(self, v: f64) -> Result<Value, InvalidValue> {
         Ok(ValueRepr::F64(v).into())
     }
 
     fn serialize_char(self, v: char) -> Result<Value, InvalidValue> {
-        Ok(ValueRepr::Char(v).into())
+        Ok(ValueRepr::String(Arc::from(v.to_string()), StringType::Normal).into())
     }
 
     fn serialize_str(self, value: &str) -> Result<Value, InvalidValue> {
-        Ok(ValueRepr::String(Arc::new(value.to_owned()), StringType::Normal).into())
+        Ok(ValueRepr::String(Arc::from(value.to_owned()), StringType::Normal).into())
     }
 
     fn serialize_bytes(self, value: &[u8]) -> Result<Value, InvalidValue> {
         Ok(ValueRepr::Bytes(Arc::new(value.to_owned())).into())
     }
 
     fn serialize_none(self) -> Result<Value, InvalidValue> {
@@ -173,50 +173,50 @@
         variant: &'static str,
         value: &T,
     ) -> Result<Value, InvalidValue>
     where
         T: Serialize,
     {
         let mut map = value_map_with_capacity(1);
-        map.insert(Key::Str(variant), transform(value));
+        map.insert(KeyRef::Str(variant), transform(value));
         Ok(ValueRepr::Map(Arc::new(map), MapType::Normal).into())
     }
 
     fn serialize_seq(self, len: Option<usize>) -> Result<Self::SerializeSeq, InvalidValue> {
         Ok(SerializeSeq {
-            elements: Vec::with_capacity(len.unwrap_or(0)),
+            elements: Vec::with_capacity(untrusted_size_hint(len.unwrap_or(0))),
         })
     }
 
     fn serialize_tuple(self, len: usize) -> Result<Self::SerializeTuple, InvalidValue> {
         Ok(SerializeTuple {
-            elements: Vec::with_capacity(len),
+            elements: Vec::with_capacity(untrusted_size_hint(len)),
         })
     }
 
     fn serialize_tuple_struct(
         self,
         _name: &'static str,
         len: usize,
     ) -> Result<Self::SerializeTupleStruct, InvalidValue> {
         Ok(SerializeTupleStruct {
-            fields: Vec::with_capacity(len),
+            fields: Vec::with_capacity(untrusted_size_hint(len)),
         })
     }
 
     fn serialize_tuple_variant(
         self,
         _name: &'static str,
         _variant_index: u32,
         variant: &'static str,
         len: usize,
     ) -> Result<Self::SerializeTupleVariant, InvalidValue> {
         Ok(SerializeTupleVariant {
             name: variant,
-            fields: Vec::with_capacity(len),
+            fields: Vec::with_capacity(untrusted_size_hint(len)),
         })
     }
 
     fn serialize_map(self, len: Option<usize>) -> Result<Self::SerializeMap, InvalidValue> {
         Ok(SerializeMap {
             entries: value_map_with_capacity(len.unwrap_or(0)),
             key: None,
@@ -326,47 +326,47 @@
         self.fields.push(transform(value));
         Ok(())
     }
 
     fn end(self) -> Result<Value, InvalidValue> {
         let mut map = value_map_with_capacity(1);
         map.insert(
-            Key::Str(self.name),
+            KeyRef::Str(self.name),
             Value(ValueRepr::Seq(self.fields.into())),
         );
         Ok(Value(ValueRepr::Map(map.into(), MapType::Normal)))
     }
 }
 
 pub struct SerializeMap {
     entries: ValueMap,
-    key: Option<StaticKey>,
+    key: Option<Value>,
 }
 
 impl ser::SerializeMap for SerializeMap {
     type Ok = Value;
     type Error = InvalidValue;
 
     fn serialize_key<T: ?Sized>(&mut self, key: &T) -> Result<(), InvalidValue>
     where
         T: Serialize,
     {
-        match key.serialize(KeySerializer) {
+        match key.serialize(ValueSerializer) {
             Ok(key) => self.key = Some(key),
             Err(_) => self.key = None,
         }
         Ok(())
     }
 
     fn serialize_value<T: ?Sized>(&mut self, value: &T) -> Result<(), InvalidValue>
     where
         T: Serialize,
     {
         if let Some(key) = self.key.take() {
-            self.entries.insert(key, transform(value));
+            self.entries.insert(KeyRef::Value(key), transform(value));
         }
         Ok(())
     }
 
     fn end(self) -> Result<Value, InvalidValue> {
         Ok(Value(ValueRepr::Map(
             Arc::new(self.entries),
@@ -379,16 +379,16 @@
         key: &K,
         value: &V,
     ) -> Result<(), InvalidValue>
     where
         K: Serialize,
         V: Serialize,
     {
-        if let Ok(key) = key.serialize(KeySerializer) {
-            self.entries.insert(key, transform(value));
+        if let Ok(key) = key.serialize(ValueSerializer) {
+            self.entries.insert(KeyRef::Value(key), transform(value));
         }
         Ok(())
     }
 }
 
 pub struct SerializeStruct {
     fields: ValueMap,
@@ -402,15 +402,15 @@
         &mut self,
         key: &'static str,
         value: &T,
     ) -> Result<(), InvalidValue>
     where
         T: Serialize,
     {
-        self.fields.insert(Key::Str(key), transform(value));
+        self.fields.insert(KeyRef::Str(key), transform(value));
         Ok(())
     }
 
     fn end(self) -> Result<Value, InvalidValue> {
         Ok(ValueRepr::Map(Arc::new(self.fields), MapType::Normal).into())
     }
 }
@@ -428,15 +428,15 @@
         &mut self,
         key: &'static str,
         value: &T,
     ) -> Result<(), InvalidValue>
     where
         T: Serialize,
     {
-        self.map.insert(Key::Str(key), transform(value));
+        self.map.insert(KeyRef::Str(key), transform(value));
         Ok(())
     }
 
     fn end(self) -> Result<Value, InvalidValue> {
         let mut rv = BTreeMap::new();
         rv.insert(
             self.variant,
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/vm/closure_object.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/vm/closure_object.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 use std::collections::BTreeMap;
 use std::fmt;
 use std::sync::{Arc, Mutex};
 
-use crate::key::{Key, StaticKey};
-use crate::value::{intern, Object, ObjectKind, StructObject, Value};
+use crate::value::{Object, ObjectKind, StructObject, Value};
 
 /// Utility to enclose values for macros.
 ///
 /// See `closure` on the [`Frame`] for how it's used.
 #[derive(Debug, Default)]
 pub(crate) struct Closure {
-    values: Mutex<BTreeMap<StaticKey, Value>>,
+    values: Mutex<BTreeMap<Arc<str>, Value>>,
 }
 
 impl Closure {
     /// Stores a value by key in the closure.
     pub fn store(&self, key: &str, value: Value) {
-        self.values
-            .lock()
-            .unwrap()
-            .insert(StaticKey::from(key), value);
+        self.values.lock().unwrap().insert(Arc::from(key), value);
     }
 
     /// Upset a value into the closure.
     #[cfg(feature = "macros")]
     pub fn store_if_missing<F: FnOnce() -> Value>(&self, key: &str, f: F) {
         let mut values = self.values.lock().unwrap();
-        if !values.contains_key(&Key::Str(key)) {
-            values.insert(key.into(), f());
+        if !values.contains_key(key) {
+            values.insert(Arc::from(key), f());
         }
     }
 }
 
 impl fmt::Display for Closure {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         let mut m = f.debug_map();
@@ -45,21 +41,15 @@
 impl Object for Closure {
     fn kind(&self) -> ObjectKind<'_> {
         ObjectKind::Struct(self)
     }
 }
 
 impl StructObject for Closure {
-    fn fields(&self) -> Vec<Arc<String>> {
-        self.values
-            .lock()
-            .unwrap()
-            .keys()
-            .filter_map(|x| x.as_str())
-            .map(intern)
-            .collect()
+    fn fields(&self) -> Vec<Arc<str>> {
+        self.values.lock().unwrap().keys().cloned().collect()
     }
 
     fn get_field(&self, name: &str) -> Option<Value> {
-        self.values.lock().unwrap().get(&Key::Str(name)).cloned()
+        self.values.lock().unwrap().get(name).cloned()
     }
 }
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/vm/context.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/vm/context.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use std::borrow::Cow;
 use std::collections::{BTreeMap, HashSet};
 use std::fmt;
 use std::sync::Arc;
 
 use crate::environment::Environment;
 use crate::error::{Error, ErrorKind};
-use crate::value::{OwnedValueIterator, Value};
+use crate::value::{OwnedValueIterator, Value, ValueRepr};
 use crate::vm::closure_object::Closure;
 use crate::vm::loop_object::Loop;
 
 type Locals<'env> = BTreeMap<&'env str, Value>;
 
 /// The maximum recursion in the VM.  Normally each stack frame
 /// adds one to this counter (eg: every time a frame is added).
@@ -44,22 +44,32 @@
 impl<'env> Default for Frame<'env> {
     fn default() -> Frame<'env> {
         Frame::new(Value::UNDEFINED)
     }
 }
 
 impl<'env> Frame<'env> {
+    /// Creates a new frame with the given context and no validation
     pub fn new(ctx: Value) -> Frame<'env> {
         Frame {
             locals: Locals::new(),
             ctx,
             current_loop: None,
             closure: None,
         }
     }
+
+    /// Creates a new frame with the given context and validates the the value is not invalid
+    pub fn new_checked(root: Value) -> Result<Frame<'env>, Error> {
+        if let ValueRepr::Invalid(ref err) = root.0 {
+            Err(Error::new(ErrorKind::BadSerialization, err.to_string()))
+        } else {
+            Ok(Frame::new(root))
+        }
+    }
 }
 
 #[cfg(feature = "internal_debug")]
 impl<'env> fmt::Debug for Frame<'env> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         let mut m = f.debug_map();
         m.entry(&"locals", &self.locals);
@@ -274,18 +284,24 @@
 
     /// Pops the topmost layer.
     #[track_caller]
     pub fn pop_frame(&mut self) -> Frame {
         self.stack.pop().unwrap()
     }
 
-    /// Returns the current locals.
+    /// Returns the root locals (exports)
+    #[track_caller]
+    pub fn exports(&self) -> &Locals<'env> {
+        &self.stack.first().unwrap().locals
+    }
+
+    /// Returns the current locals mutably.
     #[track_caller]
     #[cfg(feature = "multi_template")]
-    pub fn current_locals(&mut self) -> &mut Locals<'env> {
+    pub fn current_locals_mut(&mut self) -> &mut Locals<'env> {
         &mut self.stack.last_mut().unwrap().locals
     }
 
     /// Returns the current innermost loop.
     pub fn current_loop(&mut self) -> Option<&mut LoopState> {
         self.stack
             .iter_mut()
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/vm/loop_object.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/vm/loop_object.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/vm/macro_object.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/vm/macro_object.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 use std::collections::BTreeSet;
 use std::fmt;
 use std::sync::Arc;
 
 use crate::error::{Error, ErrorKind};
-use crate::key::Key;
 use crate::output::Output;
 use crate::utils::AutoEscape;
-use crate::value::{MapType, Object, ObjectKind, StringType, StructObject, Value, ValueRepr};
+use crate::value::{
+    KeyRef, MapType, Object, ObjectKind, StringType, StructObject, Value, ValueRepr,
+};
 use crate::vm::state::State;
 use crate::vm::Vm;
 
 pub(crate) struct MacroData {
-    pub name: Arc<String>,
-    pub arg_spec: Vec<Arc<String>>,
+    pub name: Arc<str>,
+    pub arg_spec: Vec<Arc<str>>,
     // because values need to be 'static, we can't hold a reference to the
     // instructions that declared the macro.  Instead of that we place the
     // reference to the macro instruction (and the jump offset) in the
     // state under `state.macros`.
     pub macro_ref_id: usize,
     pub closure: Value,
     pub caller_reference: bool,
@@ -57,15 +58,15 @@
             return Err(Error::from(ErrorKind::TooManyArguments));
         }
 
         let mut kwargs_used = BTreeSet::new();
         let mut arg_values = Vec::with_capacity(self.data.arg_spec.len());
         for (idx, name) in self.data.arg_spec.iter().enumerate() {
             let kwarg = match kwargs {
-                Some(kwargs) => kwargs.get(&Key::Str(name)),
+                Some(kwargs) => kwargs.get(&KeyRef::Str(name)),
                 _ => None,
             };
             arg_values.push(match (args.get(idx), kwarg) {
                 (Some(_), Some(_)) => {
                     return Err(Error::new(
                         ErrorKind::TooManyArguments,
                         format!("duplicate argument `{name}`"),
@@ -80,15 +81,15 @@
             });
         }
 
         let caller = if self.data.caller_reference {
             kwargs_used.insert("caller");
             Some(
                 kwargs
-                    .and_then(|x| x.get(&Key::Str("caller")).cloned())
+                    .and_then(|x| x.get(&KeyRef::Str("caller")).cloned())
                     .unwrap_or(Value::UNDEFINED),
             )
         } else {
             None
         };
 
         if let Some(kwargs) = kwargs {
```

### Comparing `minijinja-0.32.0/local_dependencies/minijinja/src/vm/mod.rs` & `minijinja-1.0.0/local_dependencies/minijinja/src/vm/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-use std::collections::{BTreeMap, BTreeSet};
+use std::collections::BTreeMap;
 use std::mem;
 use std::sync::atomic::{AtomicUsize, Ordering};
 use std::sync::{Arc, Mutex};
 
 use crate::compiler::instructions::{
     Instruction, Instructions, LOOP_FLAG_RECURSIVE, LOOP_FLAG_WITH_LOOP_VAR, MAX_LOCALS,
 };
 use crate::environment::Environment;
 use crate::error::{Error, ErrorKind};
 use crate::output::{CaptureMode, Output};
-use crate::utils::{AutoEscape, UndefinedBehavior};
-use crate::value::{self, ops, value_map_with_capacity, MapType, Value, ValueRepr};
+use crate::utils::{untrusted_size_hint, AutoEscape, UndefinedBehavior};
+use crate::value::{
+    ops, value_map_with_capacity, value_optimization, KeyRef, MapType, Value, ValueRepr,
+};
 use crate::vm::context::{Context, Frame, LoopState, Stack};
 use crate::vm::loop_object::Loop;
 use crate::vm::state::BlockStack;
 
 #[cfg(feature = "macros")]
 use crate::vm::macro_object::{Macro, MacroData};
 
-#[cfg(feature = "fuel")]
-use crate::vm::fuel::FuelTracker;
-
 pub use crate::vm::state::State;
 
 mod closure_object;
 mod context;
 #[cfg(feature = "fuel")]
 mod fuel;
 mod loop_object;
@@ -42,17 +41,17 @@
 
 /// Helps to evaluate something.
 #[cfg_attr(feature = "internal_debug", derive(Debug))]
 pub struct Vm<'env> {
     env: &'env Environment<'env>,
 }
 
-fn prepare_blocks<'env, 'vm>(
-    blocks: &'vm BTreeMap<&'env str, Instructions<'env>>,
-) -> BTreeMap<&'env str, BlockStack<'vm, 'env>> {
+pub(crate) fn prepare_blocks<'env, 'template>(
+    blocks: &'template BTreeMap<&'env str, Instructions<'env>>,
+) -> BTreeMap<&'env str, BlockStack<'template, 'env>> {
     blocks
         .iter()
         .map(|(name, instr)| (*name, BlockStack::new(instr)))
         .collect()
 }
 
 fn get_or_lookup_local<T, F>(vec: &mut [Option<T>], local_id: u8, f: F) -> Option<T>
@@ -73,44 +72,35 @@
 
 impl<'env> Vm<'env> {
     /// Creates a new VM.
     pub fn new(env: &'env Environment<'env>) -> Vm<'env> {
         Vm { env }
     }
 
-    /// Evaluates the given inputs
-    pub fn eval(
+    /// Evaluates the given inputs.
+    ///
+    /// It returns both the last value left on the stack as well as the state
+    /// at the end of the evaluation.
+    pub fn eval<'template>(
         &self,
-        instructions: &Instructions<'env>,
+        instructions: &'template Instructions<'env>,
         root: Value,
-        blocks: &BTreeMap<&'env str, Instructions<'env>>,
+        blocks: &'template BTreeMap<&'env str, Instructions<'env>>,
         out: &mut Output,
         auto_escape: AutoEscape,
-    ) -> Result<Option<Value>, Error> {
-        let _guard = value::value_optimization();
-        if let ValueRepr::Invalid(ref err) = root.0 {
-            return Err(Error::new(ErrorKind::BadSerialization, err.to_string()));
-        }
-        self.eval_state(
-            &mut State {
-                env: self.env,
-                ctx: Context::new(Frame::new(root)),
-                current_block: None,
-                current_call: None,
-                auto_escape,
-                instructions,
-                blocks: prepare_blocks(blocks),
-                loaded_templates: BTreeSet::new(),
-                #[cfg(feature = "macros")]
-                macros: Arc::new(Vec::new()),
-                #[cfg(feature = "fuel")]
-                fuel_tracker: self.env.fuel().map(FuelTracker::new),
-            },
-            out,
-        )
+    ) -> Result<(Option<Value>, State<'template, 'env>), Error> {
+        let _guard = value_optimization();
+        let mut state = State::new(
+            self.env,
+            Context::new(ok!(Frame::new_checked(root))),
+            auto_escape,
+            instructions,
+            prepare_blocks(blocks),
+        );
+        self.eval_state(&mut state, out).map(|x| (x, state))
     }
 
     /// Evaluate a macro in a state.
     #[cfg(feature = "macros")]
     #[allow(clippy::too_many_arguments)]
     pub fn eval_macro(
         &self,
@@ -128,19 +118,18 @@
         }
         ok!(ctx.incr_depth(state.ctx.depth() + MACRO_RECURSION_COST));
         self.eval_impl(
             &mut State {
                 env: self.env,
                 ctx,
                 current_block: None,
-                current_call: None,
                 auto_escape: state.auto_escape(),
                 instructions,
                 blocks: BTreeMap::default(),
-                loaded_templates: BTreeSet::new(),
+                loaded_templates: Default::default(),
                 #[cfg(feature = "macros")]
                 macros: state.macros.clone(),
                 #[cfg(feature = "fuel")]
                 fuel_tracker: state.fuel_tracker.clone(),
             },
             out,
             Stack::from(args),
@@ -170,15 +159,15 @@
         let mut auto_escape_stack = vec![];
         let mut next_loop_recursion_jump = None;
         let mut loaded_filters = [None; MAX_LOCALS];
         let mut loaded_tests = [None; MAX_LOCALS];
 
         // If we are extending we are holding the instructions of the target parent
         // template here.  This is used to detect multiple extends and the evaluation
-        // uses these instructions when RenderParent is evaluated.
+        // uses these instructions when it makes it to the end of the instructions.
         #[cfg(feature = "multi_template")]
         let mut parent_instructions = None;
 
         macro_rules! recurse_loop {
             ($capture:expr) => {{
                 let jump_target = ctx_ok!(self.prepare_loop_recursion(state));
                 // the way this works is that we remember the next instruction
@@ -190,15 +179,36 @@
                     out.begin_capture(CaptureMode::Capture);
                 }
                 pc = jump_target;
                 continue;
             }};
         }
 
-        while let Some(instr) = state.instructions.get(pc) {
+        loop {
+            let instr = match state.instructions.get(pc) {
+                Some(instr) => instr,
+                #[cfg(not(feature = "multi_template"))]
+                None => break,
+                #[cfg(feature = "multi_template")]
+                None => {
+                    // when an extends statement appears in a template, when we hit the
+                    // last instruction we need to check if parent instructions were
+                    // stashed away (which means we found an extends tag which invoked
+                    // `LoadBlocks`).  If we do find instructions, we reset back to 0
+                    // from the new instructions.
+                    state.instructions = match parent_instructions.take() {
+                        Some(instr) => instr,
+                        None => break,
+                    };
+                    out.end_capture(AutoEscape::None);
+                    pc = 0;
+                    continue;
+                }
+            };
+
             // if we only have two arguments that we pull from the stack, we
             // can assign them to a and b.  This slightly reduces the amount of
             // code bloat generated here.  Do the same for a potential error
             // that needs processing.
             let a;
             let b;
             let mut err;
@@ -303,30 +313,30 @@
                 Instruction::LoadConst(value) => {
                     stack.push(value.clone());
                 }
                 Instruction::BuildMap(pair_count) => {
                     let mut map = value_map_with_capacity(*pair_count);
                     for _ in 0..*pair_count {
                         let value = stack.pop();
-                        let key = ctx_ok!(stack.pop().try_into_key());
-                        map.insert(key, value);
+                        let key = stack.pop();
+                        map.insert(KeyRef::Value(key), value);
                     }
                     stack.push(Value(ValueRepr::Map(map.into(), MapType::Normal)))
                 }
                 Instruction::BuildKwargs(pair_count) => {
                     let mut map = value_map_with_capacity(*pair_count);
                     for _ in 0..*pair_count {
                         let value = stack.pop();
-                        let key = stack.pop().try_into_key().unwrap();
-                        map.insert(key, value);
+                        let key = stack.pop();
+                        map.insert(KeyRef::Value(key), value);
                     }
                     stack.push(Value(ValueRepr::Map(map.into(), MapType::Kwargs)))
                 }
                 Instruction::BuildList(count) => {
-                    let mut v = Vec::with_capacity(*count);
+                    let mut v = Vec::with_capacity(untrusted_size_hint(*count));
                     for _ in 0..*count {
                         v.push(stack.pop());
                     }
                     v.reverse();
                     stack.push(Value(ValueRepr::Seq(Arc::new(v))));
                 }
                 Instruction::UnpackList(count) => {
@@ -458,32 +468,16 @@
                         continue;
                     } else {
                         stack.pop();
                     }
                 }
                 #[cfg(feature = "multi_template")]
                 Instruction::CallBlock(name) => {
-                    if parent_instructions.is_none() {
-                        let old_block = state.current_block;
-                        state.current_block = Some(name);
-                        if let Some(block_stack) = state.blocks.get(name) {
-                            let old_instructions =
-                                mem::replace(&mut state.instructions, block_stack.instructions());
-                            ctx_ok!(state.ctx.push_frame(Frame::default()));
-                            let rv = self.eval_state(state, out);
-                            state.ctx.pop_frame();
-                            state.instructions = old_instructions;
-                            ctx_ok!(rv);
-                        } else {
-                            bail!(Error::new(
-                                ErrorKind::InvalidOperation,
-                                "tried to invoke unknown block"
-                            ));
-                        }
-                        state.current_block = old_block;
+                    if parent_instructions.is_none() && !out.is_discarding() {
+                        self.call_block(name, state, out)?;
                     }
                 }
                 Instruction::PushAutoEscape => {
                     a = stack.pop();
                     auto_escape_stack.push(state.auto_escape);
                     state.auto_escape = ctx_ok!(self.derive_auto_escape(a, initial_auto_escape));
                 }
@@ -493,48 +487,42 @@
                 Instruction::BeginCapture(mode) => {
                     out.begin_capture(*mode);
                 }
                 Instruction::EndCapture => {
                     stack.push(out.end_capture(state.auto_escape));
                 }
                 Instruction::ApplyFilter(name, arg_count, local_id) => {
-                    state.current_call = Some(name);
                     let filter =
                         ctx_ok!(get_or_lookup_local(&mut loaded_filters, *local_id, || {
                             state.env.get_filter(name)
                         })
                         .ok_or_else(|| {
                             Error::new(
                                 ErrorKind::UnknownFilter,
                                 format!("filter {name} is unknown"),
                             )
                         }));
                     let args = stack.slice_top(*arg_count);
                     a = ctx_ok!(filter.apply_to(state, args));
                     stack.drop_top(*arg_count);
                     stack.push(a);
-                    state.current_call = Some(name);
                 }
                 Instruction::PerformTest(name, arg_count, local_id) => {
-                    state.current_call = Some(name);
                     let test = ctx_ok!(get_or_lookup_local(&mut loaded_tests, *local_id, || {
                         state.env.get_test(name)
                     })
                     .ok_or_else(|| {
                         Error::new(ErrorKind::UnknownTest, format!("test {name} is unknown"))
                     }));
                     let args = stack.slice_top(*arg_count);
                     let rv = ctx_ok!(test.perform(state, args));
                     stack.drop_top(*arg_count);
                     stack.push(Value::from(rv));
-                    state.current_call = None;
                 }
                 Instruction::CallFunction(name, arg_count) => {
-                    state.current_call = Some(name);
-
                     // super is a special function reserved for super-ing into blocks.
                     if *name == "super" {
                         if *arg_count != 0 {
                             bail!(Error::new(
                                 ErrorKind::InvalidOperation,
                                 "super() takes no arguments",
                             ));
@@ -557,54 +545,48 @@
                         stack.push(a);
                     } else {
                         bail!(Error::new(
                             ErrorKind::UnknownFunction,
                             format!("{name} is unknown"),
                         ));
                     }
-
-                    state.current_call = None;
                 }
                 Instruction::CallMethod(name, arg_count) => {
-                    state.current_call = Some(name);
                     let args = stack.slice_top(*arg_count);
                     a = ctx_ok!(args[0].call_method(state, name, &args[1..]));
                     stack.drop_top(*arg_count);
                     stack.push(a);
-                    state.current_call = None;
                 }
                 Instruction::CallObject(arg_count) => {
                     let args = stack.slice_top(*arg_count);
                     a = ctx_ok!(args[0].call(state, &args[1..]));
                     stack.drop_top(*arg_count);
                     stack.push(a);
                 }
                 Instruction::DupTop => {
                     stack.push(stack.peek().clone());
                 }
                 Instruction::DiscardTop => {
                     stack.pop();
                 }
                 Instruction::FastSuper => {
-                    // Note that we don't store 'current_call' here since it
-                    // would only be visible (and unused) internally.
                     ctx_ok!(self.perform_super(state, out, false));
                 }
                 Instruction::FastRecurse => {
-                    // Note that we don't store 'current_call' here since it
-                    // would only be visible (and unused) internally.
                     recurse_loop!(false);
                 }
-                // Explanation on the behavior of `LoadBlocks` and `RenderParent`.
+                // Explanation on the behavior of `LoadBlocks` and rendering of
+                // inherited templates:
+                //
                 // MiniJinja inherits the behavior from Jinja2 where extending
                 // loads the blocks (`LoadBlocks`) and the rest of the template
                 // keeps executing but with output disabled, only at the end the
-                // parent template is then invoked (`RenderParent`).  This has the
-                // effect that you can still set variables or declare macros and
-                // that they become visible in the blocks.
+                // parent template is then invoked.  This has the effect that
+                // you can still set variables or declare macros and that they
+                // become visible in the blocks.
                 //
                 // This behavior has a few downsides.  First of all what happens
                 // in the parent template overrides what happens in the child.
                 // For instance if you declare a macro named `foo` after `{%
                 // extends %}` and then a variable with that named is also set
                 // in the parent template, then you won't be able to call that
                 // macro in the body.
@@ -624,46 +606,24 @@
                             "tried to extend a second time in a template"
                         ));
                     }
                     parent_instructions = Some(ctx_ok!(self.load_blocks(a, state)));
                     out.begin_capture(CaptureMode::Discard);
                 }
                 #[cfg(feature = "multi_template")]
-                Instruction::RenderParent => {
-                    // when an extends statement appears in a template, the last instruction
-                    // in that template is the `RenderParent` opcode.  However there is no
-                    // guarantee that we actually encountered the extends tag that would
-                    // have loaded the parent blocks (`LoadBlocks`).  Because of this it's
-                    // possible that we actually end up in this instruction without blocks
-                    // loaded.  In that case we interpret the opcode as if we're breaking
-                    // out of the eval loop.
-                    state.instructions = match parent_instructions.take() {
-                        Some(instr) => instr,
-                        None => break,
-                    };
-                    out.end_capture(AutoEscape::None);
-
-                    // then replace the instructions and set the pc to 0 again.
-                    // this effectively means that the template engine will now
-                    // execute the extended template's code instead.  From this
-                    // there is no way back.
-                    pc = 0;
-                    continue;
-                }
-                #[cfg(feature = "multi_template")]
                 Instruction::Include(ignore_missing) => {
                     a = stack.pop();
                     ctx_ok!(self.perform_include(a, state, out, *ignore_missing));
                 }
                 #[cfg(feature = "multi_template")]
                 Instruction::ExportLocals => {
-                    let locals = state.ctx.current_locals();
+                    let locals = state.ctx.current_locals_mut();
                     let mut module = value_map_with_capacity(locals.len());
                     for (key, value) in locals.iter() {
-                        module.insert((*key).into(), value.clone());
+                        module.insert(KeyRef::Value(Value::from(*key)), value.clone());
                     }
                     stack.push(Value(ValueRepr::Map(module.into(), MapType::Normal)));
                 }
                 #[cfg(feature = "macros")]
                 Instruction::BuildMacro(name, offset, flags) => {
                     self.build_macro(&mut stack, state, *offset, name, *flags);
                 }
@@ -714,17 +674,19 @@
                         templates_tried.push(choice);
                     } else {
                         return Err(err);
                     }
                     continue;
                 }
             };
+
+            let (new_instructions, new_blocks) = ok!(tmpl.instructions_and_blocks());
             let old_escape = mem::replace(&mut state.auto_escape, tmpl.initial_auto_escape());
-            let old_instructions = mem::replace(&mut state.instructions, tmpl.instructions());
-            let old_blocks = mem::replace(&mut state.blocks, prepare_blocks(tmpl.blocks()));
+            let old_instructions = mem::replace(&mut state.instructions, new_instructions);
+            let old_blocks = mem::replace(&mut state.blocks, prepare_blocks(new_blocks));
             let old_closure = state.ctx.take_closure();
             ok!(state.ctx.incr_depth(INCLUDE_RECURSION_COST));
             let rv = self.eval_state(state, out);
             state.ctx.reset_closure(old_closure);
             state.ctx.decr_depth(INCLUDE_RECURSION_COST);
             state.auto_escape = old_escape;
             state.instructions = old_instructions;
@@ -833,23 +795,49 @@
         if state.loaded_templates.contains(&name) {
             return Err(Error::new(
                 ErrorKind::InvalidOperation,
                 format!("cycle in template inheritance. {name:?} was referenced more than once"),
             ));
         }
         let tmpl = ok!(self.env.get_template(name));
-        state.loaded_templates.insert(tmpl.instructions().name());
-        for (name, instr) in tmpl.blocks().iter() {
+        let (new_instructions, new_blocks) = ok!(tmpl.instructions_and_blocks());
+        state.loaded_templates.insert(new_instructions.name());
+        for (name, instr) in new_blocks.iter() {
             state
                 .blocks
                 .entry(name)
                 .or_insert_with(BlockStack::default)
                 .append_instructions(instr);
         }
-        Ok(tmpl.instructions())
+        Ok(new_instructions)
+    }
+
+    #[cfg(feature = "multi_template")]
+    pub(crate) fn call_block(
+        &self,
+        name: &str,
+        state: &mut State<'_, 'env>,
+        out: &mut Output,
+    ) -> Result<Option<Value>, Error> {
+        if let Some((name, block_stack)) = state.blocks.get_key_value(name) {
+            let old_block = mem::replace(&mut state.current_block, Some(name));
+            let old_instructions =
+                mem::replace(&mut state.instructions, block_stack.instructions());
+            state.ctx.push_frame(Frame::default())?;
+            let rv = self.eval_state(state, out);
+            state.ctx.pop_frame();
+            state.instructions = old_instructions;
+            state.current_block = old_block;
+            rv
+        } else {
+            Err(Error::new(
+                ErrorKind::UnknownBlock,
+                format!("block '{}' not found", name),
+            ))
+        }
     }
 
     fn derive_auto_escape(
         &self,
         value: Value,
         initial_auto_escape: AutoEscape,
     ) -> Result<AutoEscape, Error> {
@@ -951,15 +939,15 @@
             _ => unreachable!(),
         };
         let closure = stack.pop();
         let macro_ref_id = state.macros.len();
         Arc::make_mut(&mut state.macros).push((state.instructions, offset));
         stack.push(Value::from_object(Macro {
             data: Arc::new(MacroData {
-                name: Arc::new(name.to_string()),
+                name: Arc::from(name.to_string()),
                 arg_spec,
                 macro_ref_id,
                 closure,
                 caller_reference: (flags & MACRO_CALLER) != 0,
             }),
         }));
     }
```

### Comparing `minijinja-0.32.0/LICENSE` & `minijinja-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `minijinja-0.32.0/README.md` & `minijinja-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 ```python
 result = env.render_template('template_name', var1="value 1", var2="value 2")
 print(result)
 ```
 
 ## Purpose
 
-MiniJinja attemps a certain level of compatibiliy with Jinja2, but it does not
+MiniJinja attempts a certain level of compatibility with Jinja2, but it does not
 try to achieve this at all costs.  As a result you will notice that quite a few
 templates will refuse to render with MiniJinja despite the fact that they probably
 look quite innocent.  It is however possible to write templates that render to the
 same results for both Jinja2 and MiniJinja.  This raises the question why you might
 want to use MiniJinja.
 
 The main benefit would be to achieve the exact same results in both Rust and Python.
@@ -67,17 +67,16 @@
 marshalling that needs to happen in either direction there is a certain amount of
 loss of information.
 
 ## Dynamic Template Loading
 
 MiniJinja's Python bindings inherit the underlying behavior of how MiniJinja loads
 templates.  Templates are loaded on first use and then cached.  The templates are
-loaded via a "source" (called `loader` in MiniJinja's Python bindings).  To trigger
-a reload you can call `env.reload()` or alternatively set `env.reload_before_render`
-to `True`.
+loaded via a loader.  To trigger a reload you can call `env.reload()` or
+alternatively set `env.reload_before_render` to `True`.
 
 ```python
 def my_loader(name):
     segments = []
     for segment in name.split("/"):
         if "\\" in segment or segment in (".", ".."):
             return None
@@ -108,15 +107,15 @@
 MiniJinja uses [markupsafe](https://github.com/pallets/markupsafe) if it's available
 on the Python side.  It will honor `__html__`.
 
 ## Finalizers
 
 Instead of custom formatters like in MiniJinja, you can define a finalizer instead
 which is similar to how it works in Jinja2.  It's passed a value (or optional also
-the state as first argument whne `pass_state` is used) and can return a new value.
+the state as first argument when `pass_state` is used) and can return a new value.
 If the special `NotImplemented` value is returned, the original value is rendered
 without any modification:
 
 ```
 from minijinja import Environment
 
 def finalizer(value):
```

### Comparing `minijinja-0.32.0/hello.py` & `minijinja-1.0.0/hello.py`

 * *Files identical despite different names*

### Comparing `minijinja-0.32.0/pyproject.toml` & `minijinja-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=0.15,<0.16"]
 build-backend = "maturin"
 
 [project]
 name = "minijinja"
-version = "0.32.0"
+version = "1.0.0"
 description = "An experimental Python binding of the Rust MiniJinja template engine."
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
     { name = "Armin Ronacher", email = "armin.ronacher@active-4.com" }
 ]
 maintainers = [
@@ -27,9 +27,10 @@
 
 [project.urls]
 Repository = "https://github.com/mitsuhiko/minijinja"
 "Issue Tracker" = "https://github.com/mitsuhiko/minijinja/issues"
 "Donate" = "https://github.com/sponsors/mitsuhiko"
 
 [tool.maturin]
+module-name = "minijinja._lowlevel"
 python-source = "python"
 strip = true
```

### Comparing `minijinja-0.32.0/python/minijinja/__init__.py` & `minijinja-1.0.0/python/minijinja/__init__.py`

 * *Files identical despite different names*

### Comparing `minijinja-0.32.0/python/minijinja/_internal.py` & `minijinja-1.0.0/python/minijinja/_internal.py`

 * *Files identical despite different names*

### Comparing `minijinja-0.32.0/src/environment.rs` & `minijinja-1.0.0/src/environment.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 use std::ffi::c_void;
 use std::sync::atomic::{AtomicBool, AtomicPtr, Ordering};
 use std::sync::Mutex;
 
 use minijinja::value::{Rest, Value};
-use minijinja::{
-    context, escape_formatter, AutoEscape, Error, Source, State, Syntax, UndefinedBehavior,
-};
+use minijinja::{context, escape_formatter, AutoEscape, Error, State, Syntax, UndefinedBehavior};
 use pyo3::conversion::AsPyPointer;
 use pyo3::exceptions::PyRuntimeError;
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyTuple};
 
 use crate::error_support::{report_unraisable, to_minijinja_error, to_py_error};
 use crate::state::bind_state;
@@ -362,51 +360,47 @@
                 }
                 Some(callback.into())
             }
         };
         let mut inner = self.inner.lock().unwrap();
         inner.loader = callback.clone();
 
-        let mut source = if let Some(callback) = callback {
-            Source::with_loader(move |name| {
+        if let Some(callback) = callback {
+            inner.env.set_loader(move |name| {
                 Python::with_gil(|py| {
                     let callback = callback.as_ref(py);
                     let rv = callback
                         .call1(PyTuple::new(py, [name]))
                         .map_err(to_minijinja_error)?;
                     if rv.is_none() {
                         Ok(None)
                     } else {
                         Ok(Some(rv.to_string()))
                     }
                 })
             })
-        } else {
-            Source::new()
-        };
-        source.set_syntax(Syntax::default()).map_err(to_py_error)?;
-        inner.env.set_source(source);
+        }
 
         Ok(())
     }
 
     /// Returns the current loader.
     #[getter]
     pub fn get_loader(&self) -> Option<Py<PyAny>> {
         self.inner.lock().unwrap().loader.clone()
     }
 
     /// Triggers a reload of the templates.
     pub fn reload(&self) -> PyResult<()> {
-        let loader = self.inner.lock().unwrap().loader.as_ref().cloned();
-        if let Some(loader) = loader {
-            Python::with_gil(|py| self.set_loader(Some(loader.as_ref(py))))
-        } else {
-            Ok(())
+        let mut inner = self.inner.lock().unwrap();
+        let loader = inner.loader.as_ref().cloned();
+        if loader.is_some() {
+            inner.env.clear_templates();
         }
+        Ok(())
     }
 
     /// Can be used to instruct the environment to automatically reload templates
     /// before each render.
     #[setter]
     pub fn set_reload_before_render(&self, yes: bool) {
         self.reload_before_render.store(yes, Ordering::Relaxed);
@@ -474,32 +468,30 @@
 
     #[getter]
     pub fn get_comment_end_string(&self) -> String {
         syntax_getter!(self, comment_end, "#}")
     }
 
     /// Manually adds a template to the environment.
-    pub fn add_template(&self, name: &str, source: &str) -> PyResult<()> {
+    pub fn add_template(&self, name: String, source: String) -> PyResult<()> {
         let mut inner = self.inner.lock().unwrap();
-        if inner.env.source().is_none() {
-            inner.env.set_source(Source::new());
-        }
         inner
             .env
-            .source_mut()
-            .unwrap()
-            .add_template(name, source)
+            .add_template_owned(name, source)
             .map_err(to_py_error)
     }
 
     /// Removes a loaded template.
     pub fn remove_template(&self, name: &str) {
-        if let Some(source) = self.inner.lock().unwrap().env.source_mut() {
-            source.remove_template(name);
-        }
+        self.inner.lock().unwrap().env.remove_template(name);
+    }
+
+    /// Clears all loaded templates.
+    pub fn clear_templates(&self) {
+        self.inner.lock().unwrap().env.clear_templates();
     }
 
     /// Renders a template looked up from the loader.
     ///
     /// The first argument is the name of the template, all other arguments must be passed
     /// as keyword arguments and are pass as render context of the template.
     #[pyo3(signature = (template_name, /, **ctx))]
```

### Comparing `minijinja-0.32.0/src/error_support.rs` & `minijinja-1.0.0/src/error_support.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.32.0/src/state.rs` & `minijinja-1.0.0/src/state.rs`

 * *Files 18% similar despite different names*

```diff
@@ -45,20 +45,14 @@
 
     /// Returns the current block
     #[getter]
     pub fn get_current_block(&self) -> PyResult<Option<String>> {
         with_state(|state| Ok(state.current_block().map(|x| x.into())))
     }
 
-    /// Returns the current call
-    #[getter]
-    pub fn get_current_call(&self) -> PyResult<Option<String>> {
-        with_state(|state| Ok(state.current_call().map(|x| x.into())))
-    }
-
     /// Looks up a variable in the context
     #[pyo3(text_signature = "(self, name)")]
     pub fn lookup(&self, name: &str) -> PyResult<Py<PyAny>> {
         with_state(|state| {
             state
                 .lookup(name)
                 .map(to_python_value)
```

### Comparing `minijinja-0.32.0/src/typeconv.rs` & `minijinja-1.0.0/src/typeconv.rs`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     fn get_field(&self, name: &str) -> Option<Value> {
         Python::with_gil(|py| {
             let inner = self.inner.as_ref(py);
             inner.get_item(name).map(to_minijinja_value)
         })
     }
 
-    fn fields(&self) -> Vec<Arc<String>> {
+    fn fields(&self) -> Vec<Arc<str>> {
         Python::with_gil(|py| {
             let inner = self.inner.as_ref(py);
             inner.keys().iter().map(|x| x.to_string().into()).collect()
         })
     }
 }
 
@@ -256,21 +256,14 @@
                     Ok(rv.into_py(py))
                 } else if let Ok(rv) = TryInto::<f64>::try_into(value) {
                     Ok(rv.into_py(py))
                 } else {
                     unreachable!()
                 }
             }
-            ValueKind::Char => {
-                if let Ok(rv) = TryInto::<char>::try_into(value.clone()) {
-                    Ok(rv.into_py(py))
-                } else {
-                    unreachable!()
-                }
-            }
             ValueKind::String => {
                 if value.is_safe() {
                     Ok(mark_string_safe(py, value.as_str().unwrap())?)
                 } else {
                     Ok(value.as_str().unwrap().into_py(py))
                 }
             }
```

### Comparing `minijinja-0.32.0/tests/test_basic.py` & `minijinja-1.0.0/tests/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     env = Environment()
     rv = env.eval_expr("[hmm.public_attr, hmm.__module__]", hmm=hmm)
     assert rv == [42, None]
 
 
 def test_generator():
     def hmm():
-        # this implicity gets converted into a list. it's not a real iterator
+        # This implicitly gets converted into a list. It's not a real iterator.
         yield 1
         yield 2
         yield 3
 
     hmm.public_attr = 42
     env = Environment()
     rv = env.eval_expr("values|list", values=hmm())
@@ -107,18 +107,18 @@
     assert env.render_template("index.html") == "Hello from index.html"
     assert env.render_template("index.html") == "Hello from index.html"
     assert env.render_template("other.html") == "Hello from other.html"
     assert env.loader is my_loader
     assert called == ["index.html", "other.html"]
     env.loader = my_loader
     assert env.render_template("index.html") == "Hello from index.html"
-    assert called == ["index.html", "other.html", "index.html"]
+    assert called == ["index.html", "other.html"]
     env.reload()
     assert env.render_template("index.html") == "Hello from index.html"
-    assert called == ["index.html", "other.html", "index.html", "index.html"]
+    assert called == ["index.html", "other.html", "index.html"]
 
 
 def test_loader_reload():
     called = []
 
     def my_loader(name):
         called.append(name)
```

### Comparing `minijinja-0.32.0/tests/test_security.py` & `minijinja-1.0.0/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `minijinja-0.32.0/tests/test_state.py` & `minijinja-1.0.0/tests/test_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     env = Environment()
 
     @pass_state
     def my_func(state):
         assert state.name == "template-name"
         assert state.auto_escape is None
         assert state.current_block == "foo"
-        assert state.current_call == "my_func"
         assert state.lookup("bar") == 23
         assert state.lookup("aha") is None
         assert state.lookup("my_func") is my_func
         assert state.env is env
         return 42
 
     rv = env.render_str(
@@ -29,15 +28,14 @@
     env = Environment()
 
     @pass_state
     def my_func(state):
         assert state.name == "template-name"
         assert state.auto_escape is None
         assert state.current_block == "foo"
-        assert state.current_call == "my_func"
         assert state.lookup("bar") == 23
         assert state.lookup("aha") is None
         assert state.env is env
         return 42
 
     env.add_global("my_func", my_func)
 
@@ -53,15 +51,14 @@
     env = Environment()
 
     @pass_state
     def my_filter(state, value):
         assert state.name == "template-name"
         assert state.auto_escape is None
         assert state.current_block == "foo"
-        assert state.current_call == "myfilter"
         assert state.lookup("bar") == 23
         assert state.lookup("aha") is None
         assert state.env is env
         return value
 
     env.add_filter("myfilter", my_filter)
 
@@ -77,15 +74,14 @@
     env = Environment()
 
     @pass_state
     def my_test(state, value):
         assert state.name == "template-name"
         assert state.auto_escape is None
         assert state.current_block == "foo"
-        assert state.current_call == "mytest"
         assert state.lookup("bar") == 23
         assert state.lookup("aha") is None
         assert state.env is env
         return True
 
     env.add_test("mytest", my_test)
```

### Comparing `minijinja-0.32.0/Cargo.lock` & `minijinja-1.0.0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,26 @@
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.0"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
+name = "android-tzdata"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5bce8d450891e3b36f85a2230cec441fddd60e0c455b61b15bb3ffba955ca85"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
@@ -192,34 +201,34 @@
  "lazy_static",
  "memchr",
  "regex-automata",
 ]
 
 [[package]]
 name = "bstr"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3d4260bcc2e8fc9df1eac4919a720effeb63a3f0952f5bf4944adfa18897f09"
+checksum = "a246e68bb43f6cd9db24bea052a53e40405417c5fb372e3d1a8a7f770a564ef5"
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "build-script"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
@@ -233,20 +242,20 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
- "num-integer",
  "num-traits",
  "winapi",
 ]
 
 [[package]]
 name = "chrono-tz"
 version = "0.6.1"
@@ -267,44 +276,44 @@
  "parse-zoneinfo",
  "phf",
  "phf_codegen",
 ]
 
 [[package]]
 name = "ciborium"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0c137568cc60b904a7724001b35ce2630fd00d5d84805fbb608ab89509d788f"
+checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
  "serde",
 ]
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "346de753af073cc87b52b2083a506b38ac176a44cfb05497b622e27be899b369"
+checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
 
 [[package]]
 name = "ciborium-ll"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213030a2b5a4e0c0892b6652260cf6ccac84827b83a85a534e178e3906c4cf1b"
+checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "bitflags",
  "clap_lex",
  "indexmap",
  "textwrap",
 ]
 
@@ -314,33 +323,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
 dependencies = [
  "os_str_bytes",
 ]
 
 [[package]]
-name = "codespan-reporting"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
-
-[[package]]
 name = "console"
-version = "0.15.5"
+version = "0.15.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3d79fbe8970a77e3e34151cc13d3b3e248aa0faaecb9f6091fa07ebefe5ad60"
+checksum = "c926e00cc70edefdc64d3a5ff31cc65bb97a3460097762bd23afb4d8145fccf8"
 dependencies = [
  "encode_unicode",
  "lazy_static",
  "libc",
- "windows-sys 0.42.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "console_error_panic_hook"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a06aeb73f470f66dcdbf7223caeebb85984942f22f1adb2a088cf9668146bbbc"
@@ -353,17 +352,17 @@
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.6"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "280a9f2d8b3a38871a3c8a46fb80db65e5e5ed97da80c4d08bf27fb63e35e181"
+checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "criterion"
 version = "0.4.0"
@@ -419,30 +418,30 @@
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset",
+ "memoffset 0.9.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
@@ -450,55 +449,18 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
-name = "cxx"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12cee708e8962df2aeb38f594aae5d827c022b6460ac71a7a3e2c3c2aae5a07b"
-dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
- "proc-macro2",
- "quote",
- "scratch",
- "syn 2.0.15",
-]
-
-[[package]]
-name = "cxxbridge-flags"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
-
-[[package]]
-name = "cxxbridge-macro"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
+name = "custom-loader"
+version = "0.1.0"
 dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.15",
+ "minijinja",
 ]
 
 [[package]]
 name = "debug"
 version = "0.1.0"
 dependencies = [
  "minijinja",
@@ -508,29 +470,36 @@
 name = "deunicode"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "850878694b7933ca4c9569d30a34b55031b9b139ee1fc7b94a527c4ef960d690"
 
 [[package]]
 name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
+name = "dsl"
+version = "0.1.0"
+dependencies = [
+ "minijinja",
+]
+
+[[package]]
 name = "dynamic-context"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
@@ -556,14 +525,21 @@
 name = "error"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
+name = "eval-to-state"
+version = "0.1.0"
+dependencies = [
+ "minijinja",
+]
+
+[[package]]
 name = "expr"
 version = "0.1.0"
 dependencies = [
  "minijinja",
  "serde_json",
 ]
 
@@ -571,15 +547,15 @@
 name = "filetime"
 version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "filters"
 version = "0.1.0"
 dependencies = [
@@ -590,17 +566,17 @@
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "fsevent-sys"
 version = "4.1.0"
@@ -650,15 +626,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -702,31 +678,31 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "globset"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "029d74589adefde59de1a0c4f4732695c32805624aec7b68d91503d4dba79afc"
 dependencies = [
  "aho-corasick 0.7.20",
- "bstr 1.4.0",
+ "bstr 1.5.0",
  "fnv",
  "log",
  "regex",
 ]
 
 [[package]]
 name = "globwalk"
@@ -908,17 +884,17 @@
 name = "half"
 version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
 
 [[package]]
 name = "handlebars"
-version = "4.3.6"
+version = "4.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "035ef95d03713f2c347a72547b7cd38cbc9af7cd51e6099fb62d586d4a6dee3a"
+checksum = "83c3372087601b532857d332f5957cbae686da52bb7810bf038c3e3c3cc2fa0d"
 dependencies = [
  "log",
  "pest",
  "pest_derive",
  "serde",
  "serde_json",
  "thiserror",
@@ -968,34 +944,33 @@
 checksum = "6cb51c9a029ddc91b07a787f1d86b53ccfa49b0e86688c946ebe8d3555685dd7"
 dependencies = [
  "libm",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.56"
+version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "ignore"
 version = "0.4.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dbe7873dab538a9a44ad79ede1faf5f30d49f9a5c883ddbab48bce81b64b7492"
@@ -1102,17 +1077,17 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "kqueue"
 version = "1.0.7"
@@ -1147,57 +1122,48 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "libm"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
-
-[[package]]
-name = "link-cplusplus"
-version = "1.0.8"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
-dependencies = [
- "cc",
-]
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
 name = "liquid"
-version = "0.26.1"
+version = "0.26.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9dfb833f0d41ed59a6c8d28e2f36d0362557c43fa83e9e096dd74e6e9517858f"
+checksum = "69f68ae1011499ae2ef879f631891f21c78e309755f4a5e483c4a8f12e10b609"
 dependencies = [
  "doc-comment",
  "liquid-core",
  "liquid-derive",
  "liquid-lib",
  "serde",
 ]
 
 [[package]]
 name = "liquid-core"
-version = "0.26.1"
+version = "0.26.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca2b58598eeb2cd39ea0e0b6c666bab002b4f58ebbeedcc649d164d6dec4b886"
+checksum = "79e0724dfcaad5cfb7965ea0f178ca0870b8d7315178f4a7179f5696f7f04d5f"
 dependencies = [
  "anymap2",
  "itertools",
  "kstring",
  "liquid-derive",
  "num-traits",
  "pest",
@@ -1205,28 +1171,28 @@
  "regex",
  "serde",
  "time",
 ]
 
 [[package]]
 name = "liquid-derive"
-version = "0.26.1"
+version = "0.26.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "611c6adfb96294233bd6f20125684a6e3dd28c3f0d057d50a65adf2426ed3f47"
+checksum = "fc2fb41a9bb4257a3803154bdf7e2df7d45197d1941c9b1a90ad815231630721"
 dependencies = [
  "proc-macro2",
- "proc-quote",
- "syn 1.0.109",
+ "quote",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "liquid-lib"
-version = "0.26.1"
+version = "0.26.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3ffe1daafef416a71da31385dd3764906cbde22349767a8458d30c96644a512"
+checksum = "e2a17e273a6fb1fb6268f7a5867ddfd0bd4683c7e19b51084f3d567fad4348c0"
 dependencies = [
  "itertools",
  "liquid-core",
  "once_cell",
  "percent-encoding",
  "regex",
  "time",
@@ -1246,38 +1212,28 @@
 version = "0.1.0"
 dependencies = [
  "minijinja",
  "serde_json",
 ]
 
 [[package]]
-name = "loader"
-version = "0.1.0"
-dependencies = [
- "minijinja",
-]
-
-[[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "macros"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
@@ -1300,14 +1256,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "mime_guess"
@@ -1317,40 +1282,41 @@
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
 name = "minijinja"
-version = "0.32.0"
+version = "1.0.0"
 dependencies = [
- "aho-corasick 1.0.0",
+ "aho-corasick 1.0.2",
  "indexmap",
  "insta",
  "memo-map",
  "percent-encoding",
  "self_cell",
  "serde",
  "serde_json",
  "similar-asserts",
+ "unicase",
  "unicode-ident",
  "v_htmlescape",
 ]
 
 [[package]]
 name = "minijinja-autoreload"
-version = "0.32.0"
+version = "1.0.0"
 dependencies = [
  "minijinja",
  "notify",
 ]
 
 [[package]]
 name = "minijinja-contrib"
-version = "0.32.0"
+version = "1.0.0"
 dependencies = [
  "minijinja",
  "similar-asserts",
 ]
 
 [[package]]
 name = "minijinja-dis"
@@ -1358,24 +1324,24 @@
 dependencies = [
  "argh",
  "minijinja",
 ]
 
 [[package]]
 name = "minijinja-py"
-version = "0.32.0"
+version = "1.0.0"
 dependencies = [
  "minijinja",
  "once_cell",
  "pyo3",
 ]
 
 [[package]]
 name = "minijinja-stack-ref"
-version = "0.32.0"
+version = "1.0.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "minimal"
 version = "0.1.0"
@@ -1387,59 +1353,49 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "mio"
-version = "0.8.6"
+version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
  "log",
  "wasi",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "notify"
-version = "5.1.0"
+version = "5.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ea850aa68a06e48fdb069c0ec44d0d64c8dbffa49bf3b6f7f0a901fdea1ba9"
+checksum = "729f63e1ca555a43fe3efa4f3efdf4801c479da85b432242a7b726f353c88486"
 dependencies = [
  "bitflags",
  "filetime",
  "fsevent-sys",
  "inotify",
  "kqueue",
  "libc",
  "mio",
  "walkdir",
- "windows-sys 0.42.0",
-]
-
-[[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
@@ -1455,106 +1411,114 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "os_str_bytes"
-version = "6.5.0"
+version = "6.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
+checksum = "4d5d9eb14b174ee9aa2ef96dc2b94637a2d4b6e7cb873c7e171f0c20c6cf3eac"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "parse-zoneinfo"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
 dependencies = [
  "regex",
 ]
 
 [[package]]
+name = "path-loader"
+version = "0.1.0"
+dependencies = [
+ "minijinja",
+ "once_cell",
+]
+
+[[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pest"
-version = "2.5.7"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1403e8401ad5dedea73c626b99758535b342502f8d1e361f4a2dd952749122"
+checksum = "e68e84bfb01f0507134eac1e9b410a12ba379d064eab48c50ba4ce329a527b70"
 dependencies = [
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_derive"
-version = "2.5.7"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be99c4c1d2fc2769b1d00239431d711d08f6efedcecb8b6e30707160aee99c15"
+checksum = "6b79d4c71c865a25a4322296122e3924d30bc8ee0834c8bfc8b95f7f054afbfb"
 dependencies = [
  "pest",
  "pest_generator",
 ]
 
 [[package]]
 name = "pest_generator"
-version = "2.5.7"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e56094789873daa36164de2e822b3888c6ae4b4f9da555a1103587658c805b1e"
+checksum = "6c435bf1076437b851ebc8edc3a18442796b30f1728ffea6262d59bbe28b077e"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.5.7"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6733073c7cff3d8459fda0e42f13a047870242aed8b509fe98000928975f359e"
+checksum = "745a452f8eb71e39ffd8ee32b3c5f51d03845f99786fa9b68db6ff509c505411"
 dependencies = [
  "once_cell",
  "pest",
  "sha2",
 ]
 
 [[package]]
@@ -1594,30 +1558,30 @@
 dependencies = [
  "siphasher",
  "uncased",
 ]
 
 [[package]]
 name = "pin-project"
-version = "1.0.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad29a609b6bcd67fee905812e544992d216af9d755757c05ed2d0e15a74c6ecc"
+checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.0.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "069bdb1e05adc7a8990dce9cc75370895fbe4e3d58b9b73bf1aee56359344a55"
+checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
@@ -1704,53 +1668,23 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
-name = "proc-macro-hack"
-version = "0.5.20+deprecated"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
-
-[[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
-name = "proc-quote"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e84ab161de78c915302ca325a19bee6df272800e2ae1a43fe3ef430bab2a100"
-dependencies = [
- "proc-macro-hack",
- "proc-macro2",
- "proc-quote-impl",
- "quote",
- "syn 1.0.109",
-]
-
-[[package]]
-name = "proc-quote-impl"
-version = "0.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fb3ec628b063cdbcf316e06a8b8c1a541d28fa6c0a8eacd2bfb2b7f49e88aa0"
-dependencies = [
- "proc-macro-hack",
- "proc-macro2",
- "quote",
-]
-
-[[package]]
 name = "prokio"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03b55e106e5791fa5a13abd13c85d6127312e8e09098059ca2bc9b03ca4cf488"
 dependencies = [
  "futures",
  "gloo",
@@ -1768,15 +1702,15 @@
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
+ "memoffset 0.8.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "serde",
  "unindent",
 ]
@@ -1822,17 +1756,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1899,35 +1833,44 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
- "aho-corasick 0.7.20",
+ "aho-corasick 1.0.2",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "render-macro"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
@@ -1972,30 +1915,24 @@
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
-name = "scratch"
-version = "1.0.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
-
-[[package]]
 name = "self_cell"
-version = "0.10.2"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ef965a420fe14fdac7dd018862966a4c14094f900e1650bbc71ddd7d580c8af"
+checksum = "4c309e515543e67811222dbc9e3dd7e1056279b782e1dacffe4242b718734fb6"
 
 [[package]]
 name = "serde"
-version = "1.0.160"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.4.5"
@@ -2005,28 +1942,28 @@
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.160"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2039,17 +1976,17 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
@@ -2099,22 +2036,14 @@
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
-name = "source"
-version = "0.1.0"
-dependencies = [
- "minijinja",
- "once_cell",
-]
-
-[[package]]
 name = "stack-ref"
 version = "0.1.0"
 dependencies = [
  "minijinja",
  "minijinja-stack-ref",
 ]
 
@@ -2133,34 +2062,34 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tera"
-version = "1.18.1"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95a665751302f22a03c56721e23094e4dc22b04a80f381e6737a07bf7a7c70c0"
+checksum = "a5ab29bb4f3e256ae6ad5c3e2775aa1f8829f2c0c101fc407bfd3a6df15c60c5"
 dependencies = [
  "chrono",
  "chrono-tz",
  "globwalk",
  "humansize 2.1.3",
  "lazy_static",
  "percent-encoding",
@@ -2172,23 +2101,14 @@
  "serde_json",
  "slug",
  "thread_local",
  "unic-segment",
 ]
 
 [[package]]
-name = "termcolor"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
-dependencies = [
- "winapi-util",
-]
-
-[[package]]
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
 [[package]]
 name = "thiserror"
@@ -2203,49 +2123,49 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5516c27b78311c50bf42c071425c560ac799b11c30b31f87e3081965fe5e0180"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.20"
+version = "0.3.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
 dependencies = [
  "itoa",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tinytemplate"
 version = "1.2.1"
@@ -2254,28 +2174,28 @@
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.27.0"
+version = "1.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0de47a4eecbe11f498978a9b29d792f0d2692d1dd003650c24c76510e3bc001"
+checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
 dependencies = [
  "autocfg",
  "pin-project-lite",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-stream"
-version = "0.1.12"
+version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8fb52b74f05dbf495a8fba459fdc331812b96aa086d9eb78101fa0d4569c3313"
+checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
@@ -2297,28 +2217,28 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.16.0"
@@ -2329,17 +2249,17 @@
 name = "ucd-trie"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
 
 [[package]]
 name = "uncased"
-version = "0.9.7"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09b01702b0fd0b3fadcf98e098780badda8742d4f4a7676615cad90e8ac73622"
+checksum = "9b9bc53168a4be7402ab86c3aad243a84dd7381d09be0eddc81280c1da95ca68"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "unic-char-property"
 version = "0.9.0"
@@ -2397,31 +2317,25 @@
 checksum = "50f37be617794602aabbeee0be4f259dc1778fabe05e2d67ee8f79326d5cb4f6"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-segmentation"
 version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
 
 [[package]]
-name = "unicode-width"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
-
-[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "v_htmlescape"
@@ -2449,93 +2363,93 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.34"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f219e0d211ba40266969f6dbdd90636da12f75bee4fc9d6c23d1260dadb51454"
+checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "wasm-yew"
 version = "0.1.0"
 dependencies = [
  "minijinja",
  "serde_json",
  "web-sys",
  "yew",
 ]
 
 [[package]]
 name = "web-sys"
-version = "0.3.61"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -2575,29 +2489,14 @@
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
  "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets 0.42.2",
 ]
```

### Comparing `minijinja-0.32.0/PKG-INFO` & `minijinja-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minijinja
-Version: 0.32.0
+Version: 1.0.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
@@ -71,15 +71,15 @@
 ```python
 result = env.render_template('template_name', var1="value 1", var2="value 2")
 print(result)
 ```
 
 ## Purpose
 
-MiniJinja attemps a certain level of compatibiliy with Jinja2, but it does not
+MiniJinja attempts a certain level of compatibility with Jinja2, but it does not
 try to achieve this at all costs.  As a result you will notice that quite a few
 templates will refuse to render with MiniJinja despite the fact that they probably
 look quite innocent.  It is however possible to write templates that render to the
 same results for both Jinja2 and MiniJinja.  This raises the question why you might
 want to use MiniJinja.
 
 The main benefit would be to achieve the exact same results in both Rust and Python.
@@ -88,17 +88,16 @@
 marshalling that needs to happen in either direction there is a certain amount of
 loss of information.
 
 ## Dynamic Template Loading
 
 MiniJinja's Python bindings inherit the underlying behavior of how MiniJinja loads
 templates.  Templates are loaded on first use and then cached.  The templates are
-loaded via a "source" (called `loader` in MiniJinja's Python bindings).  To trigger
-a reload you can call `env.reload()` or alternatively set `env.reload_before_render`
-to `True`.
+loaded via a loader.  To trigger a reload you can call `env.reload()` or
+alternatively set `env.reload_before_render` to `True`.
 
 ```python
 def my_loader(name):
     segments = []
     for segment in name.split("/"):
         if "\\" in segment or segment in (".", ".."):
             return None
@@ -129,15 +128,15 @@
 MiniJinja uses [markupsafe](https://github.com/pallets/markupsafe) if it's available
 on the Python side.  It will honor `__html__`.
 
 ## Finalizers
 
 Instead of custom formatters like in MiniJinja, you can define a finalizer instead
 which is similar to how it works in Jinja2.  It's passed a value (or optional also
-the state as first argument whne `pass_state` is used) and can return a new value.
+the state as first argument when `pass_state` is used) and can return a new value.
 If the special `NotImplemented` value is returned, the original value is rendered
 without any modification:
 
 ```
 from minijinja import Environment
 
 def finalizer(value):
```

