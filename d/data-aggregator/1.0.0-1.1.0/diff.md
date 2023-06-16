# Comparing `tmp/data_aggregator-1.0.0.tar.gz` & `tmp/data_aggregator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_aggregator-1.0.0.tar", last modified: Fri Jun 16 13:21:55 2023, max compression
+gzip compressed data, was "data_aggregator-1.1.0.tar", last modified: Fri Jun 16 22:56:54 2023, max compression
```

## Comparing `data_aggregator-1.0.0.tar` & `data_aggregator-1.1.0.tar`

### file list

```diff
@@ -1,53 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 13:21:55.538977 data_aggregator-1.0.0/
--rw-rw-rw-   0        0        0      279 2023-06-16 13:21:55.539973 data_aggregator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-03-28 11:01:43.000000 data_aggregator-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 13:21:55.549946 data_aggregator-1.0.0/data_aggregator/
--rw-rw-rw-   0        0        0       76 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/__init__.py
--rw-rw-rw-   0        0        0      518 2023-06-16 13:21:55.552938 data_aggregator-1.0.0/data_aggregator/_version.py
--rw-rw-rw-   0        0        0     4708 2023-06-16 12:47:51.000000 data_aggregator-1.0.0/data_aggregator/app.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:21:55.331280 data_aggregator-1.0.0/data_aggregator/gui/
--rw-rw-rw-   0        0        0        0 2023-05-10 23:21:25.000000 data_aggregator-1.0.0/data_aggregator/gui/__init__.py
--rw-rw-rw-   0        0        0     5436 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/gui/gui.py
--rw-rw-rw-   0        0        0     1474 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/gui/input_directory_entry_widget.py
--rw-rw-rw-   0        0        0      899 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/gui/main_window.py
--rw-rw-rw-   0        0        0     3087 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/gui/preferences_widget.py
--rw-rw-rw-   0        0        0     1747 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/gui/status_widget.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:21:55.380104 data_aggregator-1.0.0/data_aggregator/gui/ui/
--rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/gui/ui/__init__.py
--rw-rw-rw-   0        0        0     2796 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/gui/ui/input_directory_entry_widget.py
--rw-rw-rw-   0        0        0     2384 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/gui/ui/main_window.py
--rw-rw-rw-   0        0        0     5531 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/gui/ui/preferences_widget.py
--rw-rw-rw-   0        0        0     5929 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/gui/ui/preferences_window.py
--rw-rw-rw-   0        0        0     2932 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/gui/ui/status_widget.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:21:55.430081 data_aggregator-1.0.0/data_aggregator/processing/
--rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/__init__.py
--rw-rw-rw-   0        0        0     6631 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/aggregator.py
--rw-rw-rw-   0        0        0      835 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/exceptions.py
--rw-rw-rw-   0        0        0     2685 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/filesystem_watcher.py
--rw-rw-rw-   0        0        0     2349 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/input_file_tracker.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:21:55.446001 data_aggregator-1.0.0/data_aggregator/processing/processor/
--rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/processor/__init__.py
--rw-rw-rw-   0        0        0      267 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/processor/base_processor.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:21:55.465268 data_aggregator-1.0.0/data_aggregator/processing/reader/
--rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/reader/__init__.py
--rw-rw-rw-   0        0        0      292 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/reader/base_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:21:55.499086 data_aggregator-1.0.0/data_aggregator/processing/writer/
--rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/writer/__init__.py
--rw-rw-rw-   0        0        0      256 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/writer/base_writer.py
--rw-rw-rw-   0        0        0     1212 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/writer/cached_writer.py
--rw-rw-rw-   0        0        0      916 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/writer/generic_excel_writer.py
--rw-rw-rw-   0        0        0      941 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/data_aggregator/processing/writer_cache.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:21:55.279815 data_aggregator-1.0.0/data_aggregator.egg-info/
--rw-rw-rw-   0        0        0      279 2023-06-16 13:21:54.000000 data_aggregator-1.0.0/data_aggregator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1606 2023-06-16 13:21:54.000000 data_aggregator-1.0.0/data_aggregator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 13:21:54.000000 data_aggregator-1.0.0/data_aggregator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-06-16 13:21:54.000000 data_aggregator-1.0.0/data_aggregator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-16 13:21:54.000000 data_aggregator-1.0.0/data_aggregator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      220 2023-06-16 13:21:55.545957 data_aggregator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      752 2023-06-16 13:17:07.000000 data_aggregator-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:21:55.530998 data_aggregator-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     3105 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/tests/test_filesystem_watcher.py
--rw-rw-rw-   0        0        0     4118 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/tests/test_input_file_tracker.py
--rw-rw-rw-   0        0        0     2588 2023-06-16 05:57:53.000000 data_aggregator-1.0.0/tests/test_log.py
--rw-rw-rw-   0        0        0    85812 2023-06-16 05:57:54.000000 data_aggregator-1.0.0/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.614976 data_aggregator-1.1.0/
+-rw-rw-rw-   0        0        0       39 2023-06-16 20:23:51.000000 data_aggregator-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      279 2023-06-16 22:56:54.614976 data_aggregator-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-03-28 11:01:43.000000 data_aggregator-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.617967 data_aggregator-1.1.0/data_aggregator/
+-rw-rw-rw-   0        0        0       76 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-06-16 22:56:54.617967 data_aggregator-1.1.0/data_aggregator/_version.py
+-rw-rw-rw-   0        0        0     6621 2023-06-16 22:03:51.000000 data_aggregator-1.1.0/data_aggregator/aggregator.py
+-rw-rw-rw-   0        0        0     6256 2023-06-16 22:07:48.000000 data_aggregator-1.1.0/data_aggregator/base_data_aggregator_app.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.404016 data_aggregator-1.1.0/data_aggregator/gui/
+-rw-rw-rw-   0        0        0        0 2023-05-10 23:21:25.000000 data_aggregator-1.1.0/data_aggregator/gui/__init__.py
+-rw-rw-rw-   0        0        0     5488 2023-06-16 22:20:31.000000 data_aggregator-1.1.0/data_aggregator/gui/gui.py
+-rw-rw-rw-   0        0        0      915 2023-06-16 22:15:11.000000 data_aggregator-1.1.0/data_aggregator/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.309741 data_aggregator-1.1.0/data_aggregator/gui/resources/
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.419973 data_aggregator-1.1.0/data_aggregator/gui/resources/img/
+-rw-rw-rw-   0        0        0     6317 2023-05-10 23:21:25.000000 data_aggregator-1.1.0/data_aggregator/gui/resources/img/application-vnd.appimage.svg
+-rw-rw-rw-   0        0        0     1515 2023-05-10 23:21:25.000000 data_aggregator-1.1.0/data_aggregator/gui/resources/img/tab-new-symbolic.svg
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.471365 data_aggregator-1.1.0/data_aggregator/gui/ui/
+-rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/gui/ui/__init__.py
+-rw-rw-rw-   0        0        0     2796 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/gui/ui/input_directory_entry_widget.py
+-rw-rw-rw-   0        0        0     2384 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/gui/ui/main_window.py
+-rw-rw-rw-   0        0        0     5531 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/gui/ui/preferences_widget.py
+-rw-rw-rw-   0        0        0     5929 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/gui/ui/preferences_window.py
+-rw-rw-rw-   0        0        0     2932 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/gui/ui/status_widget.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.487302 data_aggregator-1.1.0/data_aggregator/gui/widgets/
+-rw-rw-rw-   0        0        0        0 2023-06-16 20:43:40.000000 data_aggregator-1.1.0/data_aggregator/gui/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/gui/widgets/input_directory_entry_widget.py
+-rw-rw-rw-   0        0        0     3095 2023-06-16 20:45:33.000000 data_aggregator-1.1.0/data_aggregator/gui/widgets/preferences_widget.py
+-rw-rw-rw-   0        0        0     1747 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/gui/widgets/status_widget.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.516225 data_aggregator-1.1.0/data_aggregator/processing/
+-rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/processing/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/processing/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.544164 data_aggregator-1.1.0/data_aggregator/processing/processor/
+-rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/processing/processor/__init__.py
+-rw-rw-rw-   0        0        0      267 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/processing/processor/base_processor.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.553140 data_aggregator-1.1.0/data_aggregator/processing/reader/
+-rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/processing/reader/__init__.py
+-rw-rw-rw-   0        0        0      292 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/processing/reader/base_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.586071 data_aggregator-1.1.0/data_aggregator/processing/writer/
+-rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/processing/writer/__init__.py
+-rw-rw-rw-   0        0        0      256 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/processing/writer/base_writer.py
+-rw-rw-rw-   0        0        0     1202 2023-06-16 22:03:51.000000 data_aggregator-1.1.0/data_aggregator/processing/writer/cached_writer.py
+-rw-rw-rw-   0        0        0      916 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/processing/writer/generic_excel_writer.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.601013 data_aggregator-1.1.0/data_aggregator/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-16 21:47:07.000000 data_aggregator-1.1.0/data_aggregator/utils/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/utils/filesystem_watcher.py
+-rw-rw-rw-   0        0        0     2349 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/utils/input_file_tracker.py
+-rw-rw-rw-   0        0        0      941 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/data_aggregator/utils/writer_cache.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.388059 data_aggregator-1.1.0/data_aggregator.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-06-16 22:56:53.000000 data_aggregator-1.1.0/data_aggregator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1815 2023-06-16 22:56:54.000000 data_aggregator-1.1.0/data_aggregator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 22:56:53.000000 data_aggregator-1.1.0/data_aggregator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-06-16 22:56:53.000000 data_aggregator-1.1.0/data_aggregator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-16 22:56:53.000000 data_aggregator-1.1.0/data_aggregator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      220 2023-06-16 22:56:54.616970 data_aggregator-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-06-16 22:51:40.000000 data_aggregator-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:56:54.613044 data_aggregator-1.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-16 05:57:53.000000 data_aggregator-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     3082 2023-06-16 22:03:51.000000 data_aggregator-1.1.0/tests/test_filesystem_watcher.py
+-rw-rw-rw-   0        0        0     4113 2023-06-16 22:03:51.000000 data_aggregator-1.1.0/tests/test_input_file_tracker.py
+-rw-rw-rw-   0        0        0    85812 2023-06-16 05:57:54.000000 data_aggregator-1.1.0/versioneer.py
```

### Comparing `data_aggregator-1.0.0/data_aggregator/app.py` & `data_aggregator-1.1.0/data_aggregator/base_data_aggregator_app.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,133 +1,178 @@
 # Copyright (C) 2022, NG:ITL
