# Comparing `tmp/websocket-client-1.5.3.tar.gz` & `tmp/websocket-client-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "websocket-client-1.5.3.tar", last modified: Fri Jun  9 09:33:59 2023, max compression
+gzip compressed data, was "websocket-client-1.6.0.tar", last modified: Sat Jun 17 08:11:40 2023, max compression
```

## Comparing `websocket-client-1.5.3.tar` & `websocket-client-1.6.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-09 09:33:59.804877 websocket-client-1.5.3/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    17264 2023-06-09 09:23:06.000000 websocket-client-1.5.3/ChangeLog
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11339 2023-02-04 17:51:20.000000 websocket-client-1.5.3/LICENSE
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       81 2023-02-04 17:51:20.000000 websocket-client-1.5.3/MANIFEST.in
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-06-09 09:33:59.804877 websocket-client-1.5.3/PKG-INFO
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     5997 2023-02-04 17:51:20.000000 websocket-client-1.5.3/README.md
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-09 09:33:59.796877 websocket-client-1.5.3/examples/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      344 2023-02-04 17:51:20.000000 websocket-client-1.5.3/examples/echo_client.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1009 2023-02-04 17:51:20.000000 websocket-client-1.5.3/examples/echoapp_client.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      351 2023-02-04 17:51:20.000000 websocket-client-1.5.3/examples/rel_client.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       59 2023-06-09 09:33:59.804877 websocket-client-1.5.3/setup.cfg
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2641 2023-06-09 09:20:50.000000 websocket-client-1.5.3/setup.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-09 09:33:59.800877 websocket-client-1.5.3/websocket/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      801 2023-06-09 09:20:59.000000 websocket-client-1.5.3/websocket/__init__.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    13619 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_abnf.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    20185 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_app.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2164 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_cookiejar.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    19872 2023-04-07 22:45:05.000000 websocket-client-1.5.3/websocket/_core.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2106 2023-04-07 22:59:49.000000 websocket-client-1.5.3/websocket/_exceptions.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     6610 2023-06-09 09:14:52.000000 websocket-client-1.5.3/websocket/_handshake.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11806 2023-04-07 22:47:13.000000 websocket-client-1.5.3/websocket/_http.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2220 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_logging.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4979 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_socket.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1122 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/_ssl_compat.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4932 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_url.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     3636 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/_utils.py
--rwxrwxr-x   0 drift3r   (1000) drift3r   (1000)     7116 2023-06-09 09:20:10.000000 websocket-client-1.5.3/websocket/_wsdump.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-09 09:33:59.800877 websocket-client-1.5.3/websocket/tests/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        0 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/__init__.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-09 09:33:59.800877 websocket-client-1.5.3/websocket/tests/data/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      163 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/data/header01.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      161 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/data/header02.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      216 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/data/header03.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      486 2023-05-21 19:20:24.000000 websocket-client-1.5.3/websocket/tests/echo-server.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4175 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/test_abnf.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    12669 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/test_app.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4325 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/test_cookiejar.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     9623 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/test_http.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    14589 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/test_url.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    18072 2023-02-04 17:51:20.000000 websocket-client-1.5.3/websocket/tests/test_websocket.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-09 09:33:59.804877 websocket-client-1.5.3/websocket_client.egg-info/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-06-09 09:33:59.000000 websocket-client-1.5.3/websocket_client.egg-info/PKG-INFO
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1014 2023-06-09 09:33:59.000000 websocket-client-1.5.3/websocket_client.egg-info/SOURCES.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        1 2023-06-09 09:33:59.000000 websocket-client-1.5.3/websocket_client.egg-info/dependency_links.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       50 2023-06-09 09:33:59.000000 websocket-client-1.5.3/websocket_client.egg-info/entry_points.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       94 2023-06-09 09:33:59.000000 websocket-client-1.5.3/websocket_client.egg-info/requires.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       10 2023-06-09 09:33:59.000000 websocket-client-1.5.3/websocket_client.egg-info/top_level.txt
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-17 08:11:39.993661 websocket-client-1.6.0/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    17445 2023-06-17 07:49:46.000000 websocket-client-1.6.0/ChangeLog
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11339 2023-06-12 20:33:24.000000 websocket-client-1.6.0/LICENSE
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       81 2023-06-12 20:33:24.000000 websocket-client-1.6.0/MANIFEST.in
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-06-17 08:11:39.993661 websocket-client-1.6.0/PKG-INFO
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     5997 2023-06-12 20:33:24.000000 websocket-client-1.6.0/README.md
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-17 08:11:39.989661 websocket-client-1.6.0/examples/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      344 2023-06-12 20:33:24.000000 websocket-client-1.6.0/examples/echo_client.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1009 2023-06-12 20:33:24.000000 websocket-client-1.6.0/examples/echoapp_client.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      351 2023-06-12 20:33:24.000000 websocket-client-1.6.0/examples/rel_client.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       59 2023-06-17 08:11:39.993661 websocket-client-1.6.0/setup.cfg
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2641 2023-06-17 07:47:12.000000 websocket-client-1.6.0/setup.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-17 08:11:39.993661 websocket-client-1.6.0/websocket/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      801 2023-06-17 07:47:23.000000 websocket-client-1.6.0/websocket/__init__.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    13656 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_abnf.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    20991 2023-06-17 07:46:23.000000 websocket-client-1.6.0/websocket/_app.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2164 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_cookiejar.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    20110 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_core.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2116 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_exceptions.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     6709 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_handshake.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11816 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_http.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2220 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_logging.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     5000 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_socket.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1122 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_ssl_compat.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4917 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_url.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     3667 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_utils.py
+-rwxrwxr-x   0 drift3r   (1000) drift3r   (1000)     7106 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_wsdump.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-17 08:11:39.993661 websocket-client-1.6.0/websocket/tests/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        0 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/__init__.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-17 08:11:39.993661 websocket-client-1.6.0/websocket/tests/data/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      163 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/data/header01.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      161 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/data/header02.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      216 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/data/header03.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      486 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/echo-server.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4175 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/test_abnf.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    12681 2023-06-17 07:58:21.000000 websocket-client-1.6.0/websocket/tests/test_app.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4325 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/test_cookiejar.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     9623 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/test_http.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    14589 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/test_url.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    18072 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/test_websocket.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-17 08:11:39.993661 websocket-client-1.6.0/websocket_client.egg-info/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-06-17 08:11:39.000000 websocket-client-1.6.0/websocket_client.egg-info/PKG-INFO
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1014 2023-06-17 08:11:39.000000 websocket-client-1.6.0/websocket_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        1 2023-06-17 08:11:39.000000 websocket-client-1.6.0/websocket_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       50 2023-06-17 08:11:39.000000 websocket-client-1.6.0/websocket_client.egg-info/entry_points.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       94 2023-06-17 08:11:39.000000 websocket-client-1.6.0/websocket_client.egg-info/requires.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       10 2023-06-17 08:11:39.000000 websocket-client-1.6.0/websocket_client.egg-info/top_level.txt
```

### Comparing `websocket-client-1.5.3/ChangeLog` & `websocket-client-1.6.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 ChangeLog
 ============
 
