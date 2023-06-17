# Comparing `tmp/object-settings-4.1.tar.gz` & `tmp/object-settings-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "object-settings-4.1.tar", last modified: Mon Jun  5 18:27:46 2023, max compression
+gzip compressed data, was "object-settings-4.2.tar", last modified: Sat Jun 17 20:31:41 2023, max compression
```

## Comparing `object-settings-4.1.tar` & `object-settings-4.2.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.295534 object-settings-4.1/
--rw-r--r--   0 samu      (1000) samu      (1000)     5600 2023-06-05 18:27:46.295534 object-settings-4.1/PKG-INFO
--rw-r--r--   0 samu      (1000) samu      (1000)     4755 2023-03-09 17:49:33.000000 object-settings-4.1/README.md
--rw-r--r--   0 samu      (1000) samu      (1000)      969 2023-06-05 18:27:20.000000 object-settings-4.1/pyproject.toml
--rw-r--r--   0 samu      (1000) samu      (1000)       38 2023-06-05 18:27:46.296534 object-settings-4.1/setup.cfg
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.284535 object-settings-4.1/src/
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.286535 object-settings-4.1/src/object_settings.egg-info/
--rw-r--r--   0 samu      (1000) samu      (1000)     5600 2023-06-05 18:27:46.000000 object-settings-4.1/src/object_settings.egg-info/PKG-INFO
--rw-r--r--   0 samu      (1000) samu      (1000)     1343 2023-06-05 18:27:46.000000 object-settings-4.1/src/object_settings.egg-info/SOURCES.txt
--rw-r--r--   0 samu      (1000) samu      (1000)        1 2023-06-05 18:27:46.000000 object-settings-4.1/src/object_settings.egg-info/dependency_links.txt
--rw-r--r--   0 samu      (1000) samu      (1000)       22 2023-06-05 18:27:46.000000 object-settings-4.1/src/object_settings.egg-info/requires.txt
--rw-r--r--   0 samu      (1000) samu      (1000)       22 2023-06-05 18:27:46.000000 object-settings-4.1/src/object_settings.egg-info/top_level.txt
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.288534 object-settings-4.1/src/settings/
--rw-r--r--   0 samu      (1000) samu      (1000)      427 2023-06-05 16:38:50.000000 object-settings-4.1/src/settings/__init__.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.289535 object-settings-4.1/src/settings/backend/
--rw-r--r--   0 samu      (1000) samu      (1000)      114 2023-03-09 16:08:28.000000 object-settings-4.1/src/settings/backend/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)     3004 2023-06-05 17:19:56.000000 object-settings-4.1/src/settings/backend/config.py
--rw-r--r--   0 samu      (1000) samu      (1000)      855 2023-06-05 14:08:02.000000 object-settings-4.1/src/settings/backend/datatype_loader.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1494 2023-06-05 17:28:50.000000 object-settings-4.1/src/settings/backend/main.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.290535 object-settings-4.1/src/settings/backend/parsers/
--rw-r--r--   0 samu      (1000) samu      (1000)      263 2023-06-05 14:30:05.000000 object-settings-4.1/src/settings/backend/parsers/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)      935 2023-06-05 14:50:54.000000 object-settings-4.1/src/settings/backend/parsers/_template.py
--rw-r--r--   0 samu      (1000) samu      (1000)      853 2023-06-05 14:30:30.000000 object-settings-4.1/src/settings/backend/parsers/cli.py
--rw-r--r--   0 samu      (1000) samu      (1000)      826 2023-06-05 14:30:55.000000 object-settings-4.1/src/settings/backend/parsers/env.py
--rw-r--r--   0 samu      (1000) samu      (1000)     2214 2023-06-05 17:16:10.000000 object-settings-4.1/src/settings/backend/parsers/files.py
--rw-r--r--   0 samu      (1000) samu      (1000)     3620 2023-06-05 17:31:48.000000 object-settings-4.1/src/settings/base.py
--rw-r--r--   0 samu      (1000) samu      (1000)     4472 2023-06-05 16:26:58.000000 object-settings-4.1/src/settings/types.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.290535 object-settings-4.1/src/settings_gui/
--rw-r--r--   0 samu      (1000) samu      (1000)      231 2023-03-04 11:44:09.000000 object-settings-4.1/src/settings_gui/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)      338 2023-06-05 15:03:20.000000 object-settings-4.1/src/settings_gui/_tk_abstractor.py
--rw-r--r--   0 samu      (1000) samu      (1000)      279 2023-03-04 22:40:29.000000 object-settings-4.1/src/settings_gui/config.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.292534 object-settings-4.1/src/settings_gui/tkinter/
--rw-r--r--   0 samu      (1000) samu      (1000)      343 2023-03-04 11:44:09.000000 object-settings-4.1/src/settings_gui/tkinter/__init__.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.293535 object-settings-4.1/src/settings_gui/tkinter/icons/
--rw-r--r--   0 samu      (1000) samu      (1000)      206 2015-11-19 10:52:05.000000 object-settings-4.1/src/settings_gui/tkinter/icons/checkmark-black.png
--rw-r--r--   0 samu      (1000) samu      (1000)     4826 2022-10-23 18:33:29.000000 object-settings-4.1/src/settings_gui/tkinter/icons/checkmark-white.png
--rw-r--r--   0 samu      (1000) samu      (1000)      333 2015-11-19 10:51:50.000000 object-settings-4.1/src/settings_gui/tkinter/icons/error.png
--rw-r--r--   0 samu      (1000) samu      (1000)      301 2015-11-21 05:08:04.000000 object-settings-4.1/src/settings_gui/tkinter/icons/folder-black.png
--rw-r--r--   0 samu      (1000) samu      (1000)     5036 2022-10-23 16:12:53.000000 object-settings-4.1/src/settings_gui/tkinter/icons/folder-white.png
--rw-r--r--   0 samu      (1000) samu      (1000)     1505 2023-06-05 17:48:09.000000 object-settings-4.1/src/settings_gui/tkinter/main.py
--rw-r--r--   0 samu      (1000) samu      (1000)      723 2023-06-05 16:49:45.000000 object-settings-4.1/src/settings_gui/tkinter/section_frames.py
--rw-r--r--   0 samu      (1000) samu      (1000)     7620 2023-06-05 16:49:23.000000 object-settings-4.1/src/settings_gui/tkinter/type_frames.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.293535 object-settings-4.1/src/settings_gui/ttk/
--rw-r--r--   0 samu      (1000) samu      (1000)      719 2022-12-16 20:12:38.000000 object-settings-4.1/src/settings_gui/ttk/__init__.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2023-06-05 18:27:46.295534 object-settings-4.1/tests/
--rw-r--r--   0 samu      (1000) samu      (1000)      923 2023-03-09 16:25:34.000000 object-settings-4.1/tests/test_cli.py
--rw-r--r--   0 samu      (1000) samu      (1000)      797 2023-03-09 15:35:21.000000 object-settings-4.1/tests/test_datafiles.py
--rw-r--r--   0 samu      (1000) samu      (1000)      791 2023-04-10 16:31:09.000000 object-settings-4.1/tests/test_datatype_loader.py
--rw-r--r--   0 samu      (1000) samu      (1000)      821 2023-03-09 16:25:34.000000 object-settings-4.1/tests/test_endurance.py
--rw-r--r--   0 samu      (1000) samu      (1000)      830 2023-03-09 14:52:24.000000 object-settings-4.1/tests/test_env.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1811 2023-06-05 17:47:04.000000 object-settings-4.1/tests/test_gui_(manual).py
--rw-r--r--   0 samu      (1000) samu      (1000)     1108 2022-10-27 17:39:38.000000 object-settings-4.1/tests/test_v1_definitions.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1466 2022-11-03 11:24:05.000000 object-settings-4.1/tests/test_validation.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-17 20:31:41.216799 object-settings-4.2/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6151 2023-06-17 20:31:41.215799 object-settings-4.2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5306 2023-06-16 16:44:59.000000 object-settings-4.2/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      999 2023-06-16 16:50:26.000000 object-settings-4.2/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       21 2023-06-14 18:02:05.000000 object-settings-4.2/requirements.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-17 20:31:41.216799 object-settings-4.2/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-17 20:31:41.211799 object-settings-4.2/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-17 20:31:41.212799 object-settings-4.2/src/object_settings.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6151 2023-06-17 20:31:41.000000 object-settings-4.2/src/object_settings.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1415 2023-06-17 20:31:41.000000 object-settings-4.2/src/object_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-17 20:31:41.000000 object-settings-4.2/src/object_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       22 2023-06-17 20:31:41.000000 object-settings-4.2/src/object_settings.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       22 2023-06-17 20:31:41.000000 object-settings-4.2/src/object_settings.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-17 20:31:41.212799 object-settings-4.2/src/settings/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      427 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-17 20:31:41.212799 object-settings-4.2/src/settings/backend/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      114 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings/backend/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3004 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings/backend/config.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      855 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings/backend/datatype_loader.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1494 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings/backend/main.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-17 20:31:41.213799 object-settings-4.2/src/settings/backend/parsers/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      263 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings/backend/parsers/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      935 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings/backend/parsers/_template.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      853 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings/backend/parsers/cli.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      826 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings/backend/parsers/env.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2214 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings/backend/parsers/files.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3621 2023-06-16 13:05:58.000000 object-settings-4.2/src/settings/base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7447 2023-06-16 15:45:18.000000 object-settings-4.2/src/settings/types.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-17 20:31:41.213799 object-settings-4.2/src/settings_gui/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      231 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings_gui/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      338 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings_gui/_tk_abstractor.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      299 2023-06-16 15:03:32.000000 object-settings-4.2/src/settings_gui/config.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-17 20:31:41.213799 object-settings-4.2/src/settings_gui/tkinter/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      354 2023-06-16 14:03:45.000000 object-settings-4.2/src/settings_gui/tkinter/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-17 20:31:41.214799 object-settings-4.2/src/settings_gui/tkinter/icons/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      206 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings_gui/tkinter/icons/checkmark-black.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4826 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings_gui/tkinter/icons/checkmark-white.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      333 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings_gui/tkinter/icons/error.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      301 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings_gui/tkinter/icons/folder-black.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5036 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings_gui/tkinter/icons/folder-white.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1851 2023-06-16 14:56:46.000000 object-settings-4.2/src/settings_gui/tkinter/lib.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-06-16 15:17:44.000000 object-settings-4.2/src/settings_gui/tkinter/main.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      723 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings_gui/tkinter/section_frames.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6523 2023-06-16 14:51:14.000000 object-settings-4.2/src/settings_gui/tkinter/type_frames.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-17 20:31:41.215799 object-settings-4.2/src/settings_gui/ttk/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      719 2023-06-14 17:22:51.000000 object-settings-4.2/src/settings_gui/ttk/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-17 20:31:41.215799 object-settings-4.2/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      923 2023-06-14 17:22:51.000000 object-settings-4.2/tests/test_cli.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      797 2023-06-14 17:22:51.000000 object-settings-4.2/tests/test_datafiles.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      791 2023-06-14 17:22:51.000000 object-settings-4.2/tests/test_datatype_loader.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      821 2023-06-14 17:22:51.000000 object-settings-4.2/tests/test_endurance.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      830 2023-06-14 17:22:51.000000 object-settings-4.2/tests/test_env.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1811 2023-06-15 13:14:31.000000 object-settings-4.2/tests/test_gui_(manual).py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      939 2023-06-15 13:37:50.000000 object-settings-4.2/tests/test_mappings.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1108 2023-06-14 17:22:51.000000 object-settings-4.2/tests/test_v1_definitions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1466 2023-06-14 17:22:51.000000 object-settings-4.2/tests/test_validation.py
```

### Comparing `object-settings-4.1/PKG-INFO` & `object-settings-4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: object-settings
-Version: 4.1
+Version: 4.2
 Summary: Simple object-oriented config library, where your settings are objects
 License: MIT License
 Project-URL: Homepage, https://github.com/SamuLumio/object-settings
 Keywords: settings,setting,config,OOP,GUI
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,168 +15,179 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Description-Content-Type: text/markdown
 
 
-# object-settings
+object-settings
+===============
 
 Simple-to-use object-oriented Python config library, where your settings are objects.
 
