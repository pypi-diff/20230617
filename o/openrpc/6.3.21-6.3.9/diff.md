# Comparing `tmp/openrpc-6.3.21.tar.gz` & `tmp/openrpc-6.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrpc-6.3.21.tar", max compression
+gzip compressed data, was "openrpc-6.3.9.tar", max compression
```

## Comparing `openrpc-6.3.21.tar` & `openrpc-6.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-06-17 01:04:15.422676 openrpc-6.3.21/LICENSE
--rw-r--r--   0        0        0     3211 2023-06-17 01:04:15.422676 openrpc-6.3.21/README.md
--rw-r--r--   0        0        0     1045 2023-06-17 01:04:15.422676 openrpc-6.3.21/openrpc/__init__.py
--rw-r--r--   0        0        0      183 2023-06-17 01:04:15.422676 openrpc-6.3.21/openrpc/_depends.py
--rw-r--r--   0        0        0    11449 2023-06-17 01:04:15.422676 openrpc-6.3.21/openrpc/_discover.py
--rw-r--r--   0        0        0     7539 2023-06-17 01:04:15.423676 openrpc-6.3.21/openrpc/_method_processor.py
--rw-r--r--   0        0        0     5590 2023-06-17 01:04:15.423676 openrpc-6.3.21/openrpc/_method_registrar.py
--rw-r--r--   0        0        0     9488 2023-06-17 01:04:15.423676 openrpc-6.3.21/openrpc/_objects.py
--rw-r--r--   0        0        0     7950 2023-06-17 01:04:15.423676 openrpc-6.3.21/openrpc/_request_processor.py
--rw-r--r--   0        0        0      280 2023-06-17 01:04:15.423676 openrpc-6.3.21/openrpc/_router.py
--rw-r--r--   0        0        0     1168 2023-06-17 01:04:15.423676 openrpc-6.3.21/openrpc/_rpcmethod.py
--rw-r--r--   0        0        0     9047 2023-06-17 01:04:15.423676 openrpc-6.3.21/openrpc/_server.py
--rw-r--r--   0        0        0        0 2023-06-17 01:04:15.446676 openrpc-6.3.21/openrpc/py.typed
--rw-r--r--   0        0        0     1103 2023-06-17 01:04:15.423676 openrpc-6.3.21/pyproject.toml
--rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 openrpc-6.3.21/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-10 02:23:48.038498 openrpc-6.3.9/LICENSE
+-rw-r--r--   0        0        0     3193 2023-03-10 02:23:48.039498 openrpc-6.3.9/README.md
+-rw-r--r--   0        0        0     1044 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/__init__.py
+-rw-r--r--   0        0        0      183 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_depends.py
+-rw-r--r--   0        0        0    11339 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_discover.py
+-rw-r--r--   0        0        0     7232 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_method_processor.py
+-rw-r--r--   0        0        0     5585 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_method_registrar.py
+-rw-r--r--   0        0        0     9488 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_objects.py
+-rw-r--r--   0        0        0     7045 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_request_processor.py
+-rw-r--r--   0        0        0      280 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_router.py
+-rw-r--r--   0        0        0     1168 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_rpcmethod.py
+-rw-r--r--   0        0        0     8406 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_server.py
+-rw-r--r--   0        0        0        0 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/py.typed
+-rw-r--r--   0        0        0     1102 2023-03-10 02:23:48.040499 openrpc-6.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4354 1970-01-01 00:00:00.000000 openrpc-6.3.9/PKG-INFO
```

### Comparing `openrpc-6.3.21/LICENSE` & `openrpc-6.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openrpc-6.3.21/README.md` & `openrpc-6.3.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,18 +42,18 @@
 from openrpc import RPCServer
 
 rpc = RPCServer(title="Demo Server", version="1.0.0")
 ```
 
 ### Register a function as an RPC Method
 
-To register a method with the RPCServer add the `@rpc.method()` decorator to a function.
+To register a method with the RPCServer add the `@rpc.method` decorator to a function.
 
 ```python
