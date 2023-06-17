# Comparing `tmp/qetrader-1.0.8.tar.gz` & `tmp/qetrader-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qetrader-1.0.8.tar", last modified: Thu Mar  2 03:19:55 2023, max compression
+gzip compressed data, was "qetrader-1.0.9.tar", last modified: Thu Mar  2 12:54:03 2023, max compression
```

## Comparing `qetrader-1.0.8.tar` & `qetrader-1.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 03:19:55.879625 qetrader-1.0.8/
--rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qetrader-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       55 2023-02-02 05:32:01.000000 qetrader-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7303 2023-03-02 03:19:55.878625 qetrader-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5521 2023-02-06 13:57:06.000000 qetrader-1.0.8/README.md
--rw-rw-rw-   0        0        0      983 2023-03-02 03:15:47.000000 qetrader-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-02 03:19:55.879625 qetrader-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-02 03:19:55.830626 qetrader-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-03-02 03:19:55.864626 qetrader-1.0.8/src/qetrader/
--rw-rw-rw-   0        0        0     1912 2023-03-02 03:15:28.000000 qetrader-1.0.8/src/qetrader/__init__.py
--rw-rw-rw-   0        0        0    11188 2022-09-12 03:17:41.000000 qetrader-1.0.8/src/qetrader/qeaccount.py
--rw-rw-rw-   0        0        0    29534 2022-07-28 14:12:29.000000 qetrader-1.0.8/src/qetrader/qearbit.py
--rw-rw-rw-   0        0        0     6404 2022-10-20 10:53:54.000000 qetrader-1.0.8/src/qetrader/qeasyncdata.py
--rw-rw-rw-   0        0        0    26564 2023-02-06 14:43:41.000000 qetrader-1.0.8/src/qetrader/qeasyncstrat.py
--rw-rw-rw-   0        0        0   127445 2023-02-02 15:35:52.000000 qetrader-1.0.8/src/qetrader/qebacktestmul.py
--rw-rw-rw-   0        0        0    42779 2023-02-01 05:50:37.000000 qetrader-1.0.8/src/qetrader/qecontext.py
--rw-rw-rw-   0        0        0     1321 2023-01-31 07:13:39.000000 qetrader-1.0.8/src/qetrader/qectpconst_wrap.py
--rw-rw-rw-   0        0        0    23778 2023-02-01 13:19:48.000000 qetrader-1.0.8/src/qetrader/qectpmarket_wrap.py
--rw-rw-rw-   0        0        0   105089 2023-03-02 03:00:28.000000 qetrader-1.0.8/src/qetrader/qectptrader_wrap.py
--rw-rw-rw-   0        0        0     6706 2023-03-01 15:09:13.000000 qetrader-1.0.8/src/qetrader/qeglobal.py
--rw-rw-rw-   0        0        0    53987 2023-02-20 11:05:55.000000 qetrader-1.0.8/src/qetrader/qeinterface.py
--rw-rw-rw-   0        0        0     5065 2023-02-02 14:07:02.000000 qetrader-1.0.8/src/qetrader/qelogger.py
--rw-rw-rw-   0        0        0    36503 2023-02-06 14:10:35.000000 qetrader-1.0.8/src/qetrader/qemain.py
--rw-rw-rw-   0        0        0     1844 2023-02-02 15:02:07.000000 qetrader-1.0.8/src/qetrader/qemonitor_log_web.py
--rw-rw-rw-   0        0        0     1752 2022-07-28 14:13:58.000000 qetrader-1.0.8/src/qetrader/qeoption.py
--rw-rw-rw-   0        0        0     2918 2023-02-06 12:10:07.000000 qetrader-1.0.8/src/qetrader/qeplugins.py
--rw-rw-rw-   0        0        0    35715 2023-02-02 12:21:37.000000 qetrader-1.0.8/src/qetrader/qeredisdb.py
--rw-rw-rw-   0        0        0     7719 2022-07-28 14:14:11.000000 qetrader-1.0.8/src/qetrader/qeriskctl.py
--rw-rw-rw-   0        0        0    55446 2023-02-01 05:55:03.000000 qetrader-1.0.8/src/qetrader/qesimtrader.py
--rw-rw-rw-   0        0        0    12252 2022-07-28 14:14:40.000000 qetrader-1.0.8/src/qetrader/qestatistics.py
--rw-rw-rw-   0        0        0     4261 2023-02-02 11:34:52.000000 qetrader-1.0.8/src/qetrader/qestratmarket_wrap.py
--rw-rw-rw-   0        0        0    26945 2023-03-01 16:48:30.000000 qetrader-1.0.8/src/qetrader/qestratprocess.py
--rw-rw-rw-   0        0        0     1642 2023-02-03 02:36:40.000000 qetrader-1.0.8/src/qetrader/qesysconf.py
--rw-rw-rw-   0        0        0     1094 2022-07-28 14:15:00.000000 qetrader-1.0.8/src/qetrader/qetype.py
--rw-rw-rw-   0        0        0     4256 2023-02-01 02:23:41.000000 qetrader-1.0.8/src/qetrader/qeudpclient.py
--rw-rw-rw-   0        0        0    49778 2023-02-06 04:11:17.000000 qetrader-1.0.8/src/qetrader/qeweb.py
-drwxrwxrwx   0        0        0        0 2023-03-02 03:19:55.872626 qetrader-1.0.8/src/qetrader/static/
--rw-rw-rw-   0        0        0   583536 2022-05-13 15:56:55.000000 qetrader-1.0.8/src/qetrader/static/canvas.js
--rw-rw-rw-   0        0        0     7284 2022-05-09 10:12:32.000000 qetrader-1.0.8/src/qetrader/static/jquery.pagination.js
--rw-rw-rw-   0        0        0     3342 2022-05-12 07:11:40.000000 qetrader-1.0.8/src/qetrader/static/jquery.timers.js
--rw-rw-rw-   0        0        0     2604 2022-02-25 07:14:44.000000 qetrader-1.0.8/src/qetrader/static/theme.css
--rw-rw-rw-   0        0        0      110 2023-02-01 11:46:22.000000 qetrader-1.0.8/src/qetrader/sysconfig.json
-drwxrwxrwx   0        0        0        0 2023-03-02 03:19:55.877626 qetrader-1.0.8/src/qetrader/templates/
--rw-rw-rw-   0        0        0    21926 2022-11-01 13:36:55.000000 qetrader-1.0.8/src/qetrader/templates/backtest.html
--rw-rw-rw-   0        0        0     3042 2022-03-23 12:37:06.000000 qetrader-1.0.8/src/qetrader/templates/base.html
--rw-rw-rw-   0        0        0     4074 2022-07-23 10:41:02.000000 qetrader-1.0.8/src/qetrader/templates/fundhome.html
--rw-rw-rw-   0        0        0    44342 2022-05-12 10:53:16.000000 qetrader-1.0.8/src/qetrader/templates/image_all.html
--rw-rw-rw-   0        0        0    32333 2022-06-23 07:29:42.000000 qetrader-1.0.8/src/qetrader/templates/image_ex.html
-drwxrwxrwx   0        0        0        0 2023-03-02 03:19:55.868626 qetrader-1.0.8/src/qetrader.egg-info/
--rw-rw-rw-   0        0        0     7303 2023-03-02 03:19:55.000000 qetrader-1.0.8/src/qetrader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1317 2023-03-02 03:19:55.000000 qetrader-1.0.8/src/qetrader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 03:19:55.000000 qetrader-1.0.8/src/qetrader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      249 2023-03-02 03:19:55.000000 qetrader-1.0.8/src/qetrader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-02 03:19:55.000000 qetrader-1.0.8/src/qetrader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-02 12:54:03.090371 qetrader-1.0.9/
+-rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qetrader-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-02-02 05:32:01.000000 qetrader-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     8741 2023-03-02 12:54:03.089375 qetrader-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6959 2023-03-02 05:39:02.000000 qetrader-1.0.9/README.md
+-rw-rw-rw-   0        0        0      983 2023-03-02 12:50:59.000000 qetrader-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-03-02 12:54:03.090371 qetrader-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-03-02 12:54:03.038401 qetrader-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-03-02 12:54:03.072371 qetrader-1.0.9/src/qetrader/
+-rw-rw-rw-   0        0        0     1912 2023-03-02 12:51:10.000000 qetrader-1.0.9/src/qetrader/__init__.py
+-rw-rw-rw-   0        0        0    11188 2022-09-12 03:17:41.000000 qetrader-1.0.9/src/qetrader/qeaccount.py
+-rw-rw-rw-   0        0        0    29534 2022-07-28 14:12:29.000000 qetrader-1.0.9/src/qetrader/qearbit.py
+-rw-rw-rw-   0        0        0     6404 2022-10-20 10:53:54.000000 qetrader-1.0.9/src/qetrader/qeasyncdata.py
+-rw-rw-rw-   0        0        0    26564 2023-02-06 14:43:41.000000 qetrader-1.0.9/src/qetrader/qeasyncstrat.py
+-rw-rw-rw-   0        0        0   127445 2023-02-02 15:35:52.000000 qetrader-1.0.9/src/qetrader/qebacktestmul.py
+-rw-rw-rw-   0        0        0    42779 2023-02-01 05:50:37.000000 qetrader-1.0.9/src/qetrader/qecontext.py
+-rw-rw-rw-   0        0        0     1321 2023-01-31 07:13:39.000000 qetrader-1.0.9/src/qetrader/qectpconst_wrap.py
+-rw-rw-rw-   0        0        0    23778 2023-02-01 13:19:48.000000 qetrader-1.0.9/src/qetrader/qectpmarket_wrap.py
+-rw-rw-rw-   0        0        0   105089 2023-03-02 03:00:28.000000 qetrader-1.0.9/src/qetrader/qectptrader_wrap.py
+-rw-rw-rw-   0        0        0     6706 2023-03-01 15:09:13.000000 qetrader-1.0.9/src/qetrader/qeglobal.py
+-rw-rw-rw-   0        0        0    53987 2023-02-20 11:05:55.000000 qetrader-1.0.9/src/qetrader/qeinterface.py
+-rw-rw-rw-   0        0        0     5065 2023-02-02 14:07:02.000000 qetrader-1.0.9/src/qetrader/qelogger.py
+-rw-rw-rw-   0        0        0    36503 2023-02-06 14:10:35.000000 qetrader-1.0.9/src/qetrader/qemain.py
+-rw-rw-rw-   0        0        0     1844 2023-02-02 15:02:07.000000 qetrader-1.0.9/src/qetrader/qemonitor_log_web.py
+-rw-rw-rw-   0        0        0     1752 2022-07-28 14:13:58.000000 qetrader-1.0.9/src/qetrader/qeoption.py
+-rw-rw-rw-   0        0        0     2918 2023-02-06 12:10:07.000000 qetrader-1.0.9/src/qetrader/qeplugins.py
+-rw-rw-rw-   0        0        0    35715 2023-02-02 12:21:37.000000 qetrader-1.0.9/src/qetrader/qeredisdb.py
+-rw-rw-rw-   0        0        0     7719 2022-07-28 14:14:11.000000 qetrader-1.0.9/src/qetrader/qeriskctl.py
+-rw-rw-rw-   0        0        0    55446 2023-02-01 05:55:03.000000 qetrader-1.0.9/src/qetrader/qesimtrader.py
+-rw-rw-rw-   0        0        0    12252 2022-07-28 14:14:40.000000 qetrader-1.0.9/src/qetrader/qestatistics.py
+-rw-rw-rw-   0        0        0     4261 2023-02-02 11:34:52.000000 qetrader-1.0.9/src/qetrader/qestratmarket_wrap.py
+-rw-rw-rw-   0        0        0    26946 2023-03-02 06:52:01.000000 qetrader-1.0.9/src/qetrader/qestratprocess.py
+-rw-rw-rw-   0        0        0     1642 2023-02-03 02:36:40.000000 qetrader-1.0.9/src/qetrader/qesysconf.py
+-rw-rw-rw-   0        0        0     1094 2022-07-28 14:15:00.000000 qetrader-1.0.9/src/qetrader/qetype.py
+-rw-rw-rw-   0        0        0     4256 2023-02-01 02:23:41.000000 qetrader-1.0.9/src/qetrader/qeudpclient.py
+-rw-rw-rw-   0        0        0    49778 2023-02-06 04:11:17.000000 qetrader-1.0.9/src/qetrader/qeweb.py
+drwxrwxrwx   0        0        0        0 2023-03-02 12:54:03.082371 qetrader-1.0.9/src/qetrader/static/
+-rw-rw-rw-   0        0        0   583536 2022-05-13 15:56:55.000000 qetrader-1.0.9/src/qetrader/static/canvas.js
+-rw-rw-rw-   0        0        0     7284 2022-05-09 10:12:32.000000 qetrader-1.0.9/src/qetrader/static/jquery.pagination.js
+-rw-rw-rw-   0        0        0     3342 2022-05-12 07:11:40.000000 qetrader-1.0.9/src/qetrader/static/jquery.timers.js
+-rw-rw-rw-   0        0        0     2604 2022-02-25 07:14:44.000000 qetrader-1.0.9/src/qetrader/static/theme.css
+-rw-rw-rw-   0        0        0      110 2023-02-01 11:46:22.000000 qetrader-1.0.9/src/qetrader/sysconfig.json
+drwxrwxrwx   0        0        0        0 2023-03-02 12:54:03.087373 qetrader-1.0.9/src/qetrader/templates/
+-rw-rw-rw-   0        0        0    21926 2022-11-01 13:36:55.000000 qetrader-1.0.9/src/qetrader/templates/backtest.html
+-rw-rw-rw-   0        0        0     3042 2022-03-23 12:37:06.000000 qetrader-1.0.9/src/qetrader/templates/base.html
+-rw-rw-rw-   0        0        0     4074 2022-07-23 10:41:02.000000 qetrader-1.0.9/src/qetrader/templates/fundhome.html
+-rw-rw-rw-   0        0        0    44342 2022-05-12 10:53:16.000000 qetrader-1.0.9/src/qetrader/templates/image_all.html
+-rw-rw-rw-   0        0        0    32333 2022-06-23 07:29:42.000000 qetrader-1.0.9/src/qetrader/templates/image_ex.html
+drwxrwxrwx   0        0        0        0 2023-03-02 12:54:03.077372 qetrader-1.0.9/src/qetrader.egg-info/
+-rw-rw-rw-   0        0        0     8741 2023-03-02 12:54:03.000000 qetrader-1.0.9/src/qetrader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1317 2023-03-02 12:54:03.000000 qetrader-1.0.9/src/qetrader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-02 12:54:03.000000 qetrader-1.0.9/src/qetrader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      249 2023-03-02 12:54:03.000000 qetrader-1.0.9/src/qetrader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-03-02 12:54:03.000000 qetrader-1.0.9/src/qetrader.egg-info/top_level.txt
```

### Comparing `qetrader-1.0.8/LICENSE` & `qetrader-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/PKG-INFO` & `qetrader-1.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qetrader
-Version: 1.0.8
+Version: 1.0.9
 Summary: Quantease Trader SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -259,7 +259,60 @@
 
 ## 如何编写策略
 
 ​	请参照[官方文档](https://quantease.cn/newdoc)文档说明
 
 
 
+## 插件使用说明
+
+
+
+### 安装
+
+以“algoex“插件为例，下载插件代码如下：
+
+```python
+from qesdk import auth
+auth('your username','your authcode')
+from qetrader.qeplugins import installPlugin
+installPlugin('algoex')
+```
+
+运行代码后，出现如下提示代表安装成功：
+
+```
+插件algoex下载成功
+在策略文件中按如下格式import该插件:
+from qetrader.plugins.qealgoex import plugin_algoex
+```
+
+> 注;下载插件需要成为VIP付费客户，否则会下载失败。注册VIP请联系客户
+
+### 引用插件
+
+以'algoex'为例，根据按照的说明，在code中使用：
+
+```python
+from qesdk import auth
+##授权码
+auth('your username','your authcode')
+from qetrader import listSimuAccounts, createSimuAccount,runStrat
+from qetrader.plugins.qealgoex import plugin_algoex 
+
+##实盘账户信息
+user_setting = {'investorid':'xxxxxx', 'password':'xxxxxxxx','broker':'xxxxxx'}
+
+if __name__=='__main__':
+    ##换成自己的用户名
+    user='myname'
+    ##如果有模拟账户，用第一个账户，没有新建一个
+    tokenlist = listSimuAccounts(user)
+    if len(tokenlist) > 0:
+        token = tokenlist[0]
+    else:
+        token = createSimuAccount(user)
+    ##运行策略，algoex插件本身就是个策略实例，可以直接使用
+    runStrat(user,'real',[plugin_algoex], simu_token=token,real_account=user_setting)
+
+```
+
```

### Comparing `qetrader-1.0.8/README.md` & `qetrader-1.0.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -223,7 +223,60 @@
 
 ## 如何编写策略
 
 ​	请参照[官方文档](https://quantease.cn/newdoc)文档说明
 
 
 
+## 插件使用说明
+
+
+
+### 安装
+
+以“algoex“插件为例，下载插件代码如下：
+
+```python
+from qesdk import auth
+auth('your username','your authcode')
+from qetrader.qeplugins import installPlugin
+installPlugin('algoex')
+```
+
+运行代码后，出现如下提示代表安装成功：
+
+```
+插件algoex下载成功
+在策略文件中按如下格式import该插件:
+from qetrader.plugins.qealgoex import plugin_algoex
+```
+
+> 注;下载插件需要成为VIP付费客户，否则会下载失败。注册VIP请联系客户
+
+### 引用插件
+
+以'algoex'为例，根据按照的说明，在code中使用：
+
+```python
+from qesdk import auth
+##授权码
+auth('your username','your authcode')
+from qetrader import listSimuAccounts, createSimuAccount,runStrat
+from qetrader.plugins.qealgoex import plugin_algoex 
+
+##实盘账户信息
+user_setting = {'investorid':'xxxxxx', 'password':'xxxxxxxx','broker':'xxxxxx'}
+
+if __name__=='__main__':
+    ##换成自己的用户名
+    user='myname'
+    ##如果有模拟账户，用第一个账户，没有新建一个
+    tokenlist = listSimuAccounts(user)
+    if len(tokenlist) > 0:
+        token = tokenlist[0]
+    else:
+        token = createSimuAccount(user)
+    ##运行策略，algoex插件本身就是个策略实例，可以直接使用
+    runStrat(user,'real',[plugin_algoex], simu_token=token,real_account=user_setting)
+
+```
+
```

### Comparing `qetrader-1.0.8/pyproject.toml` & `qetrader-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qetrader"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Scott Zhang", email="scott2011@qq.com" },
 ]
 description = "Quantease Trader SDK for quants"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `qetrader-1.0.8/src/qetrader/__init__.py` & `qetrader-1.0.9/src/qetrader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Created on Tue Nov 30 20:01:48 2021
 
 @author: ScottStation
 """
 
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 
 from .qeinterface import qeStratBase
 from .qeinterface import make_order
 from .qeinterface import cancel_order
 from .qeinterface import get_bar
 #from .qecsvorder import algo_trade
 from .qemain import runStrat
```

