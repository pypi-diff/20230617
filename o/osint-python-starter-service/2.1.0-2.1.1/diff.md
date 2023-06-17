# Comparing `tmp/osint-python-starter-service-2.1.0.tar.gz` & `tmp/osint-python-starter-service-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-starter-service-2.1.0.tar", last modified: Wed Jun  7 21:09:29 2023, max compression
+gzip compressed data, was "osint-python-starter-service-2.1.1.tar", last modified: Sat Jun 17 00:50:27 2023, max compression
```

## Comparing `osint-python-starter-service-2.1.0.tar` & `osint-python-starter-service-2.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 21:09:29.058852 osint-python-starter-service-2.1.0/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.1.0/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-07 21:09:29.058852 osint-python-starter-service-2.1.0/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1731 2023-04-25 07:13:29.000000 osint-python-starter-service-2.1.0/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 21:09:29.058852 osint-python-starter-service-2.1.0/osint_python_starter_service.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-07 21:09:29.000000 osint-python-starter-service-2.1.0/osint_python_starter_service.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      931 2023-06-07 21:09:29.000000 osint-python-starter-service-2.1.0/osint_python_starter_service.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-07 21:09:29.000000 osint-python-starter-service-2.1.0/osint_python_starter_service.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-06-07 21:09:29.000000 osint-python-starter-service-2.1.0/osint_python_starter_service.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-06-07 21:09:29.000000 osint-python-starter-service-2.1.0/osint_python_starter_service.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-07 21:09:29.058852 osint-python-starter-service-2.1.0/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-06-07 21:06:01.000000 osint-python-starter-service-2.1.0/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 21:09:29.058852 osint-python-starter-service-2.1.0/starter_service/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.1.0/starter_service/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.1.0/starter_service/api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     7256 2023-06-06 19:38:47.000000 osint-python-starter-service-2.1.0/starter_service/api_server.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     5774 2023-06-03 20:59:13.000000 osint-python-starter-service-2.1.0/starter_service/avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3670 2023-06-07 10:14:54.000000 osint-python-starter-service-2.1.0/starter_service/base_service.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1837 2023-06-07 19:08:41.000000 osint-python-starter-service-2.1.0/starter_service/env.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 21:09:29.058852 osint-python-starter-service-2.1.0/starter_service/examples/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.1.0/starter_service/examples/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      594 2023-06-07 19:05:41.000000 osint-python-starter-service-2.1.0/starter_service/examples/error.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1274 2023-06-07 20:59:38.000000 osint-python-starter-service-2.1.0/starter_service/examples/manual_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1212 2023-06-07 19:05:41.000000 osint-python-starter-service-2.1.0/starter_service/examples/multi.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1324 2023-06-07 19:08:41.000000 osint-python-starter-service-2.1.0/starter_service/examples/offset_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1156 2023-06-07 19:08:41.000000 osint-python-starter-service-2.1.0/starter_service/examples/single.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6632 2023-06-07 21:08:37.000000 osint-python-starter-service-2.1.0/starter_service/kafka_adapter.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      985 2023-04-25 07:17:35.000000 osint-python-starter-service-2.1.0/starter_service/messages.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     7571 2023-04-25 06:06:55.000000 osint-python-starter-service-2.1.0/starter_service/schemas.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-07 21:09:29.058852 osint-python-starter-service-2.1.0/starter_service/tests/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 14:40:43.000000 osint-python-starter-service-2.1.0/starter_service/tests/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      560 2023-05-18 15:14:53.000000 osint-python-starter-service-2.1.0/starter_service/tests/employee.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      699 2023-06-03 20:55:03.000000 osint-python-starter-service-2.1.0/starter_service/tests/teet.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2885 2023-06-03 20:45:37.000000 osint-python-starter-service-2.1.0/starter_service/tests/test_avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      194 2023-05-18 14:41:17.000000 osint-python-starter-service-2.1.0/starter_service/tests/tst.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:50:27.029231 osint-python-starter-service-2.1.1/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.1.1/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-17 00:50:27.029231 osint-python-starter-service-2.1.1/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1731 2023-04-25 07:13:29.000000 osint-python-starter-service-2.1.1/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:50:27.025897 osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-17 00:50:27.000000 osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      942 2023-06-17 00:50:27.000000 osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-17 00:50:27.000000 osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-06-17 00:50:27.000000 osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-06-17 00:50:27.000000 osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-17 00:50:27.029231 osint-python-starter-service-2.1.1/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-06-17 00:46:37.000000 osint-python-starter-service-2.1.1/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:50:27.025897 osint-python-starter-service-2.1.1/starter_service/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.1.1/starter_service/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.1.1/starter_service/api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6176 2023-06-17 00:42:50.000000 osint-python-starter-service-2.1.1/starter_service/api_server.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     5774 2023-06-03 20:59:13.000000 osint-python-starter-service-2.1.1/starter_service/avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3931 2023-06-16 19:55:26.000000 osint-python-starter-service-2.1.1/starter_service/base_service.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1837 2023-06-07 19:08:41.000000 osint-python-starter-service-2.1.1/starter_service/env.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:50:27.025897 osint-python-starter-service-2.1.1/starter_service/examples/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.1.1/starter_service/examples/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      594 2023-06-07 19:05:41.000000 osint-python-starter-service-2.1.1/starter_service/examples/error.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1587 2023-06-16 20:48:31.000000 osint-python-starter-service-2.1.1/starter_service/examples/manual_api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1274 2023-06-07 20:59:38.000000 osint-python-starter-service-2.1.1/starter_service/examples/manual_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1212 2023-06-07 19:05:41.000000 osint-python-starter-service-2.1.1/starter_service/examples/multi.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1324 2023-06-07 19:08:41.000000 osint-python-starter-service-2.1.1/starter_service/examples/offset_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1156 2023-06-07 19:08:41.000000 osint-python-starter-service-2.1.1/starter_service/examples/single.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     5722 2023-06-17 00:50:00.000000 osint-python-starter-service-2.1.1/starter_service/kafka_adapter.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     7571 2023-04-25 06:06:55.000000 osint-python-starter-service-2.1.1/starter_service/schemas.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:50:27.025897 osint-python-starter-service-2.1.1/starter_service/tests/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 14:40:43.000000 osint-python-starter-service-2.1.1/starter_service/tests/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      560 2023-05-18 15:14:53.000000 osint-python-starter-service-2.1.1/starter_service/tests/employee.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      699 2023-06-03 20:55:03.000000 osint-python-starter-service-2.1.1/starter_service/tests/teet.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2885 2023-06-03 20:45:37.000000 osint-python-starter-service-2.1.1/starter_service/tests/test_avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      194 2023-05-18 14:41:17.000000 osint-python-starter-service-2.1.1/starter_service/tests/tst.py
```

### Comparing `osint-python-starter-service-2.1.0/LICENSE` & `osint-python-starter-service-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/PKG-INFO` & `osint-python-starter-service-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.1.0/README.md` & `osint-python-starter-service-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/osint_python_starter_service.egg-info/PKG-INFO` & `osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.1.0/osint_python_starter_service.egg-info/SOURCES.txt` & `osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 starter_service/__init__.py
 starter_service/api.py
 starter_service/api_server.py
 starter_service/avro_parser.py
 starter_service/base_service.py
 starter_service/env.py
 starter_service/kafka_adapter.py
