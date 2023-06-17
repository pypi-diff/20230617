# Comparing `tmp/pymino-1.1.9.8.tar.gz` & `tmp/pymino-1.1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\df\dist\.tmp-h_a8124z\pymino-1.1.9.8.tar", last modified: Sat Jun 17 03:41:38 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\subb\pymino\dist\.tmp-vtx59tf_\pymino-1.1.9.9.tar", last modified: Sat Jun 17 16:18:12 2023, max compression
```

## Comparing `pymino-1.1.9.8.tar` & `pymino-1.1.9.9.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 03:41:38.071186 pymino-1.1.9.8/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.9.8/LICENSE
--rw-rw-rw-   0        0        0     7298 2023-06-17 03:41:38.071186 pymino-1.1.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     6580 2023-06-17 03:41:22.000000 pymino-1.1.9.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 03:41:38.008195 pymino-1.1.9.8/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-17 03:36:14.000000 pymino-1.1.9.8/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.9.8/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30208 2023-06-15 01:47:51.000000 pymino-1.1.9.8/pymino/bot.py
--rw-rw-rw-   0        0        0    52363 2023-06-16 20:35:00.000000 pymino-1.1.9.8/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-17 03:41:38.036963 pymino-1.1.9.8/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-11 16:50:39.000000 pymino-1.1.9.8/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.9.8/pymino/ext/account.py
--rw-rw-rw-   0        0        0   306772 2023-06-16 23:13:50.000000 pymino-1.1.9.8/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.9.8/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    24095 2023-06-16 22:46:59.000000 pymino-1.1.9.8/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.9.8/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   305392 2023-06-16 23:13:10.000000 pymino-1.1.9.8/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-11 22:20:09.000000 pymino-1.1.9.8/pymino/ext/console.py
--rw-rw-rw-   0        0        0    42101 2023-06-17 03:36:25.000000 pymino-1.1.9.8/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.9.8/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-17 03:41:38.059779 pymino-1.1.9.8/pymino/ext/entities/
--rw-rw-rw-   0        0        0      355 2023-06-16 21:57:42.000000 pymino-1.1.9.8/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-06-16 23:16:13.000000 pymino-1.1.9.8/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     1670 2023-06-16 23:16:17.000000 pymino-1.1.9.8/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    20322 2023-06-16 23:16:20.000000 pymino-1.1.9.8/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.9.8/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.9.8/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15638 2023-06-16 21:42:30.000000 pymino-1.1.9.8/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.9.8/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-11 21:21:53.000000 pymino-1.1.9.8/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.9.8/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-06-16 21:57:33.000000 pymino-1.1.9.8/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-06-16 21:59:23.000000 pymino-1.1.9.8/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.9.8/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.9.8/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.9.8/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.9.8/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.9.8/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-17 03:41:38.070195 pymino-1.1.9.8/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-11 17:31:29.000000 pymino-1.1.9.8/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.9.8/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-13 04:27:21.000000 pymino-1.1.9.8/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.9.8/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-11 22:22:27.000000 pymino-1.1.9.8/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.9.8/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-11 21:47:35.000000 pymino-1.1.9.8/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-13 03:31:19.000000 pymino-1.1.9.8/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.9.8/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-17 03:41:38.021091 pymino-1.1.9.8/pymino.egg-info/
--rw-rw-rw-   0        0        0     7298 2023-06-17 03:41:37.000000 pymino-1.1.9.8/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1380 2023-06-17 03:41:37.000000 pymino-1.1.9.8/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 03:41:37.000000 pymino-1.1.9.8/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-17 03:41:37.000000 pymino-1.1.9.8/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-17 03:41:37.000000 pymino-1.1.9.8/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-17 03:41:38.072675 pymino-1.1.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:18:12.714582 pymino-1.1.9.9/
+-rw-rw-rw-   0        0        0     1085 2023-06-17 16:15:11.000000 pymino-1.1.9.9/LICENSE
+-rw-rw-rw-   0        0        0     7298 2023-06-17 16:18:12.715079 pymino-1.1.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6580 2023-06-17 16:17:57.000000 pymino-1.1.9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 16:18:12.642246 pymino-1.1.9.9/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-17 16:16:10.000000 pymino-1.1.9.9/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30208 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/bot.py
+-rw-rw-rw-   0        0        0    65900 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:18:12.680357 pymino-1.1.9.9/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    13871 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   306780 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    24095 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   305400 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    42101 2023-06-17 16:16:22.000000 pymino-1.1.9.9/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:18:12.702678 pymino-1.1.9.9/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      355 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     1670 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    20322 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15638 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0     6185 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:18:12.713615 pymino-1.1.9.9/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6396 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10274 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:18:12.661589 pymino-1.1.9.9/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7298 2023-06-17 16:18:12.000000 pymino-1.1.9.9/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1433 2023-06-17 16:18:12.000000 pymino-1.1.9.9/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 16:18:12.000000 pymino-1.1.9.9/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-17 16:18:12.000000 pymino-1.1.9.9/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-17 16:18:12.000000 pymino-1.1.9.9/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-17 16:18:12.717062 pymino-1.1.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-06-17 16:15:11.000000 pymino-1.1.9.9/setup.py
```

### Comparing `pymino-1.1.9.8/LICENSE` & `pymino-1.1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/PKG-INFO` & `pymino-1.1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.9.8
+Version: 1.1.9.9
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
-Metadata-Version: 2.1 Name: pymino Version: 1.1.9.8 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.9.9 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.9.8/README.md` & `pymino-1.1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/__init__.py` & `pymino-1.1.9.9/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.9.8'
+__version__ = '1.1.9.9'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.1.9.8/pymino/async_bot.py` & `pymino-1.1.9.9/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/bot.py` & `pymino-1.1.9.9/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/client.py` & `pymino-1.1.9.9/pymino/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1257,12 +1257,297 @@
         else: data["type"] = 0
 
         if publishToGlobal: data["publishToGlobal"] = 1
 
         return ChatThread(
             self.request.handler(method="POST", url="/g/s/chat/thread", data=data)
         )
