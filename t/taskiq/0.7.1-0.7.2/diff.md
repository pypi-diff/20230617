# Comparing `tmp/taskiq-0.7.1.tar.gz` & `tmp/taskiq-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-0.7.1.tar", max compression
+gzip compressed data, was "taskiq-0.7.2.tar", max compression
```

## Comparing `taskiq-0.7.1.tar` & `taskiq-0.7.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1075 2023-06-11 13:52:14.706527 taskiq-0.7.1/LICENSE
--rw-r--r--   0        0        0     1875 2023-06-11 13:52:14.706527 taskiq-0.7.1/README.md
--rw-r--r--   0        0        0     2879 2023-06-11 13:52:14.710527 taskiq-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2161 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/__init__.py
--rw-r--r--   0        0        0     2093 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/__main__.py
--rw-r--r--   0        0        0      194 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/__init__.py
--rw-r--r--   0        0        0    12576 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/broker.py
--rw-r--r--   0        0        0      323 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/cmd.py
--rw-r--r--   0        0        0      629 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/formatter.py
--rw-r--r--   0        0        0     3002 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/middleware.py
--rw-r--r--   0        0        0     1376 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/result_backend.py
--rw-r--r--   0        0        0     1084 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/abc/schedule_source.py
--rw-r--r--   0        0        0      496 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/acks.py
--rw-r--r--   0        0        0       34 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/brokers/__init__.py
--rw-r--r--   0        0        0     5679 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/brokers/inmemory_broker.py
--rw-r--r--   0        0        0     2197 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/brokers/shared_broker.py
--rw-r--r--   0        0        0     2514 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/brokers/zmq_broker.py
--rw-r--r--   0        0        0       31 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/__init__.py
--rw-r--r--   0        0        0      197 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/common_args.py
--rw-r--r--   0        0        0       37 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/scheduler/__init__.py
--rw-r--r--   0        0        0     1990 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/scheduler/args.py
--rw-r--r--   0        0        0      651 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/scheduler/cmd.py
--rw-r--r--   0        0        0     3998 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/scheduler/run.py
--rw-r--r--   0        0        0     2550 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/utils.py
--rw-r--r--   0        0        0     1517 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/watcher.py
--rw-r--r--   0        0        0       43 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/worker/__init__.py
--rw-r--r--   0        0        0     6060 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/worker/args.py
--rw-r--r--   0        0        0      628 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/worker/cmd.py
--rw-r--r--   0        0        0     1742 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/worker/log_collector.py
--rw-r--r--   0        0        0     7497 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/worker/process_manager.py
--rw-r--r--   0        0        0     6163 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/cli/worker/run.py
--rw-r--r--   0        0        0     1300 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/context.py
--rw-r--r--   0        0        0     2930 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/decor.py
--rw-r--r--   0        0        0      511 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/events.py
--rw-r--r--   0        0        0     1010 2023-06-11 13:52:14.710527 taskiq-0.7.1/taskiq/exceptions.py
--rw-r--r--   0        0        0       25 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/formatters/__init__.py
--rw-r--r--   0        0        0      844 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/formatters/json_formatter.py
--rw-r--r--   0        0        0     1887 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/funcs.py
--rw-r--r--   0        0        0     5552 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/kicker.py
--rw-r--r--   0        0        0      507 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/message.py
--rw-r--r--   0        0        0       26 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/middlewares/__init__.py
--rw-r--r--   0        0        0     4315 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/middlewares/prometheus_middleware.py
--rw-r--r--   0        0        0     2438 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/middlewares/retry_middleware.py
--rw-r--r--   0        0        0        0 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/py.typed
--rw-r--r--   0        0        0      113 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/receiver/__init__.py
--rw-r--r--   0        0        0     2795 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/receiver/params_parser.py
--rw-r--r--   0        0        0    12566 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/receiver/receiver.py
--rw-r--r--   0        0        0     2020 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/result.py
--rw-r--r--   0        0        0       35 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/result_backends/__init__.py
--rw-r--r--   0        0        0     1268 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/result_backends/dummy.py
--rw-r--r--   0        0        0      146 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/schedule_sources/__init__.py
--rw-r--r--   0        0        0     1520 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/schedule_sources/label_based.py
--rw-r--r--   0        0        0      264 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/scheduler/__init__.py
--rw-r--r--   0        0        0     1056 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/scheduler/merge_functions.py
--rw-r--r--   0        0        0     1717 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/scheduler/scheduler.py
--rw-r--r--   0        0        0    11302 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/serialization.py
--rw-r--r--   0        0        0     1071 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/state.py
--rw-r--r--   0        0        0     4141 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/task.py
--rw-r--r--   0        0        0      900 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/utils.py
--rw-r--r--   0        0        0      106 2023-06-11 13:52:14.714527 taskiq-0.7.1/taskiq/warnings.py
--rw-r--r--   0        0        0     3608 1970-01-01 00:00:00.000000 taskiq-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-17 16:32:30.737189 taskiq-0.7.2/LICENSE
+-rw-r--r--   0        0        0     1875 2023-06-17 16:32:30.737189 taskiq-0.7.2/README.md
+-rw-r--r--   0        0        0     2879 2023-06-17 16:32:30.741189 taskiq-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2161 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/__init__.py
+-rw-r--r--   0        0        0     2093 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/__main__.py
+-rw-r--r--   0        0        0      194 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/__init__.py
+-rw-r--r--   0        0        0    12576 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/broker.py
+-rw-r--r--   0        0        0      323 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/cmd.py
+-rw-r--r--   0        0        0      629 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/formatter.py
+-rw-r--r--   0        0        0     3002 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/middleware.py
+-rw-r--r--   0        0        0     1376 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/result_backend.py
+-rw-r--r--   0        0        0     1084 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/abc/schedule_source.py
+-rw-r--r--   0        0        0      496 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/acks.py
+-rw-r--r--   0        0        0       34 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/brokers/__init__.py
+-rw-r--r--   0        0        0     5679 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/brokers/inmemory_broker.py
+-rw-r--r--   0        0        0     2197 2023-06-17 16:32:30.741189 taskiq-0.7.2/taskiq/brokers/shared_broker.py
+-rw-r--r--   0        0        0     2514 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/brokers/zmq_broker.py
+-rw-r--r--   0        0        0       31 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/common_args.py
+-rw-r--r--   0        0        0       37 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/scheduler/__init__.py
+-rw-r--r--   0        0        0     1990 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/scheduler/args.py
+-rw-r--r--   0        0        0      651 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/scheduler/cmd.py
+-rw-r--r--   0        0        0     3998 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/scheduler/run.py
+-rw-r--r--   0        0        0     2550 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/utils.py
+-rw-r--r--   0        0        0     1517 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/watcher.py
+-rw-r--r--   0        0        0       43 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/worker/__init__.py
+-rw-r--r--   0        0        0     6060 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/worker/args.py
+-rw-r--r--   0        0        0      628 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/worker/cmd.py
+-rw-r--r--   0        0        0     1742 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/worker/log_collector.py
+-rw-r--r--   0        0        0     7497 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/worker/process_manager.py
+-rw-r--r--   0        0        0     6163 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/cli/worker/run.py
+-rw-r--r--   0        0        0     1251 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/context.py
+-rw-r--r--   0        0        0     2930 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/decor.py
+-rw-r--r--   0        0        0      511 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/events.py
+-rw-r--r--   0        0        0     1010 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/exceptions.py
+-rw-r--r--   0        0        0       25 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/formatters/__init__.py
+-rw-r--r--   0        0        0      844 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1887 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/funcs.py
+-rw-r--r--   0        0        0     5552 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/kicker.py
+-rw-r--r--   0        0        0      507 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/message.py
+-rw-r--r--   0        0        0       26 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/middlewares/__init__.py
+-rw-r--r--   0        0        0     4315 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/middlewares/prometheus_middleware.py
+-rw-r--r--   0        0        0     2438 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/middlewares/retry_middleware.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/py.typed
+-rw-r--r--   0        0        0      113 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/receiver/__init__.py
+-rw-r--r--   0        0        0     2795 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/receiver/params_parser.py
+-rw-r--r--   0        0        0    12601 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/receiver/receiver.py
+-rw-r--r--   0        0        0     2084 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/result.py
+-rw-r--r--   0        0        0       35 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/result_backends/__init__.py
+-rw-r--r--   0        0        0     1268 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/result_backends/dummy.py
+-rw-r--r--   0        0        0      146 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/schedule_sources/__init__.py
+-rw-r--r--   0        0        0     1520 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/schedule_sources/label_based.py
+-rw-r--r--   0        0        0      264 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/scheduler/__init__.py
+-rw-r--r--   0        0        0     1056 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/scheduler/merge_functions.py
+-rw-r--r--   0        0        0     1717 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/scheduler/scheduler.py
+-rw-r--r--   0        0        0    11302 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/serialization.py
+-rw-r--r--   0        0        0     1071 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/state.py
+-rw-r--r--   0        0        0     4141 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/task.py
+-rw-r--r--   0        0        0      900 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/utils.py
+-rw-r--r--   0        0        0      106 2023-06-17 16:32:30.745189 taskiq-0.7.2/taskiq/warnings.py
+-rw-r--r--   0        0        0     3608 1970-01-01 00:00:00.000000 taskiq-0.7.2/PKG-INFO
```

### Comparing `taskiq-0.7.1/LICENSE` & `taskiq-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/README.md` & `taskiq-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/pyproject.toml` & `taskiq-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq"
-version = "0.7.1"
+version = "0.7.2"
 description = "Distributed task queue with full async support"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 maintainers = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq"
 homepage = "https://taskiq-python.github.io/"
 documentation = "https://taskiq-python.github.io/"