### Comparing `qetrader-1.0.8/src/qetrader/qeaccount.py` & `qetrader-1.0.9/src/qetrader/qeaccount.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qearbit.py` & `qetrader-1.0.9/src/qetrader/qearbit.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qeasyncdata.py` & `qetrader-1.0.9/src/qetrader/qeasyncdata.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qeasyncstrat.py` & `qetrader-1.0.9/src/qetrader/qeasyncstrat.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qebacktestmul.py` & `qetrader-1.0.9/src/qetrader/qebacktestmul.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qecontext.py` & `qetrader-1.0.9/src/qetrader/qecontext.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qectpconst_wrap.py` & `qetrader-1.0.9/src/qetrader/qectpconst_wrap.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qectpmarket_wrap.py` & `qetrader-1.0.9/src/qetrader/qectpmarket_wrap.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qectptrader_wrap.py` & `qetrader-1.0.9/src/qetrader/qectptrader_wrap.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qeglobal.py` & `qetrader-1.0.9/src/qetrader/qeglobal.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qeinterface.py` & `qetrader-1.0.9/src/qetrader/qeinterface.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qelogger.py` & `qetrader-1.0.9/src/qetrader/qelogger.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qemain.py` & `qetrader-1.0.9/src/qetrader/qemain.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qemonitor_log_web.py` & `qetrader-1.0.9/src/qetrader/qemonitor_log_web.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qeoption.py` & `qetrader-1.0.9/src/qetrader/qeoption.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qeplugins.py` & `qetrader-1.0.9/src/qetrader/qeplugins.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qeredisdb.py` & `qetrader-1.0.9/src/qetrader/qeredisdb.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qeriskctl.py` & `qetrader-1.0.9/src/qetrader/qeriskctl.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qesimtrader.py` & `qetrader-1.0.9/src/qetrader/qesimtrader.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qestatistics.py` & `qetrader-1.0.9/src/qetrader/qestatistics.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qestratmarket_wrap.py` & `qetrader-1.0.9/src/qetrader/qestratmarket_wrap.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qestratprocess.py` & `qetrader-1.0.9/src/qetrader/qestratprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
             writeStratPosition_wrap(self.name, lastday,context.position,context.instClosePnl)
             writeContractTable_wrap(self.name, lastday,context.position)
             writeStratStat_wrap(self.name,lastday, context.prodMaxMarg, context.prodTurnover)
            
     def handleOrder(self,order,context):  
         try:     
             corder = context.orders.get(order['orderid'],None)
