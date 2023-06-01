# Comparing `tmp/nonebot_plugin_mahjong_scoreboard-0.4.0a1.tar.gz` & `tmp/nonebot_plugin_mahjong_scoreboard-0.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mahjong_scoreboard-0.4.0a1.tar", max compression
+gzip compressed data, was "nonebot_plugin_mahjong_scoreboard-0.4.0a2.tar", max compression
```

## Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1.tar` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2.tar`

### file list

```diff
@@ -1,67 +1,69 @@
--rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421764 nonebot_plugin_mahjong_scoreboard-0.4.0a1/LICENSE
--rw-r--r--   0        0        0     1054 2023-05-31 16:17:17.191384 nonebot_plugin_mahjong_scoreboard-0.4.0a1/pyproject.toml
--rw-r--r--   0        0        0     6759 2023-05-07 03:20:47.530795 nonebot_plugin_mahjong_scoreboard-0.4.0a1/README.MD
--rw-r--r--   0        0        0     2335 2023-05-31 16:17:02.523326 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-31 16:17:02.544324 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/config.py
--rw-r--r--   0        0        0      287 2023-03-13 11:15:04.246316 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/__init__.py
--rw-r--r--   0        0        0     2373 2023-05-31 13:53:36.752099 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py
--rw-r--r--   0        0        0     5805 2023-05-31 12:49:29.901146 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py
--rw-r--r--   0        0        0    11539 2023-05-31 12:49:29.911147 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py
--rw-r--r--   0        0        0     4936 2023-05-31 13:38:31.503444 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py
--rw-r--r--   0        0        0     1404 2023-05-31 07:27:37.121738 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py
--rw-r--r--   0        0        0     1549 2023-05-07 03:44:28.905567 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py
--rw-r--r--   0        0        0     2443 2023-05-31 13:06:45.874125 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py
--rw-r--r--   0        0        0     2895 2023-05-31 07:27:37.122737 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py
--rw-r--r--   0        0        0     1947 2023-05-31 07:27:37.123736 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py
--rw-r--r--   0        0        0     2873 2023-05-31 13:38:31.556446 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py
--rw-r--r--   0        0        0      928 2023-05-31 07:27:37.124738 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py
--rw-r--r--   0        0        0    11888 2023-05-31 12:29:56.485530 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py
--rw-r--r--   0        0        0     1787 2023-05-31 13:38:31.575444 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py
--rw-r--r--   0        0        0     1705 2023-05-31 13:46:09.661196 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py
--rw-r--r--   0        0        0     4498 2023-05-31 12:49:29.906148 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py
--rw-r--r--   0        0        0     3134 2023-05-31 13:38:31.546447 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py
--rw-r--r--   0        0        0        0 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/__init__.py
--rw-r--r--   0        0        0     5289 2023-05-31 14:11:42.691560 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/dep.py
--rw-r--r--   0        0        0     4232 2023-05-31 12:10:39.999248 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py
--rw-r--r--   0        0        0     1070 2023-05-31 11:56:26.489690 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py
--rw-r--r--   0        0        0     2519 2023-03-13 11:15:04.258743 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py
--rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228228 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/errors.py
--rw-r--r--   0        0        0     2185 2023-05-31 13:38:31.528445 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py
--rw-r--r--   0        0        0      492 2022-10-25 11:55:32.743202 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/model/enums.py
--rw-r--r--   0        0        0        0 2023-05-31 07:27:37.128738 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/__init__.py
--rw-r--r--   0        0        0     1218 2023-05-31 13:50:13.726888 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py
--rw-r--r--   0        0        0     1287 2023-05-31 13:06:45.863127 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py
--rw-r--r--   0        0        0      755 2023-05-31 12:07:55.000532 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py
--rw-r--r--   0        0        0      772 2023-05-31 07:27:37.130736 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py
--rw-r--r--   0        0        0     1705 2023-05-31 13:51:24.924727 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py
--rw-r--r--   0        0        0      928 2023-05-31 16:16:01.038694 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py
--rw-r--r--   0        0        0      122 2023-05-31 07:27:37.130736 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/__init__.py
--rw-r--r--   0        0        0     1155 2023-05-31 07:27:37.131737 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py
--rw-r--r--   0        0        0      258 2023-05-31 16:16:01.029716 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/data_source.py
--rw-r--r--   0        0        0     2022 2023-05-31 07:27:37.132737 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py
--rw-r--r--   0        0        0      163 2023-05-31 07:27:37.132737 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/__init__.py
--rw-r--r--   0        0        0      263 2023-05-31 07:27:37.133737 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v1_to_v2.py
--rw-r--r--   0        0        0     2523 2023-05-31 07:27:37.133737 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py
--rw-r--r--   0        0        0      399 2023-05-31 07:27:37.134736 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/base.py
--rw-r--r--   0        0        0     7261 2023-05-31 12:28:17.427163 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py
--rw-r--r--   0        0        0     4184 2023-05-31 12:27:53.600829 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/game.py
--rw-r--r--   0        0        0      797 2023-05-31 12:27:53.584832 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/group.py
--rw-r--r--   0        0        0    11415 2023-05-31 12:27:53.595831 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/season.py
--rw-r--r--   0        0        0        0 2023-05-31 07:27:37.135740 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/types/__init__.py
--rw-r--r--   0        0        0      510 2023-05-31 07:27:37.136738 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/types/pydantic.py
--rw-r--r--   0        0        0      736 2023-05-31 12:27:53.606829 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/user.py
--rw-r--r--   0        0        0        0 2022-10-11 14:02:12.038461 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/__init__.py
--rw-r--r--   0        0        0    18143 2023-05-31 16:17:02.535329 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py
--rw-r--r--   0        0        0     1027 2023-05-31 12:27:53.572832 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py
--rw-r--r--   0        0        0     4122 2023-05-31 13:43:41.683542 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py
--rw-r--r--   0        0        0     4128 2023-05-31 12:27:53.612405 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py
--rw-r--r--   0        0        0     3149 2023-05-31 13:41:23.034657 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py
--rw-r--r--   0        0        0      356 2023-05-31 11:33:58.053326 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py
--rw-r--r--   0        0        0        0 2022-10-25 10:53:45.022120 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/__init__.py
--rw-r--r--   0        0        0      288 2022-10-25 10:55:21.893872 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/date.py
--rw-r--r--   0        0        0     1240 2022-10-25 10:57:00.084086 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py
--rw-r--r--   0        0        0      101 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/nonebot.py
--rw-r--r--   0        0        0      482 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/rank.py
--rw-r--r--   0        0        0      758 2023-05-31 13:06:45.885125 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/session.py
--rw-r--r--   0        0        0      761 2023-03-13 11:15:04.268743 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py
--rw-r--r--   0        0        0     7733 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421764 nonebot_plugin_mahjong_scoreboard-0.4.0a2/LICENSE
+-rw-r--r--   0        0        0     1054 2023-06-01 04:55:22.897241 nonebot_plugin_mahjong_scoreboard-0.4.0a2/pyproject.toml
+-rw-r--r--   0        0        0     6759 2023-05-07 03:20:47.530795 nonebot_plugin_mahjong_scoreboard-0.4.0a2/README.MD
+-rw-r--r--   0        0        0     2335 2023-05-31 16:17:02.523326 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-31 16:17:02.544324 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/config.py
+-rw-r--r--   0        0        0      287 2023-03-13 11:15:04.246316 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/__init__.py
+-rw-r--r--   0        0        0     2610 2023-06-01 14:08:16.854206 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py
+-rw-r--r--   0        0        0     5582 2023-06-01 14:47:11.381807 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py
+-rw-r--r--   0        0        0    11016 2023-06-01 15:07:16.677379 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py
+-rw-r--r--   0        0        0     4870 2023-06-01 14:08:16.864205 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py
+-rw-r--r--   0        0        0     1404 2023-05-31 07:27:37.121738 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py
+-rw-r--r--   0        0        0     1549 2023-05-07 03:44:28.905567 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py
+-rw-r--r--   0        0        0     2443 2023-05-31 13:06:45.874125 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py
+-rw-r--r--   0        0        0     3756 2023-06-01 14:46:47.079404 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py
+-rw-r--r--   0        0        0      935 2023-06-01 14:43:05.933065 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/pagination_mapper.py
+-rw-r--r--   0        0        0     1947 2023-05-31 07:27:37.123736 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py
+-rw-r--r--   0        0        0     2873 2023-05-31 13:38:31.556446 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py
+-rw-r--r--   0        0        0      928 2023-05-31 07:27:37.124738 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py
+-rw-r--r--   0        0        0    12214 2023-06-01 06:38:55.812825 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py
+-rw-r--r--   0        0        0     1787 2023-05-31 13:38:31.575444 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py
+-rw-r--r--   0        0        0     1834 2023-06-01 14:21:07.726683 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py
+-rw-r--r--   0        0        0     4476 2023-06-01 06:29:06.042508 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py
+-rw-r--r--   0        0        0     2879 2023-06-01 15:12:26.336136 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/__init__.py
+-rw-r--r--   0        0        0     7607 2023-06-01 06:39:56.154899 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/dep.py
+-rw-r--r--   0        0        0     4318 2023-06-01 06:19:38.626043 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py
+-rw-r--r--   0        0        0      628 2023-06-01 06:19:38.613979 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py
+-rw-r--r--   0        0        0     2778 2023-06-01 15:03:14.755037 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py
+-rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228228 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/errors.py
+-rw-r--r--   0        0        0     2185 2023-05-31 13:38:31.528445 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py
+-rw-r--r--   0        0        0      492 2022-10-25 11:55:32.743202 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/model/enums.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:27:37.128738 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/__init__.py
+-rw-r--r--   0        0        0     1218 2023-06-01 03:48:42.054855 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py
+-rw-r--r--   0        0        0     1287 2023-05-31 13:06:45.863127 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py
+-rw-r--r--   0        0        0      755 2023-05-31 12:07:55.000532 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py
+-rw-r--r--   0        0        0      772 2023-05-31 07:27:37.130736 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py
+-rw-r--r--   0        0        0     1705 2023-05-31 13:51:24.924727 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py
+-rw-r--r--   0        0        0      928 2023-06-01 03:54:03.408815 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py
+-rw-r--r--   0        0        0      122 2023-05-31 07:27:37.130736 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/__init__.py
+-rw-r--r--   0        0        0     1155 2023-05-31 07:27:37.131737 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py
+-rw-r--r--   0        0        0      258 2023-05-31 16:16:01.029716 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/data_source.py
+-rw-r--r--   0        0        0     2022 2023-05-31 07:27:37.132737 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py
+-rw-r--r--   0        0        0      163 2023-05-31 07:27:37.132737 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/__init__.py
+-rw-r--r--   0        0        0      263 2023-05-31 07:27:37.133737 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v1_to_v2.py
+-rw-r--r--   0        0        0     2523 2023-05-31 07:27:37.133737 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py
+-rw-r--r--   0        0        0      399 2023-05-31 07:27:37.134736 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/base.py
+-rw-r--r--   0        0        0     7261 2023-05-31 12:28:17.427163 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py
+-rw-r--r--   0        0        0     4450 2023-06-01 14:09:26.708031 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/game.py
+-rw-r--r--   0        0        0      797 2023-05-31 12:27:53.584832 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/group.py
+-rw-r--r--   0        0        0      174 2023-06-01 14:10:09.416142 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/pagination.py
+-rw-r--r--   0        0        0     8821 2023-06-01 14:21:07.713682 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/season.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:27:37.135740 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/types/__init__.py
+-rw-r--r--   0        0        0      510 2023-05-31 07:27:37.136738 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/types/pydantic.py
+-rw-r--r--   0        0        0      736 2023-05-31 12:27:53.606829 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/user.py
+-rw-r--r--   0        0        0        0 2022-10-11 14:02:12.038461 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/__init__.py
+-rw-r--r--   0        0        0    18332 2023-06-01 15:12:26.327144 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py
+-rw-r--r--   0        0        0     1027 2023-05-31 12:27:53.572832 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py
+-rw-r--r--   0        0        0     4122 2023-05-31 13:43:41.683542 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py
+-rw-r--r--   0        0        0     4128 2023-05-31 12:27:53.612405 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py
+-rw-r--r--   0        0        0     2851 2023-06-01 14:21:07.722683 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py
+-rw-r--r--   0        0        0      356 2023-05-31 11:33:58.053326 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py
+-rw-r--r--   0        0        0        0 2022-10-25 10:53:45.022120 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/__init__.py
+-rw-r--r--   0        0        0      288 2022-10-25 10:55:21.893872 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/date.py
+-rw-r--r--   0        0        0     1240 2022-10-25 10:57:00.084086 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py
+-rw-r--r--   0        0        0      101 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/nonebot.py
+-rw-r--r--   0        0        0      482 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/rank.py
+-rw-r--r--   0        0        0      758 2023-05-31 13:06:45.885125 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/session.py
+-rw-r--r--   0        0        0      761 2023-03-13 11:15:04.268743 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py
+-rw-r--r--   0        0        0     7733 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.4.0a2/PKG-INFO
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/LICENSE` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/pyproject.toml` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mahjong-scoreboard"
-version = "0.4.0a1"
+version = "0.4.0a2"
 description = "日麻寄分器（NoneBot插件）"
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.MD"
 license = "MIT"
 repository = "https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard"
 packages = [
     { include = "nonebot_plugin_mahjong_scoreboard", from = "src" },
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/README.MD` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/README.MD`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/config.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from nonebot import on_command
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent
 
 from .interceptor import handle_error
 from .mapper.game_csv_mapper import write_games_csv
 from .utils.dep import GroupDep, SeasonFromUnaryArgOrRunningSeason
 from .utils.general_handlers import require_store_command_args, require_platform_group_id
+from ..errors import BadRequestError
 from ..model import Group, Season
 from ..model.enums import SeasonState
 from ..platform.upload_file import upload_file
 from ..service.game_service import get_games
 from ..utils.date import encode_date
 
 # ========== 导出赛季对局 ==========
@@ -24,24 +25,27 @@
 
 @export_season_games_matcher.handle()
 @handle_error()
 async def export_season_games(bot: Bot, event: MessageEvent, group: Group = GroupDep(),
                               season: Season = SeasonFromUnaryArgOrRunningSeason()):
     games = await get_games(group_id=group.id, season_id=season.id)
 
+    if games.total == 0:
+        raise BadRequestError("本赛季还没有创建过对局")
+
     filename = f"赛季对局 {season.name}"
     if season.state == SeasonState.finished:
         filename += "（已结束）"
     else:
         now = datetime.now(tzlocal.get_localzone())
         filename += f"（截至{encode_date(now)}）"
     filename += ".csv"
 
     with StringIO() as sio:
-        await write_games_csv(sio, games)
+        await write_games_csv(sio, games.data)
 
         data = sio.getvalue().encode("utf_8_sig")
         await upload_file(bot, event, filename, data)
 
 
 # ========== 导出所有对局 ==========
 export_group_games_matcher = on_command("导出所有对局", priority=5)
@@ -51,15 +55,18 @@
 
 
 @export_group_games_matcher.handle()
 @handle_error()
 async def export_group_games(bot: Bot, event: MessageEvent, group: Group = GroupDep()):
     games = await get_games(group.id)
 
+    if games.total == 0:
+        raise BadRequestError("本群还没有创建过对局")
+
     now = datetime.now(tzlocal.get_localzone())
     filename = f"所有对局（截至{encode_date(now)}）.csv"
 
     with StringIO() as sio:
-        await write_games_csv(sio, games)
+        await write_games_csv(sio, games.data)
 
         data = sio.getvalue().encode("utf_8_sig")
         await upload_file(bot, event, filename, data)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from datetime import datetime, date, timedelta, time
 
 from nonebot import on_command, Bot
 from nonebot.internal.adapter import Event
 from nonebot.internal.matcher import Matcher
 
 from .interceptor import handle_error
-from .mapper.game_mapper import map_game
+from .mapper.game_mapper import map_game, map_game_lite
+from .mapper.pagination_mapper import map_pagination
 from .utils.dep import GroupDep, UnaryArg, UserDep
 from .utils.general_handlers import require_store_command_args, require_platform_group_id, require_platform_user_id
 from .utils.parse import parse_int_or_error
 from ..errors import BadRequestError
 from ..model import Group, User
 from ..platform.get_user_nickname import get_user_nickname
 from ..platform.send_messages import send_msgs
@@ -22,15 +23,15 @@
 require_store_command_args(query_by_code_matcher)
 require_platform_group_id(query_by_code_matcher)
 
 
 @query_by_code_matcher.handle()
 @handle_error()
 async def query_by_code(matcher: Matcher, group: Group = GroupDep(),
-                        game_code=UnaryArg(lookup_matcher_state=True, parser=lambda x: parse_int_or_error(x, '对局编号'))):
+                        game_code=UnaryArg(parser=lambda x: parse_int_or_error(x, '对局编号'))):
     if game_code is None:
         raise BadRequestError("请指定对局编号")
 
     game = await game_service.get_game(game_code, group.id)
     if game is None:
         raise BadRequestError("未找到指定对局")
 