-@rpc.method()
+@rpc.method
 def add(a: int, b: int) -> int:
     return a + b
 ```
 
 ### Process JSON RPC Request
 
 OpenRPC is transport agnostic. To use it, pass JSON RPC requests as strings or byte
@@ -93,15 +93,15 @@
 from openrpc import RPCServer
 from sanic import Request, Sanic, Websocket
 
 app = Sanic("DemoServer")
 rpc = RPCServer(title="DemoServer", version="1.0.0")
 
 
-@rpc.method()
+@rpc.method
 async def add(a: int, b: int) -> int:
     return a + b
 
 
 @app.websocket("/api/v1/")
 async def process_websocket(_request: Request, ws: Websocket) -> None:
     async for msg in ws:
@@ -115,18 +115,15 @@
 
 Example In
 
 ```json
 {
   "id": 1,
   "method": "add",
-  "params": {
-    "a": 1,
-    "b": 3
-  },
+  "params": {"a": 1, "b": 3},
   "jsonrpc": "2.0"
 }
 ```
 
 Example Result Out
 
 ```json
```

### Comparing `openrpc-6.3.21/openrpc/__init__.py` & `openrpc-6.3.9/openrpc/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,31 @@
 """Provides OpenRPC objects and the RPCServer class."""
+from openrpc._depends import Depends
+from openrpc._objects import (
+    ComponentsObject,
+    ContactObject,
+    ContentDescriptorObject,
+    ErrorObject,
+    ExampleObject,
+    ExamplePairingObject,
+    ExternalDocumentationObject,
+    InfoObject,
+    LicenseObject,
+    LinkObject,
+    MethodObject,
+    OpenRPCObject,
+    ParamStructure,
+    ReferenceObject,
+    SchemaObject,
+    ServerObject,
+    ServerVariableObject,
+    TagObject,
+)
+from openrpc._router import RPCRouter
+from openrpc._server import RPCServer
 
 __all__ = (
     "ComponentsObject",
     "ContactObject",
     "ContentDescriptorObject",
     "ErrorObject",
     "ExampleObject",
@@ -19,31 +42,7 @@
     "ReferenceObject",
     "SchemaObject",
     "ServerObject",
     "ServerVariableObject",
     "TagObject",
     "Depends",
 )
-
-from openrpc._depends import Depends
-from openrpc._objects import (
-    ComponentsObject,
-    ContactObject,
-    ContentDescriptorObject,
-    ErrorObject,
-    ExampleObject,
-    ExamplePairingObject,
-    ExternalDocumentationObject,
-    InfoObject,
-    LicenseObject,
-    LinkObject,
-    MethodObject,
-    OpenRPCObject,
-    ParamStructure,
-    ReferenceObject,
-    SchemaObject,
-    ServerObject,
-    ServerVariableObject,
-    TagObject,
-)
-from openrpc._router import RPCRouter
-from openrpc._server import RPCServer
```

### Comparing `openrpc-6.3.21/openrpc/_discover.py` & `openrpc-6.3.9/openrpc/_discover.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Handle the OpenRPC "rpc.discover" method."""
-
-__all__ = ("DiscoverHandler",)
-
+import copy
 import inspect
 from enum import Enum
 from typing import (
     Any,
     Callable,
     get_args,
     get_origin,
@@ -25,14 +23,15 @@
     MethodObject,
     OpenRPCObject,
     SchemaObject,
     SchemaType,
 )
 from openrpc._rpcmethod import RPCMethod
 
+__all__ = ("DiscoverHandler",)
 NoneType = type(None)
 
 
 class DiscoverHandler:
     """Used to discover an OpenRPC API."""
 
     def __init__(self, info: InfoObject, functions: Iterable[RPCMethod]) -> None:
@@ -41,30 +40,30 @@
         :param info: OpenRPC info object.
         :param functions: Functions to include in discover.
         """
         self._info = info
         self._methods: list[MethodObject] = []
         self._schemas: dict[str, SchemaObject] = {}
         self._flattened_schemas: dict[str, SchemaType] = {}
-        self._collect_schemas(functions)
+        self._collect_schemas(copy.deepcopy(list(functions)))
         for schema in self._schemas.values():
             self._flatten_schema(schema)
 
     def execute(self) -> OpenRPCObject:
         """Get an OpenRPCObject describing this API."""
         return OpenRPCObject(
             openrpc="1.2.6",
             info=self._info,
             methods=[
                 method for method in self._methods if method.name != "rpc.discover"
             ],
             components=ComponentsObject(schemas=self._flattened_schemas),
         )
 
