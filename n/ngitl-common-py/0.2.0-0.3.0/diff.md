# Comparing `tmp/ngitl_common_py-0.2.0.tar.gz` & `tmp/ngitl_common_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngitl_common_py-0.2.0.tar", last modified: Fri Jun 16 13:01:52 2023, max compression
+gzip compressed data, was "ngitl_common_py-0.3.0.tar", last modified: Fri Jun 16 22:48:46 2023, max compression
```

## Comparing `ngitl_common_py-0.2.0.tar` & `ngitl_common_py-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 13:01:52.704158 ngitl_common_py-0.2.0/
--rw-rw-rw-   0        0        0      274 2023-06-16 13:01:52.705155 ngitl_common_py-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 13:01:52.716437 ngitl_common_py-0.2.0/ngitl_common_py/
--rw-rw-rw-   0        0        0       76 2023-06-13 08:53:12.000000 ngitl_common_py-0.2.0/ngitl_common_py/__init__.py
--rw-rw-rw-   0        0        0      518 2023-06-16 13:01:52.717354 ngitl_common_py-0.2.0/ngitl_common_py/_version.py
--rw-rw-rw-   0        0        0     2089 2023-06-06 08:26:25.000000 ngitl_common_py-0.2.0/ngitl_common_py/autostart.py
--rw-rw-rw-   0        0        0     2659 2023-06-12 22:52:41.000000 ngitl_common_py-0.2.0/ngitl_common_py/config.py
--rw-rw-rw-   0        0        0      895 2023-06-13 09:00:23.000000 ngitl_common_py-0.2.0/ngitl_common_py/file_viewer_starter.py
--rw-rw-rw-   0        0        0     1626 2023-06-16 12:57:27.000000 ngitl_common_py-0.2.0/ngitl_common_py/log.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:01:52.625537 ngitl_common_py-0.2.0/ngitl_common_py.egg-info/
--rw-rw-rw-   0        0        0      274 2023-06-16 13:01:51.000000 ngitl_common_py-0.2.0/ngitl_common_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      475 2023-06-16 13:01:51.000000 ngitl_common_py-0.2.0/ngitl_common_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 13:01:51.000000 ngitl_common_py-0.2.0/ngitl_common_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-16 13:01:51.000000 ngitl_common_py-0.2.0/ngitl_common_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-16 13:01:51.000000 ngitl_common_py-0.2.0/ngitl_common_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      220 2023-06-16 13:01:52.710332 ngitl_common_py-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      555 2023-06-13 09:11:28.000000 ngitl_common_py-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:01:52.696217 ngitl_common_py-0.2.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-13 08:56:23.000000 ngitl_common_py-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1406 2023-06-06 07:13:53.000000 ngitl_common_py-0.2.0/tests/test_autostart.py
--rw-rw-rw-   0        0        0     2604 2023-06-16 12:57:57.000000 ngitl_common_py-0.2.0/tests/test_log.py
--rw-rw-rw-   0        0        0    83607 2023-06-07 21:51:31.000000 ngitl_common_py-0.2.0/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:48:46.780965 ngitl_common_py-0.3.0/
+-rw-rw-rw-   0        0        0      274 2023-06-16 22:48:46.781606 ngitl_common_py-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 22:48:46.783957 ngitl_common_py-0.3.0/ngitl_common_py/
+-rw-rw-rw-   0        0        0       76 2023-06-13 08:53:12.000000 ngitl_common_py-0.3.0/ngitl_common_py/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-06-16 22:48:46.783957 ngitl_common_py-0.3.0/ngitl_common_py/_version.py
+-rw-rw-rw-   0        0        0     2089 2023-06-06 08:26:25.000000 ngitl_common_py-0.3.0/ngitl_common_py/autostart.py
+-rw-rw-rw-   0        0        0     2618 2023-06-16 22:04:14.000000 ngitl_common_py-0.3.0/ngitl_common_py/config.py
+-rw-rw-rw-   0        0        0      895 2023-06-13 09:00:23.000000 ngitl_common_py-0.3.0/ngitl_common_py/file_viewer_starter.py
+-rw-rw-rw-   0        0        0     1775 2023-06-16 21:27:15.000000 ngitl_common_py-0.3.0/ngitl_common_py/log.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:48:46.750105 ngitl_common_py-0.3.0/ngitl_common_py.egg-info/
+-rw-rw-rw-   0        0        0      274 2023-06-16 22:48:46.000000 ngitl_common_py-0.3.0/ngitl_common_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      475 2023-06-16 22:48:46.000000 ngitl_common_py-0.3.0/ngitl_common_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 22:48:46.000000 ngitl_common_py-0.3.0/ngitl_common_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-16 22:48:46.000000 ngitl_common_py-0.3.0/ngitl_common_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-16 22:48:46.000000 ngitl_common_py-0.3.0/ngitl_common_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      220 2023-06-16 22:48:46.782966 ngitl_common_py-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      555 2023-06-13 09:11:28.000000 ngitl_common_py-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 22:48:46.779010 ngitl_common_py-0.3.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:56:23.000000 ngitl_common_py-0.3.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1406 2023-06-06 07:13:53.000000 ngitl_common_py-0.3.0/tests/test_autostart.py
+-rw-rw-rw-   0        0        0     2604 2023-06-16 12:57:57.000000 ngitl_common_py-0.3.0/tests/test_log.py
+-rw-rw-rw-   0        0        0    83607 2023-06-07 21:51:31.000000 ngitl_common_py-0.3.0/versioneer.py
```

### Comparing `ngitl_common_py-0.2.0/ngitl_common_py/_version.py` & `ngitl_common_py-0.3.0/ngitl_common_py/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-06-16T14:59:04+0200",
+ "date": "2023-06-17T00:47:30+0200",
  "dirty": false,
  "error": null,