-            print('stratprocess 1',corder)
+            #print('stratprocess 1',corder)
             if corder:
                 #time = str(order['timedigit'])
                 corder['status'] = order['status']
                 corder['tradevol'] = order['tradevol']
                 corder['cancelvol'] = order['cancelvol']
                 corder['leftvol'] = order['leftvol']
                 corder['stratName'] = self.name
```

### Comparing `qetrader-1.0.8/src/qetrader/qesysconf.py` & `qetrader-1.0.9/src/qetrader/qesysconf.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qetype.py` & `qetrader-1.0.9/src/qetrader/qetype.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qeudpclient.py` & `qetrader-1.0.9/src/qetrader/qeudpclient.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/qeweb.py` & `qetrader-1.0.9/src/qetrader/qeweb.py`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/static/canvas.js` & `qetrader-1.0.9/src/qetrader/static/canvas.js`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/static/jquery.pagination.js` & `qetrader-1.0.9/src/qetrader/static/jquery.pagination.js`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/static/jquery.timers.js` & `qetrader-1.0.9/src/qetrader/static/jquery.timers.js`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/static/theme.css` & `qetrader-1.0.9/src/qetrader/static/theme.css`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/templates/backtest.html` & `qetrader-1.0.9/src/qetrader/templates/backtest.html`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/templates/base.html` & `qetrader-1.0.9/src/qetrader/templates/base.html`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/templates/fundhome.html` & `qetrader-1.0.9/src/qetrader/templates/fundhome.html`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/templates/image_all.html` & `qetrader-1.0.9/src/qetrader/templates/image_all.html`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader/templates/image_ex.html` & `qetrader-1.0.9/src/qetrader/templates/image_ex.html`

 * *Files identical despite different names*