@@ -44,101 +45,89 @@
 require_store_command_args(query_user_recent_games_matcher)
 require_platform_group_id(query_user_recent_games_matcher)
 require_platform_user_id(query_user_recent_games_matcher)
 
 
 @query_user_recent_games_matcher.handle()
 @handle_error()
-async def query_user_recent_games(bot: Bot, event: Event, matcher: Matcher,
+async def query_user_recent_games(bot: Bot, event: Event,
                                   group: Group = GroupDep(),
-                                  user: User = UserDep(lookup_matcher_state=True)):
+                                  user: User = UserDep()):
     end_time = datetime.combine(date.today() + timedelta(days=1), time())
     start_time = datetime.combine(end_time - timedelta(days=7), time())
 
-    games = await get_games(group.id, user.id, limit=5, reverse_order=True, time_span=(start_time, end_time))
-    if len(games) != 0:
-        msgs = []
-        msgs.append(f"以下是[{await get_user_nickname(bot, platform_user_id, group.platform_group_id)}]"
-                    f"的最近对局：")
-
-        for g in games:
-            msgs.append(await map_game(g, detailed=True))
+    games = await get_games(group.id, user.id, reverse_order=True, time_span=(start_time, end_time))
+    msgs = await map_pagination(games.data, map_game_lite)
+    if games.total != 0:
+        msgs.insert(0, f"以下是[{await get_user_nickname(bot, user.platform_user_id, group.platform_group_id)}]"
+                       f"最近七天的对局：")
 
         await send_msgs(bot, event, msgs)
     else:
-        await matcher.send("你还没有进行过对局")
+        raise BadRequestError("用户最近七天还没有进行过对局")
 
 
 # ========== 群最近对局 ==========
 query_group_recent_games_matcher = on_command("群最近对局", aliases={"最近对局"}, priority=5)
 
 require_store_command_args(query_group_recent_games_matcher)
 require_platform_group_id(query_group_recent_games_matcher)
 
 
 @query_group_recent_games_matcher.handle()
 @handle_error()
-async def query_group_recent_games(bot: Bot, event: Event, matcher: Matcher, group=GroupDep()):
+async def query_group_recent_games(bot: Bot, event: Event, group=GroupDep()):
     end_time = datetime.combine(date.today() + timedelta(days=1), time())
     start_time = datetime.combine(end_time - timedelta(days=7), time())
 
-    games = await get_games(group.id, limit=5, reverse_order=True, time_span=(start_time, end_time))
-    if len(games) != 0:
-        msgs = []
-        msgs.append(f"以下是本群的最近对局：")
-
-        for g in games:
-            msgs.append(await map_game(g, detailed=True))
+    games = await get_games(group.id, reverse_order=True, time_span=(start_time, end_time))
+    msgs = await map_pagination(games.data, map_game_lite)
+    if games.total != 0:
+        msgs.insert(0, f"以下是本群最近七天的对局：")
 
         await send_msgs(bot, event, msgs)
     else:
-        await matcher.send("本群还没有进行过对局")
+        raise BadRequestError("本群最近七天还没有进行过对局")
 
 
 # ========== 个人未完成对局 ==========
 query_user_uncompleted_games_matcher = on_command("个人未完成对局", priority=5)
 
 require_store_command_args(query_user_uncompleted_games_matcher)
 require_platform_group_id(query_user_uncompleted_games_matcher)
 require_platform_user_id(query_user_uncompleted_games_matcher)
 
 
 @query_user_uncompleted_games_matcher.handle()
 @handle_error()
-async def query_user_uncompleted_games(bot: Bot, event: Event, matcher: Matcher,
+async def query_user_uncompleted_games(bot: Bot, event: Event,
                                        group=GroupDep(),
-                                       user: User = UserDep(lookup_matcher_state=True)):
-    games = await get_games(group.id, user.id, uncompleted_only=True, limit=10, reverse_order=True)
-    if len(games) != 0:
-        msgs = []
-        msgs.append(f"以下是[{await get_user_nickname(bot, user.platform_user_id, group.platform_group_id)}]"
-                    f"的未完成对局：")
-
-        for g in games:
-            msgs.append(await map_game(g, detailed=True))
+                                       user: User = UserDep()):
+    games = await get_games(group.id, user.id, uncompleted_only=True, reverse_order=True)
+    msgs = await map_pagination(games.data, map_game_lite)
+    if games.total != 0:
+        msgs.insert(0, f"以下是[{await get_user_nickname(bot, user.platform_user_id, group.platform_group_id)}]"
+                       f"的未完成对局：")
 
         await send_msgs(bot, event, msgs)
     else:
-        await matcher.send("你还没有未完成的对局")
+        raise BadRequestError("用户没有未完成的对局")
 
 
 # ========== 群未完成对局 ==========
 query_group_uncompleted_games_matcher = on_command("群未完成对局", aliases={"未完成对局"}, priority=5)
 
 require_store_command_args(query_group_uncompleted_games_matcher)
 require_platform_group_id(query_group_uncompleted_games_matcher)
 
 
 @query_group_uncompleted_games_matcher.handle()
 @handle_error()
-async def query_group_uncompleted_games(bot: Bot, event: Event, matcher: Matcher, group=GroupDep()):
-    games = await get_games(group.id, uncompleted_only=True, limit=10, reverse_order=True)
-    if len(games) != 0:
-        msgs = []
-        msgs.append(f"以下是本群的未完成对局：")
-
-        for g in games:
-            msgs.append(await map_game(g, detailed=True))
+async def query_group_uncompleted_games(bot: Bot, event: Event, group=GroupDep()):
+    games = await get_games(group.id, uncompleted_only=True, reverse_order=True)
+    msgs = await map_pagination(games.data, map_game_lite)
+    if games.total != 0:
+        msgs.insert(0, f"以下是本群的未完成对局：")
 
         await send_msgs(bot, event, msgs)
     else:
-        await matcher.send("本群还没有未完成的对局")
+        raise BadRequestError("本群没有未完成的对局")
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 from nonebot import on_command
 from nonebot.internal.matcher import Matcher
 from nonebot.internal.params import Depends
 from nonebot_plugin_session import Session
 
 from .interceptor import handle_error
 from .mapper.game_mapper import map_game
-from .utils.dep import GroupDep, UserDep, UnaryArg, SessionDep, MentionUserArg
-from .utils.message import SplitCommandArgs
-from .utils.parse import parse_int_or_error, try_parse_wind, parse_float_or_error
+from .utils.dep import GroupDep, UserDep, UnaryArg, SessionDep, SplitCommandArgs, SenderUserDep
+from .utils.parse import parse_int_or_error, try_parse_wind, parse_float_or_error, try_parse_game_code
 from ..errors import BadRequestError
 from ..model import Group, User
 from ..model.enums import PlayerAndWind, GameState, Wind
-from ..service import game_service, user_service
+from ..service import game_service
 from ..utils.nonebot import default_cmd_start
 from ..utils.session import get_platform_group_id
 
 group_latest_game_code = TTLCache[str, int](4096, 7200)
 
 
 def GameCodeFromGroupLatest():