```

### Comparing `taskiq-0.7.1/taskiq/__init__.py` & `taskiq-0.7.2/taskiq/__init__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/__main__.py` & `taskiq-0.7.2/taskiq/__main__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/abc/broker.py` & `taskiq-0.7.2/taskiq/abc/broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/abc/formatter.py` & `taskiq-0.7.2/taskiq/abc/formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/abc/middleware.py` & `taskiq-0.7.2/taskiq/abc/middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/abc/result_backend.py` & `taskiq-0.7.2/taskiq/abc/result_backend.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/abc/schedule_source.py` & `taskiq-0.7.2/taskiq/abc/schedule_source.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/brokers/inmemory_broker.py` & `taskiq-0.7.2/taskiq/brokers/inmemory_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/brokers/shared_broker.py` & `taskiq-0.7.2/taskiq/brokers/shared_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/brokers/zmq_broker.py` & `taskiq-0.7.2/taskiq/brokers/zmq_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/cli/scheduler/args.py` & `taskiq-0.7.2/taskiq/cli/scheduler/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/cli/scheduler/cmd.py` & `taskiq-0.7.2/taskiq/cli/scheduler/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/cli/scheduler/run.py` & `taskiq-0.7.2/taskiq/cli/scheduler/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/cli/utils.py` & `taskiq-0.7.2/taskiq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/cli/watcher.py` & `taskiq-0.7.2/taskiq/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/cli/worker/args.py` & `taskiq-0.7.2/taskiq/cli/worker/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/cli/worker/cmd.py` & `taskiq-0.7.2/taskiq/cli/worker/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/cli/worker/log_collector.py` & `taskiq-0.7.2/taskiq/cli/worker/log_collector.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/cli/worker/process_manager.py` & `taskiq-0.7.2/taskiq/cli/worker/process_manager.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/cli/worker/run.py` & `taskiq-0.7.2/taskiq/cli/worker/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/context.py` & `taskiq-0.7.2/taskiq/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from copy import copy
 from typing import TYPE_CHECKING
 
 from taskiq.abc.broker import AsyncBroker
 from taskiq.exceptions import NoResultError, TaskRejectedError
 from taskiq.message import TaskiqMessage
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -24,18 +23,17 @@
 
         This fuction creates a task with
         the same message and sends it using
         current broker.
 
         :raises NoResultError: to not store result for current task.
         """
-        message = copy(self.message)
-        requeue_count = int(message.labels.get("X-Taskiq-requeue", 0))
+        requeue_count = int(self.message.labels.get("X-Taskiq-requeue", 0))
         requeue_count += 1
-        message.labels["X-Taskiq-requeue"] = str(requeue_count)
+        self.message.labels["X-Taskiq-requeue"] = str(requeue_count)
         await self.broker.kick(self.broker.formatter.dumps(self.message))
         raise NoResultError()
 
     def reject(self) -> None:
         """
         Raise reject error.
