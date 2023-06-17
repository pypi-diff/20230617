# Comparing `tmp/pytk_net-0.2.2.tar.gz` & `tmp/pytk_net-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytk_net-0.2.2.tar", last modified: Fri Jun 16 09:05:56 2023, max compression
+gzip compressed data, was "dist\pytk_net-0.2.3.tar", last modified: Sat Jun 17 07:07:08 2023, max compression
```

## Comparing `pytk_net-0.2.2.tar` & `pytk_net-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 09:05:56.766073 pytk_net-0.2.2/
--rw-rw-rw-   0        0        0      966 2023-06-16 09:05:56.766073 pytk_net-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-06-14 06:03:47.000000 pytk_net-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 09:05:56.747701 pytk_net-0.2.2/pytk_net/
--rw-rw-rw-   0        0        0        0 2023-06-09 06:16:51.000000 pytk_net-0.2.2/pytk_net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:05:56.758281 pytk_net-0.2.2/pytk_net/ext/
--rw-rw-rw-   0        0        0        0 2023-06-15 09:25:02.000000 pytk_net-0.2.2/pytk_net/ext/__init__.py
--rw-rw-rw-   0        0        0      582 2023-06-16 07:33:50.000000 pytk_net-0.2.2/pytk_net/ext/icon.py
--rw-rw-rw-   0        0        0     3203 2023-06-16 09:04:24.000000 pytk_net-0.2.2/pytk_net/ext/navmenu.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:05:56.760802 pytk_net-0.2.2/pytk_net/icons/
--rw-rw-rw-   0        0        0    49971 2023-05-31 05:59:23.000000 pytk_net-0.2.2/pytk_net/icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   164360 2023-05-31 05:59:30.000000 pytk_net-0.2.2/pytk_net/icons/bootstrap-icons.woff
-drwxrwxrwx   0        0        0        0 2023-06-16 09:05:56.764791 pytk_net-0.2.2/pytk_net/overwrite/
--rw-rw-rw-   0        0        0     2435 2023-06-14 03:32:19.000000 pytk_net-0.2.2/pytk_net/overwrite/DateEntry.py
--rw-rw-rw-   0        0        0        0 2023-06-14 14:24:28.000000 pytk_net-0.2.2/pytk_net/overwrite/__init__.py
--rw-rw-rw-   0        0        0     2215 2023-06-16 08:55:48.000000 pytk_net-0.2.2/pytk_net/utils.py
--rw-rw-rw-   0        0        0      207 2023-06-16 06:24:00.000000 pytk_net-0.2.2/pytk_net/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:05:56.753293 pytk_net-0.2.2/pytk_net.egg-info/
--rw-rw-rw-   0        0        0      966 2023-06-16 09:05:56.000000 pytk_net-0.2.2/pytk_net.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-06-16 09:05:56.000000 pytk_net-0.2.2/pytk_net.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 09:05:56.000000 pytk_net-0.2.2/pytk_net.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-16 09:05:56.000000 pytk_net-0.2.2/pytk_net.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 09:05:56.767075 pytk_net-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-06-16 09:04:50.000000 pytk_net-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:07:08.065563 pytk_net-0.2.3/
+-rw-rw-rw-   0        0        0      966 2023-06-17 07:07:08.063576 pytk_net-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-06-14 06:03:47.000000 pytk_net-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 07:07:08.043957 pytk_net-0.2.3/pytk_net/
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:16:51.000000 pytk_net-0.2.3/pytk_net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:07:08.054763 pytk_net-0.2.3/pytk_net/ext/
+-rw-rw-rw-   0        0        0        0 2023-06-15 09:25:02.000000 pytk_net-0.2.3/pytk_net/ext/__init__.py
+-rw-rw-rw-   0        0        0      582 2023-06-16 07:33:50.000000 pytk_net-0.2.3/pytk_net/ext/icon.py
+-rw-rw-rw-   0        0        0     3203 2023-06-17 07:05:22.000000 pytk_net-0.2.3/pytk_net/ext/navmenu.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:07:08.057936 pytk_net-0.2.3/pytk_net/icons/
+-rw-rw-rw-   0        0        0    49971 2023-05-31 05:59:23.000000 pytk_net-0.2.3/pytk_net/icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   164360 2023-05-31 05:59:30.000000 pytk_net-0.2.3/pytk_net/icons/bootstrap-icons.woff
+drwxrwxrwx   0        0        0        0 2023-06-17 07:07:08.062577 pytk_net-0.2.3/pytk_net/overwrite/
+-rw-rw-rw-   0        0        0     2435 2023-06-14 03:32:19.000000 pytk_net-0.2.3/pytk_net/overwrite/DateEntry.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 14:24:28.000000 pytk_net-0.2.3/pytk_net/overwrite/__init__.py
+-rw-rw-rw-   0        0        0     2215 2023-06-16 08:55:48.000000 pytk_net-0.2.3/pytk_net/utils.py
+-rw-rw-rw-   0        0        0      207 2023-06-16 06:24:00.000000 pytk_net-0.2.3/pytk_net/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:07:08.050772 pytk_net-0.2.3/pytk_net.egg-info/
+-rw-rw-rw-   0        0        0      966 2023-06-17 07:07:07.000000 pytk_net-0.2.3/pytk_net.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-06-17 07:07:07.000000 pytk_net-0.2.3/pytk_net.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 07:07:07.000000 pytk_net-0.2.3/pytk_net.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 07:07:07.000000 pytk_net-0.2.3/pytk_net.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 07:07:08.065563 pytk_net-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-06-17 07:06:39.000000 pytk_net-0.2.3/setup.py
```

### Comparing `pytk_net-0.2.2/PKG-INFO` & `pytk_net-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytk_net
-Version: 0.2.2
+Version: 0.2.3
 Summary: TkinterHelper布局助手官方拓展和工具库
 Home-page: https://www.pytk.net
 Author: iamxcd
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 TkinterHelper布局助手官方拓展和工具库
```

### Comparing `pytk_net-0.2.2/README.md` & `pytk_net-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.2/pytk_net/ext/icon.py` & `pytk_net-0.2.3/pytk_net/ext/icon.py`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.2/pytk_net/ext/navmenu.py` & `pytk_net-0.2.3/pytk_net/ext/navmenu.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     def __init__(self, parent, menus: List[NavMenuItem], default_color=DARK, hover_color=SECONDARY,
                  selected_color=WARNING, icon_txt_color="#FFF", **kwargs):
         self.default_color = default_color
         self.hover_color = hover_color
         self.selected_color = selected_color
         self.icon_txt_color = icon_txt_color
         self.selected_menu = None
-        self.pack_propagate(False)
 
         super(NavMenu, self).__init__(parent, bootstyle=self.default_color, **kwargs)
+        self.pack_propagate(False)
         for menu in menus:
             self.create_menu(menu)
 
     def create_menu(self, menu: NavMenuItem):
         nav_menu = Frame(self, height=50, bootstyle=self.default_color, padding=(12, 0, 0, 0))
         icon = Icon(nav_menu, icon_name=menu.icon, size=30, color=self.icon_txt_color, name="icon")
         label = Label(nav_menu, text=menu.text, font=("", 12), name="label")
```

### Comparing `pytk_net-0.2.2/pytk_net/icons/bootstrap-icons.json` & `pytk_net-0.2.3/pytk_net/icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.2/pytk_net/icons/bootstrap-icons.woff` & `pytk_net-0.2.3/pytk_net/icons/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.2/pytk_net/overwrite/DateEntry.py` & `pytk_net-0.2.3/pytk_net/overwrite/DateEntry.py`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.2/pytk_net/utils.py` & `pytk_net-0.2.3/pytk_net/utils.py`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.2/pytk_net.egg-info/PKG-INFO` & `pytk_net-0.2.3/pytk_net.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytk-net
-Version: 0.2.2
+Version: 0.2.3
 Summary: TkinterHelper布局助手官方拓展和工具库
 Home-page: https://www.pytk.net
 Author: iamxcd
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 TkinterHelper布局助手官方拓展和工具库
```