@@ -35,15 +34,15 @@
 # =============== 新建对局 ===============
 new_game_matcher = on_command("新建对局", aliases={"新对局"}, priority=5)
 
 
 @new_game_matcher.handle()
 @handle_error()
 async def new_game(matcher: Matcher, player_and_wind=UnaryArg(), session: Session = SessionDep(),
-                   group=GroupDep(), promoter=UserDep()):
+                   group=GroupDep(), promoter=SenderUserDep()):
     if player_and_wind == "四人东":
         player_and_wind = PlayerAndWind.four_men_east
     elif player_and_wind == "四人南":
         player_and_wind = PlayerAndWind.four_men_south
     elif player_and_wind:
         raise BadRequestError("对局类型不合法")
 
@@ -71,16 +70,15 @@
     score = None
     wind = None
 
     for arg in args:
         if arg.type == "text":
             text = arg.data["text"]
             if text.startswith("对局"):
-                game_code = text[len("对局"):]
-                game_code = parse_int_or_error(game_code, "对局编号")
+                game_code = parse_int_or_error(text.removeprefix("对局"), "对局编号")
             elif text.endswith("风"):
                 wind = try_parse_wind(text[:len("风")])
             elif text.endswith("家"):
                 wind = try_parse_wind(text[:len("家")])
             else:
                 pending_wind = try_parse_wind(text)
                 if pending_wind is not None:
@@ -96,21 +94,17 @@
     return RecordArgs(game_code, score, wind)
 
 
 @record_matcher.handle()
 @handle_error()
 async def record(matcher: Matcher,
                  group: Group = GroupDep(),
-                 operator: User = UserDep(),
-                 platform_user_id=MentionUserArg(),
+                 user: User = UserDep(),
+                 operator: User = SenderUserDep(),
                  args=Depends(parse_record_args)):
-    if platform_user_id is None:
-        platform_user_id = operator.platform_user_id
-    user = await user_service.get_user(platform_user_id)
-
     game = await game_service.record_game(args.game_code, group.id, user.id,
                                           args.score, args.wind, operator.id)
 
     msg = await map_game(game)
     msg += '\n\n结算成功'
     if game.state == GameState.invalid_total_point:
         msg += f"\n警告：对局的成绩之和不正确，对此消息回复“{default_cmd_start}结算 <成绩>”指令重新记录你的成绩"
@@ -121,22 +115,18 @@
 revert_record_matcher = on_command("撤销结算对局", aliases={"撤销结算"}, priority=5)
 
 
 @revert_record_matcher.handle()
 @handle_error()
 async def revert_record(matcher: Matcher,
                         group: Group = GroupDep(),
-                        operator: User = UserDep(),
-                        platform_user_id=MentionUserArg(),
+                        user: User = UserDep(),
+                        operator: User = SenderUserDep(),
                         latest_game_code=GameCodeFromGroupLatest(),
-                        game_code=UnaryArg(parser=lambda x: parse_int_or_error(x, '对局编号'))):
-    if platform_user_id is None:
-        platform_user_id = operator.platform_user_id
-    user = await user_service.get_user(platform_user_id)
-
+                        game_code=UnaryArg(parser=try_parse_game_code)):
     if game_code is None:
         game_code = latest_game_code
 
     if game_code is None:
         raise BadRequestError("请指定对局编号")
 
     game = await game_service.revert_record(game_code, group.id, user.id, operator.id)
@@ -160,15 +150,15 @@
                                       game_code=GameCodeFromGroupLatest()):
     point = None
 
     for arg in args:
         if arg.type == "text":
             text = arg.data["text"]
             if text.startswith("对局"):
-                game_code = parse_int_or_error(text[len("对局"):], '对局编号')
+                game_code = parse_int_or_error(text.removeprefix("对局"), "对局编号")
             else:
                 point = text
 
     point = parse_float_or_error(point, 'PT')
 
     if game_code is None:
         raise BadRequestError("请指定对局编号")
@@ -176,37 +166,33 @@
     return SetRecordPointArgs(game_code, point)
 
 
 @set_record_point_matcher.handle()
 @handle_error()
 async def set_record_point(matcher: Matcher,
                            group: Group = GroupDep(),
-                           operator: User = UserDep(),
-                           platform_user_id=MentionUserArg(),
+                           user: User = UserDep(),
+                           operator: User = SenderUserDep(),
                            args: SetRecordPointArgs = Depends(parse_set_record_point_args)):
-    if platform_user_id is None:
-        platform_user_id = operator.platform_user_id
-    user = await user_service.get_user(platform_user_id)
-
     game = await game_service.set_record_point(args.game_code, group.id, user.id,
                                                args.point, operator.id)
 
     msg = await map_game(game)
     msg += '\n\n设置PT成功'
     await matcher.send(msg)
 
 
 # =============== 删除对局 ===============
 delete_game_matcher = on_command("删除对局", priority=5)
 
 
 @delete_game_matcher.handle()
 @handle_error()
-async def delete_game(matcher: Matcher, group: Group = GroupDep(), operator: User = UserDep(),
-                      game_code=UnaryArg(parser=lambda x: parse_int_or_error(x, '对局编号'))):
+async def delete_game(matcher: Matcher, group: Group = GroupDep(), operator: User = SenderUserDep(),
+                      game_code=UnaryArg(parser=try_parse_game_code)):
     if game_code is None:
         raise BadRequestError("请指定对局编号")
 
     await game_service.delete_game(game_code, group.id, operator.id)
 
     await matcher.send(f'成功删除对局{game_code}')
 
@@ -231,15 +217,15 @@
     round = None
     honba = None
 
     for arg in args:
         if arg.type == 'text':
             text = arg.data["text"]
             if text.startswith("对局"):
-                game_code = parse_int_or_error(text[len("对局"):], '对局编号')
+                game_code = parse_int_or_error(text.removeprefix("对局"), "对局编号")
             elif text == '完成' or text == '已完成':
                 completed = True
             else:
                 match_result = re.match(round_honba_pattern, text)
                 if match_result is not None:
                     wind, round, honba = match_result.groups()
 
@@ -255,15 +241,15 @@
         raise BadRequestError("请指定对局进度（”东/南x局y本场“或”完成“）")
 
     return MakeGameProgressArgs(game_code, completed, round, honba)
 
 
 @make_game_progress_matcher.handle()
 @handle_error()
-async def make_game_progress(matcher: Matcher, group: Group = GroupDep(), operator: User = UserDep(),
+async def make_game_progress(matcher: Matcher, group: Group = GroupDep(), operator: User = SenderUserDep(),
                              args: MakeGameProgressArgs = Depends(parse_make_game_progress_args)):
     if not args.completed:
         game = await game_service.make_game_progress(args.game_code,
                                                      args.round,
                                                      args.honba,
                                                      group.id, operator.id)
     else:
@@ -288,15 +274,15 @@
                                       game_code=GameCodeFromGroupLatest()):
     comment = StringIO()
 
     for arg in args:
         if arg.type == 'text':
             text = arg.data["text"]
             if game_code is None and text.startswith("对局"):
-                game_code = parse_int_or_error(text[len("对局"):], '对局编号')
+                game_code = parse_int_or_error(text.removeprefix("对局"), "对局编号")
             else:
                 comment.write(text)
                 comment.write(" ")
 
     comment = comment.getvalue()
     if not comment:
         raise BadRequestError("请输入备注")
@@ -305,15 +291,15 @@
         raise BadRequestError("请指定对局编号")
 
     return SetGameCommentArgs(game_code, comment)
 
 
 @set_game_comment_matcher.handle()
 @handle_error()