### Comparing `qetrader-1.0.8/src/qetrader.egg-info/PKG-INFO` & `qetrader-1.0.9/src/qetrader.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qetrader
-Version: 1.0.8
+Version: 1.0.9
 Summary: Quantease Trader SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -259,7 +259,60 @@
 
 ## 如何编写策略
 
 ​	请参照[官方文档](https://quantease.cn/newdoc)文档说明
 
 
 
+## 插件使用说明
+
+
+
+### 安装
+
+以“algoex“插件为例，下载插件代码如下：
+
+```python
+from qesdk import auth
+auth('your username','your authcode')
+from qetrader.qeplugins import installPlugin
+installPlugin('algoex')
+```
+
+运行代码后，出现如下提示代表安装成功：
+
+```
+插件algoex下载成功
+在策略文件中按如下格式import该插件:
+from qetrader.plugins.qealgoex import plugin_algoex
+```
+
+> 注;下载插件需要成为VIP付费客户，否则会下载失败。注册VIP请联系客户
+
+### 引用插件
+
+以'algoex'为例，根据按照的说明，在code中使用：
+
+```python
+from qesdk import auth
+##授权码
+auth('your username','your authcode')
+from qetrader import listSimuAccounts, createSimuAccount,runStrat
+from qetrader.plugins.qealgoex import plugin_algoex 
+
+##实盘账户信息
+user_setting = {'investorid':'xxxxxx', 'password':'xxxxxxxx','broker':'xxxxxx'}
+
+if __name__=='__main__':
+    ##换成自己的用户名
+    user='myname'
+    ##如果有模拟账户，用第一个账户，没有新建一个
+    tokenlist = listSimuAccounts(user)
+    if len(tokenlist) > 0:
+        token = tokenlist[0]
+    else:
+        token = createSimuAccount(user)
+    ##运行策略，algoex插件本身就是个策略实例，可以直接使用
+    runStrat(user,'real',[plugin_algoex], simu_token=token,real_account=user_setting)
+
+```
+
```

### Comparing `qetrader-1.0.8/src/qetrader.egg-info/SOURCES.txt` & `qetrader-1.0.9/src/qetrader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