-import argparse
 import logging
 import abc
 import sys
 import traceback
 
 from abc import ABCMeta
 from pathlib import Path
 from PySide6.QtCore import QObject, Slot
-from typing import Optional, Tuple
+from typing import Optional
+from argparse import ArgumentParser
 
 from data_aggregator.processing.processor.base_processor import BaseProcessor
 from data_aggregator.processing.reader.base_reader import BaseReader
 from data_aggregator.processing.writer.cached_writer import CachedWriter
 from data_aggregator.gui.gui import Gui
-from data_aggregator.processing.aggregator import DataAggregator
+from data_aggregator.aggregator import DataAggregator
 
-from ngitl_common_py.log import init_logging, init_emergency_logging
+from ngitl_common_py.log import init_logging, init_emergency_logging, validate_log_level
 from ngitl_common_py.config import (
     get_config,
     get_config_param,
     find_config_file,
     read_config,
     write_config_to_file,
     ConfigEntryError,
-    SEARCH_PATHS,
+    DEFAULT_CONFIG_SEARCH_PATHS,
 )
 
 
-class DataAggregatorAppMeta(type(QObject), ABCMeta):  # type: ignore
+class BaseDataAggregatorAppMeta(type(QObject), ABCMeta):  # type: ignore
     pass
 
 