-    def _collect_schemas(self, functions: Iterable[RPCMethod]) -> None:
+    def _collect_schemas(self, functions: list[RPCMethod]) -> None:
         for func in functions:
             params = self._get_params(func.function)
             result = self._get_result(func.function)
             method = MethodObject(
                 **{**func.metadata.dict(), **{"params": params, "result": result}}
             )
             self._methods.append(method)
@@ -193,21 +192,15 @@
         return "object"
     if NoneType is annotation:
         return "null"
     return py_to_schema.get(annotation) or "object"
 
 
 def _is_required(annotation: Any) -> bool:
-    def _get_name(arg: Any) -> str:
-        try:
-            return arg.__name__
-        except AttributeError:
-            return ""
-
-    return "NoneType" not in [_get_name(a) for a in get_args(annotation)]
+    return "NoneType" not in [a.__name__ for a in get_args(annotation)]
 
 
 def _update_references(
     schema: SchemaType,
     reference_to_consolidated_schema: dict[str, SchemaType],
 ) -> None:
     if isinstance(schema, bool):
```

### Comparing `openrpc-6.3.21/openrpc/_method_processor.py` & `openrpc-6.3.9/openrpc/_method_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 """Provide JSON-RPC2 server class."""
-
-__all__ = ("MethodProcessor",)
-
 import asyncio
 import json
 import logging
 from json import JSONDecodeError
 from typing import Any, Optional, Union
 
 from jsonrpcobjects.errors import INVALID_REQUEST, METHOD_NOT_FOUND, PARSE_ERROR
@@ -20,29 +17,28 @@
     RequestType,
 )
 from pydantic import ValidationError
 
 from openrpc._request_processor import RequestProcessor
 from openrpc._rpcmethod import RPCMethod
 
+__all__ = ("MethodProcessor",)
+
+
 log = logging.getLogger("openrpc")
 NotificationTypes = (NotificationObject, NotificationObjectParams)
 RequestTypes = (RequestObject, RequestObjectParams)
 _DEFAULT_ERROR_CODE = -32000
 
 
 class MethodProcessor:
     """Class to register and execute methods."""
 
-    def __init__(self, debug: bool) -> None:
-        """Init a MethodProcessor.
-
-        :param debug: Include internal error details in responses.
-        """
-        self.debug = debug
+    def __init__(self) -> None:
+        """Init a MethodProcessor."""
         self.methods: dict[str, RPCMethod] = {}
         self.uncaught_error_code = _DEFAULT_ERROR_CODE
 
     def method(self, func: RPCMethod, method_name: str) -> None:
         """Register a method with this server for later calls.
 
         :param func: Function to call for this method.
@@ -74,19 +70,15 @@
                     continue
                 if req.method not in self.methods:
                     if isinstance(req, (RequestObject, RequestObjectParams)):
                         results.append(_get_method_not_found_error(req))
                     continue
 
                 resp = RequestProcessor(
-                    self.methods[req.method],
-                    self.uncaught_error_code,
-                    req,
-                    depends,
-                    self.debug,
+                    self.methods[req.method], self.uncaught_error_code, req, depends
                 ).execute()
                 # If resp is None, request is a notification.
                 if resp is not None:
                     results.append(resp)
             return f"[{','.join(results)}]"
 
         # Single Request
@@ -94,19 +86,15 @@
         if isinstance(request, ErrorResponseObject):
             return request.json()
         if request.method not in self.methods:
             if isinstance(request, (RequestObject, RequestObjectParams)):
                 return _get_method_not_found_error(request)
             return None
         result = RequestProcessor(
-            self.methods[request.method],
-            self.uncaught_error_code,
-            request,
-            depends,
-            self.debug,
+            self.methods[request.method], self.uncaught_error_code, request, depends
         ).execute()
         return None if isinstance(request, NotificationTypes) else result
 
     async def process_async(
         self, data: Union[bytes, str], depends: Optional[dict[str, Any]]
     ) -> Optional[str]:
         """Process a JSON-RPC2 request and get the response.
