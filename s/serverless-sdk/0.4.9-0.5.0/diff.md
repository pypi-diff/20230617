# Comparing `tmp/serverless-sdk-0.4.9.tar.gz` & `tmp/serverless-sdk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-s5iy1w2o/serverless-sdk-0.4.9.tar", last modified: Thu May 18 09:11:23 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-fyjwcwni/serverless-sdk-0.5.0.tar", last modified: Sat Jun 17 19:45:58 2023, max compression
```

## Comparing `serverless-sdk-0.4.9.tar` & `serverless-sdk-0.5.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/serverless_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/sls_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/sls_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/warning_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/tests/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/tests/test_sdk_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/tests/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/tag_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/lib/warning_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/sls_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:45:58.000000 serverless-sdk-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-06-17 19:45:39.000000 serverless-sdk-0.5.0/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.4.9/PKG-INFO` & `serverless-sdk-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.9
+Version: 0.5.0
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.4.9/README.md` & `serverless-sdk-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.9/pyproject.toml` & `serverless-sdk-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.9/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.5.0/serverless_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.9
+Version: 0.5.0
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.4.9/serverless_sdk.egg-info/SOURCES.txt` & `serverless-sdk-0.5.0/serverless_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 sls_sdk/lib/error.py
 sls_sdk/lib/error_captured_event.py
 sls_sdk/lib/id.py
 sls_sdk/lib/imports.py
 sls_sdk/lib/name.py
 sls_sdk/lib/notice.py
 sls_sdk/lib/stack_trace_string.py
+sls_sdk/lib/tag_value.py
 sls_sdk/lib/tags.py
 sls_sdk/lib/timing.py
 sls_sdk/lib/trace.py
 sls_sdk/lib/warning.py
 sls_sdk/lib/warning_captured_event.py
 sls_sdk/lib/instrumentation/__init__.py
 sls_sdk/lib/instrumentation/flask.py
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/__init__.py` & `serverless-sdk-0.5.0/sls_sdk/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from __future__ import annotations
-import sys
-from os import environ
-from typing import List, Optional
-from typing_extensions import Final
-from types import SimpleNamespace
+
+from .lib.imports import internally_imported
+
+with internally_imported():
+    import sys
+    from os import environ
+    from typing import List, Optional
+
+    if sys.version_info >= (3, 8):
+        from typing import Final
+    else:
+        from typing_extensions import Final
+    from types import SimpleNamespace
 
 from .base import Nanoseconds, SLS_ORG_ID, __version__, __name__
 from .lib import trace
 from .lib.emitter import event_emitter, EventEmitter
 from .lib.tags import Tags, ValidTags
 from .lib.error_captured_event import create as create_error_captured_event
 from .lib.warning_captured_event import create as create_warning_captured_event
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/exceptions.py` & `serverless-sdk-0.5.0/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.9/sls_sdk/lib/captured_event.py` & `serverless-sdk-0.5.0/sls_sdk/lib/captured_event.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 from __future__ import annotations
-from typing import List, Optional
-import time
-import json
-from backports.cached_property import cached_property  # available in Python >=3.8
-from typing_extensions import Final
+
+from .imports import internally_imported
+
+with internally_imported():
+    from typing import List, Optional
+    import time
+    import json
+    from backports.cached_property import cached_property  # available in Python >=3.8
+    import sys
+
+    if sys.version_info >= (3, 8):
+        from typing import Final
+    else:
+        from typing_extensions import Final
+
 from .timing import to_protobuf_epoch_timestamp
 from .id import generate_id
 from .name import get_resource_name
 from .tags import Tags, convert_tags_to_protobuf
 from .trace import TraceSpan
 from ..exceptions import FutureEventTimestamp
 from .emitter import event_emitter
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/lib/error.py` & `serverless-sdk-0.5.0/sls_sdk/lib/error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import os
-from builtins import type as builtins_type
+from .imports import internally_imported
 from .stack_trace_string import resolve as resolve_stack_trace_string
 
