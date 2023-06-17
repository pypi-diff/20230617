# Comparing `tmp/q2gui-0.1.90.tar.gz` & `tmp/q2gui-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2gui-0.1.90.tar", max compression
+gzip compressed data, was "q2gui-0.1.91.tar", max compression
```

## Comparing `q2gui-0.1.90.tar` & `q2gui-0.1.91.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      576 2023-06-17 19:21:40.577730 q2gui-0.1.90/pyproject.toml
--rw-r--r--   0        0        0       39 2022-12-11 17:39:14.961644 q2gui-0.1.90/q2gui/__init__.py
--rw-r--r--   0        0        0      892 2022-12-11 17:39:14.961644 q2gui-0.1.90/q2gui/__main__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:14.961644 q2gui-0.1.90/q2gui/pyqt6/__init__.py
--rw-r--r--   0        0        0    17169 2023-06-17 19:19:44.077472 q2gui-0.1.90/q2gui/pyqt6/q2app.py
--rw-r--r--   0        0        0     9406 2023-06-16 23:30:46.736176 q2gui-0.1.90/q2gui/pyqt6/q2form.py
--rw-r--r--   0        0        0      309 2022-12-11 17:39:14.961644 q2gui-0.1.90/q2gui/pyqt6/q2model.py
--rw-r--r--   0        0        0     9758 2023-04-26 21:46:22.544312 q2gui-0.1.90/q2gui/pyqt6/q2style.py
--rw-r--r--   0        0        0     8068 2023-04-23 14:14:48.845890 q2gui-0.1.90/q2gui/pyqt6/q2widget.py
--rw-r--r--   0        0        0     4391 2023-06-17 19:21:29.680879 q2gui-0.1.90/q2gui/pyqt6/q2window.py
--rw-r--r--   0        0        0      754 2023-02-06 11:50:26.449600 q2gui-0.1.90/q2gui/pyqt6/widgets/__init__.py
--rw-r--r--   0        0        0     1320 2023-01-02 22:28:53.285564 q2gui-0.1.90/q2gui/pyqt6/widgets/q2button.py
--rw-r--r--   0        0        0     1979 2022-12-11 17:39:14.965644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2check.py
--rw-r--r--   0        0        0    15572 2023-04-22 11:24:23.071797 q2gui-0.1.90/q2gui/pyqt6/widgets/q2code.py
--rw-r--r--   0        0        0     1380 2023-03-23 12:34:19.124118 q2gui-0.1.90/q2gui/pyqt6/widgets/q2combo.py
--rw-r--r--   0        0        0     6423 2023-03-23 10:59:04.941764 q2gui-0.1.90/q2gui/pyqt6/widgets/q2date.py
--rw-r--r--   0        0        0      872 2022-12-11 17:39:14.969649 q2gui-0.1.90/q2gui/pyqt6/widgets/q2doublespin.py
--rw-r--r--   0        0        0     3384 2023-04-23 14:16:17.951094 q2gui-0.1.90/q2gui/pyqt6/widgets/q2frame.py
--rw-r--r--   0        0        0     8651 2023-04-26 22:53:02.233686 q2gui-0.1.90/q2gui/pyqt6/widgets/q2grid.py
--rw-r--r--   0        0        0     4285 2023-02-10 12:17:07.214549 q2gui-0.1.90/q2gui/pyqt6/widgets/q2image.py
--rw-r--r--   0        0        0     1699 2022-12-11 17:39:14.969649 q2gui-0.1.90/q2gui/pyqt6/widgets/q2label.py
--rw-r--r--   0        0        0     4365 2023-03-24 12:17:15.560065 q2gui-0.1.90/q2gui/pyqt6/widgets/q2line.py
--rw-r--r--   0        0        0     1207 2022-12-11 17:39:14.973644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2list.py
--rw-r--r--   0        0        0     2775 2023-01-07 23:02:31.193844 q2gui-0.1.90/q2gui/pyqt6/widgets/q2lookup.py
--rw-r--r--   0        0        0      663 2022-12-11 17:39:14.973644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2progressbar.py
--rw-r--r--   0        0        0     2406 2023-04-23 23:59:43.413400 q2gui-0.1.90/q2gui/pyqt6/widgets/q2radio.py
--rw-r--r--   0        0        0     6581 2023-03-23 18:18:53.089815 q2gui-0.1.90/q2gui/pyqt6/widgets/q2relation.py
--rw-r--r--   0        0        0      373 2022-12-11 17:39:14.973644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2scroller.py
--rw-r--r--   0        0        0    16774 2023-04-23 13:12:45.146324 q2gui-0.1.90/q2gui/pyqt6/widgets/q2sheet.py
--rw-r--r--   0        0        0      490 2022-12-11 17:39:14.977644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2space.py
--rw-r--r--   0        0        0      574 2022-12-11 17:39:14.977644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2spin.py
--rw-r--r--   0        0        0     2772 2022-12-25 20:49:02.663455 q2gui-0.1.90/q2gui/pyqt6/widgets/q2tab.py
--rw-r--r--   0        0        0      920 2023-02-02 22:06:03.288112 q2gui-0.1.90/q2gui/pyqt6/widgets/q2text.py
--rw-r--r--   0        0        0     6913 2023-04-21 18:39:08.528361 q2gui-0.1.90/q2gui/pyqt6/widgets/q2toolbar.py
--rw-r--r--   0        0        0      541 2022-12-11 17:39:14.977644 q2gui-0.1.90/q2gui/pyqt6/widgets/q2toolbutton.py
--rw-r--r--   0        0        0    20612 2023-06-17 19:08:41.267761 q2gui-0.1.90/q2gui/q2app.py
--rw-r--r--   0        0        0      252 2023-04-17 11:18:17.375721 q2gui-0.1.90/q2gui/q2colors.py
--rw-r--r--   0        0        0    12311 2023-06-09 10:52:14.113389 q2gui-0.1.90/q2gui/q2dialogs.py
--rw-r--r--   0        0        0    68487 2023-06-09 10:49:47.244921 q2gui-0.1.90/q2gui/q2form.py
--rw-r--r--   0        0        0    15084 2023-04-26 21:52:49.700754 q2gui-0.1.90/q2gui/q2model.py
--rw-r--r--   0        0        0     5284 2023-04-26 19:43:48.136965 q2gui-0.1.90/q2gui/q2style.py
--rw-r--r--   0        0        0     1515 2022-12-11 17:39:14.985654 q2gui-0.1.90/q2gui/q2utils.py
--rw-r--r--   0        0        0     4448 2023-04-23 09:29:31.258882 q2gui-0.1.90/q2gui/q2widget.py
--rw-r--r--   0        0        0     3189 2022-12-13 12:21:42.250012 q2gui-0.1.90/q2gui/q2window.py
--rw-r--r--   0        0        0       22 2023-06-17 19:21:42.987988 q2gui-0.1.90/q2gui/version.py
--rw-r--r--   0        0        0     1533 2022-12-11 17:39:14.929664 q2gui-0.1.90/README.md
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 q2gui-0.1.90/PKG-INFO
+-rw-r--r--   0        0        0      576 2023-06-17 19:42:50.489774 q2gui-0.1.91/pyproject.toml
+-rw-r--r--   0        0        0       39 2022-12-11 17:39:14.961644 q2gui-0.1.91/q2gui/__init__.py
+-rw-r--r--   0        0        0      892 2022-12-11 17:39:14.961644 q2gui-0.1.91/q2gui/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:14.961644 q2gui-0.1.91/q2gui/pyqt6/__init__.py
+-rw-r--r--   0        0        0    17169 2023-06-17 19:41:53.115862 q2gui-0.1.91/q2gui/pyqt6/q2app.py
+-rw-r--r--   0        0        0     9406 2023-06-16 23:30:46.736176 q2gui-0.1.91/q2gui/pyqt6/q2form.py
+-rw-r--r--   0        0        0      309 2022-12-11 17:39:14.961644 q2gui-0.1.91/q2gui/pyqt6/q2model.py
+-rw-r--r--   0        0        0     9758 2023-04-26 21:46:22.544312 q2gui-0.1.91/q2gui/pyqt6/q2style.py
+-rw-r--r--   0        0        0     8068 2023-04-23 14:14:48.845890 q2gui-0.1.91/q2gui/pyqt6/q2widget.py
+-rw-r--r--   0        0        0     4357 2023-06-17 19:42:41.291870 q2gui-0.1.91/q2gui/pyqt6/q2window.py
+-rw-r--r--   0        0        0      754 2023-02-06 11:50:26.449600 q2gui-0.1.91/q2gui/pyqt6/widgets/__init__.py
+-rw-r--r--   0        0        0     1320 2023-01-02 22:28:53.285564 q2gui-0.1.91/q2gui/pyqt6/widgets/q2button.py
+-rw-r--r--   0        0        0     1979 2022-12-11 17:39:14.965644 q2gui-0.1.91/q2gui/pyqt6/widgets/q2check.py
+-rw-r--r--   0        0        0    15572 2023-04-22 11:24:23.071797 q2gui-0.1.91/q2gui/pyqt6/widgets/q2code.py
+-rw-r--r--   0        0        0     1380 2023-03-23 12:34:19.124118 q2gui-0.1.91/q2gui/pyqt6/widgets/q2combo.py
+-rw-r--r--   0        0        0     6423 2023-03-23 10:59:04.941764 q2gui-0.1.91/q2gui/pyqt6/widgets/q2date.py
+-rw-r--r--   0        0        0      872 2022-12-11 17:39:14.969649 q2gui-0.1.91/q2gui/pyqt6/widgets/q2doublespin.py
+-rw-r--r--   0        0        0     3384 2023-04-23 14:16:17.951094 q2gui-0.1.91/q2gui/pyqt6/widgets/q2frame.py
+-rw-r--r--   0        0        0     8651 2023-04-26 22:53:02.233686 q2gui-0.1.91/q2gui/pyqt6/widgets/q2grid.py
+-rw-r--r--   0        0        0     4285 2023-02-10 12:17:07.214549 q2gui-0.1.91/q2gui/pyqt6/widgets/q2image.py
+-rw-r--r--   0        0        0     1699 2022-12-11 17:39:14.969649 q2gui-0.1.91/q2gui/pyqt6/widgets/q2label.py
+-rw-r--r--   0        0        0     4365 2023-03-24 12:17:15.560065 q2gui-0.1.91/q2gui/pyqt6/widgets/q2line.py
+-rw-r--r--   0        0        0     1207 2022-12-11 17:39:14.973644 q2gui-0.1.91/q2gui/pyqt6/widgets/q2list.py
+-rw-r--r--   0        0        0     2775 2023-01-07 23:02:31.193844 q2gui-0.1.91/q2gui/pyqt6/widgets/q2lookup.py
+-rw-r--r--   0        0        0      663 2022-12-11 17:39:14.973644 q2gui-0.1.91/q2gui/pyqt6/widgets/q2progressbar.py
+-rw-r--r--   0        0        0     2406 2023-04-23 23:59:43.413400 q2gui-0.1.91/q2gui/pyqt6/widgets/q2radio.py
+-rw-r--r--   0        0        0     6581 2023-03-23 18:18:53.089815 q2gui-0.1.91/q2gui/pyqt6/widgets/q2relation.py
+-rw-r--r--   0        0        0      373 2022-12-11 17:39:14.973644 q2gui-0.1.91/q2gui/pyqt6/widgets/q2scroller.py
+-rw-r--r--   0        0        0    16774 2023-04-23 13:12:45.146324 q2gui-0.1.91/q2gui/pyqt6/widgets/q2sheet.py
+-rw-r--r--   0        0        0      490 2022-12-11 17:39:14.977644 q2gui-0.1.91/q2gui/pyqt6/widgets/q2space.py
+-rw-r--r--   0        0        0      574 2022-12-11 17:39:14.977644 q2gui-0.1.91/q2gui/pyqt6/widgets/q2spin.py
+-rw-r--r--   0        0        0     2772 2022-12-25 20:49:02.663455 q2gui-0.1.91/q2gui/pyqt6/widgets/q2tab.py
+-rw-r--r--   0        0        0      920 2023-02-02 22:06:03.288112 q2gui-0.1.91/q2gui/pyqt6/widgets/q2text.py
+-rw-r--r--   0        0        0     6913 2023-04-21 18:39:08.528361 q2gui-0.1.91/q2gui/pyqt6/widgets/q2toolbar.py
+-rw-r--r--   0        0        0      541 2022-12-11 17:39:14.977644 q2gui-0.1.91/q2gui/pyqt6/widgets/q2toolbutton.py
+-rw-r--r--   0        0        0    20612 2023-06-17 19:08:41.267761 q2gui-0.1.91/q2gui/q2app.py
+-rw-r--r--   0        0        0      252 2023-04-17 11:18:17.375721 q2gui-0.1.91/q2gui/q2colors.py
+-rw-r--r--   0        0        0    12311 2023-06-09 10:52:14.113389 q2gui-0.1.91/q2gui/q2dialogs.py
+-rw-r--r--   0        0        0    68487 2023-06-09 10:49:47.244921 q2gui-0.1.91/q2gui/q2form.py
+-rw-r--r--   0        0        0    15084 2023-04-26 21:52:49.700754 q2gui-0.1.91/q2gui/q2model.py
+-rw-r--r--   0        0        0     5284 2023-04-26 19:43:48.136965 q2gui-0.1.91/q2gui/q2style.py
+-rw-r--r--   0        0        0     1515 2022-12-11 17:39:14.985654 q2gui-0.1.91/q2gui/q2utils.py
+-rw-r--r--   0        0        0     4448 2023-04-23 09:29:31.258882 q2gui-0.1.91/q2gui/q2widget.py
+-rw-r--r--   0        0        0     3189 2022-12-13 12:21:42.250012 q2gui-0.1.91/q2gui/q2window.py
+-rw-r--r--   0        0        0       22 2023-06-17 19:42:52.379839 q2gui-0.1.91/q2gui/version.py
+-rw-r--r--   0        0        0     1533 2022-12-11 17:39:14.929664 q2gui-0.1.91/README.md
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 q2gui-0.1.91/PKG-INFO
```

### Comparing `q2gui-0.1.90/pyproject.toml` & `q2gui-0.1.91/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2gui"
-version = "0.1.90"
+version = "0.1.91"
 description = "Python GUI toolkit"
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
```

### Comparing `q2gui-0.1.90/q2gui/__main__.py` & `q2gui-0.1.91/q2gui/__main__.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/q2app.py` & `q2gui-0.1.91/q2gui/pyqt6/q2app.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/q2form.py` & `q2gui-0.1.91/q2gui/pyqt6/q2form.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/q2style.py` & `q2gui-0.1.91/q2gui/pyqt6/q2style.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/q2widget.py` & `q2gui-0.1.91/q2gui/pyqt6/q2widget.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/q2window.py` & `q2gui-0.1.91/q2gui/pyqt6/q2window.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     return layout
 
 
 class Q2Frame(q2window.Q2Frame, QWidget):
     def set_mode(self, mode="v"):
         self.splitter = None
         super().set_mode(mode=mode)
