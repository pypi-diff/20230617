# Comparing `tmp/q2gui-0.1.9.tar.gz` & `tmp/q2gui-0.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2gui-0.1.9.tar", max compression
+gzip compressed data, was "q2gui-0.1.90.tar", max compression
```

## Comparing `q2gui-0.1.9.tar` & `q2gui-0.1.90.tar`

### file list

```diff
@@ -1,44 +1,47 @@
--rw-r--r--   0        0        0     1485 2022-06-24 12:23:43.313507 q2gui-0.1.9/README.md
--rw-r--r--   0        0        0      517 2022-07-01 15:10:40.217866 q2gui-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       38 2022-07-01 09:36:49.292899 q2gui-0.1.9/q2gui/__init__.py
--rw-r--r--   0        0        0      860 2022-06-14 19:03:24.026484 q2gui-0.1.9/q2gui/__main__.py
--rw-r--r--   0        0        0        0 2021-11-07 21:48:48.577075 q2gui-0.1.9/q2gui/pyqt6/__init__.py
--rw-r--r--   0        0        0    12430 2022-07-01 14:45:12.834807 q2gui-0.1.9/q2gui/pyqt6/q2app.py
--rw-r--r--   0        0        0     8864 2022-07-01 15:07:27.960200 q2gui-0.1.9/q2gui/pyqt6/q2form.py
--rw-r--r--   0        0        0      292 2022-06-07 20:23:39.392676 q2gui-0.1.9/q2gui/pyqt6/q2model.py
--rw-r--r--   0        0        0     6492 2022-06-26 09:47:38.799378 q2gui-0.1.9/q2gui/pyqt6/q2widget.py
--rw-r--r--   0        0        0     4108 2022-06-30 17:50:53.772742 q2gui-0.1.9/q2gui/pyqt6/q2window.py
--rw-r--r--   0        0        0      674 2022-06-07 22:08:27.509813 q2gui-0.1.9/q2gui/pyqt6/widgets/__init__.py
--rw-r--r--   0        0        0     1284 2022-06-11 12:01:06.240215 q2gui-0.1.9/q2gui/pyqt6/widgets/q2button.py
--rw-r--r--   0        0        0     1911 2022-06-07 22:08:27.477549 q2gui-0.1.9/q2gui/pyqt6/widgets/q2check.py
--rw-r--r--   0        0        0     4902 2022-06-07 23:01:58.204314 q2gui-0.1.9/q2gui/pyqt6/widgets/q2code.py
--rw-r--r--   0        0        0     1216 2022-06-07 22:08:27.449318 q2gui-0.1.9/q2gui/pyqt6/widgets/q2combo.py
--rw-r--r--   0        0        0     5888 2022-06-26 09:38:14.730045 q2gui-0.1.9/q2gui/pyqt6/widgets/q2date.py
--rw-r--r--   0        0        0      838 2022-06-07 22:08:27.461417 q2gui-0.1.9/q2gui/pyqt6/widgets/q2doublespin.py
--rw-r--r--   0        0        0     2867 2022-06-27 19:30:58.159858 q2gui-0.1.9/q2gui/pyqt6/widgets/q2frame.py
--rw-r--r--   0        0        0     9701 2022-06-10 16:29:58.648171 q2gui-0.1.9/q2gui/pyqt6/widgets/q2grid.py
--rw-r--r--   0        0        0     1642 2022-06-25 18:59:00.919292 q2gui-0.1.9/q2gui/pyqt6/widgets/q2label.py
--rw-r--r--   0        0        0     4191 2022-06-07 22:08:27.477549 q2gui-0.1.9/q2gui/pyqt6/widgets/q2line.py
--rw-r--r--   0        0        0     1162 2022-06-07 22:08:27.477549 q2gui-0.1.9/q2gui/pyqt6/widgets/q2list.py
--rw-r--r--   0        0        0     2632 2022-06-26 09:47:01.185401 q2gui-0.1.9/q2gui/pyqt6/widgets/q2lookup.py
--rw-r--r--   0        0        0      813 2022-06-07 22:08:27.477549 q2gui-0.1.9/q2gui/pyqt6/widgets/q2progressbar.py
--rw-r--r--   0        0        0     2300 2022-06-26 09:55:42.945002 q2gui-0.1.9/q2gui/pyqt6/widgets/q2radio.py
--rw-r--r--   0        0        0     4962 2022-06-07 22:08:27.509813 q2gui-0.1.9/q2gui/pyqt6/widgets/q2relation.py
--rw-r--r--   0        0        0      354 2022-06-07 20:52:13.645764 q2gui-0.1.9/q2gui/pyqt6/widgets/q2scroller.py
--rw-r--r--   0        0        0    15862 2022-06-10 14:26:58.494219 q2gui-0.1.9/q2gui/pyqt6/widgets/q2sheet.py
--rw-r--r--   0        0        0      469 2022-06-07 22:08:27.509813 q2gui-0.1.9/q2gui/pyqt6/widgets/q2space.py
--rw-r--r--   0        0        0      548 2022-06-07 22:08:27.509813 q2gui-0.1.9/q2gui/pyqt6/widgets/q2spin.py
--rw-r--r--   0        0        0     2671 2022-06-26 19:31:59.419828 q2gui-0.1.9/q2gui/pyqt6/widgets/q2tab.py
--rw-r--r--   0        0        0      567 2022-06-07 22:08:27.481582 q2gui-0.1.9/q2gui/pyqt6/widgets/q2text.py
--rw-r--r--   0        0        0     5924 2022-06-26 09:47:24.758829 q2gui-0.1.9/q2gui/pyqt6/widgets/q2toolbar.py
--rw-r--r--   0        0        0      519 2022-06-07 22:08:27.509813 q2gui-0.1.9/q2gui/pyqt6/widgets/q2toolbutton.py
--rw-r--r--   0        0        0    15066 2022-07-01 14:33:58.149853 q2gui-0.1.9/q2gui/q2app.py
--rw-r--r--   0        0        0     7239 2022-07-01 14:51:40.124591 q2gui-0.1.9/q2gui/q2dialogs.py
--rw-r--r--   0        0        0    45210 2022-07-01 14:39:19.872289 q2gui-0.1.9/q2gui/q2form.py
--rw-r--r--   0        0        0    15185 2022-06-27 19:23:16.054592 q2gui-0.1.9/q2gui/q2model.py
--rw-r--r--   0        0        0     1456 2022-05-01 11:47:55.707188 q2gui-0.1.9/q2gui/q2utils.py
--rw-r--r--   0        0        0     3949 2022-06-11 12:02:03.191708 q2gui-0.1.9/q2gui/q2widget.py
--rw-r--r--   0        0        0     2701 2022-07-01 14:50:49.682588 q2gui-0.1.9/q2gui/q2window.py
--rw-r--r--   0        0        0       22 2022-07-01 15:10:41.153798 q2gui-0.1.9/q2gui/version.py
--rw-r--r--   0        0        0     2210 2022-07-01 15:10:42.391558 q2gui-0.1.9/setup.py
--rw-r--r--   0        0        0     2065 2022-07-01 15:10:42.392599 q2gui-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      576 2023-06-17 19:21:40.577730 q2gui-0.1.90/pyproject.toml
+-rw-r--r--   0        0        0       39 2022-12-11 17:39:14.961644 q2gui-0.1.90/q2gui/__init__.py
+-rw-r--r--   0        0        0      892 2022-12-11 17:39:14.961644 q2gui-0.1.90/q2gui/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:14.961644 q2gui-0.1.90/q2gui/pyqt6/__init__.py
+-rw-r--r--   0        0        0    17169 2023-06-17 19:19:44.077472 q2gui-0.1.90/q2gui/pyqt6/q2app.py
+-rw-r--r--   0        0        0     9406 2023-06-16 23:30:46.736176 q2gui-0.1.90/q2gui/pyqt6/q2form.py
+-rw-r--r--   0        0        0      309 2022-12-11 17:39:14.961644 q2gui-0.1.90/q2gui/pyqt6/q2model.py
+-rw-r--r--   0        0        0     9758 2023-04-26 21:46:22.544312 q2gui-0.1.90/q2gui/pyqt6/q2style.py
+-rw-r--r--   0        0        0     8068 2023-04-23 14:14:48.845890 q2gui-0.1.90/q2gui/pyqt6/q2widget.py
+-rw-r--r--   0        0        0     4391 2023-06-17 19:21:29.680879 q2gui-0.1.90/q2gui/pyqt6/q2window.py
+-rw-r--r--   0        0        0      754 2023-02-06 11:50:26.449600 q2gui-0.1.90/q2gui/pyqt6/widgets/__init__.py
+-rw-r--r--   0        0        0     1320 2023-01-02 22:28:53.285564 q2gui-0.1.90/q2gui/pyqt6/widgets/q2button.py
+-rw-r--r--   0        0        0     1979 2022-12-11 17:39:14.965644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2check.py
+-rw-r--r--   0        0        0    15572 2023-04-22 11:24:23.071797 q2gui-0.1.90/q2gui/pyqt6/widgets/q2code.py
+-rw-r--r--   0        0        0     1380 2023-03-23 12:34:19.124118 q2gui-0.1.90/q2gui/pyqt6/widgets/q2combo.py
+-rw-r--r--   0        0        0     6423 2023-03-23 10:59:04.941764 q2gui-0.1.90/q2gui/pyqt6/widgets/q2date.py
+-rw-r--r--   0        0        0      872 2022-12-11 17:39:14.969649 q2gui-0.1.90/q2gui/pyqt6/widgets/q2doublespin.py
+-rw-r--r--   0        0        0     3384 2023-04-23 14:16:17.951094 q2gui-0.1.90/q2gui/pyqt6/widgets/q2frame.py
+-rw-r--r--   0        0        0     8651 2023-04-26 22:53:02.233686 q2gui-0.1.90/q2gui/pyqt6/widgets/q2grid.py
+-rw-r--r--   0        0        0     4285 2023-02-10 12:17:07.214549 q2gui-0.1.90/q2gui/pyqt6/widgets/q2image.py
+-rw-r--r--   0        0        0     1699 2022-12-11 17:39:14.969649 q2gui-0.1.90/q2gui/pyqt6/widgets/q2label.py
+-rw-r--r--   0        0        0     4365 2023-03-24 12:17:15.560065 q2gui-0.1.90/q2gui/pyqt6/widgets/q2line.py
+-rw-r--r--   0        0        0     1207 2022-12-11 17:39:14.973644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2list.py
+-rw-r--r--   0        0        0     2775 2023-01-07 23:02:31.193844 q2gui-0.1.90/q2gui/pyqt6/widgets/q2lookup.py
+-rw-r--r--   0        0        0      663 2022-12-11 17:39:14.973644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2progressbar.py
+-rw-r--r--   0        0        0     2406 2023-04-23 23:59:43.413400 q2gui-0.1.90/q2gui/pyqt6/widgets/q2radio.py
+-rw-r--r--   0        0        0     6581 2023-03-23 18:18:53.089815 q2gui-0.1.90/q2gui/pyqt6/widgets/q2relation.py
+-rw-r--r--   0        0        0      373 2022-12-11 17:39:14.973644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2scroller.py
+-rw-r--r--   0        0        0    16774 2023-04-23 13:12:45.146324 q2gui-0.1.90/q2gui/pyqt6/widgets/q2sheet.py
+-rw-r--r--   0        0        0      490 2022-12-11 17:39:14.977644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2space.py
+-rw-r--r--   0        0        0      574 2022-12-11 17:39:14.977644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2spin.py
+-rw-r--r--   0        0        0     2772 2022-12-25 20:49:02.663455 q2gui-0.1.90/q2gui/pyqt6/widgets/q2tab.py
+-rw-r--r--   0        0        0      920 2023-02-02 22:06:03.288112 q2gui-0.1.90/q2gui/pyqt6/widgets/q2text.py
+-rw-r--r--   0        0        0     6913 2023-04-21 18:39:08.528361 q2gui-0.1.90/q2gui/pyqt6/widgets/q2toolbar.py
+-rw-r--r--   0        0        0      541 2022-12-11 17:39:14.977644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2toolbutton.py
+-rw-r--r--   0        0        0    20612 2023-06-17 19:08:41.267761 q2gui-0.1.90/q2gui/q2app.py
+-rw-r--r--   0        0        0      252 2023-04-17 11:18:17.375721 q2gui-0.1.90/q2gui/q2colors.py
+-rw-r--r--   0        0        0    12311 2023-06-09 10:52:14.113389 q2gui-0.1.90/q2gui/q2dialogs.py
+-rw-r--r--   0        0        0    68487 2023-06-09 10:49:47.244921 q2gui-0.1.90/q2gui/q2form.py
+-rw-r--r--   0        0        0    15084 2023-04-26 21:52:49.700754 q2gui-0.1.90/q2gui/q2model.py
+-rw-r--r--   0        0        0     5284 2023-04-26 19:43:48.136965 q2gui-0.1.90/q2gui/q2style.py
+-rw-r--r--   0        0        0     1515 2022-12-11 17:39:14.985654 q2gui-0.1.90/q2gui/q2utils.py
+-rw-r--r--   0        0        0     4448 2023-04-23 09:29:31.258882 q2gui-0.1.90/q2gui/q2widget.py
+-rw-r--r--   0        0        0     3189 2022-12-13 12:21:42.250012 q2gui-0.1.90/q2gui/q2window.py
+-rw-r--r--   0        0        0       22 2023-06-17 19:21:42.987988 q2gui-0.1.90/q2gui/version.py
+-rw-r--r--   0        0        0     1533 2022-12-11 17:39:14.929664 q2gui-0.1.90/README.md
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 q2gui-0.1.90/PKG-INFO
```

### Comparing `q2gui-0.1.9/README.md` & `q2gui-0.1.90/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# The light Python GUI builder (currently based on PyQt6)
-
-# How to start 
-## With docker && x11:
-```bash
-git clone https://github.com/AndreiPuchko/q2gui.git
-#                      sudo if necessary 
-cd q2gui/docker-x11 && ./build_and_run_menu.sh
-```
-## With PyPI package:
-```bash
-poetry new project_01 && cd project_01 && poetry shell
-poetry add q2gui
-cd project_01
-python -m q2gui > example_app.py && python example_app.py
-```
-## Explore sources:
-```bash
-git clone https://github.com/AndreiPuchko/q2gui.git
-cd q2gui
-pip3 install poetry
-poetry shell
-poetry install
-python3 demo/demo_00.py     # All demo launcher
-python3 demo/demo_01.py     # basic: main menu, form & widgets
-python3 demo/demo_02.py     # forms and forms in form
-python3 demo/demo_03.py     # grid form (CSV data), automatic creation of forms based on data
-python3 demo/demo_04.py     # progressbar, data loading, sorting and filtering
-python3 demo/demo_05.py     # nonmodal form
-python3 demo/demo_06.py     # code editor
-python3 demo/demo_07.py     # database app (4 tables, mock data loading) - requires a q2db package
-python3 demo/demo_08.py     # database app, requires a q2db package, autoschema
-```
-
-## demo/demo_07.py screenshot
-=======
-![Alt text](https://andreipuchko.github.io/q2gui/screenshot.png)
-# Build standalone executable 
-(The resulting executable file will appear in the folder  dist/)
-### One file
-```bash
-pyinstaller -F demo/demo.py
-```
-
-### One directory
-```bash
-pyinstaller -D demo/demo.py
-```
+# The light Python GUI builder (currently based on PyQt6)
+
+# How to start 
+## With docker && x11:
+```bash
+git clone https://github.com/AndreiPuchko/q2gui.git
+#                      sudo if necessary 
+cd q2gui/docker-x11 && ./build_and_run_menu.sh
+```
+## With PyPI package:
+```bash
+poetry new project_01 && cd project_01 && poetry shell
+poetry add q2gui
+cd project_01
+python -m q2gui > example_app.py && python example_app.py
+```
+## Explore sources:
+```bash
+git clone https://github.com/AndreiPuchko/q2gui.git
+cd q2gui
+pip3 install poetry
+poetry shell
+poetry install
+python3 demo/demo_00.py     # All demo launcher
+python3 demo/demo_01.py     # basic: main menu, form & widgets
+python3 demo/demo_02.py     # forms and forms in form
+python3 demo/demo_03.py     # grid form (CSV data), automatic creation of forms based on data
+python3 demo/demo_04.py     # progressbar, data loading, sorting and filtering
+python3 demo/demo_05.py     # nonmodal form
+python3 demo/demo_06.py     # code editor
+python3 demo/demo_07.py     # database app (4 tables, mock data loading) - requires a q2db package
+python3 demo/demo_08.py     # database app, requires a q2db package, autoschema
+```
+
+## demo/demo_07.py screenshot
+=======
+![Alt text](https://andreipuchko.github.io/q2gui/screenshot.png)
+# Build standalone executable 
+(The resulting executable file will appear in the folder  dist/)
+### One file
+```bash
+pyinstaller -F demo/demo.py
+```
+
+### One directory
+```bash
+pyinstaller -D demo/demo.py
+```
```

### Comparing `q2gui-0.1.9/pyproject.toml` & `q2gui-0.1.90/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-[tool.poetry]
-name = "q2gui"
-version = "0.1.9"
-description = "Python GUI toolkit"
-authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
-license = "Apache 2.0"
-readme = "README.md"
-
-[tool.poetry.dependencies]
-python = "^3.8"
-PyQt6 = "^6.3.0"
-PyQt6-QScintilla = "^2.13.3"
-q2db = "latest"
-
-
-[tool.poetry.dev-dependencies]
-pytest = "^7.0.0"
-flake8 = "latest"
-black = "latest"
-pyinstaller = "latest"
-
-[tool.black]
-line-length = 110
-
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "q2gui"
+version = "0.1.90"
+description = "Python GUI toolkit"
+authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
+license = "Apache 2.0"
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = ">=3.8.1"
+PyQt6 = "^6.3.0"
+PyQt6-QScintilla = "^2.13.3"
+q2db = ">=0.1.10"
+darkdetect = "^0.8.0"
+
+
+[tool.poetry.dev-dependencies]
+pytest = "^7.0.0"
+flake8 = "^4.0.1"
+black =  "^22.3.0"
+pyinstaller = "^4.5.0"
+
+[tool.black]
+line-length = 110
+
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `q2gui-0.1.9/q2gui/__main__.py` & `q2gui-0.1.90/q2gui/__main__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-print("""
-from q2gui.q2app import Q2App
-from q2gui.q2form import Q2Form
-from q2gui.q2app import load_q2engine
-
-load_q2engine(globals(), "PyQt6")
-
-from q2gui.q2dialogs import q2Mess
-
-
-class firstApp(Q2App):
-    def on_init(self):
-        self.add_menu(
-            "File|About", lambda: q2Mess("First application!"), toolbar=1
-        )
-        self.add_menu("File|First Form", self.first_form, toolbar=1)
-        self.add_menu("File|-")
-        self.add_menu("File|Exit", self.close, toolbar=1)
-        return super().on_init()
-
-    def first_form(self):
-        form = Q2Form("FirstForm")
-        form.add_control("", "First Label")
-        form.add_control("field", "First Field")
-        form.add_control("", "Close Form", control="button", valid=form.close)
-        form.run()
-
-
-if __name__ == "__main__":
-    firstApp("q2gui - the first app").run()
-
-""")
+print("""
+from q2gui.q2app import Q2App
+from q2gui.q2form import Q2Form
+from q2gui.q2app import load_q2engine
+
+load_q2engine(globals(), "PyQt6")
+
+from q2gui.q2dialogs import q2Mess
+
+
+class firstApp(Q2App):
+    def on_init(self):
+        self.add_menu(
+            "File|About", lambda: q2Mess("First application!"), toolbar=1
+        )
+        self.add_menu("File|First Form", self.first_form, toolbar=1)
+        self.add_menu("File|-")
+        self.add_menu("File|Exit", self.close, toolbar=1)
+        return super().on_init()
+
+    def first_form(self):
+        form = Q2Form("FirstForm")
+        form.add_control("", "First Label")
+        form.add_control("field", "First Field")
+        form.add_control("", "Close Form", control="button", valid=form.close)
+        form.run()
+
+
+if __name__ == "__main__":
+    firstApp("q2gui - the first app").run()
+
+""")
```

### Comparing `q2gui-0.1.9/q2gui/pyqt6/q2form.py` & `q2gui-0.1.90/q2gui/pyqt6/q2form.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,256 +1,264 @@
-if __name__ == "__main__":
-    import sys
-    sys.path.insert(0, ".")
-    from demo.demo import demo
-
-    demo()
-
-from PyQt6.QtWidgets import QDialog, QMdiSubWindow, QApplication, QApplication
-from PyQt6.QtCore import Qt, QEvent
-from PyQt6.QtGui import QKeySequence, QKeyEvent
-
-
-import q2gui.q2app as q2app
-import q2gui.q2form as q2form
-import q2gui.pyqt6.widgets
-
-from q2gui.pyqt6.q2app import Q2QtWindow
-from q2gui.q2utils import num
-
-import q2gui.q2dialogs
-# from q2gui.q2dialogs import q2Mess, q2Wait, q2AskYN
-
-from q2gui.pyqt6.q2widget import Q2Widget
-
-
-class Q2Form(q2form.Q2Form):
-    def __init__(self, title=""):
-        super().__init__(title=title)
-        self._Q2FormWindow_class = Q2FormWindow
-        self._q2dialogs = q2gui.q2dialogs
-        self.q2_app = QApplication.activeWindow()
-        self.on_init()
-
-
-class Q2FormWindow(QDialog, q2form.Q2FormWindow, Q2QtWindow, Q2Widget):
-    def __init__(self, q2_form: Q2Form, title=""):
-        super().__init__(q2_form)
-        title = title if title else q2_form.title
-        Q2QtWindow.__init__(self, title)
-        self._widgets_package = q2gui.pyqt6.widgets
-
-    def restore_geometry(self, settings):
-        paw = self.parent()
-
-        if paw is not None:
-            # save default == minimal size
-            sizeBefore = paw.size()
-
-            if self.q2_form.do_not_save_geometry:
-                width, height = 1, 1
-            else:
-                width = num(settings.get(self.window_title, "width", "-1"))
-                height = num(settings.get(self.window_title, "height", "-1"))
-
-            if -1 in [width, height]:  # bad settings or first run
-                if self.mode != "grid" and sum(self.q2_form.init_size) > 0:
-                    # init size given
-                    width, height = self.get_init_size()
-                else:
-                    width = paw.parent().size().width() * 0.9 if self.mode == "grid" else 0.5
-                    height = paw.parent().size().height() * 0.9 if self.mode == "grid" else 0.5
-
-            paw.resize(width, height)
-
-            sizeAfter = paw.size()
-            self.expand_size(paw, sizeBefore, sizeAfter)
-
-            if self.q2_form.do_not_save_geometry:
-                left, top = self.center_pos()
-            else:
-                left = num(settings.get(self.window_title, "left", "-1"))
-                top = num(settings.get(self.window_title, "top", "-1"))
-                if -1 in [left, top]:  # bad settings or first run
-                    left, top = self.center_pos()
-
-            paw.move(left, top)
-
-            self.fit_size_and_pos(paw)
-
-            if num(settings.get(self.window_title, "is_max", "0")):
-                self.showMaximized()
-                paw.move(0, 0)
-
-    def center_pos(self):
-        left = (self.parent().parent().size().width() - self.parent().size().width()) / 2
-        top = (self.parent().parent().size().height() - self.parent().size().height()) / 2
-        return left, top
-
-    def expand_size(self, paw, sizeBefore, sizeAfter):
-        wDelta = 0 if sizeBefore.width() < sizeAfter.width() else sizeBefore.width() - sizeAfter.width()
-        hDelta = 0 if sizeBefore.height() < sizeAfter.height() else sizeBefore.height() - sizeAfter.height()
-        if wDelta or hDelta:
-            paw.resize(paw.size().width() + wDelta, paw.size().height() + hDelta)
-
-    def get_init_size(self):
-        w, h = self.q2_form.init_size
-        parent_size = self.parent().parent().size()
-        return [parent_size.width() * w / 100, parent_size.height() * h / 100]
-
-    def fit_size_and_pos(self, paw):
-        """ensure form fits outside window"""
-        parent_size = paw.parent().size()
-
-        size = paw.size()
-        original_size = paw.size()
-
-        pos = paw.pos()
-        orginal_pos = paw.pos()
-        # width
-        if parent_size.width() - (size.width()) < 0:
-            size.setWidth(parent_size.width())
-        if pos.x() + size.width() > parent_size.width():
-            pos.setX(parent_size.width() - size.width())
-        if pos.x() < 0:
-            pos.setX(0)
-        # height
-        if parent_size.height() - (size.height()) < 0:
-            size.setHeight(parent_size.height())
-
-        if pos.y() + size.height() > parent_size.height():
-            pos.setY(parent_size.height() - size.height())
-        if pos.y() < 0:
-            pos.setY(0)
-        if orginal_pos != pos:
-            paw.move(pos)
-        if size != original_size:
-            paw.resize(size)
-
-    def set_position(self, left, top):
-        left = int(left)
-        top = int(top)
-        paw = self.parent()
-        if paw is not None:
-            paw.move(left, top)
-        else:
-            self.move(left, top)
-
-    def set_size(self, w, h):
-        w = int(w)
-        h = int(h)
-        paw = self.parent()
-        if paw is not None:
-            paw.resize(w, h)
-        else:
-            self.resize(w, h)
-
-    def get_position(self):
-        parent_mdi_sub_window = self.parent()
-        if parent_mdi_sub_window is not None:
-            return (parent_mdi_sub_window.pos().x(), parent_mdi_sub_window.pos().y())
-
-    def showEvent(self, event=None):
-        if self.shown:
-            return
-        if self not in self.q2_form.form_stack:
-            self.q2_form.form_stack.append(self)
-
-        if not self.q2_form.i_am_child:
-            for widget_name in self.widgets:
-                widget = self.widgets[widget_name]
-                if widget.focusPolicy() == Qt.FocusPolicy.NoFocus:
-                    continue
-                if hasattr(widget, "isReadOnly") and widget.isReadOnly():
-                    continue
-                if widget.isEnabled():
-                    widget.setFocus()
-                    break
-
-        if event:
-            event.accept()
-
-        self.q2_form.form_is_active = True
-        # if self.mode == "form":
-        #     self.q2_form.form_is_active = True
-        #     if self.q2_form.before_form_show() is False:
-        #         # self.close()
-        #         self.q2_form.close()
-        #         return
-
-        if not isinstance(self.parent(), QMdiSubWindow):
-            self.escapeEnabled = False
-
-        self.shown = True
-        self.restore_geometry(q2app.q2_app.settings)
-
-        # if self.mode == "form":
-        #     self.parent().setWindowFlag(Qt.WindowMaximizeButtonHint, False)
-
-        if hasattr(self.parent(), "setWindowFlag"):
-            self.parent().setWindowFlag(Qt.WindowType.WindowMinimizeButtonHint, False)
-
-            if self.q2_form.hide_title:
-                self.parent().setWindowFlags(
-                    Qt.WindowType.CustomizeWindowHint
-                    | Qt.WindowType.FramelessWindowHint
-                    | Qt.WindowType.WindowStaysOnBottomHint
-                    | Qt.WindowType.WindowCloseButtonHint
-                )
-        if self.q2_form.maximized:
-            self.showMaximized()
-        if self.mode == "form":
-            self.q2_form.after_form_show()
-        elif self.mode == "grid":
-            self.q2_form.after_grid_show()
-
-    def keyPressEvent(self, event: QEvent):
-        key = event.key()
-        try:
-            keyText = QKeySequence(key).toString()
-        except Exception:
-            keyText = ""
-        if key == Qt.Key.Key_Escape and self.escapeEnabled:
-            self.close()
-        elif key == Qt.Key.Key_Escape and not self.escapeEnabled:
-            event.ignore()
-            # return
-        elif self.mode == "form" and key in (Qt.Key.Key_Up,):
-            QApplication.sendEvent(
-                self, QKeyEvent(QEvent.Type.KeyPress, Qt.Key.Key_Tab, Qt.KeyboardModifier.ShiftModifier)
-            )
-        elif self.mode == "form" and key in (Qt.Key.Key_Enter, Qt.Key.Key_Return, Qt.Key.Key_Down):
-            QApplication.sendEvent(self, QKeyEvent(QEvent.Type.KeyPress, Qt.Key.Key_Tab, event.modifiers()))
-        elif self.mode == "grid" and key in (Qt.Key.Key_Return,):
-            self.q2_form.grid_double_clicked()
-        elif keyText in self.hotkey_widgets:  # is it form hotkey
-            for widget in self.hotkey_widgets[keyText]:
-                if widget.is_enabled() and hasattr(widget, "valid"):
-                    widget.valid()
-                    return
-
-    def close(self):
-        # print("close event", self)
-        super().close()
-        if self.parent() is not None:
-            if isinstance(self.parent(), QMdiSubWindow):
-                self.parent().close()
-                # QDialog.close(self)
-        else:
-            QDialog.close(self)
-
-    def closeEvent(self, event=None):
-        super().close()
-        self.q2_form._close()
-        self.q2_form.form_is_active = False
-        if event:
-            event.accept()
-
-    def set_style_sheet(self, css):
-        self.setStyleSheet(css)
-
-
-# Tells the module which engine to use
-q2gui.q2dialogs.Q2Form = Q2Form
-# q2Mess
-# q2Wait
-# q2AskYN
+if __name__ == "__main__":
+    import sys
+
+    sys.path.insert(0, ".")
+    from demo.demo import demo
+
+    demo()
+
+from PyQt6.QtWidgets import QDialog, QMdiSubWindow, QApplication
+from PyQt6.QtCore import Qt, QEvent
+from PyQt6.QtGui import QKeySequence, QKeyEvent
+
+
+import q2gui.q2app as q2app
+import q2gui.q2form as q2form
+import q2gui.pyqt6.widgets
+
+from q2gui.pyqt6.q2app import Q2QtWindow
+from q2gui.q2utils import num
+
+import q2gui.q2dialogs
+
+# from q2gui.q2dialogs import q2Mess, q2Wait, q2AskYN
+
+from q2gui.pyqt6.q2widget import Q2Widget
+
+
+class Q2Form(q2form.Q2Form):
+    def __init__(self, title=""):
+        super().__init__(title=title)
+        self._Q2FormWindow_class = Q2FormWindow
+        self._q2dialogs = q2gui.q2dialogs
+        if QApplication.activeWindow():
+            self.q2_app = QApplication.activeWindow()
+        else:
+            self.q2_app = q2app.q2_app
+        self.on_init()
+
+
+class Q2FormWindow(QDialog, q2form.Q2FormWindow, Q2QtWindow, Q2Widget):
+    def __init__(self, q2_form: Q2Form, title=""):
+        super().__init__(q2_form, title)
+        # title = title if title else q2_form.title
+        Q2QtWindow.__init__(self, self.title)
+        self._widgets_package = q2gui.pyqt6.widgets
+        self.setObjectName("q2form")
+
+    def restore_geometry(self, settings):
+        paw = self.parent()
+
+        if paw is not None:
+            # save default == minimal size
+            sizeBefore = paw.size()
+
+            if self.q2_form.do_not_save_geometry:
+                width, height = 1, 1
+            else:
+                width = num(settings.get(self.window_title, "width", "-1"))
+                height = num(settings.get(self.window_title, "height", "-1"))
+
+            if -1 in [width, height]:  # bad settings or first run
+                if self.mode != "grid" and sum(self.q2_form.init_size) > 0:
+                    # init size given
+                    width, height = self.get_init_size()
+                else:
+                    width = paw.parent().size().width() * 0.9 if self.mode == "grid" else 0.5
+                    height = paw.parent().size().height() * 0.9 if self.mode == "grid" else 0.5
+
+            paw.resize(int(width), int(height))
+
+            sizeAfter = paw.size()
+            self.expand_size(paw, sizeBefore, sizeAfter)
+
+            if self.q2_form.do_not_save_geometry:
+                left, top = self.center_pos()
+            else:
+                left = num(settings.get(self.window_title, "left", "-1"))
+                top = num(settings.get(self.window_title, "top", "-1"))
+                if -1 in [left, top]:  # bad settings or first run
+                    left, top = self.center_pos()
+
+            paw.move(int(left), int(top))
+
+            self.fit_size_and_pos(paw)
+
+            if not self.q2_form.do_not_save_geometry:
+                if num(settings.get(self.window_title, "is_max", "0")):
+                    self.showMaximized()
+                    paw.move(0, 0)
+
+    def center_pos(self):
+        left = int((self.parent().parent().size().width() - self.parent().size().width()) / 2)
+        top = int((self.parent().parent().size().height() - self.parent().size().height()) / 2)
+        return left, top
+
+    def expand_size(self, paw, sizeBefore, sizeAfter):
+        wDelta = 0 if sizeBefore.width() < sizeAfter.width() else sizeBefore.width() - sizeAfter.width()
+        hDelta = 0 if sizeBefore.height() < sizeAfter.height() else sizeBefore.height() - sizeAfter.height()
+        if wDelta or hDelta:
+            paw.resize(paw.size().width() + wDelta, paw.size().height() + hDelta)
+
+    def get_init_size(self):
+        w, h = self.q2_form.init_size
+        parent_size = self.parent().parent().size()
+        return [int(parent_size.width() * w / 100), int(parent_size.height() * h / 100)]
+
+    def fit_size_and_pos(self, paw):
+        """ensure form fits outside window"""
+        parent_size = paw.parent().size()
+
+        size = paw.size()
+        original_size = paw.size()
+
+        pos = paw.pos()
+        orginal_pos = paw.pos()
+        # width
+        if parent_size.width() - (size.width()) < 0:
+            size.setWidth(parent_size.width())
+        if pos.x() + size.width() > parent_size.width():
+            pos.setX(parent_size.width() - size.width())
+        if pos.x() < 0:
+            pos.setX(0)
+        # height
+        if parent_size.height() - (size.height()) < 0:
+            size.setHeight(parent_size.height())
+
+        if pos.y() + size.height() > parent_size.height():
+            pos.setY(parent_size.height() - size.height())
+        if pos.y() < 0:
+            pos.setY(0)
+        if orginal_pos != pos:
+            paw.move(pos)
+        if size != original_size:
+            paw.resize(size)
+
+    def set_position(self, left, top):
+        left = int(left)
+        top = int(top)
+        paw = self.parent()
+        if paw is not None:
+            paw.move(left, top)
+        else:
+            self.move(left, top)
+
+    def set_size(self, w, h):
+        w = int(w)
+        h = int(h)
+        paw = self.parent()
+        if paw is not None:
+            paw.resize(w, h)
+        else:
+            self.resize(w, h)
+
+    def get_position(self):
+        parent_mdi_sub_window = self.parent()
+        if parent_mdi_sub_window is not None:
+            return (parent_mdi_sub_window.pos().x(), parent_mdi_sub_window.pos().y())
+
+    def showEvent(self, event=None):
+        if self.shown:
+            return
+        if self not in self.q2_form.form_stack:
+            self.q2_form.form_stack.append(self)
+
+        if not self.q2_form.i_am_child:
+            for widget_name in self.widgets:
+                widget = self.widgets[widget_name]
+                if widget.focusPolicy() == Qt.FocusPolicy.NoFocus:
+                    continue
+                if hasattr(widget, "isReadOnly") and widget.isReadOnly():
+                    continue
+                if widget.isEnabled():
+                    widget.setFocus()
+                    break
+
+        if event:
+            event.accept()
+
+        self.q2_form.form_is_active = True
+        # if self.mode == "form":
+        #     self.q2_form.form_is_active = True
+        #     if self.q2_form.before_form_show() is False:
+        #         # self.close()
+        #         self.q2_form.close()
+        #         return
+
+        if not isinstance(self.parent(), QMdiSubWindow):
+            self.escape_enabled = False
+
+        self.shown = True
+        self.restore_geometry(q2app.q2_app.settings)
+
+        # if self.mode == "form":
+        #     self.parent().setWindowFlag(Qt.WindowMaximizeButtonHint, False)
+
+        if hasattr(self.parent(), "setWindowFlag"):
+            self.parent().setWindowFlag(Qt.WindowType.WindowMinimizeButtonHint, False)
+
+            if self.q2_form.hide_title:
+                self.parent().setWindowFlags(
+                    Qt.WindowType.CustomizeWindowHint
+                    | Qt.WindowType.FramelessWindowHint
+                    | Qt.WindowType.WindowStaysOnBottomHint
+                    | Qt.WindowType.WindowCloseButtonHint
+                )
+        if self.q2_form.maximized:
+            self.showMaximized()
+        if self.mode == "form":
+            self.q2_form.after_form_show()
+            self.q2_form.show_()
+        elif self.mode == "grid":
+            self.q2_form.after_grid_show()
+
+    def keyPressEvent(self, event: QEvent):
+        key = event.key()
+        try:
+            keyText = QKeySequence(key).toString()
+        except Exception:
+            keyText = ""
+        if key == Qt.Key.Key_Escape and self.escape_enabled:
+            self.close()
+        elif key == Qt.Key.Key_Escape and not self.escape_enabled:
+            event.ignore()
+            # return
+        elif self.mode == "form" and key in (Qt.Key.Key_Up,):
+            QApplication.sendEvent(
+                self, QKeyEvent(QEvent.Type.KeyPress, Qt.Key.Key_Tab, Qt.KeyboardModifier.ShiftModifier)
+            )
+        elif self.mode == "form" and key in (Qt.Key.Key_Enter, Qt.Key.Key_Return, Qt.Key.Key_Down):
+            QApplication.sendEvent(self, QKeyEvent(QEvent.Type.KeyPress, Qt.Key.Key_Tab, event.modifiers()))
+        elif self.mode == "grid" and key in (Qt.Key.Key_Return,):
+            self.q2_form.grid_double_clicked()
+        elif keyText in self.hotkey_widgets:  # is it form hotkey
+            for widget in self.hotkey_widgets[keyText]:
+                if widget.is_enabled() and hasattr(widget, "valid"):
+                    widget.valid()
+                    return
+
+    def close(self):
+        # print("close event", self)
+        super().close()
+        if self.parent() is not None:
+            if isinstance(self.parent(), QMdiSubWindow):
+                self.parent().close()
+                # QDialog.close(self)
+        else:
+            QDialog.close(self)
+
+    def closeEvent(self, event=None):
+        super().close()
+        self.q2_form._close()
+        self.q2_form.form_is_active = False
+        if event:
+            event.accept()
+
+    def set_style_sheet(self, css):
+        self.setStyleSheet(css)
+
+
+# Tells the module which engine to use
+q2gui.q2dialogs.Q2Form = Q2Form
+# q2Mess
+# q2Wait
+# q2AskYN
```

### Comparing `q2gui-0.1.9/q2gui/pyqt6/q2widget.py` & `q2gui-0.1.90/q2gui/pyqt6/q2widget.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,205 +1,239 @@
-if __name__ == "__main__":
-    import sys
-
-    sys.path.insert(0, ".")
-
-    from demo.demo import demo
-
-    demo()
-
-
-from PyQt6.QtWidgets import QWidget, QSizePolicy
-from PyQt6.QtGui import QFontMetrics
-
-from q2gui import q2widget
-from q2gui.pyqt6.q2window import q2_align
-
-
-class Q2Widget(QWidget, q2widget.Q2Widget):
-    def __init__(self, meta={}):
-        super().__init__()
-        q2widget.Q2Widget.__init__(self, meta)
-        self.setContentsMargins(0, 0, 0, 0)
-
-    def mouseDoubleClickEvent(self, event):
-        if self.meta.get("dblclick"):
-            self.meta.get("dblclick")()
-        return super().mouseDoubleClickEvent(event)
-
-    def set_tooltip(self, mess):
-        self.setToolTip(mess)
-
-    def set_disabled(self, arg=True):
-        self.setEnabled(True if not arg else False)
-
-    def set_enabled(self, arg=True):
-        self.setEnabled(True if arg else False)
-
-    def set_text(self, text):
-        if hasattr(self, "setText"):
-            self.setText(f"{text}")
-
-    def get_text(self):
-        if hasattr(self, "text"):
-            return self.text()
-        return ""
-
-    def set_readonly(self, arg):
-        if hasattr(self, "setReadOnly"):
-            self.setReadOnly(True if arg else False)
-
-    def is_enabled(self):
-        return self.isEnabled()
-
-    def set_visible(self, arg=True):
-        self.setVisible(arg)
-
-    def is_visible(self):
-        if hasattr(self, "isVisible"):
-            return self.isVisible()
-
-    def is_readonly(self):
-        if hasattr(self, "isReadOnly"):
-            return self.isReadOnly()
-
-    def set_focus(self):
-        self.setFocus()
-
-    def set_maximum_width(self, width, char="O"):
-        if self.meta.get("control", "") not in ("radio", "check"):
-            if char != "":
-                # self.setMaximumWidth(QFontMetrics(self.font()).width(char) * width)
-                self.setMaximumWidth(QFontMetrics(self.font()).horizontalAdvance(char) * width)
-            else:
-                self.setMaximumWidth(width)
-
-    def set_fixed_width(self, width, char="O"):
-        if self.meta.get("control", "") not in ("radio", "check"):
-            if char != "":
-                self.setFixedWidth(QFontMetrics(self.font()).horizontalAdvance(char) * width)
-            else:
-                self.setFixedWidth(width)
-
-    def set_fixed_height(self, width, char="O"):
-        if self.meta.get("control", "") not in ("radio", "check"):
-            if char != "":
-                self.setFixedHeight(QFontMetrics(self.font()).height() * width)
-            else:
-                self.setFixedHeight(width)
-
-    def set_maximum_len(self, length):
-        if hasattr(self, "setMaxLength"):
-            return self.setMaxLength(length)
-
-    def set_alignment(self, alignment):
-        if hasattr(self, "setAlignment"):
-            self.setAlignment(q2_align[f"{alignment}"])
-
-    # def valid(self):
-    #     if self.meta.get("valid"):
-    #         return self.meta.get("valid", lambda: True)()
-    #     else:
-    #         return True
-
-    # def when(self):
-    #     if self.meta.get("when"):
-    #         return self.meta.get("when", lambda: True)()
-    #     else:
-    #         return True
-
-    def set_style_sheet(self, css: str):
-        super().set_style_sheet(css)
-        self.setStyleSheet(self.style_sheet)
-
-    def add_style_sheet(self, css: str):
-        last_style = self.styleSheet() + f"; {css}"
-        super().set_style_sheet(last_style)
-        self.setStyleSheet(last_style)
-
-    def get_style_sheet(self):
-        return self.styleSheet()
-
-    # def fix_default_height(self):
-    #     self.set_maximum_height(self.get_default_height())
-
-    def get_default_height(self):
-        return self.sizeHint().height()
-
-    def set_maximum_height(self, height):
-        self.setMaximumHeight(height)
-
-    # def fix_default_width(self):
-    #     self.set_maximum_width(self.get_default_width())
-
-    def get_default_width(self):
-        return self.sizeHint().width()
-
-    def set_size_policy(self, horizontal, vertical):
-        sp = {
-            "fixed": QSizePolicy.Policy.Fixed,
-            "minimum": QSizePolicy.Policy.Minimum,
-            "maximum": QSizePolicy.Policy.Maximum,
-            "preffered": QSizePolicy.Policy.Preferred,
-            "expanding": QSizePolicy.Policy.Expanding,
-            "minimalexpanding": QSizePolicy.Policy.MinimumExpanding,
-            "ignored": QSizePolicy.Policy.Ignored,
-        }
-
-        self.setSizePolicy(
-            sp.get(horizontal, QSizePolicy.Policy.Minimum), sp.get(vertical, QSizePolicy.Policy.Minimum)
-        )
-
-    def get_next_focus_widget(self, pos=1):
-        return self.nextInFocusChain()
-
-    def get_next_widget(self, pos=1):
-        return self.layout().widget()
-
-    def add_widget_above(self, widget, pos=0):
-        my_pos = self.parentWidget().layout().indexOf(self)
-        self.parent().layout().insertWidget(my_pos - pos, widget)
-
-    def add_widget_below(self, widget, pos=0):
-        if pos == -1:
-            self.parent().layout().addWidget(widget)
-        else:
-            my_pos = self.parentWidget().layout().indexOf(self)
-            self.parent().layout().insertWidget(my_pos + pos + 1, widget)
-
-    def remove(self):
-        self.parentWidget().layout().removeWidget(self)
-        self.setParent(None)
-
-    def get_layout_position(self):
-        return self.parentWidget().layout().indexOf(self)
-
-    def get_layout_count(self):
-        return self.parentWidget().layout().count()
-
-    def get_layout_widget(self, pos):
-        return self.parentWidget().layout().itemAt(pos).widget()
-
-    def get_layout_widgets(self):
-        return [self.get_layout_widget(x) for x in range(self.get_layout_count())]
-
-    def move_up(self):
-        pos = self.get_layout_position()
-        if pos > 0:
-            w = self.parentWidget().layout().takeAt(pos).widget()
-            self.parentWidget().layout().insertWidget(pos - 1, w)
-
-    def move_down(self):
-        pos = self.get_layout_position()
-        if pos < self.get_layout_count() - 1:
-            w = self.parentWidget().layout().takeAt(pos + 1).widget()
-            self.parentWidget().layout().insertWidget(pos, w)
-
-    def action_set_visible(self, text, mode=True):
-        for action in self.actions():
-            if action.text().strip() == text:
-                action.setVisible(mode)
-
-    def action_set_enabled(self, text, mode=True):
-        for action in self.actions():
-            if action.text().strip() == text:
-                action.setVisible(mode)
+if __name__ == "__main__":
+    import sys
+
+    sys.path.insert(0, ".")
+
+    from demo.demo import demo
+
+    demo()
+
+
+from decimal import Decimal
+from PyQt6.QtWidgets import QWidget, QSizePolicy
+from PyQt6.QtGui import QFontMetrics, QFont
+
+from q2gui import q2widget
+from q2gui.pyqt6.q2window import q2_align
+
+
+class Q2Widget(QWidget, q2widget.Q2Widget):
+    def __init__(self, meta={}):
+        super().__init__()
+        q2widget.Q2Widget.__init__(self, meta)
+        if self.meta.get("margins"):
+            self.apply_meta_margins()
+        else:
+            self.set_content_margins(1)
+
+    def apply_meta_margins(self):
+        meta_margins = self.meta.get("margins")
+        if isinstance(meta_margins, (int, Decimal)):
+            meta_margins = [meta_margins]
+        if not isinstance(meta_margins, list):
+            meta_margins = [0]
+        if len(meta_margins) == 1:
+            self.set_content_margins(int(meta_margins[0]))
+        elif len(meta_margins) == 2:
+            self.set_content_margins(int(meta_margins[0]), meta_margins[1])
+        elif len(meta_margins) == 3:
+            self.set_content_margins(int(meta_margins[0]), meta_margins[1], meta_margins[2])
+        else:
+            self.set_content_margins(int(meta_margins[0]), meta_margins[1], meta_margins[2], meta_margins[3])
+
+    def mouseDoubleClickEvent(self, event):
+        if self.meta.get("dblclick"):
+            self.meta.get("dblclick")()
+        return super().mouseDoubleClickEvent(event)
+
+    def set_tooltip(self, mess):
+        self.setToolTip(mess)
+
+    def set_disabled(self, arg=True):
+        self.setEnabled(True if not arg else False)
+
+    def set_enabled(self, arg=True):
+        self.setEnabled(True if arg else False)
+
+    def set_text(self, text):
+        if hasattr(self, "setText"):
+            self.setText(f"{text}")
+
+    def get_text(self):
+        if hasattr(self, "text"):
+            return self.text()
+        return ""
+
+    def set_readonly(self, arg):
+        if hasattr(self, "setReadOnly"):
+            self.setReadOnly(True if arg else False)
+
+    def is_enabled(self):
+        return self.isEnabled()
+
+    def set_visible(self, arg=True):
+        self.setVisible(arg)
+
+    def is_visible(self):
+        if hasattr(self, "isVisible"):
+            return self.isVisible()
+
+    def is_readonly(self):
+        if hasattr(self, "isReadOnly"):
+            return self.isReadOnly()
+
+    def set_font(self, font_name="", font_size=12):
+        self.setFont(QFont(font_name, font_size))
+
+    def set_focus(self):
+        self.setFocus()
+
+    def has_focus(self):
+        return self.hasFocus()
+
+    def set_maximum_width(self, width, char="O"):
+        if self.meta.get("control", "") not in ("radio", "check"):
+            if char != "":
+                # self.setMaximumWidth(QFontMetrics(self.font()).width(char) * width)
+                self.setMaximumWidth(int(QFontMetrics(self.font()).horizontalAdvance(char) * width))
+            else:
+                self.setMaximumWidth(int(width))
+
+    def set_fixed_width(self, width, char="O"):
+        if self.meta.get("control", "") not in ("radio", "check"):
+            if char != "":
+                self.setFixedWidth(int(QFontMetrics(self.font()).horizontalAdvance(char) * width))
+            else:
+                self.setFixedWidth(int(width))
+
+    def set_fixed_height(self, width, char="O"):
+        if self.meta.get("control", "") not in ("radio", "check"):
+            if char != "":
+                self.setFixedHeight(int(QFontMetrics(self.font()).height() * width))
+            else:
+                self.setFixedHeight(int(width))
+
+    def set_maximum_len(self, length):
+        if hasattr(self, "setMaxLength"):
+            return self.setMaxLength(int(length))
+
+    def set_alignment(self, alignment):
+        if hasattr(self, "setAlignment"):
+            self.setAlignment(q2_align[f"{alignment}"])
+
+    # def valid(self):
+    #     if self.meta.get("valid"):
+    #         return self.meta.get("valid", lambda: True)()
+    #     else:
+    #         return True
+
+    # def when(self):
+    #     if self.meta.get("when"):
+    #         return self.meta.get("when", lambda: True)()
+    #     else:
+    #         return True
+
+    def set_style_sheet(self, css: str):
+        super().set_style_sheet(css)
+        self.setStyleSheet(self.style_sheet)
+
+    def add_style_sheet(self, css: str):
+        last_style = " ".join([self.styleSheet(), f"; {css}"])
+        super().set_style_sheet(last_style)
+        self.setStyleSheet(last_style)
+
+    def get_style_sheet(self):
+        return self.styleSheet()
+
+    # def fix_default_height(self):
+    #     self.set_maximum_height(self.get_default_height())
+
+    def get_default_height(self):
+        return self.sizeHint().height()
+
+    def set_maximum_height(self, height):
+        self.setMaximumHeight(int(height))
+
+    # def fix_default_width(self):
+    #     self.set_maximum_width(self.get_default_width())
+
+    def get_default_width(self):
+        return self.sizeHint().width()
+
+    def set_size_policy(self, horizontal, vertical):
+        sp = {
+            "fixed": QSizePolicy.Policy.Fixed,
+            "minimum": QSizePolicy.Policy.Minimum,
+            "maximum": QSizePolicy.Policy.Maximum,
+            "preffered": QSizePolicy.Policy.Preferred,
+            "expanding": QSizePolicy.Policy.Expanding,
+            "minimalexpanding": QSizePolicy.Policy.MinimumExpanding,
+            "ignored": QSizePolicy.Policy.Ignored,
+        }
+
+        self.setSizePolicy(
+            sp.get(horizontal, QSizePolicy.Policy.Minimum), sp.get(vertical, QSizePolicy.Policy.Minimum)
+        )
+
+    def set_content_margins(self, top=0, right=None, bottom=None, left=None):
+        if right is None:
+            right = top
+        if bottom is None:
+            bottom = top
+        if left is None:
+            left = right
+        self.setContentsMargins(top, right, bottom, left)
+
+    def get_next_focus_widget(self, pos=1):
+        return self.nextInFocusChain()
+
+    def get_next_widget(self, pos=1):
+        return self.layout().widget()
+
+    def add_widget_above(self, widget, pos=0):
+        my_pos = self.parentWidget().layout().indexOf(self)
+        self.parent().layout().insertWidget(my_pos - pos, widget)
+
+    def add_widget_below(self, widget, pos=0):
+        if pos == -1:
+            self.parent().layout().addWidget(widget)
+        else:
+            my_pos = self.parentWidget().layout().indexOf(self)
+            self.parent().layout().insertWidget(my_pos + pos + 1, widget)
+
+    def remove(self):
+        self.parentWidget().layout().removeWidget(self)
+        self.setParent(None)
+
+    def get_layout_position(self):
+        return self.parentWidget().layout().indexOf(self)
+
+    def get_layout_count(self):
+        return self.parentWidget().layout().count()
+
+    def get_layout_widget(self, pos):
+        return self.parentWidget().layout().itemAt(pos).widget()
+
+    def get_layout_widgets(self):
+        return [self.get_layout_widget(x) for x in range(self.get_layout_count())]
+
+    def move_up(self):
+        pos = self.get_layout_position()
+        if pos > 0:
+            w = self.parentWidget().layout().takeAt(pos).widget()
+            self.parentWidget().layout().insertWidget(pos - 1, w)
+
+    def move_down(self):
+        pos = self.get_layout_position()
+        if pos < self.get_layout_count() - 1:
+            w = self.parentWidget().layout().takeAt(pos + 1).widget()
+            self.parentWidget().layout().insertWidget(pos, w)
+
+    def action_set_visible(self, text, mode=True):
+        for action in self.actions():
+            if action.text().strip() == text:
+                action.setVisible(mode)
+
+    def action_set_enabled(self, text, mode=True):
+        for action in self.actions():
+            if action.text().strip() == text:
+                action.setVisible(mode)
```

### Comparing `q2gui-0.1.9/q2gui/pyqt6/q2window.py` & `q2gui-0.1.90/q2gui/pyqt6/q2window.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,129 +1,130 @@
-if __name__ == "__main__":
-    import sys
-
-    sys.path.insert(0, ".")
-
-    from demo.demo import demo
-
-    demo()
-
-from PyQt6.QtWidgets import QWidget, QHBoxLayout, QVBoxLayout, QFormLayout, QGridLayout, QApplication
-from PyQt6.QtGui import QScreen
-
-from PyQt6.QtCore import Qt
-
-from q2gui import q2window
-from q2gui.q2utils import int_
-
-q2_align = {
-    "": Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignTop,
-    "-1": Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignTop,
-    "0": Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignTop,
-    "1": Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignBottom,
-    "2": Qt.AlignmentFlag.AlignHCenter | Qt.AlignmentFlag.AlignBottom,
-    "3": Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignBottom,
-    "4": Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignVCenter,
-    "5": Qt.AlignmentFlag.AlignHCenter | Qt.AlignmentFlag.AlignVCenter,
-    "6": Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignVCenter,
-    "7": Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignTop,
-    "8": Qt.AlignmentFlag.AlignHCenter | Qt.AlignmentFlag.AlignTop,
-    "9": Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignTop,
-}
-
-
-def layout(arg="h"):
-    if arg.lower().startswith("v"):
-        layout = QVBoxLayout()
-        layout.setAlignment(q2_align["7"])
-    elif arg.lower().startswith("f"):
-        layout = QFormLayout()
-        layout.setLabelAlignment(q2_align["6"])
-        layout.layout().setSpacing(2)
-    elif arg.lower().startswith("g"):
-        layout = QGridLayout()
-    else:
-        layout = QHBoxLayout()
-        layout.setAlignment(q2_align["7"])
-    layout.layout().setContentsMargins(0, 0, 0, 0)
-    return layout
-
-
-class Q2Frame(q2window.Q2Frame, QWidget):
-    def set_mode(self, mode="v"):
-        self.splitter = None
-        super().set_mode(mode=mode)
-        if self.layout() is not None:
-            return
-        self.setLayout(layout(mode))
-
-    def insert_widget(self, pos=None, widget=None):
-        # if widget:
-        #     # widget.setContentsMargins(0,20, 0, 0)
-        #     if widget.label:
-        #         print("--",widget, widget.label.get_text())
-        self.layout().addWidget(widget)
-        self.updateGeometry()
-
-    def add_row(self, label=None, widget=None):
-        # if widget:
-        #     widget.setContentsMargins(0, 0, 0, 0)
-        #     print("f", widget, widget.label.get_text())
-        self.layout().addRow(label, widget)
-        self.updateGeometry()
-
-
-class Q2QtWindow(q2window.Q2Window, Q2Frame):
-    def __init__(self, title=""):
-        super().__init__()
-        self.set_title(title)
-
-    def set_position(self, left, top):
-        if left == -9999 and top == -9999:
-            self.center_position()
-        else:
-            self.move(left, top)
-
-    def center_position(self):
-        # sw, sh = (Q_DesktopWidget().size().width(), Q_DesktopWidget().size().height())
-        screen = QApplication.screens()[0]
-
-        sw, sh = (screen.size().width(), screen.size().height())
-
-        ww, wh = self.get_size()
-
-        left = (sw - ww) / 2
-        top = (sh - wh) / 2
-        self.move(left, top)
-
-    def set_size(self, width, height):
-        self.resize(int(width), int(height))
-
-    def get_position(self):
-        return (self.pos().x(), self.pos().y())
-
-    def get_size(self):
-        if hasattr(self, "parent") and self.parent() is not None:
-            return (self.parent().size().width(), self.parent().size().height())
-        else:
-            return (self.size().width(), self.size().height())
-
-    def set_disabled(self, arg=True):
-        self.setEnabled(True if not arg else False)
-
-    def set_enabled(self, arg=True):
-        self.setEnabled(True if arg else False)
-
-    def set_title(self, title):
-        super().set_title(title)
-        QWidget.setWindowTitle(self, title)
-
-    def hide_border(self):
-        super().hide_border()
-        self.setObjectName("grb")
-        self.setStyleSheet("QGroupBox#grb {border:0}")
-
-    def is_maximized(self):
-        return 1 if QWidget.isMaximized(self) else 0
-
-    def show_maximized(self):
-        QWidget.showMaximized(self)
+if __name__ == "__main__":
+    import sys
+
+    sys.path.insert(0, ".")
+
+    from demo.demo import demo
+
+    demo()
+
+
+from PyQt6.QtWidgets import QWidget, QHBoxLayout, QVBoxLayout, QFormLayout, QGridLayout, QApplication
+from PyQt6.QtCore import Qt
+from q2gui import q2window
+
+
+q2_align = {
+    "": Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignTop,
+    "-1": Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignTop,
+    "0": Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignTop,
+    "1": Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignBottom,
+    "2": Qt.AlignmentFlag.AlignHCenter | Qt.AlignmentFlag.AlignBottom,
+    "3": Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignBottom,
+    "4": Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignVCenter,
+    "5": Qt.AlignmentFlag.AlignHCenter | Qt.AlignmentFlag.AlignVCenter,
+    "6": Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignVCenter,
+    "7": Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignTop,
+    "8": Qt.AlignmentFlag.AlignHCenter | Qt.AlignmentFlag.AlignTop,
+    "9": Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignTop,
+}
+
+
+def layout(arg="h"):
+    if arg.lower().startswith("v"):
+        layout = QVBoxLayout()
+        layout.setAlignment(q2_align["7"])
+    elif arg.lower().startswith("f"):
+        layout = QFormLayout()
+        layout.setLabelAlignment(q2_align["6"])
+        layout.layout().setSpacing(2)
+    elif arg.lower().startswith("g"):
+        layout = QGridLayout()
+    else:
+        layout = QHBoxLayout()
+        layout.setAlignment(q2_align["7"])
+    layout.layout().setContentsMargins(0, 0, 0, 0)
+    # layout.layout().setContentsMargins(3, 3, 3, 3)
+    return layout
+
+
+class Q2Frame(q2window.Q2Frame, QWidget):
+    def set_mode(self, mode="v"):
+        self.splitter = None
+        super().set_mode(mode=mode)
+        self.set_title("Output")
+        if self.layout() is not None:
+            return
+        self.setLayout(layout(mode))
+
+    def insert_widget(self, pos=None, widget=None):
+        # if widget:
+        #     # widget.setContentsMargins(0,20, 0, 0)
+        #     if widget.label:
+        #         print("--",widget, widget.label.get_text())
+        self.layout().addWidget(widget)
+        self.updateGeometry()
+
+    def add_row(self, label=None, widget=None):
+        # if widget:
+        #     widget.setContentsMargins(0, 0, 0, 0)
+        #     print("f", widget, widget.label.get_text())
+        self.layout().addRow(label, widget)
+        self.updateGeometry()
+
+
+class Q2QtWindow(q2window.Q2Window, Q2Frame):
+    def __init__(self, title=""):
+        super().__init__()
+        self.set_title(title)
+
+    def set_position(self, left, top):
+        if left == -9999 and top == -9999:
+            self.center_position()
+        else:
+            self.move(int(left), int(top))
+
+    def center_position(self):
+        # sw, sh = (Q_DesktopWidget().size().width(), Q_DesktopWidget().size().height())
+        screen = QApplication.screens()[0]
+
+        sw, sh = (screen.size().width(), screen.size().height())
+
+        ww, wh = self.get_size()
+
+        left = int((sw - ww) / 2)
+        top = int((sh - wh) / 2)
+        self.move(left, top)
+
+    def set_size(self, width, height):
+        self.resize(int(width), int(height))
+
+    def get_position(self):
+        return (self.pos().x(), self.pos().y())
+
+    def get_size(self):
+        if hasattr(self, "parent") and self.parent() is not None:
+            return (self.parent().size().width(), self.parent().size().height())
+        else:
+            return (self.size().width(), self.size().height())
+
+    def set_disabled(self, arg=True):
+        self.setEnabled(True if not arg else False)
+
+    def set_enabled(self, arg=True):
+        self.setEnabled(True if arg else False)
+
+    def set_title(self, title):
+        super().set_title(title)
+        QWidget.setWindowTitle(self, title)
+
+    def hide_border(self):
+        super().hide_border()
+        self.setObjectName("grb")
+        # self.setStyleSheet("QGroupBox#grb {border:0}")
+        self.parent().setWindowFlags(Qt.WindowType.CustomizeWindowHint | Qt.WindowType.FramelessWindowHint)
+
+    def is_maximized(self):
+        return 1 if QWidget.isMaximized(self) else 0
+
+    def show_maximized(self):
+        QWidget.showMaximized(self)
```

### Comparing `q2gui-0.1.9/q2gui/pyqt6/widgets/q2check.py` & `q2gui-0.1.90/q2gui/pyqt6/widgets/q2check.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import sys
-
-if __name__ == "__main__":
-
-    sys.path.insert(0, ".")
-
-    from demo.demo import demo
-
-    demo()
-
-from PyQt6.QtWidgets import QCheckBox, QSizePolicy
-
-from q2gui.pyqt6.q2widget import Q2Widget
-from q2gui.q2utils import int_
-
-
-class q2check(QCheckBox, Q2Widget):
-    def __init__(self, meta):
-        super().__init__(meta)
-        if meta.get("pic"):
-            self.setText(meta.get("pic"))
-        else:
-            self.setText(meta.get("label", ""))
-        self.managed_widgets = []
-        self.setSizePolicy(QSizePolicy.Policy.Maximum, QSizePolicy.Policy.Maximum)
-        self.stateChanged.connect(self.state_changed)
-
-    def state_changed(self):
-        for x in self.managed_widgets:
-            x.set_enabled(self.isChecked())
-            if x.is_enabled() and self.hasFocus():
-                x.set_focus()
-            if self.isChecked():
-                if x.meta.get("when"):
-                    x.meta.get("when")()
-            else:
-                if x.meta.get("valid"):
-                    x.meta.get("valid")()
-        self.valid()
-
-    def add_managed_widget(self, widget):
-        self.managed_widgets.append(widget)
-        widget.check = self
-
-    def remove_managed_widget(self, widget):
-        if widget in self.managed_widgets:
-            self.managed_widgets.pop(self.managed_widgets.index(widget))
-
-    def set_text(self, text):
-        if self.meta.get("num"):
-            self.setChecked(True if int_(text) else False)
-        else:
-            self.setChecked(True if text else False)
-
-    def set_title(self, title):
-        self.setText(title)
-
-    def get_text(self):
-        if self.meta.get("num"):
-            return 1 if self.isChecked() else 0
-        else:
-            return "*" if self.isChecked() else ""
-
-    def set_checked(self, mode=True):
-        self.set_text(mode)
-
-    def is_checked(self):
-        return True if self.get_text() else False
+import sys
+
+if __name__ == "__main__":
+
+    sys.path.insert(0, ".")
+
+    from demo.demo import demo
+
+    demo()
+
+from PyQt6.QtWidgets import QCheckBox, QSizePolicy
+
+from q2gui.pyqt6.q2widget import Q2Widget
+from q2gui.q2utils import int_
+
+
+class q2check(QCheckBox, Q2Widget):
+    def __init__(self, meta):
+        super().__init__(meta)
+        if meta.get("pic"):
+            self.setText(meta.get("pic"))
+        else:
+            self.setText(meta.get("label", ""))
+        self.managed_widgets = []
+        self.setSizePolicy(QSizePolicy.Policy.Maximum, QSizePolicy.Policy.Maximum)
+        self.stateChanged.connect(self.state_changed)
+
+    def state_changed(self):
+        for x in self.managed_widgets:
+            x.set_enabled(self.isChecked())
+            if x.is_enabled() and self.hasFocus():
+                x.set_focus()
+            if self.isChecked():
+                if x.meta.get("when"):
+                    x.meta.get("when")()
+            else:
+                if x.meta.get("valid"):
+                    x.meta.get("valid")()
+        self.valid()
+
+    def add_managed_widget(self, widget):
+        self.managed_widgets.append(widget)
+        widget.check = self
+
+    def remove_managed_widget(self, widget):
+        if widget in self.managed_widgets:
+            self.managed_widgets.pop(self.managed_widgets.index(widget))
+
+    def set_text(self, text):
+        if self.meta.get("num"):
+            self.setChecked(True if int_(text) else False)
+        else:
+            self.setChecked(True if text else False)
+
+    def set_title(self, title):
+        self.setText(title)
+
+    def get_text(self):
+        if self.meta.get("num"):
+            return 1 if self.isChecked() else 0
+        else:
+            return "*" if self.isChecked() else ""
+
+    def set_checked(self, mode=True):
+        self.set_text(mode)
+
+    def is_checked(self):
+        return True if self.get_text() else False
```

### Comparing `q2gui-0.1.9/q2gui/pyqt6/widgets/q2frame.py` & `q2gui-0.1.90/q2gui/pyqt6/widgets/q2frame.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,96 @@
-if __name__ == "__main__":
-
-    import sys
-
-    sys.path.insert(0, ".")
-
-    from demo.demo import demo
-
-    demo()
-
-from PyQt6.QtWidgets import QGroupBox, QSplitter, QSizePolicy
-from PyQt6.QtCore import Qt
-
-
-from q2gui.pyqt6.q2window import Q2Frame
-from q2gui.pyqt6.q2widget import Q2Widget
-
-
-class q2frame(QGroupBox, Q2Widget, Q2Frame):
-    def __init__(self, meta):
-        super().__init__(meta)
-        Q2Frame.__init__(self, meta.get("column", "/v")[1])
-        self.meta = meta
-        self.splitter = None
-        self.scroller = None
-        if meta.get("column", "")[2:3] == "s":  # Splitter!
-            self.splitter = q2splitter()
-            if meta.get("column").startswith("/v"):
-                self.splitter.setOrientation(Qt.Orientation.Vertical)
-            self.layout().addWidget(self.splitter)
-        if meta.get("label") not in ("", "-") and not meta.get("check"):
-            self.set_title(meta.get("label"))
-        if meta.get("label", "") == "":
-            self.hide_border()
-
-    def hide_border(self):
-        self.setObjectName("grb")
-        no_border_style = "QGroupBox#grb {border:0}"
-        last_style = self.styleSheet()
-        self.set_title("")
-        if no_border_style not in last_style:
-            self.setStyleSheet(last_style + " " + no_border_style)
-
-    def set_title(self, title):
-        self.setTitle(title)
-
-    def get_widget_count(self):
-        return self.layout().count()
-
-    def add_widget(self, widget=None, label=None):
-        if self.splitter is not None:
-            self.splitter.addWidget(widget)
-            if hasattr(widget, "meta"):
-                self.splitter.setStretchFactor(self.splitter.count() - 1, widget.meta.get("stretch", 0))
-        else:
-            return super().add_widget(widget=widget, label=label)
-
-
-class q2splitter(QSplitter):
-    def __init__(self):
-        super().__init__()
-        self.setSizePolicy(QSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding))
-
-    def get_sizes(self):
-        return ",".join([f"{x}" for x in self.sizes()])
-
-    def set_sizes(self, sizes):
-        if sizes == "":
-            init_sizes = [self.widget(x).meta.get("stretch", 1) for x in range(self.count())]
-            if sum(init_sizes):
-                widget_size = (
-                    self.width() if self.orientation() is Qt.Orientation.Horizontal else self.height()
-                )
-                init_sizes = [str(int(x * widget_size / sum(init_sizes))) for x in init_sizes]
-                for x in range(self.count()):
-                    widgget = self.widget(x)
-                    if widgget.meta.get("control") == "toolbar":
-                        init_sizes[x] = str(widgget.sizeHint().height())
-                sizes = ",".join(init_sizes)
-        if sizes:
-            sizes = [int(x) for x in sizes.split(",")]
-            self.setSizes(sizes)
+if __name__ == "__main__":
+
+    import sys
+
+    sys.path.insert(0, ".")
+
+    from demo.demo import demo
+
+    demo()
+
+from PyQt6.QtWidgets import QGroupBox, QSplitter, QSizePolicy
+from PyQt6.QtCore import Qt
+from PyQt6.QtCore import QSize
+
+
+from q2gui.pyqt6.q2window import Q2Frame
+from q2gui.pyqt6.q2widget import Q2Widget
+
+
+class q2frame(QGroupBox, Q2Widget, Q2Frame):
+    def __init__(self, meta):
+        super().__init__(meta)
+        Q2Frame.__init__(self, meta.get("column", "/v")[1])
+        self.meta = meta
+        self.splitter = None
+        self.scroller = None
+        if meta.get("column", "")[2:3] == "s":  # Splitter!
+            self.splitter = q2splitter()
+            if meta.get("column").startswith("/v"):
+                self.splitter.setOrientation(Qt.Orientation.Vertical)
+            self.layout().addWidget(self.splitter)
+        if meta.get("label") not in ("", "-") and not meta.get("check"):
+            self.set_title(meta.get("label"))
+            self.setObjectName("title")
+        if meta.get("label", "") == "":
+            self.hide_border()
+
+    def hide_border(self):
+        self.setObjectName("grb")
+        # self.add_style_sheet("{border:0}")
+        # self.add_style_sheet("QGroupBox#grb {border:0}")
+        no_border_style = " QGroupBox#grb {border:0} "
+        last_style = self.styleSheet()
+        self.set_title("")
+        if no_border_style not in last_style:
+            self.setStyleSheet(last_style + " " + no_border_style)
+
+    def set_title(self, title):
+        self.setTitle(title)
+
+    def get_widget_count(self):
+        return self.layout().count()
+
+    def add_widget(self, widget=None, label=None):
+        if self.splitter is not None:
+            self.splitter.addWidget(widget)
+            if hasattr(widget, "meta"):
+                self.splitter.setStretchFactor(self.splitter.count() - 1, widget.meta.get("stretch", 0))
+        else:
+            return super().add_widget(widget=widget, label=label)
+
+
+class q2splitter(QSplitter):
+    def __init__(self):
+        super().__init__()
+        # self.setSizePolicy(QSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding))
+
+    def get_sizes(self):
+        return ",".join([f"{x}" for x in self.sizes()])
+
+    def set_sizes(self, sizes):
+        if sizes == "":
+            init_sizes = [self.widget(x).meta.get("stretch", 1) for x in range(self.count())]
+            if sum(init_sizes):
+                widget_size = (
+                    self.width() if self.orientation() is Qt.Orientation.Horizontal else self.height()
+                )
+                init_sizes = [str(int(x * widget_size / sum(init_sizes))) for x in init_sizes]
+                for x in range(self.count()):
+                    widgget = self.widget(x)
+                    if widgget.meta.get("control") == "toolbar":
+                        init_sizes[x] = str(widgget.sizeHint().height())
+                sizes = ",".join(init_sizes)
+        if sizes:
+            sizes = [int(x) for x in sizes.split(",")]
+            self.setSizes(sizes)
+
+    def showEvent(self, ev):
+        self.updateGeometry()
+        return super().showEvent(ev)
+
+    def sizeHint(self):
+        if self.isVisible():
+            return QSize(99999, 99999)
+        else:
+            return super().sizeHint()
```

### Comparing `q2gui-0.1.9/q2gui/pyqt6/widgets/q2label.py` & `q2gui-0.1.90/q2gui/pyqt6/widgets/q2label.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import sys
-
-if __name__ == "__main__":
-
-    sys.path.insert(0, ".")
-
-    from demo.demo import demo
-
-    demo()
-
-from PyQt6.QtWidgets import QLabel
-from PyQt6.QtCore import Qt
-
-from q2gui.pyqt6.q2widget import Q2Widget
-
-vertical_align_dict = {
-    "top": Qt.AlignmentFlag.AlignTop,
-    "middle": Qt.AlignmentFlag.AlignVCenter,
-    "bottom": Qt.AlignmentFlag.AlignBottom,
-}
-
-horizontal_align_dict = {
-    "left": Qt.AlignmentFlag.AlignLeft,
-    "center": Qt.AlignmentFlag.AlignHCenter,
-    "justify": Qt.AlignmentFlag.AlignJustify,
-    "right": Qt.AlignmentFlag.AlignRight,
-}
-
-
-class q2label(QLabel, Q2Widget):
-    def __init__(self, meta={}):
-        super().__init__({"label": meta.get("label", ""), "dblclick": meta.get("dblclick")})
-        # super().__init__(meta)
-        self.set_text(self.meta["label"])
-        self.setWordWrap(True)
-        self.set_maximum_height(self.get_default_height() * 1.5)
-
-    def set_style_sheet(self, style_text):
-        super().set_style_sheet(style_text)
-
-        if "vertical-align" in style_text or "text-align" in style_text:
-            if isinstance(style_text, str):
-                style_dict = {
-                    x[0].strip().replace("{", ""): x[1].strip().replace("}", "")
-                    for x in [x.split(":") for x in style_text.split(";") if ":" in x]
-                }
-            else:
-                style_dict = style_text
-            CA = vertical_align_dict.get(style_dict.get("vertical-align", "top"), Qt.AlignmentFlag.AlignTop)
-            CA |= horizontal_align_dict.get(style_dict.get("text-align", "left"), Qt.AlignmentFlag.AlignLeft)
-
-            self.setAlignment(CA)
+import sys
+
+if __name__ == "__main__":
+
+    sys.path.insert(0, ".")
+
+    from demo.demo import demo
+
+    demo()
+
+from PyQt6.QtWidgets import QLabel
+from PyQt6.QtCore import Qt
+
+from q2gui.pyqt6.q2widget import Q2Widget
+
+vertical_align_dict = {
+    "top": Qt.AlignmentFlag.AlignTop,
+    "middle": Qt.AlignmentFlag.AlignVCenter,
+    "bottom": Qt.AlignmentFlag.AlignBottom,
+}
+
+horizontal_align_dict = {
+    "left": Qt.AlignmentFlag.AlignLeft,
+    "center": Qt.AlignmentFlag.AlignHCenter,
+    "justify": Qt.AlignmentFlag.AlignJustify,
+    "right": Qt.AlignmentFlag.AlignRight,
+}
+
+
+class q2label(QLabel, Q2Widget):
+    def __init__(self, meta={}):
+        super().__init__({"label": meta.get("label", ""), "dblclick": meta.get("dblclick")})
+        # super().__init__(meta)
+        self.set_text(self.meta["label"])
+        self.setWordWrap(True)
+        self.set_maximum_height(int(self.get_default_height() * 1.5))
+
+    def set_style_sheet(self, style_text):
+        super().set_style_sheet(style_text)
+
+        if "vertical-align" in style_text or "text-align" in style_text:
+            if isinstance(style_text, str):
+                style_dict = {
+                    x[0].strip().replace("{", ""): x[1].strip().replace("}", "")
+                    for x in [x.split(":") for x in style_text.split(";") if ":" in x]
+                }
+            else:
+                style_dict = style_text
+            CA = vertical_align_dict.get(style_dict.get("vertical-align", "top"), Qt.AlignmentFlag.AlignTop)
+            CA |= horizontal_align_dict.get(style_dict.get("text-align", "left"), Qt.AlignmentFlag.AlignLeft)
+
+            self.setAlignment(CA)
```

### Comparing `q2gui-0.1.9/q2gui/pyqt6/widgets/q2line.py` & `q2gui-0.1.90/q2gui/pyqt6/widgets/q2line.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,115 +1,116 @@
-import sys
-
-if __name__ == "__main__":
-
-    sys.path.insert(0, ".")
-
-    from demo.demo import demo
-
-    demo()
-
-from PyQt6.QtWidgets import QLineEdit
-
-from q2gui.pyqt6.q2widget import Q2Widget
-from q2gui.q2utils import int_, num
-from q2gui import q2app
-
-
-class q2line(QLineEdit, Q2Widget):
-    def __init__(self, meta):
-        super().__init__(meta)
-        self.last_text_len = 0
-        self.last_cur_pos = 0
-        # if self.meta.get("pic"):
-        self.TS = " "  # thousands separator
-        self.DS = "."  # decimal separator
-
-        if self.meta.get("num"):
-            self.declen = int_(self.meta.get("datadec", 0))
-            if self.meta.get("pic") == "F":  # financial
-                self.formatstring = q2app.FINANCIAL_FORMAT % self.declen
-            else:
-                self.formatstring = "{:.%sf}" % self.declen
-            self.textChanged.connect(self.format_decimal)
-            self.cursorPositionChanged.connect(self.track_cursor)
-            self.textChanged.emit("")
-
-    def track_cursor(self, old, new):
-        self.last_cur_pos = new
-
-    def get_text(self):
-        if self.meta.get("num"):
-            return self.text().replace(self.TS, "")
-        else:
-            return super().get_text()
-
-    def format_decimal(self):
-        text = self.text()
-
-        self.blockSignals(True)
-        cursor_pos = self.cursorPosition()
-        cursor_pos_right = len(text) - cursor_pos
-
-        negative = text.count("-") == 1 and text.count("+") == 0
-        # divide text by cursor pos
-        right_text = text[cursor_pos:]
-        left_text = text[:-cursor_pos_right] if cursor_pos_right else text
-
-        if left_text.endswith(","):  # replace comma with point
-            left_text = left_text[:-1] + self.DS
-
-        # TS removed
-        if left_text and len(text) < self.last_text_len and len(right_text) > 3:
-            if (
-                right_text[3] in [self.TS, self.DS]
-                and left_text[-1] != self.TS
-                and cursor_pos - self.last_cur_pos < 0
-            ):
-                left_text = left_text[:-1]  # remove TS
-        # remove non-digit chars and change cursor position
-        left_text = "".join([x for x in left_text if x in "0123456789., "])
-        text = left_text + right_text
-
-        if self.declen == 0:
-            text = text.replace(".", "")
-        else:  # for decimal only
-            if self.DS not in text:
-                text += "."
-                cursor_pos_right = self.declen
-
-            if text == "":  # empty text - just 0
-                text = "0." + "0" * self.declen
-            elif text.count(self.DS) == 0:  # DS deleted
-                text = text[:-2] + self.DS + text[-2:]
-            elif text.count(self.DS) > 1:  # entered decimal_separator - move cursor postion
-                text = left_text[:-1] + right_text
-                if "." in right_text:  # added DS left from DS
-                    cursor_pos_right = self.declen
-                else:
-                    cursor_pos_right = self.declen + 1
-            else:
-                spl = text.split(self.DS)
-                if cursor_pos_right <= self.declen:  # cursor in decimal part
-                    if len(spl[1]) < self.declen:  # deleted from decimal part
-                        text += "0"
-                        cursor_pos_right += 1
-                    elif len(spl[1]) > self.declen:  # decimal part entered
-                        text = text[: -(len(spl[1]) - self.declen)]
-                        cursor_pos_right -= 1
-                else:  # cursor left of DS
-                    if len(spl[0]) == 2 and spl[0][-1] == "0":
-                        # 0 only was left from DS-cut 0
-                        text = spl[0][:-1] + self.DS + spl[1]
-                        cursor_pos_right -= 1
-
-        text = self.formatstring.format(num(text.replace(self.TS, ""))).replace(",", self.TS)
-        cursor_pos = len(text) - cursor_pos_right
-        if negative:
-            text = f"-{text}"
-            cursor_pos += 1
-
-        self.setText(text)
-        self.setCursorPosition(cursor_pos)
-        self.last_text_len = len(text)
-        self.last_cur_pos = cursor_pos
-        self.blockSignals(False)
+import sys
+
+if __name__ == "__main__":
+
+    sys.path.insert(0, ".")
+
+    from demo.demo import demo
+
+    demo()
+
+from PyQt6.QtWidgets import QLineEdit
+
+from q2gui.pyqt6.q2widget import Q2Widget
+from q2gui.q2utils import int_, num
+from q2gui import q2app
+
+
+class q2line(QLineEdit, Q2Widget):
+    def __init__(self, meta):
+        super().__init__(meta)
+        self.last_text_len = 0
+        self.last_cur_pos = 0
+        if self.meta.get("pic") == "*":
+            self.setEchoMode(self.EchoMode.Password)
+        self.TS = " "  # thousands separator
+        self.DS = "."  # decimal separator
+
+        if self.meta.get("num"):
+            self.declen = int_(self.meta.get("datadec", 0))
+            if self.meta.get("pic") == "F":  # financial
+                self.formatstring = q2app.FINANCIAL_FORMAT % self.declen
+            else:
+                self.formatstring = "{:.%sf}" % self.declen
+            self.textChanged.connect(self.format_decimal)
+            self.cursorPositionChanged.connect(self.track_cursor)
+            self.textChanged.emit("")
+
+    def track_cursor(self, old, new):
+        self.last_cur_pos = new
+
+    def get_text(self):
+        if self.meta.get("num"):
+            return self.text().replace(self.TS, "")
+        else:
+            return super().get_text()
+
+    def format_decimal(self):
+        text = self.text()
+
+        self.blockSignals(True)
+        cursor_pos = self.cursorPosition()
+        cursor_pos_right = len(text) - cursor_pos
+
+        negative = text.count("-") == 1 and text.count("+") == 0
+        # divide text by cursor pos
+        right_text = text[cursor_pos:]
+        left_text = text[:-cursor_pos_right] if cursor_pos_right else text
+
+        if left_text.endswith(","):  # replace comma with point
+            left_text = left_text[:-1] + self.DS
+
+        # TS removed
+        if left_text and len(text) < self.last_text_len and len(right_text) > 3:
+            if (
+                right_text[3] in [self.TS, self.DS]
+                and left_text[-1] != self.TS
+                and cursor_pos - self.last_cur_pos < 0
+            ):
+                left_text = left_text[:-1]  # remove TS
+        # remove non-digit chars and change cursor position
+        left_text = "".join([x for x in left_text if x in "0123456789., "])
+        text = left_text + right_text
+
+        if self.declen == 0:
+            text = text.replace(".", "")
+        else:  # for decimal only
+            if self.DS not in text:
+                text += "."
+                cursor_pos_right = self.declen
+
+            if text == "":  # empty text - just 0
+                text = "0." + "0" * self.declen
+            elif text.count(self.DS) == 0:  # DS deleted
+                text = text[:-2] + self.DS + text[-2:]
+            elif text.count(self.DS) > 1:  # entered decimal_separator - move cursor postion
+                text = left_text[:-1] + right_text
+                if "." in right_text:  # added DS left from DS
+                    cursor_pos_right = self.declen
+                else:
+                    cursor_pos_right = self.declen + 1
+            else:
+                spl = text.split(self.DS)
+                if cursor_pos_right <= self.declen:  # cursor in decimal part
+                    if len(spl[1]) < self.declen:  # deleted from decimal part
+                        text += "0"
+                        cursor_pos_right += 1
+                    elif len(spl[1]) > self.declen:  # decimal part entered
+                        text = text[: -(len(spl[1]) - self.declen)]
+                        cursor_pos_right -= 1
+                else:  # cursor left of DS
+                    if len(spl[0]) == 1 and spl[0][-1] == "0":
+                        # 0 only was left from DS-cut 0
+                        text = spl[0][:-1] + self.DS + spl[1]
+                        cursor_pos_right -= 1
+
+        text = self.formatstring.format(num(text.replace(self.TS, ""))).replace(",", self.TS)
+        cursor_pos = len(text) - cursor_pos_right
+        if negative:
+            text = f"-{text}"
+            cursor_pos += 1
+
+        self.setText(text)
+        self.setCursorPosition(cursor_pos)
+        self.last_text_len = len(text)
+        self.last_cur_pos = cursor_pos
+        self.blockSignals(False)
```

### Comparing `q2gui-0.1.9/q2gui/pyqt6/widgets/q2lookup.py` & `q2gui-0.1.90/q2gui/pyqt6/widgets/q2lookup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,90 @@
-import sys
-
-if __name__ == "__main__":
-
-    sys.path.insert(0, ".")
-
-    from demo.demo import demo
-
-    demo()
-
-
-from PyQt6.QtWidgets import (
-    QVBoxLayout,
-    QWidget,
-)
-from PyQt6.QtGui import QKeyEvent
-
-from PyQt6.QtCore import Qt, QTimer
-
-from q2gui.pyqt6.widgets.q2line import q2line
-from q2gui.pyqt6.widgets.q2list import q2list
-
-
-class q2lookup(QWidget):
-    def __init__(self, parent, text):
-        super().__init__(parent, Qt.WindowType.Popup)
-        self.setLayout(QVBoxLayout())
-        self.layout().setContentsMargins(0, 0, 0, 0)
-        self.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
-        self.lookup_edit = q2line({})
-        self.lookup_list = q2list({})
-        self.layout().addWidget(self.lookup_edit)
-        self.layout().addWidget(self.lookup_list)
-        self.lookup_edit.set_text("" if text == "*" else text)
-        self.lookup_edit.setFocus()
-
-        self.timer = QTimer()
-        self.timer.setSingleShot(True)
-        self.timer.setInterval(500)
-        self.timer.timeout.connect(self.lookup_search)
-
-        self.lookup_edit.textChanged.connect(self.lookup_text_changed)
-        self.lookup_edit.returnPressed.connect(self.lookup_edit_return_pressed)
-
-        self.lookup_list.itemActivated.connect(self.lookup_list_selected)
-
-        self.set_geometry()
-
-    def lookup_list_selected(self):
-        print("Method lookup_list_selected has to be implemented...")
-
-    def set_geometry(self):
-        print("Method set_geometry has to be implemented...")
-
-    # def show(self, column):
-    #     self.q2_model_column = column
-    #     return super().show()
-
-    def lookup_list_selected(self):
-        print(self.lookup_list.currentItem().text())
-        self.close()
-
-    def lookup_search(self):
-        self.lookup_list.clear()
-        for x in range(6):
-            self.lookup_list.addItem(f"{x} Method lookup_search has to be implemented...")
-
-    def lookup_edit_return_pressed(self):
-        self.timer.stop()
-        self.timer.timeout.emit()
-        self.lookup_list.setFocus()
-
-    def lookup_text_changed(self):
-        if len(self.lookup_edit.get_text()) > 1:
-            self.timer.start()
-
-    def keyPressEvent(self, event: QKeyEvent):
-        if event.key() == Qt.Key.Key_Down and self.lookup_edit.hasFocus():
-            event.accept()
-            self.lookup_list.setCurrentRow(0)
-            self.lookup_list.setFocus()
-        elif event.key() == Qt.Key.Key_Up and self.lookup_list.hasFocus() and self.lookup_list.currentRow() == 0:
-            self.lookup_edit.setFocus()
-            event.accept()
-        else:
-            return super().keyPressEvent(event)
+import sys
+
+if __name__ == "__main__":
+
+    sys.path.insert(0, ".")
+
+    from demo.demo import demo
+
+    demo()
+
+
+from PyQt6.QtWidgets import (
+    QVBoxLayout,
+    QWidget,
+)
+from PyQt6.QtGui import QKeyEvent
+
+from PyQt6.QtCore import Qt, QTimer
+
+from q2gui.pyqt6.widgets.q2line import q2line
+from q2gui.pyqt6.widgets.q2list import q2list
+
+
+class q2lookup(QWidget):
+    def __init__(self, parent, text):
+        super().__init__(parent, Qt.WindowType.Popup)
+        self.setLayout(QVBoxLayout())
+        self.layout().setContentsMargins(0, 0, 0, 0)
+        self.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
+        self.lookup_edit = q2line({})
+        self.lookup_list = q2list({})
+        self.layout().addWidget(self.lookup_edit)
+        self.layout().addWidget(self.lookup_list)
+        self.lookup_edit.set_text("" if text == "*" else text)
+        self.lookup_edit.set_focus()
+
+        self.timer = QTimer()
+        self.timer.setSingleShot(True)
+        self.timer.setInterval(500)
+        self.timer.timeout.connect(self.lookup_search)
+
+        self.lookup_edit.textChanged.connect(self.lookup_text_changed)
+        self.lookup_edit.returnPressed.connect(self.lookup_edit_return_pressed)
+
+        self.lookup_list.itemActivated.connect(self.lookup_list_selected)
+
+        self.set_geometry()
+
+    # def lookup_list_selected(self):
+    #     print("Method lookup_list_selected has to be implemented...")
+
+    def set_geometry(self):
+        print("Method set_geometry has to be implemented...")
+
+    # def show(self, column):
+    #     self.q2_model_column = column
+    #     return super().show()
+
+    def lookup_list_selected(self):
+        print(self.lookup_list.currentItem().text())
+        self.close()
+
+    def lookup_search(self):
+        self.lookup_list.clear()
+        for x in range(6):
+            self.lookup_list.addItem(f"{x} Method lookup_search has to be implemented...")
+
+    def lookup_edit_return_pressed(self):
+        self.timer.stop()
+        self.timer.timeout.emit()
+        self.lookup_list.setFocus()
+
+    def lookup_text_changed(self):
+        if len(self.lookup_edit.get_text()) > 1:
+            self.timer.start()
+
+    def keyPressEvent(self, event: QKeyEvent):
+        if event.key() == Qt.Key.Key_Down and self.lookup_edit.hasFocus():
+            event.accept()
+            self.lookup_list.setCurrentRow(0)
+            self.lookup_list.setFocus()
+        elif (
+            event.key() == Qt.Key.Key_Up
+            and self.lookup_list.hasFocus()
+            and self.lookup_list.currentRow() == 0
+        ):
+            self.lookup_edit.setFocus()
+            event.accept()
+        else:
+            return super().keyPressEvent(event)
```

### Comparing `q2gui-0.1.9/q2gui/pyqt6/widgets/q2toolbutton.py` & `q2gui-0.1.90/q2gui/pyqt6/widgets/q2toolbutton.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import sys
-
-if __name__ == "__main__":
-
-    sys.path.insert(0, ".")
-
-    from demo.demo import demo
-
-    demo()
-
-from PyQt6.QtWidgets import QToolButton, QSizePolicy
-
-from q2gui.pyqt6.q2widget import Q2Widget
-
-
-class q2toolbutton(QToolButton, Q2Widget):
-    def __init__(self, meta):
-        super().__init__(meta)
-        self.setSizePolicy(QSizePolicy.Policy.Maximum, QSizePolicy.Policy.Maximum)
-        self.set_text(meta.get("label"))
-        if self.meta.get("valid"):
-            self.clicked.connect(self.valid)
+import sys
+
+if __name__ == "__main__":
+
+    sys.path.insert(0, ".")
+
+    from demo.demo import demo
+
+    demo()
+
+from PyQt6.QtWidgets import QToolButton, QSizePolicy
+
+from q2gui.pyqt6.q2widget import Q2Widget
+
+
+class q2toolbutton(QToolButton, Q2Widget):
+    def __init__(self, meta):
+        super().__init__(meta)
+        self.setSizePolicy(QSizePolicy.Policy.Maximum, QSizePolicy.Policy.Maximum)
+        self.set_text(meta.get("label"))
+        if self.meta.get("valid"):
+            self.clicked.connect(self.valid)
```

### Comparing `q2gui-0.1.9/q2gui/q2model.py` & `q2gui-0.1.90/q2gui/q2model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,466 +1,444 @@
-if __name__ == "__main__":
-    import sys
-
-    sys.path.insert(0, ".")
-
-    from demo.demo import demo
-
-    demo()
-
-import csv
-import datetime
-import re
-
-import q2gui.q2app as q2app
-from q2gui.q2utils import num
-
-try:
-    from q2db.cursor import Q2Cursor
-    from q2db.db import Q2Db
-except Exception:
-    pass
-
-
-class Q2Model:
-    def __init__(self):
-        self.q2_form = None
-        self.columns = []
-        self.headers = []
-        self.alignments = []
-
-        self.records = []
-        self.proxy_records = []
-        self.use_proxy = False
-        self.relation_cache = {}
-        self.lastdata_error_text = ""
-
-        self.meta = []
-
-        # CRUD flags
-        self.readonly = True
-        self.delete_enabled = False
-        self.insert_enabled = False
-        self.update_enabled = False
-
-        self.filterable = False
-
-        self.data_changed = False
-
-        self.order_text = ""
-        self.where_text = ""
-
-    def get_row(self, row_number):
-        if row_number < len(self.records):
-            return self.records[row_number]
-        else:
-            return None
-
-    def get_table_name(self):
-        return ""
-
-    def get_data_error(self):
-        return self.lastdata_error_text
-
-    def set_data_error(self, text=""):
-        self.lastdata_error_text = text
-
-    def update(self, record: dict, current_row, refresh=True):
-        if self.proxy_records:
-            current_row = self.proxy_records[current_row]
-        if self.records:
-            self.records[current_row].update(record)
-        self.data_changed = True
-        if refresh:
-            self.refresh()
-        return True
-
-    def insert(self, record: dict, current_row=0, refresh=True):
-        self.records.append(record)
-        self.data_changed = True
-        if refresh:
-            self.refresh()
-        return True
-
-    def delete(self, row_number, refresh=True):
-        if self.proxy_records:
-            row_number = self.proxy_records[row_number]
-        self.records.pop(row_number)
-        self.data_changed = True
-        if refresh:
-            self.refresh()
-        return True
-
-    def set_where(self, where_text=""):
-        self.where_text = where_text
-        if self.where_text:
-            self.use_proxy = True
-            self.proxy_records = []
-            for row, rec in enumerate(self.records):
-                rc = dict(rec)
-                if eval(self.where_text, rc):
-                    self.proxy_records.append(row)
-        else:
-            self.use_proxy = False
-        self.refresh()
-        return self
-
-    def get_where(self):
-        return self.where_text
-
-    def set_order(self, order_data=""):
-        if isinstance(order_data, int):
-            self.order_text = self.columns[order_data]
-        elif isinstance(order_data, list):
-            self.order_text = ",".join(order_data)
-        else:
-            self.order_text = order_data
-        if self.records:
-            colname = self.order_text
-
-            if self.proxy_records:
-                sort_records = {}
-                for x in range(len(self.proxy_records)):
-                    value = self.records[self.proxy_records[x]][colname]
-                    if value not in sort_records:
-                        sort_records[value] = [self.proxy_records[x]]
-                    else:
-                        sort_records[value].append(self.proxy_records[x])
-            else:
-                sort_records = {}
-                for x in range(len(self.records)):
-                    if self.records[x][colname] not in sort_records:
-                        sort_records[self.records[x][colname]] = [x]
-                    else:
-                        sort_records[self.records[x][colname]].append(x)
-
-            sorted_keys = sorted([x for x in sort_records.keys()])
-            # sorted_keys.sort()
-            tmp_proxy_records = []
-            for x in sorted_keys:
-                for y in sort_records[x]:
-                    tmp_proxy_records.append(y)
-
-            self.proxy_records = tmp_proxy_records
-            self.use_proxy = True
-
-    def refresh(self):
-        self.relation_cache = {}
-
-    # def refresh(self):
-    #     self.set_where(self.where_text)
-    #     self.set_order(self.order_text)
-
-    def reset(self):
-        self.records = []
-        self.proxy_records = []
-        self.use_proxy = False
-        self.relation_cache = {}
-        self.lastdata_error_text = ""
-
-    def set_records(self, records):
-        self.records = records
-
-    def build(self):
-        self.columns = []
-        self.headers = []
-        self.alignments = []
-        self.meta = []
-        for meta in self.q2_form.controls:
-            if meta.get("column", "").startswith("/") or meta.get("nogrid"):
-                continue
-            if meta.get("control", "") in ["button", "widget", "form"]:
-                continue
-            self.q2_form.model.add_column(meta)
-
-    def add_column(self, meta):
-        if not meta.get("control"):
-            meta["control"] = "line"
-
-        meta = q2app.Q2Controls.validate(meta)
-        self.columns.append(meta["column"])
-        self.headers.append(meta["gridlabel" if meta.get("gridlabel") else "label"])
-        self.alignments.append(meta.get("alignment", "7"))
-        self.meta.append(meta)
-
-    def get_record(self, row):
-        if row < 0 or row > len(self.records)-1:
-            return {}
-        if self.use_proxy:
-            return self.records[self.proxy_records[row]]
-        else:
-            return self.records[row]
-
-    def _get_related(self, value, meta, do_not_show_value=False, reset_cache=False):
-        if meta.get("num") and num(value) == 0:
-            return ""
-        elif value == "":
-            return ""
-        key = (meta["to_table"], f"{meta['to_column']}='{value}'", meta["related"])
-        if not reset_cache and key in self.relation_cache:
-            related = self.relation_cache[key]
-        else:
-            related = self.get_related(meta["to_table"], f"{meta['to_column']}='{value}'", meta["related"])
-            self.relation_cache[key] = related
-        if related is None:
-            related = ""
-        if do_not_show_value:
-            return f"{related}"
-        else:
-            return f"{value},{related}"
-
-    def get_related(self, to_table, filter, related):
-        return "get_related"
-
-    def data(self, row, col, role="display"):
-        if role == "display":
-            colName = self.columns[col]
-            value = self.get_record(row).get(colName, "")
-            meta = self.meta[col]
-            if meta.get("relation"):
-                value = self._get_related(value, meta)
-            elif self.is_strign_for_num(meta):
-                value = meta.get("pic").split(";")[int(num(value)) - 1]
-            elif meta.get("num"):  # Numeric value
-                if num(value) == 0:  # do not show zero
-                    value = ""
-                elif meta.get("pic") == "F":  # financial format
-                    format_string = q2app.FINANCIAL_FORMAT % meta.get("datadec", 0)
-                    value = format_string.format(num(value))
-            elif meta["datatype"] == "date":
-                try:
-                    value = datetime.datetime.strptime(value, "%Y-%m-%d").strftime(q2app.DATA_FORMAT_STRING)
-                except Exception:
-                    value = ""
-            return value
-
-    def is_strign_for_num(self, meta):
-        """return str data from numeric controls - radio, list, combo"""
-        return meta.get("num") and ("radio" in meta["control"] or meta["control"] in ("list", "combo"))
-
-    def alignment(self, col):
-        if self.meta[col].get("relation"):
-            return 7
-        elif self.is_strign_for_num(self.meta[col]):
-            return 7
-        return self.alignments[col]
-
-    def column_header_data(self, col):
-        return self.headers[col]
-
-    def row_header_data(self, row):
-        return f"{row}"
-
-    def row_count(self):
-        if self.use_proxy:
-            return len(self.proxy_records)
-        else:
-            return len(self.records)
-
-    def column_count(self):
-        return len(self.columns)
-
-    def parse_lookup_text(self, text):
-        text = text.upper()
-        raw_cond_list = ["+"] + re.split("([+-])", text)
-        cond_list = []
-        for cond in range(int(len(raw_cond_list) / 2)):
-            operator = raw_cond_list[cond * 2]
-            value = raw_cond_list[cond * 2 + 1]
-            if operator and value:
-                cond_list.append([operator, value])
-        return cond_list
-
-    def lookup(self, column, text):
-        """search for text in column, return list of [row, value]"""
-        cond_list = self.parse_lookup_text(text)
-        rez = []
-        for x in range(self.row_count()):
-            cond_result = True
-            for cond in cond_list:
-                operator = cond[0]
-                value = cond[1]
-                model_value = self.get_record(x)[self.columns[column]]
-                if self.meta[column].get("relation"):
-                    model_value = self._get_related(model_value, self.meta[column])
-
-                if operator == "+" and value not in model_value.upper():
-                    cond_result = False
-                elif operator == "-" and value in model_value.upper():
-                    cond_result = False
-            if cond_result:
-                rez.append([x, model_value])
-        return rez
-
-    def data_export(self, file):
-        pass
-
-    def data_import(self, file):
-        pass
-
-
-class Q2CsvModel(Q2Model):
-    def __init__(self, csv_file_object=None):
-        super().__init__()
-        csv_dict = csv.DictReader(csv_file_object)
-        # If there are names with space -  replace spaces in columns names
-        if [filename for filename in csv_dict.fieldnames if " " in filename]:
-            fieldnames = [x.replace(" ", "_") for x in csv_dict.fieldnames]
-            csv_dict = csv.DictReader(csv_file_object, fieldnames)
-        self.set_records([x for x in csv_dict])
-        self.filterable = True
-
-    # def update(self, record: dict, current_row):
-    #     self.records[current_row] = record
-    #     self.data_changed = True
-    #     self.refresh()
-    #     return True
-
-    # def insert(self, record: dict, current_row):
-    #     self.records.append(record)
-    #     self.data_changed = True
-    #     self.refresh()
-    #     return True
-
-    # def delete(self, row_number):
-    #     self.records.pop(row_number)
-    #     self.data_changed = True
-    #     self.refresh()
-    #     return True
-
-    # def set_where(self, where_text=""):
-    #     self.where_text = where_text
-    #     if self.where_text:
-    #         self.use_proxy = True
-    #         self.proxy_records = []
-    #         for row, rec in enumerate(self.records):
-    #             if eval(self.where_text, rec):
-    #                 self.proxy_records.append(row)
-    #     else:
-    #         self.use_proxy = False
-    #     self.refresh()
-
-    # def set_order(self, order_data=""):
-    #     super().set_order(order_data=order_data)
-
-    #     colname = self.order_text
-
-    #     if self.proxy_records:
-    #         sort_records = {}
-    #         for x in range(len(self.proxy_records)):
-    #             value = self.records[self.proxy_records[x]][colname]
-    #             if value not in sort_records:
-    #                 sort_records[value] = [self.proxy_records[x]]
-    #             else:
-    #                 sort_records[value].append(self.proxy_records[x])
-    #     else:
-    #         sort_records = {}
-    #         for x in range(len(self.records)):
-    #             if self.records[x][colname] not in sort_records:
-    #                 sort_records[self.records[x][colname]] = [x]
-    #             else:
-    #                 sort_records[self.records[x][colname]].append(x)
-
-    #     sorted_keys = sorted([x for x in sort_records.keys()])
-    #     # sorted_keys.sort()
-    #     tmp_proxy_records = []
-    #     for x in sorted_keys:
-    #         for y in sort_records[x]:
-    #             tmp_proxy_records.append(y)
-
-    #     self.proxy_records = tmp_proxy_records
-    #     self.use_proxy = True
-
-
-class Q2CursorModel(Q2Model):
-    def __init__(self, cursor: Q2Cursor = None):
-        super().__init__()
-        self.cursor = cursor
-
-        self.readonly = False
-        self.delete_enabled = False
-        self.insert_enabled = False
-        self.update_enabled = False
-
-    def get_table_name(self):
-        return self.cursor.table_name
-
-    def row_count(self):
-        return self.cursor.row_count()
-
-    def get_record(self, row):
-        return self.cursor.record(row)
-
-    def refresh(self):
-        super().refresh()
-        self.cursor.refresh()
-
-    def delete(self, current_row=0, refresh=True):
-        self.set_data_error()
-        record = self.get_record(current_row)
-        if self.cursor.delete(record, refresh=False):
-            if refresh:
-                self.refresh()
-            return True
-        else:
-            self.set_data_error(self.cursor.last_sql_error())
-            return False
-
-    def update(self, record: dict, current_row=0, refresh=True):
-        self.set_data_error()
-        if self.cursor.update(record):
-            if refresh:
-                self.refresh()
-            return True
-        else:
-            self.set_data_error(f"{self.cursor.last_sql_error()}<br>{self.cursor.last_sql()}")
-            return False
-
-    def insert(self, record: dict, current_row=0, refresh=True):
-        self.set_data_error()
-        if self.cursor.insert(record):
-            if refresh:
-                self.refresh()
-            return True
-        else:
-            self.set_data_error(self.cursor.last_sql_error())
-            return False
-
-    def get_related(self, to_table, filter, related):
-        db: Q2Db = self.cursor.q2_db
-        return db.get(to_table, filter, related)
-
-    def set_order(self, order_data):
-        if self.cursor.table_name:
-            super().set_order(order_data=order_data)
-            self.cursor.set_order(self.order_text)
-        return self
-
-    def set_where(self, where_text=""):
-        self.cursor.set_where(where_text)
-        self.refresh()
-        return super().set_where(where_text)
-
-    def add_column(self, meta):
-        """update metadata from db"""
-        db: Q2Db = self.cursor.q2_db
-        db_meta = db.db_schema.get_schema_table_attr(self.cursor.table_name, meta["column"])
-        meta["pk"] = db_meta.get("pk", "")
-        meta["datatype"] = db_meta.get("datatype", meta["datatype"])
-        if num(meta["datalen"]) < num(db_meta.get("datalen", 10)):
-            meta["datalen"] = int(num(db_meta.get("datalen", 10)))
-        if "datadec" not in meta:
-            meta["datadec"] = int(num(db_meta.get("datadec", 2)))
-        return super().add_column(meta)
-
-    def data_export(self, file: str):
-        if file.lower().endswith(".csv"):
-            self.cursor.export_csv(file)
-        else:
-            self.cursor.export_json(file)
-
-    def data_import(self, file: str):
-        if file.lower().endswith(".csv"):
-            self.cursor.import_csv(file)
-        else:
-            self.cursor.import_json(file)
-        self.refresh()
+if __name__ == "__main__":
+    import sys
+
+    sys.path.insert(0, ".")
+
+    from demo.demo import demo
+
+    demo()
+
+import csv
+import datetime
+import re
+
+import q2gui.q2app as q2app
+from q2gui.q2utils import num
+
+try:
+    from q2db.cursor import Q2Cursor
+    from q2db.db import Q2Db
+except Exception:
+    pass
+
+
+class Q2Model:
+    def __init__(self):
+        self.q2_form = None
+        self.columns = []
+        self.headers = []
+        self.alignments = []
+
+        self.records = []
+        self.proxy_records = []
+        self.use_proxy = False
+        self.relation_cache = {}
+        self.lastdata_error_text = ""
+
+        self.meta = []
+        self.cursor = None
+
+        # CRUD flags
+        self.readonly = True
+        self.delete_enabled = False
+        self.insert_enabled = False
+        self.update_enabled = False
+
+        self.filterable = False
+
+        self.data_changed = False
+
+        self.order_text = ""
+        self.where_text = ""
+
+    def get_row(self, row_number):
+        if row_number < len(self.records):
+            return self.records[row_number]
+        else:
+            return None
+
+    def get_table_name(self):
+        return ""
+
+    def get_data_error(self):
+        return self.lastdata_error_text
+
+    def set_data_error(self, text=""):
+        self.lastdata_error_text = text
+
+    def update(self, record: dict, current_row, refresh=True):
+        if self.proxy_records:
+            current_row = self.proxy_records[current_row]
+        if self.records:
+            self.records[current_row].update(record)
+        self.data_changed = True
+        if refresh:
+            self.refresh()
+        return True
+
+    def insert(self, record: dict, current_row=0, refresh=True):
+        self.records.append(record)
+        self.data_changed = True
+        if refresh:
+            self.refresh()
+        return True
+
+    def delete(self, row_number, refresh=True):
+        if self.proxy_records:
+            row_number = self.proxy_records[row_number]
+        self.records.pop(row_number)
+        self.data_changed = True
+        if refresh:
+            self.refresh()
+        return True
+
+    def set_where(self, where_text=""):
+        self.where_text = where_text
+        if self.where_text:
+            self.use_proxy = True
+            self.proxy_records = []
+            for row, rec in enumerate(self.records):
+                rc = dict(rec)
+                if eval(self.where_text, rc):
+                    self.proxy_records.append(row)
+        else:
+            self.use_proxy = False
+        self.refresh()
+        return self
+
+    def get_where(self):
+        return self.where_text
+
+    def set_order(self, order_data=""):
+        if isinstance(order_data, int):
+            self.order_text = self.columns[order_data]
+        elif isinstance(order_data, list):
+            self.order_text = ",".join(order_data)
+        else:
+            self.order_text = order_data
+        if self.records:
+            colname = self.order_text
+
+            if self.proxy_records:
+                sort_records = {}
+                for x in range(len(self.proxy_records)):
+                    value = self.records[self.proxy_records[x]][colname]
+                    if value not in sort_records:
+                        sort_records[value] = [self.proxy_records[x]]
+                    else:
+                        sort_records[value].append(self.proxy_records[x])
+            else:
+                sort_records = {}
+                for x in range(len(self.records)):
+                    if self.records[x][colname] not in sort_records:
+                        sort_records[self.records[x][colname]] = [x]
+                    else:
+                        sort_records[self.records[x][colname]].append(x)
+
+            sorted_keys = sorted([x for x in sort_records.keys()])
+            # sorted_keys.sort()
+            tmp_proxy_records = []
+            for x in sorted_keys:
+                for y in sort_records[x]:
+                    tmp_proxy_records.append(y)
+
+            self.proxy_records = tmp_proxy_records
+            self.use_proxy = True
+
+    def refresh(self):
+        self.relation_cache = {}
+
+    def reset(self):
+        self.records = []
+        self.proxy_records = []
+        self.use_proxy = False
+        self.relation_cache = {}
+        self.lastdata_error_text = ""
+
+    def set_records(self, records):
+        self.records = records
+
+    def build(self):
+        self.columns = []
+        self.headers = []
+        self.alignments = []
+        self.meta = []
+        for meta in self.q2_form.controls:
+            if meta.get("column", "").startswith("/") or meta.get("nogrid"):
+                # if meta.get("column", "").startswith("/"):
+                continue
+            if meta.get("control", "") in ["button", "widget", "form"]:
+                continue
+            self.q2_form.model.add_column(meta)
+
+    def add_column(self, meta):
+        if not meta.get("control"):
+            meta["control"] = "line"
+
+        meta = q2app.Q2Controls.validate(meta)
+        self.columns.append(meta["column"])
+        self.headers.append(meta["gridlabel" if meta.get("gridlabel") else "label"])
+        self.alignments.append(meta.get("alignment", "7"))
+        self.meta.append(meta)
+
+    def get_record(self, row):
+        if row < 0 or row > len(self.records) - 1:
+            return {}
+        if self.use_proxy:
+            return self.records[self.proxy_records[row]]
+        else:
+            return self.records[row]
+
+    def _get_related(self, value, meta, do_not_show_value=False, reset_cache=False):
+        if meta.get("num") and num(value) == 0:
+            return ""
+        elif value == "":
+            return ""
+        key = (meta["to_table"], f"{meta['to_column']}='{value}'", meta["related"])
+        if not reset_cache and key in self.relation_cache:
+            related = self.relation_cache[key]
+        else:
+            related = self.get_related(meta["to_table"], f"{meta['to_column']}='{value}'", meta["related"])
+            self.relation_cache[key] = related
+        if related is None or related == {}:
+            related = ""
+        if do_not_show_value:
+            return f"{related}"
+        else:
+            return f"{value},{related}"
+
+    def get_related(self, to_table, filter, related):
+        return "get_related"
+
+    def data(self, row, col, role="display"):
+        if role == "display":
+            colName = self.columns[col]
+            value = self.get_record(row).get(colName, "")
+            meta = self.meta[col]
+            if meta.get("relation"):
+                value = self._get_related(value, meta)
+            elif meta.get("show"):
+                value = meta.get("show")(mode="grid", row=row)
+            elif self.is_strign_for_num(meta):
+                if num(value) == 0:
+                    value = 1
+                value = meta.get("pic").split(";")[int(num(value)) - 1]
+            elif meta.get("num"):  # Numeric value
+                if num(value) == 0:  # do not show zero
+                    value = ""
+                elif meta.get("pic") == "F":  # financial format
+                    format_string = q2app.FINANCIAL_FORMAT % meta.get("datadec", 0)
+                    value = format_string.format(num(value))
+            elif meta["datatype"] == "date":
+                try:
+                    value = datetime.datetime.strptime(value, "%Y-%m-%d").strftime(q2app.DATE_FORMAT_STRING)
+                except Exception:
+                    value = ""
+            return value
+
+    def is_strign_for_num(self, meta):
+        """return str data from numeric controls - radio, list, combo"""
+        return meta.get("num") and ("radio" in meta["control"] or meta["control"] in ("list", "combo"))
+
+    def alignment(self, col):
+        if self.meta[col].get("relation"):
+            return 7
+        elif self.is_strign_for_num(self.meta[col]):
+            return 7
+        return self.alignments[col]
+
+    def column_header_data(self, col):
+        return self.headers[col]
+
+    def row_header_data(self, row):
+        return f"{row}"
+
+    def row_count(self):
+        if self.use_proxy:
+            return len(self.proxy_records)
+        else:
+            return len(self.records)
+
+    def column_count(self):
+        return len(self.columns)
+
+    def parse_lookup_text(self, text):
+        text = text.upper()
+        raw_cond_list = ["+"] + re.split("([+-])", text)
+        cond_list = []
+        for cond in range(int(len(raw_cond_list) / 2)):
+            operator = raw_cond_list[cond * 2]
+            value = raw_cond_list[cond * 2 + 1]
+            if operator and value:
+                cond_list.append([operator, value])
+        return cond_list
+
+    def lookup(self, column, text):
+        """search for text in column, return list of [row, value]"""
+        cond_list = self.parse_lookup_text(text)
+        rez = []
+        for x in range(self.row_count()):
+            cond_result = True
+            for cond in cond_list:
+                operator = cond[0]
+                value = cond[1]
+                model_value = self.get_record(x)[self.columns[column]]
+                if self.meta[column].get("relation"):
+                    model_value = self._get_related(model_value, self.meta[column])
+
+                if operator == "+" and value not in model_value.upper():
+                    cond_result = False
+                elif operator == "-" and value in model_value.upper():
+                    cond_result = False
+            if cond_result:
+                rez.append([x, model_value])
+        return rez
+
+    def data_export(self, file):
+        pass
+
+    def data_import(self, file):
+        pass
+
+    def seek_row(self, row_dict):
+        pk = self.get_meta_primary_key()
+        if pk and pk in row_dict:
+            for row_number in range(self.row_count()):
+                rec_dic = self.get_record(row_number)
+                if str(row_dict[pk]) == rec_dic[pk]:
+                    return row_number
+        else:
+            for row_number in range(self.row_count()):
+                rec_dic = self.get_record(row_number)
+                found = 1
+                for colname in row_dict:
+                    if row_dict[colname] != rec_dic[colname]:
+                        found = 0
+                        break
+                if found:
+                    return row_number
+        return 0
+
+    def get_meta_primary_key(self):
+        for x in self.q2_form.controls:
+            if x["pk"]:
+                return x["column"]
+
+    def get_uniq_value(self, column, value):
+        pass
+
+    def get_next_sequence(self, column, start_value=0):
+        pass
+
+
+class Q2CsvModel(Q2Model):
+    def __init__(self, csv_file_object=None):
+        super().__init__()
+        csv_dict = csv.DictReader(csv_file_object)
+        # If there are names with space -  replace spaces in columns names
+        if [filename for filename in csv_dict.fieldnames if " " in filename]:
+            fieldnames = [x.replace(" ", "_") for x in csv_dict.fieldnames]
+            csv_dict = csv.DictReader(csv_file_object, fieldnames)
+        self.set_records([x for x in csv_dict])
+        self.filterable = True
+
+
+class Q2CursorModel(Q2Model):
+    def __init__(self, cursor: Q2Cursor = None):
+        super().__init__()
+        self.cursor = cursor
+
+        self.readonly = False
+        self.delete_enabled = False
+        self.insert_enabled = False
+        self.update_enabled = False
+
+    def get_table_name(self):
+        return self.cursor.table_name
+
+    def row_count(self):
+        return self.cursor.row_count()
+
+    def get_record(self, row):
+        return self.cursor.record(row)
+
+    def refresh(self):
+        super().refresh()
+        self.cursor.refresh()
+
+    def get_uniq_value(self, column, value):
+        return self.cursor.get_uniq_value(column, value)
+
+    def get_next_sequence(self, column, start_value=0):
+        return self.cursor.get_next_sequence(column, start_value)
+
+    def delete(self, current_row=0, refresh=True):
+        self.set_data_error()
+        record = self.get_record(current_row)
+        if self.cursor.delete(record, refresh=False):
+            if refresh:
+                self.refresh()
+            return True
+        else:
+            self.set_data_error(self.cursor.last_sql_error())
+            return False
+
+    def update(self, record: dict, current_row=0, refresh=True):
+        self.set_data_error()
+        if self.cursor.update(record, refresh=False):
+            if refresh:
+                self.refresh()
+            return True
+        else:
+            self.set_data_error(f"{self.cursor.last_sql_error()}<br>{self.cursor.last_sql()}")
+            return False
+
+    def insert(self, record: dict, current_row=0, refresh=True):
+        self.set_data_error()
+        if self.cursor.insert(record, refresh=False):
+            if refresh:
+                self.refresh()
+            return True
+        else:
+            self.set_data_error(self.cursor.last_sql_error())
+            return False
+
+    def get_related(self, to_table, filter, related):
+        db: Q2Db = self.cursor.q2_db
+        return db.get(to_table, filter, related)
+
+    def set_order(self, order_data):
+        if self.cursor.table_name:
+            super().set_order(order_data=order_data)
+            self.cursor.set_order(self.order_text)
+        return self
+
+    def set_where(self, where_text=""):
+        self.cursor.set_where(where_text)
+        self.refresh()
+        return super().set_where(where_text)
+
+    def add_column(self, meta):
+        """update metadata from db"""
+        db: Q2Db = self.cursor.q2_db
+        db_meta = db.db_schema.get_schema_table_attr(self.cursor.table_name, meta["column"])
+        meta["pk"] = db_meta.get("pk", "")
+        meta["datatype"] = db_meta.get("datatype", meta["datatype"])
+        if num(meta["datalen"]) < num(db_meta.get("datalen", 10)):
+            meta["datalen"] = int(num(db_meta.get("datalen", 10)))
+        if "datadec" not in meta:
+            meta["datadec"] = int(num(db_meta.get("datadec", 2)))
+        return super().add_column(meta)
+
+    def data_export(self, file: str, tick_callback=None):
+        if file.lower().endswith(".csv"):
+            self.cursor.export_csv(file, tick_callback=tick_callback)
+        else:
+            self.cursor.export_json(file, tick_callback=tick_callback)
+
+    def data_import(self, file: str, tick_callback=None):
+        if file.lower().endswith(".csv"):
+            rez = self.cursor.import_csv(file, tick_callback=tick_callback)
+        else:
+            rez = self.cursor.import_json(file, tick_callback=tick_callback)
+        self.refresh()
+        return rez
```

### Comparing `q2gui-0.1.9/q2gui/q2utils.py` & `q2gui-0.1.90/q2gui/q2utils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-#    Copyright (C) 2021 Andrei Puchko
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-
-from decimal import Decimal
-import datetime
-
-
-def is_sub_list(sublst, lst):
-    return len([x for x in sublst if x in lst]) == len(sublst)
-
-
-def int_(toInt):
-    try:
-        return int(f"{toInt}")
-    except Exception:
-        return int(num(toInt))
-
-def float_(toFloat):
-    try:
-        return float(f"{toFloat}")
-    except Exception:
-        return float(num(toFloat))
-
-
-def num(tonum):
-    try:
-        return Decimal(f"{tonum}")
-    except Exception:
-        return 0
-
-
-def today():
-    return datetime.date.today()
-
-
-class dotdict(dict):
-    """dot.notation access to dictionary attributes"""
-
-    __getattr__ = dict.get
-    __setattr__ = dict.__setitem__
-    __delattr__ = dict.__delitem__
-
-
-def set_dict_default(_dict, _key, _value):
-    """set only key does not exist"""
-    
-    if not _dict.get(_key):
-        _dict[_key] = _value
+#    Copyright (C) 2021 Andrei Puchko
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
+from decimal import Decimal
+import datetime
+
+
+def is_sub_list(sublst, lst):
+    return len([x for x in sublst if x in lst]) == len(sublst)
+
+
+def int_(toInt):
+    try:
+        return int(f"{toInt}")
+    except Exception:
+        return int(num(toInt))
+
+def float_(toFloat):
+    try:
+        return float(f"{toFloat}")
+    except Exception:
+        return float(num(toFloat))
+
+
+def num(tonum):
+    try:
+        return Decimal(f"{tonum}")
+    except Exception:
+        return 0
+
+
+def today():
+    return datetime.date.today()
+
+
+class dotdict(dict):
+    """dot.notation access to dictionary attributes"""
+
+    __getattr__ = dict.get
+    __setattr__ = dict.__setitem__
+    __delattr__ = dict.__delitem__
+
+
+def set_dict_default(_dict, _key, _value):
+    """set only key does not exist"""
+    
+    if not _dict.get(_key):
+        _dict[_key] = _value
```

### Comparing `q2gui-0.1.9/PKG-INFO` & `q2gui-0.1.90/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: q2gui
-Version: 0.1.9
+Version: 0.1.90
 Summary: Python GUI toolkit
 License: Apache 2.0
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyQt6 (>=6.3.0,<7.0.0)
 Requires-Dist: PyQt6-QScintilla (>=2.13.3,<3.0.0)
-Requires-Dist: q2db
+Requires-Dist: darkdetect (>=0.8.0,<0.9.0)
+Requires-Dist: q2db (>=0.1.10)
 Description-Content-Type: text/markdown
 
 # The light Python GUI builder (currently based on PyQt6)
 
 # How to start 
 ## With docker && x11:
 ```bash
```

