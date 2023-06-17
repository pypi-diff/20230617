# Comparing `tmp/nonebot_plugin_moegoe-0.7.6.tar.gz` & `tmp/nonebot_plugin_moegoe-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_moegoe-0.7.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_moegoe-0.7.7.tar", max compression
```

## Comparing `nonebot_plugin_moegoe-0.7.6.tar` & `nonebot_plugin_moegoe-0.7.7.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-01-27 10:03:35.706603 nonebot_plugin_moegoe-0.7.6/LICENSE
--rw-r--r--   0        0        0     8085 2023-02-08 07:58:59.016069 nonebot_plugin_moegoe-0.7.6/README.md
--rw-r--r--   0        0        0     7650 2023-02-08 07:58:51.552198 nonebot_plugin_moegoe-0.7.6/nonebot_plugin_moegoe/__init__.py
--rw-r--r--   0        0        0     5626 2023-02-08 07:58:51.192204 nonebot_plugin_moegoe-0.7.6/nonebot_plugin_moegoe/profile.toml
--rw-r--r--   0        0        0      847 2023-02-08 07:58:51.472199 nonebot_plugin_moegoe-0.7.6/nonebot_plugin_moegoe/utils.py
--rw-r--r--   0        0        0      738 2023-02-08 07:58:58.864071 nonebot_plugin_moegoe-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     8865 1970-01-01 00:00:00.000000 nonebot_plugin_moegoe-0.7.6/setup.py
--rw-r--r--   0        0        0     8889 1970-01-01 00:00:00.000000 nonebot_plugin_moegoe-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-17 12:00:43.437461 nonebot_plugin_moegoe-0.7.7/LICENSE
+-rw-r--r--   0        0        0     6993 2023-06-17 12:00:43.437461 nonebot_plugin_moegoe-0.7.7/README.md
+-rw-r--r--   0        0        0     7688 2023-06-17 12:00:43.437461 nonebot_plugin_moegoe-0.7.7/nonebot_plugin_moegoe/__init__.py
+-rw-r--r--   0        0        0     3892 2023-06-17 12:00:43.437461 nonebot_plugin_moegoe-0.7.7/nonebot_plugin_moegoe/profile.toml
+-rw-r--r--   0        0        0      847 2023-06-17 12:00:43.437461 nonebot_plugin_moegoe-0.7.7/nonebot_plugin_moegoe/utils.py
+-rw-r--r--   0        0        0      738 2023-06-17 12:00:43.437461 nonebot_plugin_moegoe-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     7797 1970-01-01 00:00:00.000000 nonebot_plugin_moegoe-0.7.7/PKG-INFO
```

### Comparing `nonebot_plugin_moegoe-0.7.6/LICENSE` & `nonebot_plugin_moegoe-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_moegoe-0.7.6/README.md` & `nonebot_plugin_moegoe-0.7.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 <!--
  * @Author         : yiyuiii
  * @Date           : 2022-10-11 20:00:00
  * @LastEditors    : yiyuiii
- * @LastEditTime   : 2023-02-08 11:00:00
+ * @LastEditTime   : 2023-06-17 11:00:00
  * @Description    : None
  * @GitHub         : https://github.com/yiyuiii
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
-<div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-  <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
-</div>
+<p align="center">
+  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+</p>
 
 <div align="center">
 
 # nonebot-plugin-moegoe
 
 _✨ 日韩中 VITS 模型拟声 by fumiama✨_
 
@@ -40,15 +38,15 @@
 `nb plugin install nonebot_plugin_moegoe`
 或 `pip install nonebot_plugin_moegoe`
 
 ## :rocket: 使用方式
 
 **在聊天中输入:**
 