@@ -133,19 +121,19 @@
                     if isinstance(request, (RequestObject, RequestObjectParams)):
                         return _get_method_not_found_error(request)
                     return None
 
                 method = self.methods[request.method]
                 if isinstance(request, RequestTypes):
                     return await RequestProcessor(
-                        method, self.uncaught_error_code, request, depends, self.debug
+                        method, self.uncaught_error_code, request, depends
                     ).execute_async()
                 # To get here, request must be a notification.
                 await RequestProcessor(
-                    method, self.uncaught_error_code, request, depends, self.debug
+                    method, self.uncaught_error_code, request, depends
                 ).execute_async()
 
             results = await asyncio.gather(
                 *[_process_request(_get_request_object(it)) for it in parsed_json]
             )
             return f"[{','.join(str(r) for r in results if r is not None)}]"
 
@@ -154,15 +142,15 @@
         if isinstance(req, ErrorResponseObject):
             return req.json()
         if req.method not in self.methods:
             if isinstance(req, (RequestObject, RequestObjectParams)):
                 return _get_method_not_found_error(req)
             return None
         result = await RequestProcessor(
-            self.methods[req.method], self.uncaught_error_code, req, depends, self.debug
+            self.methods[req.method], self.uncaught_error_code, req, depends
         ).execute_async()
         return None if isinstance(req, NotificationTypes) else result
 
 
 def _get_method_not_found_error(req: Union[NotificationType, RequestType]) -> str:
     return ErrorResponseObject(
         id=None if isinstance(req, NotificationTypes) else req.id,
```

### Comparing `openrpc-6.3.21/openrpc/_method_registrar.py` & `openrpc-6.3.9/openrpc/_method_registrar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 """Module providing method registrar interface."""
-
-__all__ = ("MethodRegistrar", "CallableType")
-
 import inspect
 import logging
 from functools import partial
 from typing import Callable, Optional, TypeVar, Union
 
 from openrpc import Depends
 from openrpc._method_processor import MethodProcessor
@@ -17,27 +14,30 @@
     LinkObject,
     ParamStructure,
     ServerObject,
     TagObject,
 )
 from openrpc._rpcmethod import MethodMetaData, RPCMethod
 
+__all__ = ("MethodRegistrar", "CallableType")
+
+
 log = logging.getLogger("openrpc")
 
 CallableType = TypeVar("CallableType", bound=Callable)
 DecoratedCallableType = TypeVar("DecoratedCallableType", bound=Callable)
 
 
 class MethodRegistrar:
     """Interface for registering RPC methods."""
 
     def __init__(self) -> None:
         """Initialize a new instance of the MethodRegistrar class."""
         self._rpc_methods: dict[str, RPCMethod] = {}
