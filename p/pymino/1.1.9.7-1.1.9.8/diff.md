# Comparing `tmp/pymino-1.1.9.7.tar.gz` & `tmp/pymino-1.1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.9.6\dist\.tmp-lsxu854_\pymino-1.1.9.7.tar", last modified: Fri Jun 16 23:17:07 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\df\dist\.tmp-h_a8124z\pymino-1.1.9.8.tar", last modified: Sat Jun 17 03:41:38 2023, max compression
```

## Comparing `pymino-1.1.9.7.tar` & `pymino-1.1.9.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 23:17:07.373886 pymino-1.1.9.7/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.9.7/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-06-16 23:17:07.373886 pymino-1.1.9.7/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.9.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 23:17:07.307918 pymino-1.1.9.7/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-16 23:07:27.000000 pymino-1.1.9.7/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.9.7/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30208 2023-06-15 01:47:51.000000 pymino-1.1.9.7/pymino/bot.py
--rw-rw-rw-   0        0        0    52363 2023-06-16 20:35:00.000000 pymino-1.1.9.7/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:17:07.336190 pymino-1.1.9.7/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-11 16:50:39.000000 pymino-1.1.9.7/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.9.7/pymino/ext/account.py
--rw-rw-rw-   0        0        0   306772 2023-06-16 23:13:50.000000 pymino-1.1.9.7/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.9.7/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    24095 2023-06-16 22:46:59.000000 pymino-1.1.9.7/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.9.7/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   305392 2023-06-16 23:13:10.000000 pymino-1.1.9.7/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-11 22:20:09.000000 pymino-1.1.9.7/pymino/ext/console.py
--rw-rw-rw-   0        0        0    42094 2023-06-16 22:12:03.000000 pymino-1.1.9.7/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.9.7/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:17:07.358510 pymino-1.1.9.7/pymino/ext/entities/
--rw-rw-rw-   0        0        0      355 2023-06-16 21:57:42.000000 pymino-1.1.9.7/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-06-16 23:16:13.000000 pymino-1.1.9.7/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     1670 2023-06-16 23:16:17.000000 pymino-1.1.9.7/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    20322 2023-06-16 23:16:20.000000 pymino-1.1.9.7/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.9.7/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.9.7/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15638 2023-06-16 21:42:30.000000 pymino-1.1.9.7/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.9.7/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-11 21:21:53.000000 pymino-1.1.9.7/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.9.7/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-06-16 21:57:33.000000 pymino-1.1.9.7/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-06-16 21:59:23.000000 pymino-1.1.9.7/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.9.7/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.9.7/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.9.7/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.9.7/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.9.7/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:17:07.372894 pymino-1.1.9.7/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-11 17:31:29.000000 pymino-1.1.9.7/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.9.7/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-13 04:27:21.000000 pymino-1.1.9.7/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.9.7/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-11 22:22:27.000000 pymino-1.1.9.7/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.9.7/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-11 21:47:35.000000 pymino-1.1.9.7/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-13 03:31:19.000000 pymino-1.1.9.7/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.9.7/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:17:07.319822 pymino-1.1.9.7/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-06-16 23:17:07.000000 pymino-1.1.9.7/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1380 2023-06-16 23:17:07.000000 pymino-1.1.9.7/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 23:17:07.000000 pymino-1.1.9.7/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-16 23:17:07.000000 pymino-1.1.9.7/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-16 23:17:07.000000 pymino-1.1.9.7/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-16 23:17:07.379838 pymino-1.1.9.7/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 03:41:38.071186 pymino-1.1.9.8/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.9.8/LICENSE
+-rw-rw-rw-   0        0        0     7298 2023-06-17 03:41:38.071186 pymino-1.1.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6580 2023-06-17 03:41:22.000000 pymino-1.1.9.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 03:41:38.008195 pymino-1.1.9.8/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-17 03:36:14.000000 pymino-1.1.9.8/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.9.8/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30208 2023-06-15 01:47:51.000000 pymino-1.1.9.8/pymino/bot.py
+-rw-rw-rw-   0        0        0    52363 2023-06-16 20:35:00.000000 pymino-1.1.9.8/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-17 03:41:38.036963 pymino-1.1.9.8/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-11 16:50:39.000000 pymino-1.1.9.8/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.9.8/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   306772 2023-06-16 23:13:50.000000 pymino-1.1.9.8/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.9.8/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    24095 2023-06-16 22:46:59.000000 pymino-1.1.9.8/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.9.8/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   305392 2023-06-16 23:13:10.000000 pymino-1.1.9.8/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-11 22:20:09.000000 pymino-1.1.9.8/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    42101 2023-06-17 03:36:25.000000 pymino-1.1.9.8/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.9.8/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-17 03:41:38.059779 pymino-1.1.9.8/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      355 2023-06-16 21:57:42.000000 pymino-1.1.9.8/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-06-16 23:16:13.000000 pymino-1.1.9.8/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     1670 2023-06-16 23:16:17.000000 pymino-1.1.9.8/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    20322 2023-06-16 23:16:20.000000 pymino-1.1.9.8/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.9.8/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.9.8/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15638 2023-06-16 21:42:30.000000 pymino-1.1.9.8/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.9.8/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-11 21:21:53.000000 pymino-1.1.9.8/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.9.8/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-06-16 21:57:33.000000 pymino-1.1.9.8/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-06-16 21:59:23.000000 pymino-1.1.9.8/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.9.8/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.9.8/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.9.8/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.9.8/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.9.8/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-17 03:41:38.070195 pymino-1.1.9.8/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-11 17:31:29.000000 pymino-1.1.9.8/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.9.8/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-13 04:27:21.000000 pymino-1.1.9.8/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.9.8/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-11 22:22:27.000000 pymino-1.1.9.8/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.9.8/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-11 21:47:35.000000 pymino-1.1.9.8/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-13 03:31:19.000000 pymino-1.1.9.8/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.9.8/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-17 03:41:38.021091 pymino-1.1.9.8/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7298 2023-06-17 03:41:37.000000 pymino-1.1.9.8/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1380 2023-06-17 03:41:37.000000 pymino-1.1.9.8/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 03:41:37.000000 pymino-1.1.9.8/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-17 03:41:37.000000 pymino-1.1.9.8/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-17 03:41:37.000000 pymino-1.1.9.8/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-17 03:41:38.072675 pymino-1.1.9.8/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.9.8/setup.py
```

### Comparing `pymino-1.1.9.7/LICENSE` & `pymino-1.1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/PKG-INFO` & `pymino-1.1.9.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,45 @@
-Metadata-Version: 2.1
-Name: pymino
-Version: 1.1.9.7
-Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
-Home-page: https://github.com/forevercynical/pymino
-Author: forevercynical
-Author-email: me@cynical.gg
-License: MIT
-Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 <div align="center">
-  <h1>pymino</h1>
-  
-  [![Discord](https://img.shields.io/discord/926853226152755280?color=blueviolet&label=discord%20server)](https://discord.gg/JMJpzpsMNJ)
-  [![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/forevercynical/pymino?color=blueviolet)](https://libraries.io/github/forevercynical/pymino)
-  [![GitHub last commit](https://img.shields.io/github/last-commit/forevercynical/pymino?label=last%20updated&color=blueviolet)](https://github.com/forevercynical/pymino/commits/main)
-  [![PyPI - Downloads](https://img.shields.io/pypi/dw/pymino?color=blueviolet)](https://pypi.org/project/pymino/)
-  
-  <p>A Python wrapper to communicate with the Amino Apps API.</p>
-  <p>Easily create a bot for Amino Apps using a modern, easy-to-use, synchronous library.</p>
-  
-  <p>If you have any questions or need help, feel free to join the Discord server.</p>
+  <h1 style="color: #0d47a1; font-size: 3em;">pymino</h1>
   
+  <p>
+    <a href="https://discord.gg/JMJpzpsMNJ"><img src="https://img.shields.io/discord/926853226152755280?color=blueviolet&label=discord%20server" alt="Discord"></a>
+    <a href="https://libraries.io/github/forevercynical/pymino"><img src="https://img.shields.io/librariesio/github/forevercynical/pymino?color=blueviolet" alt="Libraries.io dependency status for GitHub repo"></a>
+    <a href="https://github.com/forevercynical/pymino/commits/main"><img src="https://img.shields.io/github/last-commit/forevercynical/pymino?label=last%20updated&color=blueviolet" alt="GitHub last commit"></a>
+    <a href="https://pypi.org/project/pymino/"><img src="https://img.shields.io/pypi/dw/pymino?color=blueviolet" alt="PyPI - Downloads"></a>
+  </p>
+
+  <p style="font-size: 1.2em; color: #424242;">A Python wrapper to communicate with the Amino Apps API.</p>
+  <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use, synchronous library.</p>
+
+  <div style="border: 3px solid red; padding: 10px; margin: 15px 0;">
+    <h3 style="color: red;"><strong> WARNING </strong></h3>
+    <p><strong>Pymino is a fully reverse-engineered client. By using this client, you may be violating the Amino Apps' Terms of Service. This could lead to your account being suspended or permanently banned. Please use Pymino responsibly and at your own risk.</strong></p>
+    <p><strong>Understand that the developers and maintainers of Pymino are not responsible for any actions taken against your account as a result of using this client. Proceed with caution.</strong></p>
+  </div>
+
+  <p style="font-size: 1.2em; color: #424242;">If you have any questions or need help, feel free to join the Discord server.</p>
   
   <a href="https://discord.gg/JMJpzpsMNJ">
     <img src="https://cdn.discordapp.com/attachments/965797874791223317/1081754594977267833/discord-button.png" alt="Join Our Discord Server" width="150" height="50">
   </a>
   
-  <h2>Installation</h2>
+  <h2 style="color: #0d47a1; font-size: 2em;">Installation</h2>
   
-  <p>Recommended installation method is through pip:</p>
+  <p style="font-size: 1.2em; color: #424242;">Recommended installation method is through pip:</p>
   
-  <pre><code>pip install pymino</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">pip install pymino</code></pre>
   
-  <p>Alternatively, you can clone the repository and install it manually:</p>
+  <p style="font-size: 1.2em; color: #424242;">Alternatively, you can clone the repository and install it manually:</p>
   
-  <pre><code>git clone https://github.com/forevercynical/pymino.git
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">git clone https://github.com/forevercynical/pymino.git
   cd pymino
   python setup.py install</code></pre>
   
-  <p>For more detailed documentation and usage examples, check out the project's <a href="https://pymino.info/index.html">official documentation</a>.</p>
+  <p style="font-size: 1.2em; color: #424242;">For more detailed documentation and usage examples, check out the project's <a href="https://pymino.info/index.html">official documentation</a>.</p>
 </div>
 
 <div>
   <h2 align="center">Client Class Usage</h2>
 
   <pre><code class="language-python">
 >>> from pymino import Client
```

#### html2text {}

```diff
@@ -1,31 +1,21 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.9.7 Summary: Easily create a
-bot for Amino Apps using a modern easy to use synchronous library. Home-page:
-https://github.com/forevercynical/pymino Author: forevercynical Author-email:
-me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
-bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE
                              ****** pymino ******
-                  [![Discord](https://img.shields.io/discord/
-     926853226152755280?color=blueviolet&label=discord%20server)](https://
-   discord.gg/JMJpzpsMNJ) [![Libraries.io dependency status for GitHub repo]
-          (https://img.shields.io/librariesio/github/forevercynical/
-pymino?color=blueviolet)](https://libraries.io/github/forevercynical/pymino) [!
-[GitHub last commit](https://img.shields.io/github/last-commit/forevercynical/
-      pymino?label=last%20updated&color=blueviolet)](https://github.com/
-       forevercynical/pymino/commits/main) [![PyPI - Downloads](https://
-  img.shields.io/pypi/dw/pymino?color=blueviolet)](https://pypi.org/project/
-                                   pymino/)
+[Discord] [Libraries.io_dependency_status_for_GitHub_repo] [GitHub_last_commit]
+                              [PyPI_-_Downloads]
            A Python wrapper to communicate with the Amino Apps API.
   Easily create a bot for Amino Apps using a modern, easy-to-use, synchronous
                                    library.
+                               **** WARNING ****
+ Pymino is a fully reverse-engineered client. By using this client, you may be
+  violating the Amino Apps' Terms of Service. This could lead to your account
+  being suspended or permanently banned. Please use Pymino responsibly and at
+                                your own risk.
+ Understand that the developers and maintainers of Pymino are not responsible
+ for any actions taken against your account as a result of using this client.
+                             Proceed with caution.
  If you have any questions or need help, feel free to join the Discord server.
                            [Join_Our_Discord_Server]
                            ***** Installation *****
                 Recommended installation method is through pip:
                               pip install pymino
      Alternatively, you can clone the repository and install it manually:
             git clone https://github.com/forevercynical/pymino.git
```

### Comparing `pymino-1.1.9.7/pymino/__init__.py` & `pymino-1.1.9.8/pymino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.9.7'
+__version__ = '1.1.9.8'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.1.9.7/pymino/async_bot.py` & `pymino-1.1.9.8/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/bot.py` & `pymino-1.1.9.8/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/client.py` & `pymino-1.1.9.8/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/account.py` & `pymino-1.1.9.8/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/async_community.py` & `pymino-1.1.9.8/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/async_context.py` & `pymino-1.1.9.8/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/async_event_handler.py` & `pymino-1.1.9.8/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/async_socket.py` & `pymino-1.1.9.8/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/community.py` & `pymino-1.1.9.8/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/console.py` & `pymino-1.1.9.8/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/context.py` & `pymino-1.1.9.8/pymino/ext/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1251,15 +1251,15 @@
             if event == "text_message":
                 context = self.context(data, self.request, self.intents)
                 if all([self.intents, not self.command_exists(
                     command_name=data.content[len(self.command_prefix):].split(" ")[0]
                     )]):
                         self._add_cache(data.chatId, data.author.userId, data.content)
 
-                self._handle_command(data=data, context=context)
+                return self._handle_command(data=data, context=context)
             
             if event in self._events:
                 context = self.context(data, self.request, self.intents)
 
                 if event in {
                     "user_online",
                     "member_set_you_host",
```

### Comparing `pymino-1.1.9.7/pymino/ext/dispatcher.py` & `pymino-1.1.9.8/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/acm.py` & `pymino-1.1.9.8/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/api_response.py` & `pymino-1.1.9.8/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/chat_threads.py` & `pymino-1.1.9.8/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/comments.py` & `pymino-1.1.9.8/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/enums.py` & `pymino-1.1.9.8/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/exceptions.py` & `pymino-1.1.9.8/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/general.py` & `pymino-1.1.9.8/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/handlers.py` & `pymino-1.1.9.8/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/link_info.py` & `pymino-1.1.9.8/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/member.py` & `pymino-1.1.9.8/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/messages.py` & `pymino-1.1.9.8/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/notification.py` & `pymino-1.1.9.8/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/userprofile.py` & `pymino-1.1.9.8/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/entities/wsevents.py` & `pymino-1.1.9.8/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/handle_queue.py` & `pymino-1.1.9.8/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/socket.py` & `pymino-1.1.9.8/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/utilities/async_request_handler.py` & `pymino-1.1.9.8/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/utilities/chat_console.py` & `pymino-1.1.9.8/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/utilities/commands.py` & `pymino-1.1.9.8/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/utilities/community_console.py` & `pymino-1.1.9.8/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/utilities/generate.py` & `pymino-1.1.9.8/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/utilities/menu.py` & `pymino-1.1.9.8/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/utilities/profile_console.py` & `pymino-1.1.9.8/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino/ext/utilities/request_handler.py` & `pymino-1.1.9.8/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/pymino.egg-info/PKG-INFO` & `pymino-1.1.9.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.9.7
+Version: 1.1.9.8
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
@@ -12,46 +12,52 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 <div align="center">
-  <h1>pymino</h1>
-  
-  [![Discord](https://img.shields.io/discord/926853226152755280?color=blueviolet&label=discord%20server)](https://discord.gg/JMJpzpsMNJ)
-  [![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/forevercynical/pymino?color=blueviolet)](https://libraries.io/github/forevercynical/pymino)
-  [![GitHub last commit](https://img.shields.io/github/last-commit/forevercynical/pymino?label=last%20updated&color=blueviolet)](https://github.com/forevercynical/pymino/commits/main)
-  [![PyPI - Downloads](https://img.shields.io/pypi/dw/pymino?color=blueviolet)](https://pypi.org/project/pymino/)
-  
-  <p>A Python wrapper to communicate with the Amino Apps API.</p>
-  <p>Easily create a bot for Amino Apps using a modern, easy-to-use, synchronous library.</p>
-  
-  <p>If you have any questions or need help, feel free to join the Discord server.</p>
+  <h1 style="color: #0d47a1; font-size: 3em;">pymino</h1>
   
+  <p>
+    <a href="https://discord.gg/JMJpzpsMNJ"><img src="https://img.shields.io/discord/926853226152755280?color=blueviolet&label=discord%20server" alt="Discord"></a>
+    <a href="https://libraries.io/github/forevercynical/pymino"><img src="https://img.shields.io/librariesio/github/forevercynical/pymino?color=blueviolet" alt="Libraries.io dependency status for GitHub repo"></a>
+    <a href="https://github.com/forevercynical/pymino/commits/main"><img src="https://img.shields.io/github/last-commit/forevercynical/pymino?label=last%20updated&color=blueviolet" alt="GitHub last commit"></a>
+    <a href="https://pypi.org/project/pymino/"><img src="https://img.shields.io/pypi/dw/pymino?color=blueviolet" alt="PyPI - Downloads"></a>
+  </p>
+
+  <p style="font-size: 1.2em; color: #424242;">A Python wrapper to communicate with the Amino Apps API.</p>
+  <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use, synchronous library.</p>
+
+  <div style="border: 3px solid red; padding: 10px; margin: 15px 0;">
+    <h3 style="color: red;"><strong> WARNING </strong></h3>
+    <p><strong>Pymino is a fully reverse-engineered client. By using this client, you may be violating the Amino Apps' Terms of Service. This could lead to your account being suspended or permanently banned. Please use Pymino responsibly and at your own risk.</strong></p>
+    <p><strong>Understand that the developers and maintainers of Pymino are not responsible for any actions taken against your account as a result of using this client. Proceed with caution.</strong></p>
+  </div>
+
+  <p style="font-size: 1.2em; color: #424242;">If you have any questions or need help, feel free to join the Discord server.</p>
   
   <a href="https://discord.gg/JMJpzpsMNJ">
     <img src="https://cdn.discordapp.com/attachments/965797874791223317/1081754594977267833/discord-button.png" alt="Join Our Discord Server" width="150" height="50">
   </a>
   
-  <h2>Installation</h2>
+  <h2 style="color: #0d47a1; font-size: 2em;">Installation</h2>
   
-  <p>Recommended installation method is through pip:</p>
+  <p style="font-size: 1.2em; color: #424242;">Recommended installation method is through pip:</p>
   
-  <pre><code>pip install pymino</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">pip install pymino</code></pre>
   
-  <p>Alternatively, you can clone the repository and install it manually:</p>
+  <p style="font-size: 1.2em; color: #424242;">Alternatively, you can clone the repository and install it manually:</p>
   
-  <pre><code>git clone https://github.com/forevercynical/pymino.git
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">git clone https://github.com/forevercynical/pymino.git
   cd pymino
   python setup.py install</code></pre>
   
-  <p>For more detailed documentation and usage examples, check out the project's <a href="https://pymino.info/index.html">official documentation</a>.</p>
+  <p style="font-size: 1.2em; color: #424242;">For more detailed documentation and usage examples, check out the project's <a href="https://pymino.info/index.html">official documentation</a>.</p>
 </div>
 
 <div>
   <h2 align="center">Client Class Usage</h2>
 
   <pre><code class="language-python">
 >>> from pymino import Client
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.9.7 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.9.8 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                              ****** pymino ******
-                  [![Discord](https://img.shields.io/discord/
-     926853226152755280?color=blueviolet&label=discord%20server)](https://
-   discord.gg/JMJpzpsMNJ) [![Libraries.io dependency status for GitHub repo]
-          (https://img.shields.io/librariesio/github/forevercynical/
-pymino?color=blueviolet)](https://libraries.io/github/forevercynical/pymino) [!
-[GitHub last commit](https://img.shields.io/github/last-commit/forevercynical/
-      pymino?label=last%20updated&color=blueviolet)](https://github.com/
-       forevercynical/pymino/commits/main) [![PyPI - Downloads](https://
-  img.shields.io/pypi/dw/pymino?color=blueviolet)](https://pypi.org/project/
-                                   pymino/)
+[Discord] [Libraries.io_dependency_status_for_GitHub_repo] [GitHub_last_commit]
+                              [PyPI_-_Downloads]
            A Python wrapper to communicate with the Amino Apps API.
   Easily create a bot for Amino Apps using a modern, easy-to-use, synchronous
                                    library.
+                               **** WARNING ****
+ Pymino is a fully reverse-engineered client. By using this client, you may be
+  violating the Amino Apps' Terms of Service. This could lead to your account
+  being suspended or permanently banned. Please use Pymino responsibly and at
+                                your own risk.
+ Understand that the developers and maintainers of Pymino are not responsible
+ for any actions taken against your account as a result of using this client.
+                             Proceed with caution.
  If you have any questions or need help, feel free to join the Discord server.
                            [Join_Our_Discord_Server]
                            ***** Installation *****
                 Recommended installation method is through pip:
                               pip install pymino
      Alternatively, you can clone the repository and install it manually:
             git clone https://github.com/forevercynical/pymino.git
```

### Comparing `pymino-1.1.9.7/pymino.egg-info/SOURCES.txt` & `pymino-1.1.9.8/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.7/setup.cfg` & `pymino-1.1.9.8/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e39 2e37 0d0a 6175  on = 1.1.9.7..au
+00000020: 6f6e 203d 2031 2e31 2e39 2e38 0d0a 6175  on = 1.1.9.8..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.9.7/setup.py` & `pymino-1.1.9.8/setup.py`

 * *Files identical despite different names*

