# Comparing `tmp/meowerbot-2.6.1.tar.gz` & `tmp/meowerbot-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meowerbot-2.6.1.tar", max compression
+gzip compressed data, was "meowerbot-2.6.2.tar", max compression
```

## Comparing `meowerbot-2.6.1.tar` & `meowerbot-2.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.6.1/LICENSE
--rw-r--r--   0        0        0      191 2023-06-17 05:37:22.980987 meowerbot-2.6.1/MeowerBot/__init__.py
--rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.6.1/MeowerBot/_Commands.py
--rw-r--r--   0        0        0     1381 2023-05-24 23:08:36.965919 meowerbot-2.6.1/MeowerBot/API.py
--rw-r--r--   0        0        0    14580 2023-06-17 05:35:58.108283 meowerbot-2.6.1/MeowerBot/Bot.py
--rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.6.1/MeowerBot/cl/__init__.py
--rw-r--r--   0        0        0     8937 2023-06-17 04:05:40.519304 meowerbot-2.6.1/MeowerBot/cl/cloudlink.py
--rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.6.1/MeowerBot/cog.py
--rw-r--r--   0        0        0     3543 2023-06-17 03:52:08.597897 meowerbot-2.6.1/MeowerBot/command.py
--rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.6.1/MeowerBot/context.py
--rw-r--r--   0        0        0     1639 2023-06-17 05:37:22.981985 meowerbot-2.6.1/MeowerBot/ext/discord.py
--rw-r--r--   0        0        0     1941 2023-06-17 04:53:04.923013 meowerbot-2.6.1/MeowerBot/ext/help.py
--rw-r--r--   0        0        0      681 2023-06-17 05:37:22.981985 meowerbot-2.6.1/pyproject.toml
--rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.6.1/README.md
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 meowerbot-2.6.1/setup.py
--rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 meowerbot-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.6.2/LICENSE
+-rw-r--r--   0        0        0      191 2023-06-17 19:53:47.067042 meowerbot-2.6.2/MeowerBot/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.6.2/MeowerBot/_Commands.py
+-rw-r--r--   0        0        0     1381 2023-05-24 23:08:36.965919 meowerbot-2.6.2/MeowerBot/API.py
+-rw-r--r--   0        0        0    14580 2023-06-17 05:35:58.108283 meowerbot-2.6.2/MeowerBot/Bot.py
+-rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.6.2/MeowerBot/cl/__init__.py
+-rw-r--r--   0        0        0     8937 2023-06-17 04:05:40.519304 meowerbot-2.6.2/MeowerBot/cl/cloudlink.py
+-rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.6.2/MeowerBot/cog.py
+-rw-r--r--   0        0        0     3543 2023-06-17 03:52:08.597897 meowerbot-2.6.2/MeowerBot/command.py
+-rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.6.2/MeowerBot/context.py
+-rw-r--r--   0        0        0     1639 2023-06-17 05:37:22.981985 meowerbot-2.6.2/MeowerBot/ext/discord.py
+-rw-r--r--   0        0        0     2315 2023-06-17 19:48:22.139910 meowerbot-2.6.2/MeowerBot/ext/help.py
+-rw-r--r--   0        0        0      681 2023-06-17 19:53:47.067042 meowerbot-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.6.2/README.md
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 meowerbot-2.6.2/setup.py
+-rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 meowerbot-2.6.2/PKG-INFO
```

### Comparing `meowerbot-2.6.1/LICENSE` & `meowerbot-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meowerbot-2.6.1/MeowerBot/API.py` & `meowerbot-2.6.2/MeowerBot/API.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.6.1/MeowerBot/Bot.py` & `meowerbot-2.6.2/MeowerBot/Bot.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.6.1/MeowerBot/cl/cloudlink.py` & `meowerbot-2.6.2/MeowerBot/cl/cloudlink.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.6.1/MeowerBot/cog.py` & `meowerbot-2.6.2/MeowerBot/cog.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.6.1/MeowerBot/command.py` & `meowerbot-2.6.2/MeowerBot/command.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.6.1/MeowerBot/context.py` & `meowerbot-2.6.2/MeowerBot/context.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.6.1/MeowerBot/ext/discord.py` & `meowerbot-2.6.2/MeowerBot/ext/discord.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.6.1/MeowerBot/ext/help.py` & `meowerbot-2.6.2/MeowerBot/ext/help.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 import inspect
 
 def _get_index_or(l, i, d):
 	try:
 		r = l[i]
 		if str(r) == str(inspect._empty):
 			return d