+    
+    @authenticated
+    def blocker_users(self, start: int = 0, size: int = 25):
+        """
+        Retrieves a list of users what are blocking the logged account.
+        :param start: The index to start retrieving the list from (optional, default: 0).
+        :type start: int, optional
+        :param size: The number of users to retrieve (optional, default: 25).
+        :type size: int, optional
+        :return: A list of user IDs representing the blocker users.
+        :rtype: list
+        """
+        return self.request.handler(
+            method = "GET",
+            url = f"/g/s/block/full-list?start={start}&size={size}"
+        )["blockerUidList"]
 
+    def fetch_wall_comments(self, userId: str, sorting: str = "newest", start: int = 0, size: int = 25) -> CommentList:
+        """
+        Fetches wall comments for a user.
 
+        :param userId: The ID of the user whose wall comments will be fetched.
+        :type userId: str
+        :param sorting: The sorting method for the comments. Options: "newest" (default), "oldest", "top".
+        :type sorting: str, optional
+        :param start: The starting index of the comments to fetch (pagination). Default is 0.
+        :type start: int, optional
+        :param size: The number of comments to fetch (pagination). Default is 25.
+        :type size: int, optional
+        :return: The list of wall comments for the specified user.
+        :rtype: CommentList
+        :raises ValueError: If an incorrect sorting method is provided.
 
+        This method retrieves wall comments for a specific user. The comments can be sorted by "newest" (default), "oldest", or "top".
+        The `start` parameter specifies the index of the first comment to fetch, while the `size` parameter determines the number of
+        comments to retrieve. The comments are returned as a `CommentList` object.
 
+        **Example usage:**
 
+        To fetch the newest 25 wall comments for a user:
+
+        >>> comments = client.fetch_wall_comments(userId="00000000-0000-0000-0000-000000000000")
+        >>> for comment in comments:
+        ...     print(comment.content)
+        """
+        if sorting.lower() == "newest": sorting = "newest"
+        elif sorting.lower() == "oldest": sorting = "oldest"
+        elif sorting.lower() == "top": sorting = "vote"
+        else: raise ValueError("Incorrect sorting method.")
+
+        return CommentList(self.request.handler(
+            method = "GET",
+            url = f"/g/s/user-profile/{userId}/g-comment?sort={sorting}&start={start}&size={size}"
+        ))
+    
+    @authenticated
+    def delete_message(self, chatId: str, messageId: str):
+        """
+        Deletes a message in a chat thread.
+
+        :param chatId: The ID of the chat thread where the message is located.
+        :type chatId: str
+        :param messageId: The ID of the message to delete.
+        :type messageId: str
+        :return: The API response indicating the success or failure of the deletion.
+        :rtype: ApiResponse
+
+        This method allows the authenticated user to delete a specific message in a chat thread. The `chatId` parameter identifies the
+        chat thread, while the `messageId` parameter specifies the ID of the message to be deleted.
+
+        **Note:** Only authorized users can delete messages in a chat thread. If the deletion is successful, the API response will indicate
+        a successful deletion. Otherwise, an error message will be returned.
+
+        **Example usage:**
+
+        To delete a message with the ID "00000000-0000-0000-0000-000000000000" in a chat thread with the ID "00000000-0000-0000-0000-000000000000":
+
+        >>> response = client.delete_message(chatId="00000000-0000-0000-0000-000000000000", messageId="00000000-0000-0000-0000-000000000000")
+        >>> if response.success:
+        ...     print("Message deleted successfully!")
+        ... else:
+        ...     print("Failed to delete message.")
+        """
+        return ApiResponse(self.request.handler(
+            method = "DELETE",
+            url = f"/g/s/chat/thread/{chatId}/message/{messageId}"
+        ))
+    
+    @authenticated
+    def edit_chat(self,
+                  chatId: str,
+                  doNotDisturb: bool = None,
+                  pinChat: bool = None,
+                  title: str = None,
+                  icon: str = None,
+                  backgroundImage: str = None,
+                  content: str = None,
+                  announcement: str = None,
+                  coHosts: list = None,
+                  keywords: list = None,
+                  pinAnnouncement: bool = None,
+                  publishToGlobal: bool = None,
+                  canTip: bool = None,
+                  viewOnly: bool = None,
+                  canInvite: bool = None,
+                  fansOnly: bool = None) -> list:
+        """
+        Edits the settings of a chat.
+
+        :param chatId: The ID of the chat to be edited.
+        :type chatId: str
+        :param doNotDisturb: Set to True to enable "Do Not Disturb" mode for the chat, False to disable it. Default is None.
+        :type doNotDisturb: bool, optional
+        :param pinChat: Set to True to pin the chat, False to unpin it. Default is None.
+        :type pinChat: bool, optional
+        :param title: The new title for the chat.
+        :type title: str, optional
+        :param icon: The new icon image file for the chat.
+        :type icon: str, optional
+        :param backgroundImage: The new background image file for the chat.
+        :type backgroundImage: str, optional
+        :param content: The new content for the chat.
+        :type content: str, optional
+        :param announcement: The new announcement for the chat.
+        :type announcement: str, optional
+        :param coHosts: A list of user IDs to set as co-hosts for the chat.
+        :type coHosts: list, optional
+        :param keywords: A list of keywords to associate with the chat.
+        :type keywords: list, optional
+        :param pinAnnouncement: Set to True to pin the announcement, False to unpin it. Default is None.
+        :type pinAnnouncement: bool, optional
+        :param publishToGlobal: Set to True to publish the chat to the global feed, False to unpublish it. Default is None.
+        :type publishToGlobal: bool, optional
+        :param canTip: Set to True to enable tipping permissions for the chat, False to disable it. Default is None.
+        :type canTip: bool, optional
+        :param viewOnly: Set to True to enable view-only mode for the chat, False to disable it. Default is None.
+        :type viewOnly: bool, optional
+        :param canInvite: Set to True to allow members to invite others to the chat, False to disable it. Default is None.
+        :type canInvite: bool, optional
+        :param fansOnly: Set to True to enable "Fans Only" mode for the chat, False to disable it. Default is None.
+        :type fansOnly: bool, optional
+        :return: A list of HTTP status codes for each operation performed during the chat edit.
+        :rtype: list
+
+        This method allows the authenticated user to edit various settings of a chat, such as "Do Not Disturb" mode, pinning,
+        title, icon, background image, content, announcement, co-hosts, keywords, pinning the announcement, publishing to the
+        global feed, tipping permissions, view-only mode, allowing members to invite others, and "Fans Only" mode. Only the
+        specified parameters will be updated.
+
+        The function returns a list of HTTP status codes for each operation performed during the chat edit.
+
+        **Example usage:**
+
+        To edit the title and pin the chat:
+
+        >>> response_codes = client.edit_chat(chatId="chat123", title="New Chat Title", pinChat=True)
+        >>> if all(code == 200 for code in response_codes):
+        ...     print("Chat edited successfully!")
+        ... else:
+        ...     print("Failed to edit chat.")
+        """
+        data = {"timestamp": int(time() * 1000)}
+
+        if title: data["title"] = title
+        if content: data["content"] = content
+        if icon: data["icon"] = self.upload_image(icon)
+        if keywords: data["keywords"] = keywords
+        if announcement: data["extensions"] = {"announcement": announcement}
+        if pinAnnouncement: data["extensions"] = {"pinAnnouncement": pinAnnouncement}
+        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+        if publishToGlobal: data["publishToGlobal"] = 0
+        if not publishToGlobal: data["publishToGlobal"] = 1
+
+        responses = []
+
+        if doNotDisturb is not None:
+            responses.append(ApiResponse(self.request.handler(
+                method = "POST",
+                url = f"/g/s/chat/thread/{chatId}/member/{self.userId}/alert",
+                data = {
+                    "alertOption": 2 if doNotDisturb else 1,
+                    "timestamp": int(time() * 1000)
+                }
+            )).status_code)
+        
+        if pinChat is not None:
+            responses.append(ApiResponse(self.request.handler(
+                method = "POST",
+                url = f"/g/s/chat/thread/{chatId}/{'pin' if pinChat else 'unpin'}"
+            )).status_code)
+        
+        if backgroundImage is not None:
+            responses.append(ApiResponse(self.request.handler(
+                method = "POST",
+                url = f"/g/s/chat/thread/{chatId}/member/{self.userId}/background",
+                data = {
+                    "media": [100, self.upload_image(backgroundImage), None],
+                    "timestamp": int(time() * 1000)
+                }
+            )).status_code)
+        
+        if coHosts is not None:
+            responses.append(ApiResponse(self.request.handler(
+                method = "POST",
+                url = f"/g/s/chat/thread/{chatId}/co-host",
+                data = {
+                    "uidList": coHosts,
+                    "timestamp": int(time() * 1000)
+                }
+            )).status_code)
+        
+        if viewOnly is not None:
+            responses.append(ApiResponse(self.request.handler(
+                method = "POST",
+                url = f"/g/s/chat/thread/{chatId}/view-only/{'enable' if viewOnly else 'disable'}"
+            )).status_code)
+        
+        if canInvite is not None:
+            responses.append(ApiResponse(self.request.handler(
+                method = "POST",
+                url = f"/g/s/chat/thread/{chatId}/members-can-invite/{'enable' if canInvite else 'disable'}"
+            )).status_code)
+        
+        if canTip is not None:
+            responses.append(ApiResponse(
+                method = "POST",
+                url = f"/g/s/chat/thread/{chatId}/tipping-perm-status/{'enable' if canTip else 'disable'}"
+            ).status_code)
+        
+        responses.append(ApiResponse(self.request.handler(
+            method = "POST",
+            url = f"/g/s/chat/thread/{chatId}",
+            data = data
+        )).status_code)
+
+        return responses
+    
+    @authenticated
+    def follow(self, userId: Union[str, list]):
+        """
+        Follows a user or a list of users.
+
+        :param userId: The ID of the user or a list of user IDs to follow.
+        :type userId: Union[str, list]
+        :return: The status code of the API response.
+        :rtype: int
+
+        This method allows the authenticated user to follow another user or a list of users. The `userId` parameter can be a single
+        user ID (string) or a list of user IDs. If a single user ID is provided, the method will follow that user. If a list of user IDs
+        is provided, the method will follow all the users in the list.
+
+        If a single user ID is provided, the function will make a POST request to "/g/s/user-profile/{userId}/member" to follow the user.
+        If a list of user IDs is provided, the function will make a POST request to "/g/s/user-profile/{self.userId}/joined" with the
+        `targetUidList` parameter set to the list of user IDs and the `timestamp` parameter set to the current timestamp.
+
+        The function returns the status code of the API response.
+
+        **Example usage:**
+
+        To follow a single user:
+
+        >>> response_code = client.follow(userId="user123")
+        >>> if response_code == 200:
+        ...     print("User followed successfully!")
+        ... else:
+        ...     print("Failed to follow user.")
+
+        To follow multiple users:
+
+        >>> user_ids = ["user123", "user456", "user789"]
+        >>> response_code = client.follow(userId=user_ids)
+        >>> if response_code == 200:
+        ...     print("Users followed successfully!")
+        ... else:
+        ...     print("Failed to follow users.")
+        """
+        if isinstance(userId, str):
+            return ApiResponse(self.request.handler(
+                method = "POST",
+                url = f"/g/s/user-profile/{userId}/member"
+            )).status_code
+        if isinstance(userId, list):
+            return ApiResponse(self.request.handler(
+                method = "POST",
+                url = f"/g/s/user-profile/{self.userId}/joined",
+                data = {
+                    "targetUidList": userId,
+                    "timestamp": int(time() * 1000)
+                }
+            )).status_code
```

### Comparing `pymino-1.1.9.8/pymino/ext/account.py` & `pymino-1.1.9.9/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/async_community.py` & `pymino-1.1.9.9/pymino/ext/async_community.py`

 * *Files 0% similar despite different names*

```diff
@@ -5982,67 +5982,67 @@
             responses.append(ApiResponse(await self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{self.userId}/alert",
                 data = {
                     "alertOption": 2 if doNotDisturb else 1,
                     "timestamp": int(time() * 1000)
                 }
-            )).statuscode)
+            )).status_code)
             
         
         if pinChat is not None:
             responses.append(ApiResponse(await self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/{'pin' if pinChat else 'unpin'}",
                 data = data
-            )).statuscode)
+            )).status_code)
         
         if backgroundImage is not None:
             responses.append(ApiResponse(await self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{self.userId}/background",
                 data = {
                     "media": [100, await self.__handle_media__(backgroundImage, "image/jpg", media_value=True), None],
                     "timestamp": int(time() * 1000)
                 }
-            )).statuscode)
+            )).status_code)
         
         if coHost is not None:
             responses.append(ApiResponse(await self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/co-host",
                 data = {
                     "uidList": coHost,
                     "timestamp": int(time() * 1000)
                 }
-            )).statuscode)
+            )).status_code)
         
         if viewOnly is not None:
             responses.append(ApiResponse(await self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}/view-only/{'enable' if viewOnly else 'disable'}"
-            )).statuscode)
+            )).status_code)
         
         if canInvite is not None:
             responses.append(ApiResponse(await self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}/members-can-invite/{'enable' if canInvite else 'disable'}"
-            )).statuscode)
+            )).status_code)
         
         if canTip is not None:
             responses.append(ApiResponse(await self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}/tipping-perm-status/{'enable' if canTip else 'disable'}"
-            )).statuscode)
+            )).status_code)
         
         responses.append(ApiResponse(await self.session.handler(
             method = "POST",
             url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}",
             data = data
-        )).statuscode)
+        )).status_code)
 
         return responses
 
     @community
     async def edit_profile(self, nickname: str = None, content: str = None, icon: str = None, chatRequestPrivilege: str = None, imageList: list = None, captionList: list = None, backgroundImage: str = None, backgroundColor: str = None, titles: list = None, colors: list = None, defaultBubbleId: str = None, comId: Union[str, int] = None):
         """
         Edits the user profile.
```

### Comparing `pymino-1.1.9.8/pymino/ext/async_context.py` & `pymino-1.1.9.9/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/async_event_handler.py` & `pymino-1.1.9.9/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/async_socket.py` & `pymino-1.1.9.9/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/community.py` & `pymino-1.1.9.9/pymino/ext/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -5882,67 +5882,67 @@
             responses.append(ApiResponse(self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{self.userId}/alert",
                 data = {
                     "alertOption": 2 if doNotDisturb else 1,
                     "timestamp": int(time() * 1000)
                 }
-            )).statuscode)
+            )).status_code)
             
         
         if pinChat is not None:
             responses.append(ApiResponse(self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/{'pin' if pinChat else 'unpin'}",
                 data = data
-            )).statuscode)
+            )).status_code)
         
         if backgroundImage is not None:
             responses.append(ApiResponse(self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{self.userId}/background",
                 data = {
                     "media": [100, self.__handle_media__(backgroundImage, "image/jpg", True), None],
                     "timestamp": int(time() * 1000)
                 }
-            )).statuscode)
+            )).status_code)
         
         if coHost is not None:
             responses.append(ApiResponse(self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/co-host",
                 data = {
                     "uidList": coHost,
                     "timestamp": int(time() * 1000)
                 }
-            )).statuscode)
+            )).status_code)
         
         if viewOnly is not None:
             responses.append(ApiResponse(self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}/view-only/{'enable' if viewOnly else 'disable'}"
-            )).statuscode)
+            )).status_code)
         
         if canInvite is not None:
             responses.append(ApiResponse(self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}/members-can-invite/{'enable' if canInvite else 'disable'}"
-            )).statuscode)
+            )).status_code)
         
         if canTip is not None:
             responses.append(ApiResponse(self.session.handler(
                 method = "POST",
                 url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}/tipping-perm-status/{'enable' if canTip else 'disable'}"
-            )).statuscode)
+            )).status_code)
         
         responses.append(ApiResponse(self.session.handler(
             method = "POST",
             url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}",
             data = data
-        )).statuscode)
+        )).status_code)
 
         return responses
 
     @community
     def edit_profile(self, nickname: str = None, content: str = None, icon: str = None, chatRequestPrivilege: str = None, imageList: list = None, captionList: list = None, backgroundImage: str = None, backgroundColor: str = None, titles: list = None, colors: list = None, defaultBubbleId: str = None, comId: Union[str, int] = None):
         """
         Edits the user profile.
