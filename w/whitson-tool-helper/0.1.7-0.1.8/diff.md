# Comparing `tmp/whitson_tool_helper-0.1.7.tar.gz` & `tmp/whitson_tool_helper-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/markus/Documents/BitBucket/whitson-tool-helper/dist/.tmp-v15_p695/whitson_tool_helper-0.1.7.tar", last modified: Mon Jun 12 08:07:42 2023, max compression
+gzip compressed data, was "/home/markus/Documents/BitBucket/whitson-tool-helper/dist/.tmp-gzk2loz2/whitson_tool_helper-0.1.8.tar", last modified: Sat Jun 17 16:29:58 2023, max compression
```

## Comparing `whitson_tool_helper-0.1.7.tar` & `whitson_tool_helper-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-12 08:07:42.000000 whitson_tool_helper-0.1.7/
--rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-06-12 08:07:42.000000 whitson_tool_helper-0.1.7/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      705 2023-06-12 08:07:35.000000 whitson_tool_helper-0.1.7/pyproject.toml
--rw-rw-r--   0 markus    (1000) markus    (1000)       38 2023-06-12 08:07:42.000000 whitson_tool_helper-0.1.7/setup.cfg
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-12 08:07:42.000000 whitson_tool_helper-0.1.7/src/
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-12 08:07:42.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper/
--rw-rw-r--   0 markus    (1000) markus    (1000)      107 2023-04-26 09:25:11.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)       66 2023-04-26 13:06:47.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper/logger.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-12 08:07:42.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper/messaging/
--rw-rw-r--   0 markus    (1000) markus    (1000)      370 2023-05-28 08:36:59.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper/messaging/helper.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     2729 2023-05-29 07:32:28.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper/messaging/main.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3746 2023-06-12 08:05:49.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper/messaging/pubsub.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3648 2023-05-29 07:34:29.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper/messaging/rabbitmq.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      574 2023-04-25 15:19:43.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper/timeout.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      704 2023-04-26 12:57:07.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper/whitson_exceptions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-12 08:07:42.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper.egg-info/
--rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-06-12 08:07:42.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      575 2023-06-12 08:07:42.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-06-12 08:07:42.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)      116 2023-06-12 08:07:42.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       20 2023-06-12 08:07:42.000000 whitson_tool_helper-0.1.7/src/whitson_tool_helper.egg-info/top_level.txt
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      705 2023-06-17 16:25:45.000000 whitson_tool_helper-0.1.8/pyproject.toml
+-rw-rw-r--   0 markus    (1000) markus    (1000)       38 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/setup.cfg
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      107 2023-04-26 09:25:11.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)       66 2023-04-26 13:06:47.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/logger.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      370 2023-05-28 08:36:59.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/helper.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     2729 2023-05-29 07:32:28.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/main.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3746 2023-06-12 08:05:49.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/pubsub.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3652 2023-06-17 16:24:47.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/rabbitmq.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      574 2023-04-25 15:19:43.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/timeout.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      704 2023-04-26 12:57:07.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/whitson_exceptions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      575 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)      116 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       20 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/top_level.txt
```

### Comparing `whitson_tool_helper-0.1.7/pyproject.toml` & `whitson_tool_helper-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whitson_tool_helper"
-version =  "0.1.7"
+version =  "0.1.8"
 authors = [
   { name="Markus Blytt", email="blytt@whitson.com" },
   { name="Jason Hu", email="jason@whitson.com" },
   { name="Arnaud Hoffmann", email="arnaud@whitson.com" },
 ]
 description = "A Toolbox for whitson cloud software solutions"
 dependencies = ["pika==1.3.1", "google-auth==2.16.0","google-cloud-pubsub==2.14.0", "google-cloud-storage==2.7.0","google-cloud-logging==3.5.0"]
```

### Comparing `whitson_tool_helper-0.1.7/src/whitson_tool_helper/messaging/main.py` & `whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/main.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.7/src/whitson_tool_helper/messaging/pubsub.py` & `whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/pubsub.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.7/src/whitson_tool_helper/messaging/rabbitmq.py` & `whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/rabbitmq.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     def publish_many(self, topic, payloads: List[dict], priority: int = 50):
         connection = pika.BlockingConnection(self.parameters)
         channel = connection.channel()
 
         for message in payloads:
             channel.basic_publish(
-                exchange="engines",
+                exchange=self.exchange,
                 routing_key=topic,
                 body=json.dumps(message).encode("utf-8"),
                 properties=pika.BasicProperties(
                     delivery_mode=pika.spec.PERSISTENT_DELIVERY_MODE,
                     priority=priority,
                 ),
             )
```

### Comparing `whitson_tool_helper-0.1.7/src/whitson_tool_helper/timeout.py` & `whitson_tool_helper-0.1.8/src/whitson_tool_helper/timeout.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.7/src/whitson_tool_helper/whitson_exceptions.py` & `whitson_tool_helper-0.1.8/src/whitson_tool_helper/whitson_exceptions.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.7/src/whitson_tool_helper.egg-info/SOURCES.txt` & `whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