-starter_service/messages.py
 starter_service/schemas.py
 starter_service/examples/__init__.py
 starter_service/examples/error.py
+starter_service/examples/manual_api.py
 starter_service/examples/manual_kafka.py
 starter_service/examples/multi.py
 starter_service/examples/offset_kafka.py
 starter_service/examples/single.py
 starter_service/tests/__init__.py
 starter_service/tests/employee.py
 starter_service/tests/teet.py
```

### Comparing `osint-python-starter-service-2.1.0/setup.py` & `osint-python-starter-service-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 setuptools.setup(
     name="osint-python-starter-service",
-    version="2.1.0",
+    version="2.1.1",
     author="mindpetk",
     author_email="petkeviciusm@gmail.com",
     description="Python starter service",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-starter-service",
     include_package_data=True,
```

### Comparing `osint-python-starter-service-2.1.0/starter_service/api.py` & `osint-python-starter-service-2.1.1/starter_service/api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/starter_service/api_server.py` & `osint-python-starter-service-2.1.1/starter_service/api_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,35 +6,34 @@
 from fastapi.encoders import jsonable_encoder
 from pydantic import ValidationError
 from starlette.responses import Response, JSONResponse
 from starlette.status import HTTP_200_OK
 
 from starter_service.api import API
 from starter_service.env import ENV
-from starter_service.messages import MessageHistory
 from starter_service.schemas import SchemaRegistry
 
 
 class APIServer:
 
     def __init__(self, name=None, ready: callable = None, health: callable = None, kafka_status: str = None,
                  base_service=None, callback=None, **kwargs):
         self.name = name
         self._validated()
-        self.app = FastAPI(title=self.name)
-        self.router = APIRouter()
+        self._fast_api = FastAPI(title=self.name)
+        self._router = APIRouter()
         self.callback = callback
 
-        @self.app.exception_handler(Exception)
+        @self._fast_api.exception_handler(Exception)
         async def validation_exception_handler(request, err):
             base_error_message = f"Failed to execute: {request.method}: {request.url}"
             # Change here to LOGGER
             return JSONResponse(status_code=400, content={"message": f"{base_error_message}. Detail: {err}"})
 
-        @self.app.exception_handler(ValidationError)
+        @self._fast_api.exception_handler(ValidationError)
         async def validation_exception_handler(request, err):
             base_error_message = f"Failed to execute: {request.method}: {request.url}"
             # Change here to LOGGER
             return JSONResponse(status_code=400, content={"message": f"{base_error_message}. Detail: {err}"})
 
         self.host = ENV.REST_API_HOST
         self.port = ENV.REST_API_PORT
@@ -46,22 +45,29 @@
 
         self._thread = None
         self._uptime = None
         self._running = False
         self._base_service = base_service
 
         self._register_static_routes()
-        self._register_message_routes()
         self._register_dynamic_routes()
-        self.app.include_router(self.router)
+        self._fast_api.include_router(self._router)
+
+    @property
+    def fast_api(self):
+        return self._fast_api
+
+    @property
+    def router(self):
+        return self._router
 
     def _register_static_routes(self):
         self._logger.info("Registering static routes")
 
-        @self.router.get("/")
+        @self._router.get("/")
         def root():
             return {
                 "client_id": ENV.CLIENT_ID,
                 "uptime": self._uptime,
                 "docs": "/docs",
                 "redoc": "/redoc",
                 "openapi": "/openapi.json",
@@ -82,27 +88,27 @@
                 },
                 "environment": {key: value for key, value in ENV.__dict__.items() if
                                 not key.startswith("_") and key not in ["SET", "GET", "update"]},
                 "schemas:": SchemaRegistry.get_schemas_dict(),
                 "methods": API.functions
             }
 
