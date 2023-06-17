# Comparing `tmp/progression_qc-0.4.3.tar.gz` & `tmp/progression_qc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progression_qc-0.4.3.tar", last modified: Tue Jun 13 07:19:24 2023, max compression
+gzip compressed data, was "progression_qc-0.5.0.tar", last modified: Sat Jun 17 03:02:39 2023, max compression
```

## Comparing `progression_qc-0.4.3.tar` & `progression_qc-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:19:24.035076 progression_qc-0.4.3/
--rw-rw-rw-   0 root         (0) root         (0)    35074 2023-06-13 06:37:01.000000 progression_qc-0.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      570 2023-06-13 07:19:24.031076 progression_qc-0.4.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:19:24.031076 progression_qc-0.4.3/progression_qc/
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-13 07:19:13.000000 progression_qc-0.4.3/progression_qc/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-06-13 07:19:13.000000 progression_qc-0.4.3/progression_qc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1146 2023-06-13 06:37:01.000000 progression_qc-0.4.3/progression_qc/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     7864 2023-06-13 06:37:01.000000 progression_qc-0.4.3/progression_qc/progression_qc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:19:24.031076 progression_qc-0.4.3/progression_qc/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 07:19:13.000000 progression_qc-0.4.3/progression_qc/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-06-13 06:37:01.000000 progression_qc-0.4.3/progression_qc/schemas/question_base.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-13 06:37:01.000000 progression_qc-0.4.3/progression_qc/schemas/question_bd.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-06-13 06:37:01.000000 progression_qc-0.4.3/progression_qc/schemas/question_prog.py
--rw-rw-rw-   0 root         (0) root         (0)     1647 2023-06-13 06:37:01.000000 progression_qc-0.4.3/progression_qc/schemas/question_sys.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-13 06:37:01.000000 progression_qc-0.4.3/progression_qc/schemas/question_vcs.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-13 06:37:01.000000 progression_qc-0.4.3/progression_qc/schemas/rétroactions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:19:24.031076 progression_qc-0.4.3/progression_qc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      570 2023-06-13 07:19:24.000000 progression_qc-0.4.3/progression_qc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      615 2023-06-13 07:19:24.000000 progression_qc-0.4.3/progression_qc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 07:19:24.000000 progression_qc-0.4.3/progression_qc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-13 07:19:24.000000 progression_qc-0.4.3/progression_qc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 07:19:24.000000 progression_qc-0.4.3/progression_qc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 07:19:24.035076 progression_qc-0.4.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-13 07:19:13.000000 progression_qc-0.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:19:24.031076 progression_qc-0.4.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     9214 2023-06-13 06:37:01.000000 progression_qc-0.4.3/tests/test_progression_qc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:02:39.189458 progression_qc-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35074 2023-06-13 05:16:01.000000 progression_qc-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      570 2023-06-17 03:02:39.189458 progression_qc-0.5.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:02:39.189458 progression_qc-0.5.0/progression_qc/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-17 02:56:34.000000 progression_qc-0.5.0/progression_qc/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-06-17 02:09:58.000000 progression_qc-0.5.0/progression_qc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2023-06-13 05:16:01.000000 progression_qc-0.5.0/progression_qc/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7946 2023-06-17 02:56:34.000000 progression_qc-0.5.0/progression_qc/progression_qc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:02:39.189458 progression_qc-0.5.0/progression_qc/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-17 03:02:29.000000 progression_qc-0.5.0/progression_qc/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-06-13 05:36:49.000000 progression_qc-0.5.0/progression_qc/schemas/question_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-06-17 02:56:34.000000 progression_qc-0.5.0/progression_qc/schemas/question_bd.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-17 02:56:34.000000 progression_qc-0.5.0/progression_qc/schemas/question_prog.py
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-06-17 02:56:34.000000 progression_qc-0.5.0/progression_qc/schemas/question_sys.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-06-17 02:56:34.000000 progression_qc-0.5.0/progression_qc/schemas/question_vcs.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-13 05:16:01.000000 progression_qc-0.5.0/progression_qc/schemas/rétroactions.py
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-06-17 02:56:34.000000 progression_qc-0.5.0/progression_qc/schemas/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-06-17 02:56:34.000000 progression_qc-0.5.0/progression_qc/schemas/test_prog.py
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-06-17 02:56:34.000000 progression_qc-0.5.0/progression_qc/schemas/test_sys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:02:39.189458 progression_qc-0.5.0/progression_qc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      570 2023-06-17 03:02:39.000000 progression_qc-0.5.0/progression_qc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      722 2023-06-17 03:02:39.000000 progression_qc-0.5.0/progression_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 03:02:39.000000 progression_qc-0.5.0/progression_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-17 03:02:39.000000 progression_qc-0.5.0/progression_qc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 03:02:39.000000 progression_qc-0.5.0/progression_qc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 03:02:39.189458 progression_qc-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-17 02:09:58.000000 progression_qc-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:02:39.189458 progression_qc-0.5.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     9214 2023-06-13 05:16:01.000000 progression_qc-0.5.0/tests/test_progression_qc.py
```

### Comparing `progression_qc-0.4.3/LICENSE` & `progression_qc-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `progression_qc-0.4.3/PKG-INFO` & `progression_qc-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progression_qc
-Version: 0.4.3
+Version: 0.5.0
 Summary: progression_qc est un compilateur/validateur pour la production de d'exercices pour Progression. progression_qc reçoit sur l'entrée standard ou en paramètre un fichier YAML contenant la description d'une question et reproduit sur la sortie standard le résultat traité et validé.
 Home-page: https://git.dti.crosemont.quebec/progression/validateur
 Author: Patrick Lafrance
 Author-email: plafrance@crosemont.qc.ca
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `progression_qc-0.4.3/progression_qc/__main__.py` & `progression_qc-0.5.0/progression_qc/__main__.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.4.3/progression_qc/progression_qc.py` & `progression_qc-0.5.0/progression_qc/progression_qc.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,37 +36,36 @@
 
 
 def valider_schema_yaml_infos_question(contenu_fichier):
     schema_registry.add(
         "rétroactions", eval(pkg_resources.read_text(schemas, "rétroactions.py"))
     )
     schema_registry.add(
+        "test_base", eval(pkg_resources.read_text(schemas, "test_base.py"))
+    )
+    schema_registry.add(
+        "test_prog", eval(pkg_resources.read_text(schemas, "test_prog.py"))
+    )
+    schema_registry.add(
+        "test_sys", eval(pkg_resources.read_text(schemas, "test_sys.py"))
+    )
+    schema_registry.add(
         "question_base", eval(pkg_resources.read_text(schemas, "question_base.py"))
     )
     schema_registry.add(
         "question_prog",
-        {
-            **schema_registry.get("question_base"),
-            **eval(pkg_resources.read_text(schemas, "question_prog.py")),
-        },
+        eval(pkg_resources.read_text(schemas, "question_prog.py")),
     )
     schema_registry.add(
         "question_sys",
-        {
-            **schema_registry.get("question_base"),
-            **eval(pkg_resources.read_text(schemas, "question_sys.py")),
-        },
+        eval(pkg_resources.read_text(schemas, "question_sys.py")),
     )
