# Comparing `tmp/data_aggregator-1.1.1.tar.gz` & `tmp/data_aggregator-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_aggregator-1.1.1.tar", last modified: Sat Jun 17 00:28:25 2023, max compression
+gzip compressed data, was "data_aggregator-1.1.2.tar", last modified: Sat Jun 17 00:42:19 2023, max compression
```

## Comparing `data_aggregator-1.1.1.tar` & `data_aggregator-1.1.2.tar`

### file list

```diff
@@ -1,61 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:25.097707 data_aggregator-1.1.1/
--rw-rw-rw-   0        0        0       39 2023-06-16 20:23:51.000000 data_aggregator-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      279 2023-06-17 00:28:25.097707 data_aggregator-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-03-28 11:01:43.000000 data_aggregator-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:25.099673 data_aggregator-1.1.1/data_aggregator/
--rw-rw-rw-   0        0        0       76 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/__init__.py
--rw-rw-rw-   0        0        0      518 2023-06-17 00:28:25.099673 data_aggregator-1.1.1/data_aggregator/_version.py
--rw-rw-rw-   0        0        0     6621 2023-06-16 22:03:51.000000 data_aggregator-1.1.1/data_aggregator/aggregator.py
--rw-rw-rw-   0        0        0     6256 2023-06-16 22:07:48.000000 data_aggregator-1.1.1/data_aggregator/base_data_aggregator_app.py
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:24.999308 data_aggregator-1.1.1/data_aggregator/gui/
--rw-rw-rw-   0        0        0        0 2023-05-10 23:21:25.000000 data_aggregator-1.1.1/data_aggregator/gui/__init__.py
--rw-rw-rw-   0        0        0     5740 2023-06-17 00:11:46.000000 data_aggregator-1.1.1/data_aggregator/gui/gui.py
--rw-rw-rw-   0        0        0      915 2023-06-16 22:15:11.000000 data_aggregator-1.1.1/data_aggregator/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:24.942094 data_aggregator-1.1.1/data_aggregator/gui/resources/
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:25.003298 data_aggregator-1.1.1/data_aggregator/gui/resources/img/
--rw-rw-rw-   0        0        0     6317 2023-05-10 23:21:25.000000 data_aggregator-1.1.1/data_aggregator/gui/resources/img/application-vnd.appimage.svg
--rw-rw-rw-   0        0        0     1515 2023-05-10 23:21:25.000000 data_aggregator-1.1.1/data_aggregator/gui/resources/img/tab-new-symbolic.svg
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:25.023245 data_aggregator-1.1.1/data_aggregator/gui/ui/
--rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/gui/ui/__init__.py
--rw-rw-rw-   0        0        0     2796 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/gui/ui/input_directory_entry_widget.py
--rw-rw-rw-   0        0        0     2384 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/gui/ui/main_window.py
--rw-rw-rw-   0        0        0     5531 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/gui/ui/preferences_widget.py
--rw-rw-rw-   0        0        0     5929 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/gui/ui/preferences_window.py
--rw-rw-rw-   0        0        0     2932 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/gui/ui/status_widget.py
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:25.031223 data_aggregator-1.1.1/data_aggregator/gui/widgets/
--rw-rw-rw-   0        0        0        0 2023-06-16 20:43:40.000000 data_aggregator-1.1.1/data_aggregator/gui/widgets/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/gui/widgets/input_directory_entry_widget.py
--rw-rw-rw-   0        0        0     3095 2023-06-16 20:45:33.000000 data_aggregator-1.1.1/data_aggregator/gui/widgets/preferences_widget.py
--rw-rw-rw-   0        0        0     1747 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/gui/widgets/status_widget.py
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:25.046228 data_aggregator-1.1.1/data_aggregator/processing/
--rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/processing/__init__.py
--rw-rw-rw-   0        0        0      835 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/processing/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:25.049837 data_aggregator-1.1.1/data_aggregator/processing/processor/
--rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/processing/processor/__init__.py
--rw-rw-rw-   0        0        0      267 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/processing/processor/base_processor.py
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:25.055783 data_aggregator-1.1.1/data_aggregator/processing/reader/
--rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/processing/reader/__init__.py
--rw-rw-rw-   0        0        0      292 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/processing/reader/base_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:25.083713 data_aggregator-1.1.1/data_aggregator/processing/writer/
--rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/processing/writer/__init__.py
--rw-rw-rw-   0        0        0      256 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/processing/writer/base_writer.py
--rw-rw-rw-   0        0        0     1202 2023-06-16 22:03:51.000000 data_aggregator-1.1.1/data_aggregator/processing/writer/cached_writer.py
--rw-rw-rw-   0        0        0      916 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/processing/writer/generic_excel_writer.py
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:25.090725 data_aggregator-1.1.1/data_aggregator/utils/
--rw-rw-rw-   0        0        0        0 2023-06-16 21:47:07.000000 data_aggregator-1.1.1/data_aggregator/utils/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/utils/filesystem_watcher.py
--rw-rw-rw-   0        0        0     2349 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/utils/input_file_tracker.py
--rw-rw-rw-   0        0        0      941 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/data_aggregator/utils/writer_cache.py
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:24.984348 data_aggregator-1.1.1/data_aggregator.egg-info/
--rw-rw-rw-   0        0        0      279 2023-06-17 00:28:24.000000 data_aggregator-1.1.1/data_aggregator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1815 2023-06-17 00:28:24.000000 data_aggregator-1.1.1/data_aggregator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 00:28:24.000000 data_aggregator-1.1.1/data_aggregator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-06-17 00:28:24.000000 data_aggregator-1.1.1/data_aggregator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-17 00:28:24.000000 data_aggregator-1.1.1/data_aggregator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      220 2023-06-17 00:28:25.098789 data_aggregator-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      783 2023-06-16 22:51:40.000000 data_aggregator-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 00:28:25.095713 data_aggregator-1.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     3082 2023-06-16 22:03:51.000000 data_aggregator-1.1.1/tests/test_filesystem_watcher.py
--rw-rw-rw-   0        0        0     4113 2023-06-16 22:03:51.000000 data_aggregator-1.1.1/tests/test_input_file_tracker.py
--rw-rw-rw-   0        0        0    85812 2023-06-16 05:57:54.000000 data_aggregator-1.1.1/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:42:19.201969 data_aggregator-1.1.2/
+-rw-rw-rw-   0        0        0      279 2023-06-17 00:42:19.201969 data_aggregator-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-03-28 11:01:43.000000 data_aggregator-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 00:42:19.203964 data_aggregator-1.1.2/data_aggregator/
+-rw-rw-rw-   0        0        0       76 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-06-17 00:42:19.204962 data_aggregator-1.1.2/data_aggregator/_version.py
+-rw-rw-rw-   0        0        0     6621 2023-06-16 22:03:51.000000 data_aggregator-1.1.2/data_aggregator/aggregator.py
+-rw-rw-rw-   0        0        0     6256 2023-06-16 22:07:48.000000 data_aggregator-1.1.2/data_aggregator/base_data_aggregator_app.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:42:19.144015 data_aggregator-1.1.2/data_aggregator/gui/
+-rw-rw-rw-   0        0        0        0 2023-05-10 23:21:25.000000 data_aggregator-1.1.2/data_aggregator/gui/__init__.py
+-rw-rw-rw-   0        0        0     5631 2023-06-17 00:39:33.000000 data_aggregator-1.1.2/data_aggregator/gui/gui.py
+-rw-rw-rw-   0        0        0      915 2023-06-16 22:15:11.000000 data_aggregator-1.1.2/data_aggregator/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:42:19.155095 data_aggregator-1.1.2/data_aggregator/gui/ui/
+-rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/gui/ui/__init__.py
+-rw-rw-rw-   0        0        0     2796 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/gui/ui/input_directory_entry_widget.py
+-rw-rw-rw-   0        0        0     2384 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/gui/ui/main_window.py
+-rw-rw-rw-   0        0        0     5531 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/gui/ui/preferences_widget.py
+-rw-rw-rw-   0        0        0     5929 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/gui/ui/preferences_window.py
+-rw-rw-rw-   0        0        0     2932 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/gui/ui/status_widget.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:42:19.162077 data_aggregator-1.1.2/data_aggregator/gui/widgets/
+-rw-rw-rw-   0        0        0        0 2023-06-16 20:43:40.000000 data_aggregator-1.1.2/data_aggregator/gui/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/gui/widgets/input_directory_entry_widget.py
+-rw-rw-rw-   0        0        0     3095 2023-06-16 20:45:33.000000 data_aggregator-1.1.2/data_aggregator/gui/widgets/preferences_widget.py
+-rw-rw-rw-   0        0        0     1747 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/gui/widgets/status_widget.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:42:19.168061 data_aggregator-1.1.2/data_aggregator/processing/
+-rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/processing/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/processing/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:42:19.172616 data_aggregator-1.1.2/data_aggregator/processing/processor/
+-rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/processing/processor/__init__.py
+-rw-rw-rw-   0        0        0      267 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/processing/processor/base_processor.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:42:19.178034 data_aggregator-1.1.2/data_aggregator/processing/reader/
+-rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/processing/reader/__init__.py
+-rw-rw-rw-   0        0        0      292 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/processing/reader/base_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:42:19.186013 data_aggregator-1.1.2/data_aggregator/processing/writer/
+-rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/processing/writer/__init__.py
+-rw-rw-rw-   0        0        0      256 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/processing/writer/base_writer.py
+-rw-rw-rw-   0        0        0     1202 2023-06-16 22:03:51.000000 data_aggregator-1.1.2/data_aggregator/processing/writer/cached_writer.py
+-rw-rw-rw-   0        0        0      916 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/processing/writer/generic_excel_writer.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:42:19.194988 data_aggregator-1.1.2/data_aggregator/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-16 21:47:07.000000 data_aggregator-1.1.2/data_aggregator/utils/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/utils/filesystem_watcher.py
+-rw-rw-rw-   0        0        0     2349 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/utils/input_file_tracker.py
+-rw-rw-rw-   0        0        0      941 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/data_aggregator/utils/writer_cache.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:42:19.139029 data_aggregator-1.1.2/data_aggregator.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-06-17 00:42:18.000000 data_aggregator-1.1.2/data_aggregator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1682 2023-06-17 00:42:18.000000 data_aggregator-1.1.2/data_aggregator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 00:42:18.000000 data_aggregator-1.1.2/data_aggregator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-06-17 00:42:18.000000 data_aggregator-1.1.2/data_aggregator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-17 00:42:18.000000 data_aggregator-1.1.2/data_aggregator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      220 2023-06-17 00:42:19.202967 data_aggregator-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      751 2023-06-17 00:38:39.000000 data_aggregator-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:42:19.199975 data_aggregator-1.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     3082 2023-06-16 22:03:51.000000 data_aggregator-1.1.2/tests/test_filesystem_watcher.py
+-rw-rw-rw-   0        0        0     4113 2023-06-16 22:03:51.000000 data_aggregator-1.1.2/tests/test_input_file_tracker.py
+-rw-rw-rw-   0        0        0    85812 2023-06-16 05:57:54.000000 data_aggregator-1.1.2/versioneer.py
```

### Comparing `data_aggregator-1.1.1/data_aggregator/aggregator.py` & `data_aggregator-1.1.2/data_aggregator/aggregator.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/base_data_aggregator_app.py` & `data_aggregator-1.1.2/data_aggregator/base_data_aggregator_app.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/gui/gui.py` & `data_aggregator-1.1.2/data_aggregator/gui/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 class MessageType(Enum):
     INFO = QSystemTrayIcon.Information  # type: ignore
     WARNING = QSystemTrayIcon.Warning  # type: ignore
     ERROR = QSystemTrayIcon.Critical  # type: ignore
 
 
 def resource_path() -> Path:
-    """ Get absolute path to resource, works for dev and for PyInstaller """
-    base_path = getattr(sys, '_MEIPASS', os.path.dirname(os.path.abspath(__file__)))
+    base_path = getattr(sys, '_MEIPASS', os.getcwd())
     return Path(base_path)
 
 
 class Gui(QObject):
     show_message_signal = Signal(str, str, MessageType)
     request_write_config_to_file_signal = Signal()
     request_reinit_signal = Signal()
```

### Comparing `data_aggregator-1.1.1/data_aggregator/gui/main_window.py` & `data_aggregator-1.1.2/data_aggregator/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/gui/ui/input_directory_entry_widget.py` & `data_aggregator-1.1.2/data_aggregator/gui/ui/input_directory_entry_widget.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/gui/ui/main_window.py` & `data_aggregator-1.1.2/data_aggregator/gui/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/gui/ui/preferences_widget.py` & `data_aggregator-1.1.2/data_aggregator/gui/ui/preferences_widget.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/gui/ui/preferences_window.py` & `data_aggregator-1.1.2/data_aggregator/gui/ui/preferences_window.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/gui/ui/status_widget.py` & `data_aggregator-1.1.2/data_aggregator/gui/ui/status_widget.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/gui/widgets/input_directory_entry_widget.py` & `data_aggregator-1.1.2/data_aggregator/gui/widgets/input_directory_entry_widget.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/gui/widgets/preferences_widget.py` & `data_aggregator-1.1.2/data_aggregator/gui/widgets/preferences_widget.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/gui/widgets/status_widget.py` & `data_aggregator-1.1.2/data_aggregator/gui/widgets/status_widget.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/processing/exceptions.py` & `data_aggregator-1.1.2/data_aggregator/processing/exceptions.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/processing/writer/cached_writer.py` & `data_aggregator-1.1.2/data_aggregator/processing/writer/cached_writer.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/processing/writer/generic_excel_writer.py` & `data_aggregator-1.1.2/data_aggregator/processing/writer/generic_excel_writer.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/utils/filesystem_watcher.py` & `data_aggregator-1.1.2/data_aggregator/utils/filesystem_watcher.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/utils/input_file_tracker.py` & `data_aggregator-1.1.2/data_aggregator/utils/input_file_tracker.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator/utils/writer_cache.py` & `data_aggregator-1.1.2/data_aggregator/utils/writer_cache.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/data_aggregator.egg-info/SOURCES.txt` & `data_aggregator-1.1.2/data_aggregator.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 data_aggregator/__init__.py
 data_aggregator/_version.py
 data_aggregator/aggregator.py
