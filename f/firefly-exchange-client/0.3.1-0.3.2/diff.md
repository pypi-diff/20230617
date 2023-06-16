# Comparing `tmp/firefly_exchange_client-0.3.1.tar.gz` & `tmp/firefly_exchange_client-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefly_exchange_client-0.3.1.tar", last modified: Tue Jun  6 11:22:30 2023, max compression
+gzip compressed data, was "firefly_exchange_client-0.3.2.tar", last modified: Fri Jun 16 22:30:55 2023, max compression
```

## Comparing `firefly_exchange_client-0.3.1.tar` & `firefly_exchange_client-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:22:30.321473 firefly_exchange_client-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-06 11:22:30.321473 firefly_exchange_client-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:22:30.321473 firefly_exchange_client-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:22:30.317473 firefly_exchange_client-0.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:22:30.317473 firefly_exchange_client-0.3.1/src/firefly_exchange_client/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/api_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    36516 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/contract_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/onboarding_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/order_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/socket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-06 11:22:19.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:22:30.317473 firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-06 11:22:30.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-06 11:22:30.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:22:30.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 11:22:30.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 11:22:30.000000 firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:55.903680 firefly_exchange_client-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-16 22:30:55.903680 firefly_exchange_client-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 22:30:55.903680 firefly_exchange_client-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:55.899680 firefly_exchange_client-0.3.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:55.899680 firefly_exchange_client-0.3.2/src/firefly_exchange_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36559 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/contract_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/onboarding_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/order_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/socket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:55.903680 firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-16 22:30:55.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-16 22:30:55.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 22:30:55.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 22:30:55.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 22:30:55.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/top_level.txt
```

### Comparing `firefly_exchange_client-0.3.1/LICENSE` & `firefly_exchange_client-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/PKG-INFO` & `firefly_exchange_client-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly_exchange_client
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `firefly_exchange_client-0.3.1/README.md` & `firefly_exchange_client-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/pyproject.toml` & `firefly_exchange_client-0.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "firefly_exchange_client"
-version = "0.3.1"
+version = "0.3.2"
 description = "Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["firefly", "exchange", "decentralized", "perpetuals", "blockchain"]
 dependencies = [
   'web3 ~= 5.31.3',
   'requests ~= 2.28.1',
```

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/api_service.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/api_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,105 @@
+import json
 import aiohttp
 from .interfaces import *
 
+
 class APIService():
     def __init__(self, url):
         self.server_url = url
         self.auth_token = None
-        self.client = aiohttp.ClientSession() 
+        self.client = aiohttp.ClientSession()
 
     async def close_session(self):
         if self.client is not None:
             return await self.client.close()
 
     async def get(self, service_url, query={}, auth_required=False):
         """
             Makes a GET request and returns the results
             Inputs:
                 - service_url(str): the url to make the request to.
                 - query(dict): the get query.
-                - auth_required(bool): indicates whether authorization is required for the call or not.  
+                - auth_required(bool): indicates whether authorization is required for the call or not.
         """
         url = self._create_url(service_url)
 
         response = None
         if auth_required:
             response = await self.client.get(
-                url, 
-                params=query, 
+                url,
+                params=query,
                 headers={'Authorization': 'Bearer {}'.format(self.auth_token)})
         else:
             response = await self.client.get(url, params=query)
 
         try:
-            if response.status != 503: #checking for service unavailitbility 
+            if response.status != 503:  # checking for service unavailitbility
                 return await response.json()
             else:
-               return response
+                return response
         except:
             raise Exception("Error while getting {}: {}".format(url, response))
-        
-    async def post(self, service_url, data, auth_required=False):
+
+    async def post(self, service_url, data, auth_required=False, contentType = ""):
         """
             Makes a POST request and returns the results
             Inputs:
                 - service_url(str): the url to make the request to.
                 - data(dict): the data to post with POST request.
                 - auth_required(bool): indicates whether authorization is required for the call or not.
         """
         url = self._create_url(service_url)
         response = None
