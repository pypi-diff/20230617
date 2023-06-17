# Comparing `tmp/meowerbot-2.5.7.tar.gz` & `tmp/meowerbot-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meowerbot-2.5.7.tar", max compression
+gzip compressed data, was "meowerbot-2.6.0.tar", max compression
```

## Comparing `meowerbot-2.5.7.tar` & `meowerbot-2.6.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.5.7/LICENSE
--rw-r--r--   0        0        0      191 2023-05-30 05:10:00.997418 meowerbot-2.5.7/MeowerBot/__init__.py
--rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.5.7/MeowerBot/_Commands.py
--rw-r--r--   0        0        0     1381 2023-05-24 23:08:36.965919 meowerbot-2.5.7/MeowerBot/API.py
--rw-r--r--   0        0        0    14286 2023-05-30 05:08:19.515887 meowerbot-2.5.7/MeowerBot/Bot.py
--rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.5.7/MeowerBot/cloudlink/__init__.py
--rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.5.7/MeowerBot/cloudlink/cloudlink.py
--rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.5.7/MeowerBot/cog.py
--rw-r--r--   0        0        0     2443 2023-05-25 00:29:18.441297 meowerbot-2.5.7/MeowerBot/command.py
--rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.5.7/MeowerBot/context.py
--rw-r--r--   0        0        0      681 2023-05-30 05:09:48.150426 meowerbot-2.5.7/pyproject.toml
--rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.5.7/README.md
--rw-r--r--   0        0        0     1099 1970-01-01 00:00:00.000000 meowerbot-2.5.7/setup.py
--rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 meowerbot-2.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.6.0/LICENSE
+-rw-r--r--   0        0        0      191 2023-06-17 04:54:29.183483 meowerbot-2.6.0/MeowerBot/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.6.0/MeowerBot/_Commands.py
+-rw-r--r--   0        0        0     1381 2023-05-24 23:08:36.965919 meowerbot-2.6.0/MeowerBot/API.py
+-rw-r--r--   0        0        0    14662 2023-06-17 04:15:40.638689 meowerbot-2.6.0/MeowerBot/Bot.py
+-rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.6.0/MeowerBot/cl/__init__.py
+-rw-r--r--   0        0        0     8937 2023-06-17 04:05:40.519304 meowerbot-2.6.0/MeowerBot/cl/cloudlink.py
+-rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.6.0/MeowerBot/cog.py
+-rw-r--r--   0        0        0     3543 2023-06-17 03:52:08.597897 meowerbot-2.6.0/MeowerBot/command.py
+-rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.6.0/MeowerBot/context.py
+-rw-r--r--   0        0        0     1941 2023-06-17 04:53:04.923013 meowerbot-2.6.0/MeowerBot/ext/help.py
+-rw-r--r--   0        0        0      681 2023-06-17 04:54:29.183483 meowerbot-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.6.0/README.md
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 meowerbot-2.6.0/setup.py
+-rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 meowerbot-2.6.0/PKG-INFO
```

### Comparing `meowerbot-2.5.7/LICENSE` & `meowerbot-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.7/MeowerBot/API.py` & `meowerbot-2.6.0/MeowerBot/API.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.7/MeowerBot/Bot.py` & `meowerbot-2.6.0/MeowerBot/Bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import threading
 import shlex
 
-from .cloudlink import CloudLink
+from .cl import CloudLink
 import sys
 
 import json
 import traceback
 
 import requests
 
@@ -141,33 +141,44 @@
 
     def __handle_error__(self, e):
         self.run_cb("error", args=(e,))
         if type(e) == WebSocketConnectionClosedException and self.autoreload:
             self.__handle_close__()
             return
 
+        if (type(e)) == KeyboardInterrupt:
+            #kill all bot threads
+            self.bad_exit = True
+
+            self.wss = None # effectively kill the bot
+            self.__handle_close__(            )            
+            return
+        
+        
 
         
 
 
     def _debug_fix(self, packet):
         packet = json.loads(packet)  # Server bug workaround
 
         try:
             self.__handle_packet__(packet)
