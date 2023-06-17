# Comparing `tmp/pgqmini-0.0.3.tar.gz` & `tmp/pgqmini-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqmini-0.0.3.tar", last modified: Thu Jun 15 18:08:07 2023, max compression
+gzip compressed data, was "pgqmini-0.0.4.tar", last modified: Sat Jun 17 05:14:51 2023, max compression
```

## Comparing `pgqmini-0.0.3.tar` & `pgqmini-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 18:08:07.994202 pgqmini-0.0.3/
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     1070 2023-06-15 16:54:52.000000 pgqmini-0.0.3/LICENSE
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2474 2023-06-15 18:08:07.994202 pgqmini-0.0.3/PKG-INFO
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2143 2023-06-15 18:07:07.000000 pgqmini-0.0.3/README.md
-drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 18:08:07.994202 pgqmini-0.0.3/pgqmini/
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       60 2023-06-15 17:48:41.000000 pgqmini-0.0.3/pgqmini/__init__.py
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     8629 2023-06-15 17:48:41.000000 pgqmini-0.0.3/pgqmini/pgq.py
-drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 18:08:07.994202 pgqmini-0.0.3/pgqmini.egg-info/
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2474 2023-06-15 18:08:07.000000 pgqmini-0.0.3/pgqmini.egg-info/PKG-INFO
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      245 2023-06-15 18:08:07.000000 pgqmini-0.0.3/pgqmini.egg-info/SOURCES.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-15 18:08:07.000000 pgqmini-0.0.3/pgqmini.egg-info/dependency_links.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-15 18:08:07.000000 pgqmini-0.0.3/pgqmini.egg-info/not-zip-safe
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       16 2023-06-15 18:08:07.000000 pgqmini-0.0.3/pgqmini.egg-info/requires.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        8 2023-06-15 18:08:07.000000 pgqmini-0.0.3/pgqmini.egg-info/top_level.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       38 2023-06-15 18:08:07.994202 pgqmini-0.0.3/setup.cfg
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      582 2023-06-15 18:04:44.000000 pgqmini-0.0.3/setup.py
+drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-17 05:14:51.132916 pgqmini-0.0.4/
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     1070 2023-06-15 16:54:52.000000 pgqmini-0.0.4/LICENSE
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2385 2023-06-17 05:14:51.132916 pgqmini-0.0.4/PKG-INFO
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2054 2023-06-17 05:12:41.000000 pgqmini-0.0.4/README.md
+drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-17 05:14:51.132916 pgqmini-0.0.4/pgqmini/
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       40 2023-06-16 14:18:20.000000 pgqmini-0.0.4/pgqmini/__init__.py
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)    11588 2023-06-17 04:27:13.000000 pgqmini-0.0.4/pgqmini/pgq.py
+drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-17 05:14:51.132916 pgqmini-0.0.4/pgqmini.egg-info/
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2385 2023-06-17 05:14:51.000000 pgqmini-0.0.4/pgqmini.egg-info/PKG-INFO
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      245 2023-06-17 05:14:51.000000 pgqmini-0.0.4/pgqmini.egg-info/SOURCES.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-17 05:14:51.000000 pgqmini-0.0.4/pgqmini.egg-info/dependency_links.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-17 05:14:51.000000 pgqmini-0.0.4/pgqmini.egg-info/not-zip-safe
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       16 2023-06-17 05:14:51.000000 pgqmini-0.0.4/pgqmini.egg-info/requires.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        8 2023-06-17 05:14:51.000000 pgqmini-0.0.4/pgqmini.egg-info/top_level.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       38 2023-06-17 05:14:51.132916 pgqmini-0.0.4/setup.cfg
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      582 2023-06-17 05:12:35.000000 pgqmini-0.0.4/setup.py
```

### Comparing `pgqmini-0.0.3/LICENSE` & `pgqmini-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqmini-0.0.3/PKG-INFO` & `pgqmini-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pgqmini
-Version: 0.0.3
+Version: 0.0.4
 Summary: pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues.
 Home-page: http://github.com/over-engineers/pgqmini
 Author: Kajago
 Author-email: jangsc0000@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **pgqmini**
 
