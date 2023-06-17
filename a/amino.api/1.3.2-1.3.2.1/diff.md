# Comparing `tmp/amino.api-1.3.2.tar.gz` & `tmp/amino.api-1.3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.api-1.3.2.tar", last modified: Fri Jun 16 16:41:20 2023, max compression
+gzip compressed data, was "amino.api-1.3.2.1.tar", last modified: Sat Jun 17 10:23:03 2023, max compression
```

## Comparing `amino.api-1.3.2.tar` & `amino.api-1.3.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 16:41:20.320867 amino.api-1.3.2/
--rw-rw-rw-   0        0        0      773 2023-06-16 16:41:20.321868 amino.api-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 16:41:20.264458 amino.api-1.3.2/amino/
--rw-rw-rw-   0        0        0      922 2023-06-16 16:39:59.000000 amino.api-1.3.2/amino/__init__.py
--rw-rw-rw-   0        0        0       50 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/async_client.py
--rw-rw-rw-   0        0        0       56 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/async_full_client.py
--rw-rw-rw-   0        0        0       59 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/async_local_client.py
--rw-rw-rw-   0        0        0       50 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/async_socket.py
--rw-rw-rw-   0        0        0    36040 2023-06-16 16:38:19.000000 amino.api-1.3.2/amino/client.py
--rw-rw-rw-   0        0        0    18999 2023-06-16 16:29:27.000000 amino.api-1.3.2/amino/full_client.py
--rw-rw-rw-   0        0        0    67936 2023-06-16 16:38:27.000000 amino.api-1.3.2/amino/local_client.py
--rw-rw-rw-   0        0        0    11538 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-16 16:41:20.318867 amino.api-1.3.2/amino/utils/
--rw-rw-rw-   0        0        0        0 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/utils/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/utils/exceptions.py
--rw-rw-rw-   0        0        0     7539 2023-06-16 16:28:31.000000 amino.api-1.3.2/amino/utils/helpers.py
--rw-rw-rw-   0        0        0    14913 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/utils/objects.py
--rw-rw-rw-   0        0        0     2302 2023-06-16 16:28:44.000000 amino.api-1.3.2/amino/utils/requester.py
--rw-rw-rw-   0        0        0     3660 2023-05-28 18:51:42.000000 amino.api-1.3.2/amino/utils/snippetTools.py
-drwxrwxrwx   0        0        0        0 2023-06-16 16:41:20.293464 amino.api-1.3.2/amino.api.egg-info/
--rw-rw-rw-   0        0        0      773 2023-06-16 16:41:18.000000 amino.api-1.3.2/amino.api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2023-06-16 16:41:19.000000 amino.api-1.3.2/amino.api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 16:41:18.000000 amino.api-1.3.2/amino.api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-16 16:41:18.000000 amino.api-1.3.2/amino.api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 16:41:18.000000 amino.api-1.3.2/amino.api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 16:41:20.323868 amino.api-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-06-16 16:40:44.000000 amino.api-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 10:23:03.091438 amino.api-1.3.2.1/
+-rw-rw-rw-   0        0        0      775 2023-06-17 10:23:03.092438 amino.api-1.3.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.3.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 10:23:03.040337 amino.api-1.3.2.1/amino/
+-rw-rw-rw-   0        0        0      924 2023-06-17 10:05:54.000000 amino.api-1.3.2.1/amino/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-05-28 18:51:42.000000 amino.api-1.3.2.1/amino/async_client.py
+-rw-rw-rw-   0        0        0       56 2023-05-28 18:51:42.000000 amino.api-1.3.2.1/amino/async_full_client.py
+-rw-rw-rw-   0        0        0       59 2023-05-28 18:51:42.000000 amino.api-1.3.2.1/amino/async_local_client.py
+-rw-rw-rw-   0        0        0       50 2023-05-28 18:51:42.000000 amino.api-1.3.2.1/amino/async_socket.py
+-rw-rw-rw-   0        0        0    36040 2023-06-17 10:07:23.000000 amino.api-1.3.2.1/amino/client.py
+-rw-rw-rw-   0        0        0    20660 2023-06-17 10:08:04.000000 amino.api-1.3.2.1/amino/full_client.py
+-rw-rw-rw-   0        0        0    68121 2023-06-17 10:11:46.000000 amino.api-1.3.2.1/amino/local_client.py
+-rw-rw-rw-   0        0        0    11538 2023-05-28 18:51:42.000000 amino.api-1.3.2.1/amino/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-17 10:23:03.090440 amino.api-1.3.2.1/amino/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-28 18:51:42.000000 amino.api-1.3.2.1/amino/utils/__init__.py
+-rw-rw-rw-   0        0        0     7226 2023-06-17 09:58:47.000000 amino.api-1.3.2.1/amino/utils/exceptions.py
+-rw-rw-rw-   0        0        0     7539 2023-06-17 10:13:06.000000 amino.api-1.3.2.1/amino/utils/helpers.py
+-rw-rw-rw-   0        0        0    14913 2023-05-28 18:51:42.000000 amino.api-1.3.2.1/amino/utils/objects.py
+-rw-rw-rw-   0        0        0     2302 2023-06-17 10:15:01.000000 amino.api-1.3.2.1/amino/utils/requester.py
+-rw-rw-rw-   0        0        0     3660 2023-05-28 18:51:42.000000 amino.api-1.3.2.1/amino/utils/snippetTools.py
+drwxrwxrwx   0        0        0        0 2023-06-17 10:23:03.067347 amino.api-1.3.2.1/amino.api.egg-info/
+-rw-rw-rw-   0        0        0      775 2023-06-17 10:23:01.000000 amino.api-1.3.2.1/amino.api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-06-17 10:23:02.000000 amino.api-1.3.2.1/amino.api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 10:23:01.000000 amino.api-1.3.2.1/amino.api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-17 10:23:01.000000 amino.api-1.3.2.1/amino.api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-17 10:23:01.000000 amino.api-1.3.2.1/amino.api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 10:23:03.093437 amino.api-1.3.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1605 2023-06-17 10:22:39.000000 amino.api-1.3.2.1/setup.py
```

### Comparing `amino.api-1.3.2/PKG-INFO` & `amino.api-1.3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.3.2
+Version: 1.3.2.1
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino.API</h1>
```

### Comparing `amino.api-1.3.2/amino/__init__.py` & `amino.api-1.3.2.1/amino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from json import loads
 from requests import get
 
 __title__ = 'amino.api'
 __author__ = 'Xsarz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Xsarz'
