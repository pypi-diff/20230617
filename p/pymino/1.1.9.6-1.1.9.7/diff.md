# Comparing `tmp/pymino-1.1.9.6.tar.gz` & `tmp/pymino-1.1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.9.4\dist\.tmp-jkpe4sap\pymino-1.1.9.6.tar", last modified: Thu Jun 15 01:48:57 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.9.6\dist\.tmp-lsxu854_\pymino-1.1.9.7.tar", last modified: Fri Jun 16 23:17:07 2023, max compression
```

## Comparing `pymino-1.1.9.6.tar` & `pymino-1.1.9.7.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 01:48:57.083114 pymino-1.1.9.6/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.9.6/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-06-15 01:48:57.083610 pymino-1.1.9.6/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.9.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 01:48:57.021114 pymino-1.1.9.6/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-15 01:48:31.000000 pymino-1.1.9.6/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.9.6/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30208 2023-06-15 01:47:51.000000 pymino-1.1.9.6/pymino/bot.py
--rw-rw-rw-   0        0        0    52073 2023-06-13 03:02:06.000000 pymino-1.1.9.6/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:48:57.053354 pymino-1.1.9.6/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-11 16:50:39.000000 pymino-1.1.9.6/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.9.6/pymino/ext/account.py
--rw-rw-rw-   0        0        0   287511 2023-06-08 12:33:03.000000 pymino-1.1.9.6/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.9.6/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    24041 2023-06-15 01:41:25.000000 pymino-1.1.9.6/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.9.6/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   292004 2023-06-11 18:06:25.000000 pymino-1.1.9.6/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-11 22:20:09.000000 pymino-1.1.9.6/pymino/ext/console.py
--rw-rw-rw-   0        0        0    41963 2023-06-11 20:52:12.000000 pymino-1.1.9.6/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.9.6/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:48:57.070218 pymino-1.1.9.6/pymino/ext/entities/
--rw-rw-rw-   0        0        0      312 2023-06-08 07:25:34.000000 pymino-1.1.9.6/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-08 12:22:47.000000 pymino-1.1.9.6/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    20323 2023-06-08 12:02:08.000000 pymino-1.1.9.6/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.9.6/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.9.6/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    16021 2023-06-10 00:36:20.000000 pymino-1.1.9.6/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.9.6/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-11 21:21:53.000000 pymino-1.1.9.6/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.9.6/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0    42516 2023-06-08 07:28:10.000000 pymino-1.1.9.6/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.9.6/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.9.6/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.9.6/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.9.6/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.9.6/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:48:57.082123 pymino-1.1.9.6/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-11 17:31:29.000000 pymino-1.1.9.6/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.9.6/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-13 04:27:21.000000 pymino-1.1.9.6/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.9.6/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-11 22:22:27.000000 pymino-1.1.9.6/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.9.6/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-11 21:47:35.000000 pymino-1.1.9.6/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-13 03:31:19.000000 pymino-1.1.9.6/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.9.6/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:48:57.037978 pymino-1.1.9.6/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-06-15 01:48:56.000000 pymino-1.1.9.6/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1323 2023-06-15 01:48:57.000000 pymino-1.1.9.6/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 01:48:56.000000 pymino-1.1.9.6/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-15 01:48:56.000000 pymino-1.1.9.6/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-15 01:48:56.000000 pymino-1.1.9.6/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-15 01:48:57.089562 pymino-1.1.9.6/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:17:07.373886 pymino-1.1.9.7/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.9.7/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-06-16 23:17:07.373886 pymino-1.1.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.9.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 23:17:07.307918 pymino-1.1.9.7/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-16 23:07:27.000000 pymino-1.1.9.7/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.9.7/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30208 2023-06-15 01:47:51.000000 pymino-1.1.9.7/pymino/bot.py
+-rw-rw-rw-   0        0        0    52363 2023-06-16 20:35:00.000000 pymino-1.1.9.7/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:17:07.336190 pymino-1.1.9.7/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-11 16:50:39.000000 pymino-1.1.9.7/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.9.7/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   306772 2023-06-16 23:13:50.000000 pymino-1.1.9.7/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.9.7/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    24095 2023-06-16 22:46:59.000000 pymino-1.1.9.7/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.9.7/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   305392 2023-06-16 23:13:10.000000 pymino-1.1.9.7/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-11 22:20:09.000000 pymino-1.1.9.7/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    42094 2023-06-16 22:12:03.000000 pymino-1.1.9.7/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.9.7/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:17:07.358510 pymino-1.1.9.7/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      355 2023-06-16 21:57:42.000000 pymino-1.1.9.7/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-06-16 23:16:13.000000 pymino-1.1.9.7/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     1670 2023-06-16 23:16:17.000000 pymino-1.1.9.7/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    20322 2023-06-16 23:16:20.000000 pymino-1.1.9.7/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.9.7/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.9.7/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15638 2023-06-16 21:42:30.000000 pymino-1.1.9.7/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.9.7/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-11 21:21:53.000000 pymino-1.1.9.7/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.9.7/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-06-16 21:57:33.000000 pymino-1.1.9.7/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-06-16 21:59:23.000000 pymino-1.1.9.7/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.9.7/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.9.7/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.9.7/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.9.7/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.9.7/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:17:07.372894 pymino-1.1.9.7/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-11 17:31:29.000000 pymino-1.1.9.7/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.9.7/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-13 04:27:21.000000 pymino-1.1.9.7/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.9.7/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-11 22:22:27.000000 pymino-1.1.9.7/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.9.7/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-11 21:47:35.000000 pymino-1.1.9.7/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-13 03:31:19.000000 pymino-1.1.9.7/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.9.7/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:17:07.319822 pymino-1.1.9.7/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-06-16 23:17:07.000000 pymino-1.1.9.7/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1380 2023-06-16 23:17:07.000000 pymino-1.1.9.7/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 23:17:07.000000 pymino-1.1.9.7/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-16 23:17:07.000000 pymino-1.1.9.7/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-16 23:17:07.000000 pymino-1.1.9.7/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-16 23:17:07.379838 pymino-1.1.9.7/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.9.7/setup.py
```

### Comparing `pymino-1.1.9.6/LICENSE` & `pymino-1.1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/PKG-INFO` & `pymino-1.1.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.9.6
+Version: 1.1.9.7
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.9.6 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.9.7 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.9.6/README.md` & `pymino-1.1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/__init__.py` & `pymino-1.1.9.7/pymino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.9.6'
+__version__ = '1.1.9.7'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.1.9.6/pymino/async_bot.py` & `pymino-1.1.9.7/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/bot.py` & `pymino-1.1.9.7/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/client.py` & `pymino-1.1.9.7/pymino/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -724,20 +724,22 @@
         """
         for key in ["sid", "userId", "community.userId", "request.sid", "request.userId", "is_authenticated"]:
             setattr(self, key, None)
         return None
 
 
     @authenticated
-    def join_community(self, community_id: int) -> ApiResponse:
+    def join_community(self, community_id: int, invitationId = None) -> ApiResponse:
         """
         Joins the user to a community with the provided community ID.
 
         :param community_id: The ID of the community to join.
         :type community_id: int