-		return r
+		return r.__name__
 	except IndexError:
 		return d
 
 class Help(Cog):
 	def __init__(self, bot, *args, **kwargs):
 		self.bot = bot
 		self.page = ""
+		self.bot.callback(self._login, "login")
 		Cog.__init__(self)
-
+		
 		
 
 	def generate_help(self):
+		if self.bot.prefix == f"@{self.bot.username}":
+			self.bot.prefix = f"@{self.bot.username} "
 		self.pages = []
 		self.page = ""
 		page_size = 0
 		for name, cog in self.bot.cogs.items():
 
 			self.page+= f"-- [ {name} ] --\n"
 			page_size = len(self.page)
@@ -49,20 +52,23 @@
 			if page_size >= 500:
 				self.pages.append(page)
 				self.page = f"-- [ Unsorted ] --\n"
 				page_size = len(self.page)
 
 		self.pages.append(self.page)
 
+		if self.bot.prefix == f"@{self.bot.username} ":
+			self.bot.prefix = f"@{self.bot.username}"
+
 	
 	def handle_command(self, name, cmd):
 		self.page += (f"{self.bot.prefix}{name} ")
 
 		for arg in cmd.args:
-			self.page += f"<{arg[0][0]}: {str(_get_index_or(arg, 1, 'any'))}> "
+			self.page += f"<{arg[0]}: {str(_get_index_or(arg, 1, 'any'))}> "
 
 		
 		for arg in cmd.optional_args:
 			self.page += f"[{arg[0]}: {str(_get_index_or(arg, 1, 'any'))}: optional ] "
 		
 		self.page += "\n"
 
@@ -76,9 +82,13 @@
 	@command(name="help")
 	def help(self, ctx, page: int=0):
 
 		if page >= len(self.pages):
 			page = len(self.pages) - 1
 		
 		ctx.send_msg(self.pages[page])
+	
+
+	def _login(self, bot):
+		self.generate_help() #generate help on login, bugfix for default prefix and people being dumb
```

### Comparing `meowerbot-2.6.1/pyproject.toml` & `meowerbot-2.6.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MeowerBot"
-version = "2.6.1"
+version = "2.6.2"
 description = "A meower bot lib for py"
 authors = ["showierdata9978 <68120127+showierdata9978@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "MeowerBot"}
 ]
```

### Comparing `meowerbot-2.6.1/setup.py` & `meowerbot-2.6.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['requests>=2.28.0,<3.0.0', 'websocket-client']
 
 extras_require = \
 {':python_version < "3.11"': ['backports-strenum>=1.2.4,<2.0.0']}
 
 setup_kwargs = {
     'name': 'meowerbot',
-    'version': '2.6.1',
+    'version': '2.6.2',
     'description': 'A meower bot lib for py',
     'long_description': '# MeowerBot.py\n\nA bot lib for Meower\n\n\n## License\n\nsee [LICENSE](./LICENSE)\n\n\n## docs\n\nThe Docs are located [here](https://meowerbot-py.showierdata.tech/)\n\n\n## Quick Example\n\nlook at the [tests directory](./tests) for examples ',
     'author': 'showierdata9978',
     'author_email': '68120127+showierdata9978@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/MeowerBots/MeowerBot.py',
```

### Comparing `meowerbot-2.6.1/PKG-INFO` & `meowerbot-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meowerbot
-Version: 2.6.1
+Version: 2.6.2
 Summary: A meower bot lib for py
 Home-page: https://github.com/MeowerBots/MeowerBot.py
 License: MIT
 Author: showierdata9978
 Author-email: 68120127+showierdata9978@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