-class DataAggregatorApp(QObject, metaclass=DataAggregatorAppMeta):
+class BaseDataAggregatorApp(QObject, metaclass=BaseDataAggregatorAppMeta):
     def __init__(self, parent: Optional[QObject] = None):
         QObject.__init__(self, parent)
 
-        self.config_filepath = self.setup_config()
-        self.setup_logging()
+        self.input_reader: Optional[BaseReader] = None
+        self.processor: Optional[BaseProcessor] = None
+        self.output_writer: Optional[CachedWriter] = None
 
-        self.gui = self.setup_gui()
-        self.input_reader, self.processor, self.output_writer = self.setup_components()
-        self.data_aggregator: Optional[DataAggregator] = self.setup_aggregator()
+        self.args = self._parse_args()
+        self.config_filepath = self._setup_config()
+        self._setup_logging()
+
+        self.gui = self._setup_gui()
+
+        self.setup_processing()
+
+        self.data_aggregator = self._setup_aggregator()
+
+    @abc.abstractmethod
+    def add_cli_arguments(self, argument_parser: ArgumentParser) -> None:
+        raise NotImplementedError
 
     @abc.abstractmethod
-    def setup_components(self) -> Tuple[BaseReader, BaseProcessor, CachedWriter]:
+    def setup_processing(self) -> None:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def setup_gui(self, gui: Gui) -> None:
         raise NotImplementedError
 
     @abc.abstractmethod
     def validate_config(self, config: dict) -> None:
         raise NotImplementedError
 
     @abc.abstractmethod
     def get_version(self) -> str:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def get_name(self) -> str:
+    def get_app_name(self) -> str:
         raise NotImplementedError
 
-    def setup_config(self) -> Path:
-        name = self.get_name()
-        config_filepath = find_config_file(f"{name}_config.json")
+    def _parse_args(self):
+        arg_parser = ArgumentParser(prog="data_aggregator", description="Smart data processing")
+        arg_parser.add_argument("--version", action="store_true",
+                                help="Prints the version.")
+        arg_parser.add_argument('-c', '--config', dest='config_filepath',
+                                help="Override the config filepath.")
+        arg_parser.add_argument('-l', '--log-level', dest='log_level',
+                                help="Override the log level.")
+        self.add_cli_arguments(arg_parser)
+        return arg_parser.parse_args()
+
+    def _determine_config_filepath(self) -> Optional[Path]:
+        if self.args.config_filepath:
+            return self.args.config_filepath
+        else:
+            app_name = self.get_app_name()
+            return find_config_file(f"{app_name}_config.json")
+
+    def _setup_config(self) -> Path:
+        app_name = self.get_app_name()
+        config_filepath = self._determine_config_filepath()
         if config_filepath is None:
-            init_emergency_logging(name)
-            logging.error("Unable to find config file in search paths: %s", SEARCH_PATHS)
+            init_emergency_logging(app_name)
+            logging.error("Unable to find config file in search paths: %s", DEFAULT_CONFIG_SEARCH_PATHS)
             sys.exit(-1)
         read_config(config_filepath)
         try:
             config = get_config()
             self.validate_config(config)
         except ConfigEntryError as e:
-            init_emergency_logging(name)
+            init_emergency_logging(app_name)
             logging.error(e)
             sys.exit(-1)
         return config_filepath
 
-    def setup_logging(self) -> None:
+    def _determine_log_level(self) -> str:
+        log_level: Optional[str] = None
+        if self.args.log_level:
+            log_level = self.args.log_level
+        else:
+            log_level = get_config_param("logging_level")
+
+        if validate_log_level(log_level):
+            return log_level
+        else:
+            return "DEBUG"
+
+    def _setup_logging(self) -> None:
         log_file_directory = Path(get_config_param("log_file_directory"))
-        logging_level = get_config_param("logging_level")
+        logging_level = self._determine_log_level()
         init_logging("data_aggregator", log_file_directory, logging_level)
