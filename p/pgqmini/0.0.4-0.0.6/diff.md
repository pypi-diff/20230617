# Comparing `tmp/pgqmini-0.0.4.tar.gz` & `tmp/pgqmini-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqmini-0.0.4.tar", last modified: Sat Jun 17 05:14:51 2023, max compression
+gzip compressed data, was "pgqmini-0.0.6.tar", last modified: Sat Jun 17 05:30:31 2023, max compression
```

## Comparing `pgqmini-0.0.4.tar` & `pgqmini-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-17 05:14:51.132916 pgqmini-0.0.4/
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     1070 2023-06-15 16:54:52.000000 pgqmini-0.0.4/LICENSE
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2385 2023-06-17 05:14:51.132916 pgqmini-0.0.4/PKG-INFO
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2054 2023-06-17 05:12:41.000000 pgqmini-0.0.4/README.md
-drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-17 05:14:51.132916 pgqmini-0.0.4/pgqmini/
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       40 2023-06-16 14:18:20.000000 pgqmini-0.0.4/pgqmini/__init__.py
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)    11588 2023-06-17 04:27:13.000000 pgqmini-0.0.4/pgqmini/pgq.py
-drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-17 05:14:51.132916 pgqmini-0.0.4/pgqmini.egg-info/
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2385 2023-06-17 05:14:51.000000 pgqmini-0.0.4/pgqmini.egg-info/PKG-INFO
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      245 2023-06-17 05:14:51.000000 pgqmini-0.0.4/pgqmini.egg-info/SOURCES.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-17 05:14:51.000000 pgqmini-0.0.4/pgqmini.egg-info/dependency_links.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-17 05:14:51.000000 pgqmini-0.0.4/pgqmini.egg-info/not-zip-safe
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       16 2023-06-17 05:14:51.000000 pgqmini-0.0.4/pgqmini.egg-info/requires.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        8 2023-06-17 05:14:51.000000 pgqmini-0.0.4/pgqmini.egg-info/top_level.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       38 2023-06-17 05:14:51.132916 pgqmini-0.0.4/setup.cfg
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      582 2023-06-17 05:12:35.000000 pgqmini-0.0.4/setup.py
+drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-17 05:30:31.687288 pgqmini-0.0.6/
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     1070 2023-06-15 16:54:52.000000 pgqmini-0.0.6/LICENSE
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2390 2023-06-17 05:30:31.687288 pgqmini-0.0.6/PKG-INFO
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2059 2023-06-17 05:29:23.000000 pgqmini-0.0.6/README.md
+drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-17 05:30:31.687288 pgqmini-0.0.6/pgqmini/
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       40 2023-06-16 14:18:20.000000 pgqmini-0.0.6/pgqmini/__init__.py
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)    11468 2023-06-17 05:15:59.000000 pgqmini-0.0.6/pgqmini/pgq.py
+drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-17 05:30:31.687288 pgqmini-0.0.6/pgqmini.egg-info/
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2390 2023-06-17 05:30:31.000000 pgqmini-0.0.6/pgqmini.egg-info/PKG-INFO
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      245 2023-06-17 05:30:31.000000 pgqmini-0.0.6/pgqmini.egg-info/SOURCES.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-17 05:30:31.000000 pgqmini-0.0.6/pgqmini.egg-info/dependency_links.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-17 05:30:31.000000 pgqmini-0.0.6/pgqmini.egg-info/not-zip-safe
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       16 2023-06-17 05:30:31.000000 pgqmini-0.0.6/pgqmini.egg-info/requires.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        8 2023-06-17 05:30:31.000000 pgqmini-0.0.6/pgqmini.egg-info/top_level.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       38 2023-06-17 05:30:31.687288 pgqmini-0.0.6/setup.cfg
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      582 2023-06-17 05:29:18.000000 pgqmini-0.0.6/setup.py
```

### Comparing `pgqmini-0.0.4/LICENSE` & `pgqmini-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqmini-0.0.4/PKG-INFO` & `pgqmini-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pgqmini
-Version: 0.0.4
+Version: 0.0.6
 Summary: pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues.
 Home-page: http://github.com/over-engineers/pgqmini
 Author: Kajago
 Author-email: jangsc0000@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **pgqmini**
 