-async def set_game_comment(matcher: Matcher, group: Group = GroupDep(), operator: User = UserDep(),
+async def set_game_comment(matcher: Matcher, group: Group = GroupDep(), operator: User = SenderUserDep(),
                            args: SetGameCommentArgs = Depends(parse_set_game_comment_args)):
     game = await game_service.set_game_comment(args.game_code, group.id, args.comment,
                                                operator.id)
 
     msg = await map_game(game)
     msg += "\n\n成功设置对局备注"
     await matcher.send(msg)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,36 +23,36 @@
 require_platform_user_id(query_season_user_trend_matcher)
 
 
 @query_season_user_trend_matcher.handle()
 @handle_error()
 async def query_season_user_trend(bot: Bot, matcher: Matcher, group: Group = GroupDep(),
                                   session: Session = SessionDep(),
-                                  user: User = UserDep(lookup_matcher_state=True),
+                                  user: User = UserDep(),
                                   season: Season = RunningSeasonDep()):
     games = await get_games(group.id, user.id, season.id, limit=10, reverse_order=True, completed_only=True)
 
-    if len(games) != 0:
+    if games.total != 0:
         with StringIO() as sio:
             sio.write(f"用户[{await get_user_nickname(bot, user.platform_user_id, get_platform_group_id(session))}]"
                       f"的最近走势如下：\n")
 
-            for game in games:
+            for game in games.data:
                 record = game.records[0]
                 for r in game.records:
                     if r.user.id == user.id:
                         record = r
 
                 sio.write(f"  {record.rank}位    {record.score}点  "
                           f"({map_point(record.raw_point, record.point_scale)})  "
                           f"对局{game.code}\n")
 
             await matcher.send(sio.getvalue().strip())
     else:
-        raise BadRequestError("你还没有参加过对局")
+        raise BadRequestError("用户还没有参加过对局")
 
 
 # ============ 对战数据 ============
 async def map_game_statistics(game_statistics: GameStatistics, user: User, group: Group) -> str:
     bot = current_bot.get()
     with StringIO() as sio:
         sio.write(f"用户[{await get_user_nickname(bot, user.platform_user_id, group.platform_group_id)}]的对战数据：\n")
@@ -74,15 +74,15 @@
 require_platform_group_id(query_user_statistics_matcher)
 require_platform_user_id(query_user_statistics_matcher)
 
 
 @query_user_statistics_matcher.handle()
 @handle_error()
 async def query_user_statistics(matcher: Matcher, group: Group = GroupDep(),
-                                user: User = UserDep(lookup_matcher_state=True)):
+                                user: User = UserDep()):
     game_statistics = await get_game_statistics(group.id, user.id)
     msg = await map_game_statistics(game_statistics, user, group)
     await matcher.send(msg)
 
 
 # ============ 赛季对战数据 ============
 query_season_user_statistics_matcher = on_command("赛季对战数据", priority=5)
@@ -91,12 +91,12 @@
 require_platform_group_id(query_season_user_statistics_matcher)
 require_platform_user_id(query_season_user_statistics_matcher)
 
 
 @query_season_user_statistics_matcher.handle()
 @handle_error()
 async def query_season_user_statistics(matcher: Matcher, group: Group = GroupDep(),
-                                       user: User = UserDep(lookup_matcher_state=True),
+                                       user: User = UserDep(),
                                        season: Season = SeasonFromUnaryArgOrRunningSeason()):
     game_statistics = await get_season_game_statistics(group.id, user.id, season.id)
     msg = await  map_game_statistics(game_statistics, user, group)
     await matcher.send(msg)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,18 +33,19 @@
         if detailed:
             # 所属赛季：Season Name
             season_name = '无'
             if game.season is not None:
                 season_name = game.season.name
             io.write(f'所属赛季：{season_name}\n')
 
-            io.write(f'创建者：{game.promoter.platform_user_id}\n')
+            io.write(
+                f'创建者：{await get_user_nickname(bot, game.promoter.platform_user_id, game.group.platform_group_id)}\n')
 
         # 状态：未完成
-        io.write(f'状态：{game_state_mapping[GameState(game.state)]}')
+        io.write(f'状态：{game_state_mapping[game.state]}')
         if game.state != GameState.completed:
             sum_score = sum(map(lambda r: r.score, game.records))
             io.write(f"  （合计{sum_score}点）")
         io.write('\n')
 
         if detailed and game.state == GameState.completed:
             io.write(f'完成时间：{map_datetime(game.complete_time)}\n')
@@ -74,7 +75,26 @@
         if game.comment:
             io.write('\n')
             io.write("备注：")
             io.write(game.comment)
             io.write('\n')
 
         return io.getvalue().strip()
+
+
+async def map_game_lite(game: Game) -> str:
+    bot = current_bot.get()
+    with StringIO() as io:
+        # 对局23060101 [已完成]  Player Name(+5)  Player Name(+5)  Player Name(+5)  Player Name(+5)
+        io.write(f"对局{game.code}  ")
+
+        if game.progress is not None:
+            io.write(f"[{map_game_progress(game.progress)}]")
+        else:
+            io.write(f"[{game_state_mapping[game.state]}]")
+
+        for r in sorted(game.records, key=lambda r: r.raw_point, reverse=True):
+            io.write(f"  {await get_user_nickname(bot, r.user.platform_user_id, game.group.platform_group_id)}")
+            if game.state == GameState.completed:
+                io.write(f"({map_point(r.raw_point, r.point_scale)})")
+
+        return io.getvalue().strip()
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from nonebot import on_command
 from nonebot.internal.adapter import Event
 from nonebot.internal.matcher import Matcher
 from nonebot.internal.params import ArgPlainText
 
 from .interceptor import handle_interruption, handle_error
 from .mapper.season_mapper import map_season
-from .utils.dep import GroupDep, UserDep, UnaryArg, RunningSeasonDep
-from .utils.general_handlers import hint_for_question_flow_on_first
+from .utils.dep import GroupDep, UnaryArg, RunningSeasonDep, SenderUserDep, GroupAdminDep
+from .utils.general_handlers import hint_for_question_flow_on_first, require_store_command_args
 from .utils.parse import parse_int_or_reject
 from ..errors import BadRequestError
 from ..model import Group, Season, User, SeasonConfig
 from ..model.enums import SeasonState
 from ..service import season_service
 from ..service.season_service import get_season_by_code, new_season, start_season, finish_season
 
@@ -23,15 +23,16 @@
 
 
 @new_season_matcher.got("code", "赛季代号？")
 @handle_error()
 @handle_interruption()
 async def new_season_got_code(matcher: Matcher,
                               raw_arg=ArgPlainText("code"),
-                              group: Group = GroupDep()):
+                              group: Group = GroupDep(),
+                              group_admin=GroupAdminDep()):
     match_result = re.match(r"[_a-zA-Z]\w*", raw_arg)
     if match_result is None:
         await matcher.reject("赛季代号不合法。请重新输入。（赛季代号只允许包含字母、数字和下划线，且必须以字母或下划线开头）")
 
     season = await get_season_by_code(raw_arg, group.id)
     if season is not None:
         await matcher.reject("该赛季代号已被使用。请重新输入")
@@ -190,30 +191,31 @@
         await matcher.pause("赛季创建成功。是否立刻开启该赛季？(y/n)")
     else:
         await matcher.finish("取消赛季创建")
 
 
 @new_season_matcher.handle()
 @handle_error()
-async def new_season_start(event: Event, matcher: Matcher, operator: User = UserDep()):
+async def new_season_start(event: Event, matcher: Matcher, operator: User = SenderUserDep()):
     if event.get_message().extract_plain_text() == 'y':
         await start_season(matcher.state["season"].id, operator.id)
         await matcher.send("赛季开启成功")
     else:
         await matcher.send(f"稍后可以使用“/开启赛季 {matcher.state['season'].code}”命令开启赛季")
 
 
 # ========== 开启赛季 ==========
 start_season_matcher = on_command("开启赛季", priority=5)
 
 
 @start_season_matcher.handle()
 @handle_error()
 async def start_season_matcher_confirm(matcher: Matcher, group: Group = GroupDep(),
-                                       season_code=UnaryArg()):
+                                       season_code=UnaryArg(),
+                                       group_admin=GroupAdminDep()):
     if season_code is None:
         raise BadRequestError("请指定赛季编号。使用“/新赛季”指令创建赛季")
 
     season = await get_season_by_code(season_code, group.id)
     if season is None:
         raise BadRequestError("找不到该赛季。使用“/新赛季”指令创建赛季")
 
@@ -226,53 +228,55 @@
     else:
         msg += "\n\n确定开启赛季吗？(y/n)"
         await matcher.pause(msg)
 
 
 @start_season_matcher.handle()
 @handle_error()
-async def start_season_end(event: Event, matcher: Matcher, operator: User = UserDep()):
+async def start_season_end(event: Event, matcher: Matcher, operator: User = SenderUserDep()):
     if event.get_message().extract_plain_text() == 'y':
         await season_service.start_season(matcher.state["season"].id, operator.id)
         await matcher.send("赛季开启成功")
     else:
         await matcher.send("取消开启赛季")
 
 
 # ========== 结束赛季 ==========
 finish_season_matcher = on_command("结束赛季", priority=5)
 
 
 @finish_season_matcher.handle()
 @handle_error()