```

### Comparing `taskiq-0.7.1/taskiq/decor.py` & `taskiq-0.7.2/taskiq/decor.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/exceptions.py` & `taskiq-0.7.2/taskiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/formatters/json_formatter.py` & `taskiq-0.7.2/taskiq/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/funcs.py` & `taskiq-0.7.2/taskiq/funcs.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/kicker.py` & `taskiq-0.7.2/taskiq/kicker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/middlewares/prometheus_middleware.py` & `taskiq-0.7.2/taskiq/middlewares/prometheus_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/middlewares/retry_middleware.py` & `taskiq-0.7.2/taskiq/middlewares/retry_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/receiver/params_parser.py` & `taskiq-0.7.2/taskiq/receiver/params_parser.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/receiver/receiver.py` & `taskiq-0.7.2/taskiq/receiver/receiver.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,15 @@
         # Assemble result.
         result: "TaskiqResult[Any]" = TaskiqResult(
             is_err=found_exception is not None,
             log=None,
             return_value=returned,
             execution_time=round(execution_time, 2),
             error=found_exception,
+            labels=message.labels,
         )
         # If exception is found we execute middlewares.
         if found_exception is not None:
             for middleware in self.broker.middlewares:
                 if middleware.__class__.on_error != TaskiqMiddleware.on_error:
                     await maybe_awaitable(
                         middleware.on_error(
```

### Comparing `taskiq-0.7.1/taskiq/result.py` & `taskiq-0.7.2/taskiq/result.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import pickle  # noqa: S403
 from functools import partial
 from typing import Any, Callable, Dict, Generic, Optional, TypeVar
 
-from pydantic import validator
+from pydantic import Field, validator
 from pydantic.generics import GenericModel
 from typing_extensions import Self
 
 from taskiq.serialization import exception_to_python, prepare_exception
 
 _ReturnType = TypeVar("_ReturnType")
 
@@ -29,14 +29,15 @@
     is_err: bool
     # Log is a deprecated field. It would be removed in future
     # releases of not, if we find a way to capture logs in async
     # environment.
     log: Optional[str] = None
     return_value: _ReturnType
     execution_time: float
+    labels: Dict[str, str] = Field(default_factory=dict)
 
     error: Optional[BaseException] = None
 
     class Config:
         arbitrary_types_allowed = True
         json_dumps = _json_dumps  # type: ignore
         json_loads = json.loads
```

### Comparing `taskiq-0.7.1/taskiq/result_backends/dummy.py` & `taskiq-0.7.2/taskiq/result_backends/dummy.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/schedule_sources/label_based.py` & `taskiq-0.7.2/taskiq/schedule_sources/label_based.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/scheduler/merge_functions.py` & `taskiq-0.7.2/taskiq/scheduler/merge_functions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/scheduler/scheduler.py` & `taskiq-0.7.2/taskiq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/serialization.py` & `taskiq-0.7.2/taskiq/serialization.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/state.py` & `taskiq-0.7.2/taskiq/state.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/task.py` & `taskiq-0.7.2/taskiq/task.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/taskiq/utils.py` & `taskiq-0.7.2/taskiq/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.7.1/PKG-INFO` & `taskiq-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq
-Version: 0.7.1
+Version: 0.7.2
 Summary: Distributed task queue with full async support
 Home-page: https://taskiq-python.github.io/
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Maintainer: Pavel Kirilin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskiq Version: 0.7.1 Summary: Distributed task
+Metadata-Version: 2.1 Name: taskiq Version: 0.7.2 Summary: Distributed task
 queue with full async support Home-page: https://taskiq-python.github.io/
 License: LICENSE Keywords: taskiq,tasks,distributed,async Author: Pavel Kirilin
 Author-email: win10@list.ru Maintainer: Pavel Kirilin Maintainer-email:
 win10@list.ru Requires-Python: >=3.8.1,<4.0.0 Classifier: Development Status ::
 3 - Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 Other/Proprietary License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

