# Comparing `tmp/kultimate-0.2.2.tar.gz` & `tmp/kultimate-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kultimate-0.2.2.tar", max compression
+gzip compressed data, was "kultimate-0.2.3.tar", max compression
```

## Comparing `kultimate-0.2.2.tar` & `kultimate-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     3303 2023-06-15 16:08:28.186725 kultimate-0.2.2/README.md
--rw-r--r--   0        0        0       22 2023-06-05 20:11:41.877983 kultimate-0.2.2/kultimate/__init__.py
--rw-r--r--   0        0        0     1475 2023-06-15 17:00:17.893459 kultimate-0.2.2/kultimate/app.css
--rw-r--r--   0        0        0    20867 2023-06-16 17:10:05.146824 kultimate-0.2.2/kultimate/app.py
--rw-r--r--   0        0        0      100 2023-06-15 16:48:15.913444 kultimate-0.2.2/kultimate/screens/__init__.py
--rw-r--r--   0        0        0      896 2023-06-14 18:50:13.597219 kultimate-0.2.2/kultimate/screens/addTask.py
--rw-r--r--   0        0        0      988 2023-06-14 16:24:13.233698 kultimate-0.2.2/kultimate/screens/deleteTask.py
--rw-r--r--   0        0        0      815 2023-06-15 16:47:43.396777 kultimate-0.2.2/kultimate/screens/selectFile.py
--rw-r--r--   0        0        0      125 2023-06-09 21:48:51.262790 kultimate-0.2.2/kultimate/utils/__init__.py
--rw-r--r--   0        0        0     2068 2023-06-12 23:04:04.110731 kultimate-0.2.2/kultimate/utils/app_config.py
--rw-r--r--   0        0        0     2048 2023-06-15 16:30:13.640087 kultimate-0.2.2/kultimate/utils/html_to_markdown.py
--rw-r--r--   0        0        0     1885 2023-06-16 17:10:49.190158 kultimate-0.2.2/kultimate/utils/parser_html.py
--rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.2.2/kultimate/utils/process_yaml.py
--rw-r--r--   0        0        0      743 2023-06-16 16:51:32.056800 kultimate-0.2.2/kultimate/utils/prueba.py
--rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.2.2/kultimate/widgets/__init__.py
--rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.2.2/kultimate/widgets/directory.py
--rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.2.2/kultimate/widgets/stages.py
--rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.2.2/kultimate/widgets/stagesContainer.py
--rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.2.2/kultimate/widgets/task.py
--rw-r--r--   0        0        0      606 2023-06-16 17:15:41.136831 kultimate-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3930 1970-01-01 00:00:00.000000 kultimate-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3324 2023-06-16 17:23:36.106841 kultimate-0.2.3/README.md
+-rw-r--r--   0        0        0       22 2023-06-05 20:11:41.877983 kultimate-0.2.3/kultimate/__init__.py
+-rw-r--r--   0        0        0     1485 2023-06-16 17:46:06.106871 kultimate-0.2.3/kultimate/app.css
+-rw-r--r--   0        0        0    21568 2023-06-16 18:09:25.626901 kultimate-0.2.3/kultimate/app.py
+-rw-r--r--   0        0        0      132 2023-06-16 17:31:28.773518 kultimate-0.2.3/kultimate/screens/__init__.py
+-rw-r--r--   0        0        0      895 2023-06-16 18:08:55.503567 kultimate-0.2.3/kultimate/screens/addTask.py
+-rw-r--r--   0        0        0      988 2023-06-14 16:24:13.233698 kultimate-0.2.3/kultimate/screens/deleteTask.py
+-rw-r--r--   0        0        0      983 2023-06-16 18:08:37.863566 kultimate-0.2.3/kultimate/screens/edit_task.py
+-rw-r--r--   0        0        0      815 2023-06-15 16:47:43.396777 kultimate-0.2.3/kultimate/screens/selectFile.py
+-rw-r--r--   0        0        0      125 2023-06-09 21:48:51.262790 kultimate-0.2.3/kultimate/utils/__init__.py
+-rw-r--r--   0        0        0     2068 2023-06-12 23:04:04.110731 kultimate-0.2.3/kultimate/utils/app_config.py
+-rw-r--r--   0        0        0     2048 2023-06-15 16:30:13.640087 kultimate-0.2.3/kultimate/utils/html_to_markdown.py
+-rw-r--r--   0        0        0     1885 2023-06-16 17:10:49.190158 kultimate-0.2.3/kultimate/utils/parser_html.py
+-rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.2.3/kultimate/utils/process_yaml.py
+-rw-r--r--   0        0        0      743 2023-06-16 16:51:32.056800 kultimate-0.2.3/kultimate/utils/prueba.py
+-rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.2.3/kultimate/widgets/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.2.3/kultimate/widgets/directory.py
+-rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.2.3/kultimate/widgets/stages.py
+-rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.2.3/kultimate/widgets/stagesContainer.py
+-rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.2.3/kultimate/widgets/task.py
+-rw-r--r--   0        0        0      606 2023-06-16 18:11:27.996904 kultimate-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 kultimate-0.2.3/PKG-INFO
```

### Comparing `kultimate-0.2.2/README.md` & `kultimate-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 | o                   | Agregar tarea al final de la columna actual   |
 | ctrl+l              | Mueve la tarea a la última columna            |
 | ctrl+d              | Borra la tarea seleccionada                   |
 | q                   | Salir de la aplicación                        |
 
 ## ToDo
 