-        self._method_processor = MethodProcessor(False)
+        self._method_processor = MethodProcessor()
 
     def method(
         self,
         *args: CallableType,
         name: Optional[str] = None,
         params: Optional[list[ContentDescriptorObject]] = None,
         result: Optional[ContentDescriptorObject] = None,
```

### Comparing `openrpc-6.3.21/openrpc/_objects.py` & `openrpc-6.3.9/openrpc/_objects.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 """Python class representations of OpenRPC and JSON Schema objects."""
 from __future__ import annotations
 
+from enum import Enum
+from typing import Any, Optional, Union
+
+from pydantic import BaseModel, Field
+
 __all__ = (
     "ComponentsObject",
     "ContactObject",
     "ContentDescriptorObject",
     "ErrorObject",
     "ExampleObject",
     "ExamplePairingObject",
@@ -19,19 +24,14 @@
     "SchemaObject",
     "SchemaType",
     "ServerObject",
     "ServerVariableObject",
     "TagObject",
 )
 
-from enum import Enum
-from typing import Any, Optional, Union
-
-from pydantic import BaseModel, Field
-
 SchemaType = Union["SchemaObject", bool]
 
 
 class ParamStructure(Enum):
     """OpenRPC method param structure options."""
 
     BY_NAME = "by-name"
```

### Comparing `openrpc-6.3.21/openrpc/_request_processor.py` & `openrpc-6.3.9/openrpc/_request_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,38 @@
 """Provides RequestProcessor class for processing a single request."""
-
-__all__ = ("RequestProcessor",)
-
 import inspect
 import logging
 from enum import Enum
 from typing import (
     Any,
     get_args,
     get_origin,
     get_type_hints,
     Optional,
     Type,
     Union,
 )
 
-from jsonrpcobjects.errors import (
-    INTERNAL_ERROR,
-    InternalError,
-    InvalidParams,
-    JSONRPCError,
-)
+from jsonrpcobjects.errors import INTERNAL_ERROR, InternalError, JSONRPCError
 from jsonrpcobjects.objects import (
-    ErrorObject,
     ErrorObjectData,
     ErrorResponseObject,
-    ErrorType,
     NotificationObject,
     NotificationObjectParams,
     NotificationType,
     RequestObject,
     RequestObjectParams,
     RequestType,
     ResultResponseObject,
 )
 
-from openrpc import ParamStructure
 from openrpc._rpcmethod import RPCMethod
 
+__all__ = ("RequestProcessor",)
 log = logging.getLogger("openrpc")
-by_position_error = ErrorObjectData(
-    code=-32602, message="Invalid params", data="Params must be passed by position."
-)
-by_name_error = ErrorObjectData(
-    code=-32602, message="Invalid params", data="Params must be passed by name."
-)
 
 
 class DeserializationError(InternalError):
     """Raised when a request param cannot be deserialized."""
 
     def __init__(self, param: Any, p_type: Any) -> None:
         msg = f"Failed to deserialize request param [{param}] to type [{p_type}]"
@@ -71,25 +55,22 @@
 
     def __init__(
         self,
         method: RPCMethod,
         uncaught_error_code: int,
         request: Union[RequestType, NotificationType],
         depends_values: Optional[dict[str, Any]],
-        debug: bool,
     ) -> None:
         """Init a request processor.
 
         :param method: The Python callable.
         :param uncaught_error_code: Code for errors raised by method.
         :param request: Request to execute.
         :param depends_values: Values passed to functions with dependencies.
-        :param debug: Include internal error details in responses.
         """
-        self.debug = debug
         self.method = method
         self.request = request
         self.uncaught_error_code = uncaught_error_code
         self.depends = depends_values or {}
 
     def execute(self) -> Optional[str]:
         """Execute the method and get the JSON-RPC2 response."""
@@ -133,22 +114,18 @@
                 f" for method [{self.method.metadata.name}]"
             )
         dependencies = {k: self.depends.get(k) for k in self.method.depends_params}
         # Call method.
         if isinstance(self.request, (RequestObject, NotificationObject)):
             result = self.method.function(**dependencies)
         elif isinstance(self.request.params, list):
-            if self.method.metadata.param_structure == ParamStructure.BY_NAME:
-                raise InvalidParams(by_name_error)
             params = self._get_list_params(self.request.params, annotations)
             result = self.method.function(*params, **dependencies)
             params_msg = ", ".join(str(p) for p in params)
         else:
-            if self.method.metadata.param_structure == ParamStructure.BY_POSITION:
-                raise InvalidParams(by_position_error)
             params = self._get_dict_params(self.request.params, annotations)
             result = self.method.function(**params, **dependencies)
             params_msg = ", ".join(f"{k}={v}" for k, v in params.items())
 
         # Logging
         id_msg = "None"
         if isinstance(self.request, (RequestObject, RequestObjectParams)):
@@ -161,25 +138,22 @@
 
     def _get_error_response(self, error: Exception) -> Optional[str]:
         log.exception("%s:", type(error).__name__)
         if not isinstance(self.request, (RequestObjectParams, RequestObject)):
             return None
         if isinstance(error, JSONRPCError):
             return ErrorResponseObject(id=self.request.id, error=error.rpc_error).json()
