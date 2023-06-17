# Comparing `tmp/kultimate-0.2.6.tar.gz` & `tmp/kultimate-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kultimate-0.2.6.tar", max compression
+gzip compressed data, was "kultimate-0.2.7.tar", max compression
```

## Comparing `kultimate-0.2.6.tar` & `kultimate-0.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3579 2023-06-17 00:35:38.560480 kultimate-0.2.6/README.md
--rw-r--r--   0        0        0      211 2023-06-17 00:35:38.560480 kultimate-0.2.6/kultimate/__init__.py
--rw-r--r--   0        0        0     2191 2023-06-17 00:35:38.560480 kultimate-0.2.6/kultimate/app.css
--rw-r--r--   0        0        0    22214 2023-06-17 00:40:55.140487 kultimate-0.2.6/kultimate/app.py
--rw-r--r--   0        0        0      168 2023-06-17 00:35:38.560480 kultimate-0.2.6/kultimate/screens/__init__.py
--rw-r--r--   0        0        0      897 2023-06-16 20:11:44.883725 kultimate-0.2.6/kultimate/screens/addTask.py
--rw-r--r--   0        0        0     1630 2023-06-17 00:35:38.563814 kultimate-0.2.6/kultimate/screens/create_file.py
--rw-r--r--   0        0        0      992 2023-06-17 00:52:35.603836 kultimate-0.2.6/kultimate/screens/deleteTask.py
--rw-r--r--   0        0        0      986 2023-06-16 20:10:08.290390 kultimate-0.2.6/kultimate/screens/edit_task.py
--rw-r--r--   0        0        0      815 2023-06-15 16:47:43.396777 kultimate-0.2.6/kultimate/screens/selectFile.py
--rw-r--r--   0        0        0      175 2023-06-17 00:35:38.563814 kultimate-0.2.6/kultimate/utils/__init__.py
--rw-r--r--   0        0        0     2372 2023-06-17 00:35:38.563814 kultimate-0.2.6/kultimate/utils/app_config.py
--rw-r--r--   0        0        0     1784 2023-06-17 00:35:38.563814 kultimate-0.2.6/kultimate/utils/create_file.py
--rw-r--r--   0        0        0     2048 2023-06-15 16:30:13.640087 kultimate-0.2.6/kultimate/utils/html_to_markdown.py
--rw-r--r--   0        0        0     1885 2023-06-16 17:10:49.190158 kultimate-0.2.6/kultimate/utils/parser_html.py
--rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.2.6/kultimate/utils/process_yaml.py
--rw-r--r--   0        0        0      743 2023-06-16 16:51:32.056800 kultimate-0.2.6/kultimate/utils/prueba.py
--rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.2.6/kultimate/widgets/__init__.py
--rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.2.6/kultimate/widgets/directory.py
--rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.2.6/kultimate/widgets/stages.py
--rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.2.6/kultimate/widgets/stagesContainer.py
--rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.2.6/kultimate/widgets/task.py
--rw-r--r--   0        0        0      606 2023-06-17 00:52:01.800502 kultimate-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     4206 1970-01-01 00:00:00.000000 kultimate-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     3673 2023-06-17 01:35:44.660558 kultimate-0.2.7/README.md
+-rw-r--r--   0        0        0      211 2023-06-17 00:35:38.560480 kultimate-0.2.7/kultimate/__init__.py
+-rw-r--r--   0        0        0     2191 2023-06-17 00:35:38.560480 kultimate-0.2.7/kultimate/app.css
+-rw-r--r--   0        0        0    22125 2023-06-17 01:40:14.290564 kultimate-0.2.7/kultimate/app.py
+-rw-r--r--   0        0        0      168 2023-06-17 00:35:38.560480 kultimate-0.2.7/kultimate/screens/__init__.py
+-rw-r--r--   0        0        0      897 2023-06-16 20:11:44.883725 kultimate-0.2.7/kultimate/screens/addTask.py
+-rw-r--r--   0        0        0     1630 2023-06-17 00:35:38.563814 kultimate-0.2.7/kultimate/screens/create_file.py
+-rw-r--r--   0        0        0      992 2023-06-17 00:52:35.603836 kultimate-0.2.7/kultimate/screens/deleteTask.py
+-rw-r--r--   0        0        0      986 2023-06-16 20:10:08.290390 kultimate-0.2.7/kultimate/screens/edit_task.py
+-rw-r--r--   0        0        0      815 2023-06-15 16:47:43.396777 kultimate-0.2.7/kultimate/screens/selectFile.py
+-rw-r--r--   0        0        0      175 2023-06-17 00:35:38.563814 kultimate-0.2.7/kultimate/utils/__init__.py
+-rw-r--r--   0        0        0     2372 2023-06-17 00:35:38.563814 kultimate-0.2.7/kultimate/utils/app_config.py
+-rw-r--r--   0        0        0     1582 2023-06-17 01:40:35.177231 kultimate-0.2.7/kultimate/utils/create_file.py
+-rw-r--r--   0        0        0     2048 2023-06-15 16:30:13.640087 kultimate-0.2.7/kultimate/utils/html_to_markdown.py
+-rw-r--r--   0        0        0     1885 2023-06-16 17:10:49.190158 kultimate-0.2.7/kultimate/utils/parser_html.py
+-rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.2.7/kultimate/utils/process_yaml.py
+-rw-r--r--   0        0        0      743 2023-06-16 16:51:32.056800 kultimate-0.2.7/kultimate/utils/prueba.py
+-rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.2.7/kultimate/widgets/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.2.7/kultimate/widgets/directory.py
+-rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.2.7/kultimate/widgets/stages.py
+-rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.2.7/kultimate/widgets/stagesContainer.py
+-rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.2.7/kultimate/widgets/task.py
+-rw-r--r--   0        0        0      606 2023-06-17 01:41:03.647232 kultimate-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 kultimate-0.2.7/PKG-INFO
```

### Comparing `kultimate-0.2.6/README.md` & `kultimate-0.2.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # Kultimate
 
 ![kultimate](render1686782901985.gif)
 
 Aplicación CLI Python para manejar archivos markdown como tableros Kanban.
 Programado con [textual](https://textual.textualize.io/).
 
-# Instalación
+## Requerimientos
+
+`python = "^3.10"`
+
+Se ha probado en Linux, y tal vez funcione en MacOS.
+
+## Instalación
 
 ```sh
 pip install kultimate
 ```
 
 ## Configuración
 
@@ -31,15 +37,15 @@
 | o                   | Agregar tarea al final de la columna actual   |
 | ctrl+l              | Mueve la tarea a la última columna            |
 | ctrl+d              | Borra la tarea seleccionada                   |
 | q                   | Salir de la aplicación                        |
 
 ## ToDo
 
-- [ ] TODO: Crear nuevo archivo. Usar el esqueleto creado en el archivo de configuración
+- [x] DONE: Crear nuevo archivo. Usar el esqueleto creado en el archivo de configuración
 - [x] DONE: Rehacer la configuración de la aplicación.
 - [x] DONE: Hacer esqueleto para crear los nuevos archivos.
 - [x] DONE: Si no existe directorio crearlo.
 - [x] DONE: Reducir el tamaño de la caja para capturar las tareas.
 - [x] DONE: Editar tareas
 - [x] DONE: Al mover las tareas entre columnas visualmente se ve bien, pero al
       grabar a disco se queda en todas las columnas por donde pasa.
```

### Comparing `kultimate-0.2.6/kultimate/app.css` & `kultimate-0.2.7/kultimate/app.css`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.6/kultimate/app.py` & `kultimate-0.2.7/kultimate/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -600,16 +600,15 @@
             self.get_total_stages()
 
             self.__scroll_and_focus_stage()
             # self.current_task = self.total_tasks
             self.__focus_task()
 
         except IndexError:
-            with open("/home/felipe/Dropbox/kanban3/nel.txt", "w") as ff:
-                ff.write("nel")
+            pass
 
     # DONE: Seleccionar un archivo para mostrar.
     # File selected
     async def on_directory_tree_file_selected(
         self,
         event: Directory.FileSelected,
     ) -> None:
```

### Comparing `kultimate-0.2.6/kultimate/screens/addTask.py` & `kultimate-0.2.7/kultimate/screens/addTask.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.6/kultimate/screens/create_file.py` & `kultimate-0.2.7/kultimate/screens/create_file.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.6/kultimate/screens/deleteTask.py` & `kultimate-0.2.7/kultimate/screens/deleteTask.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.6/kultimate/screens/edit_task.py` & `kultimate-0.2.7/kultimate/screens/edit_task.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.6/kultimate/screens/selectFile.py` & `kultimate-0.2.7/kultimate/screens/selectFile.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.6/kultimate/utils/app_config.py` & `kultimate-0.2.7/kultimate/utils/app_config.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.6/kultimate/utils/create_file.py` & `kultimate-0.2.7/kultimate/utils/create_file.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,21 +8,16 @@
 config_object = ConfigParser()
 
 
 def create_new_markdown_file(directory: str, dictio: dict) -> bool:
     """Create a new markdown directory on directory"""
 
     if not dictio["name_file"]:
-        with open("/home/felipe/no_file.txt", "w") as ff:
-            ff.write("no file")
         return False
 
-    with open("/home/felipe/no_file.txt", "w") as ff:
-        ff.write(f"{directory}/{dictio['name_file']}\n")
-
     file_config_exists = exists(path_file_config)
 
     stages_three = ["ToDo", "Doing", "Done"]
     stages_five = ["BackLog", "ToDo", "Doing", "Waiting", "Done"]
 
     if file_config_exists:
         config_object.read(path_file_config)
```

### Comparing `kultimate-0.2.6/kultimate/utils/html_to_markdown.py` & `kultimate-0.2.7/kultimate/utils/html_to_markdown.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.6/kultimate/utils/parser_html.py` & `kultimate-0.2.7/kultimate/utils/parser_html.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.6/kultimate/utils/process_yaml.py` & `kultimate-0.2.7/kultimate/utils/process_yaml.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.6/kultimate/utils/prueba.py` & `kultimate-0.2.7/kultimate/utils/prueba.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.6/kultimate/widgets/directory.py` & `kultimate-0.2.7/kultimate/widgets/directory.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.6/pyproject.toml` & `kultimate-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kultimate"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["Felipe <104157442+justafewwords4@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 textual = { extras = ["dev"], version = "^0.27.0" }
```

### Comparing `kultimate-0.2.6/PKG-INFO` & `kultimate-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kultimate
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Author: Felipe
 Author-email: 104157442+justafewwords4@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,15 +19,21 @@
 # Kultimate
 
 ![kultimate](render1686782901985.gif)
 
 Aplicación CLI Python para manejar archivos markdown como tableros Kanban.
 Programado con [textual](https://textual.textualize.io/).
 
-# Instalación
+## Requerimientos
+
+`python = "^3.10"`
+
+Se ha probado en Linux, y tal vez funcione en MacOS.
+
+## Instalación
 
 ```sh
 pip install kultimate
 ```
 
 ## Configuración
 
@@ -49,15 +55,15 @@
 | o                   | Agregar tarea al final de la columna actual   |
 | ctrl+l              | Mueve la tarea a la última columna            |
 | ctrl+d              | Borra la tarea seleccionada                   |
 | q                   | Salir de la aplicación                        |
 
 ## ToDo
 
-- [ ] TODO: Crear nuevo archivo. Usar el esqueleto creado en el archivo de configuración
+- [x] DONE: Crear nuevo archivo. Usar el esqueleto creado en el archivo de configuración
 - [x] DONE: Rehacer la configuración de la aplicación.
 - [x] DONE: Hacer esqueleto para crear los nuevos archivos.
 - [x] DONE: Si no existe directorio crearlo.
 - [x] DONE: Reducir el tamaño de la caja para capturar las tareas.
 - [x] DONE: Editar tareas
 - [x] DONE: Al mover las tareas entre columnas visualmente se ve bien, pero al
       grabar a disco se queda en todas las columnas por donde pasa.
```