-        logging.info("Config search paths: %s", SEARCH_PATHS)
+        logging.info("Config search paths: %s", DEFAULT_CONFIG_SEARCH_PATHS)
         logging.info("Using config file: %s", self.config_filepath)
 
-    def setup_gui(self) -> Gui:
+    def _setup_gui(self) -> Gui:
         gui = Gui()
         gui.request_reinit_signal.connect(self.handle_reinit_signal)
         return gui
 
-    def setup_aggregator(self) -> DataAggregator:
+    def _setup_aggregator(self) -> DataAggregator:
         data_aggregator = DataAggregator(self.input_reader, self.processor, self.output_writer)
 
         data_aggregator.show_message_signal.connect(self.gui.handle_show_message_signal)
         data_aggregator.processing_results_signal.connect(self.gui.handle_processing_results)
         self.gui.request_cache_flush_signal.connect(data_aggregator.handle_cache_flush_request)
         self.gui.request_write_config_to_file_signal.connect(self.handle_request_write_config_to_file_signal)
 
         data_aggregator.start_initial_file_check()
         data_aggregator.start_filesystem_watcher()
         return data_aggregator
 
-    def stop_processor(self) -> None:
+    def _stop_aggregator(self) -> None:
         if self.data_aggregator:
             self.data_aggregator.stop()
             self.data_aggregator = None
 
     @Slot()
     def handle_reinit_signal(self) -> None:
         logging.info("Reinit signal triggered")
-        self.stop_processor()
-        self.data_aggregator = self.setup_aggregator()
+        self._stop_aggregator()
+        self.data_aggregator = self._setup_aggregator()
 
     @Slot()
     def handle_request_write_config_to_file_signal(self) -> None:
         logging.info("Writing config to file")
         write_config_to_file(self.config_filepath)
 
+    def process_cli_arguments(self):
+        if self.args.version:
+            print(self.get_version())
+            sys.exit(0)
+
     def run(self) -> None:
         try:
-            parser = argparse.ArgumentParser(prog="data_aggregator", description="Smart data processing")
-            parser.add_argument("--version", action="store_true")
-            args = parser.parse_args()
-
-            if args.version:
-                print(self.get_version())
-                sys.exit(0)
+
+            self.process_cli_arguments()
 
             self.gui.run()
 
         except Exception as e:
             logging.error(traceback.format_exc())
             raise e
```

### Comparing `data_aggregator-1.0.0/data_aggregator/gui/gui.py` & `data_aggregator-1.1.0/data_aggregator/gui/gui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # Copyright (C) 2022, NG:ITL
 import logging
 from enum import Enum
+from pathlib import Path
 from typing import Optional, List
 
 from PySide6.QtCore import QObject, Signal, Slot
 from PySide6.QtGui import QIcon, QAction
 from PySide6.QtWidgets import QApplication, QSystemTrayIcon, QMenu
 
-# from data_aggregator.gui.preferences_window import PreferencesWindow
 from data_aggregator.gui.main_window import MainWindow
-from ngitl_common_py.config import get_config, write_config_to_file, set_config_param
-from ngitl_common_py.log import Log
+
+from ngitl_common_py.config import set_config_param
+from ngitl_common_py.log import get_log_filepath
 from ngitl_common_py.autostart import activate_autostart, deactivate_autostart
 from ngitl_common_py.file_viewer_starter import open_file_viewer
 
 
+BASE_DIR = Path(__file__).parent
+
+
 class MessageType(Enum):
     INFO = QSystemTrayIcon.Information  # type: ignore
     WARNING = QSystemTrayIcon.Warning  # type: ignore
     ERROR = QSystemTrayIcon.Critical  # type: ignore
 
 
 class Gui(QObject):
@@ -26,14 +30,16 @@
     request_write_config_to_file_signal = Signal()
     request_reinit_signal = Signal()
     request_cache_flush_signal = Signal()
 
     def __init__(self, parent: Optional[QObject] = None):
         QObject.__init__(self, parent)
 