-__version__ = '1.3.2'
+__version__ = '1.3.2.1'
 __newest__ = loads(get("https://pypi.org/pypi/amino.api/json").text)["info"]["version"]
 
 
 
 if __version__ != __newest__:
 	s('cls || clear')
 	print(f'\033[38;5;214m{__title__} made by {__author__}\nPlease update the library. Your version: {__version__}  A new version:{__newest__}\033[0m')
```

### Comparing `amino.api-1.3.2/amino/client.py` & `amino.api-1.3.2.1/amino/client.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.3.2/amino/full_client.py` & `amino.api-1.3.2.1/amino/full_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from requests import Session
 from typing import Union, BinaryIO
 from base64 import b64encode
 from uuid import uuid4
 from io import BytesIO
 
 class FullClient(SocketHandler, Callbacks):
-	def __init__(self, language: str = 'ru', socket_enabled: bool = True, socket_debug: bool = False, socket_trace: bool = False,  auto_device: bool = False, deviceId: str = None, proxies: dict = None, certificatePath = None):
+	def __init__(self,  language: str = 'ru', socket_enabled: bool = True, socket_debug: bool = False, socket_trace: bool = False,  auto_device: bool = False, deviceId: str = None, proxies: dict = None, certificatePath = None):
 		self.session = Session()
 		self.profile = objects.profile()
 		self.req = Requester(session=self.session, deviceId=deviceId, auto_device=auto_device, proxies=proxies, verify=certificatePath, language=language)
 		self.socket_enabled = socket_enabled
 
 		SocketHandler.__init__(self, self.req, socket_trace, socket_debug)
 		Callbacks.__init__(self)
@@ -512,8 +512,59 @@
 		response = self.req.make_request(method="GET", endpoint=f"/g/s/topic/0/feed/community?size={size}&categoryKey=recommendation&type=discover&pagingType=t")
 		return objects.communityList(response.json())
 
 
 	def get_user_info(self, userId: str, comId: str = None):
 
 		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/user-profile/{userId}" if comId else f"/g/s/user-profile/{userId}")