```

### Comparing `pymino-1.1.9.8/pymino/ext/console.py` & `pymino-1.1.9.9/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/context.py` & `pymino-1.1.9.9/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/dispatcher.py` & `pymino-1.1.9.9/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/acm.py` & `pymino-1.1.9.9/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/api_response.py` & `pymino-1.1.9.9/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/chat_threads.py` & `pymino-1.1.9.9/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/comments.py` & `pymino-1.1.9.9/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/enums.py` & `pymino-1.1.9.9/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/exceptions.py` & `pymino-1.1.9.9/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/general.py` & `pymino-1.1.9.9/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/handlers.py` & `pymino-1.1.9.9/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/link_info.py` & `pymino-1.1.9.9/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/member.py` & `pymino-1.1.9.9/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/messages.py` & `pymino-1.1.9.9/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/notification.py` & `pymino-1.1.9.9/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/userprofile.py` & `pymino-1.1.9.9/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/entities/wsevents.py` & `pymino-1.1.9.9/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/handle_queue.py` & `pymino-1.1.9.9/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/socket.py` & `pymino-1.1.9.9/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/utilities/async_request_handler.py` & `pymino-1.1.9.9/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/utilities/chat_console.py` & `pymino-1.1.9.9/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/utilities/commands.py` & `pymino-1.1.9.9/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/utilities/community_console.py` & `pymino-1.1.9.9/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/utilities/generate.py` & `pymino-1.1.9.9/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/utilities/menu.py` & `pymino-1.1.9.9/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/utilities/profile_console.py` & `pymino-1.1.9.9/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino/ext/utilities/request_handler.py` & `pymino-1.1.9.9/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.8/pymino.egg-info/PKG-INFO` & `pymino-1.1.9.9/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.9.8
+Version: 1.1.9.9
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
-Metadata-Version: 2.1 Name: pymino Version: 1.1.9.8 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.9.9 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.9.8/pymino.egg-info/SOURCES.txt` & `pymino-1.1.9.9/pymino.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 pymino/client.py
 pymino.egg-info/PKG-INFO
 pymino.egg-info/SOURCES.txt
 pymino.egg-info/dependency_links.txt
 pymino.egg-info/requires.txt
 pymino.egg-info/top_level.txt
 pymino/ext/__init__.py