-async def finish_season_confirm(matcher: Matcher, season: Season = RunningSeasonDep()):
+async def finish_season_confirm(matcher: Matcher, season: Season = RunningSeasonDep(),
+                                group_admin=GroupAdminDep()):
     matcher.state["season"] = season
     msg = map_season(season)
     msg += "\n\n结束赛季将删除赛季的所有未完成对局，并且无法再修改赛季的已完成对局。\n确定结束赛季吗？(y/n)"
     await matcher.pause(msg)
 
 
 @finish_season_matcher.handle()
 @handle_error()
-async def finish_season_end(event: Event, matcher: Matcher, operator: User = UserDep()):
+async def finish_season_end(event: Event, matcher: Matcher, operator: User = SenderUserDep()):
     if event.get_message().extract_plain_text() == 'y':
         await finish_season(matcher.state["season"].id, operator.id)
         await matcher.send("赛季结束成功")
     else:
         await matcher.send("取消结束赛季")
 
 
 # ========== 删除赛季 ==========
 remove_season_matcher = on_command("删除赛季", priority=5)
 
 
 @remove_season_matcher.handle()
 @handle_error()
 async def remove_season_confirm(matcher: Matcher, group: Group = GroupDep(),
-                                season_code=UnaryArg()):
+                                season_code=UnaryArg(),
+                                group_admin=GroupAdminDep()):
     if season_code is None:
         raise BadRequestError("请指定赛季编号")
 
     season = await get_season_by_code(season_code, group.id)
     if season is None:
         raise BadRequestError("找不到该赛季")
 
@@ -285,13 +289,13 @@
     else:
         msg += "\n\n确定删除赛季吗？(y/n)"
         await matcher.pause(msg)
 
 
 @remove_season_matcher.handle()
 @handle_error()
-async def remove_season_end(event: Event, matcher: Matcher, operator: User = UserDep()):
+async def remove_season_end(event: Event, matcher: Matcher, operator: User = SenderUserDep()):
     if event.get_message().extract_plain_text() == 'y':
         await season_service.remove_season(matcher.state["season"].id, operator.id)
         await matcher.send("赛季删除成功")
     else:
         await matcher.send("取消删除赛季")
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent
 from nonebot_plugin_gocqhttp_cross_machine_upload_file import upload_file
 
 from .interceptor import handle_error
 from .mapper.season_user_point_csv_mapper import write_season_user_point_change_logs_csv
 from .utils.dep import SeasonFromUnaryArgOrRunningSeason
 from .utils.general_handlers import require_store_command_args, require_platform_group_id
+from ..errors import BadRequestError
 from ..model import Season
 from ..model.enums import SeasonState
 from ..service.season_user_point_service import get_season_user_point_change_logs
 from ..utils.date import encode_date
 
 # ========== 导出榜单 ==========
 export_season_ranking_matcher = on_command("导出榜单", priority=5)
@@ -24,14 +25,17 @@
 
 @export_season_ranking_matcher.handle()
 @handle_error()
 async def export_season_ranking(bot: Bot, event: MessageEvent,
                                 season: Season = SeasonFromUnaryArgOrRunningSeason()):
     logs = await get_season_user_point_change_logs(season.id)
 
+    if len(logs) == 0:
+        raise BadRequestError("还没有用户参与该赛季")
+
     filename = f"赛季榜单 {season.name}"
     if season.state == SeasonState.finished:
         filename += "（已结束）"
     else:
         now = datetime.now(tzlocal.get_localzone())
         filename += f"（截至{encode_date(now)}）"
     filename += ".csv"
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 from nonebot import on_command, Bot
 from nonebot.internal.adapter import Event
 from nonebot.internal.matcher import Matcher
 from nonebot_plugin_session import Session
 
 from .interceptor import handle_error
 from .mapper.season_user_point_mapper import map_season_user_point
-from .utils.dep import UserDep, GroupDep, RunningSeasonDep, SessionDep, UnaryArg
+from .utils.dep import UserDep, GroupDep, RunningSeasonDep, SessionDep, UnaryArg, SenderUserDep, GroupAdminDep
 from .utils.general_handlers import require_store_command_args, require_platform_group_id, require_platform_user_id
 from .utils.parse import parse_float_or_error
 from ..model import Group, User, Season
 from ..platform.get_user_nickname import get_user_nickname
 from ..service.season_user_point_service import reset_season_user_point, change_season_user_point_manually
 from ..utils.session import get_platform_group_id
 
 # ========== 设置用户PT ==========
 set_season_user_point_matcher = on_command("设置用户PT", aliases={"设置用户pt", "设置PT", "设置pt"}, priority=5)
 
 require_store_command_args(set_season_user_point_matcher)
 require_platform_group_id(set_season_user_point_matcher)
-require_platform_user_id(set_season_user_point_matcher, sender_as_default_on_group_message=False)
+require_platform_user_id(set_season_user_point_matcher, use_sender_on_group_message=False)
 
 
 @set_season_user_point_matcher.handle()
 @handle_error()
 async def set_season_user_point_confirm(bot: Bot, matcher: Matcher, session: Session = SessionDep(),
-                                        user: User = UserDep(lookup_matcher_state=True),
-                                        pt=UnaryArg(lookup_matcher_state=True,
-                                                    parser=lambda x: parse_float_or_error(x, 'PT'))):
+                                        user: User = UserDep(use_sender=False),
+                                        pt=UnaryArg(parser=lambda x: parse_float_or_error(x, 'PT')),
+                                        group_admin=GroupAdminDep()):
     await matcher.pause(
         f"确定设置用户[{await get_user_nickname(bot, user.platform_user_id, get_platform_group_id(session))}]"
         f"PT为{pt}吗？(y/n)")
 
 
 @set_season_user_point_matcher.handle()
 @handle_error()
 async def set_season_user_point_end(event: Event, matcher: Matcher,
                                     group: Group = GroupDep(),
-                                    user: User = UserDep(lookup_matcher_state=True),
-                                    operator: User = UserDep(),
+                                    user: User = UserDep(use_sender=False),
+                                    operator: User = SenderUserDep(),
                                     season: Season = RunningSeasonDep(),
-                                    pt=UnaryArg(lookup_matcher_state=True,
-                                                parser=lambda x: parse_float_or_error(x, 'PT'))):
+                                    pt=UnaryArg(parser=lambda x: parse_float_or_error(x, 'PT'))):
     if event.get_message().extract_plain_text() == 'y':
         sup = await change_season_user_point_manually(season.id,
                                                       group.id, user.id,
                                                       pt,
                                                       operator.id)
         msg = await map_season_user_point(sup, season)
         msg += "\n\n设置用户PT成功"
@@ -54,32 +53,33 @@
 
 
 # ========== 重置用户PT ==========
 reset_season_user_point_matcher = on_command("重置用户PT", aliases={"重置用户pt", "重置PT", "重置pt"}, priority=5)
 
 require_store_command_args(reset_season_user_point_matcher)
 require_platform_group_id(reset_season_user_point_matcher)
