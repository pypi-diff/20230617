# Comparing `tmp/motion_python-0.1.65.tar.gz` & `tmp/motion_python-0.1.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.65.tar", max compression
+gzip compressed data, was "motion_python-0.1.66.tar", max compression
```

## Comparing `motion_python-0.1.65.tar` & `motion_python-0.1.66.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-15 21:58:24.341203 motion_python-0.1.65/README.md
--rw-r--r--   0        0        0      276 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/cli.py
--rw-r--r--   0        0        0    23922 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/component.py
--rw-r--r--   0        0        0    17554 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/execute.py
--rw-r--r--   0        0        0    12849 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      619 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/route.py
--rw-r--r--   0        0        0     5815 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/server/fit_task.py
--rw-r--r--   0        0        0     8853 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-06-15 21:58:45.189559 motion_python-0.1.65/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.65/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-17 07:58:41.152077 motion_python-0.1.66/README.md
+-rw-r--r--   0        0        0      276 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/cli.py
+-rw-r--r--   0        0        0    23922 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/component.py
+-rw-r--r--   0        0        0    17554 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/execute.py
+-rw-r--r--   0        0        0    12849 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      619 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/route.py
+-rw-r--r--   0        0        0     5944 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/server/fit_task.py
+-rw-r--r--   0        0        0     9082 2023-06-17 07:58:41.152077 motion_python-0.1.66/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-06-17 07:58:59.924236 motion_python-0.1.66/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.66/PKG-INFO
```

### Comparing `motion_python-0.1.65/README.md` & `motion_python-0.1.66/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.65/motion/cli.py` & `motion_python-0.1.66/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.65/motion/component.py` & `motion_python-0.1.66/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.65/motion/execute.py` & `motion_python-0.1.66/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.65/motion/instance.py` & `motion_python-0.1.66/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.65/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.66/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.65/motion/route.py` & `motion_python-0.1.66/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.65/motion/server/fit_task.py` & `motion_python-0.1.66/motion/server/fit_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,15 @@
                 if not job["identifier"].startswith("NOOP_"):
                     values.append(job["value"])
                     infer_results.append(job["infer_result"])
                 identifiers.append(job["identifier"])
 
             # Check that there are elements in values and infer_results
             # Acquire lock and run op
+            exception_str = ""
             if len(values) >= 1:
                 acquired_lock = lock.acquire(blocking=True)
                 if acquired_lock:
                     try:
                         old_state = loadState(
                             redis_con, self.instance_name, self.load_state_func
                         )
@@ -128,26 +129,27 @@
                             saveState(
                                 old_state,
                                 redis_con,
                                 self.instance_name,
                                 self.save_state_func,
                             )
                     except Exception as e:
-                        logger.error(f"Error in {self.queue_identifier} fit: {e}")
+                        # logger.error(f"Error in {self.queue_identifier} fit: {e}")
                         logger.error(traceback.format_exc())
+                        exception_str = str(e)
                     finally:
                         logger.info("Releasing lock.")
                         lock.release()
                 else:
                     logger.error("Lock not acquired; batch lost.")
 
             for identifier in identifiers:
                 redis_con.publish(
                     self.channel_identifier,
-                    identifier,
+                    str({"identifier": identifier, "exception": exception_str}),
                 )
 
             # Clear batch
             self.batch = []
 
     def cleanup(self) -> None:
         redis_con = redis.Redis(
```

### Comparing `motion_python-0.1.65/motion/utils.py` & `motion_python-0.1.66/motion/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,19 +231,28 @@
         self.channel = channel
         self.pubsub = redis_con.pubsub()
         self.identifier = identifier
         self.pubsub.subscribe(channel)
 
     def wait(self) -> None:
         for message in self.pubsub.listen():
-            if (
-                message["type"] == "message"
-                and message["data"].decode() == self.identifier
-            ):
-                break
+            if message["type"] != "message":
+                continue
+
+            error_data = eval(message["data"])
+            identifier = error_data["identifier"]
+            exception_str = error_data["exception"]
+
+            if identifier != self.identifier:
+                continue
+
+            if exception_str:
+                raise RuntimeError(exception_str)
+
+            break
 
 
 class FitEventGroup:
     """Stores the events for fit operations on a given key."""
 
     def __init__(self, key: str) -> None:
         self.key = key
```

### Comparing `motion_python-0.1.65/pyproject.toml` & `motion_python-0.1.66/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.65"
+version = "0.1.66"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.65/PKG-INFO` & `motion_python-0.1.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.65
+Version: 0.1.66
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