-        self.set_title("Output")
         if self.layout() is not None:
             return
         self.setLayout(layout(mode))
 
     def insert_widget(self, pos=None, widget=None):
         # if widget:
         #     # widget.setContentsMargins(0,20, 0, 0)
```

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/__init__.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2button.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2button.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2check.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2check.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2code.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2code.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2combo.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2combo.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2date.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2date.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2doublespin.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2doublespin.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2frame.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2frame.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2grid.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2grid.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2image.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2image.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2label.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2label.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2line.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2line.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2list.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2list.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2lookup.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2lookup.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2progressbar.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2progressbar.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2radio.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2radio.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2relation.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2relation.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2sheet.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2sheet.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2spin.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2spin.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2tab.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2tab.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2text.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2text.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2toolbar.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2toolbar.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/pyqt6/widgets/q2toolbutton.py` & `q2gui-0.1.91/q2gui/pyqt6/widgets/q2toolbutton.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/q2app.py` & `q2gui-0.1.91/q2gui/q2app.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/q2dialogs.py` & `q2gui-0.1.91/q2gui/q2dialogs.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/q2form.py` & `q2gui-0.1.91/q2gui/q2form.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/q2model.py` & `q2gui-0.1.91/q2gui/q2model.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/q2style.py` & `q2gui-0.1.91/q2gui/q2style.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/q2utils.py` & `q2gui-0.1.91/q2gui/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/q2widget.py` & `q2gui-0.1.91/q2gui/q2widget.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/q2gui/q2window.py` & `q2gui-0.1.91/q2gui/q2window.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/README.md` & `q2gui-0.1.91/README.md`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.90/PKG-INFO` & `q2gui-0.1.91/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2gui
-Version: 0.1.90
+Version: 0.1.91
 Summary: Python GUI toolkit
 License: Apache 2.0
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