-        if self.debug:
-            error_object: ErrorType = ErrorObjectData(
+        return ErrorResponseObject(
+            id=self.request.id,
+            error=ErrorObjectData(
                 code=self.uncaught_error_code,
                 message="Server error",
                 data=f"{type(error).__name__}: {error}",
-            )
-        else:
-            error_object = ErrorObject(
-                code=self.uncaught_error_code, message="Server error"
-            )
-        return ErrorResponseObject(id=self.request.id, error=error_object).json()
+            ),
+        ).json()
 
     def _get_list_params(self, params: list, annotations: dict) -> list:
         try:
             return [
                 self._deserialize(p, list(annotations.values())[i])
                 for i, p in enumerate(params)
             ]
```

### Comparing `openrpc-6.3.21/openrpc/_rpcmethod.py` & `openrpc-6.3.9/openrpc/_rpcmethod.py`

 * *Files identical despite different names*

### Comparing `openrpc-6.3.21/openrpc/_server.py` & `openrpc-6.3.9/openrpc/_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module providing RPCServer class."""
 import logging
 from typing import Any, Callable, Optional, Union
 
 from jsonrpcobjects.errors import INTERNAL_ERROR
-from jsonrpcobjects.objects import ErrorObject, ErrorObjectData, ErrorResponseObject
+from jsonrpcobjects.objects import ErrorObjectData
 
 from openrpc import RPCRouter
 from openrpc._discover import DiscoverHandler
 from openrpc._method_registrar import CallableType, MethodRegistrar
 from openrpc._objects import (
     ContactObject,
     ContentDescriptorObject,
@@ -31,30 +31,26 @@
         self,
         title: Optional[str] = None,
         version: Optional[str] = None,
         description: Optional[str] = None,
         terms_of_service: Optional[str] = None,
         contact: Optional[ContactObject] = None,
         license_: Optional[LicenseObject] = None,
-        debug: bool = False,
     ) -> None:
         """Init an OpenRPC server.
 
         :param title: OpenRPC title.
         :param version: API version.
         :param description: Description of the app.
         :param terms_of_service: App terms of service.
         :param contact: Contact information.
         :param license_: App license.
-        :param debug: Include internal error details in responses.
         """
         super().__init__()
-        self._method_processor.debug = debug
         # Set OpenRPC server info.
-        self._debug = debug
         self._info = InfoObject(
             title=title or "RPC Server",
             version=version or "0.1.0",
             description=description,
             termsOfService=terms_of_service,
             contact=contact,
             license=license_,
@@ -132,24 +128,14 @@
         self._method_processor.uncaught_error_code = default_error_code
 
     @property
     def methods(self) -> list[MethodObject]:
         """Get all methods of this server."""
         return DiscoverHandler(self._info, self._rpc_methods.values()).execute().methods
 
-    @property
-    def debug(self) -> bool:
-        """Include internal error details in responses if True."""
-        return self._debug
-
-    @debug.setter
-    def debug(self, debug: bool) -> None:
-        self._method_processor.debug = debug
-        self._debug = debug
-
     def include_router(
         self,
         router: RPCRouter,
         prefix: Optional[str] = None,
         tags: Optional[list[Union[TagObject, str]]] = None,
     ) -> None:
         """Add an RPC method router to this server.
@@ -209,15 +195,18 @@
         try:
             log.debug("Processing request: %s", data)
             resp = self._method_processor.process(data, depends)
             if resp:
                 log.debug("Responding: %s", resp)
             return resp
         except Exception as error:
