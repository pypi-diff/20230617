# Comparing `tmp/nonebot_plugin_couplets-0.1.0.tar.gz` & `tmp/nonebot_plugin_couplets-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_couplets-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_couplets-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_couplets-0.1.0.tar` & `nonebot_plugin_couplets-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    34523 2023-01-03 10:42:16.797036 nonebot_plugin_couplets-0.1.0/LICENSE
--rw-r--r--   0        0        0     1909 2023-01-03 10:42:16.797036 nonebot_plugin_couplets-0.1.0/README.md
--rw-r--r--   0        0        0     1563 2023-01-03 10:42:16.797036 nonebot_plugin_couplets-0.1.0/nonebot_plugin_couplets/__init__.py
--rw-r--r--   0        0        0      656 2023-01-03 10:42:16.797036 nonebot_plugin_couplets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2753 1970-01-01 00:00:00.000000 nonebot_plugin_couplets-0.1.0/setup.py
--rw-r--r--   0        0        0     2691 1970-01-01 00:00:00.000000 nonebot_plugin_couplets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-17 07:46:18.918986 nonebot_plugin_couplets-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1218 2023-06-17 07:46:18.918986 nonebot_plugin_couplets-0.2.0/README.md
+-rw-r--r--   0        0        0     1614 2023-06-17 07:46:18.918986 nonebot_plugin_couplets-0.2.0/nonebot_plugin_couplets/__init__.py
+-rw-r--r--   0        0        0      619 2023-06-17 07:46:18.918986 nonebot_plugin_couplets-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 nonebot_plugin_couplets-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_couplets-0.1.0/LICENSE` & `nonebot_plugin_couplets-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_couplets-0.1.0/README.md` & `nonebot_plugin_couplets-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -22,52 +22,19 @@
 
 ## 📖 介绍
 
 基于[王斌给您对对联API](https://ai.binwang.me/couplet/)的Nonebot2对对联插件。
 
 ## 💿 安装
 
-<details>
-<summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
-    nb plugin install nonebot-plugin-couplets
-
-</details>
-
-<details>
-<summary>使用包管理器安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
-
-<details>
-<summary>pip</summary>
-
-    pip install nonebot-plugin-couplets
-</details>
-<details>
-<summary>pdm</summary>
-
-    pdm add nonebot-plugin-couplets
-</details>
-<details>
-<summary>poetry</summary>
-
-    poetry add nonebot-plugin-couplets
-</details>
-<details>
-<summary>conda</summary>
-
-    conda install nonebot-plugin-couplets
-</details>
-
-打开 nonebot2 项目的 `bot.py` 文件, 在其中写入
-
-    nonebot.load_plugin('nonebot_plugin_couplets')
-
-</details>
+```shell
+nb plugin install nonebot-plugin-couplets
+```
 
 
 ## ☀ ️指令
 ```
 对联 <上联内容> (数量)
 · 数量可选，默认为1
 ```
```

#### html2text {}

```diff
@@ -1,16 +1,10 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-couplets _â¨ Nonebot2å¯¹å¯¹èæä»¶ â¨_ [license] [pypi]
                                    [python]
 ## ð ä»ç» åºäº[çæç»æ¨å¯¹å¯¹èAPI](https://ai.binwang.me/couplet/
-)çNonebot2å¯¹å¯¹èæä»¶ã ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨
-nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
-nb plugin install nonebot-plugin-couplets   ä½¿ç¨åç®¡çå¨å®è£ å¨
-nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
-æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install
-nonebot-plugin-couplets   pdm pdm add nonebot-plugin-couplets   poetry poetry
-add nonebot-plugin-couplets   conda conda install nonebot-plugin-couplets
-æå¼ nonebot2 é¡¹ç®ç `bot.py` æä»¶, å¨å¶ä¸­åå¥ nonebot.load_plugin
-('nonebot_plugin_couplets')  ## â ï¸æä»¤ ``` å¯¹è <ä¸èåå®¹>
-(æ°é) Â· æ°éå¯éï¼é»è®¤ä¸º1 ``` ä¾å¦ï¼`å¯¹è
+)çNonebot2å¯¹å¯¹èæä»¶ã ## ð¿ å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```shell
+nb plugin install nonebot-plugin-couplets ``` ## â ï¸æä»¤ ``` å¯¹è
+<ä¸èåå®¹> (æ°é) Â· æ°éå¯éï¼é»è®¤ä¸º1 ``` ä¾å¦ï¼`å¯¹è
 èå©å½å®¶çæ­»ä»¥ 3`
```

### Comparing `nonebot_plugin_couplets-0.1.0/nonebot_plugin_couplets/__init__.py` & `nonebot_plugin_couplets-0.2.0/nonebot_plugin_couplets/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-from typing import List
-
 import httpx
 from nonebot import on_command
-from nonebot.adapters.onebot.v11 import Message
-from nonebot.adapters.onebot.v11.helpers import Numbers
+from nonebot.adapters import Message
 from nonebot.params import CommandArg
 from nonebot.plugin import PluginMetadata
 from nonebot.typing import T_State
 
 __plugin_meta__ = PluginMetadata(
     name="对对联",
     description="人工智能和你对对联",
-    usage="对联<内容>(数量)",
+    usage="对联<内容> (数量)",
+    type="application",
+    homepage="https://github.com/CMHopeSunshine/nonebot-plugin-couplets",
+    supported_adapters=None,
     extra={
         "author":  "惜月 <277073121@qq.com>",
         "version": "1.0.0",
     },
 )
 
 couplets = on_command('对联', aliases={'对对联'}, priority=13, block=True, state={
-    'pm_usage': '对联<内容>(数量)',
+    'pm_usage': '对联<内容> (数量)',
     'pm_describe': '人工智能和你对对联',
     'pm_priority': 15
 })
 
 
 @couplets.handle()
-async def _(state: T_State, msg: Message = CommandArg(), num: List[float] = Numbers()):
-    msg = msg.extract_plain_text().strip()
-    if msg:
-        for n in num:
-            msg = msg.replace(str(int(n)), '')
-    if msg:
-        state['text'] = msg
+async def _(state: T_State, msg: Message = CommandArg()):
+    msg_text = msg.extract_plain_text().strip()
+    args = msg_text.split(' ', 1)
+    if len(args) == 2 and args[1].isdigit():
+        num = int(args[1])
+    else:
+        num = None
+    if args[0]:
+        state['text'] = args[0]
     if num:
-        state['num'] = int(num[0]) if num[0] <= 10 else 10
+        state['num'] = min(num, 10)
     else:
         state['num'] = 1
 
 
 @couplets.got('text', prompt='请输入上联内容')
 async def couplets_handler(state: T_State):
     url = f'https://seq2seq-couplet-model.rssbrain.com/v0.2/couplet/{state["text"]}'
```