+        :param invitationId: The ID of the invitation link.
+        :type invitationId: str
         :return: An ApiResponse object containing the server response.
         :rtype: ApiResponse
         :raises LoginRequired: If the user is not logged in.
 
         This function first checks if the client is logged in by checking for a valid session ID. If not, it raises a
         LoginRequired exception.
 
@@ -745,18 +747,24 @@
         The request includes the client's session ID and the ID of the community to join.
 
         The function returns an ApiResponse object containing the server response.
 
         **Note:** This function can be used to join the user to a community with the provided community ID. Once joined,
         the user can make API calls related to the community, such as posting or retrieving posts.
         """
-        return ApiResponse(self.request.handler(
-            method="POST",
-            url=f"/x{community_id}/s/community/join"
-            ))
+        data = {"timestamp": int(time() * 1000)}
+        if invitationId:
+            data["invitationId"] = invitationId
+
+        return ApiResponse(
+            self.request.handler(
+                method="POST",
+                url=f"/x{community_id}/s/community/join",
+                data = data
+        ))
 
     @authenticated
     def leave_community(self, community_id: int) -> ApiResponse:
         """
         Leaves the user from a community with the provided community ID.
 
         :param community_id: The ID of the community to leave.
```

### Comparing `pymino-1.1.9.6/pymino/ext/account.py` & `pymino-1.1.9.7/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/async_community.py` & `pymino-1.1.9.7/pymino/ext/async_community.py`

 * *Files 0% similar despite different names*

```diff
@@ -2351,27 +2351,14 @@
             await self.session.handler(
             method="DELETE",
             url=f"/x{self.community_id if comId is None else comId}/s/block/{userId}"
             ))
 
 
     @community