-            return self._get_error_response(error).json()
+            log.exception("%s:", type(error).__name__)
+            error_object = ErrorObjectData(**INTERNAL_ERROR.dict())
+            error_object.data = f"{type(error).__name__}: {', '.join(error.args)}"
+            return error_object.json()
 
     async def process_request_async(
         self, data: Union[bytes, str], depends: Optional[dict[str, Any]] = None
     ) -> Optional[str]:
         """Process a JSON-RPC2 request and get the response.
 
         If the method called by the request is async it will be awaited.
@@ -231,29 +220,19 @@
         try:
             log.debug("Processing request: %s", data)
             resp = await self._method_processor.process_async(data, depends)
             if resp:
                 log.debug("Responding: %s", resp)
             return resp
         except Exception as error:
-            return self._get_error_response(error).json()
+            log.exception("%s:", type(error).__name__)
+            error_object = ErrorObjectData(**INTERNAL_ERROR.dict())
+            error_object.data = f"{type(error).__name__}: {', '.join(error.args)}"
+            return error_object.json()
 
     def discover(self) -> dict[str, Any]:
         """Execute "rpc.discover" method defined in OpenRPC spec."""
         return (
             DiscoverHandler(self._info, self._rpc_methods.values())
             .execute()
             .dict(by_alias=True, exclude_unset=True, exclude_none=True)
         )
-
-    def _get_error_response(self, error: Exception) -> ErrorResponseObject:
-        log.exception("%s:", type(error).__name__)
-        if self._debug:
-            error_object: Union[ErrorObject, ErrorObjectData] = ErrorObjectData(
-                **{
-                    **INTERNAL_ERROR.dict(),
-                    **{"data": f"{type(error).__name__}: {error}"},
-                }
-            )
-        else:
-            error_object = ErrorObject(**INTERNAL_ERROR.dict())
-        return ErrorResponseObject(id=None, error=error_object)
```

### Comparing `openrpc-6.3.21/pyproject.toml` & `openrpc-6.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openrpc"
-version = "6.3.21"
+version = "6.3.9"
 description = "OpenRPC provides classes to rapidly develop an OpenRPC server."
 readme = "README.md"
 repository = "https://gitlab.com/mburkard/openrpc"
 homepage = "https://gitlab.com/mburkard/openrpc"
 license = "MIT"
 authors = ["Matthew Burkard <matthewjburkard@gmail.com>"]
 classifiers = [
@@ -19,21 +19,21 @@
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1.10.6"
 jsonrpc2-objects = "^2.0.0"
-case-switcher = "^1.3.13"
+case-switcher = "^1.2.13"
 
 [tool.poetry.dev-dependencies]
 coverage = "^7.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 black = "^23.1.0"
 pytest = "^7.2.1"
-pytest-asyncio = "^0.21.0"
+pytest-asyncio = "^0.20.3"
 
 [build-system]
 
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openrpc-6.3.21/PKG-INFO` & `openrpc-6.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: openrpc
-Version: 6.3.21
+Version: 6.3.9
 Summary: OpenRPC provides classes to rapidly develop an OpenRPC server.
 Home-page: https://gitlab.com/mburkard/openrpc
 License: MIT
 Author: Matthew Burkard
 Author-email: matthewjburkard@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: case-switcher (>=1.3.13,<2.0.0)
+Requires-Dist: case-switcher (>=1.2.13,<2.0.0)
 Requires-Dist: jsonrpc2-objects (>=2.0.0,<3.0.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Project-URL: Repository, https://gitlab.com/mburkard/openrpc
 Description-Content-Type: text/markdown
 
 <div align=center>
   <h1>OpenRPC</h1>
@@ -67,18 +70,18 @@
 from openrpc import RPCServer
 
 rpc = RPCServer(title="Demo Server", version="1.0.0")
 ```
 
 ### Register a function as an RPC Method
 
-To register a method with the RPCServer add the `@rpc.method()` decorator to a function.
+To register a method with the RPCServer add the `@rpc.method` decorator to a function.
 
 ```python
-@rpc.method()
+@rpc.method
 def add(a: int, b: int) -> int:
     return a + b
 ```
 
 ### Process JSON RPC Request
 
 OpenRPC is transport agnostic. To use it, pass JSON RPC requests as strings or byte
@@ -118,15 +121,15 @@
 from openrpc import RPCServer
 from sanic import Request, Sanic, Websocket
 
 app = Sanic("DemoServer")
 rpc = RPCServer(title="DemoServer", version="1.0.0")
 
 
-@rpc.method()
+@rpc.method
 async def add(a: int, b: int) -> int:
     return a + b
 
 
 @app.websocket("/api/v1/")
 async def process_websocket(_request: Request, ws: Websocket) -> None:
     async for msg in ws:
@@ -140,18 +143,15 @@
 
 Example In
 
 ```json
 {
   "id": 1,
   "method": "add",
-  "params": {
-    "a": 1,
-    "b": 3
-  },
+  "params": {"a": 1, "b": 3},
   "jsonrpc": "2.0"
 }
 ```
 
 Example Result Out
 
 ```json
```

