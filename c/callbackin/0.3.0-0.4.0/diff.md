# Comparing `tmp/callbackin-0.3.0.tar.gz` & `tmp/callbackin-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callbackin-0.3.0.tar", max compression
+gzip compressed data, was "callbackin-0.4.0.tar", max compression
```

## Comparing `callbackin-0.3.0.tar` & `callbackin-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1535 2023-06-17 11:36:46.832824 callbackin-0.3.0/README.md
--rw-r--r--   0        0        0       21 2023-06-17 12:13:11.499908 callbackin-0.3.0/callbackin/__init__.py
--rw-r--r--   0        0        0       49 2023-06-17 11:29:59.539358 callbackin-0.3.0/callbackin/__main__.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.295912 callbackin-0.3.0/callbackin/handler/__init__.py
--rw-r--r--   0        0        0     2029 2023-06-17 11:10:29.612392 callbackin-0.3.0/callbackin/handler/callback.py
--rw-r--r--   0        0        0     1944 2023-06-17 11:55:24.500003 callbackin-0.3.0/callbackin/handler/login.py
--rw-r--r--   0        0        0     4919 2023-06-17 12:13:32.477157 callbackin-0.3.0/callbackin/main.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.286706 callbackin-0.3.0/callbackin/schemas/__init__.py
--rw-r--r--   0        0        0      210 2023-06-17 10:51:29.288644 callbackin-0.3.0/callbackin/schemas/callback.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.261151 callbackin-0.3.0/callbackin/utils/__init__.py
--rw-r--r--   0        0        0     1322 2023-06-17 11:08:57.376439 callbackin-0.3.0/callbackin/utils/config.py
--rw-r--r--   0        0        0     1493 2023-06-17 11:32:01.695647 callbackin-0.3.0/callbackin/utils/request.py
--rw-r--r--   0        0        0      440 2023-06-17 12:13:20.202361 callbackin-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 callbackin-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1535 2023-06-17 11:36:46.832824 callbackin-0.4.0/README.md
+-rw-r--r--   0        0        0       21 2023-06-17 12:19:12.890621 callbackin-0.4.0/callbackin/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-17 11:29:59.539358 callbackin-0.4.0/callbackin/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.295912 callbackin-0.4.0/callbackin/handler/__init__.py
+-rw-r--r--   0        0        0     2034 2023-06-17 12:19:01.116279 callbackin-0.4.0/callbackin/handler/callback.py
+-rw-r--r--   0        0        0     1944 2023-06-17 11:55:24.500003 callbackin-0.4.0/callbackin/handler/login.py
+-rw-r--r--   0        0        0     4813 2023-06-17 12:18:07.035407 callbackin-0.4.0/callbackin/main.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.286706 callbackin-0.4.0/callbackin/schemas/__init__.py
+-rw-r--r--   0        0        0      210 2023-06-17 10:51:29.288644 callbackin-0.4.0/callbackin/schemas/callback.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.261151 callbackin-0.4.0/callbackin/utils/__init__.py
+-rw-r--r--   0        0        0     1322 2023-06-17 11:08:57.376439 callbackin-0.4.0/callbackin/utils/config.py
+-rw-r--r--   0        0        0     1493 2023-06-17 11:32:01.695647 callbackin-0.4.0/callbackin/utils/request.py
+-rw-r--r--   0        0        0      440 2023-06-17 12:19:07.437376 callbackin-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 callbackin-0.4.0/PKG-INFO
```

### Comparing `callbackin-0.3.0/README.md` & `callbackin-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `callbackin-0.3.0/callbackin/handler/callback.py` & `callbackin-0.4.0/callbackin/handler/callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,11 +40,11 @@
                 case "PUT":
                     response = requests.put(self.callback.local_endpoint, data=body, headers=headers)
             typer.echo(f"Response from {self.callback.local_endpoint} -> {response.status_code}")
 
     def run(self):
         typer.echo(f"Running callback {self.callback.name} -> {self.callback.local_endpoint}")
         mqtt_config = get_mqtt_config()
-        self.client.connect(mqtt_config["host"], mqtt_config["port"], 60)
+        self.client.connect(mqtt_config["host"], int(mqtt_config["port"]), 60)
         self.client.loop_forever()
```

### Comparing `callbackin-0.3.0/callbackin/handler/login.py` & `callbackin-0.4.0/callbackin/handler/login.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.3.0/callbackin/main.py` & `callbackin-0.4.0/callbackin/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,15 @@
 
     response = post("/callbacks", data={
         "name": name,
         "local_endpoint": local_endpoint,
         "description": description,
     })
     if response.status_code == 200:
-        print(response.json())
         callback = Callback(**response.json())
-        typer.echo(f"Callback created successfully with ID {callback.id}")
         typer.echo(f"Using This URL to use your endpoint: {BASE_URL}/handle/{callback.path}")
     else:
         typer.echo("Error creating callback")
 
 @app.command("list")
 def list_callbacks():
     typer.echo("Listing callbacks")
```

### Comparing `callbackin-0.3.0/callbackin/utils/config.py` & `callbackin-0.4.0/callbackin/utils/config.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.3.0/callbackin/utils/request.py` & `callbackin-0.4.0/callbackin/utils/request.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.3.0/PKG-INFO` & `callbackin-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: callbackin
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: ibrahim4529
 Author-email: ibrahim.hanif4529@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