+        self.icon = QIcon(str(BASE_DIR / "resources/img/application-vnd.appimage.svg"))
+
         self.app: QApplication
         self.main_window: MainWindow
         self.tray_icon: QSystemTrayIcon
         self.menu: QMenu
         self.about_action: QAction
         self.preferences_action: QAction
         self.log_action: QAction
@@ -53,22 +59,22 @@
         self.app = QApplication([])
         self.app.setQuitOnLastWindowClosed(False)
         self.app.setApplicationName("DataAggregator")
 
     def setup_main_window(self):
         self.main_window = MainWindow()
         self.main_window.setup_ui()
+        self.main_window.setWindowIcon(self.icon)
 
     def setup_trayicon(self):
         # Create the icon
-        icon = QIcon("./resources/img/application-vnd.appimage.svg")
 
         # Create the tray
         self.tray_icon = QSystemTrayIcon()
-        self.tray_icon.setIcon(icon)
+        self.tray_icon.setIcon(self.icon)
         self.tray_icon.setVisible(True)
 
         # Create the menu
         self.menu = QMenu()
 
         self.about_action = QAction("About")
         self.menu.addAction(self.about_action)
@@ -132,14 +138,14 @@
     @Slot()
     def handle_preferences_action_triggered(self):
         self.main_window.show()
         self.main_window.main_window.tabWidget.setCurrentIndex(1)
 
     @Slot()
     def handle_log_action_triggered(self):
-        open_file_viewer(Log.log_filepath)
+        open_file_viewer(get_log_filepath())
 
     def show_info_message(self, title: str, message: str):
         self.show_message_signal.emit(title, message, MessageType.INFO)
 
     def run(self):
         self.app.exec_()
```

### Comparing `data_aggregator-1.0.0/data_aggregator/gui/input_directory_entry_widget.py` & `data_aggregator-1.1.0/data_aggregator/gui/widgets/input_directory_entry_widget.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.0.0/data_aggregator/gui/main_window.py` & `data_aggregator-1.1.0/data_aggregator/gui/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2023, NG:ITL
 from typing import Optional
 
 from PySide6.QtWidgets import QMainWindow, QWidget
 
 from data_aggregator.gui.ui.main_window import Ui_MainWindow
-from data_aggregator.gui.preferences_widget import PreferencesWidget
-from data_aggregator.gui.status_widget import StatusWidget
+from data_aggregator.gui.widgets.preferences_widget import PreferencesWidget
+from data_aggregator.gui.widgets.status_widget import StatusWidget
 
 
 class MainWindow(QMainWindow):
     def __init__(self, parent: Optional[QWidget] = None):
         super(MainWindow, self).__init__(parent)
         self.main_window = Ui_MainWindow()
         self.main_window.setupUi(self)
```

### Comparing `data_aggregator-1.0.0/data_aggregator/gui/preferences_widget.py` & `data_aggregator-1.1.0/data_aggregator/gui/widgets/preferences_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2023, NG:ITL
 from typing import List, Optional
 
 from PySide6.QtCore import Signal, Slot
 from PySide6.QtWidgets import QFileDialog, QWidget
 
 from data_aggregator.gui.ui.preferences_widget import Ui_PreferencesWidget
-from data_aggregator.gui.input_directory_entry_widget import InputDirectoryEntryWidget
+from data_aggregator.gui.widgets.input_directory_entry_widget import InputDirectoryEntryWidget
 from ngitl_common_py.config import get_config_param
 from ngitl_common_py.autostart import is_autostart_enabled
 
 
 class PreferencesWidget(QWidget):
     apply_signal = Signal()
