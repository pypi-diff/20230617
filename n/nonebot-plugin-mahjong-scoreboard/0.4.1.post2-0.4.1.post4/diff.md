# Comparing `tmp/nonebot_plugin_mahjong_scoreboard-0.4.1.post2.tar.gz` & `tmp/nonebot_plugin_mahjong_scoreboard-0.4.1.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mahjong_scoreboard-0.4.1.post2.tar", max compression
+gzip compressed data, was "nonebot_plugin_mahjong_scoreboard-0.4.1.post4.tar", max compression
```

## Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2.tar` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421764 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/LICENSE
--rw-r--r--   0        0        0     1055 2023-06-03 01:21:34.413482 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/pyproject.toml
--rw-r--r--   0        0        0     6690 2023-06-02 03:44:53.162732 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/README.MD
--rw-r--r--   0        0        0     3108 2023-06-03 01:21:14.369541 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/__init__.py
--rw-r--r--   0        0        0     1052 2023-06-02 00:08:25.892232 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/config.py
--rw-r--r--   0        0        0      287 2023-03-13 11:15:04.246316 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/__init__.py
--rw-r--r--   0        0        0     2860 2023-06-03 01:11:07.278231 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py
--rw-r--r--   0        0        0     6192 2023-06-03 01:12:04.997398 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py
--rw-r--r--   0        0        0    11880 2023-06-03 01:10:38.251192 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py
--rw-r--r--   0        0        0     5262 2023-06-03 01:12:05.029399 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py
--rw-r--r--   0        0        0     1551 2023-06-03 01:13:59.870976 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py
--rw-r--r--   0        0        0     1549 2023-05-07 03:44:28.905567 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py
--rw-r--r--   0        0        0     2640 2023-06-03 00:45:52.599182 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py
--rw-r--r--   0        0        0     3937 2023-06-03 00:45:52.625179 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py
--rw-r--r--   0        0        0      935 2023-06-02 00:08:25.897230 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/pagination_mapper.py
--rw-r--r--   0        0        0     1947 2023-06-02 00:08:25.897230 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py
--rw-r--r--   0        0        0     2873 2023-06-02 00:08:25.898229 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py
--rw-r--r--   0        0        0      928 2023-06-02 00:08:25.899230 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py
--rw-r--r--   0        0        0      229 2023-06-02 00:08:25.899230 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mg.py
--rw-r--r--   0        0        0    13031 2023-06-03 01:12:05.024401 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py
--rw-r--r--   0        0        0     2030 2023-06-03 01:12:04.988398 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py
--rw-r--r--   0        0        0     1985 2023-06-03 01:12:05.015398 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py
--rw-r--r--   0        0        0     4763 2023-06-03 01:12:05.003402 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py
--rw-r--r--   0        0        0     3150 2023-06-03 01:12:05.010398 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py
--rw-r--r--   0        0        0        0 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/__init__.py
--rw-r--r--   0        0        0     7606 2023-06-03 01:10:38.238192 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/dep.py
--rw-r--r--   0        0        0     4318 2023-06-02 00:08:25.903232 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py
--rw-r--r--   0        0        0      481 2023-06-02 03:44:53.191732 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py
--rw-r--r--   0        0        0     2778 2023-06-02 00:08:25.904230 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py
--rw-r--r--   0        0        0      378 2023-06-03 01:10:38.228192 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/errors.py
--rw-r--r--   0        0        0     2185 2023-06-02 00:08:25.905230 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py
--rw-r--r--   0        0        0      492 2022-10-25 11:55:32.743202 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/model/enums.py
--rw-r--r--   0        0        0        0 2023-06-02 00:08:25.905230 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/__init__.py
--rw-r--r--   0        0        0     1218 2023-06-02 00:08:25.906230 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py
--rw-r--r--   0        0        0     1287 2023-06-02 00:08:25.906230 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py
--rw-r--r--   0        0        0      755 2023-06-02 00:08:25.907233 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py
--rw-r--r--   0        0        0      772 2023-06-02 00:08:25.907233 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py
--rw-r--r--   0        0        0     1705 2023-06-02 00:08:25.908230 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py
--rw-r--r--   0        0        0      928 2023-06-02 00:08:25.908230 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py
--rw-r--r--   0        0        0      122 2023-06-02 00:08:25.909232 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/__init__.py
--rw-r--r--   0        0        0     1155 2023-06-02 00:08:25.909232 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py
--rw-r--r--   0        0        0      258 2023-06-02 00:08:25.909232 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/data_source.py
--rw-r--r--   0        0        0     2022 2023-06-02 00:08:25.910232 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py
--rw-r--r--   0        0        0      163 2023-06-02 00:08:25.910232 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/__init__.py
--rw-r--r--   0        0        0      263 2023-06-02 00:08:25.911229 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v1_to_v2.py
--rw-r--r--   0        0        0     2523 2023-06-02 00:08:25.911229 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py
--rw-r--r--   0        0        0      399 2023-06-02 00:08:25.912229 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/base.py
--rw-r--r--   0        0        0     7261 2023-06-02 00:08:25.912229 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py
--rw-r--r--   0        0        0     4444 2023-06-02 00:08:25.913229 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/game.py
--rw-r--r--   0        0        0      797 2023-06-02 00:08:25.913229 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/group.py
--rw-r--r--   0        0        0      174 2023-06-02 00:08:25.913229 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/pagination.py
--rw-r--r--   0        0        0     8813 2023-06-03 01:10:38.219196 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/season.py
--rw-r--r--   0        0        0        0 2023-06-02 00:08:25.914233 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/types/__init__.py
--rw-r--r--   0        0        0      510 2023-06-02 00:08:25.915229 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/types/pydantic.py
--rw-r--r--   0        0        0      736 2023-06-02 00:08:25.915229 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/user.py
--rw-r--r--   0        0        0        0 2022-10-11 14:02:12.038461 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/service/__init__.py
--rw-r--r--   0        0        0    18263 2023-06-03 01:10:38.189194 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py
--rw-r--r--   0        0        0     1027 2023-06-02 00:08:25.916229 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py
--rw-r--r--   0        0        0     4122 2023-06-02 00:08:25.917229 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py
--rw-r--r--   0        0        0     4108 2023-06-03 01:10:38.193191 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py
--rw-r--r--   0        0        0     2797 2023-06-03 01:10:38.206194 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py
--rw-r--r--   0        0        0      356 2023-06-02 00:08:25.918232 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py
--rw-r--r--   0        0        0        0 2022-10-25 10:53:45.022120 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/utils/__init__.py
--rw-r--r--   0        0        0      288 2022-10-25 10:55:21.893872 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/utils/date.py
--rw-r--r--   0        0        0     1240 2022-10-25 10:57:00.084086 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py
--rw-r--r--   0        0        0      101 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/utils/nonebot.py
--rw-r--r--   0        0        0      482 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/utils/rank.py
--rw-r--r--   0        0        0      758 2023-06-02 00:08:25.919230 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/utils/session.py
--rw-r--r--   0        0        0      761 2023-03-13 11:15:04.268743 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py
--rw-r--r--   0        0        0     7667 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.4.1.post2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421764 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/LICENSE
+-rw-r--r--   0        0        0     1058 2023-06-17 16:28:29.592471 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/pyproject.toml
+-rw-r--r--   0        0        0     6690 2023-06-02 03:44:53.162732 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/README.MD
+-rw-r--r--   0        0        0     3108 2023-06-03 01:21:14.369541 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/__init__.py
+-rw-r--r--   0        0        0     1052 2023-06-02 00:08:25.892232 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/config.py
+-rw-r--r--   0        0        0      287 2023-03-13 11:15:04.246316 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/__init__.py
+-rw-r--r--   0        0        0     2860 2023-06-03 01:11:07.278231 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py
+-rw-r--r--   0        0        0     6192 2023-06-03 01:12:04.997398 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py
+-rw-r--r--   0        0        0    11880 2023-06-03 01:10:38.251192 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py
+-rw-r--r--   0        0        0     5262 2023-06-03 01:12:05.029399 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py
+-rw-r--r--   0        0        0     1551 2023-06-03 01:13:59.870976 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py
+-rw-r--r--   0        0        0     1549 2023-05-07 03:44:28.905567 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py
+-rw-r--r--   0        0        0     2640 2023-06-03 00:45:52.599182 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py
+-rw-r--r--   0        0        0     3937 2023-06-03 00:45:52.625179 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py
+-rw-r--r--   0        0        0      935 2023-06-02 00:08:25.897230 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/pagination_mapper.py
+-rw-r--r--   0        0        0     1947 2023-06-02 00:08:25.897230 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py
+-rw-r--r--   0        0        0     2873 2023-06-02 00:08:25.898229 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py
+-rw-r--r--   0        0        0      928 2023-06-02 00:08:25.899230 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py
+-rw-r--r--   0        0        0      229 2023-06-02 00:08:25.899230 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mg.py
+-rw-r--r--   0        0        0    13031 2023-06-03 01:12:05.024401 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py
+-rw-r--r--   0        0        0     2030 2023-06-03 01:12:04.988398 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py
+-rw-r--r--   0        0        0     1985 2023-06-03 01:12:05.015398 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py
+-rw-r--r--   0        0        0     4763 2023-06-03 01:12:05.003402 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py
+-rw-r--r--   0        0        0     3150 2023-06-03 01:12:05.010398 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/utils/__init__.py
+-rw-r--r--   0        0        0     7606 2023-06-03 01:10:38.238192 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/utils/dep.py
+-rw-r--r--   0        0        0     4318 2023-06-02 00:08:25.903232 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py
+-rw-r--r--   0        0        0      481 2023-06-02 03:44:53.191732 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py
+-rw-r--r--   0        0        0     2778 2023-06-02 00:08:25.904230 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py
+-rw-r--r--   0        0        0      378 2023-06-03 01:10:38.228192 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/errors.py
+-rw-r--r--   0        0        0     2185 2023-06-02 00:08:25.905230 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py
+-rw-r--r--   0        0        0      492 2022-10-25 11:55:32.743202 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/model/enums.py
+-rw-r--r--   0        0        0        0 2023-06-02 00:08:25.905230 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/__init__.py
+-rw-r--r--   0        0        0     1218 2023-06-02 00:08:25.906230 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py
+-rw-r--r--   0        0        0     1287 2023-06-02 00:08:25.906230 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py
+-rw-r--r--   0        0        0      755 2023-06-02 00:08:25.907233 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py
+-rw-r--r--   0        0        0      772 2023-06-02 00:08:25.907233 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-02 00:08:25.908230 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py
+-rw-r--r--   0        0        0      928 2023-06-02 00:08:25.908230 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py
+-rw-r--r--   0        0        0      122 2023-06-02 00:08:25.909232 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-02 00:08:25.909232 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py
+-rw-r--r--   0        0        0      258 2023-06-02 00:08:25.909232 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/data_source.py
+-rw-r--r--   0        0        0     2022 2023-06-02 00:08:25.910232 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py
+-rw-r--r--   0        0        0      163 2023-06-02 00:08:25.910232 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/__init__.py
+-rw-r--r--   0        0        0      263 2023-06-02 00:08:25.911229 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v1_to_v2.py
+-rw-r--r--   0        0        0     2523 2023-06-02 00:08:25.911229 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py
+-rw-r--r--   0        0        0      399 2023-06-02 00:08:25.912229 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/base.py
+-rw-r--r--   0        0        0     7261 2023-06-02 00:08:25.912229 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py
+-rw-r--r--   0        0        0     4444 2023-06-02 00:08:25.913229 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/game.py
+-rw-r--r--   0        0        0      797 2023-06-02 00:08:25.913229 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/group.py
+-rw-r--r--   0        0        0      174 2023-06-02 00:08:25.913229 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/pagination.py
+-rw-r--r--   0        0        0     8813 2023-06-03 01:10:38.219196 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/season.py
+-rw-r--r--   0        0        0        0 2023-06-02 00:08:25.914233 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/types/__init__.py
+-rw-r--r--   0        0        0      510 2023-06-02 00:08:25.915229 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/types/pydantic.py
+-rw-r--r--   0        0        0      736 2023-06-02 00:08:25.915229 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/user.py
+-rw-r--r--   0        0        0        0 2022-10-11 14:02:12.038461 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/service/__init__.py
+-rw-r--r--   0        0        0    18263 2023-06-03 01:10:38.189194 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py
+-rw-r--r--   0        0        0     1027 2023-06-02 00:08:25.916229 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py
+-rw-r--r--   0        0        0     4122 2023-06-02 00:08:25.917229 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py
+-rw-r--r--   0        0        0     4108 2023-06-03 01:10:38.193191 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py
+-rw-r--r--   0        0        0     2797 2023-06-03 01:10:38.206194 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py
+-rw-r--r--   0        0        0      356 2023-06-02 00:08:25.918232 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py
+-rw-r--r--   0        0        0        0 2022-10-25 10:53:45.022120 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/utils/__init__.py
+-rw-r--r--   0        0        0      288 2022-10-25 10:55:21.893872 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/utils/date.py
+-rw-r--r--   0        0        0     1240 2022-10-25 10:57:00.084086 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py
+-rw-r--r--   0        0        0      101 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/utils/nonebot.py
+-rw-r--r--   0        0        0      482 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/utils/rank.py
+-rw-r--r--   0        0        0      758 2023-06-02 00:08:25.919230 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/utils/session.py
+-rw-r--r--   0        0        0      761 2023-03-13 11:15:04.268743 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py
+-rw-r--r--   0        0        0     7648 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.4.1.post4/PKG-INFO
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/LICENSE` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/pyproject.toml` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "nonebot-plugin-mahjong-scoreboard"
-version = "0.4.1.post2"
+version = "0.4.1.post4"
 description = "日麻寄分器（NoneBot插件）"
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.MD"
 license = "MIT"
 repository = "https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard"
 packages = [
     { include = "nonebot_plugin_mahjong_scoreboard", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = "^2.2.2"
 nonebot_plugin_apscheduler = "^0.2.0"
-nonebot-plugin-gocqhttp-cross-machine-upload-file = "^0.1.5"
+nonebot-plugin-gocqhttp-cross-machine-upload-file = ">=0.1.5"
 nonebot-plugin-localstore = "^0.4.1"
 nonebot-plugin-sqlalchemy = "^0.2.1"
-nonebot-plugin-session = "^0.0.3"
+nonebot-plugin-session = ">=0.0.3"
 aiosqlite = ">=0.17,<0.19"
-tzlocal = "^4.2"
+tzlocal = ">=4.2"
 cachetools = "^5.2.0"
 
 [tool.poetry.group.dev.dependencies]
 nonebot2 = { extras = ["httpx", "fastapi"], version = "^2.0.0rc3" }
 nonebot-adapter-qqguild = "^0.2.2"
 nonebug = "^0.2.1"
 flake8 = "^5.0.4"
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/README.MD` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/README.MD`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/config.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/pagination_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/pagination_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/dep.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/utils/dep.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/game.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/group.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/season.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/season.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/repository/user.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/repository/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/utils/session.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/utils/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.1.post2/PKG-INFO` & `nonebot_plugin_mahjong_scoreboard-0.4.1.post4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mahjong-scoreboard
-Version: 0.4.1.post2
+Version: 0.4.1.post4
 Summary: 日麻寄分器（NoneBot插件）
 Home-page: https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiosqlite (>=0.17,<0.19)
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
-Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-file (>=0.1.5,<0.2.0)
+Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-file (>=0.1.5)
 Requires-Dist: nonebot-plugin-localstore (>=0.4.1,<0.5.0)
-Requires-Dist: nonebot-plugin-session (>=0.0.3,<0.0.4)
+Requires-Dist: nonebot-plugin-session (>=0.0.3)
 Requires-Dist: nonebot-plugin-sqlalchemy (>=0.2.1,<0.3.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: tzlocal (>=4.2,<5.0)
+Requires-Dist: tzlocal (>=4.2)
 Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard
 Description-Content-Type: text/plain
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1 Name: nonebot-plugin-mahjong-scoreboard Version:
-0.4.1.post2 Summary: æ¥éº»å¯åå¨ï¼NoneBotæä»¶ï¼ Home-page: https://
+0.4.1.post4 Summary: æ¥éº»å¯åå¨ï¼NoneBotæä»¶ï¼ Home-page: https://
 github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard License: MIT Author:
 ssttkkl Author-email: huang.wen.long@hotmail.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiosqlite (>=0.17,<0.19) Requires-
 Dist: cachetools (>=5.2.0,<6.0.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-
-file (>=0.1.5,<0.2.0) Requires-Dist: nonebot-plugin-localstore (>=0.4.1,<0.5.0)
-Requires-Dist: nonebot-plugin-session (>=0.0.3,<0.0.4) Requires-Dist: nonebot-
-plugin-sqlalchemy (>=0.2.1,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
-Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
-tzlocal (>=4.2,<5.0) Project-URL: Repository, https://github.com/ssttkkl/
-nonebot-plugin-mahjong-scoreboard Description-Content-Type: text/plain
+file (>=0.1.5) Requires-Dist: nonebot-plugin-localstore (>=0.4.1,<0.5.0)
+Requires-Dist: nonebot-plugin-session (>=0.0.3) Requires-Dist: nonebot-plugin-
+sqlalchemy (>=0.2.1,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-
+Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist: tzlocal
+(>=4.2) Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-
+mahjong-scoreboard Description-Content-Type: text/plain
                                    [nonebot]
           nonebot-plugin-mahjong-scoreboard ============ _â¨ NoneBot
                           æ¥éº»è®°åå¨æä»¶ â¨_
                            [license] [pypi] [python]
 æ¯æééå¨ï¼[OneBot V11](https://onebot.adapters.nonebot.dev/)ã[QQ
 Guild](https://github.com/nonebot/adapter-qqguild) ## åè½
 ä¸ºç¾¤åæä¾æ¥éº»å¯¹å±åæ°è®°å½ãæ ¹æ®é©¬ç¹è¿è¡PTç²¾ç®ï¼ç»è®¡PTå¢åï¼æ¯æå¯¹å±ä¸æ¦åæ¥è¯¢ä¸å¯¼åºã
```