@@ -11,16 +10,14 @@
 data_aggregator.egg-info/SOURCES.txt
 data_aggregator.egg-info/dependency_links.txt
 data_aggregator.egg-info/requires.txt
 data_aggregator.egg-info/top_level.txt
 data_aggregator/gui/__init__.py
 data_aggregator/gui/gui.py
 data_aggregator/gui/main_window.py
-data_aggregator/gui/resources/img/application-vnd.appimage.svg
-data_aggregator/gui/resources/img/tab-new-symbolic.svg
 data_aggregator/gui/ui/__init__.py
 data_aggregator/gui/ui/input_directory_entry_widget.py
 data_aggregator/gui/ui/main_window.py
 data_aggregator/gui/ui/preferences_widget.py
 data_aggregator/gui/ui/preferences_window.py
 data_aggregator/gui/ui/status_widget.py
 data_aggregator/gui/widgets/__init__.py
```

### Comparing `data_aggregator-1.1.1/setup.py` & `data_aggregator-1.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,10 +18,9 @@
         "ngitl-common-py~=0.3.0",
         "openpyxl~=3.0.10",
         "watchdog~=3.0.0",
         "PySide6~=6.5.1",
         "pywin32==306",
         "requests~=2.31.0",
         "chardet~=5.1.0",
-    ],
-    include_package_data=True
+    ]
 )
```

### Comparing `data_aggregator-1.1.1/tests/test_filesystem_watcher.py` & `data_aggregator-1.1.2/tests/test_filesystem_watcher.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/tests/test_input_file_tracker.py` & `data_aggregator-1.1.2/tests/test_input_file_tracker.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.1.1/versioneer.py` & `data_aggregator-1.1.2/versioneer.py`

 * *Files identical despite different names*