+- 1.6.0
+  - Fix teardown issue when ping thread is not properly ended (#918)
+  - Fix double ping wait time on first ping (#912)
+  - Minor typehints improvements (eda6724, 54b3013)
+
 - 1.5.3
   - Add logic to avoid error in the case where content-length header does not exist, bug introduced in 1.5.2 (#911)
   - Fix wsdump.py script typing, bug introduced in 1.5.2 (#914)
 
 - 1.5.2
   - Add typehints (#908)
   - Fix pytype errors (#906)
```

### Comparing `websocket-client-1.5.3/LICENSE` & `websocket-client-1.6.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2022 engn33r
+   Copyright 2023 engn33r
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `websocket-client-1.5.3/PKG-INFO` & `websocket-client-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websocket-client
-Version: 1.5.3
+Version: 1.6.0
 Summary: WebSocket client for Python with low level API options
 Home-page: https://github.com/websocket-client/websocket-client.git
 Download-URL: https://github.com/websocket-client/websocket-client/releases
 Author: liris
 Author-email: liris.pp@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://websocket-client.readthedocs.io/
```

### Comparing `websocket-client-1.5.3/README.md` & `websocket-client-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.3/examples/echoapp_client.py` & `websocket-client-1.6.0/examples/echoapp_client.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.3/setup.py` & `websocket-client-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 import pkg_resources
 from setuptools import setup, find_packages
 
 """
 setup.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-VERSION = "1.5.3"
+VERSION = "1.6.0"
 
 install_requires = []
 tests_require = []
 
 setup(
     name="websocket-client",
     version=VERSION,
```

### Comparing `websocket-client-1.5.3/websocket/__init__.py` & `websocket-client-1.6.0/websocket/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 __init__.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -19,8 +19,8 @@
 from ._abnf import *
 from ._app import WebSocketApp, setReconnect
 from ._core import *
 from ._exceptions import *
 from ._logging import *
 from ._socket import *
 
-__version__ = "1.5.3"
+__version__ = "1.6.0"
```

### Comparing `websocket-client-1.5.3/websocket/_abnf.py` & `websocket-client-1.6.0/websocket/_abnf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ._utils import validate_utf8
 from threading import Lock
 
 """
 _abnf.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -36,15 +36,15 @@
     def _mask(_m, _d) -> bytes:
         return XorMaskerSimple(_m).process(_d)
 
 except ImportError:
     # wsaccel is not available, use websocket-client _mask()
     native_byteorder = sys.byteorder
 
-    def _mask(mask_value: int, data_value: int) -> bytes:
+    def _mask(mask_value: array.array, data_value: array.array) -> bytes:
         datalen = len(data_value)
         data_value = int.from_bytes(data_value, native_byteorder)
         mask_value = int.from_bytes(mask_value * (datalen // 4) + mask_value[: datalen % 4], native_byteorder)
         return (data_value ^ mask_value).to_bytes(datalen, native_byteorder)
 
 
 __all__ = [
@@ -128,15 +128,15 @@
 
     # data length threshold.
     LENGTH_7 = 0x7e
     LENGTH_16 = 1 << 16
     LENGTH_63 = 1 << 63
 
     def __init__(self, fin: int = 0, rsv1: int = 0, rsv2: int = 0, rsv3: int = 0,
-                 opcode: int = OPCODE_TEXT, mask: int = 1, data: str = "") -> None:
+                 opcode: int = OPCODE_TEXT, mask: int = 1, data: str or bytes = "") -> None:
         """
         Constructor for ABNF. Please check RFC for arguments.
         """
         self.fin = fin
         self.rsv1 = rsv1
         self.rsv2 = rsv2
         self.rsv3 = rsv3
@@ -189,21 +189,21 @@
     @staticmethod
     def create_frame(data: str, opcode: int, fin: int = 1) -> 'ABNF':
         """
         Create frame to send text, binary and other data.
 
         Parameters
         ----------
-        data: <type>
+        data: str
             data to send. This is string value(byte array).
             If opcode is OPCODE_TEXT and this value is unicode,
             data value is converted into unicode string, automatically.
-        opcode: <type>
-            operation code. please see OPCODE_XXX.
-        fin: <type>
+        opcode: int
+            operation code. please see OPCODE_MAP.
+        fin: int
             fin flag. if set to 0, create continue fragmentation.
         """
         if opcode == ABNF.OPCODE_TEXT and isinstance(data, str):
             data = data.encode("utf-8")
         # mask must be set if send data from client
         return ABNF(fin, 0, 0, 0, opcode, 1, data)
 
@@ -233,24 +233,24 @@
 
         if not self.mask:
             return frame_header + self.data
         else:
             mask_key = self.get_mask_key(4)
             return frame_header + self._get_masked(mask_key)
 
-    def _get_masked(self, mask_key: bytes) -> bytes:
+    def _get_masked(self, mask_key: str or bytes) -> bytes:
         s = ABNF.mask(mask_key, self.data)
 
         if isinstance(mask_key, str):
             mask_key = mask_key.encode('utf-8')
 
         return mask_key + s
 
     @staticmethod
-    def mask(mask_key: bytes, data: bytes) -> bytes:
+    def mask(mask_key: str or bytes, data: str or bytes) -> bytes:
         """
         Mask or unmask data. Just do xor for each byte
 
         Parameters
         ----------
         mask_key: bytes or str
             4 byte mask.
```

### Comparing `websocket-client-1.5.3/websocket/_app.py` & `websocket-client-1.6.0/websocket/_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ._core import WebSocket, getdefaulttimeout
 from ._exceptions import *
 
 """
 _app.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -43,15 +43,15 @@
     RECONNECT = reconnectInterval
 
 
 class DispatcherBase:
     """
     DispatcherBase
     """
-    def __init__(self, app: Any, ping_timeout: int or float) -> None:
+    def __init__(self, app: Any, ping_timeout: float) -> None:
         self.app = app
         self.ping_timeout = ping_timeout
 
     def timeout(self, seconds: int, callback: Callable) -> None:
         time.sleep(seconds)
         callback()
 
@@ -65,65 +65,68 @@
             _logging.info("User exited {err}".format(err=e))
 
 
 class Dispatcher(DispatcherBase):
     """
     Dispatcher
     """
-    def read(self, sock: socket, read_callback: Callable, check_callback: Callable) -> None:
-        while self.app.keep_running:
-            sel = selectors.DefaultSelector()
-            sel.register(self.app.sock.sock, selectors.EVENT_READ)
-
-            r = sel.select(self.ping_timeout)
-            if r:
-                if not read_callback():
-                    break
-            check_callback()
+    def read(self, sock: socket.socket, read_callback: Callable, check_callback: Callable) -> None:
+        sel = selectors.DefaultSelector()
+        sel.register(self.app.sock.sock, selectors.EVENT_READ)
+        try:
+            while self.app.keep_running:
+                r = sel.select(self.ping_timeout)
+                if r:
+                    if not read_callback():
+                        break
+                check_callback()
+        finally:
             sel.close()
 
 
 class SSLDispatcher(DispatcherBase):
     """
     SSLDispatcher
     """
-    def read(self, sock: socket, read_callback: Callable, check_callback: Callable) -> None:
-        while self.app.keep_running:
-            r = self.select()
-            if r:
-                if not read_callback():
-                    break
-            check_callback()
+    def read(self, sock: socket.socket, read_callback: Callable, check_callback: Callable) -> None:
+        sock = self.app.sock.sock
+        sel = selectors.DefaultSelector()
+        sel.register(sock, selectors.EVENT_READ)
+        try:
+            while self.app.keep_running:
+                r = self.select(sock, sel)
+                if r:
+                    if not read_callback():
+                        break
+                check_callback()
+        finally:
+            sel.close()
 
-    def select(self) -> list:
+    def select(self, sock, sel:selectors.DefaultSelector):
         sock = self.app.sock.sock
         if sock.pending():
             return [sock,]
 
-        sel = selectors.DefaultSelector()
-        sel.register(sock, selectors.EVENT_READ)
-
         r = sel.select(self.ping_timeout)
-        sel.close()
 
         if len(r) > 0:
             return r[0][0]
 
 
 class WrappedDispatcher:
     """
     WrappedDispatcher
     """
-    def __init__(self, app, ping_timeout: int or float, dispatcher: Dispatcher) -> None:
+    def __init__(self, app, ping_timeout: float, dispatcher: Dispatcher) -> None:
         self.app = app
         self.ping_timeout = ping_timeout
         self.dispatcher = dispatcher
         dispatcher.signal(2, dispatcher.abort)  # keyboard interrupt
 
-    def read(self, sock: socket, read_callback: Callable, check_callback: Callable) -> None:
+    def read(self, sock: socket.socket, read_callback: Callable, check_callback: Callable) -> None:
         self.dispatcher.read(sock, read_callback)
         self.ping_timeout and self.timeout(self.ping_timeout, check_callback)
 
     def timeout(self, seconds: int, callback: Callable) -> None:
         self.dispatcher.timeout(seconds, callback)
 
     def reconnect(self, seconds: int, reconnector: Callable) -> None:
@@ -138,15 +141,15 @@
     def __init__(self, url: str, header: list or dict = None,
                  on_open: Callable = None, on_message: Callable = None, on_error: Callable = None,
                  on_close: Callable = None, on_ping: Callable = None, on_pong: Callable = None,
                  on_cont_message: Callable = None,
                  keep_running: bool = True, get_mask_key: Callable = None, cookie: str = None,
                  subprotocols: list = None,
                  on_data: Callable = None,
-                 socket: socket = None) -> None:
+                 socket: socket.socket = None) -> None:
         """
         WebSocketApp initialization
 
         Parameters
         ----------
         url: str
             Websocket url.
@@ -222,14 +225,16 @@
         self.stop_ping = None
         self.ping_interval = 0
         self.ping_timeout = None
         self.ping_payload = ""
         self.subprotocols = subprotocols
         self.prepared_socket = socket
         self.has_errored = False
+        self.has_done_teardown = False
+        self.has_done_teardown_lock = threading.Lock()
 
     def send(self, data: str, opcode: int = ABNF.OPCODE_TEXT) -> None:
         """
         send message
 
         Parameters
         ----------
@@ -264,31 +269,31 @@
         if self.stop_ping:
             self.stop_ping.set()
         if self.ping_thread and self.ping_thread.is_alive():
             self.ping_thread.join(3)
         self.last_ping_tm = self.last_pong_tm = 0
 
     def _send_ping(self) -> None:
-        if self.stop_ping.wait(self.ping_interval):
+        if self.stop_ping.wait(self.ping_interval) or self.keep_running is False:
             return
-        while not self.stop_ping.wait(self.ping_interval):
+        while not self.stop_ping.wait(self.ping_interval) and self.keep_running is True:
             if self.sock:
                 self.last_ping_tm = time.time()
                 try:
                     _logging.debug("Sending ping")
                     self.sock.ping(self.ping_payload)
                 except Exception as e:
                     _logging.debug("Failed to send ping: {err}".format(err=e))
 
     def run_forever(self, sockopt: tuple = None, sslopt: dict = None,
-                    ping_interval: int or float = 0, ping_timeout: int or float = None,
+                    ping_interval: float = 0, ping_timeout: float or None = None,
                     ping_payload: str = "",
                     http_proxy_host: str = None, http_proxy_port: int or str = None,
                     http_no_proxy: list = None, http_proxy_auth: tuple = None,
-                    http_proxy_timeout: int or float = None,
+                    http_proxy_timeout: float = None,
                     skip_utf8_validation: bool = False,
                     host: str = None, origin: str = None, dispatcher: Dispatcher = None,
                     suppress_origin: bool = False, proxy_type: str = None, reconnect: int = None) -> bool:
         """
         Run event loop for WebSocket framework.
 
         This loop is an infinite loop and is alive while websocket is available.
@@ -358,25 +363,32 @@
             raise WebSocketException("socket is already opened")
 
         self.ping_interval = ping_interval
         self.ping_timeout = ping_timeout
         self.ping_payload = ping_payload
         self.keep_running = True
 
-        def teardown(close_frame: ABNF = None) -> None:
+        def teardown(close_frame: ABNF = None):
             """
             Tears down the connection.
 
             Parameters
             ----------
             close_frame: ABNF frame
                 If close_frame is set, the on_close handler is invoked
                 with the statusCode and reason from the provided frame.
             """
 
+            # teardown() is called in many code paths to ensure resources are cleaned up and on_close is fired.
+            # To ensure the work is only done once, we use this bool and lock.
+            with self.has_done_teardown_lock:
+                if self.has_done_teardown:
+                    return
+                self.has_done_teardown = True
+
             self._stop_ping_thread()
             self.keep_running = False
             if self.sock:
                 self.sock.close()
             close_status_code, close_reason = self._get_close_args(
                 close_frame if close_frame else None)
             self.sock = None
@@ -480,19 +492,23 @@
             else:
                 _logging.error("{err} - goodbye".format(err=e))
                 teardown()
 
         custom_dispatcher = bool(dispatcher)
         dispatcher = self.create_dispatcher(ping_timeout, dispatcher, parse_url(self.url)[3])
 
-        setSock()
-        if not custom_dispatcher and reconnect:
-            while self.keep_running:
-                _logging.debug("Calling dispatcher reconnect [{frame_count} frames in stack]".format(frame_count=len(inspect.stack())))
-                dispatcher.reconnect(reconnect, setSock)
+        try:
+            setSock()
+            if not custom_dispatcher and reconnect:
+                while self.keep_running:
+                    _logging.debug("Calling dispatcher reconnect [{frame_count} frames in stack]".format(frame_count=len(inspect.stack())))
+                    dispatcher.reconnect(reconnect, setSock)
+        finally:
+            # Ensure teardown was called before returning from run_forever
+            teardown()
 
         return self.has_errored
 
     def create_dispatcher(self, ping_timeout: int, dispatcher: Dispatcher = None, is_ssl: bool = False) -> DispatcherBase:
         if dispatcher:  # If custom dispatcher is set, use WrappedDispatcher
             return WrappedDispatcher(self, ping_timeout, dispatcher)
         timeout = ping_timeout or 10
@@ -516,15 +532,15 @@
             close_status_code = 256 * close_frame.data[0] + close_frame.data[1]
             reason = close_frame.data[2:].decode('utf-8')
             return [close_status_code, reason]
         else:
             # Most likely reached this because len(close_frame_data.data) < 2
             return [None, None]
 
-    def _callback(self, callback: Callable, *args: tuple) -> None:
+    def _callback(self, callback, *args) -> None:
         if callback:
             try:
                 callback(self, *args)
 
             except Exception as e:
                 _logging.error("error from callback {callback}: {err}".format(callback=callback, err=e))
                 if self.on_error:
```

### Comparing `websocket-client-1.5.3/websocket/_cookiejar.py` & `websocket-client-1.6.0/websocket/_cookiejar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import http.cookies
 
 """
 _cookiejar.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `websocket-client-1.5.3/websocket/_core.py` & `websocket-client-1.6.0/websocket/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ._ssl_compat import *
 from ._utils import *
 
 """
 _core.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -70,16 +70,16 @@
     enable_multithread: bool
         If set to True, lock send method.
     skip_utf8_validation: bool
         Skip utf8 validation.
     """
 
     def __init__(self, get_mask_key=None, sockopt=None, sslopt=None,
-                 fire_cont_frame=False, enable_multithread=True,
-                 skip_utf8_validation=False, **_):
+                 fire_cont_frame: bool = False, enable_multithread: bool = True,
+                 skip_utf8_validation: bool = False, **_):
         """
         Initialize WebSocket object.
 
         Parameters
         ----------
         sslopt: dict
             Optional dict object for ssl socket options. See FAQ for details.
@@ -129,26 +129,26 @@
             callable object. the func takes 1 argument as integer.
             The argument means length of mask key.
             This func must return string(byte array),
             which length is argument specified.
         """
         self.get_mask_key = func
 
-    def gettimeout(self):
+    def gettimeout(self) -> float:
         """
         Get the websocket timeout (in seconds) as an int or float
 
         Returns
         ----------
         timeout: int or float
              returns timeout value (in seconds). This value could be either float/integer.
         """
         return self.sock_opt.timeout
 
-    def settimeout(self, timeout):
+    def settimeout(self, timeout: float):
         """
         Set the timeout to the websocket.
 
         Parameters
         ----------
         timeout: int or float
             timeout time (in seconds). This value could be either float/integer.
@@ -261,15 +261,15 @@
             self.connected = True
         except:
             if self.sock:
                 self.sock.close()
                 self.sock = None
             raise
 
-    def send(self, payload, opcode=ABNF.OPCODE_TEXT):
+    def send(self, payload: bytes or str, opcode: int = ABNF.OPCODE_TEXT) -> int:
         """
         Send the data as string.
 
         Parameters
         ----------
         payload: str
             Payload must be utf-8 string or unicode,
@@ -278,15 +278,15 @@
         opcode: int
             Operation code (opcode) to send.
         """
 
         frame = ABNF.create_frame(payload, opcode)
         return self.send_frame(frame)
 
-    def send_frame(self, frame):
+    def send_frame(self, frame) -> int:
         """
         Send the data frame.
 
         >>> ws = create_connection("ws://echo.websocket.events")
         >>> frame = ABNF.create_frame("Hello", ABNF.OPCODE_TEXT)
         >>> ws.send_frame(frame)
         >>> cont_frame = ABNF.create_frame("My name is ", ABNF.OPCODE_CONT, 0)
@@ -309,52 +309,52 @@
         with self.lock:
             while data:
                 l = self._send(data)
                 data = data[l:]
 
         return length
 
-    def send_binary(self, payload):
+    def send_binary(self, payload: bytes) -> int:
         """
         Send a binary message (OPCODE_BINARY).
 
         Parameters
         ----------
         payload: bytes
             payload of message to send.
         """
         return self.send(payload, ABNF.OPCODE_BINARY)
 
-    def ping(self, payload=""):
+    def ping(self, payload: str or bytes = ""):
         """
         Send ping data.
 
         Parameters
         ----------
         payload: str
             data payload to send server.
         """
         if isinstance(payload, str):
             payload = payload.encode("utf-8")
         self.send(payload, ABNF.OPCODE_PING)
 
-    def pong(self, payload=""):
+    def pong(self, payload: str or bytes = ""):
         """
         Send pong data.
 
         Parameters
         ----------
         payload: str
             data payload to send server.
         """
         if isinstance(payload, str):
             payload = payload.encode("utf-8")
         self.send(payload, ABNF.OPCODE_PONG)
 
-    def recv(self):
+    def recv(self) -> str or bytes:
         """
         Receive string data(byte array) from the server.
 
         Returns
         ----------
         data: string (byte array) value.
         """
@@ -363,15 +363,15 @@
         if opcode == ABNF.OPCODE_TEXT:
             return data.decode("utf-8")
         elif opcode == ABNF.OPCODE_TEXT or opcode == ABNF.OPCODE_BINARY:
             return data
         else:
             return ''
 
-    def recv_data(self, control_frame=False):
+    def recv_data(self, control_frame: bool = False) -> tuple:
         """
         Receive data with operation code.
 
         Parameters
         ----------
         control_frame: bool
             a boolean flag indicating whether to return control frame
@@ -381,15 +381,15 @@
         -------
         opcode, frame.data: tuple
             tuple of operation code and string(byte array) value.
         """
         opcode, frame = self.recv_data_frame(control_frame)
         return opcode, frame.data
 
-    def recv_data_frame(self, control_frame=False):
+    def recv_data_frame(self, control_frame: bool = False):
         """
         Receive data with operation code.
 
         If a valid ping message is received, a pong response is sent.
 
         Parameters
         ----------
@@ -440,15 +440,15 @@
 
         Returns
         -------
         self.frame_buffer.recv_frame(): ABNF frame object
         """
         return self.frame_buffer.recv_frame()
 
-    def send_close(self, status=STATUS_NORMAL, reason=b""):
+    def send_close(self, status: int = STATUS_NORMAL, reason: bytes = b""):
         """
         Send close data to the server.
 
         Parameters
         ----------
         status: int
             Status code to send. See STATUS_XXX.
@@ -456,22 +456,22 @@
             The reason to close. This must be string or UTF-8 bytes.
         """
         if status < 0 or status >= ABNF.LENGTH_16:
             raise ValueError("code is invalid range")
         self.connected = False
         self.send(struct.pack('!H', status) + reason, ABNF.OPCODE_CLOSE)
 
-    def close(self, status=STATUS_NORMAL, reason=b"", timeout=3):
+    def close(self, status: int = STATUS_NORMAL, reason: bytes = b"", timeout: float = 3):
         """
         Close Websocket object
 
         Parameters
         ----------
         status: int
-            Status code to send. See STATUS_XXX.
+            Status code to send. See VALID_CLOSE_STATUS in ABNF.
         reason: bytes
             The reason to close in UTF-8.
         timeout: int or float
             Timeout until receive a close frame.
             If None, it will wait forever until receive a close frame.
         """
         if self.connected:
@@ -517,29 +517,29 @@
         close socket, immediately.
         """
         if self.sock:
             self.sock.close()
             self.sock = None
             self.connected = False
 
-    def _send(self, data):
+    def _send(self, data: str or bytes):
         return send(self.sock, data)
 
     def _recv(self, bufsize):
         try:
             return recv(self.sock, bufsize)
         except WebSocketConnectionClosedException:
             if self.sock:
                 self.sock.close()
             self.sock = None
             self.connected = False
             raise
 
 
-def create_connection(url, timeout=None, class_=WebSocket, **options):
+def create_connection(url: str, timeout=None, class_=WebSocket, **options):
     """
     Connect to url and return websocket object.
 
     Connect to url and return the WebSocket object.
     Passing optional timeout parameter will set the timeout on the socket.
     If no timeout is supplied,
     the global default timeout setting returned by getdefaulttimeout() is used.
```

### Comparing `websocket-client-1.5.3/websocket/_exceptions.py` & `websocket-client-1.6.0/websocket/_exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 _exceptions.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -62,15 +62,15 @@
 
 
 class WebSocketBadStatusException(WebSocketException):
     """
     WebSocketBadStatusException will be raised when we get bad handshake status code.
     """
 
-    def __init__(self, message, status_code, status_message=None, resp_headers=None, resp_body=None):
+    def __init__(self, message: str, status_code: int, status_message=None, resp_headers=None, resp_body=None):
         super().__init__(message)
         self.status_code = status_code
         self.resp_headers = resp_headers
         self.resp_body = resp_body
 
 
 class WebSocketAddressException(WebSocketException):
```

### Comparing `websocket-client-1.5.3/websocket/_handshake.py` & `websocket-client-1.6.0/websocket/_handshake.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 _handshake.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -36,22 +36,22 @@
 SUCCESS_STATUSES = SUPPORTED_REDIRECT_STATUSES + (HTTPStatus.SWITCHING_PROTOCOLS,)
 
 CookieJar = SimpleCookieJar()
 
 
 class handshake_response:
 
-    def __init__(self, status, headers, subprotocol):
+    def __init__(self, status: int, headers: dict, subprotocol):
         self.status = status
         self.headers = headers
         self.subprotocol = subprotocol
         CookieJar.add(headers.get("set-cookie"))
 
 
-def handshake(sock, url, hostname, port, resource, **options):
+def handshake(sock, url: str, hostname: str, port: int, resource: str, **options):
     headers, key = _get_handshake_headers(resource, url, hostname, port, options)
 
     header_str = "\r\n".join(headers)
     send(sock, header_str)
     dump("request header", header_str)
 
     status, resp = _get_resp_headers(sock)
@@ -60,23 +60,23 @@
     success, subproto = _validate(resp, key, options.get("subprotocols"))
     if not success:
         raise WebSocketException("Invalid WebSocket Header")
 
     return handshake_response(status, resp, subproto)
 
 
-def _pack_hostname(hostname):
+def _pack_hostname(hostname: str) -> str:
     # IPv6 address
     if ':' in hostname:
         return '[' + hostname + ']'
 
     return hostname
 
 
-def _get_handshake_headers(resource, url, host, port, options):
+def _get_handshake_headers(resource: str, url: str, host: str, port: int, options: dict):
     headers = [
         "GET {resource} HTTP/1.1".format(resource=resource),
         "Upgrade: websocket"
     ]
     if port == 80 or port == 443:
         hostport = _pack_hostname(host)
     else:
@@ -135,15 +135,15 @@
     if cookie:
         headers.append("Cookie: {cookie}".format(cookie=cookie))
 
     headers.extend(("", ""))
     return headers, key
 
 
-def _get_resp_headers(sock, success_statuses=SUCCESS_STATUSES):
+def _get_resp_headers(sock, success_statuses: tuple = SUCCESS_STATUSES) -> tuple:
     status, resp_headers, status_message = read_headers(sock)
     if status not in success_statuses:
         content_len = resp_headers.get('content-length')
         if content_len:
             response_body = sock.recv(int(content_len))  # read the body of the HTTP error message response and include it in the exception
         else:
             response_body = None
@@ -153,15 +153,15 @@
 
 _HEADERS_TO_CHECK = {
     "upgrade": "websocket",
     "connection": "upgrade",
 }
 
 
-def _validate(headers, key, subprotocols):
+def _validate(headers, key: str, subprotocols):
     subproto = None
     for k, v in _HEADERS_TO_CHECK.items():
         r = headers.get(k, None)
         if not r:
             return False, None
         r = [x.strip().lower() for x in r.split(',')]
         if v not in r:
@@ -188,10 +188,10 @@
 
     if success:
         return True, subproto
     else:
         return False, None
 
 
-def _create_sec_websocket_key():
+def _create_sec_websocket_key() -> str:
     randomness = os.urandom(16)
     return base64encode(randomness).decode('utf-8').strip()
```

### Comparing `websocket-client-1.5.3/websocket/_http.py` & `websocket-client-1.6.0/websocket/_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 _http.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -65,15 +65,15 @@
         else:
             self.proxy_port = 0
             self.auth = None
             self.no_proxy = None
             self.proxy_protocol = "http"
 
 
-def _start_proxied_socket(url, options, proxy):
+def _start_proxied_socket(url: str, options, proxy):
     if not HAVE_PYTHON_SOCKS:
         raise WebSocketException("Python Socks is needed for SOCKS proxying but is not available")
 
     hostname, port, resource, is_secure = parse_url(url)
 
     if proxy.proxy_protocol == "socks5":
         rdns = False
@@ -103,15 +103,15 @@
         sock = _ssl_socket(sock, options.sslopt, hostname)
     elif is_secure:
         raise WebSocketException("SSL not available.")
 
     return sock, (hostname, port, resource)
 
 
-def connect(url, options, proxy, socket):
+def connect(url: str, options, proxy, socket):
     # Use _start_proxied_socket() only for socks4 or socks5 proxy
     # Use _tunnel() for http proxy
     # TODO: Use python-socks for http protocol also, to standardize flow
     if proxy.proxy_host and not socket and not (proxy.proxy_protocol == "http"):
         return _start_proxied_socket(url, options, proxy)
 
     hostname, port_from_url, resource, is_secure = parse_url(url)
```

### Comparing `websocket-client-1.5.3/websocket/_logging.py` & `websocket-client-1.6.0/websocket/_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 """
 _logging.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `websocket-client-1.5.3/websocket/_socket.py` & `websocket-client-1.6.0/websocket/_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ._ssl_compat import *
 from ._utils import *
 
 """
 _socket.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -74,15 +74,15 @@
     ----------
     _default_timeout: int or float
         Return the global timeout setting (in seconds) to connect.
     """
     return _default_timeout
 
 
-def recv(sock: socket, bufsize: int) -> bytes:
+def recv(sock: socket.socket, bufsize: int) -> bytes:
     if not sock:
         raise WebSocketConnectionClosedException("socket is already closed.")
 
     def _recv():
         try:
             return sock.recv(bufsize)
         except SSLWantReadError:
@@ -121,25 +121,25 @@
     if not bytes_:
         raise WebSocketConnectionClosedException(
             "Connection to remote host was lost.")
 
     return bytes_
 
 
-def recv_line(sock: socket) -> bytes:
+def recv_line(sock: socket.socket) -> bytes:
     line = []
     while True:
         c = recv(sock, 1)
         line.append(c)
         if c == b'\n':
             break
     return b''.join(line)
 
 
-def send(sock: socket, data: bytes) -> int:
+def send(sock: socket.socket, data: bytes) -> int:
     if isinstance(data, str):
         data = data.encode('utf-8')
 
     if not sock:
         raise WebSocketConnectionClosedException("socket is already closed.")
 
     def _send():
```

### Comparing `websocket-client-1.5.3/websocket/_ssl_compat.py` & `websocket-client-1.6.0/websocket/_ssl_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 _ssl_compat.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `websocket-client-1.5.3/websocket/_url.py` & `websocket-client-1.6.0/websocket/_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from urllib.parse import unquote, urlparse
 
 """
 _url.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -136,19 +136,19 @@
     hostname: str
         Websocket server name.
     is_secure: bool
         Is the connection secure? (wss) looks for "https_proxy" in env
         before falling back to "http_proxy"
     proxy_host: str
         http proxy host name.
-    http_proxy_port: str or int
+    proxy_port: str or int
         http proxy port.
-    http_no_proxy: list
+    no_proxy: list
         Whitelisted host names that don't use the proxy.
-    http_proxy_auth: tuple
+    proxy_auth: tuple
         HTTP proxy auth information. Tuple of username and password. Default is None.
     proxy_type: str
         Specify the proxy protocol (http, socks4, socks4a, socks5, socks5h). Default is "http".
         Use socks4a or socks5h if you want to send DNS requests through the proxy.
     """
     if _is_no_proxy_host(hostname, no_proxy):
         return None, 0, None
```

### Comparing `websocket-client-1.5.3/websocket/_utils.py` & `websocket-client-1.6.0/websocket/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 _url.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -59,35 +59,35 @@
         # of a state of the automaton and a character class to a state.
         0,12,24,36,60,96,84,12,12,12,48,72, 12,12,12,12,12,12,12,12,12,12,12,12,
         12, 0,12,12,12,12,12, 0,12, 0,12,12, 12,24,12,12,12,12,12,24,12,24,12,12,
         12,12,12,12,12,12,12,24,12,12,12,12, 12,24,12,12,12,12,12,12,12,24,12,12,
         12,12,12,12,12,12,12,36,12,36,12,12, 12,36,12,12,12,12,12,36,12,36,12,12,
         12,36,12,12,12,12,12,12,12,12,12,12, ]
 
-    def _decode(state, codep, ch) -> tuple:
+    def _decode(state: int, codep: int, ch: int) -> tuple:
         tp = _UTF8D[ch]
 
         codep = (ch & 0x3f) | (codep << 6) if (
             state != _UTF8_ACCEPT) else (0xff >> tp) & ch
         state = _UTF8D[256 + state + tp]
 
         return state, codep
 
-    def _validate_utf8(utfbytes: bytes) -> bool:
+    def _validate_utf8(utfbytes: str or bytes) -> bool:
         state = _UTF8_ACCEPT
         codep = 0
         for i in utfbytes:
             state, codep = _decode(state, codep, i)
             if state == _UTF8_REJECT:
                 return False
 
         return True
 
 
-def validate_utf8(utfbytes: str) -> bool:
+def validate_utf8(utfbytes: str or bytes) -> bool:
     """
     validate utf8 byte string.
     utfbytes: utf byte string to check.
     return value: if valid utf8 string, return true. Otherwise, return false.
     """
     return _validate_utf8(utfbytes)
```

### Comparing `websocket-client-1.5.3/websocket/_wsdump.py` & `websocket-client-1.6.0/websocket/_wsdump.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 """
 wsdump.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -150,15 +150,15 @@
     ws = websocket.create_connection(args.url, sslopt=opts, **options)
     if args.raw:
         console = NonInteractive()
     else:
         console = InteractiveConsole()
         print("Press Ctrl+C to quit")
 
-    def recv() -> tuple[int, str]:
+    def recv() -> tuple:
         try:
             frame = ws.recv_frame()
         except websocket.WebSocketException:
             return websocket.ABNF.OPCODE_CLOSE, ""
         if not frame:
             raise websocket.WebSocketException("Not a valid frame {frame}".format(frame=frame))
         elif frame.opcode in OPCODE_DATA:
```

### Comparing `websocket-client-1.5.3/websocket/tests/test_abnf.py` & `websocket-client-1.6.0/websocket/tests/test_abnf.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from websocket._abnf import *
 import unittest
 
 """
 test_abnf.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `websocket-client-1.5.3/websocket/tests/test_app.py` & `websocket-client-1.6.0/websocket/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import ssl
 import unittest
 
 """
 test_app.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -306,13 +306,13 @@
                 # Got second pong after reconnect
                 app.close()
 
         app = ws.WebSocketApp('ws://127.0.0.1:' + LOCAL_WS_SERVER_PORT, on_pong=on_pong, on_error=on_error)
         app.run_forever(ping_interval=2, ping_timeout=1, reconnect=3)
 
         self.assertEqual(pong_count, 2)
-        self.assertIsInstance(exc, ValueError)
-        self.assertEqual(str(exc), "Invalid file object: None")
+        self.assertIsInstance(exc, ws.WebSocketTimeoutException)
+        self.assertEqual(str(exc), "ping/pong timed out")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `websocket-client-1.5.3/websocket/tests/test_cookiejar.py` & `websocket-client-1.6.0/websocket/tests/test_cookiejar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 from websocket._cookiejar import SimpleCookieJar
 
 """
 test_cookiejar.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `websocket-client-1.5.3/websocket/tests/test_http.py` & `websocket-client-1.6.0/websocket/tests/test_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import websocket
 import socket
 
 """
 test_http.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `websocket-client-1.5.3/websocket/tests/test_url.py` & `websocket-client-1.6.0/websocket/tests/test_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import unittest
 from websocket._url import get_proxy_info, parse_url, _is_address_in_network, _is_no_proxy_host
 
 """
 test_url.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `websocket-client-1.5.3/websocket/tests/test_websocket.py` & `websocket-client-1.6.0/websocket/tests/test_websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from websocket._utils import validate_utf8
 from base64 import decodebytes as base64decode
 
 """
 test_websocket.py
 websocket - WebSocket client library for Python
 
-Copyright 2022 engn33r
+Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `websocket-client-1.5.3/websocket_client.egg-info/PKG-INFO` & `websocket-client-1.6.0/websocket_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websocket-client
-Version: 1.5.3
+Version: 1.6.0
 Summary: WebSocket client for Python with low level API options
 Home-page: https://github.com/websocket-client/websocket-client.git
 Download-URL: https://github.com/websocket-client/websocket-client/releases
 Author: liris
 Author-email: liris.pp@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://websocket-client.readthedocs.io/
```

### Comparing `websocket-client-1.5.3/websocket_client.egg-info/SOURCES.txt` & `websocket-client-1.6.0/websocket_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

