# Comparing `tmp/nonebot_plugin_treehelp-0.2.0.tar.gz` & `tmp/nonebot_plugin_treehelp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_treehelp-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_treehelp-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_treehelp-0.2.0.tar` & `nonebot_plugin_treehelp-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-06-06 08:36:24.907264 nonebot_plugin_treehelp-0.2.0/LICENSE
--rw-r--r--   0        0        0     2452 2023-06-06 08:36:24.907264 nonebot_plugin_treehelp-0.2.0/README.md
--rw-r--r--   0        0        0     1585 2023-06-06 08:36:24.907264 nonebot_plugin_treehelp-0.2.0/nonebot_plugin_treehelp/__init__.py
--rw-r--r--   0        0        0     5532 2023-06-06 08:36:24.907264 nonebot_plugin_treehelp-0.2.0/nonebot_plugin_treehelp/data_source.py
--rw-r--r--   0        0        0     1348 2023-06-06 08:36:24.907264 nonebot_plugin_treehelp-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3266 1970-01-01 00:00:00.000000 nonebot_plugin_treehelp-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-17 14:47:05.931916 nonebot_plugin_treehelp-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2550 2023-06-17 14:47:05.935916 nonebot_plugin_treehelp-0.3.0/README.md
+-rw-r--r--   0        0        0     1631 2023-06-17 14:47:05.935916 nonebot_plugin_treehelp-0.3.0/nonebot_plugin_treehelp/__init__.py
+-rw-r--r--   0        0        0      289 2023-06-17 14:47:05.935916 nonebot_plugin_treehelp-0.3.0/nonebot_plugin_treehelp/config.py
+-rw-r--r--   0        0        0     5660 2023-06-17 14:47:05.935916 nonebot_plugin_treehelp-0.3.0/nonebot_plugin_treehelp/data_source.py
+-rw-r--r--   0        0        0     1348 2023-06-17 14:47:05.935916 nonebot_plugin_treehelp-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3364 1970-01-01 00:00:00.000000 nonebot_plugin_treehelp-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_treehelp-0.2.0/LICENSE` & `nonebot_plugin_treehelp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_treehelp-0.2.0/README.md` & `nonebot_plugin_treehelp-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -58,24 +58,27 @@
 通过设置 adapters 属性来指定支持的适配器。如果不设置或留空则默认支持全部适配器。如果插件不支持该适配器，则不会在帮助列表上显示。
 
 ```python
 __plugin_meta__ = PluginMetadata(
     name="OneBot",
     description="测试 OneBot 适配器",
     usage="/onebot",
-    extra={
-        "adapters": ["OneBot V11"],
-    },
+    type="application",
+    supported_adapters={"~onebot.v11", "~onebot.v12"},
 )
 ```
 
 ## 配置项
 
 配置方式：直接在 `NoneBot` 全局配置文件中添加以下配置项即可。
 
-暂时还没有可配置的东西。
+### treehelp_ignored_plugins
+
+- 类型: `list[str]`
+- 默认: `[]`
+- 说明: 需要忽略的插件名称列表
 
 ## 计划
 
 - [ ] 支持输出插件版本
 - [x] 支持输出插件树
 - [ ] 支持输出插件内的命令名称