-
     schema_registry.add(
         "question_vcs",
-        {
-            **schema_registry.get("question_sys"),
-            **eval(pkg_resources.read_text(schemas, "question_vcs.py")),
-        },
+        eval(pkg_resources.read_text(schemas, "question_vcs.py")),
     )
 
     schema_registry.add(
         "question_bd",
         {
             **schema_registry.get("question_sys"),
             **eval(pkg_resources.read_text(schemas, "question_bd.py")),
```

### Comparing `progression_qc-0.4.3/progression_qc/schemas/question_base.py` & `progression_qc-0.5.0/progression_qc/schemas/question_base.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.4.3/progression_qc/schemas/question_sys.py` & `progression_qc-0.5.0/progression_qc/schemas/question_sys.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,24 @@
 {
+    **schema_registry.get("question_base"),
     "image": {
         "required": True,
         "type": "string",
         "empty": False,
         "nullable": True,
     },
     "tests": {
         "excludes": "réponse",
         "required": True,
         "type": "list",
         "empty": False,
         "schema": {
             "required": True,
             "type": "dict",
-            "schema": {
-                "nom": {"required": False, "type": "string"},
-                "validation": {
-                    "required": True,
-                    "type": "string",
-                    "empty": False,
-                    "nullable": False,
-                },
-                "sortie": {
-                    "required": True,
-                    "type": ["string", "integer"],
-                    "nullable": False,
-                },
-                "utilisateur": {
-                    "required": False,
-                    "type": "string",
-                    "regex": "^[a-z][-a-z0-9_]*$",
-                    "nullable": False,
-                },
-                "rétroactions": {
-                    "required": False,
-                    "type": "dict",
-                    "schema": "rétroactions",
-                },
-            },
+            "schema": "test_sys",
         },
     },
     "réponse": {
         "excludes": "tests",
         "required": True,
         "type": "string",
         "empty": False,
```

### Comparing `progression_qc-0.4.3/progression_qc.egg-info/PKG-INFO` & `progression_qc-0.5.0/progression_qc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progression-qc
-Version: 0.4.3
+Version: 0.5.0
 Summary: progression_qc est un compilateur/validateur pour la production de d'exercices pour Progression. progression_qc reçoit sur l'entrée standard ou en paramètre un fichier YAML contenant la description d'une question et reproduit sur la sortie standard le résultat traité et validé.
 Home-page: https://git.dti.crosemont.quebec/progression/validateur
 Author: Patrick Lafrance
 Author-email: plafrance@crosemont.qc.ca
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `progression_qc-0.4.3/progression_qc.egg-info/SOURCES.txt` & `progression_qc-0.5.0/progression_qc.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,8 +12,11 @@
 progression_qc/schemas/__init__.py
 progression_qc/schemas/question_base.py
 progression_qc/schemas/question_bd.py
 progression_qc/schemas/question_prog.py
 progression_qc/schemas/question_sys.py
 progression_qc/schemas/question_vcs.py
 progression_qc/schemas/rétroactions.py
+progression_qc/schemas/test_base.py
+progression_qc/schemas/test_prog.py
+progression_qc/schemas/test_sys.py
 tests/test_progression_qc.py
```

### Comparing `progression_qc-0.4.3/setup.py` & `progression_qc-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.4.3/tests/test_progression_qc.py` & `progression_qc-0.5.0/tests/test_progression_qc.py`

 * *Files identical despite different names*