-require_platform_user_id(reset_season_user_point_matcher, sender_as_default_on_group_message=False)
+require_platform_user_id(reset_season_user_point_matcher, use_sender_on_group_message=False)
 
 
 @reset_season_user_point_matcher.handle()
 @handle_error()
 async def reset_season_user_point_confirm(bot: Bot, matcher: Matcher, session: Session = SessionDep(),
-                                          user: User = UserDep(lookup_matcher_state=True)):
+                                          user: User = UserDep(use_sender=False),
+                                          group_admin=GroupAdminDep()):
     await matcher.pause(
         f"确定重置用户[{await get_user_nickname(bot, user.platform_user_id, get_platform_group_id(session))}]"
         f"PT吗？(y/n)")
 
 
 @reset_season_user_point_matcher.handle()
 @handle_error()
 async def reset_season_user_point_end(event: Event, matcher: Matcher,
                                       group: Group = GroupDep(),
-                                      user: User = UserDep(lookup_matcher_state=True),
-                                      operator: User = UserDep(),
+                                      user: User = UserDep(use_sender=False),
+                                      operator: User = SenderUserDep(),
                                       season: Season = RunningSeasonDep()):
     if event.get_message().extract_plain_text() == 'y':
         await reset_season_user_point(season.id,
                                       group.id, user.id,
                                       operator.id)
         await matcher.send("重置用户PT成功")
     else:
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,32 +76,34 @@
 
     return matcher_type
 
 
 def require_platform_user_id(matcher_type: Type[Matcher], *, dest: str = "platform_user_id",
                              lookup_matcher_state: bool = True,
                              lookup_matcher_state_key: Optional[str] = "command_args_store",
-                             sender_as_default_on_group_message: bool = True):
+                             use_sender_on_group_message: bool = True,
+                             ask_on_group_message: bool = False):
     """
     私聊环境下向用户询问用户号，群聊环境下则使用消息中的艾特或是发送者。保存到matcher.state[dest]
     """
 
     @matcher_type.handle()
     @handle_error()
     async def prepare(matcher: Matcher, session: Session = SessionDep(),
                       mention_user_id=MentionUserArg(lookup_matcher_state=lookup_matcher_state,
                                                      lookup_matcher_state_key=lookup_matcher_state_key)):
         platform_user_id = None
         if lookup_matcher_state_key is not None:
             platform_user_id = mention_user_id
 
-        if sender_as_default_on_group_message:
+        if use_sender_on_group_message:
             platform_group_id = get_platform_group_id(session)
             if platform_group_id is not None:  # 群聊环境
                 platform_user_id = get_platform_user_id(session)
 
         if platform_user_id is not None:
             matcher.state[dest] = platform_user_id
 
-    require_arg(matcher_type, dest, "用户ID", parser=_parse_platform_id)
+    if ask_on_group_message:
+        require_arg(matcher_type, dest, "用户ID", parser=_parse_platform_id)
 
     return matcher_type
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             x = int(raw)
 
         if max is not None and x > max or min is not None and x < min:
             raise ValueError(x)
 
         return x
     except ValueError:
-        comment = []
+        comment = [f"输入的{desc}不合法", f"输入值：{raw}"]
         if min is not None:
             comment.append(f"最小值：{min}")
         if max is not None:
             comment.append(f"最大值：{max}")
         comment = '，'.join(comment)
         if len(comment) != 0:
             comment = f"（{comment}）"
@@ -52,15 +52,15 @@
 def parse_float_or_error(raw: Union[float, int, str, None], desc: str) -> float:
     if not raw:
         raise BadRequestError(f"请指定{desc}")
 
     try:
         return float(raw)
     except ValueError:
-        raise BadRequestError(f"输入的{desc}不合法")
+        raise BadRequestError(f"输入的{desc}不合法，输入值：{raw}")
 
 
 async def parse_float_or_reject(raw: Union[float, int, str, None], desc: str) -> float:
     matcher = current_matcher.get()
 
     try:
         return parse_float_or_error(raw, desc)
@@ -74,7 +74,13 @@
     if text == "南":
         return Wind.south
     if text == "西":
         return Wind.west
     if text == "北":
         return Wind.north
     return None
+
+
+def try_parse_game_code(text: str) -> Optional[int]:
+    if text.startswith("对局"):
+        return parse_int_or_error(text.removeprefix("对局"), "对局编号")
+    return None
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/game.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/game.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from datetime import datetime, timedelta
 from typing import List, Optional, Tuple, overload
 
-from sqlalchemy import update, Select, select
+from sqlalchemy import update, Select, select, func
 from sqlalchemy.orm import selectinload
 
 from .base import Repository
 from .data_model import GameOrm, GameProgressOrm, GameRecordOrm
+from .pagination import Page
 from ..model.enums import GameState
 
 
 class GameRepository(Repository[GameOrm]):
     async def get_by_pk(self, pk: int) -> Optional[GameOrm]:
         stmt = select(GameOrm).where(
             GameOrm.id == pk,
@@ -60,36 +61,42 @@
                   user_id: Optional[int] = ...,
                   season_id: Optional[int] = ...,
                   *, uncompleted_only: bool = False,
                   completed_only: bool = False,
                   offset: Optional[int] = None,
                   limit: Optional[int] = None,
                   reverse_order: bool = False,
-                  time_span: Optional[Tuple[datetime, datetime]] = None) -> List[GameOrm]:
+                  time_span: Optional[Tuple[datetime, datetime]] = None) -> Page[GameOrm]:
         ...
 
     async def get(self, group_id: Optional[int] = None,
                   user_id: Optional[int] = None,
                   season_id: Optional[int] = None,
-                  **kwargs) -> List[GameOrm]:
-        stmt = select(GameOrm)
+                  **kwargs) -> Page[GameOrm]:
+        stmt = select(GameOrm, func.count(GameOrm.id).over().label("total"))
 
         if group_id is not None:
             stmt = stmt.where(GameOrm.group_id == group_id)
 
         if user_id is not None:
             stmt = stmt.join(GameRecordOrm).where(GameRecordOrm.user_id == user_id)
 
         if season_id is not None:
             stmt = stmt.where(GameOrm.season_id == season_id)
 
         stmt = self._build_game_query(stmt, **kwargs)
 
-        result = await self.session.execute(stmt)
-        return [row[0] for row in result]
+        result = (await self.session.execute(stmt)).all()
+
+        if len(result) > 0:
+            data = [row[0] for row in result]
+            total = result[0][1]
+            return Page(data=data, total=total)
+        else:
+            return Page(data=[], total=0)
 
     async def get_progress(self, game_id: int) -> Optional[GameProgressOrm]:
         return await self.session.get(GameProgressOrm, game_id)
 
     async def delete_all_uncompleted_game(self) -> int:
         now = datetime.utcnow()
         one_day_ago = now - timedelta(days=1)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/group.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/season.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/season.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
-from typing import Optional, List, overload, Literal, Tuple, Union
+from typing import Optional, List
 
 from sqlalchemy import update, select, and_, delete, func
 from sqlalchemy.sql.functions import count
 
 from .base import Repository
-from .data_model import GameOrm, GameRecordOrm, SeasonOrm, SeasonUserPointOrm, SeasonUserPointChangeLogOrm
+from .data_model import GameOrm, SeasonOrm, SeasonUserPointOrm, SeasonUserPointChangeLogOrm
 from ..errors import BadRequestError
 from ..model.enums import GameState, SeasonUserPointChangeType
 from ..utils.rank import ranked
 
 
 class SeasonRepository(Repository[SeasonOrm]):
     async def get_by_pk(self, pk: int) -> Optional[SeasonOrm]:
@@ -76,74 +76,27 @@
     async def get_season_user_points(self, season_id: int) -> List[SeasonUserPointOrm]:
         stmt = select(SeasonUserPointOrm).where(
             SeasonUserPointOrm.season_id == season_id
         ).order_by(SeasonUserPointOrm.point.desc())
         sup = (await self.session.execute(stmt)).scalars().all()
         return sup
 
-    @overload
-    async def get_season_user_point_change_logs(self, season_id: Optional[int] = ...,
-                                                user_id: Optional[int] = ...,
-                                                *, offset: Optional[int] = ...,
-                                                limit: Optional[int] = ...,
-                                                reverse_order: bool = ...,
-                                                join_game_and_record: Literal[False] = ...) \
-            -> List[SeasonUserPointChangeLogOrm]:
-        ...
-
-    @overload
-    async def get_season_user_point_change_logs(self, season_id: Optional[int] = ...,
-                                                user_id: Optional[int] = ...,
-                                                *, offset: Optional[int] = ...,
-                                                limit: Optional[int] = ...,
-                                                reverse_order: bool = ...,
-                                                join_game_and_record: Literal[True] = ...) \
-            -> List[Tuple[SeasonUserPointChangeLogOrm, GameOrm, GameRecordOrm]]:
-        ...
-
     async def get_season_user_point_change_logs(self, season_id: Optional[int] = None,
-                                                user_id: Optional[int] = None,
-                                                *, offset: Optional[int] = None,
-                                                limit: Optional[int] = None,
-                                                reverse_order: bool = False,
-                                                join_game_and_record: bool = False) \
-            -> Union[
-                List[SeasonUserPointChangeLogOrm],
-                List[Tuple[SeasonUserPointChangeLogOrm, GameOrm, GameRecordOrm]]
-            ]:
-        if not join_game_and_record:
-            stmt = select(SeasonUserPointChangeLogOrm)
-        else:
-            stmt = (select(SeasonUserPointChangeLogOrm, GameOrm, GameRecordOrm)
-                    .join_from(SeasonUserPointChangeLogOrm, GameOrm,
-                               SeasonUserPointChangeLogOrm.related_game_id == GameOrm.id)
-                    .join_from(SeasonUserPointChangeLogOrm, GameRecordOrm,
-                               and_(
-                                   SeasonUserPointChangeLogOrm.related_game_id == GameRecordOrm.game_id,
-                                   SeasonUserPointChangeLogOrm.user_id == GameRecordOrm.user_id
-                               )))
+                                                user_id: Optional[int] = None) -> List[SeasonUserPointChangeLogOrm]:
+        stmt = select(SeasonUserPointChangeLogOrm, func.count(SeasonUserPointChangeLogOrm.id).over().label("total"))
 
         if season_id is not None:
             stmt = stmt.where(SeasonUserPointChangeLogOrm.season_id == season_id)
 
         if user_id is not None:
             stmt = stmt.where(SeasonUserPointChangeLogOrm.user_id == user_id)
 