-
         if auth_required:
-            response = await self.client.post(
-                url=url, 
-                data=data, 
-                headers={'Authorization': 'Bearer {}'.format(self.auth_token),'Content-type': 'application/json'})
+            headers = {'Authorization': 'Bearer {}'.format(self.auth_token)}
+
+            if contentType is not "":
+               headers['Content-type'] = contentType
+
+            response = await self.client.post(url=url, data=data, headers=headers)
         else:
             response = await self.client.post(url=url, data=data)
 
         try:
-            if response.status != 503: #checking for service unavailitbility 
+            if response.status != 503:  # checking for service unavailitbility
                 return await response.json()
             else:
-               return response
+                return response
         except:
-            raise Exception("Error while posting to {}: {}".format(url, response))
-        
-    async def delete(self,service_url, data, auth_required=False):
+            raise Exception(
+                "Error while posting to {}: {}".format(url, response))
+
+    async def delete(self, service_url, data, auth_required=False):
         """
             Makes a DELETE request and returns the results
             Inputs:
                 - service_url(str): the url to make the request to.
                 - data(dict): the data to post with POST request.
                 - auth_required(bool): indicates whether authorization is required for the call or not.
         """
         url = self._create_url(service_url)
 
         response = None
         if auth_required:
             response = await self.client.delete(
-                url=url, 
-                data=data, 
+                url=url,
+                data=data,
                 headers={'Authorization': 'Bearer {}'.format(self.auth_token)})
         else:
             response = await self.client.delete(url=url, data=data)
-        
+
         try:
             return await response.json()
         except:
-            raise Exception("Error while posting to {}: {}".format(url, response))
- 
+            raise Exception(
+                "Error while posting to {}: {}".format(url, response))
+
     '''
         Private methods
     '''
+
     def _create_url(self, path):
         """
             Appends namespace to server url
         """
         return "{}{}".format(self.server_url, path)
```

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/client.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -879,15 +879,16 @@
                 - PostTimerResponse: 
                     - acceptedToReset: array with symbols for which timer was reset successfully
                     - failedReset: aray with symbols for whcih timer failed to reset 
         """
         response = await self.dmsApi.post(
             SERVICE_URLS["USER"]["CANCEL_ON_DISCONNECT"],
             json.dumps(params),
-            auth_required=True   
+            auth_required=True,
+            contentType = 'application/json'
         )
         # check for service unavailibility
         if hasattr(response, 'status') and response.status == 503:
              raise Exception("Cancel on Disconnect (dead-mans-switch) feature is currently unavailable")
         return response
        
     ## Internal methods
```

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/constants.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/constants.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/contract_abis.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/contract_abis.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/contracts.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/contracts.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/enumerations.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/enumerations.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/interfaces.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,16 @@
 class GetUserTransferHistoryResponse(TypedDict):
   isMoreDataAvailable: bool # boolean indicating if there is more data available
   nextCursor: int # next page number
   data: List[UserTransferHistoryResponse]
 
 class CountDown(TypedDict):
   symbol: str
-  count: int
+  countDown: int
+
 class GetCancelOnDisconnectTimerRequest(TypedDict):
   symbol: MARKET_SYMBOLS  # will fetch Cancel On Disconnect Timer of provided market
   parentAddress: str # (optional) should be provided by a sub account 
 
 class PostTimerAttributes(TypedDict):
   countDowns: List[CountDown]
   parentAddress: str
```

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/onboarding_signer.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/onboarding_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/order_signer.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/order_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/signer.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/socket_manager.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/socket_manager.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/sockets.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/sockets.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/utilities.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/utilities.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client/websocket_client.py` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client/websocket_client.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/PKG-INFO` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly-exchange-client
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `firefly_exchange_client-0.3.1/src/firefly_exchange_client.egg-info/SOURCES.txt` & `firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

