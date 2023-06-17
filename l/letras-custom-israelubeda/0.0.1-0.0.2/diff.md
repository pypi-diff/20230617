# Comparing `tmp/letras_custom_israelubeda-0.0.1.tar.gz` & `tmp/letras_custom_israelubeda-0.0.2.tar.gz`

## Comparing `letras_custom_israelubeda-0.0.1.tar` & `letras_custom_israelubeda-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 letras_custom_israelubeda-0.0.1/src/letras_custom_israelubeda/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 letras_custom_israelubeda-0.0.1/src/letras_custom_israelubeda/my_libreria.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 letras_custom_israelubeda-0.0.1/LICENSE
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 letras_custom_israelubeda-0.0.1/README.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 letras_custom_israelubeda-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 letras_custom_israelubeda-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 letras_custom_israelubeda-0.0.2/src/letras_custom_israelubeda/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 letras_custom_israelubeda-0.0.2/src/letras_custom_israelubeda/my_libreria.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 letras_custom_israelubeda-0.0.2/LICENSE
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 letras_custom_israelubeda-0.0.2/README.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 letras_custom_israelubeda-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 letras_custom_israelubeda-0.0.2/PKG-INFO
```

### Comparing `letras_custom_israelubeda-0.0.1/src/letras_custom_israelubeda/my_libreria.py` & `letras_custom_israelubeda-0.0.2/src/letras_custom_israelubeda/my_libreria.py`

 * *Files identical despite different names*

### Comparing `letras_custom_israelubeda-0.0.1/LICENSE` & `letras_custom_israelubeda-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `letras_custom_israelubeda-0.0.1/pyproject.toml` & `letras_custom_israelubeda-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "letras_custom_israelubeda"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Israel Ubeda", email="israel.ubedabravo@gmail.com" },
 ]
 description = "Una libreria que transforma una letra por otra , ejemplo la letra A ,se transforma en letra Z"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `letras_custom_israelubeda-0.0.1/PKG-INFO` & `letras_custom_israelubeda-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letras_custom_israelubeda
-Version: 0.0.1
+Version: 0.0.2
 Summary: Una libreria que transforma una letra por otra , ejemplo la letra A ,se transforma en letra Z
 Project-URL: Homepage, https://github.com/israelubeda
 Project-URL: Bug Tracker, https://github.com/israelubeda
 Author-email: Israel Ubeda <israel.ubedabravo@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,7 +14,31 @@
 
 # Libreria transformadora de texto
 
 _Una libreria que transforma una letra por otra , ejemplo la letra A ,se transforma en letra Z_
 
 
 ## Comenzando 🚀
+
+_instalar la libreria_
+
+~~~
+pip install letras-custom-israelubeda
+~~~
+
+*Modo de uso
+
+Ejemplo:
+
+example.py
+~~~
+from letras_custom_israelubeda import sustituir_letras
+
+palabra = sustituir_letras("hola mundo")
+print(palabra)
+
+~~~
+
+output: sooz nunwo
+
+
+
```