-        except Exception as e:  # cq: skip #IDC ABOUT GENERAL EXCP
-
+        except BaseException as e:  # cq: skip #IDC ABOUT GENERAL EXCP
+            self.__handle_error__(e)
             self.logger.error(traceback.format_exc())
             self.run_cb("error", args=(e, ))
 
         try:
             self.run_cb("__raw__", args=(packet, ))  # raw packets
-        except Exception as e:  # cq: skip #IDC ABOUT GENERAL EXCP
+        except BaseException as e:  # cq: skip #IDC ABOUT GENERAL EXCP
+            self.__handle_error__(e)
             self.logger.error(traceback.format_exc())
             self.run_cb("error", args=(e, ))
+            
 
     def __handle_on_connect__(self):
         self.wss.sendPacket(
             {
                 "cmd": "direct",
                 "val": {"cmd": "type", "val": "py"},
             }
@@ -236,15 +247,16 @@
                         "post": "ERROR: MeowerBot.py Webhooks Logging\n\n Account Softlocked.",
                         "username": self.username,
                     },
                     timeout=5
                 )
                 print("CRITICAL ERROR! ACCOUNT SOFTLOCKED!!!!.", file=sys.__stdout__)
                 self.bad_exit = True
-                self.wss.stop()
+                del self.wss
+                
                 return
 
             if status != "I:100 | OK":
                 raise RuntimeError("Password Or Username Is Incorrect")
 
             time.sleep(0.5)
             self.run_cb("login", args=(), kwargs={})
```

### Comparing `meowerbot-2.5.7/MeowerBot/cloudlink/cloudlink.py` & `meowerbot-2.6.0/MeowerBot/cl/cloudlink.py`

 * *Files 17% similar despite different names*

```diff
@@ -72,16 +72,17 @@
             # Format dict for storing this mode's specific data
             self.statedata = {
                 "ulist": {"usernames": []},
             }
 
             # Run the client
             self.wss.run_forever()
-        except Exception as e:
+        except BaseException as e:
             self.logging.error(f"Error at client: {e}")
+            self._on_error_client(self.wss, e)
 
     def stop(self, abrupt=False):  # Stops CloudLink (not sure if working)
         self.wss.close()
 
     def callback(
         self, callback_id, function
     ):  # Add user-friendly callbacks for CloudLink to be useful as a module
@@ -90,26 +91,28 @@
                 self.callback_function[callback_id] = function
 
                 self.logging.debug(f"Binded callback {callback_id}.")
             else:
                 self.logging.error(
                     f"Error: Callback {callback_id} is not a valid callback id!"
                 )
-        except Exception as e:
+        except BaseException as e:
             self.logging.error(f"Error at callback: {e}")
+            self._on_error_client(self.wss, e)
 
     def sendPacket(
         self, msg
     ):  # User-friendly message sender for both server and client.
         try:
 
             self.logging.debug(f"Sending {json.dumps(msg)}")
             self.wss.send(json.dumps(msg))
-        except Exception as e:
+        except BaseException as e:
             self.logging.error(f"Error on sendPacket (client): {e}")
+            self._on_error_client(self.wss, e)
 
     def getUsernames(self):  # Returns the username list.
         return self.statedata["ulist"]["usernames"]
 
 
 class CloudLink(API):
     def __init__(self):  # Initializes CloudLink
@@ -145,20 +148,23 @@
                 json.dumps({"cmd": "direct", "val": {"cmd": "type", "val": "py"}})
             )  # Specify to the server that the client is based on Python
             if not self.callback_function["on_connect"] is None:
 
                 def run(*args):
                     try:
                         self.callback_function["on_connect"]()
-                    except Exception as e:
+                    except BaseException as e:
                         self.logging.error(f"Error on _on_connection_client: {e}")
+                        self._on_error_client(self.wss, error)
 
                 threading.Thread(target=run).start()
-        except Exception as e:
+        except BaseException as e:
             self.logging.info(f"Error on _on_connection_client: {e}")
