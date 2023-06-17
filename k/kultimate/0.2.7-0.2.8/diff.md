# Comparing `tmp/kultimate-0.2.7.tar.gz` & `tmp/kultimate-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kultimate-0.2.7.tar", max compression
+gzip compressed data, was "kultimate-0.2.8.tar", max compression
```

## Comparing `kultimate-0.2.7.tar` & `kultimate-0.2.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3673 2023-06-17 01:35:44.660558 kultimate-0.2.7/README.md
--rw-r--r--   0        0        0      211 2023-06-17 00:35:38.560480 kultimate-0.2.7/kultimate/__init__.py
--rw-r--r--   0        0        0     2191 2023-06-17 00:35:38.560480 kultimate-0.2.7/kultimate/app.css
--rw-r--r--   0        0        0    22125 2023-06-17 01:40:14.290564 kultimate-0.2.7/kultimate/app.py
--rw-r--r--   0        0        0      168 2023-06-17 00:35:38.560480 kultimate-0.2.7/kultimate/screens/__init__.py
--rw-r--r--   0        0        0      897 2023-06-16 20:11:44.883725 kultimate-0.2.7/kultimate/screens/addTask.py
--rw-r--r--   0        0        0     1630 2023-06-17 00:35:38.563814 kultimate-0.2.7/kultimate/screens/create_file.py
--rw-r--r--   0        0        0      992 2023-06-17 00:52:35.603836 kultimate-0.2.7/kultimate/screens/deleteTask.py
--rw-r--r--   0        0        0      986 2023-06-16 20:10:08.290390 kultimate-0.2.7/kultimate/screens/edit_task.py
--rw-r--r--   0        0        0      815 2023-06-15 16:47:43.396777 kultimate-0.2.7/kultimate/screens/selectFile.py
--rw-r--r--   0        0        0      175 2023-06-17 00:35:38.563814 kultimate-0.2.7/kultimate/utils/__init__.py
--rw-r--r--   0        0        0     2372 2023-06-17 00:35:38.563814 kultimate-0.2.7/kultimate/utils/app_config.py
--rw-r--r--   0        0        0     1582 2023-06-17 01:40:35.177231 kultimate-0.2.7/kultimate/utils/create_file.py
--rw-r--r--   0        0        0     2048 2023-06-15 16:30:13.640087 kultimate-0.2.7/kultimate/utils/html_to_markdown.py
--rw-r--r--   0        0        0     1885 2023-06-16 17:10:49.190158 kultimate-0.2.7/kultimate/utils/parser_html.py
--rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.2.7/kultimate/utils/process_yaml.py
--rw-r--r--   0        0        0      743 2023-06-16 16:51:32.056800 kultimate-0.2.7/kultimate/utils/prueba.py
--rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.2.7/kultimate/widgets/__init__.py
--rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.2.7/kultimate/widgets/directory.py
--rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.2.7/kultimate/widgets/stages.py
--rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.2.7/kultimate/widgets/stagesContainer.py
--rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.2.7/kultimate/widgets/task.py
--rw-r--r--   0        0        0      606 2023-06-17 01:41:03.647232 kultimate-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 kultimate-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     3673 2023-06-17 01:35:44.660558 kultimate-0.2.8/README.md
+-rw-r--r--   0        0        0      211 2023-06-17 00:35:38.560480 kultimate-0.2.8/kultimate/__init__.py
+-rw-r--r--   0        0        0     2191 2023-06-17 00:35:38.560480 kultimate-0.2.8/kultimate/app.css
+-rw-r--r--   0        0        0    22125 2023-06-17 01:40:14.290564 kultimate-0.2.8/kultimate/app.py
+-rw-r--r--   0        0        0      168 2023-06-17 00:35:38.560480 kultimate-0.2.8/kultimate/screens/__init__.py
+-rw-r--r--   0        0        0      897 2023-06-16 20:11:44.883725 kultimate-0.2.8/kultimate/screens/addTask.py
+-rw-r--r--   0        0        0     1658 2023-06-17 01:51:58.863913 kultimate-0.2.8/kultimate/screens/create_file.py
+-rw-r--r--   0        0        0      992 2023-06-17 00:52:35.603836 kultimate-0.2.8/kultimate/screens/deleteTask.py
+-rw-r--r--   0        0        0      986 2023-06-16 20:10:08.290390 kultimate-0.2.8/kultimate/screens/edit_task.py
+-rw-r--r--   0        0        0      815 2023-06-15 16:47:43.396777 kultimate-0.2.8/kultimate/screens/selectFile.py
+-rw-r--r--   0        0        0      175 2023-06-17 00:35:38.563814 kultimate-0.2.8/kultimate/utils/__init__.py
+-rw-r--r--   0        0        0     2222 2023-06-17 01:53:14.730581 kultimate-0.2.8/kultimate/utils/app_config.py
+-rw-r--r--   0        0        0     1614 2023-06-17 01:49:15.327242 kultimate-0.2.8/kultimate/utils/create_file.py
+-rw-r--r--   0        0        0     2048 2023-06-15 16:30:13.640087 kultimate-0.2.8/kultimate/utils/html_to_markdown.py
+-rw-r--r--   0        0        0     1885 2023-06-16 17:10:49.190158 kultimate-0.2.8/kultimate/utils/parser_html.py
+-rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.2.8/kultimate/utils/process_yaml.py
+-rw-r--r--   0        0        0      743 2023-06-16 16:51:32.056800 kultimate-0.2.8/kultimate/utils/prueba.py
+-rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.2.8/kultimate/widgets/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.2.8/kultimate/widgets/directory.py
+-rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.2.8/kultimate/widgets/stages.py
+-rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.2.8/kultimate/widgets/stagesContainer.py
+-rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.2.8/kultimate/widgets/task.py
+-rw-r--r--   0        0        0      606 2023-06-17 01:53:34.323915 kultimate-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 kultimate-0.2.8/PKG-INFO
```

### Comparing `kultimate-0.2.7/README.md` & `kultimate-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.7/kultimate/app.css` & `kultimate-0.2.8/kultimate/app.css`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.7/kultimate/app.py` & `kultimate-0.2.8/kultimate/app.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.7/kultimate/screens/addTask.py` & `kultimate-0.2.8/kultimate/screens/addTask.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.7/kultimate/screens/create_file.py` & `kultimate-0.2.8/kultimate/screens/create_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     def action_exit(self) -> None:
         """Salir"""
         self.dismiss({"name_file": "", "columns": 0})
 
     def on_radio_set_changed(self, event: RadioSet.Changed) -> None:
         el_input = self.query_one(Input)
         name_file = el_input.value
+        el_input.value = ""
         index = event.radio_set.pressed_index
         self.dismiss({"name_file": name_file, "columns": index})
 
     def on_input_submitted(self, event: Input.Submitted) -> None:
         the_text = event.input.value
         event.input.value = ""
         if event.input.id == "question-1":
```