- "full-revisionid": "c2b0254ed925bf15a1794c333524c4f6be79df1f",
- "version": "0.2.0"
+ "full-revisionid": "b56265b8e450690a8632294667f0c1c373663c8d",
+ "version": "0.3.0"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `ngitl_common_py-0.2.0/ngitl_common_py/autostart.py` & `ngitl_common_py-0.3.0/ngitl_common_py/autostart.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.2.0/ngitl_common_py/config.py` & `ngitl_common_py-0.3.0/ngitl_common_py/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Copyright (C) 2023, NG:ITL
 import json
 import os
 from pathlib import Path
 from typing import Optional, Any
+from ngitl_common_py.log import LOG_LEVELS
 
-SEARCH_PATHS = [Path.cwd(), Path.cwd().parent, Path.home()]
-
-AVAILABLE_LOG_LEVELS = {"DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"}
+DEFAULT_CONFIG_SEARCH_PATHS = [Path.cwd(), Path.home()]
 
 __config = {}
 
 
 class ConfigEntryError(Exception):
     def __init__(self, msg: str, *args):
         super().__init__(args)
@@ -19,15 +18,15 @@
     def __str__(self):
         return self.msg
 
 
 class ConfigEntryInvalidLogLevelError(ConfigEntryError):
     def __init__(self, log_level: str, *args):
         super().__init__(
-            f"Invalid log level requested: {log_level}, available log level: {AVAILABLE_LOG_LEVELS}",
+            f"Invalid log level requested: {log_level}, available log level: {LOG_LEVELS}",
             args,
         )
 
 
 class ConfigEntryNotADirectoryError(ConfigEntryError):
     def __init__(self, directory_path: Path, *args):
         super().__init__(
@@ -38,15 +37,15 @@
 
 class ConfigEntryFileNotFoundError(ConfigEntryError):
     def __init__(self, file_path: Path, *args):
         super().__init__(f'Invalid config entry, file "{file_path}" is not a valid file!', args)
 
 
 def find_config_file(config_filename: str) -> Optional[Path]:
-    for search_path in SEARCH_PATHS:
+    for search_path in DEFAULT_CONFIG_SEARCH_PATHS:
         filepath_to_check = search_path / config_filename
         if filepath_to_check.exists():
             return filepath_to_check
     return None
 
 
 def read_config(config_file_path: Path):
@@ -69,15 +68,15 @@
 
 def validate_file_path(file_path: Path):
     if not os.path.isfile(file_path):
         raise ConfigEntryFileNotFoundError(file_path)
 
 
 def validate_log_level(log_level_str: str):
-    if log_level_str not in AVAILABLE_LOG_LEVELS:
+    if log_level_str not in LOG_LEVELS:
         raise ConfigEntryInvalidLogLevelError(log_level_str)
 
 
 def get_config() -> dict:
     global __config
     return __config
```

### Comparing `ngitl_common_py-0.2.0/ngitl_common_py/file_viewer_starter.py` & `ngitl_common_py-0.3.0/ngitl_common_py/file_viewer_starter.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.2.0/ngitl_common_py/log.py` & `ngitl_common_py-0.3.0/ngitl_common_py/log.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Copyright (C) 2023, NG:ITL
 import logging
 import datetime
 import sys
 from pathlib import Path
 from typing import Optional
 
-
-EMERGENCY_LOGGING_LOG_LEVEL = "DEBUG"
-
+LOG_LEVELS = {"DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"}
 LOG_FORMAT = "%(asctime)s [%(levelname)s][%(module)s]: %(message)s"
+EMERGENCY_LOGGING_LOG_LEVEL = "DEBUG"
 
 log_filepath: Optional[Path] = None
 
 
 def init_logging(component_name: str, log_file_directory: Path, logging_level: str):
     global log_filepath
     timestamp = datetime.datetime.now()
@@ -39,14 +38,18 @@
         handlers=[stdout_handler, file_handler],
         level=EMERGENCY_LOGGING_LOG_LEVEL,
         format=LOG_FORMAT,
     )
     logging.error("Emergency log initialized!")
 
 
+def validate_log_level(log_level: str) -> bool:
+    return log_level in LOG_LEVELS
+
+
 def get_log_filepath() -> Path:
     global log_filepath
     return log_filepath
 
 
 def flush():
     logger = logging.getLogger()
```

### Comparing `ngitl_common_py-0.2.0/setup.py` & `ngitl_common_py-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.2.0/tests/test_autostart.py` & `ngitl_common_py-0.3.0/tests/test_autostart.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.2.0/tests/test_log.py` & `ngitl_common_py-0.3.0/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.2.0/versioneer.py` & `ngitl_common_py-0.3.0/versioneer.py`

 * *Files identical despite different names*