+            self._on_error_client(self.wss, e)
+
 
     def _on_packet_client(self, ws, message):  # Client-side packet handler
         try:
 
             self.logging.debug(f"New packet: {message}")
 
             tmp = json.loads(message)
@@ -173,52 +179,59 @@
                 )
 
             if not self.callback_function["on_packet"] == None:
 
                 def run(*args):
                     try:
                         self.callback_function["on_packet"](message)
-                    except Exception as e:
+                    except BaseException as e:
 
                         self.logging.error(f"Error on _on_packet_client: {e}")
+                        self._on_error_client(self.wss, e)
 
                 threading.Thread(target=run).start()
-        except Exception as e:
+        except BaseException as e:
             self.logging.error(f"Error on _on_packet_client: {e}")
+            self._on_error_client(self.wss, e)
 
     def _on_error_client(self, ws, error):  # Client-side error handler
         try:
 
             self.logging.error(f"Error: {error}")
             if not self.callback_function["on_error"] is None:
 
                 def run(*args):
                     try:
                         self.callback_function["on_error"](error)
-                    except Exception as e:
+                    except BaseException as e:
                         self.logging.error(f"Error on _on_error_client: {e}")
 
+                        self._on_error_client(self.wss, e)
+
                 threading.Thread(target=run).start()
-        except Exception as e:
+        except BaseException as e:
 
             self.logging.error(f"Error on _on_error_client: {e}")
+            self._on_error_client(self.wss, e)
 
     def _closed_connection_client(
         self, ws, close_status_code, close_msg
     ):  # Client-side closed connection handler
         try:
 
             self.logging.info(
                 f"Closed, status: {close_status_code} with code {close_msg}"
             )
             if not self.callback_function["on_close"] is None:
 
                 def run(*args):
                     try:
                         self.callback_function["on_close"]()
-                    except Exception as e:
+                    except BaseException as e:
 
                         self.logging.error(f"Error on _closed_connection_client: {e}")
+                        self._on_error_client(self.wss, e)
 
                 threading.Thread(target=run).start()
-        except Exception as e:
+        except BaseException as e:
             self.logging.error(f"Error on _closed_connection_client: {e}")
+            self._on_error_client(self.wss, e)
```

### Comparing `meowerbot-2.5.7/MeowerBot/cog.py` & `meowerbot-2.6.0/MeowerBot/cog.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.7/MeowerBot/context.py` & `meowerbot-2.6.0/MeowerBot/context.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.7/pyproject.toml` & `meowerbot-2.6.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MeowerBot"
-version = "2.5.7"
+version = "2.6.0"
 description = "A meower bot lib for py"
 authors = ["showierdata9978 <68120127+showierdata9978@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "MeowerBot"}
 ]
```

### Comparing `meowerbot-2.5.7/setup.py` & `meowerbot-2.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['MeowerBot', 'MeowerBot.cloudlink']
+['MeowerBot', 'MeowerBot.cl', 'MeowerBot.ext']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.0,<3.0.0', 'websocket-client']
 
 extras_require = \
 {':python_version < "3.11"': ['backports-strenum>=1.2.4,<2.0.0']}
 
 setup_kwargs = {
     'name': 'meowerbot',
-    'version': '2.5.7',
+    'version': '2.6.0',
     'description': 'A meower bot lib for py',
     'long_description': '# MeowerBot.py\n\nA bot lib for Meower\n\n\n## License\n\nsee [LICENSE](./LICENSE)\n\n\n## docs\n\nThe Docs are located [here](https://meowerbot-py.showierdata.tech/)\n\n\n## Quick Example\n\nlook at the [tests directory](./tests) for examples ',
     'author': 'showierdata9978',
     'author_email': '68120127+showierdata9978@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/MeowerBots/MeowerBot.py',
```

### Comparing `meowerbot-2.5.7/PKG-INFO` & `meowerbot-2.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meowerbot
-Version: 2.5.7
+Version: 2.6.0
 Summary: A meower bot lib for py
 Home-page: https://github.com/MeowerBots/MeowerBot.py
 License: MIT
 Author: showierdata9978
 Author-email: 68120127+showierdata9978@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

