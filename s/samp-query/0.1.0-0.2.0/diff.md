# Comparing `tmp/samp_query-0.1.0.tar.gz` & `tmp/samp_query-0.2.0.tar.gz`

## Comparing `samp_query-0.1.0.tar` & `samp_query-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 samp_query-0.1.0/.coverage
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 samp_query-0.1.0/main.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 samp_query-0.1.0/requirements-test.txt
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 samp_query-0.1.0/requirements.txt
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 samp_query-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 samp_query-0.1.0/samp_query/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.1.0/test/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.1.0/test/conftest.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 samp_query-0.1.0/test/test_client.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 samp_query-0.1.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.1.0/LICENSE
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 samp_query-0.1.0/README.md
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 samp_query-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 samp_query-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 samp_query-0.2.0/.coverage
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 samp_query-0.2.0/main.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 samp_query-0.2.0/requirements-test.txt
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 samp_query-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 samp_query-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 samp_query-0.2.0/samp_query/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 samp_query-0.2.0/samp_query/rcon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.2.0/test/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.2.0/test/conftest.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 samp_query-0.2.0/test/test_client.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 samp_query-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.2.0/LICENSE
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 samp_query-0.2.0/README.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 samp_query-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 samp_query-0.2.0/PKG-INFO
```

### Comparing `samp_query-0.1.0/.coverage` & `samp_query-0.2.0/.coverage`

 * *Files identical despite different names*

### Comparing `samp_query-0.1.0/main.py` & `samp_query-0.2.0/main.py`

 * *Files identical despite different names*

### Comparing `samp_query-0.1.0/.github/workflows/ci.yml` & `samp_query-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `samp_query-0.1.0/samp_query/__init__.py` & `samp_query-0.2.0/samp_query/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,39 +2,45 @@
 import struct
 import random
 from dataclasses import dataclass, field
 
 import cchardet as chardet  # type: ignore
 import trio
 
-# Assuming latency variance is less than 100%
-MAX_LATENCY_VARIANCE = 2
+# Assuming ratio between max and min ping can't be higher than this
+MAX_LATENCY_VARIANCE = 5
 
 
 def encode_codepage(string: str) -> bytes:
     for codepage in range(1250, 1259):
         try:
             return string.encode(f'cp{codepage}')
         except UnicodeEncodeError:
             continue
 
-    raise ValueError(f'Unable to encode string "{string}"')
+    raise UnicodeEncodeError(
+        'cp1250-1258',
+        string,
+        0,
+        len(string),
+        'Unable to find a suitable codepage',
+    )
 
 
 def pack_string(string: str, len_type: str) -> bytes:
     format = f'<{len_type}'
     return struct.pack(format, len(string)) + encode_codepage(string)
 
 
 def unpack_string(data: bytes, len_type: str) -> tuple[str, bytes]:
     format = f'<{len_type}'
     size = struct.calcsize(format)
     str_len, data = *struct.unpack_from(format, data), data[size:]
     string, data = data[:str_len], data[str_len:]
-    encoding: str = chardet.detect(string)['encoding']
+    encoding = chardet.detect(string)['encoding'] or 'ascii'
     return string.decode(encoding), data
 
 
 class MissingRCONPassword(Exception):
     pass
 
 
@@ -242,19 +248,17 @@
         response = ''
 
         with trio.move_on_after(MAX_LATENCY_VARIANCE * ping) as cancel_scope:
             while True:
                 start_time = trio.current_time()
                 data = await self.receive(header=self.prefix + b'x')
                 receive_duration = trio.current_time() - start_time
-                line_len = struct.unpack_from('<H', data)[0]
-                data = data[2:]  # short, see above
-                assert len(data) == line_len
-                encoding: str = chardet.detect(data)['encoding']
-                response += data.decode(encoding) + '\n'
+                line, data = unpack_string(data, 'H')
+                assert not data
+                response += line + '\n'
                 cancel_scope.deadline += receive_duration
 
         if not response:
             raise RCONDisabled()
 
         if response == 'Invalid RCON password.\n':
             raise InvalidRCONPassword()
```

### Comparing `samp_query-0.1.0/LICENSE` & `samp_query-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `samp_query-0.1.0/pyproject.toml` & `samp_query-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "samp_query"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="The Cheaterman", email="the.cheaterman@gmail.com" },
 ]
 description = "A SAMP query/RCON client for Python using trio."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -13,14 +13,17 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "trio",
   "faust-cchardet",
 ]
 
+[project.scripts]
+samp-rcon = "samp_query.rcon:run"
+
 [project.urls]
 "Homepage" = "https://github.com/Cheaterman/samp-query"
 "Bug Tracker" = "https://github.com/Cheaterman/samp-query/issues"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `samp_query-0.1.0/PKG-INFO` & `samp_query-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samp_query
-Version: 0.1.0
+Version: 0.2.0
 Summary: A SAMP query/RCON client for Python using trio.
 Project-URL: Homepage, https://github.com/Cheaterman/samp-query
 Project-URL: Bug Tracker, https://github.com/Cheaterman/samp-query/issues
 Author-email: The Cheaterman <the.cheaterman@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