-        if reverse_order:
-            stmt = stmt.order_by(SeasonUserPointChangeLogOrm.id.desc())
-        else:
-            stmt = stmt.order_by(SeasonUserPointChangeLogOrm.id)
-
-        stmt = stmt.offset(offset).limit(limit)
-
         result = (await self.session.execute(stmt)).all()
-        if join_game_and_record:
-            return [(a, b, c) for (a, b, c) in result]
-        else:
-            return [x for (x,) in result]
+        data = [row[0] for row in result]
+        return data
 
     async def change_season_user_point_manually(self, season_id: int,
                                                 user_id: int,
                                                 point: float) -> SeasonUserPointOrm:
         season = await self.get_by_pk(season_id)
         sup = await self.get_season_user_point(season_id, user_id, insert_on_missing=True)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/user.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .mapper import map_game
 from ..errors import BadRequestError
 from ..model import Game, GameStatistics
 from ..model.enums import GameState, PlayerAndWind, Wind, SeasonState
 from ..repository import data_source
 from ..repository.data_model import GroupOrm, GameOrm, GameRecordOrm, GameProgressOrm, SeasonOrm
 from ..repository.game import GameRepository
+from ..repository.pagination import Page
 from ..repository.season import SeasonRepository
 from ..utils.date import encode_date
 from ..utils.integer import count_digit
 
 
 @scheduler.scheduled_job("cron", hour="*/2", id="delete_all_uncompleted_game")
 async def _delete_all_uncompleted_game():
@@ -262,15 +263,15 @@
     await _ensure_permission(game, group_id, operator_user_id)
 
     for r in game.records:
         if r.user_id == user_id:
             record = r
             break
     else:
-        raise BadRequestError("你还没有记录过这场对局")
+        raise BadRequestError("用户还没有记录过这场对局")
 
     if game.state == GameState.completed and game.season_id:
         await season_repo.revert_season_user_point_by_game(game)
 
     game.state = GameState.uncompleted
     game.records.remove(record)
     await session.delete(record)
@@ -337,14 +338,15 @@
         session.add(progress)
 
     progress.round = round
     progress.honba = honba
 
     game.update_time = datetime.utcnow()
     await session.commit()
+    await session.refresh(game)  # 刷新一下，保证能拿到game.progress
     return await map_game(game, session)
 
 
 async def remove_game_progress(game_code: int, group_id: int):
     session = data_source.session()
 
     game_repo = GameRepository(session)
@@ -430,24 +432,26 @@
 @overload
 async def get_games(group_id: int, user_id: Optional[int] = None, season_id: Optional[int] = None,
                     *, uncompleted_only: bool = ...,
                     completed_only: bool = ...,
                     offset: Optional[int] = ...,
                     limit: Optional[int] = ...,
                     reverse_order: bool = ...,
-                    time_span: Optional[Tuple[datetime, datetime]] = ...) -> List[Game]:
+                    time_span: Optional[Tuple[datetime, datetime]] = ...) -> Page[Game]:
     ...
 
 
 async def get_games(group_id: int, user_id: Optional[int] = None, season_id: Optional[int] = None, **kwargs) -> \
-        List[Game]:
+        Page[Game]:
     session = data_source.session()
     game_repo = GameRepository(session)
     games = await game_repo.get(group_id, user_id, season_id, **kwargs)
-    return [await map_game(g, session) for g in games]
+
+    data = [await map_game(g, session) for g in games.data]
+    return Page(data=data, total=games.total)
 
 
 def _get_game_statistics_by_games(games: List[GameOrm], user_id: int,
                                   is_same_season: bool = False) -> GameStatistics:
     if len(games) == 0:
         raise BadRequestError("你还没有进行对局")
 
@@ -495,23 +499,23 @@
 
 
 async def get_game_statistics(group_id: int, user_id: int):
     session = data_source.session()
 
     game_repo = GameRepository(session)
     games = await game_repo.get(group_id, user_id, completed_only=True)
-    return _get_game_statistics_by_games(games, user_id)
+    return _get_game_statistics_by_games(games.data, user_id)
 
 
 async def get_season_game_statistics(group_id: int, user_id: int, season_id: int):
     session = data_source.session()
 
     season = await session.get(SeasonOrm, season_id)
 
     game_repo = GameRepository(session)
     games = await game_repo.get(group_id, user_id, season.id, completed_only=True)
-    return _get_game_statistics_by_games(games, user_id, is_same_season=True)
+    return _get_game_statistics_by_games(games.data, user_id, is_same_season=True)
 
 
 __all__ = ("new_game", "delete_game", "record_game", "revert_record", "set_record_point",
            "make_game_progress", "remove_game_progress",
            "delete_uncompleted_season_games")
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional, List
 
 from .group_service import is_group_admin
 from .mapper import map_season_user_point, map_season_user_point_change_log
 from ..errors import BadRequestError
 from ..model import SeasonUserPoint, SeasonUserPointChangeLog
 from ..repository import data_source
+from ..repository.pagination import Page
 from ..repository.season import SeasonRepository
 
 
 async def get_season_user_point(season_id: int, user_id: int) -> Optional[SeasonUserPoint]:
     session = data_source.session()
     repo = SeasonRepository(session)
     sup = await repo.get_season_user_point(season_id, user_id)
@@ -31,22 +32,18 @@
         x.rank = i + 1
         x.total = len(sups)
 
     return sups
 
 
 async def get_season_user_point_change_logs(season_id: Optional[int] = None,
-                                            user_id: Optional[int] = None,
-                                            *, offset: Optional[int] = None,
-                                            limit: Optional[int] = None,
-                                            reverse_order: bool = False) -> List[SeasonUserPointChangeLog]:
+                                            user_id: Optional[int] = None) -> List[SeasonUserPointChangeLog]:
     session = data_source.session()
     repo = SeasonRepository(session)
-    logs = await repo.get_season_user_point_change_logs(season_id, user_id, offset=offset, limit=limit,
-                                                        reverse_order=reverse_order)
+    logs = await repo.get_season_user_point_change_logs(season_id, user_id)
     logs = [await map_season_user_point_change_log(x, session) for x in logs]
     return logs
 
 
 async def reset_season_user_point(season_id: int,
                                   group_id: int,
                                   user_id: int,
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/session.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a1/PKG-INFO` & `nonebot_plugin_mahjong_scoreboard-0.4.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mahjong-scoreboard
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: 日麻寄分器（NoneBot插件）
 Home-page: https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mahjong-scoreboard Version: 0.4.0a1
+Metadata-Version: 2.1 Name: nonebot-plugin-mahjong-scoreboard Version: 0.4.0a2
 Summary: æ¥éº»å¯åå¨ï¼NoneBotæä»¶ï¼ Home-page: https://github.com/
 ssttkkl/nonebot-plugin-mahjong-scoreboard License: MIT Author: ssttkkl Author-
 email: huang.wen.long@hotmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: aiosqlite (>=0.17,<0.19) Requires-Dist:
```