+pymino/ext/_global.py
 pymino/ext/account.py
 pymino/ext/async_community.py
 pymino/ext/async_context.py
 pymino/ext/async_event_handler.py
 pymino/ext/async_socket.py
 pymino/ext/community.py
 pymino/ext/console.py
@@ -32,14 +33,15 @@
 pymino/ext/entities/exceptions.py
 pymino/ext/entities/general.py
 pymino/ext/entities/handlers.py
 pymino/ext/entities/link_info.py
 pymino/ext/entities/member.py
 pymino/ext/entities/messages.py
 pymino/ext/entities/notification.py
+pymino/ext/entities/threads.py
 pymino/ext/entities/userprofile.py
 pymino/ext/entities/wsevents.py
 pymino/ext/utilities/__init__.py
 pymino/ext/utilities/async_request_handler.py
 pymino/ext/utilities/chat_console.py
 pymino/ext/utilities/commands.py
 pymino/ext/utilities/community_console.py
```

### Comparing `pymino-1.1.9.8/setup.cfg` & `pymino-1.1.9.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e39 2e38 0d0a 6175  on = 1.1.9.8..au
+00000020: 6f6e 203d 2031 2e31 2e39 2e39 0d0a 6175  on = 1.1.9.9..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.9.8/setup.py` & `pymino-1.1.9.9/setup.py`

 * *Files identical despite different names*