-- FIXME: Al mover las tareas entre columnas visualmente se ve bien, pero al
+- TODO: Editar tareas
+- DONE: Al mover las tareas entre columnas visualmente se ve bien, pero al
   grabar a disco se queda en todas las columnas por donde pasa.
 - TODO: Reducir el tamaño de la caja para capturar las tareas.
 - TODO: Rehacer la configuración de la aplicación.
 - TODO: Hacer esqueleto para crear los nuevos archivos.
 - TODO: Crear nuevo archivo.
 - TODO: Si no existe directorio pedirlo.
 - TODO: Agregar columnas.
```

### Comparing `kultimate-0.2.2/kultimate/app.css` & `kultimate-0.2.3/kultimate/app.css`

 * *Files 7% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ._actual > Task._active {
   color: $background-darken-3;
   border: inner $error-lighten-2;
   background: $warning-lighten-1;
 }
 
-DeleteTask, AddTask, SelectAFile {
+DeleteTask, AddTask, SelectAFile, EditTask {
   align: center middle;
 }
 
 #dialog {
   grid-size: 2;
   grid-gutter: 1 2;
   grid-rows: 1fr 3;
```

### Comparing `kultimate-0.2.2/kultimate/app.py` & `kultimate-0.2.3/kultimate/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 from textual.app import App, ComposeResult
 from textual.css.query import QueryError
 from textual.reactive import var
 from textual.widgets import Footer, Header
 
-from .screens import AddTask, DeleteTask, SelectAFile
+from .screens import AddTask, DeleteTask, EditTask, SelectAFile
 from .utils import ParserMarkdown, StagesToMarkdown
 from .widgets import Directory, Stage, StagesContainer, Task
 
 # DONE: Hay errores al navegar entre las columnas.
 
 
 class KanbanUltimate(App):