```

### Comparing `data_aggregator-1.0.0/data_aggregator/gui/status_widget.py` & `data_aggregator-1.1.0/data_aggregator/gui/widgets/status_widget.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.0.0/data_aggregator/gui/ui/input_directory_entry_widget.py` & `data_aggregator-1.1.0/data_aggregator/gui/ui/input_directory_entry_widget.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.0.0/data_aggregator/gui/ui/main_window.py` & `data_aggregator-1.1.0/data_aggregator/gui/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.0.0/data_aggregator/gui/ui/preferences_widget.py` & `data_aggregator-1.1.0/data_aggregator/gui/ui/preferences_widget.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.0.0/data_aggregator/gui/ui/preferences_window.py` & `data_aggregator-1.1.0/data_aggregator/gui/ui/preferences_window.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.0.0/data_aggregator/gui/ui/status_widget.py` & `data_aggregator-1.1.0/data_aggregator/gui/ui/status_widget.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.0.0/data_aggregator/processing/aggregator.py` & `data_aggregator-1.1.0/data_aggregator/aggregator.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from PySide6.QtCore import QObject, Signal, Slot
 
 from data_aggregator.gui.gui import MessageType
 from data_aggregator.processing.writer.cached_writer import CachedWriter
 from data_aggregator.processing.processor.base_processor import BaseProcessor
 from data_aggregator.processing.reader.base_reader import BaseReader
 from data_aggregator.processing.exceptions import ReaderException, ProcessorException, WriterException
-from data_aggregator.processing.input_file_tracker import InputFileTracker
-from data_aggregator.processing.filesystem_watcher import FilesystemWatcher
+from data_aggregator.utils.input_file_tracker import InputFileTracker
+from data_aggregator.utils.filesystem_watcher import FilesystemWatcher
 
 from ngitl_common_py.config import get_config_param
 
 
 class DataAggregator(QObject):
     show_message_signal = Signal(str, str, MessageType)
     processing_results_signal = Signal(list, list)
```

### Comparing `data_aggregator-1.0.0/data_aggregator/processing/exceptions.py` & `data_aggregator-1.1.0/data_aggregator/processing/exceptions.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.0.0/data_aggregator/processing/filesystem_watcher.py` & `data_aggregator-1.1.0/data_aggregator/utils/filesystem_watcher.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.0.0/data_aggregator/processing/input_file_tracker.py` & `data_aggregator-1.1.0/data_aggregator/utils/input_file_tracker.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.0.0/data_aggregator/processing/writer/cached_writer.py` & `data_aggregator-1.1.0/data_aggregator/processing/writer/cached_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2023, NG:ITL
 import logging
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 from pathlib import Path
 from typing import List
 
 from data_aggregator.processing.writer.base_writer import BaseWriter
-from data_aggregator.processing.writer_cache import WriterCache
+from data_aggregator.utils.writer_cache import WriterCache
 
 
 class CachedWriter(BaseWriter):
     def __init__(self, cache_filepath: Path):
         super().__init__()
         self.writer_cache = WriterCache(cache_filepath)
```

### Comparing `data_aggregator-1.0.0/data_aggregator/processing/writer/generic_excel_writer.py` & `data_aggregator-1.1.0/data_aggregator/processing/writer/generic_excel_writer.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.0.0/data_aggregator/processing/writer_cache.py` & `data_aggregator-1.1.0/data_aggregator/utils/writer_cache.py`

 * *Files identical despite different names*

### Comparing `data_aggregator-1.0.0/data_aggregator.egg-info/SOURCES.txt` & `data_aggregator-1.1.0/data_aggregator.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,46 @@
+MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 data_aggregator/__init__.py
 data_aggregator/_version.py
-data_aggregator/app.py
+data_aggregator/aggregator.py
+data_aggregator/base_data_aggregator_app.py
 data_aggregator.egg-info/PKG-INFO
 data_aggregator.egg-info/SOURCES.txt
 data_aggregator.egg-info/dependency_links.txt
 data_aggregator.egg-info/requires.txt
 data_aggregator.egg-info/top_level.txt
 data_aggregator/gui/__init__.py
 data_aggregator/gui/gui.py
-data_aggregator/gui/input_directory_entry_widget.py
 data_aggregator/gui/main_window.py