### Comparing `kultimate-0.2.7/kultimate/screens/deleteTask.py` & `kultimate-0.2.8/kultimate/screens/deleteTask.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.7/kultimate/screens/edit_task.py` & `kultimate-0.2.8/kultimate/screens/edit_task.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.7/kultimate/screens/selectFile.py` & `kultimate-0.2.8/kultimate/screens/selectFile.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.7/kultimate/utils/app_config.py` & `kultimate-0.2.8/kultimate/utils/app_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,19 +18,14 @@
 
 default_config = ConfigParser()
 
 default_config["WORKING_DIRECTORY"] = {
     "path": f"{user_home_directory}/kultimate",
 }
 
-default_config["SKELETONS"] = {
-    "three_stages": ["ToDo", "Doing", "Done"],
-    "five_stages": ["BackLog", "ToDo", "Doing", "Waiting", "Done"],
-}
-
 
 def check_directory(path: str) -> None:
     """Verifica si existe el directorio, si no, sale del programa"""
     working_directory_exists = exists(path)
     if working_directory_exists:
         main(path)
     else:
```

### Comparing `kultimate-0.2.7/kultimate/utils/create_file.py` & `kultimate-0.2.8/kultimate/utils/create_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import json
-from configparser import ConfigParser
+# import json
+# from configparser import ConfigParser
 from os.path import exists
 from pathlib import Path
 
 user_home_directory = Path.home()
 path_file_config = f"{user_home_directory}/.kultimate.ini"
-config_object = ConfigParser()
+# config_object = ConfigParser()
 
 
 def create_new_markdown_file(directory: str, dictio: dict) -> bool:
     """Create a new markdown directory on directory"""
 
     if not dictio["name_file"]:
         return False
 
-    file_config_exists = exists(path_file_config)
+    # file_config_exists = exists(path_file_config)
 
     stages_three = ["ToDo", "Doing", "Done"]
     stages_five = ["BackLog", "ToDo", "Doing", "Waiting", "Done"]
 
-    if file_config_exists:
-        config_object.read(path_file_config)
+    # if file_config_exists:
+    #     config_object.read(path_file_config)
 
-        if "SKELETONS" in config_object:
-            try:
-                stages_three = json.loads(
-                    config_object.get("SKELETONS", "three_stages"),
-                )
-                stages_five = json.loads(
-                    config_object.get("SKELETONS", "five_stages"),
-                )
-            except IndexError:
-                pass
+    #     if "SKELETONS" in config_object:
+    #         try:
+    #             stages_three = json.loads(
+    #                 config_object.get("SKELETONS", "three_stages"),
+    #             )
+    #             stages_five = json.loads(
+    #                 config_object.get("SKELETONS", "five_stages"),
+    #             )
+    #         except IndexError:
+    #             pass
 
     name_file = dictio["name_file"]
     if not name_file.endswith(".md"):
         name_file += ".md"
 
     new_file = f"{directory}/{name_file}"
```

### Comparing `kultimate-0.2.7/kultimate/utils/html_to_markdown.py` & `kultimate-0.2.8/kultimate/utils/html_to_markdown.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.7/kultimate/utils/parser_html.py` & `kultimate-0.2.8/kultimate/utils/parser_html.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.7/kultimate/utils/process_yaml.py` & `kultimate-0.2.8/kultimate/utils/process_yaml.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.7/kultimate/utils/prueba.py` & `kultimate-0.2.8/kultimate/utils/prueba.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.7/kultimate/widgets/directory.py` & `kultimate-0.2.8/kultimate/widgets/directory.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.7/pyproject.toml` & `kultimate-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kultimate"
-version = "0.2.7"
+version = "0.2.8"
 description = ""
 authors = ["Felipe <104157442+justafewwords4@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 textual = { extras = ["dev"], version = "^0.27.0" }
```

### Comparing `kultimate-0.2.7/PKG-INFO` & `kultimate-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kultimate
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 Author: Felipe
 Author-email: 104157442+justafewwords4@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

