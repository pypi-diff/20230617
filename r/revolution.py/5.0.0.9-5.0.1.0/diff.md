# Comparing `tmp/revolution.py-5.0.0.9.tar.gz` & `tmp/revolution.py-5.0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revolution.py-5.0.0.9.tar", last modified: Mon Jun 12 06:49:04 2023, max compression
+gzip compressed data, was "revolution.py-5.0.1.0.tar", last modified: Sat Jun 17 05:27:33 2023, max compression
```

## Comparing `revolution.py-5.0.0.9.tar` & `revolution.py-5.0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 06:49:04.775824 revolution.py-5.0.0.9/
--rw-rw-rw-   0        0        0    35823 2023-06-11 23:52:23.000000 revolution.py-5.0.0.9/LICENSE
--rw-rw-rw-   0        0        0      449 2023-06-12 06:49:04.773603 revolution.py-5.0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      928 2023-06-12 05:49:37.000000 revolution.py-5.0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 06:49:04.706735 revolution.py-5.0.0.9/revolution/
--rw-rw-rw-   0        0        0     4979 2023-06-12 06:20:33.000000 revolution.py-5.0.0.9/revolution/lib.py
--rw-rw-rw-   0        0        0     3162 2023-06-12 03:43:38.000000 revolution.py-5.0.0.9/revolution/main.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:49:04.771800 revolution.py-5.0.0.9/revolution.py.egg-info/
--rw-rw-rw-   0        0        0      449 2023-06-12 06:49:04.000000 revolution.py-5.0.0.9/revolution.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-12 06:49:04.000000 revolution.py-5.0.0.9/revolution.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:49:04.000000 revolution.py-5.0.0.9/revolution.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 06:49:04.000000 revolution.py-5.0.0.9/revolution.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 06:49:04.775824 revolution.py-5.0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      626 2023-06-12 06:48:59.000000 revolution.py-5.0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 05:27:33.750781 revolution.py-5.0.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-06-11 23:52:23.000000 revolution.py-5.0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      449 2023-06-17 05:27:33.744304 revolution.py-5.0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      928 2023-06-12 05:49:37.000000 revolution.py-5.0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 05:27:33.699879 revolution.py-5.0.1.0/revolution/
+-rw-rw-rw-   0        0        0     4878 2023-06-17 05:25:59.000000 revolution.py-5.0.1.0/revolution/lib.py
+-rw-rw-rw-   0        0        0     3162 2023-06-12 03:43:38.000000 revolution.py-5.0.1.0/revolution/main.py
+drwxrwxrwx   0        0        0        0 2023-06-17 05:27:33.742540 revolution.py-5.0.1.0/revolution.py.egg-info/
+-rw-rw-rw-   0        0        0      449 2023-06-17 05:27:32.000000 revolution.py-5.0.1.0/revolution.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-17 05:27:32.000000 revolution.py-5.0.1.0/revolution.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 05:27:32.000000 revolution.py-5.0.1.0/revolution.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-17 05:27:32.000000 revolution.py-5.0.1.0/revolution.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 05:27:33.750781 revolution.py-5.0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-06-17 05:26:10.000000 revolution.py-5.0.1.0/setup.py
```

### Comparing `revolution.py-5.0.0.9/LICENSE` & `revolution.py-5.0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revolution.py-5.0.0.9/README.md` & `revolution.py-5.0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `revolution.py-5.0.0.9/revolution/lib.py` & `revolution.py-5.0.1.0/revolution/lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,16 +41,15 @@
         self.watching_servers = in_server
         if token == None or token == "": return print(f"{Color.FAIL}revolution.bot.run.error{Color.ENDC}{Color.NORMAL_SPACE}{Color.WARNING}Bot cannot run: token has not been set correctly.{Color.ENDC}")
         request = RequestHandler(Request("http://revolution.ericplayzyt.repl.co/api/v1/python/token_exists", "GET", headers={"token": token}).request(), RequestType.GET, "json").c()
         if request['token_exists'] == "false": return print(f"{Color.FAIL}revolution.bot.run.error{Color.ENDC}{Color.NORMAL_SPACE}{Color.WARNING}Bot cannot run: token has not been set correctly. (NO TOKEN FOUND IN DB){Color.ENDC}")
         print(f"{Color.OKCYAN}revolution.bot.api{Color.ENDC}{Color.NORMAL_SPACE}   {Color.OKGREEN}Hosting bot to servers: {Color.ENDC}{Color.OKBLUE}{in_server}{Color.ENDC}")
         try: await self.events['ready']()
         except Exception as e: print(e)
-        pingrequest = PingRequest("https://revolution.ericplayzyt.repl.co/api/v1/python/ping_bot_online", RequestType.GET)
-        await pingrequest.request(0.5, self.after_each_request)
+        # 17/06/23 = ping requests are removed for overlogging the API and the server.
     
     def get(self):
         return self.bot
     
     def setup(self, name):
         if self.invoked:
             return print(f"{Color.FAIL}revolution.bot.before_invoke.error{Color.ENDC}{Color.NORMAL_SPACE}{Color.WARNING}{Color.ENDC}")
```

### Comparing `revolution.py-5.0.0.9/revolution/main.py` & `revolution.py-5.0.1.0/revolution/main.py`

 * *Files identical despite different names*

### Comparing `revolution.py-5.0.0.9/setup.py` & `revolution.py-5.0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "revolution.py",
-    version = "5.0.0.9",
+    version = "5.0.1.0",
     description = "A simple Py package to integrate Revolution's bot API into python.",
     long_description = "A simple Py package to integrate Revolution's bot API into Python. \nhttps://github.com/JustAnEric/Revolution.py",
     author = "JustAnEric",
     maintainer = "Revolution Corporation",
     requires = ["requests"],
     url = "https://revolution.ericplayzyt.repl.co/",
     packages = ["revolution"],
```