-        @self.router.get("/api/health", tags=["status"])
+        @self._router.get("/api/health", tags=["status"])
         def health(verbose: bool = False):
             """Return health status"""
             health = self._health()
             if health:
                 if verbose:
                     return health
                 else:
                     return Response(status_code=HTTP_200_OK)
             else:
                 return Response(status_code=503)
 
-        @self.router.get("/api/ready", tags=["status"])
+        @self._router.get("/api/ready", tags=["status"])
         def ready():
             """Return 200 OK if server is ready"""
             response = self._ready()
             if response:
                 return Response(status_code=HTTP_200_OK)
             else:
                 return Response(status_code=503)
@@ -119,15 +125,15 @@
     def stop(self):
         self._logger.info("Stopping API server")
         self._running = False
         self._thread.join()
 
     def _run(self):
         import uvicorn
-        uvicorn.run(self.app, host=ENV.REST_API_HOST, port=ENV.REST_API_PORT)
+        uvicorn.run(self._fast_api, host=ENV.REST_API_HOST, port=ENV.REST_API_PORT)
 
     def _validated(self):
         """Validate that the server is configured correctly"""
         if ENV.REST_API_ENABLED is False:
             raise Exception("REST API is disabled. To enable REST API set REST_API_ENABLED to true")
 
     def _register_dynamic_routes(self):