-import logging
+with internally_imported():
+    import os
+    from builtins import type as builtins_type
+    import logging
 
 
 logger = logging.getLogger(__name__)
 
 
 def report(error, type: str = "INTERNAL"):
     if os.environ.get("SLS_CRASH_ON_SDK_ERROR", None):
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/lib/error_captured_event.py` & `serverless-sdk-0.5.0/sls_sdk/lib/warning_captured_event.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,65 @@
-import logging
-import time
-from builtins import type as builtins_type
-from typing import Optional
+from .imports import internally_imported
+
+with internally_imported():
+    import logging
+    import time
+    from typing import Optional
+
 from .tags import Tags
 from .captured_event import CapturedEvent
 from .stack_trace_string import resolve as resolve_stack_trace_string
 
 
 logger = logging.getLogger(__name__)
 
 
 TYPE_MAP = {
-    "unhandled": 1,
-    "handledUser": 2,
-    "handledSdkUser": 3,
-    "handledSdkInternal": 4,
+    "user": 1,
+    "sdkUser": 2,
+    "sdkInternal": 3,
 }
 
 
 def create(
-    error,
-    timestamp: Optional[int] = None,
+    message: str,
     tags: Optional[Tags] = None,
-    type: str = "handledUser",
-    name=None,
-    stack=None,
+    type: str = "user",
     origin: Optional[str] = None,
     fingerprint: Optional[str] = None,
 ):
-    timestamp = timestamp or time.perf_counter_ns()
+    timestamp = time.perf_counter_ns()
+    stack_trace = resolve_stack_trace_string()
+
     tags = tags or Tags()
     captured_event = CapturedEvent(
-        "telemetry.error.generated.v1",
+        "telemetry.warning.generated.v1",
         timestamp=timestamp,
         custom_tags=tags,
-        origin=origin,
         custom_fingerprint=fingerprint,
+        tags={
+            "warning.message": message,
+            "warning.type": TYPE_MAP[type],
+            "warning.stacktrace": stack_trace,
+        },
+        origin=origin,
     )
-    _tags = {
-        "type": TYPE_MAP[type],
-    }
-    if isinstance(error, Exception):
-        _tags["name"] = builtins_type(error).__name__
-        _tags["message"] = str(error)
-    else:
-        _tags["name"] = name or builtins_type(error).__name__
-        _tags["message"] = str(error)
-    _tags["stacktrace"] = stack or resolve_stack_trace_string(error)
-    captured_event.tags.update(_tags, prefix="error")
-
     # to avoid circular dependency, require inline
     from .. import serverlessSdk
 
     if (
         origin == "pythonLogging"
-        or type != "handledUser"
+        or type != "user"
         or serverlessSdk._settings.disable_captured_events_stdout
     ):
         return captured_event
 