-    async def post_blog(self, title: str, content: str, comId: Union[str, int] = None) -> CBlog: #TODO: ADD DOCSTRING
-        return CBlog(
-            await self.session.handler(
-            method="POST",
-            url=f"/x{self.community_id if comId is None else comId}/s/blog",
-            data={
-                "content": content,
-                "title": title,
-                "timestamp": int(time() * 1000)
-                }))
-
-
-    @community
     async def delete_blog(self, blogId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
         Deletes the specified blog.
 
         :param blogId: The ID of the blog to delete.
         :type blogId: str
         :param comId: The ID of the community to delete the blog from. If not provided, the current community ID is used.
@@ -6193,12 +6180,469 @@
             data["extensions"] = {
                 "customTitles": [
                     {"title": title, "color": color}
                     for title, color in zip(titles, colors)
                 ]
             }
 
-        return UserProfile(await self.session.handler(
-            method = "POST",
-            url = f"/x{self.community_id or comId}/s/user-profile/{self.userId}",
-            data = data
+        return UserProfile(
+            await self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id or comId}/s/user-profile/{self.userId}",
+                data = data
+        ))
+
+
+    @community
+    async def change_username(self, username: str, comId: Union[str, int] = None) -> UserProfile:
+        """
+        Edits the user profile username.
+
+        :param username: The new username for the user profile.
+        :type username: str
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile username.
+
+        `UserProfile`:
+
+        - `username` (str): The username of the user.
+
+        **Example usage:**
+
+        >>> profile = client.community.edit_profile_username("JohnDoe")
+        ... print(profile.username)
+        """
+        return await self.edit_profile(username=username, comId=comId)
+    
+
+    @community
+    async def change_icon(self, icon: str, comId: Union[str, int] = None) -> UserProfile:
+        """
+        Edits the user profile icon.
+
+        :param icon: The new icon image file for the user profile.
+        :type icon: str
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile icon.
+
+        `UserProfile`:
+
+        - `icon` (str): The URL of the icon image.
+
+        **Example usage:**
+
+        >>> profile = client.community.edit_profile_icon("path/to/icon.jpg")
+        ... print(profile.icon)
+        """
+        return await self.edit_profile(icon=icon, comId=comId)
+    
+
+    @community
+    async def edit_profile_background(self, backgroundImage: str, backgroundColor: str = None, comId: Union[str, int] = None) -> UserProfile:
+        """
+        Edits the user profile background.
+
+        :param backgroundImage: The new background image file for the user profile.
+        :type backgroundImage: str
+        :param backgroundColor: The new background color for the user profile.
+        :type backgroundColor: str
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile background.
+
+        `UserProfile`:
+
+        - `backgroundImage` (str): The URL of the background image.
+        - `backgroundColor` (str): The background color of the user profile.
+
+        **Example usage:**
+
+        >>> profile = client.community.edit_profile_background("path/to/background.jpg", "#FFFFFF")
+        ... print(profile.backgroundImage)
+        ... print(profile.backgroundColor)
+        """
+        return await self.edit_profile(backgroundImage=backgroundImage, backgroundColor=backgroundColor, comId=comId)
+    
+
+    @community
+    async def edit_profile_titles(self, titles: list, colors: list, comId: Union[str, int] = None) -> UserProfile:
+        """
+        Edits the user profile custom titles.
+
+        :param titles: A list of custom titles to set.
+        :type titles: list
+        :param colors: A list of colors corresponding to the custom titles.
+        :type colors: list
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile custom titles.
+
+        `UserProfile`:
+
+        - `titles` (list): A list of custom titles.
+        - `colors` (list): A list of colors corresponding to the custom titles.
+
+        **Example usage:**
+
+        >>> titles = ["Title 1", "Title 2"]
+        ... colors = ["#FF0000", "#00FF00"]
+        ... profile = client.community.edit_profile_titles(titles, colors)
+        ... print(profile.titles)
+        ... print(profile.colors)
+        """
+        return await self.edit_profile(titles=titles, colors=colors, comId=comId)
+    
+
+    @community
+    async def edit_profile_default_bubble(self, defaultBubbleId: str, comId: Union[str, int] = None) -> UserProfile:
+        """
+        Edits the user profile default bubble.
+
+        :param defaultBubbleId: The ID of the default bubble to set.
+        :type defaultBubbleId: str
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile default bubble.
+
+        `UserProfile`:
+
+        - `defaultBubbleId` (str): The ID of the default bubble.
+
+        **Example usage:**
+
+        >>> profile = client.community.edit_profile_default_bubble("bubble123")
+        ... print(profile.defaultBubbleId)
+        """
+        return await self.edit_profile(defaultBubbleId=defaultBubbleId, comId=comId)
+    
+
+    @community
+    async def chat_request_privilege(self, privilege: bool, comId: Union[str, int] = None) -> UserProfile:
+        """
+        Edits the user profile chat request privilege.
+
+        :param privilege: Whether or not to enable chat request privilege.
+        :type privilege: bool
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile chat request privilege.
+
+        `UserProfile`:
+
+        - `chatRequestPrivilege` (bool): Whether or not chat request privilege is enabled.
+
+        **Example usage:**
+
+        >>> profile = client.community.chat_request_privilege(True)
+        ... print(profile.chatRequestPrivilege)
+        """
+        return await self.edit_profile(chatRequestPrivilege=1 if privilege else 2, comId=comId)
+
+
+    @community
+    async def post_blog(self,
+                  title: str,
+                  content: str,
+                  imageList: list = None,
+                  captionList: list = None,
+                  categoriesList: list = None,
+                  backgroundColor: str = None,
+                  fansOnly: bool = False,
+                  extensions: dict = None,
+                  comId: Union[str, int] = None) -> CBlog:
+        """
+        Posts a blog in the community.
+
+        :param title: The title of the blog.
+        :type title: str
+        :param content: The content of the blog.
+        :type content: str
+        :param imageList: A list of image paths to include in the blog. (Optional)
+        :type imageList: list, optional
+        :param captionList: A list of captions corresponding to the images. (Optional)
+        :type captionList: list, optional
+        :param categoriesList: A list of category IDs to assign to the blog. (Optional)
+        :type categoriesList: list, optional
+        :param backgroundColor: The background color of the blog. (Optional)
+        :type backgroundColor: str, optional
+        :param fansOnly: Whether the blog is for fans only. (Default: False)
+        :type fansOnly: bool, optional
+        :param extensions: Additional extensions for the blog. (Optional)
+        :type extensions: dict, optional
+        :param comId: The ID of the community to post the blog in. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `CBlog` object representing the posted blog.
+        :rtype: CBlog
+
+        This function posts a blog in the specified community using the provided information.
+
+        `CBlog` represents a blog on the platform.
+
+        **Example usage:**
+
+        >>> blog = client.community.post_blog("My Blog", "This is the content of my blog.", imageList=["image1.jpg", "image2.jpg"])
+        ... print(blog.title)
+        ... print(blog.content)
+        """
+        media = []
+        if captionList is not None: media.append([100, await self.__handle_media__(image, "image/jpg", True), None] for image in captionList)
+        elif imageList is not None: media.append([100, await self.__handle_media__(image, "image/jpg", True), None] for image in imageList)
+
+        data = dict(address = None,
+                    content = content,
+                    title = title,
+                    mediaList = media,
+                    extensions = extensions,
+                    latitude = 0,
+                    longitude = 0,
+                    eventSource = "GlobalComposeMenu",
+                    timestamp = int(time() * 1000))
+        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+        if backgroundColor:
+            data["extensions"] = {
+                "style": {
+                    "backgroundColor": backgroundColor
+                    if backgroundColor.startswith("#")
+                    else f"#{backgroundColor}"
+                }
+            }
+        if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
+
+        return CBlog(
+            await self.session.handler(
+                method = "POST",
+                url = f"/x{comId or self.community_id}/s/blog",
+                data = data
+        ))
+
+
+    @community
+    async def fetch_invites(self, size: int = 25, status: str = "normal", start: int = 0, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Fetches generated invites for the community.
+
+        :param size: The number of invites to fetch. (Default: 25)
+        :type size: int, optional
+        :param status: The status of the invites to fetch. (Default: "normal")
+        :type status: str, optional
+        :param start: The index to start fetching invites from. (Default: 0)
+        :type start: int, optional
+
+        This function sends a GET request to the API to fetch generated invites for the community.
+
+        :returns: A `ApiResponse` object containing the API response.
+        :rtype: ApiResponse
+
+        `ApiResponse`:
+
+        - `code` (int): The status code of the API response.
+        - `api:status` (int): The status of the API response.
+        - `api:statuscode` (int): The status code of the API response.
+        - `api:message` (str): The message of the API response.
+        
+        **Example usage:**
+
+        >>> invites = client.community.fetch_invites()
+        ... print(invites.json()['communityInvitationList'])
+        ... for invite in invites.json()['communityInvitationList']:
+        ...     print(invite['invitationId'])
+        """
+        return ApiResponse(
+            await self.session.handler(
+                method = "GET",
+                url = f"http://service.aminoapps.com/api/v1/g/s-x{self.community_id or comId}/community/invitation?size={size}&status={status}&start={start}"
+        ))
+    
+
+    @community
+    async def revoke_invite(self, invitationId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Revokes an invite for the community.
+        
+        :param invitationId: The ID of the invite to revoke.
+        :type invitationId: str
+        :param comId: The ID of the community to revoke the invite in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `ApiResponse` object containing the API response.
+        :rtype: ApiResponse
+        
+        This function sends a DELETE request to the API to revoke an invite for the community.
+        
+        :returns: A `ApiResponse` object containing the API response.
+        :rtype: ApiResponse
+        
+        `ApiResponse`:
+        
+        - `code` (int): The status code of the API response.
+        - `api:status` (int): The status of the API response.
+        - `api:statuscode` (int): The status code of the API response.
+        - `api:message` (str): The message of the API response.
+        
+        **Example usage:**
+        
+        >>> client.community.revoke_invite("invitationId")
+        """
+        return ApiResponse(
+            await self.session.handler(
+                method = "DELETE",
+                url = f"http://service.aminoapps.com/api/v1/g/s-x{self.community_id or comId}/community/invitation/{invitationId}"
+        ))
+
+
+    @community
+    async def fetch_membership_requests(self, size: int = 25, status: str = "pending", start: int = 0, comId: Union[str, int] = None) -> CommunityMembershipRequestList:
+        """
+        Fetches membership requests for the community.
+        Used for approving or declining membership requests into the community.
+        
+        :param size: The number of requests to fetch. (Default: 25)
+        :type size: int, optional
+        :param status: The status of the requests to fetch. (Default: "pending")
+        :type status: str, optional
+        :param start: The index to start fetching requests from. (Default: 0)
+        :type start: int, optional
+        :param comId: The ID of the community to fetch requests from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `CommunityMembershipRequestList` object containing the membership requests for the community.
+        :rtype: CommunityMembershipRequestList
+        
+        This function sends a GET request to the API to fetch membership requests for the community.
+        
+        :returns: A `CommunityMembershipRequestList` object containing the membership requests for the community.
+        :rtype: CommunityMembershipRequestList
+        >>> userIds = client.community.fetch_membership_requests().applicant.userId
+        ... for userId in userIds:
+        ...     client.community.approve_membership_request(userId)
+        """
+        return CommunityMembershipRequestList(
+            await self.session.handler(
+                method = "GET",
+                url = f"http://service.aminoapps.com/api/v1/x{comId or self.community_id}/s/community/membership-request?size={size}&status={status}&start={start}"
+        ))
+
+
+    @community
+    async def approve_membership_request(self, requestId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Approves a membership request for the community.
+        
+        :param requestId: The ID of the request to approve.
+        :type requestId: str
+        :param comId: The ID of the community to approve the request in. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `ApiResponse` object containing the API response.
+        
+        This function sends a POST request to the API to approve a membership request for the community.
+        
+        :returns: A `ApiResponse` object containing the API response.
+        :rtype: ApiResponse
+        
+        `ApiResponse`:
+        
+        - `code` (int): The status code of the API response.
+        - `api:status` (int): The status of the API response.
+        - `api:statuscode` (int): The status code of the API response.
+        - `api:message` (str): The message of the API response.
+        
+        **Example usage:**
+        
+        >>> client.community.approve_membership_request("requestId")
+        """
+        return ApiResponse(
+            await self.session.handler(
+                method = "POST",
+                url = f"http://service.aminoapps.com/api/v1/x{comId or self.community_id}/s/community/membership-request/{requestId}/approve"
+        ))
+
+
+    @community
+    async def decline_membership_request(self, requestId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Declines a membership request for the community.
+        
+        :param requestId: The ID of the request to decline.
+        :type requestId: str
+        :param comId: The ID of the community to decline the request in. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `ApiResponse` object containing the API response.
+        
+        This function sends a POST request to the API to decline a membership request for the community.
+        
+        :returns: A `ApiResponse` object containing the API response.
+        :rtype: ApiResponse
+        
+        `ApiResponse`:
+            - `message` (str): The message of the API response.
+            - `status_code` (int): The status code of the API response.
+            - `duration` (float): The duration of the API response.
+            - `timestamp` (int): The timestamp of the API response.
+
+        **Example usage:**
+
+        >>> client.community.decline_membership_request("requestId")
+        ... client.community.decline_membership_request("requestId", comId="comId")
+        """
+        return ApiResponse(
+            await self.session.handler(
+                method = "POST",
+                url = f"http://service.aminoapps.com/api/v1/x{comId or self.community_id}/s/community/membership-request/{requestId}/reject"
+        ))
+
+
+    @community
+    async def fetch_community_stats(self, comId: Union[str, int] = None) -> CommunityStats:
+        """
+        Fetches community statistics.
+        
+        :param comId: The ID of the community to fetch statistics from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `CommunityStats` object containing the community statistics.
+        :rtype: CommunityStats
+        
+        This function sends a GET request to the API to fetch community statistics.
+        
+        :returns: A `CommunityStats` object containing the community statistics.
+        :rtype: CommunityStats
+
+        `CommunityStats`:
+            - daily_active_members: The daily active members of the community.
+            - monthly_active_members: The monthly active members of the community.
+            - total_time_spent: The total time spent in the community.
+            - total_posts_created: The total posts created in the community.
+            - new_members_today: The new members today in the community.
+            - total_members: The total members in the community.
+
+        Example usage:
+
+        >>> community = client.fetch_community_stats()
+        ... print(community.daily_active_members)
+        ... print(community.monthly_active_members)
+        ... print(community.total_time_spent)
+        ... print(community.total_posts_created)
+        ... print(community.new_members_today)
+        ... print(community.total_members)
+        """
+        return CommunityStats(
+            await self.session.handler(
+                method = "GET",
+                url = f"http://service.aminoapps.com/api/v1/x{comId or self.community_id}/s/community/stats"
         ))
```

### Comparing `pymino-1.1.9.6/pymino/ext/async_context.py` & `pymino-1.1.9.7/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/async_event_handler.py` & `pymino-1.1.9.7/pymino/ext/async_event_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         try:
             userId = context.author.userId
         except AttributeError:
             userId = None
 
         potential_parameters = {
             "ctx": context,
+            "member": Member(context.author.json()),
             "message": message,
             "username": username,
             "userId": userId
         }
 
         return [
             potential_parameters.get(parameter)
```

### Comparing `pymino-1.1.9.6/pymino/ext/async_socket.py` & `pymino-1.1.9.7/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/community.py` & `pymino-1.1.9.7/pymino/ext/community.py`

 * *Files 2% similar despite different names*

```diff
@@ -2317,26 +2317,14 @@
         return ApiResponse(self.session.handler(
             method = "DELETE",
             url = f"/x{self.community_id if comId is None else comId}/s/block/{userId}"
             ))
 
 
     @community
-    def post_blog(self, title: str, content: str, comId: Union[str, int] = None) -> CBlog: #TODO: ADD DOCSTRING
-        return CBlog(self.session.handler(
-            method = "POST",
-            url = f"/x{self.community_id if comId is None else comId}/s/blog",
-            data = {
-                "content": content,
-                "title": title,
-                "timestamp": int(time() * 1000)
-                }))
-
-
-    @community
     def delete_blog(self, blogId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
         Deletes the specified blog.
 
         :param blogId: The ID of the blog to delete.
         :type blogId: str
         :param comId: The ID of the community to delete the blog from. If not provided, the current community ID is used.
@@ -6262,8 +6250,313 @@
         - `chatRequestPrivilege` (bool): Whether or not chat request privilege is enabled.
 
         **Example usage:**
 
         >>> profile = client.community.chat_request_privilege(True)
         ... print(profile.chatRequestPrivilege)
         """
-        return self.edit_profile(chatRequestPrivilege=1 if privilege else 2, comId=comId)
+        return self.edit_profile(chatRequestPrivilege=1 if privilege else 2, comId=comId)
+
+
+    @community
+    def post_blog(self,
+                  title: str,
+                  content: str,
+                  imageList: list = None,
+                  captionList: list = None,
+                  categoriesList: list = None,
+                  backgroundColor: str = None,
+                  fansOnly: bool = False,
+                  extensions: dict = None,
+                  comId: Union[str, int] = None) -> CBlog:
+        """
+        Posts a blog in the community.
+
+        :param title: The title of the blog.
+        :type title: str
+        :param content: The content of the blog.
+        :type content: str
+        :param imageList: A list of image paths to include in the blog. (Optional)
+        :type imageList: list, optional
+        :param captionList: A list of captions corresponding to the images. (Optional)
+        :type captionList: list, optional
+        :param categoriesList: A list of category IDs to assign to the blog. (Optional)
+        :type categoriesList: list, optional
+        :param backgroundColor: The background color of the blog. (Optional)
+        :type backgroundColor: str, optional
+        :param fansOnly: Whether the blog is for fans only. (Default: False)
+        :type fansOnly: bool, optional
+        :param extensions: Additional extensions for the blog. (Optional)
+        :type extensions: dict, optional
+        :param comId: The ID of the community to post the blog in. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `CBlog` object representing the posted blog.
+        :rtype: CBlog
+
+        This function posts a blog in the specified community using the provided information.
+
+        `CBlog` represents a blog on the platform.
+
+        **Example usage:**
+
+        >>> blog = client.community.post_blog("My Blog", "This is the content of my blog.", imageList=["image1.jpg", "image2.jpg"])
+        ... print(blog.title)
+        ... print(blog.content)
+        """
+        media = []
+        if captionList is not None: media.append([100, self.__handle_media__(image, "image/jpg", True), None] for image in captionList)
+        elif imageList is not None: media.append([100, self.__handle_media__(image, "image/jpg", True), None] for image in imageList)
+
+        data = dict(address = None,
+                    content = content,
+                    title = title,
+                    mediaList = media,
+                    extensions = extensions,
+                    latitude = 0,
+                    longitude = 0,
+                    eventSource = "GlobalComposeMenu",
+                    timestamp = int(time() * 1000))
+        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+        if backgroundColor:
+            data["extensions"] = {
+                "style": {
+                    "backgroundColor": backgroundColor
+                    if backgroundColor.startswith("#")
+                    else f"#{backgroundColor}"
+                }
+            }
+        if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
+
+        return CBlog(self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/blog",
+            data = data
+        ))
+
+
+    @community
+    def fetch_invites(self, size: int = 25, status: str = "normal", start: int = 0, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Fetches generated invites for the community.
+
+        :param size: The number of invites to fetch. (Default: 25)
+        :type size: int, optional
+        :param status: The status of the invites to fetch. (Default: "normal")
+        :type status: str, optional
+        :param start: The index to start fetching invites from. (Default: 0)
+        :type start: int, optional
+
+        This function sends a GET request to the API to fetch generated invites for the community.
+
+        :returns: A `ApiResponse` object containing the API response.
+        :rtype: ApiResponse
+
+        `ApiResponse`:
+
+        - `code` (int): The status code of the API response.
+        - `api:status` (int): The status of the API response.
+        - `api:statuscode` (int): The status code of the API response.
+        - `api:message` (str): The message of the API response.
+        
+        **Example usage:**
+
+        >>> invites = client.community.fetch_invites()
+        ... print(invites.json()['communityInvitationList'])
+        ... for invite in invites.json()['communityInvitationList']:
+        ...     print(invite['invitationId'])
+        """
+        return ApiResponse(self.session.handler(
+            method = "GET",
+            url = f"http://service.aminoapps.com/api/v1/g/s-x{self.community_id or comId}/community/invitation?size={size}&status={status}&start={start}"
+        ))
+    
+
+    @community
+    def revoke_invite(self, invitationId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Revokes an invite for the community.
+        Used for revoking invites that have been generated.
+        
+        :param invitationId: The ID of the invite to revoke.
+        :type invitationId: str
+        :param comId: The ID of the community to revoke the invite in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `ApiResponse` object containing the API response.
+        :rtype: ApiResponse
+        
+        This function sends a DELETE request to the API to revoke an invite for the community.
+        
+        :returns: A `ApiResponse` object containing the API response.
+        :rtype: ApiResponse
+        
+        `ApiResponse`:
+        
+        - `code` (int): The status code of the API response.
+        - `api:status` (int): The status of the API response.
+        - `api:statuscode` (int): The status code of the API response.
+        - `api:message` (str): The message of the API response.
+        
+        **Example usage:**
+        
+        >>> client.community.revoke_invite("invitationId")
+        """
+        try:
+            return ApiResponse(
+                self.session.handler(
+                    method = "DELETE",
+                    url = f"http://service.aminoapps.com/api/v1/g/s-x{self.community_id or comId}/community/invitation/{invitationId}"
+            ))
+        except AccessDenied as e:
+            raise AccessDenied("You must be a leader to revoke invites.") from e
+
+
+    @community
+    def fetch_membership_requests(self, size: int = 25, status: str = "pending", start: int = 0, comId: Union[str, int] = None) -> CommunityMembershipRequestList:
+        """
+        Fetches membership requests for the community.
+        Used for approving or declining membership requests into the community.
+        
+        :param size: The number of requests to fetch. (Default: 25)
+        :type size: int, optional
+        :param status: The status of the requests to fetch. (Default: "pending")
+        :type status: str, optional
+        :param start: The index to start fetching requests from. (Default: 0)
+        :type start: int, optional
+        :param comId: The ID of the community to fetch requests from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `CommunityMembershipRequestList` object containing the membership requests for the community.
+        :rtype: CommunityMembershipRequestList
+        
+        This function sends a GET request to the API to fetch membership requests for the community.
+        
+        :returns: A `CommunityMembershipRequestList` object containing the membership requests for the community.
+        :rtype: CommunityMembershipRequestList
+        >>> userIds = client.community.fetch_membership_requests().applicant.userId
+        ... for userId in userIds:
+        ...     client.community.approve_membership_request(userId)
+        """
+        try:
+            return CommunityMembershipRequestList(
+                self.session.handler(
+                    method = "GET",
+                    url = f"http://service.aminoapps.com/api/v1/x{comId or self.community_id}/s/community/membership-request?size={size}&status={status}&start={start}"
+            ))
+        except AccessDenied as e:
+            raise AccessDenied("You must be a leader to fetch membership requests.") from e
+
+
+
+    @community
+    def approve_membership_request(self, requestId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Approves a membership request for the community.
+        
+        :param requestId: The ID of the request to approve.
+        :type requestId: str
+        :param comId: The ID of the community to approve the request in. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `ApiResponse` object containing the API response.
+        
+        This function sends a POST request to the API to approve a membership request for the community.
+        
+        :returns: A `ApiResponse` object containing the API response.
+        :rtype: ApiResponse
+        
+        `ApiResponse`:
+            - `message` (str): The message of the API response.
+            - `status_code` (int): The status code of the API response.
+            - `duration` (float): The duration of the API response.
+            - `timestamp` (int): The timestamp of the API response.
+        
+        **Example usage:**
+        
+        >>> client.community.approve_membership_request("requestId")
+        ... client.community.approve_membership_request("requestId", comId="comId")
+        """
+        try:
+            return ApiResponse(
+                self.session.handler(
+                    method = "POST",
+                    url = f"http://service.aminoapps.com/api/v1/x{comId or self.community_id}/s/community/membership-request/{requestId}/approve"
+            ))
+        except AccessDenied as e:
+            raise AccessDenied("You must be a leader to approve membership requests.") from e
+
+
+    @community
+    def decline_membership_request(self, requestId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Declines a membership request for the community.
+        
+        :param requestId: The ID of the request to decline.
+        :type requestId: str
+        :param comId: The ID of the community to decline the request in. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `ApiResponse` object containing the API response.
+        
+        This function sends a POST request to the API to decline a membership request for the community.
+        
+        :returns: A `ApiResponse` object containing the API response.
+        :rtype: ApiResponse
+        
+        `ApiResponse`:
+            - `message` (str): The message of the API response.
+            - `status_code` (int): The status code of the API response.
+            - `duration` (float): The duration of the API response.
+            - `timestamp` (int): The timestamp of the API response.
+
+        **Example usage:**
+
+        >>> client.community.decline_membership_request("requestId")
+        ... client.community.decline_membership_request("requestId", comId="comId")
+        """
+        try:
+            return ApiResponse(
+                self.session.handler(
+                    method = "POST",
+                    url = f"http://service.aminoapps.com/api/v1/x{comId or self.community_id}/s/community/membership-request/{requestId}/reject"
+            ))
+        except AccessDenied as e:
+            raise AccessDenied("You must be a leader to decline membership requests.") from e
+
+
+    @community
+    def fetch_community_stats(self, comId: Union[str, int] = None) -> CommunityStats:
+        """
+        Fetches community statistics.
+        
+        :param comId: The ID of the community to fetch statistics from. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: A `CommunityStats` object containing the community statistics.
+        :rtype: CommunityStats
+        
+        This function sends a GET request to the API to fetch community statistics.
+        
+        :returns: A `CommunityStats` object containing the community statistics.
+        :rtype: CommunityStats
+
+        `CommunityStats`:
+            - daily_active_members: The daily active members of the community.
+            - monthly_active_members: The monthly active members of the community.
+            - total_time_spent: The total time spent in the community.
+            - total_posts_created: The total posts created in the community.
+            - new_members_today: The new members today in the community.
+            - total_members: The total members in the community.
+
+        Example usage:
+
+        >>> community = client.fetch_community_stats()
+        ... print(community.daily_active_members)
+        ... print(community.monthly_active_members)
+        ... print(community.total_time_spent)
+        ... print(community.total_posts_created)
+        ... print(community.new_members_today)
+        ... print(community.total_members)
+        """
+        try:
+            return CommunityStats(
+                self.session.handler(
+                    method = "GET",
+                    url = f"http://service.aminoapps.com/api/v1/x{comId or self.community_id}/s/community/stats"
+            ))
+        except AccessDenied as e:
+            raise AccessDenied("You must be a leader to fetch community statistics.") from e
```

### Comparing `pymino-1.1.9.6/pymino/ext/console.py` & `pymino-1.1.9.7/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/context.py` & `pymino-1.1.9.7/pymino/ext/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         self.message:   Message = message
         self.userId:    str = session.userId
         self.request    = session
 
     @property
     def author(self) -> MessageAuthor:
         """The author of the message."""
-        with suppress(AttributeError): return self.message.author
+        with suppress(AttributeError):
+            return self.message.author
 
     @property
     def communityId(self) -> str:
         """Sets the url to community/global."""
         return {True: "g", False: f"x{self.message.comId}"}[self.message.comId == 0]
 
     @property
@@ -601,14 +602,15 @@
         try:
             userId = context.author.userId
         except AttributeError:
             userId = None
 
         potential_parameters = {
             "ctx": context,
+            "member": Member(context.author.json()),
             "message": message,
             "username": username,
             "userId": userId
         }
 
         return [
             potential_parameters.get(parameter)
@@ -637,14 +639,15 @@
         - `command_name` - The name of the command.
         - `command_description` - The description of the command.
         - `aliases` - The other names the command can be called by.
         - `cooldown` - The cooldown of the command in seconds.
 
         `**Function Parameters**``
         - `ctx` - The context of the command.
+        - `member` - The Member(member) who called the command.
         - `message` - The message that called the command.
         - `username` - The username of the person who called the command.
         - `userId` - The userId of the person who called the command.
 
         Do I need a `command_description`?
             - No, you don't need a command description however it is recommended.
             - If you don't supply a command description the command will not show up in the help command.
@@ -751,15 +754,15 @@
             return None
 
         message = data.content[len(self.command_prefix) + len(command_name) + 1:]
         command_name = dict(self._commands.__command_aliases__().copy()).get(command_name, command_name)
 
         response = self._check_cooldown(command_name, data, context)
 
-        if response  != 403:
+        if response != 403:
             func = self._commands.fetch_command(command_name).func
             return func(*self._set_parameters(context=context, func=func, message=message))
 
         return None
 
         
     def _check_cooldown(self, command_name: str, data: Message, context: Context) -> None:
```

### Comparing `pymino-1.1.9.6/pymino/ext/dispatcher.py` & `pymino-1.1.9.7/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/entities/api_response.py` & `pymino-1.1.9.7/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/entities/chat_threads.py` & `pymino-1.1.9.7/pymino/ext/entities/chat_threads.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,15 @@
     def threadId(self) -> str:
         """Returns the thread id"""
         return self.data.get("threadId")
     
     @property
     def chatId(self) -> str:
         """Returns the thread id"""
-        return self.thread_id
+        return self.threadId
     
     @property
     def keywords(self) -> List[str]:
         """Returns a list of keywords"""
         return self.data.get("keywords")
     
     @property
```

### Comparing `pymino-1.1.9.6/pymino/ext/entities/comments.py` & `pymino-1.1.9.7/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/entities/enums.py` & `pymino-1.1.9.7/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/entities/exceptions.py` & `pymino-1.1.9.7/pymino/ext/entities/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from contextlib import suppress
-
 class UnsupportedService(Exception):
     def __init__(self, response: str):
         super().__init__(response)
 
 class FileTooLarge(Exception):
     def __init__(self, response: str):
         super().__init__(response)
@@ -286,15 +284,15 @@
 
 class PostedTooRecently(Exception):
     def __init__(self, response: str):
         super().__init__(response)
 
 class APIException(Exception):
     def __init__(self, response: dict):
-        self.exception_map = {
+        exception_map = {
             100: UnsupportedService,
             101: InternalServerError,
             102: FileTooLarge,
             103: InvalidRequest,
             104: InvalidRequest,
             105: InvalidSession,
             106: AccessDenied,
@@ -361,34 +359,30 @@
             4300: NotEnoughCoins,
             4400: AlreadyPlayedLottery,
             4500: CannotSendCoins,
             6001: AminoIDAlreadyChanged,
             6002: InvalidAminoID,
             99001: InvalidName
         }
-    
-        self.url = None
-        self.message = None
-        self.status_code = None
-
-        with suppress(Exception):
-            self.status_code: int = response.get("api:statuscode", response)
-            self.message: str = response.get("api:message", response)
-            self.url: str = response.get("url")
-        
-            if not any([not isinstance(self.status_code, int), self.status_code not in self.exception_map]):
-                exception = self.exception_map.get(self.status_code)
 
-                if self.url is not None:
-                    self.message = f"{self.message} ({self.url})"
+        status_code = response.get("api:statuscode")
+        message = response.get("api:message")
+        url = response.get("url")
+
+        if status_code in exception_map:
+            exception = exception_map.get(status_code)
+
+            if url is not None:
+                message = f"{message} ({url})"
+
+            if exception:
+                raise exception(message)
 
-                if exception is not None:
-                    raise exception(self.message)
-            
         raise API_ERROR(response)
+
             
 class MissingCommunityId(Exception):
     def __init__(self):
         super().__init__(
             "Please provide a community id to the bot before running it or add it to the function call."
             )
```

### Comparing `pymino-1.1.9.6/pymino/ext/entities/general.py` & `pymino-1.1.9.7/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/entities/handlers.py` & `pymino-1.1.9.7/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/entities/link_info.py` & `pymino-1.1.9.7/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/entities/messages.py` & `pymino-1.1.9.7/pymino/ext/entities/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
             }
         [self.base_message.update({key: kwargs[key]}) for key in kwargs]
 
     def json(self):
         """`JSON` - returns the raw data."""
         return self.base_message
 
+
 class MessageAuthor:
     def __init__(self, data: Union[dict, str]) -> None:
         self.data = data
 
     @property
     def uid(self) -> Union[str, None]:
         """
@@ -143,14 +144,15 @@
         """
         return self.data.get("avatarFrame")
         
     def json(self) -> Union[dict, str]:
         """`JSON` - returns the raw data."""
         return self.data
 
+
 class CMessage:
     def __init__(self, data: Union[dict, str]) -> None:
         self.data: dict = data.get('result') or data.get('message', data)
 
     def return_none(func):
         def wrapper(*args, **kwargs):
             return None if args[0].data is None else func(*args, **kwargs)
```

### Comparing `pymino-1.1.9.6/pymino/ext/entities/notification.py` & `pymino-1.1.9.7/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/entities/userprofile.py` & `pymino-1.1.9.7/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/entities/wsevents.py` & `pymino-1.1.9.7/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/handle_queue.py` & `pymino-1.1.9.7/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/socket.py` & `pymino-1.1.9.7/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/utilities/async_request_handler.py` & `pymino-1.1.9.7/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/utilities/chat_console.py` & `pymino-1.1.9.7/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/utilities/commands.py` & `pymino-1.1.9.7/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/utilities/community_console.py` & `pymino-1.1.9.7/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/utilities/generate.py` & `pymino-1.1.9.7/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/utilities/menu.py` & `pymino-1.1.9.7/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/utilities/profile_console.py` & `pymino-1.1.9.7/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino/ext/utilities/request_handler.py` & `pymino-1.1.9.7/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.6/pymino.egg-info/PKG-INFO` & `pymino-1.1.9.7/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.9.6
+Version: 1.1.9.7
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.9.6 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.9.7 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.9.6/pymino.egg-info/SOURCES.txt` & `pymino-1.1.9.7/pymino.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 pymino/ext/community.py
 pymino/ext/console.py
 pymino/ext/context.py
 pymino/ext/dispatcher.py
 pymino/ext/handle_queue.py
 pymino/ext/socket.py
 pymino/ext/entities/__init__.py
+pymino/ext/entities/acm.py
 pymino/ext/entities/api_response.py
 pymino/ext/entities/chat_threads.py
 pymino/ext/entities/comments.py
 pymino/ext/entities/enums.py
 pymino/ext/entities/exceptions.py
 pymino/ext/entities/general.py
 pymino/ext/entities/handlers.py
 pymino/ext/entities/link_info.py
+pymino/ext/entities/member.py
 pymino/ext/entities/messages.py
 pymino/ext/entities/notification.py
 pymino/ext/entities/userprofile.py
 pymino/ext/entities/wsevents.py
 pymino/ext/utilities/__init__.py
 pymino/ext/utilities/async_request_handler.py
 pymino/ext/utilities/chat_console.py
```

### Comparing `pymino-1.1.9.6/setup.cfg` & `pymino-1.1.9.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e39 2e36 0d0a 6175  on = 1.1.9.6..au
+00000020: 6f6e 203d 2031 2e31 2e39 2e37 0d0a 6175  on = 1.1.9.7..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.9.6/setup.py` & `pymino-1.1.9.7/setup.py`

 * *Files identical despite different names*