-		return objects.UserProfile(response.json()["userProfile"])
+		return objects.UserProfile(response.json()["userProfile"])
+
+
+
+	def get_all_users(self, comId: Union[str, int], type: str = "recent", start: int = 0, size: int = 25):
+
+		if type not in ["recent", "banned", "featured", "leaders", "curators"]:raise exceptions.IncorrectType(type)
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/user-profile?type={type}&start={start}&size={size}")
+		return objects.userProfileList(response.json())
+
+
+	def get_online_users(self, comId: Union[str, int], start: int = 0, size: int = 25):
+
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/live-layer?topic=ndtopic:x{comId}:online-members&start={start}&size={size}")
+		return objects.userProfileList(response.json())
+
+
+
+
+
+	def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None, isGuest: bool = False, comId: Union[str, int] = None):
+		data = {
+			"content": message,
+			"stickerId": None,
+			"type": 0,
+			"timestamp": int(timestamp() * 1000)
+		}
+
+		if replyTo: data["respondTo"] = replyTo
+
+
+		comType = "g-comment" if comId is None else "g-comment" if isGuest else "comment"
+
+		if userId:
+			data["eventSource"] = "UserProfileView"
+			url = f"/s/user-profile/{userId}/{comType}"
+
+		elif blogId:
+			data["eventSource"] = "PostDetailView"
+			url = f"/s/blog/{blogId}/{comType}"
+
+		elif wikiId:
+			data["eventSource"] = "PostDetailView"
+			url = f"/s/item/{wikiId}/{comType}"
+
+		else: raise exceptions.IncorrectType()
+
+		if comId: url= f"/x{comId}"+ url
+		else:url= "/g" + url
+
+		response = self.req.make_request(method="POST", endpoint=url, body=dumps(data))
+		return response.status_code
```

### Comparing `amino.api-1.3.2/amino/local_client.py` & `amino.api-1.3.2.1/amino/local_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,28 @@
 from json import loads, dumps
 from requests import Session
 from base64 import b64encode
 from typing import BinaryIO, Union
 from uuid import uuid4
 from io import BytesIO
 from time import timezone
+
+
+
 class LocalClient(Client):
-	def __init__(self, comId: int, profile: objects.profile, deviceId: str = None, proxies: dict = None, certificatePath = None):
-		self.profile = profile
+	def __init__(self, comId: Union[str,int] = None, profile: objects.profile = None, language: str = 'ru', deviceId: str = None, proxies: dict = None, certificatePath = None):
+		self.profile = profile if profile else objects.profile()
+		self.comId = comId
+		Client.__init__(self, deviceId=deviceId, proxies=proxies, certificatePath=certificatePath,  language=language)
+
+
+	def set_comId(self, comId: Union[str,int] = None):
 		self.comId = comId
-		Client.__init__(self, deviceId=deviceId, proxies=proxies, certificatePath=certificatePath)
+		return self.comId
+
 
 	def join_chat(self, chatId: str):
 		response = self.req.make_request(method="POST", endpoint=f"/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", type="application/x-www-form-urlencoded")
 		return response.status_code
 
 	def leave_chat(self, chatId: str):
 		response = self.req.make_request(method="DELETE", endpoint=f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}")
@@ -306,26 +315,14 @@
 
 	def view_wiki(self, wikiId: str):
 		response = self.req.make_request(method="GET", endpoint=f"/x{self.comId}/s/item/{wikiId}")
 		return response.json()
 
 
 
-
-
-
-
-
-
-
-
-
-
-
-
 	def get_invite_codes(self, status: str = "normal", start: int = 0, size: int = 25):
 		response = self.req.make_request(method="GET", endpoint=f"/g/s-x{self.comId}/community/invitation?status={status}&start={start}&size={size}")
 		return response.json()["communityInvitationList"]
 
 
 	def generate_invite_code(self, duration: int = 0, force: bool = True):
 		data = dumps({
```

### Comparing `amino.api-1.3.2/amino/socket.py` & `amino.api-1.3.2.1/amino/socket.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.3.2/amino/utils/helpers.py` & `amino.api-1.3.2.1/amino/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.3.2/amino/utils/objects.py` & `amino.api-1.3.2.1/amino/utils/objects.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.3.2/amino/utils/requester.py` & `amino.api-1.3.2.1/amino/utils/requester.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.3.2/amino/utils/snippetTools.py` & `amino.api-1.3.2.1/amino/utils/snippetTools.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.3.2/amino.api.egg-info/PKG-INFO` & `amino.api-1.3.2.1/amino.api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.3.2
+Version: 1.3.2.1
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino.API</h1>
```

### Comparing `amino.api-1.3.2/amino.api.egg-info/SOURCES.txt` & `amino.api-1.3.2.1/amino.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.api-1.3.2/setup.py` & `amino.api-1.3.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 info = {
 	"name": "amino.api",
-	"version": "1.3.2",
+	"version": "1.3.2.1",
 	"github_page": "https://github.com/xXxCLOTIxXx/amino.api",
 	"download_link": "https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip",
 	"license": "MIT",
 	"author": "Xsarz",
 	"author_email": "xsarzy@gmail.com",
 	"description": "Library for creating amino bots and scripts.",
 	"long_description": None,
```

