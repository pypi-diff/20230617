# Comparing `tmp/nonebot_adapter_villa-0.2.0.tar.gz` & `tmp/nonebot_adapter_villa-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.2.1.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.2.0.tar` & `nonebot_adapter_villa-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1062 2023-06-16 14:06:25.691916 nonebot_adapter_villa-0.2.0/LICENSE
--rw-r--r--   0        0        0     5070 2023-06-16 14:06:25.691916 nonebot_adapter_villa-0.2.0/README.md
--rw-r--r--   0        0        0      235 2023-06-16 14:06:25.691916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0     4668 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0     2905 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/cilent.pyi
--rw-r--r--   0        0        0     3714 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0    12434 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0    10411 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    12230 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      263 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0     8936 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0     6704 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0       76 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-17 08:49:37.971137 nonebot_adapter_villa-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5070 2023-06-17 08:49:37.971137 nonebot_adapter_villa-0.2.1/README.md
+-rw-r--r--   0        0        0      235 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0     5056 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0     2905 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/cilent.pyi
+-rw-r--r--   0        0        0     3714 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0    12434 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0    10411 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1514 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    12230 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      263 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0     8936 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     1755 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0     6704 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0       76 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     1134 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.2.1/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.2.0/LICENSE` & `nonebot_adapter_villa-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.0/README.md` & `nonebot_adapter_villa-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,17 +72,26 @@
                                 if bot.bot_id == bot_id
                             ),
                             None,
                         )
                     ) is not None:
                         bot = Bot(self, bot_id, payload.robot, bot_secret=bot_secret)
                         self.bot_connect(bot)
-                        log("INFO", f"<y>Bot {escape_tag(bot.self_id)} connected</y>")
+                        log("INFO", f"<y>Bot {bot.self_id} connected</y>")
                     else:
-                        log("WARNING", f"<r>Missing bot secret for bot {bot_id}</r>")
+                        log(
+                            "WARNING",
+                            f"<r>Missing bot secret for bot {bot_id}</r>, event will not be handle",
+                        )
+                        return Response(
+                            200,
+                            content=json.dumps(
+                                {"retcode": 0, "message": "NoneBot2 Get it!"}
+                            ),
+                        )
                 bot = cast(Bot, bot)
                 bot._bot_info = payload.robot
 
                 if (event_class := event_classes.get(payload.type, None)) and (
                     event_class.__type__.name in payload.extend_data["EventData"]
                 ):
                     try:
@@ -96,24 +105,24 @@
                             e,
                         )
                     else:
                         asyncio.create_task(bot.handle_event(event))
                 else:
                     log(
                         "INFO",
-                        f"Unknown event type: {payload.type} data={payload.extend_data}",
+                        f"Unknown event type: {payload.type} data={escape_tag(str(payload.extend_data))}",
                     )
                 # (Path().cwd() / f'test_event_{payload.created_at}.json').write_text(json.dumps(json_data, indent=4, ensure_ascii=False), encoding='utf-8')
                 return Response(
                     200,
                     content=json.dumps({"retcode": 0, "message": "NoneBot2 Get it!"}),
                 )
             return Response(400, content="Invalid Request Body")
         return Response(400, content="Invalid Request Body")
 
     @overrides(BaseAdapter)
     async def _call_api(self, bot: Bot, api: str, **data: Any) -> Any:
         log("DEBUG", f"Calling API <y>{api}</y>")
-        log("TRACE", f"With Data <y>{data}</y>")
+        log("TRACE", f"With Data <y>{escape_tag(str(data))}</y>")
         if (api_handler := API_HANDLERS.get(api)) is None:
             raise ApiNotAvailable(api)
         return await api_handler(self, bot, **data)
```

### Comparing `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/cilent.pyi` & `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/cilent.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/client.py` & `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.0/pyproject.toml` & `nonebot_adapter_villa-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.2.0"
+version = "0.2.1"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.2.0/PKG-INFO` & `nonebot_adapter_villa-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.2.0
+Version: 0.2.1
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.2.1 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

