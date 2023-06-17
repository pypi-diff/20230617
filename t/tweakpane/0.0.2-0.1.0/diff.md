# Comparing `tmp/tweakpane-0.0.2.tar.gz` & `tmp/tweakpane-0.1.0.tar.gz`

## Comparing `tweakpane-0.0.2.tar` & `tweakpane-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tweakpane-0.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 tweakpane-0.0.2/src/tweakpane/__init__.py
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 tweakpane-0.0.2/src/tweakpane/index.js
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tweakpane-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tweakpane-0.0.2/LICENSE
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 tweakpane-0.0.2/README.md
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 tweakpane-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 tweakpane-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tweakpane-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 tweakpane-0.1.0/src/tweakpane/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 tweakpane-0.1.0/src/tweakpane/index.js
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tweakpane-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tweakpane-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 tweakpane-0.1.0/README.md
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 tweakpane-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 tweakpane-0.1.0/PKG-INFO
```

### Comparing `tweakpane-0.0.2/.github/workflows/release.yml` & `tweakpane-0.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tweakpane-0.0.2/src/tweakpane/__init__.py` & `tweakpane-0.1.0/src/tweakpane/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,22 @@
+import contextlib
 from importlib.metadata import PackageNotFoundError, version
+import pathlib
+
+import anywidget
+import traitlets
 
 try:
     __version__ = version("tweakpane")
 except PackageNotFoundError:
     __version__ = "uninstalled"
 
-import contextlib
-
-import anywidget
-import traitlets
-
-__DEV__ = False
-
-if __DEV__:
-    ESM = "http://localhost:5173/src/tweakpane/index.js?anywidget"
-else:
-    import pathlib
-
-    src = pathlib.Path(__file__).parent / "index.js"
-    ESM = src.read_text()
-
 
 class Pane(anywidget.AnyWidget):
-    _esm = traitlets.Unicode(ESM).tag(sync=True)
+    _esm = pathlib.Path(__file__).parent / "index.js"
     _inputs = traitlets.List([]).tag(sync=True)
     _context = None
 
     def _append_input(self, input):
         if self._context is None:
             self._inputs = self._inputs + [input]
         else:
```

### Comparing `tweakpane-0.0.2/src/tweakpane/index.js` & `tweakpane-0.1.0/src/tweakpane/index.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,98 +1,92 @@
 import * as Tweakpane from "https://esm.sh/tweakpane@3";
 
-function addInput(pane, PARAMS, name, options, view) {
+function addInput(pane, PARAMS, name, options, model) {
     pane.addInput(PARAMS, name, options).on("change", (e) => {
         // tweakpane mutates PARAMS in place, so e.value is a reference
         // to the original object. We need to clone objects so that
         // Jupyter actually emits a change on `model.set`
         let value = typeof e.value === "object" ?
             structuredClone(e.value) :
             e.value;
-        view.model.set(name, value, view);
-        view.model.save_changes();
+        model.set(name, value);
+        model.save_changes();
     });
 
-    view.listenTo(view.model, `change:${name}`, (_model, value, context) => {
-        // only need to refresh if change comes from other JS views or Python
-        if (context?.cid === view.cid) {
-            return;
-        }
-        PARAMS[name] = value;
-        pane.refresh();
+    model.on(`change:${name}`, () => {
+        PARAMS[name] = model.get(name);
+        pane.refresh?.();
     });
 }
 
-function addMonitor(pane, PARAMS, name, options, view) {
+function addMonitor(pane, PARAMS, name, options, model) {
     pane.addMonitor(PARAMS, name, options);
-    view.listenTo(view.model, `change:${name}`, (_, value, ctx) => {
-        if (ctx?.cid === view.cid) {
-            return;
-        }
-        PARAMS[name] = value;
+    model.on(`change:${name}`, () => {
+        PARAMS[name] = model.get(name);
     });
 }
 
-function addAll(pane, PARAMS, inputs, view) {
+function addAll(pane, PARAMS, inputs, model) {
     for (let [type, ...rest] of inputs) {
         if (type === "input") {
             let [name, options] = rest;
-            addInput(pane, PARAMS, name, options, view);
+            addInput(pane, PARAMS, name, options, model);
             continue;
         }
         if (type === "monitor") {
             let [name, options] = rest;
-            addMonitor(pane, PARAMS, name, options, view);
+            addMonitor(pane, PARAMS, name, options, model);
             continue;
         }
         if (type === "folder") {
             let [folderOptions, inputs] = rest;
             let folder = pane.addFolder(folderOptions);
-            addAll(folder, PARAMS, inputs, view);
+            addAll(folder, PARAMS, inputs, model);
             continue;
         }
         throw new Error(`Tweakpane type '${type}' not supported.`);
     }
-
 }
 
 function* getNames(inputs) {
     for (let [type, ...rest] of inputs) {
         if (type === "input") {
-            yield rest[0]
+            yield rest[0];
             continue;
         }
         if (type === "monitor") {
-            yield rest[0]
+            yield rest[0];
             continue;
         }
         if (type === "folder") {
-            yield* getNames(rest[1])
+            yield* getNames(rest[1]);
             continue;
         }
         throw new Error(`Tweakpane type '${type}' not supported.`);
-
     }
 }
 
-export function render(view) {
+export function render({
+    model,
+    el
+}) {
     function init(inputs) {
         let pane = new Tweakpane.Pane({
-            container: view.el
+            container: el
         });
         let PARAMS = {};
         for (let name of getNames(inputs)) {
-            PARAMS[name] = view.model.get(name);
+            PARAMS[name] = model.get(name);
         }
-        addAll(pane, PARAMS, inputs, view);
+        addAll(pane, PARAMS, inputs, model);
         return () => {
             pane.dispose();
-            view.stopListening(view.model);
+            model.off();
         };
     }
 
-    let dispose = init(view.model.get("_inputs"));
-    view.model.on("change:_inputs", (_, inputs) => {
+    let dispose = init(model.get("_inputs"));
+    model.on("change:_inputs", (_, inputs) => {
         dispose();
         dispose = init(inputs);
     });
 }
```

### Comparing `tweakpane-0.0.2/LICENSE` & `tweakpane-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tweakpane-0.0.2/README.md` & `tweakpane-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tweakpane-0.0.2/pyproject.toml` & `tweakpane-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-  "anywidget"
+  "anywidget>=0.4.3,<1"
 ]
 
 [project.urls]
 Documentation = "https://github.com/manzt/ipytweakpane#readme"
 Issues = "https://github.com/manzt/ipytweakpane/issues"
 Source = "https://github.com/manzt/ipytweakpane"
```

### Comparing `tweakpane-0.0.2/PKG-INFO` & `tweakpane-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweakpane
-Version: 0.0.2
+Version: 0.1.0
 Summary: Python bindings for Tweakpane UI
 Project-URL: Documentation, https://github.com/manzt/ipytweakpane#readme
 Project-URL: Issues, https://github.com/manzt/ipytweakpane/issues
 Project-URL: Source, https://github.com/manzt/ipytweakpane
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Requires-Dist: anywidget
+Requires-Dist: anywidget<1,>=0.4.3
 Description-Content-Type: text/markdown
 
 # (ipy)tweakpane
 
 [![PyPI](https://img.shields.io/pypi/v/tweakpane.svg?color=green)](https://pypi.org/project/tweakpane)
 [![License](https://img.shields.io/pypi/l/tweakpane.svg?color=green)](https://github.com/manzt/ipytweakpane/raw/main/LICENSE)
```