-Their values have automatic validation and get saved to a file that's seamlessly
-written and read in the background, so you don't have to worry about any of it. 
-This makes it quick to define and use settings (see examples below).
+Their values have automatic validation and get saved to a file that's seamlessly written and read in the background, so you don't have to worry about any of it. This makes it quick to define and use settings (see examples below).
 
 
 
-Installation & usage
-====================
+## Installation & usage
 
 This package is on PyPi, so you can just do `pip install object-settings`
 
 After which it will be available with just the module name `settings`
 
-    import settings
-    settings.setup("Your app name")
+```python
+import settings
+settings.setup("Your app name")
     
-    your_option1 = settings.Toggle("Your first option label")
-    your_option2 = settings.Number("Your second option label")
+your_option1 = settings.Toggle("Your first option label")
+your_option2 = settings.Number("Your second option label")
+```
 
 
 
-Simple objects
-==============
+## Just simple objects
 
 For example, you can set a font size at the top of your ui file:
 
-    font = settings.Number(default=14)
+```python
+font = settings.Number(default=14)
 
-    ...
-    someuilib.Label("Bababooey", size=font.value)
-    ...
-    someuilib.Textbox("Lorem ipsum dolor...", font_size=font.value)
-    ...
+...
+someuilib.Label("Bababooey", size=font.value)
+...
+someuilib.Textbox("Lorem ipsum dolor...", font_size=font.value)
+...
+```
 
 Or if a setting is only checked in one place, it can be used without defining a variable:
 