-![version](https://img.shields.io/badge/version-0.0.3-blue)
+![version](https://img.shields.io/badge/version-0.0.4-blue)
 ![license](https://img.shields.io/badge/license-MIT-green)
 
 pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues. It provides a simple interface for adding and retrieving messages from a PostgreSQL-based queue, as well as handling timeouts and managing message processing.
 
 ## **Table of Contents**
 
 1. **[Installation](#installation)**
@@ -49,15 +49,15 @@
     user="username",
     password="password",
     port=5432,
 )
 
 pgq.connect()
 
-pgq.pub_message('{"key1": "value1", "key2": "value2"}')
+pgq.pub('{"key1": "value1", "key2": "value2"}')
 
 pgq.disconnect()
 ```
 
 ### **Subscriber**
 ```python
 from pgqmini import PGQ
@@ -69,21 +69,19 @@
     user="username",
     password="password",
     port=5432,
 )
 
 pgq.connect()
 
+def process_message(payload: str):
+    print(payload)
+
 while True:
-    try:
-        msg = pgq.sub_message()
-        process_message(msg)
-        pgq.complete_message(msg)
-    except Exception as e:
-        pgq.rollback_message(msg)
+    pgq.sub(process_message)
 ```
 
 In this code, we first create a **`PGQ`** object with the necessary database connection parameters. We then connect to the database and enter a loop where we process messages from the queue.
 
 For a more detailed usage guide, please check out the [Usage Guide](https://github.com/over-engineers/pgqmini/wiki/PGQ-Class-Documentation) in our wiki.
```

### Comparing `pgqmini-0.0.3/README.md` & `pgqmini-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **pgqmini**
 
-![version](https://img.shields.io/badge/version-0.0.3-blue)
+![version](https://img.shields.io/badge/version-0.0.4-blue)
 ![license](https://img.shields.io/badge/license-MIT-green)
 
 pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues. It provides a simple interface for adding and retrieving messages from a PostgreSQL-based queue, as well as handling timeouts and managing message processing.
 
 ## **Table of Contents**
 
 1. **[Installation](#installation)**
@@ -38,15 +38,15 @@
     user="username",
     password="password",
     port=5432,
 )
 
 pgq.connect()
 
-pgq.pub_message('{"key1": "value1", "key2": "value2"}')
+pgq.pub('{"key1": "value1", "key2": "value2"}')
 
 pgq.disconnect()
 ```
 
 ### **Subscriber**
 ```python
 from pgqmini import PGQ
@@ -58,21 +58,19 @@
     user="username",
     password="password",
     port=5432,
 )
 
 pgq.connect()
 
+def process_message(payload: str):
+    print(payload)
+
 while True:
-    try:
-        msg = pgq.sub_message()
-        process_message(msg)
-        pgq.complete_message(msg)
-    except Exception as e:
-        pgq.rollback_message(msg)
+    pgq.sub(process_message)
 ```
 
 In this code, we first create a **`PGQ`** object with the necessary database connection parameters. We then connect to the database and enter a loop where we process messages from the queue.
 
 For a more detailed usage guide, please check out the [Usage Guide](https://github.com/over-engineers/pgqmini/wiki/PGQ-Class-Documentation) in our wiki.
```

### Comparing `pgqmini-0.0.3/pgqmini/pgq.py` & `pgqmini-0.0.4/pgqmini/pgq.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from psycopg2.extensions import ISOLATION_LEVEL_AUTOCOMMIT
-import psycopg2
 from dataclasses import dataclass, asdict
-from typing import Any
 import select
+from typing import Any, Callable
+import logging
+from psycopg2.extensions import ISOLATION_LEVEL_AUTOCOMMIT
+import psycopg2
 
 
 @dataclass(frozen=True)
 class Message:
     """
     A class that represents a message in the queue.
     It is an immutable class, hence decorated with the 'frozen=True' parameter.
@@ -29,33 +30,62 @@
     port: int  # The port number on which the database server is listening
     dbname: str  # The name of the database
     qname: str  # The name of the queue
 
 
 class PGQ:
     """
-    A class for managing a PostgreSQL-based message queue.
+    The PGQ (PostgreSQL Queue) class represents a queue in a PostgreSQL database.
+    It allows for the publishing and subscribing of messages to and from the queue.
+
+    The PGQ class manages the connection to the PostgreSQL database, the creation of the database and queue (if they do not already exist),
+    and the insertion and retrieval of messages from the queue.
+
+    Each message in the queue has a status, which can be 'PENDING', 'PROCESSING', or 'COMPLETED'.
+    When a new message is inserted into the queue, its status is set to 'PENDING'.
+    When a message is retrieved from the queue for processing, its status is set to 'PROCESSING'.
+    If the message is processed successfully, its status is updated to 'COMPLETED'.
+    If an exception occurs during the processing of the message, its status is rolled back to 'PENDING'.
+
+    The PGQ class also provides a method for rolling back the status of messages that have been in the 'PROCESSING' state for longer than a specified timeout.
+
+    Attributes:
+        conn: A psycopg2 connection object for the PostgreSQL database.
+        curs: A cursor object for executing PostgreSQL commands.
+        qinfo: An instance of the QueueInfo dataclass, which stores the information necessary to connect to the queue.
     """
 
     conn: Any
     curs: Any
     qinfo: QueueInfo
 
     def __init__(self, host, user, password, port, dbname="pgq", qname="message_queue"):
         """
-        Initialize the instance with connection details.
+        The constructor of the PGQ class. It sets up the necessary variables to establish a connection to a PostgreSQL database.
+        It also sets up a logger for logging purposes.
+
+        :param host: The hostname of the database server.
+        :param user: The username to connect to the database.
+        :param password: The password to connect to the database.
+        :param port: The port number on which the database server is listening.
+        :param dbname: The name of the database. Defaults to 'pgq'.
+        :param qname: The name of the queue. Defaults to 'message_queue'.
         """
+        self.logger = logging.getLogger(__name__)
+
         self.qinfo = QueueInfo(host, user, password, port, dbname, qname)
 
     def _create_db(self):
         """
-        A private method to create a database if it doesn't already exist.
+        A private method that creates a new database if it does not already exist.
+        It does this by first connecting to the default 'postgres' database.
         """
         dbinfo = asdict(self.qinfo)
         dbinfo.update(dbname="postgres", qname=None)
+
         conn = psycopg2.connect(**dbinfo)
         conn.set_isolation_level(ISOLATION_LEVEL_AUTOCOMMIT)
 
         curs = conn.cursor()
 
         try:
             curs.execute(
@@ -68,185 +98,190 @@
             pass
         finally:
             curs.close()
             conn.close()
 
     def _create_queue(self):
         """
-        A private method to create a queue if it doesn't already exist.
+        A private method that creates a new table (queue) in the database if it does not already exist.
+        It also sets up the necessary triggers and trigger functions for the queue.
         """
         try:
             self.curs.execute(
                 f"""
                     -- Create a table
+                    CREATE TYPE message_status AS ENUM ('PENDING', 'PROCESSING', 'COMPLETED');
+
                     CREATE TABLE {self.qinfo.qname} (
                         id SERIAL PRIMARY KEY,
                         payload JSON NOT NULL,
-                        status VARCHAR(10) NOT NULL DEFAULT 'PENDING',
+                        status message_status NOT NULL DEFAULT 'PENDING',
                         created_at TIMESTAMP WITH TIME ZONE NOT NULL DEFAULT CURRENT_TIMESTAMP,
                         updated_at TIMESTAMP WITH TIME ZONE NOT NULL DEFAULT CURRENT_TIMESTAMP
                     );
 
                     -- Create indexes on status, updated_at columns
                     CREATE INDEX idx_{self.qinfo.qname}_status ON {self.qinfo.qname}(status);
                     CREATE INDEX idx_{self.qinfo.qname}_updated_at ON {self.qinfo.qname}(updated_at);
 
                     -- Create a function
                     CREATE OR REPLACE FUNCTION update_updated_at_column()
                     RETURNS TRIGGER AS $$
                     BEGIN
-                       NEW.updated_at = NOW();
-                       RETURN NEW;
+                        NEW.updated_at = NOW();
+                        -- Rollback
+                        IF (NEW.status = 0 AND NEW.status <> OLD.status) THEN
+                            PERFORM pg_notify('new_message', NEW.id::text);
+                        END IF;
+                        RETURN NEW;
                     END;
                     $$ language 'plpgsql';                  
 
                     -- Create a trigger
-                    CREATE TRIGGER update_{self.qinfo.qname}_updated_at
+                    CREATE OR REPLACE TRIGGER update_{self.qinfo.qname}_updated_at
                     BEFORE UPDATE ON {self.qinfo.qname}
                     FOR EACH ROW
                     EXECUTE PROCEDURE update_updated_at_column();
 
                     -- Create a trigger function
                     CREATE OR REPLACE FUNCTION notify_insert_message() RETURNS TRIGGER AS $$
                     DECLARE
                     BEGIN
-                      -- Trigger an event named 'new_message', passing the ID of the new row
-                      PERFORM pg_notify('new_message', NEW.id::text);
-                      RETURN NEW;
+                        -- Trigger an event named 'new_message', passing the ID of the new row
+                        PERFORM pg_notify('new_message', NEW.id::text);
+                        RETURN NEW;
                     END;
                     $$ LANGUAGE plpgsql;
 
                     -- Define a trigger to call the trigger function whenever a new row is inserted in the table
                     CREATE OR REPLACE TRIGGER {self.qinfo.qname}_trigger
                     AFTER INSERT ON {self.qinfo.qname}
                     FOR EACH ROW EXECUTE PROCEDURE notify_insert_message();
                 """
             )
         except psycopg2.errors.DuplicateTable as e:
             pass
 
     def connect(self):
         """
-        Establishes the connection to the PostgreSQL server and creates the queue.
+        Connects to the PostgreSQL database and creates a cursor object for executing PostgreSQL commands.
+        It also calls the _create_db and _create_queue methods to ensure that the database and queue are set up.
         """
         self._create_db()
 
         dbinfo = asdict(self.qinfo)
         dbinfo.update(qname=None)
         self.conn = psycopg2.connect(**dbinfo)
         self.conn.set_isolation_level(ISOLATION_LEVEL_AUTOCOMMIT)
         self.curs = self.conn.cursor()
 
         self._create_queue()
 
     def disconnect(self):
         """
-        Closes the connection to the PostgreSQL server.
+        Closes the cursor and the connection to the PostgreSQL database.
         """
         self.curs.close()
         self.conn.close()
 
-    def pub_message(self, payload):
+    def pub(self, payload):
         """
-        Publishes a new message to the queue.
+        Inserts a new message into the queue with the specified payload.
+
+        :param payload: The actual content of the message, which is a JSON-formatted string.
         """
         self.curs.execute(
             f"""
                 -- Insert a message into the queue
                 INSERT INTO {self.qinfo.qname} (payload)
                 VALUES ('{payload}');
             """
         )
 
-    def sub_message(self):
+    def sub(self, callback: Callable[[str], None]):
         """
-        Subscribes to the queue and selects a pending message to process.
+        Subscribes to the queue and continuously processes new messages as they arrive.
+        When a new message is processed, the specified callback function is called with the message's payload.
+
+        :param callback: A function to be called when a new message is processed. This function should take a single argument, which is the payload of the message.
         """
         self.curs.execute("LISTEN new_message;")
-        while True:
-            self.curs.execute(
-                f"""
-                    -- Select a message to process and update its status to 'PROCESSING'
-                    UPDATE {self.qinfo.qname}
-                    SET status = 'PROCESSING'
-                    FROM (
-                        -- Select a message from the queue
-                        SELECT id FROM {self.qinfo.qname}
-                        WHERE status = 'PENDING'
-                        ORDER BY id
-                        FOR UPDATE SKIP LOCKED
-                        LIMIT 1
-                    ) sub
-                    WHERE {self.qinfo.qname}.id = sub.id
-                    RETURNING {self.qinfo.qname}.id, payload
-                """
-            )
 
-            # Fetch the message to be processed
-            msg = self.curs.fetchone()
-            if msg is None:
-                select.select([self.conn], [], [])
-                continue
-            return Message(id=msg[0], payload=msg[1])
+        try:
+            while True:
+                msg = None
+                self.curs.execute(
+                    f"""
+                        -- Select a message to process and update its status to 'PROCESSING'
+                        UPDATE {self.qinfo.qname}
+                        SET status = 'PROCESSING'
+                        FROM (
+                            -- Select a message from the queue
+                            SELECT id FROM {self.qinfo.qname}
+                            WHERE status = 'PENDING'
+                            ORDER BY id
+                            FOR UPDATE SKIP LOCKED
+                            LIMIT 1
+                        ) sub
+                        WHERE {self.qinfo.qname}.id = sub.id
+                        RETURNING {self.qinfo.qname}.id, payload
+                    """
+                )
+
+                # Fetch the message to be processed
+                row = self.curs.fetchone()
+
+                if row is None:
+                    select.select([self.conn], [], [])
+                    continue
+                msg = Message(id=row[0], payload=row[1])
+
+                callback(msg.payload)
+                self._complete_message(msg)
+                return
+        except Exception as e:
+            if msg:
+                self._rollback_message(msg)
+            raise Exception
 
-    def complete_message(self, msg: Message):
+    def _complete_message(self, msg: Message):
         """
-        Marks a message as completed. The input is a Message object.
+        A private method that updates the status of a message to 'COMPLETED' after it has been processed.
+
+        :param msg: The message that has been processed.
         """
         self.curs.execute(
             f"""
                 -- Update the status of a message to 'COMPLETED'
                 UPDATE {self.qinfo.qname}
                 SET status = 'COMPLETED'
                 WHERE id = {msg.id}
             """
         )
 
-    def complete_message_by_id(self, id: int):
+    def _rollback_message(self, msg: Message):
         """
-        Marks a message as completed by its ID.
-        """
-        self.curs.execute(
-            f"""
-                -- Update the status of a message to 'COMPLETED' by its ID
-                UPDATE {self.qinfo.qname}
-                SET status = 'COMPLETED'
-                WHERE id = {id}
-            """
-        )
+        A private method that updates the status of a message to 'PENDING' if an exception occurs during the processing of the message.
 
-    def rollback_message(self, msg: Message):
-        """
-        Reverts the status of a message to 'PENDING'. The input is a Message object.
+        :param msg: The message whose processing resulted in an exception.
         """
         self.curs.execute(
             f"""
                 -- Update the status of a message to 'PENDING'
                 UPDATE {self.qinfo.qname}
                 SET status = 'PENDING'
                 WHERE id = {msg.id}
             """
         )
 
-    def rollback_message_by_id(self, id: int):
-        """
-        Reverts the status of a message to 'PENDING' by its ID.
-        """
-        self.curs.execute(
-            f"""
-                -- Update the status of a message to 'PENDING' by its ID
-                UPDATE {self.qinfo.qname}
-                SET status = 'PENDING'
-                WHERE id = {id}
-            """
-        )
-
     def rollback_timeout_messages(self, timeout: int):
         """
-        Reverts the status of messages that have timed out to 'PENDING'.
+        Updates the status of all messages that have been in the 'PROCESSING' state for longer than the specified timeout to 'PENDING'.
+
+        :param timeout: The number of seconds after which a message in the 'PROCESSING' state is considered to have timed out.
         """
         self.curs.execute(
             f"""
                 -- Update the status of messages to 'PENDING' if they have timed out
                 UPDATE {self.qinfo.qname}
                 SET status = 'PENDING'
                 WHERE status='PROCESSING' and updated_at + interval '{timeout} seconds' < now()
```

### Comparing `pgqmini-0.0.3/pgqmini.egg-info/PKG-INFO` & `pgqmini-0.0.4/pgqmini.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pgqmini
-Version: 0.0.3
+Version: 0.0.4
 Summary: pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues.
 Home-page: http://github.com/over-engineers/pgqmini
 Author: Kajago
 Author-email: jangsc0000@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **pgqmini**
 
-![version](https://img.shields.io/badge/version-0.0.3-blue)
+![version](https://img.shields.io/badge/version-0.0.4-blue)
 ![license](https://img.shields.io/badge/license-MIT-green)
 
 pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues. It provides a simple interface for adding and retrieving messages from a PostgreSQL-based queue, as well as handling timeouts and managing message processing.
 
 ## **Table of Contents**
 
 1. **[Installation](#installation)**
@@ -49,15 +49,15 @@
     user="username",
     password="password",
     port=5432,
 )
 
 pgq.connect()
 
-pgq.pub_message('{"key1": "value1", "key2": "value2"}')
+pgq.pub('{"key1": "value1", "key2": "value2"}')
 
 pgq.disconnect()
 ```
 
 ### **Subscriber**
 ```python
 from pgqmini import PGQ
@@ -69,21 +69,19 @@
     user="username",
     password="password",
     port=5432,
 )
 
 pgq.connect()
 
+def process_message(payload: str):
+    print(payload)
+
 while True:
-    try:
-        msg = pgq.sub_message()
-        process_message(msg)
-        pgq.complete_message(msg)
-    except Exception as e:
-        pgq.rollback_message(msg)
+    pgq.sub(process_message)
 ```
 
 In this code, we first create a **`PGQ`** object with the necessary database connection parameters. We then connect to the database and enter a loop where we process messages from the queue.
 
 For a more detailed usage guide, please check out the [Usage Guide](https://github.com/over-engineers/pgqmini/wiki/PGQ-Class-Documentation) in our wiki.
```

### Comparing `pgqmini-0.0.3/setup.py` & `pgqmini-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name="pgqmini",
-    version="0.0.3",
+    version="0.0.4",
     description="pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/over-engineers/pgqmini",
     author="Kajago",
     author_email="jangsc0000@gmail.com",
     license="MIT",
```