-    error_log_data = {
+    warn_log_data = {
         "source": "serverlessSdk",
-        "type": "ERROR_TYPE_CAUGHT_USER",
-        "name": _tags["name"],
-        "message": _tags["message"],
-        "stack": _tags["stacktrace"],
+        "type": "WARNING_TYPE_USER",
+        "message": message,
+        "stack": stack_trace,
     }
     if fingerprint:
-        error_log_data["fingerprint"] = fingerprint
-    logger.error(error_log_data)
+        warn_log_data["fingerprint"] = fingerprint
+    logger.warning(warn_log_data)
     return captured_event
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/flask.py` & `serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/flask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-import re
 from sls_sdk import serverlessSdk
+
+from ..imports import internally_imported
+
+with internally_imported():
+    import re
+    from functools import partial
+
 from ..error import report as report_error
-from functools import partial
 from .import_hook import ImportHook
 
 _instrumenter = None
 _import_hook = ImportHook("flask")
 
 
 class Instrumenter:
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/http.py` & `serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from __future__ import annotations
-import time
-import contextvars
-import contextlib
-from urllib.parse import urlparse
-from urllib.parse import parse_qs
+
+import sls_sdk
+
+from ..imports import internally_imported
+
+with internally_imported():
+    import time
+    import contextvars
+    import contextlib
+    from urllib.parse import urlparse
+    from urllib.parse import parse_qs
+    import io
+    from typing import Iterable
+
 from ..error import report as report_error
 from .import_hook import ImportHook
-import sls_sdk
 from .wrapper import replace_method
-import io
-from typing import Iterable
+
 
 SDK = sls_sdk.serverlessSdk
 _IGNORE_FOLLOWING_REQUEST = contextvars.ContextVar("ignore", default=False)
 
 
 def ignore_following_request():
     _IGNORE_FOLLOWING_REQUEST.set(True)
@@ -393,37 +400,50 @@
             self._capture_request_body(trace_span, body)
 
             with URLLib3Instrumenter._prevent_recursive_instrumentation():
                 response = actual_url_open(*args, **kwargs)
 
                 trace_span.tags["http.status_code"] = response.status
                 self._capture_response_body(trace_span, response)
-
                 return response
         except Exception as ex:
             trace_span.tags["http.error_code"] = ex.__class__.__name__
             raise
         finally:
             if trace_span.end_time is None:
                 trace_span.close()
 
     def _capture_response_body(self, trace_span, response):
         if not self.should_monitor_request_response:
             return
-        response_body = response.data
+
         response_length = int(response.headers.get("Content-Length", 0))
         if response_length > SDK._maximum_body_byte_length:
             SDK._report_notice(
                 "Large body excluded",
                 "OUTPUT_BODY_TOO_LARGE",
                 trace_span,
             )
             return
+
+        response_body = None
+        # if data is peekable, use it instead of the response.data
+        # this makes sure the response body is not consumed when
+        # instrumenting http requests through "requests" library.
+        if (
+            hasattr(response, "_original_response")
+            and hasattr(response._original_response, "peek")
+            and callable(response._original_response.peek)
+        ):
+            response_body = response._original_response.peek()
+            length = len(response_body)
+            if length == 0 and length != response_length:
+                response_body = response.data
         try:
-            if response_body:
+            if response_body is not None:
                 trace_span.output = _decode_body(response_body)
         except Exception as ex:
             report_error(ex)
 
     def _install(self, module):
         self._module = module
         replace_method(
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/import_hook.py` & `serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/import_hook.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-import sys
-from importlib.machinery import PathFinder, SourceFileLoader
+from ..imports import internally_imported
+
+with internally_imported():
+    import sys
+    from importlib.machinery import PathFinder, SourceFileLoader
 
 
 class CustomImporter:
     def __init__(self, module_name, hook_fn=None):
         self._hook_fn = hook_fn
         self._module_name = module_name
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from logging import Logger
-import json
+
+from ..imports import internally_imported
+
+with internally_imported():
+    import json
 
 from ..error import report as report_error
 from ..error_captured_event import create as create_error_captured_event
 from ..warning_captured_event import create as create_warning_captured_event
 
 
 _is_installed = False
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/wrapper.py` & `serverless-sdk-0.5.0/sls_sdk/lib/instrumentation/wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from functools import partial
+from ..imports import internally_imported
+
+with internally_imported():
+    from functools import partial
 
 
 class ReplacementMethod(object):
     def __init__(self, class_, method_name, target_method) -> None:
         self.class_ = class_
         self.method_name = method_name
         self.target_method = target_method
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/lib/name.py` & `serverless-sdk-0.5.0/sls_sdk/lib/name.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from __future__ import annotations
-from re import Pattern
+
 from .imports import internally_imported
 
-with internally_imported("js_regex"):
+with internally_imported():
+    from re import Pattern
     from js_regex import compile
+    import sys
+
+    if sys.version_info >= (3, 8):
+        from typing import Final
+    else:
+        from typing_extensions import Final
 
-from typing_extensions import Final
 from ..exceptions import InvalidTraceSpanName
 
 
 # from https://github.com/serverless/console/blob/main/node/packages/sdk/lib/get-ensure-resource-name.js#L7
 RE: Final[str] = (
     r"^[a-z][a-z0-9]*"
     r"(?:_[a-z][a-z0-9]*)*"
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/lib/stack_trace_string.py` & `serverless-sdk-0.5.0/sls_sdk/lib/stack_trace_string.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-import traceback
-import sys
-import inspect
-from typing import Optional, Any
+from .imports import internally_imported
+
+with internally_imported():
+    import traceback
+    import sys
+    import inspect
+    from typing import Optional, Any
 
 
 def resolve(error: Optional[Any] = None) -> str:
     if isinstance(error, BaseException):
         # in case of an actual Exception, stack trace is already set up.
         return "".join(traceback.format_exception(None, error, error.__traceback__))
     else:
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/lib/tags.py` & `serverless-sdk-0.5.0/sls_sdk/lib/tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 from __future__ import annotations
-import re
-from datetime import datetime
-from math import inf, nan
-from re import Pattern
-from typing import Dict, List, Mapping, Tuple, Optional, Any
+
 from .imports import internally_imported
 
-with internally_imported("js_regex"):
+with internally_imported():
+    import re
+    from datetime import datetime
+    import json
+    from math import inf, nan
+    from re import Pattern
+    from typing import Dict, List, Mapping, Tuple, Optional, Any
     from js_regex import compile
+    import sys
+
+    if sys.version_info >= (3, 8):
+        from typing import Final, get_args
+    else:
+        from typing_extensions import Final, get_args
+    from threading import Lock
 
-from typing_extensions import Final, get_args
-from threading import Lock
+from .tag_value import MAX_VALUE_LENGTH
 from .error import report as report_error
 from ..base import TagType, ValidTags
 from ..exceptions import (
     DuplicateTraceSpanName,
     InvalidTraceSpanTagName,
     InvalidTraceSpanTagValue,
     SdkException,
 )
 
-# from https://github.com/serverless/console/blob/fe64a4f53529285e89a64f7d50ec9528a3c4ce57/node/packages/sdk/lib/tags.js#L12
-RE: Final[str] = r"^[a-zA-Z0-9_.-]+$"
+RE: Final[str] = r"^[a-zA-Z0-9_.-]{1,256}$"
 RE_C: Final[Pattern] = compile(RE)
 
 
 class Tags(Dict[str, ValidTags]):
     def __init__(self):
         super().__init__()
         self._lock = Lock()
@@ -122,31 +129,35 @@
     raise InvalidTraceSpanTagName(
         f"Invalid trace span tag {name}: {name.capitalize()} "
         f"should contain dot separated tokens that follow "
         f'"[a-z][a-z0-9_]*" pattern. Received {name}'
     )
 
 
-def ensure_tag_value(attr: str, value: ValidTags) -> ValidTags:
+def _ensure_singular_tag_value(attr: str, value: TagType) -> TagType:
     valid_types: Tuple[type] = get_args(TagType)  # type: ignore
-    valid_types = (*valid_types, list)  # type: ignore
 
     if not isinstance(value, valid_types):
         raise InvalidTraceSpanTagValue(
             f"Invalid trace span tag value for {attr}: "
             f"Expected {valid_types}, received {value}"
         )
 
     if isinstance(value, datetime):
         return value.isoformat()
 
     if isinstance(value, str) and is_date(value):
         return value
 
     elif isinstance(value, str):
+        if len(value.encode()) > MAX_VALUE_LENGTH:
+            raise InvalidTraceSpanTagValue(
+                f"Invalid trace span tag value for {attr}: "
+                f"Too large string: {value}"
+            )
         return value
 
     elif isinstance(value, (int, float)):
         invalid = inf, -inf, nan
 
         if value in invalid:
             raise InvalidTraceSpanTagValue(
@@ -155,26 +166,33 @@
             )
 
         return value
 
     elif isinstance(value, bool):
         return value
 
-    if isinstance(value, List):
-        valid: bool = all(ensure_tag_value("tags", item) is not None for item in value)
-
-        if valid:
-            return value
-
     raise InvalidTraceSpanTagValue(
         f"Invalid trace span tag value for {attr}: "
         f"Expected {valid_types}, received {value}"
     )
 
 
+def ensure_tag_value(attr: str, value: ValidTags) -> ValidTags:
+    if isinstance(value, List):
+        normalized_value = [_ensure_singular_tag_value("tags", item) for item in value]
+        if len(json.dumps(normalized_value, default=str).encode()) > MAX_VALUE_LENGTH:
+            raise InvalidTraceSpanTagValue(
+                f"Invalid trace span tag value for {attr}: "
+                f"Too large string: {value}"
+            )
+        return normalized_value
+    else:
+        return _ensure_singular_tag_value(attr, value)
+
+
 def _snake_to_camel_case(string):
     return re.sub(r"_(.)", lambda match: match.group(1).upper(), string)
 
 
 def convert_tags_to_protobuf(tags: Tags):
     protobuf_tags: Any = {}
     for key, value in tags.items():
```

### Comparing `serverless-sdk-0.4.9/sls_sdk/lib/trace.py` & `serverless-sdk-0.5.0/sls_sdk/lib/trace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 from __future__ import annotations
-from collections.abc import Iterable
-import logging
-import time
-import threading
-from typing import List, Optional, Callable
-from contextvars import ContextVar
-from backports.cached_property import cached_property  # available in Python >=3.8
-from typing_extensions import Final
-import json
+
+from .imports import internally_imported
+
+with internally_imported():
+    from collections.abc import Iterable
+    import time
+    import threading
+    from typing import List, Optional, Callable
+    from contextvars import ContextVar
+    from backports.cached_property import cached_property  # available in Python >=3.8
+    import sys
+
+    if sys.version_info >= (3, 8):
+        from typing import Final
+    else:
+        from typing_extensions import Final
+
+    import json
+
 from .instrumentation.import_hook import ImportHook
 from .timing import to_protobuf_epoch_timestamp
 from ..base import Nanoseconds, TraceId
 from ..exceptions import (
     ClosureOnClosedSpan,
     FutureSpanStartTime,
     InvalidType,
@@ -21,16 +31,14 @@
 )
 from .emitter import event_emitter
 from .id import generate_id
 from .name import get_resource_name
 from .tags import Tags, convert_tags_to_protobuf
 from .instrumentation.wrapper import replace_method
 
-logger = logging.getLogger(__name__)
-
 
 __all__: Final[List[str]] = [
     "TraceSpan",
 ]
 
 
 TraceSpanContext = ContextVar[Optional["TraceSpan"]]
@@ -224,17 +232,21 @@
                     if sub_span._on_close_by_root:
                         sub_span._on_close_by_root()
                     sub_span.close(end_time=self.end_time)
                     left_over_spans.append(sub_span)
 
             if left_over_spans:
                 spans = ", ".join([s.name for s in left_over_spans])
-                logger.error(
+                from .. import serverlessSdk
+
+                serverlessSdk._report_warning(
                     "Serverless SDK Warning: Following trace spans didn't end before"
-                    + f" end of lambda invocation: {spans}"
+                    + f" end of lambda invocation: {spans}",
+                    "SDK_SPAN_NOT_CLOSED",
+                    "USER",
                 )
             _CONTEXT.set(self)
         else:
             # if this is not the root span and context points to this
             # then we need to reset the context to the first open ancestor span
             current = _CONTEXT.get()
             if self is current:
```

### Comparing `serverless-sdk-0.4.9/tests/test_sdk.py` & `serverless-sdk-0.5.0/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.9/tests/test_thread_safety.py` & `serverless-sdk-0.5.0/tests/test_thread_safety.py`

 * *Files identical despite different names*