-- **让**[派蒙|空|荧|阿贝多|枫原万叶|温迪|八重神子|纳西妲|钟离|诺艾尔|凝光|托马|北斗|莫娜|荒泷一斗|提纳里|芭芭拉|艾尔海森|雷电将军|赛诺|琴|班尼特|五郎|神里绫华|迪希雅|夜兰|辛焱|安柏|宵宫|云堇|妮露|烟绯|鹿野院平藏|凯亚|达达利亚|迪卢克|可莉|早柚|香菱|重云|刻晴|久岐忍|珊瑚宫心海|迪奥娜|戴因斯雷布|魈|神里绫人|丽莎|优菈|凯瑟琳|雷泽|菲谢尔|九条裟罗|甘雨|行秋|胡桃|迪娜泽黛|柯莱|申鹤|砂糖|萍姥姥|奥兹|罗莎莉亚|式大将|哲平|坎蒂丝|托克|留云借风真君|昆钧|塞琉斯|多莉|大肉丸|莱依拉|散兵|拉赫曼|杜拉夫|阿守|玛乔丽|纳比尔|海芭夏|九条镰治|阿娜耶|阿晃|阿扎尔|七七|博士|白术|埃洛伊|大慈树王|女士|丽塔|失落迷迭|缭乱星棘|伊甸|伏特加女孩|狂热蓝调|莉莉娅|萝莎莉娅|八重樱|八重霞|卡莲|第六夜想曲|卡萝尔|姬子|极地战刃|布洛妮娅|次生银翼|理之律者|迷城骇兔|希儿|魇夜星渊|黑希儿|帕朵菲莉丝|天元骑英|幽兰黛尔|德丽莎|月下初拥|朔夜观星|暮光骑士|明日香|李素裳|格蕾修|梅比乌斯|渡鸦|人之律者|爱莉希雅|爱衣|天穹游侠|琪亚娜|空之律者|薪炎之律者|云墨丹心|符华|识之律者|维尔薇|芽衣|雷之律者|阿波尼亚]**说**(中文)
+- **让**[派蒙|凯亚|安柏|丽莎|琴|香菱|枫原万叶|迪卢克|温迪|可莉|早柚|托马|芭芭拉|优菈|云堇|钟离|魈|凝光|雷电将军|北斗|甘雨|七七|刻晴|神里绫华|戴因斯雷布|雷泽|神里绫人|罗莎莉亚|阿贝多|八重神子|宵宫|荒泷一斗|九条裟罗|夜兰|珊瑚宫心海|五郎|散兵|女士|达达利亚|莫娜|班尼特|申鹤|行秋|烟绯|久岐忍|辛焱|砂糖|胡桃|重云|菲谢尔|诺艾尔|迪奥娜|鹿野院平藏]**说**(中文)
 - **让**[宁宁|爱瑠|芳乃|茉子|丛雨|小春|七海|妃爱|华乃|亚澄|诗樱|天梨|里|广梦|莉莉子]**说日语：**(日语)
 - **让**[Sua|Mimiru|Arin|Yeonhwa|Yuhwa|Seonbae]**说韩语：**(韩语)
 
 例：
 
 - [让派蒙说你好！旅行者。](https://genshin.azurewebsites.net/api/speak?format=mp3&text=你好！旅行者。&id=0)
 - [让宁宁说日语：hello.](https://moegoe.azurewebsites.net/api/speak?text=hello!&id=0)
@@ -73,16 +71,14 @@
 - 插件优先级 priority
 - 触发正则语句 regex
 
 等等。 修改后保存，重启生效。
 
 **注意：**
 
-yuanshenai中文API暂时没有秘钥限制。
-
 因使用人数过多，genshin中文API设置了秘钥限制。在自行获取APIKey后，在配置文件的cnapi url末尾`"`前加上`&code=你的APIKey`，即可使用。参考[Issue 17](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/17#issuecomment-1336317427)
 
 日文和韩文的API目前正常。
 
 当插件版本更新时新配置将覆盖旧配置，如果不希望被覆盖可以在profile.toml中把版本调高。
 
 ## :speech_balloon: 常见问题
@@ -119,22 +115,26 @@
 [Issue 7](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/7) | [Issue 15](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/15)
 
 </details>
 
 
 ## :clipboard: 更新日志
 
-#### 2023.02.08 > v0.7.6 :fire:
+#### 2023.06.17 > v0.7.7 :fire:
+
+- 更新了cnapi的角色名单，并加入了一些api参数。
+
+#### 2023.02.08 > v0.7.6
 
-- 更新了新的中文api：yuanshenai.azurewebsites.net，目前免费使用。该api支持更多角色。
+- 更新了新的中文api：yuanshenai.azurewebsites.net **（目前已失效）**
 - 增加了更多api配置选项，如果url中存在对应空位则生效，目前可以在profile.toml中修改。
 - 更新profile.toml时自动将原有文件备份为profile.bak。
 - 加入在线更新profile的指令 moegoe load。
 
-#### 2023.01.27 > v0.7.5 ​
+#### 2023.01.27 > v0.7.5 
 
 - 增加了回复形式的设置，详见profile.toml中[api]一栏。
 
 #### 2022.12.25 > v0.7.4
 
 - 应官方要求升级包依赖版本。
```

#### html2text {}

```diff
@@ -1,31 +1,30 @@
 
-                             [NoneBotPluginLogo]
-                              [NoneBotPluginText]
+                                   [nonebot]
     # nonebot-plugin-moegoe _â¨ æ¥é©ä¸­ VITS æ¨¡åæå£° by fumiamaâ¨_
  æ¬è¿èªZeroBot-Pluginä»åºï¼https://github.com/FloatTech/ZeroBot-Plugin/
                            tree/master/plugin/moegoe
                            [license] [pypi] [python]
 ## :gear: å®è£æ¹æ³ `nb plugin install nonebot_plugin_moegoe` æ `pip
 install nonebot_plugin_moegoe` ## :rocket: ä½¿ç¨æ¹å¼ **å¨èå¤©ä¸­è¾å¥:**
 - **è®©**
-[æ´¾è|ç©º|è§|é¿è´å¤|æ«åä¸å¶|æ¸©è¿ª|å«éç¥å­|çº³è¥¿å¦²|éç¦»|è¯ºè¾å°|åå|æé©¬|åæ|è«å¨|èæ³·ä¸æ|æçº³é|è­è­æ|è¾å°æµ·æ£®|é·çµå°å|èµè¯º|ç´|ç­å°¼ç¹|äºé|ç¥éç»«å|è¿ªå¸é|å¤å°|è¾ç±|å®æ|å®µå®«|äºå |å¦®é²|çç»¯|é¹¿éé¢å¹³è|å¯äº|è¾¾è¾¾å©äº|è¿ªå¢å|å¯è|æ©æ|é¦è±|éäº|å»æ´|ä¹å²å¿|ççå®«å¿æµ·|è¿ªå¥¥å¨|æ´å æ¯é·å¸|é­|ç¥éç»«äºº|ä¸½è|ä¼è|å¯çç³|é·æ³½|è²è°¢å°|ä¹æ¡è£ç½|çé¨|è¡ç§|è¡æ¡|è¿ªå¨æ³½é»|æ¯è±|ç³é¹¤|ç ç³|èå§¥å§¥|å¥¥å¹|ç½èèäº|å¼å¤§å°|å²å¹³|åèä¸|æå|çäºåé£çå|æé§|å¡çæ¯|å¤è|å¤§èä¸¸|è±ä¾æ|æ£åµ|æèµ«æ¼|ææå¤«|é¿å®|çä¹ä¸½|çº³æ¯å°|æµ·è­å¤|ä¹æ¡é°æ²»|é¿å¨è¶|é¿æ|é¿æå°|ä¸ä¸|åå£«|ç½æ¯|åæ´ä¼|å¤§ææ ç|å¥³å£«|ä¸½å¡|å¤±è½è¿·è¿­|ç¼­ä¹±ææ£|ä¼ç¸|ä¼ç¹å å¥³å­©|çç­èè°|èèå¨|èèèå¨|å«éæ¨±|å«éé|å¡è²|ç¬¬å­å¤æ³æ²|å¡èå°|å§¬å­|æå°æå|å¸æ´å¦®å¨|æ¬¡çé¶ç¿¼|çä¹å¾è|è¿·åéªå|å¸å¿|é­å¤ææ¸|é»å¸å¿|å¸æµè²èä¸|å¤©åéªè±|å¹½å°é»å°|å¾·ä¸½è|æä¸åæ¥|æå¤è§æ|æ®åéªå£«|ææ¥é¦|æç´ è£³|æ ¼è¾ä¿®|æ¢æ¯ä¹æ¯|æ¸¡é¸¦|äººä¹å¾è|ç±èå¸é|ç±è¡£|å¤©ç©¹æ¸¸ä¾ |çªäºå¨|ç©ºä¹å¾è|èªçä¹å¾è|äºå¢¨ä¸¹å¿|ç¬¦å|è¯ä¹å¾è|ç»´å°è|è½è¡£|é·ä¹å¾è|é¿æ³¢å°¼äº]**è¯´**
+[æ´¾è|å¯äº|å®æ|ä¸½è|ç´|é¦è±|æ«åä¸å¶|è¿ªå¢å|æ¸©è¿ª|å¯è|æ©æ|æé©¬|è­è­æ|ä¼è|äºå |éç¦»|é­|åå|é·çµå°å|åæ|çé¨|ä¸ä¸|å»æ´|ç¥éç»«å|æ´å æ¯é·å¸|é·æ³½|ç¥éç»«äºº|ç½èèäº|é¿è´å¤|å«éç¥å­|å®µå®«|èæ³·ä¸æ|ä¹æ¡è£ç½|å¤å°|ççå®«å¿æµ·|äºé|æ£åµ|å¥³å£«|è¾¾è¾¾å©äº|è«å¨|ç­å°¼ç¹|ç³é¹¤|è¡ç§|çç»¯|ä¹å²å¿|è¾ç±|ç ç³|è¡æ¡|éäº|è²è°¢å°|è¯ºè¾å°|è¿ªå¥¥å¨|é¹¿éé¢å¹³è]**è¯´**
 (ä¸­æ) - **è®©**
 [å®å®|ç±ç |è³ä¹|èå­|ä¸é¨|å°æ¥|ä¸æµ·|å¦ç±|åä¹|äºæ¾|è¯æ¨±|å¤©æ¢¨|é|å¹¿æ¢¦|èèå­]**è¯´æ¥è¯­ï¼**
 (æ¥è¯­) - **è®©**[Sua|Mimiru|Arin|Yeonhwa|Yuhwa|Seonbae]**è¯´é©è¯­ï¼**
 (é©è¯­) ä¾ï¼ - [è®©æ´¾èè¯´ä½ å¥½ï¼æè¡èã](https://
 genshin.azurewebsites.net/api/speak?format=mp3&text=ä½ å¥½ï¼æè¡èã&id=0)
 - [è®©å®å®è¯´æ¥è¯­ï¼hello.](https://moegoe.azurewebsites.net/api/
 speak?text=hello!&id=0) - [è®©Suaè¯´é©è¯­ï¼hello.](https://
 moegoe.azurewebsites.net/api/speakkr?text=hello!&id=0) **Botè¿åè¯­é³**
 **å¨èå¤©ä¸­è¾å¥:** `moegoe load` å¯ä»¥å¨çº¿æ´æ°profileã ## :wrench:
 éç½®æ¹æ³ å¨æä»¶åæ¬¡èç½æåè¿è¡åï¼å¯ä»¥åç° BOTROOT/data/
 moegoe/ è·¯å¾ä¸æprofile.tomlæä»¶ï¼å¶ä¸­å¯ä»¥éç½® - æä»¶ä¼åçº§
 priority - è§¦åæ­£åè¯­å¥ regex ç­ç­ã ä¿®æ¹åä¿å­ï¼éå¯çæã
-**æ³¨æï¼** yuanshenaiä¸­æAPIææ¶æ²¡æç§é¥éå¶ã
+**æ³¨æï¼**
 å ä½¿ç¨äººæ°è¿å¤ï¼genshinä¸­æAPIè®¾ç½®äºç§é¥éå¶ãå¨èªè¡è·åAPIKeyåï¼å¨éç½®æä»¶çcnapi
 urlæ«å°¾`"`åå ä¸`&code=ä½ çAPIKey`ï¼å³å¯ä½¿ç¨ãåè[Issue 17]
 (https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/17#issuecomment-
 1336317427) æ¥æåé©æçAPIç®åæ­£å¸¸ã
 å½æä»¶çæ¬æ´æ°æ¶æ°éç½®å°è¦çæ§éç½®ï¼å¦æä¸å¸æè¢«è¦çå¯ä»¥å¨profile.tomlä¸­æçæ¬è°é«ã
 ## :speech_balloon: å¸¸è§é®é¢  æ¥é ERROR: No matching distribution found
 for nonebot-plugin-moegoe [Issue 1](https://github.com/Yiyuiii/nonebot-plugin-
@@ -41,21 +40,22 @@
 -
 ç¬¬ä¸ç§æåµï¼**æ¬æä»¶é»è®¤ä¼åçº§ä¸º5**ï¼è¥æå¶å®çæä»¶ä¼åçº§æ¯5å¼ºï¼ä¸è¯¥æä»¶æblockæªæ­ï¼åæ¬æä»¶å¯è½æ æ³æ¶å°å¹¶å¤çæ¶æ¯ãç®åéè¦èªè¡è°æ´æä»¶çä¼åçº§ã
 APIä¸è½çæè¾é¿è¯­é³
 ç®åAPIçæè¾é¿è¯­é³çéåº¦å¾æ¢ï¼ä»æ°åç§å°æ°åéï¼ï¼ä¸ºé¿åè¯¥ç±»è¯·æ±çå¹¶åé æèµæºé»å¡ï¼ä»£ç ä¸­éå¶äºè¯·æ±æ¶é¿ï¼å¯èªè¡ä¿®æ¹ã
 `resp = await client.get(url, timeout=120)`   APIæäº [Issue 7](https://
 github.com/Yiyuiii/nonebot-plugin-moegoe/issues/7) | [Issue 15](https://
 github.com/Yiyuiii/nonebot-plugin-moegoe/issues/15)  ## :clipboard:
-æ´æ°æ¥å¿ #### 2023.02.08 > v0.7.6 :fire: -
-æ´æ°äºæ°çä¸­æapiï¼yuanshenai.azurewebsites.netï¼ç®ååè´¹ä½¿ç¨ãè¯¥apiæ¯ææ´å¤è§è²ã
--
+æ´æ°æ¥å¿ #### 2023.06.17 > v0.7.7 :fire: -
+æ´æ°äºcnapiçè§è²ååï¼å¹¶å å¥äºä¸äºapiåæ°ã #### 2023.02.08
+> v0.7.6 - æ´æ°äºæ°çä¸­æapiï¼yuanshenai.azurewebsites.net
+**ï¼ç®åå·²å¤±æï¼** -
 å¢å äºæ´å¤apiéç½®éé¡¹ï¼å¦æurlä¸­å­å¨å¯¹åºç©ºä½åçæï¼ç®åå¯ä»¥å¨profile.tomlä¸­ä¿®æ¹ã
 - æ´æ°profile.tomlæ¶èªå¨å°åææä»¶å¤ä»½ä¸ºprofile.bakã -
-å å¥å¨çº¿æ´æ°profileçæä»¤ moegoe loadã #### 2023.01.27 > v0.7.5 â
-- å¢å äºåå¤å½¢å¼çè®¾ç½®ï¼è¯¦è§profile.tomlä¸­[api]ä¸æ ã ####
+å å¥å¨çº¿æ´æ°profileçæä»¤ moegoe loadã #### 2023.01.27 > v0.7.5 -
+å¢å äºåå¤å½¢å¼çè®¾ç½®ï¼è¯¦è§profile.tomlä¸­[api]ä¸æ ã ####
 2022.12.25 > v0.7.4 - åºå®æ¹è¦æ±åçº§åä¾èµçæ¬ã #### 2022.12.18 >
 v0.7.1 -
 ä¿®å¤å®è£å¤±è´¥çBUGãprofile.tomlçä½ç½®æ¹åï¼ä¹åçæ¬çéç½®å¯è½æ æ³èªå¨æ´æ°profile.tomléç½®æä»¶ã
 #### 2022.11.29 > v0.7.0 -
 ä»__init__.pyæ½ç¦»ä¸äºéç½®ç»æprofile.tomléç½®æä»¶ï¼ç°å¨å¯ä»¥èªå¨ä»githubä¸æåurlç­éç½®çæ´æ°äºã
 #### 2022.10.11 > v0.6.0 - åæ­¥æ´æ°ä¸­æåç¥è¯­é³api #### 2022.10.03 >
 v0.5.2 - å¢å åä¾èµçnonebotçæ¬éå¶ï¼ä»æ­¤èå·²ï¼ ####
```

### Comparing `nonebot_plugin_moegoe-0.7.6/nonebot_plugin_moegoe/__init__.py` & `nonebot_plugin_moegoe-0.7.7/nonebot_plugin_moegoe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,16 @@
         profileData = await download_url(profileDict['download']['profile_url'])
     if profileData is None:
         logger.warning(f"Error updating profile for moegoe.")
         return
 
     newProfileDict = tomllib.loads(profileData.decode('utf-8'))
     if versionGreater(newProfileDict['version'], profileDict['version']):
-        os.rename(profilePath, bakProfilePath)
+        if profilePath.exists():
+            os.rename(profilePath, bakProfilePath)
         write_file(profilePath, profileData)
         profileDict = newProfileDict
         profilePreprocess()
         logger.info(f"moegoe profile updated to version {profileDict['version']}.")
     else:
         logger.info("moegoe profile checked.")
```

### Comparing `nonebot_plugin_moegoe-0.7.6/nonebot_plugin_moegoe/utils.py` & `nonebot_plugin_moegoe-0.7.7/nonebot_plugin_moegoe/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_moegoe-0.7.6/pyproject.toml` & `nonebot_plugin_moegoe-0.7.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-moegoe"
-version = "0.7.6"
+version = "0.7.7"
 description = "日韩中 VITS 模型拟声"
 license = "MIT"
 authors = ["yiyuiii <yiyuiii@foxmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/yiyuiii/nonebot-plugin-moegoe"
 repository = "https://github.com/yiyuiii/nonebot-plugin-moegoe"
 documentation = "https://github.com/yiyuiii/nonebot-plugin-moegoe#readme"
```

### Comparing `nonebot_plugin_moegoe-0.7.6/setup.py` & `nonebot_plugin_moegoe-0.7.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,186 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-moegoe
+Version: 0.7.7
+Summary: 日韩中 VITS 模型拟声
+Home-page: https://github.com/yiyuiii/nonebot-plugin-moegoe
+License: MIT
+Keywords: nonebot,nonebot2,moegoe
+Author: yiyuiii
+Author-email: yiyuiii@foxmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.1.1,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0b5,<3.0.0)
+Requires-Dist: rtoml (>=0.9.0,<0.10.0)
+Project-URL: Documentation, https://github.com/yiyuiii/nonebot-plugin-moegoe#readme
+Project-URL: Repository, https://github.com/yiyuiii/nonebot-plugin-moegoe
+Description-Content-Type: text/markdown
 
-packages = \
-['nonebot_plugin_moegoe']
+<!--
+ * @Author         : yiyuiii
+ * @Date           : 2022-10-11 20:00:00
+ * @LastEditors    : yiyuiii
+ * @LastEditTime   : 2023-06-17 11:00:00
+ * @Description    : None
+ * @GitHub         : https://github.com/yiyuiii
+-->
 
-package_data = \
-{'': ['*']}
+<!-- markdownlint-disable MD033 MD036 MD041 -->
 
-install_requires = \
-['httpx>=0.23.0,<0.24.0',
- 'nonebot-adapter-onebot>=2.1.1,<3.0.0',
- 'nonebot2>=2.0.0b5,<3.0.0',
- 'rtoml>=0.9.0,<0.10.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-moegoe',
-    'version': '0.7.6',
-    'description': '日韩中 VITS 模型拟声',
-    'long_description': '<!--\n * @Author         : yiyuiii\n * @Date           : 2022-10-11 20:00:00\n * @LastEditors    : yiyuiii\n * @LastEditTime   : 2023-02-08 11:00:00\n * @Description    : None\n * @GitHub         : https://github.com/yiyuiii\n-->\n\n<!-- markdownlint-disable MD033 MD036 MD041 -->\n\n<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-moegoe\n\n_✨ 日韩中 VITS 模型拟声 by fumiama✨_\n\n搬运自ZeroBot-Plugin仓库：https://github.com/FloatTech/ZeroBot-Plugin/tree/master/plugin/moegoe\n\n</div>\n\n<p align="center">\n  <a href="https://raw.githubusercontent.com/Yiyuiii/nonebot-plugin-moegoe/master/LICENSE">\n    <img src="https://img.shields.io/github/license/Yiyuiii/nonebot-plugin-moegoe.svg" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/nonebot-plugin-moegoe">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-moegoe.svg" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n</p>\n\n## :gear: 安装方法\n\n`nb plugin install nonebot_plugin_moegoe`\n或 `pip install nonebot_plugin_moegoe`\n\n## :rocket: 使用方式\n\n**在聊天中输入:**\n\n- **让**[派蒙|空|荧|阿贝多|枫原万叶|温迪|八重神子|纳西妲|钟离|诺艾尔|凝光|托马|北斗|莫娜|荒泷一斗|提纳里|芭芭拉|艾尔海森|雷电将军|赛诺|琴|班尼特|五郎|神里绫华|迪希雅|夜兰|辛焱|安柏|宵宫|云堇|妮露|烟绯|鹿野院平藏|凯亚|达达利亚|迪卢克|可莉|早柚|香菱|重云|刻晴|久岐忍|珊瑚宫心海|迪奥娜|戴因斯雷布|魈|神里绫人|丽莎|优菈|凯瑟琳|雷泽|菲谢尔|九条裟罗|甘雨|行秋|胡桃|迪娜泽黛|柯莱|申鹤|砂糖|萍姥姥|奥兹|罗莎莉亚|式大将|哲平|坎蒂丝|托克|留云借风真君|昆钧|塞琉斯|多莉|大肉丸|莱依拉|散兵|拉赫曼|杜拉夫|阿守|玛乔丽|纳比尔|海芭夏|九条镰治|阿娜耶|阿晃|阿扎尔|七七|博士|白术|埃洛伊|大慈树王|女士|丽塔|失落迷迭|缭乱星棘|伊甸|伏特加女孩|狂热蓝调|莉莉娅|萝莎莉娅|八重樱|八重霞|卡莲|第六夜想曲|卡萝尔|姬子|极地战刃|布洛妮娅|次生银翼|理之律者|迷城骇兔|希儿|魇夜星渊|黑希儿|帕朵菲莉丝|天元骑英|幽兰黛尔|德丽莎|月下初拥|朔夜观星|暮光骑士|明日香|李素裳|格蕾修|梅比乌斯|渡鸦|人之律者|爱莉希雅|爱衣|天穹游侠|琪亚娜|空之律者|薪炎之律者|云墨丹心|符华|识之律者|维尔薇|芽衣|雷之律者|阿波尼亚]**说**(中文)\n- **让**[宁宁|爱瑠|芳乃|茉子|丛雨|小春|七海|妃爱|华乃|亚澄|诗樱|天梨|里|广梦|莉莉子]**说日语：**(日语)\n- **让**[Sua|Mimiru|Arin|Yeonhwa|Yuhwa|Seonbae]**说韩语：**(韩语)\n\n例：\n\n- [让派蒙说你好！旅行者。](https://genshin.azurewebsites.net/api/speak?format=mp3&text=你好！旅行者。&id=0)\n- [让宁宁说日语：hello.](https://moegoe.azurewebsites.net/api/speak?text=hello!&id=0)\n- [让Sua说韩语：hello.](https://moegoe.azurewebsites.net/api/speakkr?text=hello!&id=0)\n\n**Bot返回语音**\n\n<!-- <p align="center">\n  <audio src="https://yuanshenai.azurewebsites.net/api?speaker=派蒙&text=你好！旅行者。&format=mp3&length=1&noise=0.6&noisew=0.8"></audio>\n\n<audio src="https://moegoe.azurewebsites.net/api/speak?text=hello!&id=0"></audio>\n\n<audio src="https://moegoe.azurewebsites.net/api/speakkr?text=hello!&id=0"></audio>\n</p> -->\n\n**在聊天中输入:**  `moegoe load` 可以在线更新profile。\n\n## :wrench: 配置方法\n\n在插件初次联网成功运行后，可以发现 BOTROOT/data/moegoe/ 路径下有profile.toml文件，其中可以配置\n\n- 插件优先级 priority\n- 触发正则语句 regex\n\n等等。 修改后保存，重启生效。\n\n**注意：**\n\nyuanshenai中文API暂时没有秘钥限制。\n\n因使用人数过多，genshin中文API设置了秘钥限制。在自行获取APIKey后，在配置文件的cnapi url末尾`"`前加上`&code=你的APIKey`，即可使用。参考[Issue 17](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/17#issuecomment-1336317427)\n\n日文和韩文的API目前正常。\n\n当插件版本更新时新配置将覆盖旧配置，如果不希望被覆盖可以在profile.toml中把版本调高。\n\n## :speech_balloon: 常见问题\n\n<details>\n<summary>报错 ERROR: No matching distribution found for nonebot-plugin-moegoe</summary>\n\n[Issue 1](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/1)\n\n - 注意安装的包名是带**下划线**的：nonebot_plugin_moegoe\n</details>\n\n<details>\n<summary>API不能正确生成语音</summary>\n\n[Issue 2](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/2) | [Issue 4](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/4)\n\n- 第一种情况：**中文语音api对输入要求很严**，只支持中文字符和几个标点符号，输入如果包含api无法处理的字符就会无法生成语音，包括英文、叠词、奇怪标点符号等就大概率不行。\n- 第二种情况：当后台在报`encode silk failed: convert pcm file error: exec: "ffmpeg": executable file not found in %PATH% `错误时，表示go-cqhttp编码音频所依赖的ffmpeg包没有被安装，所以不能发送音频。**请自行安装ffmpeg**。*（不过ffmpeg可能不是必须的。如果有人在不安装ffmpeg时能正常使用，请向我反馈，这一点还没有经过测试。）*\n- 第三种情况：**本插件默认优先级为5**，若有其它的插件优先级比5强，且该插件有block截断，则本插件可能无法收到并处理消息。目前需要自行调整插件的优先级。\n</details>\n\n<details>\n<summary>API不能生成较长语音</summary>\n\n目前API生成较长语音的速度很慢（从数十秒到数分钟），为避免该类请求的并发造成资源阻塞，代码中限制了请求时长，可自行修改。\n\n`resp = await client.get(url, timeout=120)`\n</details>\n\n<details>\n<summary>API挂了</summary>\n\n[Issue 7](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/7) | [Issue 15](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/15)\n\n</details>\n\n\n## :clipboard: 更新日志\n\n#### 2023.02.08 > v0.7.6 :fire:\n\n- 更新了新的中文api：yuanshenai.azurewebsites.net，目前免费使用。该api支持更多角色。\n- 增加了更多api配置选项，如果url中存在对应空位则生效，目前可以在profile.toml中修改。\n- 更新profile.toml时自动将原有文件备份为profile.bak。\n- 加入在线更新profile的指令 moegoe load。\n\n#### 2023.01.27 > v0.7.5 \u200b\n\n- 增加了回复形式的设置，详见profile.toml中[api]一栏。\n\n#### 2022.12.25 > v0.7.4\n\n- 应官方要求升级包依赖版本。\n\n#### 2022.12.18 > v0.7.1\n- 修复安装失败的BUG。profile.toml的位置改变，之前版本的配置可能无法自动更新profile.toml配置文件。\n\n#### 2022.11.29 > v0.7.0\n- 从__init__.py抽离一些配置组成profile.toml配置文件，现在可以自动从github上抓取url等配置的更新了。\n\n#### 2022.10.11 > v0.6.0\n- 同步更新中文原神语音api\n\n#### 2022.10.03 > v0.5.2\n- 增加包依赖的nonebot版本限制（仅此而已）\n\n#### 2022.08.24 > v0.5.1\n- 在`让xx说xx：`正则式中添加冒号的全角半角匹配`(：|:)`（此外，之前版本已经添加形如`(日语|日文|日本语)`的正则匹配）\n\n#### 2022.08.24 > v0.5.0\n- 添加日语speaker2的API，增加8名可选语音人物\n- 换用httpx以修正requests阻塞多协程的BUG\n- 在中文语音中，将输入文字中的英文符号和0-9数字预处理为中文\n- 优化报错提示\n- 整理代码\n',
-    'author': 'yiyuiii',
-    'author_email': 'yiyuiii@foxmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/yiyuiii/nonebot-plugin-moegoe',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+<p align="center">
+  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+</p>
 
+<div align="center">
+
+# nonebot-plugin-moegoe
+
+_✨ 日韩中 VITS 模型拟声 by fumiama✨_
+
+搬运自ZeroBot-Plugin仓库：https://github.com/FloatTech/ZeroBot-Plugin/tree/master/plugin/moegoe
+
+</div>
+
+<p align="center">
+  <a href="https://raw.githubusercontent.com/Yiyuiii/nonebot-plugin-moegoe/master/LICENSE">
+    <img src="https://img.shields.io/github/license/Yiyuiii/nonebot-plugin-moegoe.svg" alt="license">
+  </a>
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-moegoe">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-moegoe.svg" alt="pypi">
+  </a>
+  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+</p>
+
+## :gear: 安装方法
+
+`nb plugin install nonebot_plugin_moegoe`
+或 `pip install nonebot_plugin_moegoe`
+
+## :rocket: 使用方式
+
+**在聊天中输入:**
+
+- **让**[派蒙|凯亚|安柏|丽莎|琴|香菱|枫原万叶|迪卢克|温迪|可莉|早柚|托马|芭芭拉|优菈|云堇|钟离|魈|凝光|雷电将军|北斗|甘雨|七七|刻晴|神里绫华|戴因斯雷布|雷泽|神里绫人|罗莎莉亚|阿贝多|八重神子|宵宫|荒泷一斗|九条裟罗|夜兰|珊瑚宫心海|五郎|散兵|女士|达达利亚|莫娜|班尼特|申鹤|行秋|烟绯|久岐忍|辛焱|砂糖|胡桃|重云|菲谢尔|诺艾尔|迪奥娜|鹿野院平藏]**说**(中文)
+- **让**[宁宁|爱瑠|芳乃|茉子|丛雨|小春|七海|妃爱|华乃|亚澄|诗樱|天梨|里|广梦|莉莉子]**说日语：**(日语)
+- **让**[Sua|Mimiru|Arin|Yeonhwa|Yuhwa|Seonbae]**说韩语：**(韩语)
+
+例：
+
+- [让派蒙说你好！旅行者。](https://genshin.azurewebsites.net/api/speak?format=mp3&text=你好！旅行者。&id=0)
+- [让宁宁说日语：hello.](https://moegoe.azurewebsites.net/api/speak?text=hello!&id=0)
+- [让Sua说韩语：hello.](https://moegoe.azurewebsites.net/api/speakkr?text=hello!&id=0)
+
+**Bot返回语音**
+
+<!-- <p align="center">
+  <audio src="https://yuanshenai.azurewebsites.net/api?speaker=派蒙&text=你好！旅行者。&format=mp3&length=1&noise=0.6&noisew=0.8"></audio>
+
+<audio src="https://moegoe.azurewebsites.net/api/speak?text=hello!&id=0"></audio>
+
+<audio src="https://moegoe.azurewebsites.net/api/speakkr?text=hello!&id=0"></audio>
+</p> -->
+
+**在聊天中输入:**  `moegoe load` 可以在线更新profile。
+
+## :wrench: 配置方法
+
+在插件初次联网成功运行后，可以发现 BOTROOT/data/moegoe/ 路径下有profile.toml文件，其中可以配置
+
+- 插件优先级 priority
+- 触发正则语句 regex
+
+等等。 修改后保存，重启生效。
+
+**注意：**
+
+因使用人数过多，genshin中文API设置了秘钥限制。在自行获取APIKey后，在配置文件的cnapi url末尾`"`前加上`&code=你的APIKey`，即可使用。参考[Issue 17](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/17#issuecomment-1336317427)
+
+日文和韩文的API目前正常。
+
+当插件版本更新时新配置将覆盖旧配置，如果不希望被覆盖可以在profile.toml中把版本调高。
+
+## :speech_balloon: 常见问题
+
+<details>
+<summary>报错 ERROR: No matching distribution found for nonebot-plugin-moegoe</summary>
+
+[Issue 1](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/1)
+
+ - 注意安装的包名是带**下划线**的：nonebot_plugin_moegoe
+</details>
+
+<details>
+<summary>API不能正确生成语音</summary>
+
+[Issue 2](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/2) | [Issue 4](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/4)
+
+- 第一种情况：**中文语音api对输入要求很严**，只支持中文字符和几个标点符号，输入如果包含api无法处理的字符就会无法生成语音，包括英文、叠词、奇怪标点符号等就大概率不行。
+- 第二种情况：当后台在报`encode silk failed: convert pcm file error: exec: "ffmpeg": executable file not found in %PATH% `错误时，表示go-cqhttp编码音频所依赖的ffmpeg包没有被安装，所以不能发送音频。**请自行安装ffmpeg**。*（不过ffmpeg可能不是必须的。如果有人在不安装ffmpeg时能正常使用，请向我反馈，这一点还没有经过测试。）*
+- 第三种情况：**本插件默认优先级为5**，若有其它的插件优先级比5强，且该插件有block截断，则本插件可能无法收到并处理消息。目前需要自行调整插件的优先级。
+</details>
+
+<details>
+<summary>API不能生成较长语音</summary>
+
+目前API生成较长语音的速度很慢（从数十秒到数分钟），为避免该类请求的并发造成资源阻塞，代码中限制了请求时长，可自行修改。
+
+`resp = await client.get(url, timeout=120)`
+</details>
+
+<details>
+<summary>API挂了</summary>
+
+[Issue 7](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/7) | [Issue 15](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/15)
+
+</details>
+
+
+## :clipboard: 更新日志
+
+#### 2023.06.17 > v0.7.7 :fire:
+
+- 更新了cnapi的角色名单，并加入了一些api参数。
+
+#### 2023.02.08 > v0.7.6
+
+- 更新了新的中文api：yuanshenai.azurewebsites.net **（目前已失效）**
+- 增加了更多api配置选项，如果url中存在对应空位则生效，目前可以在profile.toml中修改。
+- 更新profile.toml时自动将原有文件备份为profile.bak。
+- 加入在线更新profile的指令 moegoe load。
+
+#### 2023.01.27 > v0.7.5 
+
+- 增加了回复形式的设置，详见profile.toml中[api]一栏。
+
+#### 2022.12.25 > v0.7.4
+
+- 应官方要求升级包依赖版本。
+
+#### 2022.12.18 > v0.7.1
+- 修复安装失败的BUG。profile.toml的位置改变，之前版本的配置可能无法自动更新profile.toml配置文件。
+
+#### 2022.11.29 > v0.7.0
+- 从__init__.py抽离一些配置组成profile.toml配置文件，现在可以自动从github上抓取url等配置的更新了。
+
+#### 2022.10.11 > v0.6.0
+- 同步更新中文原神语音api
+
+#### 2022.10.03 > v0.5.2
+- 增加包依赖的nonebot版本限制（仅此而已）
+
+#### 2022.08.24 > v0.5.1
+- 在`让xx说xx：`正则式中添加冒号的全角半角匹配`(：|:)`（此外，之前版本已经添加形如`(日语|日文|日本语)`的正则匹配）
+
+#### 2022.08.24 > v0.5.0
+- 添加日语speaker2的API，增加8名可选语音人物
+- 换用httpx以修正requests阻塞多协程的BUG
+- 在中文语音中，将输入文字中的英文符号和0-9数字预处理为中文
+- 优化报错提示
+- 整理代码
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,78 +1,81 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_moegoe'] package_data = \ {'': ['*']} install_requires = \
-['httpx>=0.23.0,<0.24.0', 'nonebot-adapter-onebot>=2.1.1,<3.0.0',
-'nonebot2>=2.0.0b5,<3.0.0', 'rtoml>=0.9.0,<0.10.0'] setup_kwargs = { 'name':
-'nonebot-plugin-moegoe', 'version': '0.7.6', 'description': 'æ¥é©ä¸­ VITS
-æ¨¡åæå£°', 'long_description': '\n\n\n\n
-                           \n [NoneBotPluginLogo]\n
-                                      \n
-                              [NoneBotPluginText]
-                                      \n
-\n\n
-      \n\n# nonebot-plugin-moegoe\n\n_â¨ æ¥é©ä¸­ VITS æ¨¡åæå£° by
- fumiamaâ¨_\n\næ¬è¿èªZeroBot-Pluginä»åºï¼https://github.com/FloatTech/
-                 ZeroBot-Plugin/tree/master/plugin/moegoe\n\n
-\n\n
-                 \n \n_[license]\n\n \n_[pypi]\n\n [python]\n
-\n\n## :gear: å®è£æ¹æ³\n\n`nb plugin install nonebot_plugin_moegoe`\næ
-`pip install nonebot_plugin_moegoe`\n\n## :rocket:
-ä½¿ç¨æ¹å¼\n\n**å¨èå¤©ä¸­è¾å¥:**\n\n- **è®©**
-[æ´¾è|ç©º|è§|é¿è´å¤|æ«åä¸å¶|æ¸©è¿ª|å«éç¥å­|çº³è¥¿å¦²|éç¦»|è¯ºè¾å°|åå|æé©¬|åæ|è«å¨|èæ³·ä¸æ|æçº³é|è­è­æ|è¾å°æµ·æ£®|é·çµå°å|èµè¯º|ç´|ç­å°¼ç¹|äºé|ç¥éç»«å|è¿ªå¸é|å¤å°|è¾ç±|å®æ|å®µå®«|äºå |å¦®é²|çç»¯|é¹¿éé¢å¹³è|å¯äº|è¾¾è¾¾å©äº|è¿ªå¢å|å¯è|æ©æ|é¦è±|éäº|å»æ´|ä¹å²å¿|ççå®«å¿æµ·|è¿ªå¥¥å¨|æ´å æ¯é·å¸|é­|ç¥éç»«äºº|ä¸½è|ä¼è|å¯çç³|é·æ³½|è²è°¢å°|ä¹æ¡è£ç½|çé¨|è¡ç§|è¡æ¡|è¿ªå¨æ³½é»|æ¯è±|ç³é¹¤|ç ç³|èå§¥å§¥|å¥¥å¹|ç½èèäº|å¼å¤§å°|å²å¹³|åèä¸|æå|çäºåé£çå|æé§|å¡çæ¯|å¤è|å¤§èä¸¸|è±ä¾æ|æ£åµ|æèµ«æ¼|ææå¤«|é¿å®|çä¹ä¸½|çº³æ¯å°|æµ·è­å¤|ä¹æ¡é°æ²»|é¿å¨è¶|é¿æ|é¿æå°|ä¸ä¸|åå£«|ç½æ¯|åæ´ä¼|å¤§ææ ç|å¥³å£«|ä¸½å¡|å¤±è½è¿·è¿­|ç¼­ä¹±ææ£|ä¼ç¸|ä¼ç¹å å¥³å­©|çç­èè°|èèå¨|èèèå¨|å«éæ¨±|å«éé|å¡è²|ç¬¬å­å¤æ³æ²|å¡èå°|å§¬å­|æå°æå|å¸æ´å¦®å¨|æ¬¡çé¶ç¿¼|çä¹å¾è|è¿·åéªå|å¸å¿|é­å¤ææ¸|é»å¸å¿|å¸æµè²èä¸|å¤©åéªè±|å¹½å°é»å°|å¾·ä¸½è|æä¸åæ¥|æå¤è§æ|æ®åéªå£«|ææ¥é¦|æç´ è£³|æ ¼è¾ä¿®|æ¢æ¯ä¹æ¯|æ¸¡é¸¦|äººä¹å¾è|ç±èå¸é|ç±è¡£|å¤©ç©¹æ¸¸ä¾ |çªäºå¨|ç©ºä¹å¾è|èªçä¹å¾è|äºå¢¨ä¸¹å¿|ç¬¦å|è¯ä¹å¾è|ç»´å°è|è½è¡£|é·ä¹å¾è|é¿æ³¢å°¼äº]**è¯´**
-(ä¸­æ)\n- **è®©**
+Metadata-Version: 2.1 Name: nonebot-plugin-moegoe Version: 0.7.7 Summary:
+æ¥é©ä¸­ VITS æ¨¡åæå£° Home-page: https://github.com/yiyuiii/nonebot-
+plugin-moegoe License: MIT Keywords: nonebot,nonebot2,moegoe Author: yiyuiii
+Author-email: yiyuiii@foxmail.com Requires-Python: >=3.8,<4.0 Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Dist: httpx (>=0.23.0,<0.24.0) Requires-Dist: nonebot-adapter-onebot
+(>=2.1.1,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0b5,<3.0.0) Requires-Dist:
+rtoml (>=0.9.0,<0.10.0) Project-URL: Documentation, https://github.com/yiyuiii/
+nonebot-plugin-moegoe#readme Project-URL: Repository, https://github.com/
+yiyuiii/nonebot-plugin-moegoe Description-Content-Type: text/markdown
+                                   [nonebot]
+    # nonebot-plugin-moegoe _â¨ æ¥é©ä¸­ VITS æ¨¡åæå£° by fumiamaâ¨_
+ æ¬è¿èªZeroBot-Pluginä»åºï¼https://github.com/FloatTech/ZeroBot-Plugin/
+                           tree/master/plugin/moegoe
+                           [license] [pypi] [python]
+## :gear: å®è£æ¹æ³ `nb plugin install nonebot_plugin_moegoe` æ `pip
+install nonebot_plugin_moegoe` ## :rocket: ä½¿ç¨æ¹å¼ **å¨èå¤©ä¸­è¾å¥:**
+- **è®©**
+[æ´¾è|å¯äº|å®æ|ä¸½è|ç´|é¦è±|æ«åä¸å¶|è¿ªå¢å|æ¸©è¿ª|å¯è|æ©æ|æé©¬|è­è­æ|ä¼è|äºå |éç¦»|é­|åå|é·çµå°å|åæ|çé¨|ä¸ä¸|å»æ´|ç¥éç»«å|æ´å æ¯é·å¸|é·æ³½|ç¥éç»«äºº|ç½èèäº|é¿è´å¤|å«éç¥å­|å®µå®«|èæ³·ä¸æ|ä¹æ¡è£ç½|å¤å°|ççå®«å¿æµ·|äºé|æ£åµ|å¥³å£«|è¾¾è¾¾å©äº|è«å¨|ç­å°¼ç¹|ç³é¹¤|è¡ç§|çç»¯|ä¹å²å¿|è¾ç±|ç ç³|è¡æ¡|éäº|è²è°¢å°|è¯ºè¾å°|è¿ªå¥¥å¨|é¹¿éé¢å¹³è]**è¯´**
+(ä¸­æ) - **è®©**
 [å®å®|ç±ç |è³ä¹|èå­|ä¸é¨|å°æ¥|ä¸æµ·|å¦ç±|åä¹|äºæ¾|è¯æ¨±|å¤©æ¢¨|é|å¹¿æ¢¦|èèå­]**è¯´æ¥è¯­ï¼**
-(æ¥è¯­)\n- **è®©**[Sua|Mimiru|Arin|Yeonhwa|Yuhwa|Seonbae]**è¯´é©è¯­ï¼**
-(é©è¯­)\n\nä¾ï¼\n\n- [è®©æ´¾èè¯´ä½ å¥½ï¼æè¡èã](https://
-genshin.azurewebsites.net/api/
-speak?format=mp3&text=ä½ å¥½ï¼æè¡èã&id=0)\n-
-[è®©å®å®è¯´æ¥è¯­ï¼hello.](https://moegoe.azurewebsites.net/api/
-speak?text=hello!&id=0)\n- [è®©Suaè¯´é©è¯­ï¼hello.](https://
-moegoe.azurewebsites.net/api/
-speakkr?text=hello!&id=0)\n\n**Botè¿åè¯­é³**\n\n\n\n**å¨èå¤©ä¸­è¾å¥:**
-`moegoe load` å¯ä»¥å¨çº¿æ´æ°profileã\n\n## :wrench:
-éç½®æ¹æ³\n\nå¨æä»¶åæ¬¡èç½æåè¿è¡åï¼å¯ä»¥åç° BOTROOT/
-data/moegoe/ è·¯å¾ä¸æprofile.tomlæä»¶ï¼å¶ä¸­å¯ä»¥éç½®\n\n-
-æä»¶ä¼åçº§ priority\n- è§¦åæ­£åè¯­å¥ regex\n\nç­ç­ã
-ä¿®æ¹åä¿å­ï¼éå¯çæã\n\n**æ³¨æï¼**\n\nyuanshenaiä¸­æAPIææ¶æ²¡æç§é¥éå¶ã\n\nå ä½¿ç¨äººæ°è¿å¤ï¼genshinä¸­æAPIè®¾ç½®äºç§é¥éå¶ãå¨èªè¡è·åAPIKeyåï¼å¨éç½®æä»¶çcnapi
+(æ¥è¯­) - **è®©**[Sua|Mimiru|Arin|Yeonhwa|Yuhwa|Seonbae]**è¯´é©è¯­ï¼**
+(é©è¯­) ä¾ï¼ - [è®©æ´¾èè¯´ä½ å¥½ï¼æè¡èã](https://
+genshin.azurewebsites.net/api/speak?format=mp3&text=ä½ å¥½ï¼æè¡èã&id=0)
+- [è®©å®å®è¯´æ¥è¯­ï¼hello.](https://moegoe.azurewebsites.net/api/
+speak?text=hello!&id=0) - [è®©Suaè¯´é©è¯­ï¼hello.](https://
+moegoe.azurewebsites.net/api/speakkr?text=hello!&id=0) **Botè¿åè¯­é³**
+**å¨èå¤©ä¸­è¾å¥:** `moegoe load` å¯ä»¥å¨çº¿æ´æ°profileã ## :wrench:
+éç½®æ¹æ³ å¨æä»¶åæ¬¡èç½æåè¿è¡åï¼å¯ä»¥åç° BOTROOT/data/
+moegoe/ è·¯å¾ä¸æprofile.tomlæä»¶ï¼å¶ä¸­å¯ä»¥éç½® - æä»¶ä¼åçº§
+priority - è§¦åæ­£åè¯­å¥ regex ç­ç­ã ä¿®æ¹åä¿å­ï¼éå¯çæã
+**æ³¨æï¼**
+å ä½¿ç¨äººæ°è¿å¤ï¼genshinä¸­æAPIè®¾ç½®äºç§é¥éå¶ãå¨èªè¡è·åAPIKeyåï¼å¨éç½®æä»¶çcnapi
 urlæ«å°¾`"`åå ä¸`&code=ä½ çAPIKey`ï¼å³å¯ä½¿ç¨ãåè[Issue 17]
 (https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/17#issuecomment-
-1336317427)\n\næ¥æåé©æçAPIç®åæ­£å¸¸ã\n\nå½æä»¶çæ¬æ´æ°æ¶æ°éç½®å°è¦çæ§éç½®ï¼å¦æä¸å¸æè¢«è¦çå¯ä»¥å¨profile.tomlä¸­æçæ¬è°é«ã\n\n##
-:speech_balloon: å¸¸è§é®é¢\n\n\næ¥é ERROR: No matching distribution found
-for nonebot-plugin-moegoe\n\n[Issue 1](https://github.com/Yiyuiii/nonebot-
-plugin-moegoe/issues/1)\n\n -
-æ³¨æå®è£çååæ¯å¸¦**ä¸åçº¿**çï¼nonebot_plugin_moegoe\n\n\n\nAPIä¸è½æ­£ç¡®çæè¯­é³\n\n
-[Issue 2](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/2) | [Issue
-4](https://github.com/Yiyuiii/nonebot-plugin-moegoe/issues/4)\n\n-
-ç¬¬ä¸ç§æåµï¼**ä¸­æè¯­é³apiå¯¹è¾å¥è¦æ±å¾ä¸¥**ï¼åªæ¯æä¸­æå­ç¬¦åå ä¸ªæ ç¹ç¬¦å·ï¼è¾å¥å¦æåå«apiæ æ³å¤ççå­ç¬¦å°±ä¼æ æ³çæè¯­é³ï¼åæ¬è±æãå è¯ãå¥æªæ ç¹ç¬¦å·ç­å°±å¤§æ¦çä¸è¡ã\n-
-ç¬¬äºç§æåµï¼å½åå°å¨æ¥`encode silk failed: convert pcm file error:
+1336317427) æ¥æåé©æçAPIç®åæ­£å¸¸ã
+å½æä»¶çæ¬æ´æ°æ¶æ°éç½®å°è¦çæ§éç½®ï¼å¦æä¸å¸æè¢«è¦çå¯ä»¥å¨profile.tomlä¸­æçæ¬è°é«ã
+## :speech_balloon: å¸¸è§é®é¢  æ¥é ERROR: No matching distribution found
+for nonebot-plugin-moegoe [Issue 1](https://github.com/Yiyuiii/nonebot-plugin-
+moegoe/issues/1) -
+æ³¨æå®è£çååæ¯å¸¦**ä¸åçº¿**çï¼nonebot_plugin_moegoe
+APIä¸è½æ­£ç¡®çæè¯­é³ [Issue 2](https://github.com/Yiyuiii/nonebot-
+plugin-moegoe/issues/2) | [Issue 4](https://github.com/Yiyuiii/nonebot-plugin-
+moegoe/issues/4) -
+ç¬¬ä¸ç§æåµï¼**ä¸­æè¯­é³apiå¯¹è¾å¥è¦æ±å¾ä¸¥**ï¼åªæ¯æä¸­æå­ç¬¦åå ä¸ªæ ç¹ç¬¦å·ï¼è¾å¥å¦æåå«apiæ æ³å¤ççå­ç¬¦å°±ä¼æ æ³çæè¯­é³ï¼åæ¬è±æãå è¯ãå¥æªæ ç¹ç¬¦å·ç­å°±å¤§æ¦çä¸è¡ã
+- ç¬¬äºç§æåµï¼å½åå°å¨æ¥`encode silk failed: convert pcm file error:
 exec: "ffmpeg": executable file not found in %PATH% `éè¯¯æ¶ï¼è¡¨ç¤ºgo-
-cqhttpç¼ç é³é¢æä¾èµçffmpegåæ²¡æè¢«å®è£ï¼æä»¥ä¸è½åéé³é¢ã**è¯·èªè¡å®è£ffmpeg**ã*ï¼ä¸è¿ffmpegå¯è½ä¸æ¯å¿é¡»çãå¦ææäººå¨ä¸å®è£ffmpegæ¶è½æ­£å¸¸ä½¿ç¨ï¼è¯·åæåé¦ï¼è¿ä¸ç¹è¿æ²¡æç»è¿æµè¯ãï¼*\n-
-ç¬¬ä¸ç§æåµï¼**æ¬æä»¶é»è®¤ä¼åçº§ä¸º5**ï¼è¥æå¶å®çæä»¶ä¼åçº§æ¯5å¼ºï¼ä¸è¯¥æä»¶æblockæªæ­ï¼åæ¬æä»¶å¯è½æ æ³æ¶å°å¹¶å¤çæ¶æ¯ãç®åéè¦èªè¡è°æ´æä»¶çä¼åçº§ã\n\n\n\nAPIä¸è½çæè¾é¿è¯­é³\n\nç®åAPIçæè¾é¿è¯­é³çéåº¦å¾æ¢ï¼ä»æ°åç§å°æ°åéï¼ï¼ä¸ºé¿åè¯¥ç±»è¯·æ±çå¹¶åé æèµæºé»å¡ï¼ä»£ç ä¸­éå¶äºè¯·æ±æ¶é¿ï¼å¯èªè¡ä¿®æ¹ã\n\n`resp
-= await client.get(url, timeout=120)`\n\n\n\nAPIæäº\n\n[Issue 7](https://
+cqhttpç¼ç é³é¢æä¾èµçffmpegåæ²¡æè¢«å®è£ï¼æä»¥ä¸è½åéé³é¢ã**è¯·èªè¡å®è£ffmpeg**ã*ï¼ä¸è¿ffmpegå¯è½ä¸æ¯å¿é¡»çãå¦ææäººå¨ä¸å®è£ffmpegæ¶è½æ­£å¸¸ä½¿ç¨ï¼è¯·åæåé¦ï¼è¿ä¸ç¹è¿æ²¡æç»è¿æµè¯ãï¼*
+-
+ç¬¬ä¸ç§æåµï¼**æ¬æä»¶é»è®¤ä¼åçº§ä¸º5**ï¼è¥æå¶å®çæä»¶ä¼åçº§æ¯5å¼ºï¼ä¸è¯¥æä»¶æblockæªæ­ï¼åæ¬æä»¶å¯è½æ æ³æ¶å°å¹¶å¤çæ¶æ¯ãç®åéè¦èªè¡è°æ´æä»¶çä¼åçº§ã
+APIä¸è½çæè¾é¿è¯­é³
+ç®åAPIçæè¾é¿è¯­é³çéåº¦å¾æ¢ï¼ä»æ°åç§å°æ°åéï¼ï¼ä¸ºé¿åè¯¥ç±»è¯·æ±çå¹¶åé æèµæºé»å¡ï¼ä»£ç ä¸­éå¶äºè¯·æ±æ¶é¿ï¼å¯èªè¡ä¿®æ¹ã
+`resp = await client.get(url, timeout=120)`   APIæäº [Issue 7](https://
 github.com/Yiyuiii/nonebot-plugin-moegoe/issues/7) | [Issue 15](https://
-github.com/Yiyuiii/nonebot-plugin-moegoe/issues/15)\n\n\n\n\n## :clipboard:
-æ´æ°æ¥å¿\n\n#### 2023.02.08 > v0.7.6 :fire:\n\n-
-æ´æ°äºæ°çä¸­æapiï¼yuanshenai.azurewebsites.netï¼ç®ååè´¹ä½¿ç¨ãè¯¥apiæ¯ææ´å¤è§è²ã\n-
-å¢å äºæ´å¤apiéç½®éé¡¹ï¼å¦æurlä¸­å­å¨å¯¹åºç©ºä½åçæï¼ç®åå¯ä»¥å¨profile.tomlä¸­ä¿®æ¹ã\n-
-æ´æ°profile.tomlæ¶èªå¨å°åææä»¶å¤ä»½ä¸ºprofile.bakã\n-
-å å¥å¨çº¿æ´æ°profileçæä»¤ moegoe loadã\n\n#### 2023.01.27 > v0.7.5
-\u200b\n\n- å¢å äºåå¤å½¢å¼çè®¾ç½®ï¼è¯¦è§profile.tomlä¸­
-[api]ä¸æ ã\n\n#### 2022.12.25 > v0.7.4\n\n-
-åºå®æ¹è¦æ±åçº§åä¾èµçæ¬ã\n\n#### 2022.12.18 > v0.7.1\n-
-ä¿®å¤å®è£å¤±è´¥çBUGãprofile.tomlçä½ç½®æ¹åï¼ä¹åçæ¬çéç½®å¯è½æ æ³èªå¨æ´æ°profile.tomléç½®æä»¶ã\n\n####
-2022.11.29 > v0.7.0\n-
-ä»__init__.pyæ½ç¦»ä¸äºéç½®ç»æprofile.tomléç½®æä»¶ï¼ç°å¨å¯ä»¥èªå¨ä»githubä¸æåurlç­éç½®çæ´æ°äºã\n\n####
-2022.10.11 > v0.6.0\n- åæ­¥æ´æ°ä¸­æåç¥è¯­é³api\n\n#### 2022.10.03 >
-v0.5.2\n- å¢å åä¾èµçnonebotçæ¬éå¶ï¼ä»æ­¤èå·²ï¼\n\n####
-2022.08.24 > v0.5.1\n-
+github.com/Yiyuiii/nonebot-plugin-moegoe/issues/15)  ## :clipboard:
+æ´æ°æ¥å¿ #### 2023.06.17 > v0.7.7 :fire: -
+æ´æ°äºcnapiçè§è²ååï¼å¹¶å å¥äºä¸äºapiåæ°ã #### 2023.02.08
+> v0.7.6 - æ´æ°äºæ°çä¸­æapiï¼yuanshenai.azurewebsites.net
+**ï¼ç®åå·²å¤±æï¼** -
+å¢å äºæ´å¤apiéç½®éé¡¹ï¼å¦æurlä¸­å­å¨å¯¹åºç©ºä½åçæï¼ç®åå¯ä»¥å¨profile.tomlä¸­ä¿®æ¹ã
+- æ´æ°profile.tomlæ¶èªå¨å°åææä»¶å¤ä»½ä¸ºprofile.bakã -
+å å¥å¨çº¿æ´æ°profileçæä»¤ moegoe loadã #### 2023.01.27 > v0.7.5 -
+å¢å äºåå¤å½¢å¼çè®¾ç½®ï¼è¯¦è§profile.tomlä¸­[api]ä¸æ ã ####
+2022.12.25 > v0.7.4 - åºå®æ¹è¦æ±åçº§åä¾èµçæ¬ã #### 2022.12.18 >
+v0.7.1 -
+ä¿®å¤å®è£å¤±è´¥çBUGãprofile.tomlçä½ç½®æ¹åï¼ä¹åçæ¬çéç½®å¯è½æ æ³èªå¨æ´æ°profile.tomléç½®æä»¶ã
+#### 2022.11.29 > v0.7.0 -
+ä»__init__.pyæ½ç¦»ä¸äºéç½®ç»æprofile.tomléç½®æä»¶ï¼ç°å¨å¯ä»¥èªå¨ä»githubä¸æåurlç­éç½®çæ´æ°äºã
+#### 2022.10.11 > v0.6.0 - åæ­¥æ´æ°ä¸­æåç¥è¯­é³api #### 2022.10.03 >
+v0.5.2 - å¢å åä¾èµçnonebotçæ¬éå¶ï¼ä»æ­¤èå·²ï¼ ####
+2022.08.24 > v0.5.1 -
 å¨`è®©xxè¯´xxï¼`æ­£åå¼ä¸­æ·»å åå·çå¨è§åè§å¹é`(ï¼|:
 )`ï¼æ­¤å¤ï¼ä¹åçæ¬å·²ç»æ·»å å½¢å¦`
-(æ¥è¯­|æ¥æ|æ¥æ¬è¯­)`çæ­£åå¹éï¼\n\n#### 2022.08.24 > v0.5.0\n-
-æ·»å æ¥è¯­speaker2çAPIï¼å¢å 8åå¯éè¯­é³äººç©\n-
-æ¢ç¨httpxä»¥ä¿®æ­£requestsé»å¡å¤åç¨çBUG\n-
+(æ¥è¯­|æ¥æ|æ¥æ¬è¯­)`çæ­£åå¹éï¼ #### 2022.08.24 > v0.5.0 -
+æ·»å æ¥è¯­speaker2çAPIï¼å¢å 8åå¯éè¯­é³äººç© -
+æ¢ç¨httpxä»¥ä¿®æ­£requestsé»å¡å¤åç¨çBUG -
 å¨ä¸­æè¯­é³ä¸­ï¼å°è¾å¥æå­ä¸­çè±æç¬¦å·å0-
-9æ°å­é¢å¤çä¸ºä¸­æ\n- ä¼åæ¥éæç¤º\n- æ´çä»£ç \n', 'author':
-'yiyuiii', 'author_email': 'yiyuiii@foxmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/yiyuiii/nonebot-plugin-
-moegoe', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.8,<4.0', } setup
-(**setup_kwargs)
+9æ°å­é¢å¤çä¸ºä¸­æ - ä¼åæ¥éæç¤º - æ´çä»£ç 
```