-    if settings.Toggle("Update app automatically", default=True):
-        # do update
+```python
+if settings.Toggle("Update app automatically", default=True):
+    # do update
+```
 
 (it doesn't matter if the same setting is initialized multiple times)
 
 
 
-Integration
-===========
+## Integration
 
 The setting objects support "equals"-checking with actual values:
 
-    speed = settings.Number("Speed limit", 5)
-    
-    print(speed == 5)
-    >> True
-    print(speed == 3)
-    >> False
+```python
+speed = settings.Number("Speed limit", 5)
+
+print(speed == 5)
+>> True
+print(speed == 3)
+>> False
+```
 
 In addition, they work with many type-specific operations:
 
-    for selection in settings.Multichoice():
-        ...
+```python
+for selection in settings.Multichoice():
+    ...
+
+if settings.Toggle():
+    ...
+```
+
 
-    if settings.Toggle():
-        ...
 
+## Automatic storing
 
+When a setting's value is read/set, object-settings automatically creates and updates a config file on the disk in the background. It can read many file types, like `.cfg`, `.json` and `.yaml`. Any file deletions or unparsable external modifications are also handled.
 
-Automatic storing
-=================
+By default, the files are saved to a standard config location, depending on the platform (uses [appdirs](https://github.com/ActiveState/appdirs) package for paths). You can also set a custom directory for e.g. running in a Docker container.
 
-When a setting's value is read/set, object-settings automatically creates and updates 
-a config file on the disk in the background. 
-It can read many file types, like `.cfg`, `.json` and `.yaml`.
-Any file deletions or unparsable external modifications are also handled.
+Setting values are also automatically read from the environment, like from env vars or command line options. The under-the-hood parser system is also very extensible, so you can create and add custom ones for e.g. a custom database.
 
-By default, the files are saved to a standard config location, depending on the platform 
-(uses [appdirs](https://github.com/ActiveState/appdirs) package for paths). 
-You can also set a custom directory for e.g. running in a Docker container.
 
-Setting values are also automatically read from the environment, like from env vars or command line options.
-The under-the-hood parser system is also very extensible, so you can create and add custom ones for e.g. a custom database.
 
+## Value validation
 
+When a new value is set, it automatically gets validated and raises a `ValueError` if it doesn't pass:
 
-Value validation
-================
+```python
+update_interval = settings.Number("Update interval", default=5)
+update_interval.set("Daily")
+>> ValueError
+```
 
-When a new value is set, it automatically gets validated and raises a `ValueError` if it doesn't pass.
-This validation includes more than just datatypes, for example numbers can have min/max limits, 
-or a path setting can be set to require an existing path.
+This validation includes more than just datatypes, for example numbers can have min/max limits, or a path setting can be set to require an existing path:
 
+```python
+path = settings.Path("Download path", has_to_exist=True)
+path.set("/nonexistent/directory")
+>> ValueError
+```
 
 
-Listen for changes
-==================
 
-If you have some update function that you want to be called when a setting is changed, 
-you can add that function as a listener:
+## Listen for changes
 
-    some_setting.add_listener(your_function)
+If you have some update function that you want to be called when a setting is changed, you can add that function as a listener:
+
+```python
+some_setting.add_listener(your_function)
+```
 
 Now the function will be called every time when a new value is set.
 
 
 
-Sections
-========
+## Sections
 
-Optionally, if you have a lot of settings, you can organize them into sections 
-(which also works well with UIs)
+Optionally, if you have a lot of settings, you can organize them into sections (which also works well with UIs):
 
-    download_options = settings.Section("Downloader settings")
-    speed = settings.Number("Speed limit", 5, section=download_options)
-    dir = settings.Path("Target directory", '/home/yomama/Downloads', section=download_options)
-    server = settings.Choice("Mirror", ["Europe", "Asia", "America", "Africa"], "Asia", section=download_options)
+```python
+download_options = settings.Section("Downloader settings")
+speed = settings.Number("Speed limit", 5, section=download_options)
+dir = settings.Path("Target directory", '/home/yomama/Downloads', section=download_options)
+server = settings.Choice("Mirror", ["Europe", "Asia", "America", "Africa"], "Asia", section=download_options)
+```
 
 
 
-Did I mention free GUIs?
-========================
+## Did I mention free GUIs?
 
-That's right, this library also includes a separate `settings_gui` package that has 
-pre-made settings menus for both tkinter and ttk, with GTK and others to come.
-They have full integration with the aforementioned systems, like validation and sections.
+That's right, this library also includes a separate `settings_gui` package that has pre-made settings menus for both tkinter and ttk, with GTK and others to come. They have full integration with the aforementioned systems, like validation and sections.
 
 Here's an example of some dummy settings with both libraries: 
-(notice the warning for the misspelt download path)
 
-<figure>
-  <img src="readme-images/ttk.png">
-  <figcaption>Nice-looking ttk (theme: Sun Valley dark)</figcaption>
-</figure>
+*(notice the warning for the misspelt download path)*
+
+![Ttk](https://github.com/SamuLumio/object-settings/blob/master/readme-images/ttk.png?raw=true)
+*Nice-looking ttk (theme: Sun Valley dark)*
 
-<figure>
-  <img src="readme-images/tkinter.png">
-  <figcaption>Bare tkinter works too</figcaption>
-</figure>
+![Tkinter](https://github.com/SamuLumio/object-settings/blob/master/readme-images/tkinter.png?raw=true)
+*Bare tkinter works too*
 
-And you can get this automatically for all your defined settings by just calling one function! 
-(`SettingsFrame` or `SettingsWindow`, depending on preference)
+And you can get this automatically for all your defined settings by just calling one function (`SettingsFrame` or `SettingsWindow`, depending on preference)
 
-Or, if you want to get more custom/contextual, you can also use the individual 
-setting widgets and place them around your app (submodule `type_frames`).
+Or, if you want to get more custom/contextual, you can also use the individual setting widgets and place them around your app (submodule `type_frames`).
 
 
 
-Setting types
-=============
+## Setting types
 
 List of currently available setting types:
 
-- Toggle (bool)
-- Choice (str)  [from a list of options]
-- Multichoice (list)  [of things from a list of options]
-- Text (str)
-- Path (str)
-- Number (int)
+- `Toggle`:
+    A boolean True/False
+- `Choice`:
+    Choose an option (str) from a list
+- `MappedChoice`:
+    Choose an option (str) from a list, but have a different internal value mapped to it
+- `Multichoice`:
+    Choose multiple options (str) from a list
+- `MappedMultichoice`:
+    Choose multiple options (str) from a list, but have different internal values mapped to them
+- `Text`:
+    Just a basic text value
+- `Path`:
+    A file path whose existence can be checked
+- `Number`:
+    An integer that can be set or incremented and decremented
 
-You can also inherit from the base Setting class to easily create custom ones.
+You can also inherit from the `BaseSetting` class to easily create custom ones.
```

### Comparing `object-settings-4.1/README.md` & `object-settings-4.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,162 +1,173 @@
 
-# object-settings
+object-settings
+===============
 
 Simple-to-use object-oriented Python config library, where your settings are objects.
 
-Their values have automatic validation and get saved to a file that's seamlessly
-written and read in the background, so you don't have to worry about any of it. 
-This makes it quick to define and use settings (see examples below).
+Their values have automatic validation and get saved to a file that's seamlessly written and read in the background, so you don't have to worry about any of it. This makes it quick to define and use settings (see examples below).
 
 
 
-Installation & usage
-====================
+## Installation & usage
 
 This package is on PyPi, so you can just do `pip install object-settings`
 
 After which it will be available with just the module name `settings`
 
-    import settings
-    settings.setup("Your app name")
+```python
+import settings
+settings.setup("Your app name")
     
-    your_option1 = settings.Toggle("Your first option label")
-    your_option2 = settings.Number("Your second option label")
+your_option1 = settings.Toggle("Your first option label")
+your_option2 = settings.Number("Your second option label")
+```
 
 
 
-Simple objects
-==============
+## Just simple objects
 
 For example, you can set a font size at the top of your ui file:
 
-    font = settings.Number(default=14)
+```python
+font = settings.Number(default=14)
 
-    ...
-    someuilib.Label("Bababooey", size=font.value)
-    ...
-    someuilib.Textbox("Lorem ipsum dolor...", font_size=font.value)
-    ...
+...
+someuilib.Label("Bababooey", size=font.value)
+...
+someuilib.Textbox("Lorem ipsum dolor...", font_size=font.value)
+...
+```
 
 Or if a setting is only checked in one place, it can be used without defining a variable:
 
-    if settings.Toggle("Update app automatically", default=True):
-        # do update
+```python
+if settings.Toggle("Update app automatically", default=True):
+    # do update
+```
 
 (it doesn't matter if the same setting is initialized multiple times)
 
 
 
-Integration
-===========
+## Integration
 
 The setting objects support "equals"-checking with actual values:
 
-    speed = settings.Number("Speed limit", 5)
-    
-    print(speed == 5)
-    >> True
-    print(speed == 3)
-    >> False
+```python
+speed = settings.Number("Speed limit", 5)
+
+print(speed == 5)
+>> True
+print(speed == 3)
+>> False
+```
 
 In addition, they work with many type-specific operations:
 
-    for selection in settings.Multichoice():
-        ...
+```python
+for selection in settings.Multichoice():
+    ...
+
+if settings.Toggle():
+    ...
+```
+
 
-    if settings.Toggle():
-        ...
 
+## Automatic storing
 
+When a setting's value is read/set, object-settings automatically creates and updates a config file on the disk in the background. It can read many file types, like `.cfg`, `.json` and `.yaml`. Any file deletions or unparsable external modifications are also handled.
 
-Automatic storing
-=================
+By default, the files are saved to a standard config location, depending on the platform (uses [appdirs](https://github.com/ActiveState/appdirs) package for paths). You can also set a custom directory for e.g. running in a Docker container.
 
-When a setting's value is read/set, object-settings automatically creates and updates 
-a config file on the disk in the background. 
-It can read many file types, like `.cfg`, `.json` and `.yaml`.
-Any file deletions or unparsable external modifications are also handled.
+Setting values are also automatically read from the environment, like from env vars or command line options. The under-the-hood parser system is also very extensible, so you can create and add custom ones for e.g. a custom database.
 
-By default, the files are saved to a standard config location, depending on the platform 
-(uses [appdirs](https://github.com/ActiveState/appdirs) package for paths). 
-You can also set a custom directory for e.g. running in a Docker container.
 
-Setting values are also automatically read from the environment, like from env vars or command line options.
-The under-the-hood parser system is also very extensible, so you can create and add custom ones for e.g. a custom database.
 
+## Value validation
 
+When a new value is set, it automatically gets validated and raises a `ValueError` if it doesn't pass:
 
-Value validation
-================
+```python
+update_interval = settings.Number("Update interval", default=5)
+update_interval.set("Daily")
+>> ValueError
+```
 
-When a new value is set, it automatically gets validated and raises a `ValueError` if it doesn't pass.
-This validation includes more than just datatypes, for example numbers can have min/max limits, 
-or a path setting can be set to require an existing path.
+This validation includes more than just datatypes, for example numbers can have min/max limits, or a path setting can be set to require an existing path:
 
+```python
+path = settings.Path("Download path", has_to_exist=True)
+path.set("/nonexistent/directory")
+>> ValueError
+```
 
 
-Listen for changes
-==================
 
-If you have some update function that you want to be called when a setting is changed, 
-you can add that function as a listener:
+## Listen for changes
 
-    some_setting.add_listener(your_function)
+If you have some update function that you want to be called when a setting is changed, you can add that function as a listener:
+
+```python
+some_setting.add_listener(your_function)
+```
 
 Now the function will be called every time when a new value is set.
 
 
 
-Sections
-========
+## Sections
 
-Optionally, if you have a lot of settings, you can organize them into sections 
-(which also works well with UIs)
+Optionally, if you have a lot of settings, you can organize them into sections (which also works well with UIs):
 
-    download_options = settings.Section("Downloader settings")
-    speed = settings.Number("Speed limit", 5, section=download_options)
-    dir = settings.Path("Target directory", '/home/yomama/Downloads', section=download_options)
-    server = settings.Choice("Mirror", ["Europe", "Asia", "America", "Africa"], "Asia", section=download_options)
+```python
+download_options = settings.Section("Downloader settings")
+speed = settings.Number("Speed limit", 5, section=download_options)
+dir = settings.Path("Target directory", '/home/yomama/Downloads', section=download_options)
+server = settings.Choice("Mirror", ["Europe", "Asia", "America", "Africa"], "Asia", section=download_options)
+```
 
 
 
-Did I mention free GUIs?
-========================
+## Did I mention free GUIs?
 
-That's right, this library also includes a separate `settings_gui` package that has 
-pre-made settings menus for both tkinter and ttk, with GTK and others to come.
-They have full integration with the aforementioned systems, like validation and sections.
+That's right, this library also includes a separate `settings_gui` package that has pre-made settings menus for both tkinter and ttk, with GTK and others to come. They have full integration with the aforementioned systems, like validation and sections.
 
 Here's an example of some dummy settings with both libraries: 
-(notice the warning for the misspelt download path)
 
-<figure>
-  <img src="readme-images/ttk.png">
-  <figcaption>Nice-looking ttk (theme: Sun Valley dark)</figcaption>
-</figure>
+*(notice the warning for the misspelt download path)*
+
+![Ttk](https://github.com/SamuLumio/object-settings/blob/master/readme-images/ttk.png?raw=true)
+*Nice-looking ttk (theme: Sun Valley dark)*
 
-<figure>
-  <img src="readme-images/tkinter.png">
-  <figcaption>Bare tkinter works too</figcaption>
-</figure>
+![Tkinter](https://github.com/SamuLumio/object-settings/blob/master/readme-images/tkinter.png?raw=true)
+*Bare tkinter works too*
 
-And you can get this automatically for all your defined settings by just calling one function! 
-(`SettingsFrame` or `SettingsWindow`, depending on preference)
+And you can get this automatically for all your defined settings by just calling one function (`SettingsFrame` or `SettingsWindow`, depending on preference)
 
-Or, if you want to get more custom/contextual, you can also use the individual 
-setting widgets and place them around your app (submodule `type_frames`).
+Or, if you want to get more custom/contextual, you can also use the individual setting widgets and place them around your app (submodule `type_frames`).
 
 
 
-Setting types
-=============
+## Setting types
 
 List of currently available setting types:
 
-- Toggle (bool)
-- Choice (str)  [from a list of options]
-- Multichoice (list)  [of things from a list of options]
-- Text (str)
-- Path (str)
-- Number (int)
+- `Toggle`:
+    A boolean True/False
+- `Choice`:
+    Choose an option (str) from a list
+- `MappedChoice`:
+    Choose an option (str) from a list, but have a different internal value mapped to it
+- `Multichoice`:
+    Choose multiple options (str) from a list
+- `MappedMultichoice`:
+    Choose multiple options (str) from a list, but have different internal values mapped to them
+- `Text`:
+    Just a basic text value
+- `Path`:
+    A file path whose existence can be checked
+- `Number`:
+    An integer that can be set or incremented and decremented
 
-You can also inherit from the base Setting class to easily create custom ones.
+You can also inherit from the `BaseSetting` class to easily create custom ones.
```

### Comparing `object-settings-4.1/pyproject.toml` & `object-settings-4.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 [project]
 
 name = "object-settings"
-version = "4.1"
+version = "4.2"
 description = "Simple object-oriented config library, where your settings are objects"
 readme = "README.md"
+dynamic = ["dependencies"]
 keywords = ["settings", "setting", "config", "OOP", "GUI"]
 urls = {"Homepage"="https://github.com/SamuLumio/object-settings"}
 license = {text="MIT License"}
 
-dependencies = [
-    "appdirs>=1.3.0",
-    "PyYAML"
-]
-
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Typing :: Typed",
     "Intended Audience :: Developers",
@@ -25,8 +21,9 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: User Interfaces"
 ]
 
 [tool.setuptools]
 include-package-data = true
-package-data = {'settings_gui.tkinter'=['icons/*']}
+package-data = {'settings_gui.tkinter'=['icons/*']}
+dynamic = { dependencies = {file = "requirements.txt"} }
```

### Comparing `object-settings-4.1/src/object_settings.egg-info/PKG-INFO` & `object-settings-4.2/src/object_settings.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: object-settings
-Version: 4.1
+Version: 4.2
 Summary: Simple object-oriented config library, where your settings are objects
 License: MIT License
 Project-URL: Homepage, https://github.com/SamuLumio/object-settings
 Keywords: settings,setting,config,OOP,GUI
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,168 +15,179 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Description-Content-Type: text/markdown
 
 
-# object-settings
+object-settings
+===============
 
 Simple-to-use object-oriented Python config library, where your settings are objects.
 
-Their values have automatic validation and get saved to a file that's seamlessly
-written and read in the background, so you don't have to worry about any of it. 
-This makes it quick to define and use settings (see examples below).
+Their values have automatic validation and get saved to a file that's seamlessly written and read in the background, so you don't have to worry about any of it. This makes it quick to define and use settings (see examples below).
 
 
 
-Installation & usage
-====================
+## Installation & usage
 
 This package is on PyPi, so you can just do `pip install object-settings`
 
 After which it will be available with just the module name `settings`
 
-    import settings
-    settings.setup("Your app name")
+```python
+import settings
+settings.setup("Your app name")
     
-    your_option1 = settings.Toggle("Your first option label")
-    your_option2 = settings.Number("Your second option label")
+your_option1 = settings.Toggle("Your first option label")
+your_option2 = settings.Number("Your second option label")
+```
 
 
 
-Simple objects
-==============
+## Just simple objects
 
 For example, you can set a font size at the top of your ui file:
 
-    font = settings.Number(default=14)
+```python
+font = settings.Number(default=14)
 
-    ...
-    someuilib.Label("Bababooey", size=font.value)
-    ...
-    someuilib.Textbox("Lorem ipsum dolor...", font_size=font.value)
-    ...
+...
+someuilib.Label("Bababooey", size=font.value)
+...
+someuilib.Textbox("Lorem ipsum dolor...", font_size=font.value)
+...
+```
 
 Or if a setting is only checked in one place, it can be used without defining a variable:
 
-    if settings.Toggle("Update app automatically", default=True):
-        # do update
+```python
+if settings.Toggle("Update app automatically", default=True):
+    # do update
+```
 
 (it doesn't matter if the same setting is initialized multiple times)
 
 
 
-Integration
-===========
+## Integration
 
 The setting objects support "equals"-checking with actual values:
 
-    speed = settings.Number("Speed limit", 5)
-    
-    print(speed == 5)
-    >> True
-    print(speed == 3)
-    >> False
+```python
+speed = settings.Number("Speed limit", 5)
+
+print(speed == 5)
+>> True
+print(speed == 3)
+>> False
+```
 
 In addition, they work with many type-specific operations:
 
-    for selection in settings.Multichoice():
-        ...
+```python
+for selection in settings.Multichoice():
+    ...
+
+if settings.Toggle():
+    ...
+```
+
 
-    if settings.Toggle():
-        ...
 
+## Automatic storing
 
+When a setting's value is read/set, object-settings automatically creates and updates a config file on the disk in the background. It can read many file types, like `.cfg`, `.json` and `.yaml`. Any file deletions or unparsable external modifications are also handled.
 
-Automatic storing
-=================
+By default, the files are saved to a standard config location, depending on the platform (uses [appdirs](https://github.com/ActiveState/appdirs) package for paths). You can also set a custom directory for e.g. running in a Docker container.
 
-When a setting's value is read/set, object-settings automatically creates and updates 
-a config file on the disk in the background. 
-It can read many file types, like `.cfg`, `.json` and `.yaml`.
-Any file deletions or unparsable external modifications are also handled.
+Setting values are also automatically read from the environment, like from env vars or command line options. The under-the-hood parser system is also very extensible, so you can create and add custom ones for e.g. a custom database.
 
-By default, the files are saved to a standard config location, depending on the platform 
-(uses [appdirs](https://github.com/ActiveState/appdirs) package for paths). 
-You can also set a custom directory for e.g. running in a Docker container.
 
-Setting values are also automatically read from the environment, like from env vars or command line options.
-The under-the-hood parser system is also very extensible, so you can create and add custom ones for e.g. a custom database.
 
+## Value validation
 
+When a new value is set, it automatically gets validated and raises a `ValueError` if it doesn't pass:
 
-Value validation
-================
+```python
+update_interval = settings.Number("Update interval", default=5)
+update_interval.set("Daily")
+>> ValueError
+```
 
-When a new value is set, it automatically gets validated and raises a `ValueError` if it doesn't pass.
-This validation includes more than just datatypes, for example numbers can have min/max limits, 
-or a path setting can be set to require an existing path.
+This validation includes more than just datatypes, for example numbers can have min/max limits, or a path setting can be set to require an existing path:
 
+```python
+path = settings.Path("Download path", has_to_exist=True)
+path.set("/nonexistent/directory")
+>> ValueError
+```
 
 
-Listen for changes
-==================
 
-If you have some update function that you want to be called when a setting is changed, 
-you can add that function as a listener:
+## Listen for changes
 
-    some_setting.add_listener(your_function)
+If you have some update function that you want to be called when a setting is changed, you can add that function as a listener:
+
+```python
+some_setting.add_listener(your_function)
+```
 
 Now the function will be called every time when a new value is set.
 
 
 
-Sections
-========
+## Sections
 
-Optionally, if you have a lot of settings, you can organize them into sections 
-(which also works well with UIs)
+Optionally, if you have a lot of settings, you can organize them into sections (which also works well with UIs):
 
-    download_options = settings.Section("Downloader settings")
-    speed = settings.Number("Speed limit", 5, section=download_options)
-    dir = settings.Path("Target directory", '/home/yomama/Downloads', section=download_options)
-    server = settings.Choice("Mirror", ["Europe", "Asia", "America", "Africa"], "Asia", section=download_options)
+```python
+download_options = settings.Section("Downloader settings")
+speed = settings.Number("Speed limit", 5, section=download_options)
+dir = settings.Path("Target directory", '/home/yomama/Downloads', section=download_options)
+server = settings.Choice("Mirror", ["Europe", "Asia", "America", "Africa"], "Asia", section=download_options)
+```
 
 
 
-Did I mention free GUIs?
-========================
+## Did I mention free GUIs?
 
-That's right, this library also includes a separate `settings_gui` package that has 
-pre-made settings menus for both tkinter and ttk, with GTK and others to come.
-They have full integration with the aforementioned systems, like validation and sections.
+That's right, this library also includes a separate `settings_gui` package that has pre-made settings menus for both tkinter and ttk, with GTK and others to come. They have full integration with the aforementioned systems, like validation and sections.
 
 Here's an example of some dummy settings with both libraries: 
-(notice the warning for the misspelt download path)
 
-<figure>
-  <img src="readme-images/ttk.png">
-  <figcaption>Nice-looking ttk (theme: Sun Valley dark)</figcaption>
-</figure>
+*(notice the warning for the misspelt download path)*
+
+![Ttk](https://github.com/SamuLumio/object-settings/blob/master/readme-images/ttk.png?raw=true)
+*Nice-looking ttk (theme: Sun Valley dark)*
 
-<figure>
-  <img src="readme-images/tkinter.png">
-  <figcaption>Bare tkinter works too</figcaption>
-</figure>
+![Tkinter](https://github.com/SamuLumio/object-settings/blob/master/readme-images/tkinter.png?raw=true)
+*Bare tkinter works too*
 
-And you can get this automatically for all your defined settings by just calling one function! 
-(`SettingsFrame` or `SettingsWindow`, depending on preference)
+And you can get this automatically for all your defined settings by just calling one function (`SettingsFrame` or `SettingsWindow`, depending on preference)
 
-Or, if you want to get more custom/contextual, you can also use the individual 
-setting widgets and place them around your app (submodule `type_frames`).
+Or, if you want to get more custom/contextual, you can also use the individual setting widgets and place them around your app (submodule `type_frames`).
 
 
 
-Setting types
-=============
+## Setting types
 
 List of currently available setting types:
 
-- Toggle (bool)
-- Choice (str)  [from a list of options]
-- Multichoice (list)  [of things from a list of options]
-- Text (str)
-- Path (str)
-- Number (int)
+- `Toggle`:
+    A boolean True/False
+- `Choice`:
+    Choose an option (str) from a list
+- `MappedChoice`:
+    Choose an option (str) from a list, but have a different internal value mapped to it
+- `Multichoice`:
+    Choose multiple options (str) from a list
+- `MappedMultichoice`:
+    Choose multiple options (str) from a list, but have different internal values mapped to them
+- `Text`:
+    Just a basic text value
+- `Path`:
+    A file path whose existence can be checked
+- `Number`:
+    An integer that can be set or incremented and decremented
 
-You can also inherit from the base Setting class to easily create custom ones.
+You can also inherit from the `BaseSetting` class to easily create custom ones.
```

### Comparing `object-settings-4.1/src/object_settings.egg-info/SOURCES.txt` & `object-settings-4.2/src/object_settings.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 README.md
 pyproject.toml
+requirements.txt
 src/object_settings.egg-info/PKG-INFO
 src/object_settings.egg-info/SOURCES.txt
 src/object_settings.egg-info/dependency_links.txt
 src/object_settings.egg-info/requires.txt
 src/object_settings.egg-info/top_level.txt
 src/settings/__init__.py
 src/settings/base.py
@@ -17,14 +18,15 @@
 src/settings/backend/parsers/cli.py
 src/settings/backend/parsers/env.py
 src/settings/backend/parsers/files.py
 src/settings_gui/__init__.py
 src/settings_gui/_tk_abstractor.py
 src/settings_gui/config.py
 src/settings_gui/tkinter/__init__.py
+src/settings_gui/tkinter/lib.py
 src/settings_gui/tkinter/main.py
 src/settings_gui/tkinter/section_frames.py
 src/settings_gui/tkinter/type_frames.py
 src/settings_gui/tkinter/icons/checkmark-black.png
 src/settings_gui/tkinter/icons/checkmark-white.png
 src/settings_gui/tkinter/icons/error.png
 src/settings_gui/tkinter/icons/folder-black.png
@@ -32,9 +34,10 @@
 src/settings_gui/ttk/__init__.py
 tests/test_cli.py
 tests/test_datafiles.py
 tests/test_datatype_loader.py
 tests/test_endurance.py
 tests/test_env.py
 tests/test_gui_(manual).py
+tests/test_mappings.py
 tests/test_v1_definitions.py
 tests/test_validation.py
```

### Comparing `object-settings-4.1/src/settings/backend/config.py` & `object-settings-4.2/src/settings/backend/config.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/src/settings/backend/datatype_loader.py` & `object-settings-4.2/src/settings/backend/datatype_loader.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/src/settings/backend/main.py` & `object-settings-4.2/src/settings/backend/main.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/src/settings/backend/parsers/_template.py` & `object-settings-4.2/src/settings/backend/parsers/_template.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/src/settings/backend/parsers/cli.py` & `object-settings-4.2/src/settings/backend/parsers/cli.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/src/settings/backend/parsers/env.py` & `object-settings-4.2/src/settings/backend/parsers/env.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/src/settings/backend/parsers/files.py` & `object-settings-4.2/src/settings/backend/parsers/files.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/src/settings/base.py` & `object-settings-4.2/src/settings/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 		return self == default_section
 
 
 all_sections: list[Section] = []
 
 
 
+
 class _DefaultSection(Section):
 
 	@property
 	def name(self):
 		return config.default_section_name
 	
 	@name.setter
```

### Comparing `object-settings-4.1/src/settings_gui/tkinter/icons/checkmark-white.png` & `object-settings-4.2/src/settings_gui/tkinter/icons/checkmark-white.png`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/src/settings_gui/tkinter/icons/folder-white.png` & `object-settings-4.2/src/settings_gui/tkinter/icons/folder-white.png`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/src/settings_gui/tkinter/main.py` & `object-settings-4.2/src/settings_gui/tkinter/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 import settings, tkinter, typing
 
-from ..config import config
+from ..config import config, strings
 from . import section_frames, a
 
 
 class SettingsFrame(a.layer.Frame): # type: ignore
-	def __init__(self, master, autosave=True, save_button: typing.Optional[str] = None):
+	def __init__(self, master, autosave=True, save_button=False):
 		super().__init__(master)
 		self.sections = []
 
 		for section in settings.all_sections:
 			if section.settings != []:
 				a.layer.Frame(self).pack(pady=config.padding)  # for padding
 				a.layer.Label(self, text=section.name, font='big').pack(padx=config.padding)
 				section_frame = section_frames.SectionFrame(self, section, autosave=autosave)
 				section_frame.pack(fill='x', expand=True, padx=2*config.padding, pady=3*config.padding)
 				self.sections.append(section_frame)
 
 		if isinstance(save_button, str):
-			button = a.layer.Button(self, command=self.save_settings, text=save_button)
+			save_text = save_button  # For backwards compatibility
+		else:
+			save_text = strings.save
+
+		if save_button:
+			button = a.layer.Button(self, command=self.save_settings, text=save_text)
 			if a.is_ttk():
 				button.configure(style='Accent.TButton')  # type: ignore
 			button.pack(pady=config.padding*3)
 
 	def save_settings(self):
 		for section_frame in self.sections:
 			section_frame.save_settings()
 		if isinstance(self.master, SettingsWindow):
 			self.master.destroy()
 
 
 
 class SettingsWindow(tkinter.Toplevel):
-	def __init__(self, master, title="Settings", autosave=True, save_button: typing.Optional[str] = None):
+	def __init__(self, master, title="Settings", autosave=True, save_button=False):
 		super().__init__(master)
 		SettingsFrame(self, autosave, save_button).pack(padx=config.padding*2, pady=config.padding*2, fill='both')
 
 		self.title(title)
 	#	self.minsize(self.winfo_width(), self.winfo_height())
 		self.resizable(False, False)
```

### Comparing `object-settings-4.1/src/settings_gui/tkinter/section_frames.py` & `object-settings-4.2/src/settings_gui/tkinter/section_frames.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/src/settings_gui/tkinter/type_frames.py` & `object-settings-4.2/src/settings_gui/tkinter/type_frames.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os, typing, colorsys, settings, subprocess, tkinter.filedialog
 import tkinter as tk
 
 from ..config import config, strings
-from . import a
+from . import a, lib
 
 
 
 class _Base(a.layer.Frame): # type: ignore
 	def __init__(self, master, setting: settings.BaseSetting, autosave: bool, width_limit=30):
 		super().__init__(master)
 		settings.BaseSetting
 		self.setting = setting
 		self.variable = tk.Variable()
 		self.widget: a.layer.Widget | None = None # type: ignore
 		self.autosave = autosave
 		self.width_limit = width_limit
 
-		self.error_photoimage = tk.PhotoImage(file=_icon_path('error'))
-		self.error_icon = _AppearingWidget(a.layer.Label(self, image=self.error_photoimage))
+		self.error_photoimage = lib.Icon('error')
+		self.error_icon = lib.AppearingWidget(a.layer.Label(self, image=self.error_photoimage))
 
 		a.layer.Label(self, text=setting.name).pack(side='left', padx=config.padding)
 		a.layer.Frame(self).pack(side='left', padx=config.padding*3)
 
 		self.init()
 
 		# Settings set from envvars can't be changed
@@ -34,14 +34,15 @@
 
 		if isinstance(self.widget, (a.layer.Entry, a.layer.Spinbox, a.layer.OptionMenu)):
 			self.variable.trace_add('write', self.update_width)
 			self.variable.trace_add('write', self.validate)
 
 		self.variable.set(self.setting.get())
 
+
 	def init(self):
 		"""For faster subclassing"""
 
 
 	def set_error(self, error: bool):
 		if error:
 			self.error_icon.show()
@@ -81,58 +82,61 @@
 	def save_from_widget(self, *args):
 		if self.autosave:
 			self.save()
 
 
 
 
+
 class Toggle(_Base):
 	"""A checkbutton, or a switch if available from ttk theme"""
 	def init(self):
 		self.variable = tk.BooleanVar()
 		self.widget = a.layer.Checkbutton(self, variable=self.variable, command=self.save_from_widget)
 		if a.is_ttk():
 			self.widget.configure(style='Switch.TCheckbutton')
 
 
 
 
+
 class Choice(_Base):
 	"""A horizontal radiobutton-row or an expandable menu, depending on the number of options"""
 	def init(self):
 		self.setting: settings.Choice
 		self.variable = tk.StringVar()
-		if _options_size(self.setting) <= self.width_limit:
+		options_size = lib.calculate_options_size(self.setting.options)
+		if options_size <= self.width_limit:
 			frame = a.layer.Frame(self)
 			for option in reversed(self.setting.options):
 				a.layer.Radiobutton(frame, text=option, value=option, variable=self.variable,
 				                    command=self.save_from_widget).pack(side='right', padx=config.padding)
 			self.widget = frame
 		else:
 			self.widget = a.layer.OptionMenu(self, self.variable, self.setting.value, *self.setting.options,
 			                                 command=self.save_from_widget)
 
 
 
 
+
 class Multichoice(_Base):
 	"""Either a horizontal or vertical checkbutton-row, depending on the number of options"""
 	def init(self):
 		self.setting: settings.Multichoice
 		self.variable = self.MultichoiceVar(self.setting.options)
 		self.widget = a.layer.Frame(self)
-		direction = 'left' if (_options_size(self.setting) <= self.width_limit) else 'top'
+		options_size = lib.calculate_options_size(self.setting.options)
+		direction = 'left' if options_size <= self.width_limit else 'top'
 
 		for option in self.setting.options:
-			# noinspection PyTypeChecker
 			a.layer.Checkbutton(self.widget, text=option, variable=self.variable[option],
 			                    command=self.save_from_widget).pack(side=direction, anchor='w',
 			                                                        padx=config.padding / 2)
 
-
 	class MultichoiceVar:
 		def __init__(self, options: list):
 			super().__init__()
 			self.variables = {}
 			for option in options:
 				self.variables[option] = tk.BooleanVar()
 
@@ -145,64 +149,43 @@
 
 		def __getitem__(self, item):
 			return self.variables[item]
 
 
 
 
+
 class Text(_Base):
 	"""Entry field with an appearing done-button (if autosave)"""
 	def init(self):
 		self.variable = tk.StringVar()
 		self.widget = a.layer.Entry(self, textvariable=self.variable)
-		self.icons = []
-		self.done_button = _AppearingWidget(self.icon_button('checkmark', self.save_from_widget))
+		self.done_button = lib.AppearingWidget(lib.icon_button(self, 'checkmark', self.save_from_widget))
 
 		if self.autosave:
 			self.variable.trace_add('write', lambda *args: self.show_done_button())
 
 	def show_done_button(self):
 		if self.variable.get() != self.setting.get():
 			self.done_button.show()
 
 	def save_from_widget(self, *args):
 		super().save_from_widget(*args)
 		self.done_button.hide()
 
 
-	def icon_button(self, icon: str, command: typing.Callable):
-
-		if a.is_ttk():
-			hex = a.layer.Style().lookup('TButton', 'background') # type: ignore
-			hex = str(hex).removeprefix('#')
-			rgb = tuple(int(hex[i:i + 2], 16) for i in (0, 2, 4))
-			hls = colorsys.rgb_to_hls(*rgb)
-			brightness = hls[1]
-			if brightness > 50:
-				icon += '-black'
-			else:
-				icon += '-white'
-		else:
-			icon += '-black'
-
-		path = _icon_path(icon)
-
-		icon_image = tk.PhotoImage(file=path)
-		self.icons.append(icon_image)
-		return a.layer.Button(self, image=icon_image, command=command)
-
 
 
 
 class Path(Text):
 	"""Like Text, but with a button to open a file chooser"""
 	def init(self):
 		super().init()
 		if not self.setting.set_externally:
-			self.icon_button('folder', self.browse).pack(side='right', padx=config.padding)
+			lib.icon_button(self, 'folder', self.browse).pack(side='right', padx=config.padding)
 
 	def browse(self):
 		try:
 			out = subprocess.run(['zenity', '--file-selection'], capture_output=True)
 			dir = out.stdout.decode().strip()
 			if dir:
 				self.variable.set(dir)
@@ -215,14 +198,15 @@
 			popup.add_command(label=strings.file, command=lambda: open(tkinter.filedialog.askopenfilename))
 			popup.add_command(label=strings.dir, command=lambda: open(tkinter.filedialog.askdirectory))
 			popup.tk_popup(*self.winfo_pointerxy())
 
 
 
 
+
 class Number(_Base):
 	"""Spinbox that allows to increment/decrement (or manually type in)"""
 	def init(self):
 		self.setting: settings.Number
 		self.variable = tk.IntVar()
 		self.widget = a.layer.Spinbox(self, textvariable=self.variable,
 		                              from_=self.setting.lower_limit, to=self.setting.upper_limit)
@@ -236,54 +220,12 @@
 
 
 
 types = {
 	settings.Toggle: Toggle,
 	settings.Text: Text,
 	settings.Choice: Choice,
+	settings.MappedChoice: Choice,
 	settings.Multichoice: Multichoice,
 	settings.Path: Path,
 	settings.Number: Number
 }
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-def _icon_path(icon: str):
-	if '.' not in icon:
-		icon += '.png'
-	return os.path.join(os.path.dirname(__file__), 'icons', icon)
-
-
-def _options_size(setting):
-	text = sum(len(o) for o in setting.options)
-	icons = len(setting.options) * 3
-	return text + icons
-
-
-
-
-class _AppearingWidget:
-	def __init__(self, widget: a.layer.Widget): # type: ignore
-		self.widget = widget
-		self.visible = False
-
-	def show(self):
-		if not self.visible:
-			self.widget.pack(side='right', padx=config.padding*2)
-			self.visible = True
-
-	def hide(self):
-		if self.visible:
-			self.widget.forget()
-			self.visible = False
```

### Comparing `object-settings-4.1/src/settings_gui/ttk/__init__.py` & `object-settings-4.2/src/settings_gui/ttk/__init__.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/tests/test_cli.py` & `object-settings-4.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/tests/test_datafiles.py` & `object-settings-4.2/tests/test_datafiles.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/tests/test_datatype_loader.py` & `object-settings-4.2/tests/test_datatype_loader.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/tests/test_endurance.py` & `object-settings-4.2/tests/test_endurance.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/tests/test_env.py` & `object-settings-4.2/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/tests/test_gui_(manual).py` & `object-settings-4.2/tests/test_gui_(manual).py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/tests/test_v1_definitions.py` & `object-settings-4.2/tests/test_v1_definitions.py`

 * *Files identical despite different names*

### Comparing `object-settings-4.1/tests/test_validation.py` & `object-settings-4.2/tests/test_validation.py`

 * *Files identical despite different names*