```

#### html2text {}

```diff
@@ -11,12 +11,13 @@
 æµè¯æä»¶äºçº§æä»¶ âââ ç®ååè½ # æµè¯æä»¶ç®åå­æä»¶
 ``` ## ä½¿ç¨æ¹å¼ å è½½æä»¶ååé `/help help` æ `/help --help`
 è·åå·ä½ç¨æ³ã ## æä»¶éé æä»¶ä¸å­æä»¶åæ³å¯åè
 [ç¤ºä¾æä»¶](./tests/plugins/tree/)ã ### å£°æééå¨ éè¿è®¾ç½®
 adapters
 å±æ§æ¥æå®æ¯æçééå¨ãå¦æä¸è®¾ç½®æçç©ºåé»è®¤æ¯æå¨é¨ééå¨ãå¦ææä»¶ä¸æ¯æè¯¥ééå¨ï¼åä¸ä¼å¨å¸®å©åè¡¨ä¸æ¾ç¤ºã
 ```python __plugin_meta__ = PluginMetadata( name="OneBot", description="æµè¯
-OneBot ééå¨", usage="/onebot", extra={ "adapters": ["OneBot V11"], }, )
-``` ## éç½®é¡¹ éç½®æ¹å¼ï¼ç´æ¥å¨ `NoneBot`
-å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã
-ææ¶è¿æ²¡æå¯éç½®çä¸è¥¿ã ## è®¡å - [ ] æ¯æè¾åºæä»¶çæ¬ -
+OneBot ééå¨", usage="/onebot", type="application", supported_adapters=
+{"~onebot.v11", "~onebot.v12"}, ) ``` ## éç½®é¡¹ éç½®æ¹å¼ï¼ç´æ¥å¨
+`NoneBot` å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ###
+treehelp_ignored_plugins - ç±»å: `list[str]` - é»è®¤: `[]` - è¯´æ:
+éè¦å¿½ç¥çæä»¶åç§°åè¡¨ ## è®¡å - [ ] æ¯æè¾åºæä»¶çæ¬ -
 [x] æ¯æè¾åºæä»¶æ  - [ ] æ¯æè¾åºæä»¶åçå½ä»¤åç§°
```

### Comparing `nonebot_plugin_treehelp-0.2.0/nonebot_plugin_treehelp/__init__.py` & `nonebot_plugin_treehelp-0.3.0/nonebot_plugin_treehelp/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from nonebot import on_shell_command
 from nonebot.adapters import Bot
 from nonebot.exception import ParserExit
 from nonebot.params import ShellCommandArgs
 from nonebot.plugin import PluginMetadata
 from nonebot.rule import ArgumentParser, Namespace
 
+from .config import Config
 from .data_source import get_plugin_help, get_plugin_list
 
 __plugin_meta__ = PluginMetadata(
     name="帮助",
     description="获取插件帮助信息",
     usage="""获取插件列表
 /help
@@ -22,14 +23,15 @@
 获取某个插件的帮助
 /help 插件名
 获取某个插件的树
 /help --tree 插件名
 """,
     type="application",
     homepage="https://github.com/he0119/nonebot-plugin-treehelp",
+    config=Config,
 )
 
 parser = ArgumentParser("帮助", description="获取插件帮助信息")
 parser.add_argument("plugin_name", nargs="?", type=str, help="插件名", metavar="插件名")
 parser.add_argument("-t", "--tree", action="store_true", help="获取插件树")
 help_cmd = on_shell_command("help", aliases={"帮助"}, parser=parser)
```

### Comparing `nonebot_plugin_treehelp-0.2.0/nonebot_plugin_treehelp/data_source.py` & `nonebot_plugin_treehelp-0.3.0/nonebot_plugin_treehelp/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 获取插件的帮助信息，并通过子插件的形式获取次级菜单
 """
 from typing import TYPE_CHECKING, Dict, List, Optional, Set, Tuple, Union, cast
 
 from nonebot import get_driver, get_loaded_plugins
 from nonebot.rule import CommandRule, ShellCommandRule
 
+from .config import plugin_config
+
 if TYPE_CHECKING:
     from nonebot.adapters import Bot
     from nonebot.plugin import Plugin, PluginMetadata
 
 global_config = get_driver().config
 
 _plugins: Optional[Dict[str, "Plugin"]] = None
@@ -82,14 +84,17 @@
 
 
 def is_supported(bot: "Bot", plugin: "Plugin") -> bool:
     """是否是支持的插件"""
     if plugin.metadata is None:
         return False
 
+    if plugin.metadata.name in plugin_config.treehelp_ignored_plugins:
+        return False
+
     if not is_supported_type(plugin.metadata):
         return False
 
     if not is_supported_adapter(bot, plugin.metadata):
         return False
 
     return True
```

### Comparing `nonebot_plugin_treehelp-0.2.0/pyproject.toml` & `nonebot_plugin_treehelp-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-treehelp"
-version = "0.2.0"
+version = "0.3.0"
 description = "适用于 Nonebot2 的树形帮助插件"
 authors = ["hemengyang <hmy0119@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/he0119/nonebot-plugin-treehelp"
 repository = "https://github.com/he0119/nonebot-plugin-treehelp"
 documentation = "https://github.com/he0119/nonebot-plugin-treehelp#readme"
```

### Comparing `nonebot_plugin_treehelp-0.2.0/PKG-INFO` & `nonebot_plugin_treehelp-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-treehelp
-Version: 0.2.0
+Version: 0.3.0
 Summary: 适用于 Nonebot2 的树形帮助插件
 Home-page: https://github.com/he0119/nonebot-plugin-treehelp
 License: MIT
 Author: hemengyang
 Author-email: hmy0119@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -78,25 +78,28 @@
 通过设置 adapters 属性来指定支持的适配器。如果不设置或留空则默认支持全部适配器。如果插件不支持该适配器，则不会在帮助列表上显示。
 
 ```python
 __plugin_meta__ = PluginMetadata(
     name="OneBot",
     description="测试 OneBot 适配器",
     usage="/onebot",
-    extra={
-        "adapters": ["OneBot V11"],
-    },
+    type="application",
+    supported_adapters={"~onebot.v11", "~onebot.v12"},
 )
 ```
 
 ## 配置项
 
 配置方式：直接在 `NoneBot` 全局配置文件中添加以下配置项即可。
 
-暂时还没有可配置的东西。
+### treehelp_ignored_plugins
+
+- 类型: `list[str]`
+- 默认: `[]`
+- 说明: 需要忽略的插件名称列表
 
 ## 计划
 
 - [ ] 支持输出插件版本
 - [x] 支持输出插件树
 - [ ] 支持输出插件内的命令名称
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-treehelp Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-treehelp Version: 0.3.0 Summary:
 éç¨äº Nonebot2 çæ å½¢å¸®å©æä»¶ Home-page: https://github.com/he0119/
 nonebot-plugin-treehelp License: MIT Author: hemengyang Author-email:
 hmy0119@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot2
@@ -22,12 +22,13 @@
 æµè¯æä»¶äºçº§æä»¶ âââ ç®ååè½ # æµè¯æä»¶ç®åå­æä»¶
 ``` ## ä½¿ç¨æ¹å¼ å è½½æä»¶ååé `/help help` æ `/help --help`
 è·åå·ä½ç¨æ³ã ## æä»¶éé æä»¶ä¸å­æä»¶åæ³å¯åè
 [ç¤ºä¾æä»¶](./tests/plugins/tree/)ã ### å£°æééå¨ éè¿è®¾ç½®
 adapters
 å±æ§æ¥æå®æ¯æçééå¨ãå¦æä¸è®¾ç½®æçç©ºåé»è®¤æ¯æå¨é¨ééå¨ãå¦ææä»¶ä¸æ¯æè¯¥ééå¨ï¼åä¸ä¼å¨å¸®å©åè¡¨ä¸æ¾ç¤ºã
 ```python __plugin_meta__ = PluginMetadata( name="OneBot", description="æµè¯
-OneBot ééå¨", usage="/onebot", extra={ "adapters": ["OneBot V11"], }, )
-``` ## éç½®é¡¹ éç½®æ¹å¼ï¼ç´æ¥å¨ `NoneBot`
-å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã
-ææ¶è¿æ²¡æå¯éç½®çä¸è¥¿ã ## è®¡å - [ ] æ¯æè¾åºæä»¶çæ¬ -
+OneBot ééå¨", usage="/onebot", type="application", supported_adapters=
+{"~onebot.v11", "~onebot.v12"}, ) ``` ## éç½®é¡¹ éç½®æ¹å¼ï¼ç´æ¥å¨
+`NoneBot` å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ###
+treehelp_ignored_plugins - ç±»å: `list[str]` - é»è®¤: `[]` - è¯´æ:
+éè¦å¿½ç¥çæä»¶åç§°åè¡¨ ## è®¡å - [ ] æ¯æè¾åºæä»¶çæ¬ -
 [x] æ¯æè¾åºæä»¶æ  - [ ] æ¯æè¾åºæä»¶åçå½ä»¤åç§°
```

