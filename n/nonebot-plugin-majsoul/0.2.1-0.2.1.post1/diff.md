# Comparing `tmp/nonebot_plugin_majsoul-0.2.1.tar.gz` & `tmp/nonebot_plugin_majsoul-0.2.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_majsoul-0.2.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_majsoul-0.2.1.post1.tar", max compression
```

## Comparing `nonebot_plugin_majsoul-0.2.1.tar` & `nonebot_plugin_majsoul-0.2.1.post1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448957 nonebot_plugin_majsoul-0.2.1/LICENSE
--rw-r--r--   0        0        0      729 2023-06-02 03:58:06.011897 nonebot_plugin_majsoul-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3619 2023-05-25 09:15:00.279006 nonebot_plugin_majsoul-0.2.1/README.md
--rw-r--r--   0        0        0     1144 2023-05-29 13:21:52.045266 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/__init__.py
--rw-r--r--   0        0        0      366 2023-05-25 08:45:02.584548 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/config.py
--rw-r--r--   0        0        0      189 2022-12-04 13:51:12.479077 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/errors.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.480120 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/interceptors/__init__.py
--rw-r--r--   0        0        0     1463 2022-12-05 01:32:49.512537 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/interceptors/handle_error.py
--rw-r--r--   0        0        0        0 2022-12-04 15:13:35.630196 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/network/__init__.py
--rw-r--r--   0        0        0      730 2022-12-09 13:59:04.659310 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/network/auto_retry.py
--rw-r--r--   0        0        0     3623 2022-12-09 13:59:04.628312 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/network/host_prober.py
--rw-r--r--   0        0        0      108 2022-12-05 07:11:39.022841 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475435 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/__init__.py
--rw-r--r--   0        0        0     5024 2022-12-05 14:11:58.665190 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/api.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475949 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/__init__.py
--rw-r--r--   0        0        0     1194 2022-12-05 03:49:36.925512 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py
--rw-r--r--   0        0        0     1967 2022-12-13 10:02:54.142968 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py
--rw-r--r--   0        0        0      608 2022-12-05 14:13:38.468214 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py
--rw-r--r--   0        0        0       85 2022-12-04 13:51:12.476988 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/player_num.py
--rw-r--r--   0        0        0     1538 2023-05-10 04:19:02.870093 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py
--rw-r--r--   0        0        0      490 2022-12-13 10:02:53.723372 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/player_stats.py
--rw-r--r--   0        0        0     2153 2022-12-04 13:51:12.478551 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.481159 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/mappers/__init__.py
--rw-r--r--   0        0        0     2377 2022-12-05 07:11:39.023842 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py
--rw-r--r--   0        0        0      262 2022-12-04 13:51:12.481677 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/mappers/general.py
--rw-r--r--   0        0        0     1634 2022-12-04 14:39:58.711032 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py
--rw-r--r--   0        0        0      232 2022-12-04 13:58:13.904298 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/mappers/player_num.py
--rw-r--r--   0        0        0      480 2023-05-10 04:19:26.060573 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/mappers/player_rank.py
--rw-r--r--   0        0        0     2536 2022-12-05 14:13:31.596221 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py
--rw-r--r--   0        0        0     4126 2022-12-04 13:58:13.909299 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.483754 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/parsers/__init__.py
--rw-r--r--   0        0        0      568 2023-01-25 14:19:08.842106 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py
--rw-r--r--   0        0        0     2544 2022-12-04 15:26:45.927547 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py
--rw-r--r--   0        0        0     1189 2023-01-25 14:19:08.832105 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py
--rw-r--r--   0        0        0     7318 2023-05-10 04:08:59.781216 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py
--rw-r--r--   0        0        0     9721 2023-06-02 03:57:51.665919 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py
--rw-r--r--   0        0        0     6945 2023-05-10 04:08:59.775198 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py
--rw-r--r--   0        0        0       67 2023-05-25 08:11:04.925321 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paipu/__init__.py
--rw-r--r--   0        0        0      887 2023-05-25 08:12:40.329877 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paipu/downloader.py
--rw-r--r--   0        0        0     2729 2023-06-01 06:50:23.321782 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paipu/query_paipu.py
--rw-r--r--   0        0        0        0 2023-05-25 08:00:39.014941 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/utils/__init__.py
--rw-r--r--   0        0        0     1148 2022-12-04 13:51:12.509611 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/utils/decode_integer.py
--rw-r--r--   0        0        0      354 2022-12-11 14:52:31.955889 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/utils/my_executor.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247572 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/utils/nonebot.py
--rw-r--r--   0        0        0       98 2022-12-04 14:29:52.531881 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/utils/percentile.py
--rw-r--r--   0        0        0      482 2022-12-05 03:18:06.269891 nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/utils/rank.py
--rw-r--r--   0        0        0     4491 1970-01-01 00:00:00.000000 nonebot_plugin_majsoul-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448957 nonebot_plugin_majsoul-0.2.1.post1/LICENSE
+-rw-r--r--   0        0        0      739 2023-06-17 15:15:01.368383 nonebot_plugin_majsoul-0.2.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     3619 2023-05-25 09:15:00.279006 nonebot_plugin_majsoul-0.2.1.post1/README.md
+-rw-r--r--   0        0        0     1144 2023-05-29 13:21:52.045266 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/__init__.py
+-rw-r--r--   0        0        0      366 2023-05-25 08:45:02.584548 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/config.py
+-rw-r--r--   0        0        0      189 2022-12-04 13:51:12.479077 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/errors.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.480120 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/interceptors/__init__.py
+-rw-r--r--   0        0        0     1463 2022-12-05 01:32:49.512537 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/interceptors/handle_error.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:13:35.630196 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/network/__init__.py
+-rw-r--r--   0        0        0      730 2022-12-09 13:59:04.659310 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/network/auto_retry.py
+-rw-r--r--   0        0        0     3623 2022-12-09 13:59:04.628312 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/network/host_prober.py
+-rw-r--r--   0        0        0      108 2022-12-05 07:11:39.022841 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475435 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/__init__.py
+-rw-r--r--   0        0        0     5024 2022-12-05 14:11:58.665190 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/api.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475949 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/__init__.py
+-rw-r--r--   0        0        0     1194 2022-12-05 03:49:36.925512 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py
+-rw-r--r--   0        0        0     1967 2022-12-13 10:02:54.142968 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py
+-rw-r--r--   0        0        0      608 2022-12-05 14:13:38.468214 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py
+-rw-r--r--   0        0        0       85 2022-12-04 13:51:12.476988 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_num.py
+-rw-r--r--   0        0        0     1538 2023-05-10 04:19:02.870093 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py
+-rw-r--r--   0        0        0      490 2022-12-13 10:02:53.723372 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_stats.py
+-rw-r--r--   0        0        0     2153 2022-12-04 13:51:12.478551 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.481159 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/__init__.py
+-rw-r--r--   0        0        0     2377 2022-12-05 07:11:39.023842 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py
+-rw-r--r--   0        0        0      262 2022-12-04 13:51:12.481677 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/general.py
+-rw-r--r--   0        0        0     1634 2022-12-04 14:39:58.711032 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py
+-rw-r--r--   0        0        0      232 2022-12-04 13:58:13.904298 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/player_num.py
+-rw-r--r--   0        0        0      480 2023-05-10 04:19:26.060573 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/player_rank.py
+-rw-r--r--   0        0        0     2536 2022-12-05 14:13:31.596221 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py
+-rw-r--r--   0        0        0     4126 2022-12-04 13:58:13.909299 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.483754 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/__init__.py
+-rw-r--r--   0        0        0      568 2023-01-25 14:19:08.842106 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py
+-rw-r--r--   0        0        0     2544 2022-12-04 15:26:45.927547 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py
+-rw-r--r--   0        0        0     1189 2023-01-25 14:19:08.832105 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py
+-rw-r--r--   0        0        0     7318 2023-05-10 04:08:59.781216 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py
+-rw-r--r--   0        0        0     9721 2023-06-02 03:57:51.665919 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py
+-rw-r--r--   0        0        0     6945 2023-05-10 04:08:59.775198 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py
+-rw-r--r--   0        0        0       67 2023-05-25 08:11:04.925321 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paipu/__init__.py
+-rw-r--r--   0        0        0      887 2023-05-25 08:12:40.329877 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paipu/downloader.py
+-rw-r--r--   0        0        0     2729 2023-06-01 06:50:23.321782 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paipu/query_paipu.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:00:39.014941 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/__init__.py
+-rw-r--r--   0        0        0     1148 2022-12-04 13:51:12.509611 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/decode_integer.py
+-rw-r--r--   0        0        0      354 2022-12-11 14:52:31.955889 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/my_executor.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247572 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/nonebot.py
+-rw-r--r--   0        0        0       98 2022-12-04 14:29:52.531881 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/percentile.py
+-rw-r--r--   0        0        0      482 2022-12-05 03:18:06.269891 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/rank.py
+-rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 nonebot_plugin_majsoul-0.2.1.post1/PKG-INFO
```

### Comparing `nonebot_plugin_majsoul-0.2.1/LICENSE` & `nonebot_plugin_majsoul-0.2.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/pyproject.toml` & `nonebot_plugin_majsoul-0.2.1.post1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "nonebot-plugin-majsoul"
-version = "0.2.1"
-description = ""
+version = "0.2.1.post1"
+description = "NoneBot2 雀魂信息查询插件"
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 packages = [
     { include = "nonebot_plugin_majsoul", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = {extras = ["httpx"], version = "^2.0.0"}
 nonebot-adapter-onebot = "^2.2.3"
 nonebot-plugin-send-anything-anywhere = ">=0.2.1"
 nonebot-plugin-gocqhttp-cross-machine-upload-file = ">=0.1.4"
-tzlocal = "^4.2"
+tzlocal = ">=4.2"
 monthdelta = "^0.9.1"
 icmplib = "^3.0.3"
 matplotlib = "^3.6.2"
-typing-extensions = "^4.4.0"
 tensoul = "^0.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_majsoul-0.2.1/README.md` & `nonebot_plugin_majsoul-0.2.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/__init__.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/interceptors/handle_error.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/interceptors/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/network/auto_retry.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/network/auto_retry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/network/host_prober.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/network/host_prober.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/api.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paipu/downloader.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paipu/downloader.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/paipu/query_paipu.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paipu/query_paipu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/src/nonebot_plugin_majsoul/utils/decode_integer.py` & `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/decode_integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1/PKG-INFO` & `nonebot_plugin_majsoul-0.2.1.post1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-majsoul
-Version: 0.2.1
-Summary: 
+Version: 0.2.1.post1
+Summary: NoneBot2 雀魂信息查询插件
 License: AGPL-3.0
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,16 +15,15 @@
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: monthdelta (>=0.9.1,<0.10.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-file (>=0.1.4)
 Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.1)
 Requires-Dist: nonebot2[httpx] (>=2.0.0,<3.0.0)
 Requires-Dist: tensoul (>=0.1.0,<0.2.0)
-Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
-Requires-Dist: tzlocal (>=4.2,<5.0)
+Requires-Dist: tzlocal (>=4.2)
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-majsoul Version: 0.2.1 Summary:
-License: AGPL-3.0 Author: ssttkkl Author-email: huang.wen.long@hotmail.com
-Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU Affero
-General Public License v3 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: icmplib (>=3.0.3,<4.0.0) Requires-Dist: matplotlib
-(>=3.6.2,<4.0.0) Requires-Dist: monthdelta (>=0.9.1,<0.10.0) Requires-Dist:
-nonebot-adapter-onebot (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-gocqhttp-
-cross-machine-upload-file (>=0.1.4) Requires-Dist: nonebot-plugin-send-
-anything-anywhere (>=0.2.1) Requires-Dist: nonebot2[httpx] (>=2.0.0,<3.0.0)
-Requires-Dist: tensoul (>=0.1.0,<0.2.0) Requires-Dist: typing-extensions
-(>=4.4.0,<5.0.0) Requires-Dist: tzlocal (>=4.2,<5.0) Description-Content-Type:
-text/markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-majsoul Version: 0.2.1.post1
+Summary: NoneBot2 éé­ä¿¡æ¯æ¥è¯¢æä»¶ License: AGPL-3.0 Author: ssttkkl
+Author-email: huang.wen.long@hotmail.com Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: icmplib
+(>=3.0.3,<4.0.0) Requires-Dist: matplotlib (>=3.6.2,<4.0.0) Requires-Dist:
+monthdelta (>=0.9.1,<0.10.0) Requires-Dist: nonebot-adapter-onebot
+(>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-
+file (>=0.1.4) Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.1)
+Requires-Dist: nonebot2[httpx] (>=2.0.0,<3.0.0) Requires-Dist: tensoul
+(>=0.1.0,<0.2.0) Requires-Dist: tzlocal (>=4.2) Description-Content-Type: text/
+markdown
                                    [nonebot]
     nonebot-plugin-majsoul ============ _â¨ éé­ä¿¡æ¯æ¥è¯¢æä»¶ â¨_
                            [license] [pypi] [python]
 å[DaiShengSheng/Majsoul_bot](https://github.com/DaiShengSheng/
 Majsoul_bot)å¯åèåçéé­ä¿¡æ¯æ¥è¯¢ Bot æä»¶ã
 æ¯æééå¨ï¼Onebot V11 ## åè½ ### éé­çè°±å± ####
 æ¥è¯¢ä¸ªäººæ°æ®ï¼å¯æç§æ¶é´ãæç§åºæ°ãæç§æ¿é´ç±»åæ¥è¯¢ï¼
```