-![version](https://img.shields.io/badge/version-0.0.4-blue)
+![version](https://img.shields.io/badge/version-0.0.6-blue)
 ![license](https://img.shields.io/badge/license-MIT-green)
 
 pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues. It provides a simple interface for adding and retrieving messages from a PostgreSQL-based queue, as well as handling timeouts and managing message processing.
 
 ## **Table of Contents**
 
 1. **[Installation](#installation)**
@@ -78,15 +78,15 @@
 
 while True:
     pgq.sub(process_message)
 ```
 
 In this code, we first create a **`PGQ`** object with the necessary database connection parameters. We then connect to the database and enter a loop where we process messages from the queue.
 
-For a more detailed usage guide, please check out the [Usage Guide](https://github.com/over-engineers/pgqmini/wiki/PGQ-Class-Documentation) in our wiki.
+For a more detailed usage guide, please check out the [Usage Guide](https://github.com/over-engineers/pgqmini/wiki/PGQ-(PostgreSQL-Queue)-Class) in our wiki.
 
 
 ## **License**
 
 pgqmini is released under the MIT License. See the `LICENSE` file for more details.
 
 ## **Contact**
```

### Comparing `pgqmini-0.0.4/README.md` & `pgqmini-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **pgqmini**
 
-![version](https://img.shields.io/badge/version-0.0.4-blue)
+![version](https://img.shields.io/badge/version-0.0.6-blue)
 ![license](https://img.shields.io/badge/license-MIT-green)
 
 pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues. It provides a simple interface for adding and retrieving messages from a PostgreSQL-based queue, as well as handling timeouts and managing message processing.
 
 ## **Table of Contents**
 
 1. **[Installation](#installation)**
@@ -67,15 +67,15 @@
 
 while True:
     pgq.sub(process_message)
 ```
 
 In this code, we first create a **`PGQ`** object with the necessary database connection parameters. We then connect to the database and enter a loop where we process messages from the queue.
 
-For a more detailed usage guide, please check out the [Usage Guide](https://github.com/over-engineers/pgqmini/wiki/PGQ-Class-Documentation) in our wiki.
+For a more detailed usage guide, please check out the [Usage Guide](https://github.com/over-engineers/pgqmini/wiki/PGQ-(PostgreSQL-Queue)-Class) in our wiki.
 
 
 ## **License**
 
 pgqmini is released under the MIT License. See the `LICENSE` file for more details.
 
 ## **Contact**
```

### Comparing `pgqmini-0.0.4/pgqmini/pgq.py` & `pgqmini-0.0.6/pgqmini/pgq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from dataclasses import dataclass, asdict
 import select
 from typing import Any, Callable
-import logging
 from psycopg2.extensions import ISOLATION_LEVEL_AUTOCOMMIT
 import psycopg2
 
 
 @dataclass(frozen=True)
 class Message:
     """
@@ -57,24 +56,22 @@
     conn: Any
     curs: Any
     qinfo: QueueInfo
 
     def __init__(self, host, user, password, port, dbname="pgq", qname="message_queue"):
         """
         The constructor of the PGQ class. It sets up the necessary variables to establish a connection to a PostgreSQL database.
-        It also sets up a logger for logging purposes.
 
         :param host: The hostname of the database server.
         :param user: The username to connect to the database.
         :param password: The password to connect to the database.
         :param port: The port number on which the database server is listening.
         :param dbname: The name of the database. Defaults to 'pgq'.
         :param qname: The name of the queue. Defaults to 'message_queue'.
         """
-        self.logger = logging.getLogger(__name__)
 
         self.qinfo = QueueInfo(host, user, password, port, dbname, qname)
 
     def _create_db(self):
         """
         A private method that creates a new database if it does not already exist.
         It does this by first connecting to the default 'postgres' database.
```

### Comparing `pgqmini-0.0.4/pgqmini.egg-info/PKG-INFO` & `pgqmini-0.0.6/pgqmini.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pgqmini
-Version: 0.0.4
+Version: 0.0.6
 Summary: pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues.
 Home-page: http://github.com/over-engineers/pgqmini
 Author: Kajago
 Author-email: jangsc0000@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **pgqmini**
 
-![version](https://img.shields.io/badge/version-0.0.4-blue)
+![version](https://img.shields.io/badge/version-0.0.6-blue)
 ![license](https://img.shields.io/badge/license-MIT-green)
 
 pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues. It provides a simple interface for adding and retrieving messages from a PostgreSQL-based queue, as well as handling timeouts and managing message processing.
 
 ## **Table of Contents**
 
 1. **[Installation](#installation)**
@@ -78,15 +78,15 @@
 
 while True:
     pgq.sub(process_message)
 ```
 
 In this code, we first create a **`PGQ`** object with the necessary database connection parameters. We then connect to the database and enter a loop where we process messages from the queue.
 
-For a more detailed usage guide, please check out the [Usage Guide](https://github.com/over-engineers/pgqmini/wiki/PGQ-Class-Documentation) in our wiki.
+For a more detailed usage guide, please check out the [Usage Guide](https://github.com/over-engineers/pgqmini/wiki/PGQ-(PostgreSQL-Queue)-Class) in our wiki.
 
 
 ## **License**
 
 pgqmini is released under the MIT License. See the `LICENSE` file for more details.
 
 ## **Contact**
```

### Comparing `pgqmini-0.0.4/setup.py` & `pgqmini-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name="pgqmini",
-    version="0.0.4",
+    version="0.0.6",
     description="pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/over-engineers/pgqmini",
     author="Kajago",
     author_email="jangsc0000@gmail.com",
     license="MIT",
```