-data_aggregator/gui/preferences_widget.py
-data_aggregator/gui/status_widget.py
+data_aggregator/gui/resources/img/application-vnd.appimage.svg
+data_aggregator/gui/resources/img/tab-new-symbolic.svg
 data_aggregator/gui/ui/__init__.py
 data_aggregator/gui/ui/input_directory_entry_widget.py
 data_aggregator/gui/ui/main_window.py
 data_aggregator/gui/ui/preferences_widget.py
 data_aggregator/gui/ui/preferences_window.py
 data_aggregator/gui/ui/status_widget.py
+data_aggregator/gui/widgets/__init__.py
+data_aggregator/gui/widgets/input_directory_entry_widget.py
+data_aggregator/gui/widgets/preferences_widget.py
+data_aggregator/gui/widgets/status_widget.py
 data_aggregator/processing/__init__.py
-data_aggregator/processing/aggregator.py
 data_aggregator/processing/exceptions.py
-data_aggregator/processing/filesystem_watcher.py
-data_aggregator/processing/input_file_tracker.py
-data_aggregator/processing/writer_cache.py
 data_aggregator/processing/processor/__init__.py
 data_aggregator/processing/processor/base_processor.py
 data_aggregator/processing/reader/__init__.py
 data_aggregator/processing/reader/base_reader.py
 data_aggregator/processing/writer/__init__.py
 data_aggregator/processing/writer/base_writer.py
 data_aggregator/processing/writer/cached_writer.py
 data_aggregator/processing/writer/generic_excel_writer.py
+data_aggregator/utils/__init__.py
+data_aggregator/utils/filesystem_watcher.py
+data_aggregator/utils/input_file_tracker.py
+data_aggregator/utils/writer_cache.py
 tests/__init__.py
 tests/test_filesystem_watcher.py
-tests/test_input_file_tracker.py
-tests/test_log.py
+tests/test_input_file_tracker.py
```

### Comparing `data_aggregator-1.0.0/setup.py` & `data_aggregator-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,17 @@
     description="Simple data aggregator framework to simplify data processing",
     author="NG:ITL",
     license="GPLv3",
     author_email="torsten.wylegala@volkswagen.de",
     url="https://github.com/vw-wob-it-edu-ngitl/data_aggregator/",
     packages=find_packages("."),
     install_requires=[
-        "ngitl-common-py~=0.2.0",
+        "ngitl-common-py~=0.3.0",
         "openpyxl~=3.0.10",
         "watchdog~=3.0.0",
         "PySide6~=6.5.1",
         "pywin32==306",
         "requests~=2.31.0",
         "chardet~=5.1.0",
     ],
+    include_package_data=True
 )
```

### Comparing `data_aggregator-1.0.0/tests/test_filesystem_watcher.py` & `data_aggregator-1.1.0/tests/test_filesystem_watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Copyright (C) 2023, NG:ITL
-import os
 import tempfile
 import time
 import unittest
 
 from pathlib import Path
-from typing import List, Tuple
+from typing import List
 
-from data_aggregator.processing.filesystem_watcher import FilesystemWatcher
+from data_aggregator.utils.filesystem_watcher import FilesystemWatcher
 
 
 class FilesystemWatcherTest(unittest.TestCase):
 
     FILESYSTEM_WATCHER_DELAY = 0.3
 
     def setUp(self) -> None:
```

### Comparing `data_aggregator-1.0.0/tests/test_input_file_tracker.py` & `data_aggregator-1.1.0/tests/test_input_file_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import unittest
 import csv
 
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
-from data_aggregator.processing.input_file_tracker import InputFileTracker
+from data_aggregator.utils.input_file_tracker import InputFileTracker
 
 
 class FilesystemWatcherTest(unittest.TestCase):
 
     INPUT_FILE_TRACKER_FILENAME = "input_file_tracker_history.csv"
 
     def setUp(self) -> None:
```

### Comparing `data_aggregator-1.0.0/versioneer.py` & `data_aggregator-1.1.0/versioneer.py`

 * *Files identical despite different names*