@@ -143,40 +149,9 @@
 
         self._logger.info(f"Registering route {consumer}:{consumer_class} -> {producer}:{producer_class} ({doc})")
         func_wrapper = lambda message: func(self._base_service, message) \
             if isinstance(message, str) else func(self._base_service, jsonable_encoder(message))
         path = f"/api{f'/{consumer}' if consumer else ''}{f'/{producer}' if producer else ''}"
 
         func_wrapper.__annotations__ = {'message': consumer_class, 'return': producer_class}
-        self.router.add_api_route(path, func_wrapper, methods=[_type], response_model=producer_class, tags=["topics"],
-                                  summary=doc)
-
-    def _register_message_routes(self):
-        # TODO fully test this
-        if not ENV.REST_LOG_MESSAGES:
-            return
-
-        @self.router.get("/api/messages/consume", tags=["messages"])
-        def consume():
-            """Return last consumed messages"""
-            return MessageHistory.get_incoming_messages()
-
-        @self.router.get("/api/messages/consume/{uuid}", tags=["messages"])
-        def consume_uuid(uuid: str):
-            """Return consumed message by uuid"""
-            msg = MessageHistory.get_incoming_message(uuid)
-            if msg:
-                return msg
-            return Response(status_code=404)
-
-        @self.router.get("/api/messages/produce", tags=["messages"])
-        def produce():
-            """Return last produced messages"""
-            return MessageHistory.get_outgoing_messages()
-
-        @self.router.get("/api/messages/produce/{uuid}", tags=["messages"])
-        def produce_uuid(uuid: str):
-            """Return produced message by uuid"""
-            msg = MessageHistory.get_outgoing_message(uuid)
-            if msg:
-                return msg
-            return Response(status_code=404)
+        self._router.add_api_route(path, func_wrapper, methods=[_type], response_model=producer_class, tags=["topics"],
+                                   summary=doc)
```

### Comparing `osint-python-starter-service-2.1.0/starter_service/avro_parser.py` & `osint-python-starter-service-2.1.1/starter_service/avro_parser.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/starter_service/base_service.py` & `osint-python-starter-service-2.1.1/starter_service/base_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,22 @@
         self._kafka = None
         self._api = None
         self._schemas = None
         self._functions = None
         self._initialize()
         self._schema_registry = None
 
+    @property
+    def api(self):
+        return self._api
+
+    @property
+    def kafka(self):
+        return self._kafka
+
     @abstractmethod
     def ready(self) -> bool:
         """Return True if service is ready to receive messages, False otherwise."""
         pass
 
     @abstractmethod
     def health(self) -> str:
@@ -62,14 +70,16 @@
             self._kafka.start()
             self.logger.info(f"Kafka initialized.")
         except Exception as e:
             _kafka_status = f"Error: {e}"
             _kafka_callback()
             self.logger.error(f'Error initializing kafka: {e}')
 
+        self.callback()
+
     def _register_api(self, _kafka_status, callback):
         try:
             self._api = APIServer(name=self.name, ready=self.ready, health=self.health, kafka_status=_kafka_status,
                                   base_service=self, callback=callback)
             self._api.start()
             self.logger.info(f"REST API initialized.")
         except Exception as e:
@@ -93,7 +103,11 @@
     def kafka_callback(self):
         """Override this method to callback after service is initialized"""
         pass
 
     def api_callback(self):
         """Override this method to callback after service is initialized"""
         pass
+
+    def callback(self):
+        """Override this method to callback after service is initialized"""
+        pass
```

### Comparing `osint-python-starter-service-2.1.0/starter_service/env.py` & `osint-python-starter-service-2.1.1/starter_service/env.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/starter_service/examples/error.py` & `osint-python-starter-service-2.1.1/starter_service/examples/error.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/starter_service/examples/manual_kafka.py` & `osint-python-starter-service-2.1.1/starter_service/examples/manual_kafka.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/starter_service/examples/multi.py` & `osint-python-starter-service-2.1.1/starter_service/examples/multi.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/starter_service/examples/offset_kafka.py` & `osint-python-starter-service-2.1.1/starter_service/examples/offset_kafka.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/starter_service/examples/single.py` & `osint-python-starter-service-2.1.1/starter_service/examples/single.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/starter_service/kafka_adapter.py` & `osint-python-starter-service-2.1.1/starter_service/kafka_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,63 +40,34 @@
         self._callback = callback
         self._base_service = base_service
 
     def start(self):
         """Start the service"""
         self._init_producers()
         self._test_bed_adapter.initialize()
-        listener_threads = []
-        run = True
 
         # Create threads for each consume topic
         for topic in ENV.CONSUME.split(','):
             topic = topic.strip()
             if not topic:
                 self.logger.warning("Empty topic, skipping")
                 continue
             _consumer = ConsumerManager(
                 options=self._test_bed_options,
                 kafka_topic=topic,
-                handle_message=self._handle_message,
-                run=lambda: run
+                handle_message=self._handle_message
             )
+            _consumer.start()
             self.logger.info(f"Registering schema from kafka for {topic}")
             SchemaRegistry.register_schema(_consumer.schema_str, topic)
             self.logger.info(f"Initializing listener for topic {topic}")
-            listener_threads.append(threading.Thread(
-                target=_consumer.listen)
-            )
-
-        # start all threads
-        for thread in listener_threads:
-            thread.daemon = True
-            thread.start()
 
         if self._callback:
             self._callback()
 
-        while run:
-            # make sure we check thread health every 10 sec
-            time.sleep(10)
-            for thread in listener_threads:
-                if not thread.is_alive():
-                    run = False
-                    self.logger.error("Thread died, shutting down")
-
-        # Stop test bed
-        self._test_bed_adapter.stop()
-        for producer in self._producers.values():
-            self.logger.info(f"Stopping producer {producer}")
-            producer.stop()
-
-        # Clean after ourselves
-        for thread in listener_threads:
-            thread.join()
-
-        raise Exception
 
     def send_message(self, message, topics=None, testing=False):
         """Send message to kafka topic"""
         if testing:
             self.logger.info(f"Sending test message to {topics}\n{message}")
             return
 
@@ -168,8 +139,8 @@
             try:
                 response = func(self._base_service, message)
                 if producer and response:
                     self.logger.info(f"Sending response: {producer}, {str(response)[:100]}")
                     self.send_message(response, topics=producer)
             except Exception as e:
                 traceback.print_exc()
-                self.logger.error(e)
+                self.logger.error(e)
```

### Comparing `osint-python-starter-service-2.1.0/starter_service/schemas.py` & `osint-python-starter-service-2.1.1/starter_service/schemas.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/starter_service/tests/employee.py` & `osint-python-starter-service-2.1.1/starter_service/tests/employee.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/starter_service/tests/teet.py` & `osint-python-starter-service-2.1.1/starter_service/tests/teet.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.0/starter_service/tests/test_avro_parser.py` & `osint-python-starter-service-2.1.1/starter_service/tests/test_avro_parser.py`

 * *Files identical despite different names*