@@ -18,21 +18,23 @@
     TITLE = "KUltimate"
     SUB_TITLE = "Using Kanban with Markdown"
     CSS_PATH = "app.css"
     SCREENS = {
         "delete_task": DeleteTask,
         "add_task": AddTask,
         "select_file": SelectAFile,
+        "edit_task": EditTask,
     }
 
     BINDINGS = [
         ("s", "select_file", "Select File"),
         # opción temporal, el archivo se debe guardar
         # cada que se modifique el contenido
         ("o", "add_task", "Add Task"),  # DONE: Guardar archivo
+        ("e", "edit_task", "Edit Task"),  # DONE: Guardar archivo
         ("ctrl+l", "mark_as_done", "Mark as Done"),  # DONE: Guardar archivo
         ("ctrl+d", "delete_task", "Delete Task"),  # DONE: Guardar archivo
         ("q", "quit", "Quit"),
         # inician las teclas sin leyendas
         ("l, right", "go_to_right"),
         ("h, left", "go_to_left"),
         ("j, down", "go_to_down"),
@@ -133,22 +135,22 @@
         """Add class self.class_for_active_task"""
         try:
             self.list_tasks[current_task].add_class(self.class_for_active_task)
             self.list_tasks[current_task].scroll_visible(force=True)
         except IndexError:
             pass
 
-    def __remove_class_for_active_task(self, current_task: int) -> None:
-        """Add class self.class_for_active_task"""
-        try:
-            self.list_tasks[current_task].remove_class(
-                self.class_for_active_task,
-            )
-        except IndexError:
-            pass
+    # def __remove_class_for_active_task(self, current_task: int) -> None:
+    #     """Add class self.class_for_active_task"""
+    #     try:
+    #         self.list_tasks[current_task].remove_class(
+    #             self.class_for_active_task,
+    #         )
+    #     except IndexError:
+    #         pass
 
     def __add_class_for_active_stage(self, stage: int) -> None:
         """Add class self.class_for_active_stage"""
         try:
             self.list_stages[stage].add_class(self.class_for_active_stage)
         except IndexError:
             pass
@@ -249,14 +251,29 @@
                 self.__save_to_file()
 
         if self.actual_file:
             self.push_screen("add_task", get_value_from_input)
         else:
             self.push_screen("select_file")
 
+    def action_edit_task(self) -> None:
+        """Edit self.current_task"""
+
+        def new_value_for_task(new_text_for_task: str) -> None:
+            """Obtiene el valor de la tarea"""
+            self.list_tasks[self.current_task].update(new_text_for_task)
+            # guardar al archivo
+            self.__save_to_file()
+
+        if self.actual_file:
+            task_text = str(self.list_tasks[self.current_task].renderable)
+            screen_edit = EditTask()
+            screen_edit.set_text(task_text)
+            self.push_screen(screen_edit, new_value_for_task)
+
     def action_delete_task(self) -> None:
         """Delete task from stage"""
 
         async def check_delete_task(delete_task: bool) -> None:
             """Called when DeleteTask is dismissed"""
             if delete_task:
                 if len(self.list_tasks) > 0:
```

### Comparing `kultimate-0.2.2/kultimate/screens/addTask.py` & `kultimate-0.2.3/kultimate/screens/addTask.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from textual.app import ComposeResult
 from textual.containers import Grid
 from textual.screen import ModalScreen
 from textual.widgets import Input
 
 
-class AddTask(ModalScreen[bool]):
+class AddTask(ModalScreen[str]):
     """Screen with a dialog to return yes or not"""
 
     BINDINGS = [
         ("escape", "exit", ""),
     ]
 
     def compose(self) -> ComposeResult:
```

### Comparing `kultimate-0.2.2/kultimate/screens/deleteTask.py` & `kultimate-0.2.3/kultimate/screens/deleteTask.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.2/kultimate/screens/selectFile.py` & `kultimate-0.2.3/kultimate/screens/selectFile.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.2/kultimate/utils/app_config.py` & `kultimate-0.2.3/kultimate/utils/app_config.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.2/kultimate/utils/html_to_markdown.py` & `kultimate-0.2.3/kultimate/utils/html_to_markdown.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.2/kultimate/utils/parser_html.py` & `kultimate-0.2.3/kultimate/utils/parser_html.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.2/kultimate/utils/process_yaml.py` & `kultimate-0.2.3/kultimate/utils/process_yaml.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.2/kultimate/utils/prueba.py` & `kultimate-0.2.3/kultimate/utils/prueba.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.2/kultimate/widgets/directory.py` & `kultimate-0.2.3/kultimate/widgets/directory.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.2/pyproject.toml` & `kultimate-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kultimate"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Felipe <104157442+justafewwords4@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 textual = { extras = ["dev"], version = "^0.27.0" }
```

### Comparing `kultimate-0.2.2/PKG-INFO` & `kultimate-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kultimate
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Felipe
 Author-email: 104157442+justafewwords4@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -49,15 +49,16 @@
 | o                   | Agregar tarea al final de la columna actual   |
 | ctrl+l              | Mueve la tarea a la última columna            |
 | ctrl+d              | Borra la tarea seleccionada                   |
 | q                   | Salir de la aplicación                        |
 
 ## ToDo
 
-- FIXME: Al mover las tareas entre columnas visualmente se ve bien, pero al
+- TODO: Editar tareas
+- DONE: Al mover las tareas entre columnas visualmente se ve bien, pero al
   grabar a disco se queda en todas las columnas por donde pasa.
 - TODO: Reducir el tamaño de la caja para capturar las tareas.
 - TODO: Rehacer la configuración de la aplicación.
 - TODO: Hacer esqueleto para crear los nuevos archivos.
 - TODO: Crear nuevo archivo.
 - TODO: Si no existe directorio pedirlo.
 - TODO: Agregar columnas.
```

