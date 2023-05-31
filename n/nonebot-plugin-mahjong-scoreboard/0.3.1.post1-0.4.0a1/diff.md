# Comparing `tmp/nonebot_plugin_mahjong_scoreboard-0.3.1.post1.tar.gz` & `tmp/nonebot_plugin_mahjong_scoreboard-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mahjong_scoreboard-0.3.1.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_mahjong_scoreboard-0.4.0a1.tar", max compression
```

## Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1.tar` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1.tar`

### file list

```diff
@@ -1,61 +1,67 @@
--rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421764 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/LICENSE
--rw-r--r--   0        0        0      938 2023-05-07 03:46:59.348863 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/pyproject.toml
--rw-r--r--   0        0        0     6759 2023-05-07 03:20:47.530795 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/README.MD
--rw-r--r--   0        0        0     2090 2023-04-04 02:00:50.079979 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/__init__.py
--rw-r--r--   0        0        0      347 2023-03-13 11:15:04.245799 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/config.py
--rw-r--r--   0        0        0      287 2023-03-13 11:15:04.246316 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/__init__.py
--rw-r--r--   0        0        0      489 2022-10-29 10:31:10.715954 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/context.py
--rw-r--r--   0        0        0     3647 2023-03-01 06:19:33.483226 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py
--rw-r--r--   0        0        0     7291 2023-03-13 11:15:04.246837 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py
--rw-r--r--   0        0        0    14581 2023-03-13 11:15:04.247882 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py
--rw-r--r--   0        0        0     5417 2023-05-07 03:20:47.531830 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py
--rw-r--r--   0        0        0     7254 2023-03-13 11:15:04.249448 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/general_handlers.py
--rw-r--r--   0        0        0      439 2022-10-29 12:00:29.945522 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py
--rw-r--r--   0        0        0     1160 2023-03-01 06:35:10.159635 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_error_impl.py
--rw-r--r--   0        0        0      519 2022-10-25 08:26:38.853725 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_interruption_impl.py
--rw-r--r--   0        0        0     1549 2023-05-07 03:44:28.905567 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py
--rw-r--r--   0        0        0     2770 2023-03-13 11:15:04.250961 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py
--rw-r--r--   0        0        0     3722 2023-03-13 11:15:04.251961 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py
--rw-r--r--   0        0        0     2669 2023-05-07 03:45:01.376945 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_statistics_mapper.py
--rw-r--r--   0        0        0     2494 2023-03-13 11:15:04.252961 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py
--rw-r--r--   0        0        0     3086 2023-03-01 06:19:33.488463 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py
--rw-r--r--   0        0        0     3027 2023-03-13 11:15:04.253961 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py
--rw-r--r--   0        0        0    13761 2023-03-13 11:15:04.254961 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py
--rw-r--r--   0        0        0     2811 2023-03-13 11:15:04.255960 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py
--rw-r--r--   0        0        0     2807 2023-03-01 06:19:33.490557 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py
--rw-r--r--   0        0        0     5297 2023-05-07 03:20:47.532347 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py
--rw-r--r--   0        0        0     3427 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py
--rw-r--r--   0        0        0        0 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/__init__.py
--rw-r--r--   0        0        0     1022 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py
--rw-r--r--   0        0        0     2519 2023-03-13 11:15:04.258743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py
--rw-r--r--   0        0        0     1708 2023-03-13 11:15:04.258743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/send_messages.py
--rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228228 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/errors.py
--rw-r--r--   0        0        0        0 2022-10-11 14:30:16.137278 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py
--rw-r--r--   0        0        0      492 2022-10-25 11:55:32.743202 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/enums.py
--rw-r--r--   0        0        0      251 2023-05-07 03:20:47.949666 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/game_statistics.py
--rw-r--r--   0        0        0       39 2023-03-13 11:15:04.259743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/__init__.py
--rw-r--r--   0        0        0      129 2023-03-13 11:15:04.259743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/__init__.py
--rw-r--r--   0        0        0     2014 2023-03-13 13:49:53.073496 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/metainfo.py
--rw-r--r--   0        0        0      653 2023-03-13 11:15:04.261743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/__init__.py
--rw-r--r--   0        0        0      255 2023-03-13 11:15:04.261743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/v1_to_v2.py
--rw-r--r--   0        0        0      584 2023-04-04 02:00:50.080978 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/src.py
--rw-r--r--   0        0        0     3842 2023-05-07 03:44:12.878318 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/game.py
--rw-r--r--   0        0        0      876 2023-03-13 11:15:04.263743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/group.py
--rw-r--r--   0        0        0     3819 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/season.py
--rw-r--r--   0        0        0        0 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/__init__.py
--rw-r--r--   0        0        0      522 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/userdict.py
--rw-r--r--   0        0        0      461 2023-03-13 11:15:04.265743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/user.py
--rw-r--r--   0        0        0        0 2022-10-11 14:02:12.038461 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/__init__.py
--rw-r--r--   0        0        0    19271 2023-05-07 03:44:45.192491 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py
--rw-r--r--   0        0        0     2196 2023-03-13 11:15:04.266743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py
--rw-r--r--   0        0        0     3736 2023-03-01 06:19:33.494591 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py
--rw-r--r--   0        0        0    10068 2023-03-13 13:34:40.919314 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py
--rw-r--r--   0        0        0      582 2023-03-01 06:19:33.495592 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py
--rw-r--r--   0        0        0        0 2022-10-25 10:53:45.022120 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/__init__.py
--rw-r--r--   0        0        0      288 2022-10-25 10:55:21.893872 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/date.py
--rw-r--r--   0        0        0     1240 2022-10-25 10:57:00.084086 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py
--rw-r--r--   0        0        0      101 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/nonebot.py
--rw-r--r--   0        0        0      482 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/rank.py
--rw-r--r--   0        0        0      256 2023-02-24 10:26:11.257181 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/upload_file.py
--rw-r--r--   0        0        0      761 2023-03-13 11:15:04.268743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py
--rw-r--r--   0        0        0     7624 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421764 nonebot_plugin_mahjong_scoreboard-0.4.0a1/LICENSE
+-rw-r--r--   0        0        0     1054 2023-05-31 16:17:17.191384 nonebot_plugin_mahjong_scoreboard-0.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     6759 2023-05-07 03:20:47.530795 nonebot_plugin_mahjong_scoreboard-0.4.0a1/README.MD
+-rw-r--r--   0        0        0     2335 2023-05-31 16:17:02.523326 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-31 16:17:02.544324 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/config.py
+-rw-r--r--   0        0        0      287 2023-03-13 11:15:04.246316 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/__init__.py
+-rw-r--r--   0        0        0     2373 2023-05-31 13:53:36.752099 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py
+-rw-r--r--   0        0        0     5805 2023-05-31 12:49:29.901146 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py
+-rw-r--r--   0        0        0    11539 2023-05-31 12:49:29.911147 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py
+-rw-r--r--   0        0        0     4936 2023-05-31 13:38:31.503444 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py
+-rw-r--r--   0        0        0     1404 2023-05-31 07:27:37.121738 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py
+-rw-r--r--   0        0        0     1549 2023-05-07 03:44:28.905567 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py
+-rw-r--r--   0        0        0     2443 2023-05-31 13:06:45.874125 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py
+-rw-r--r--   0        0        0     2895 2023-05-31 07:27:37.122737 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py
+-rw-r--r--   0        0        0     1947 2023-05-31 07:27:37.123736 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py
+-rw-r--r--   0        0        0     2873 2023-05-31 13:38:31.556446 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py
+-rw-r--r--   0        0        0      928 2023-05-31 07:27:37.124738 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py
+-rw-r--r--   0        0        0    11888 2023-05-31 12:29:56.485530 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py
+-rw-r--r--   0        0        0     1787 2023-05-31 13:38:31.575444 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py
+-rw-r--r--   0        0        0     1705 2023-05-31 13:46:09.661196 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py
+-rw-r--r--   0        0        0     4498 2023-05-31 12:49:29.906148 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py
+-rw-r--r--   0        0        0     3134 2023-05-31 13:38:31.546447 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/__init__.py
+-rw-r--r--   0        0        0     5289 2023-05-31 14:11:42.691560 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/dep.py
+-rw-r--r--   0        0        0     4232 2023-05-31 12:10:39.999248 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py
+-rw-r--r--   0        0        0     1070 2023-05-31 11:56:26.489690 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py
+-rw-r--r--   0        0        0     2519 2023-03-13 11:15:04.258743 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py
+-rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228228 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/errors.py
+-rw-r--r--   0        0        0     2185 2023-05-31 13:38:31.528445 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py
+-rw-r--r--   0        0        0      492 2022-10-25 11:55:32.743202 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/model/enums.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:27:37.128738 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/__init__.py
+-rw-r--r--   0        0        0     1218 2023-05-31 13:50:13.726888 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py
+-rw-r--r--   0        0        0     1287 2023-05-31 13:06:45.863127 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py
+-rw-r--r--   0        0        0      755 2023-05-31 12:07:55.000532 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py
+-rw-r--r--   0        0        0      772 2023-05-31 07:27:37.130736 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py
+-rw-r--r--   0        0        0     1705 2023-05-31 13:51:24.924727 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py
+-rw-r--r--   0        0        0      928 2023-05-31 16:16:01.038694 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py
+-rw-r--r--   0        0        0      122 2023-05-31 07:27:37.130736 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/__init__.py
+-rw-r--r--   0        0        0     1155 2023-05-31 07:27:37.131737 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py
+-rw-r--r--   0        0        0      258 2023-05-31 16:16:01.029716 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/data_source.py
+-rw-r--r--   0        0        0     2022 2023-05-31 07:27:37.132737 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py
+-rw-r--r--   0        0        0      163 2023-05-31 07:27:37.132737 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/__init__.py
+-rw-r--r--   0        0        0      263 2023-05-31 07:27:37.133737 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v1_to_v2.py
+-rw-r--r--   0        0        0     2523 2023-05-31 07:27:37.133737 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py
+-rw-r--r--   0        0        0      399 2023-05-31 07:27:37.134736 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/base.py
+-rw-r--r--   0        0        0     7261 2023-05-31 12:28:17.427163 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py
+-rw-r--r--   0        0        0     4184 2023-05-31 12:27:53.600829 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/game.py
+-rw-r--r--   0        0        0      797 2023-05-31 12:27:53.584832 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/group.py
+-rw-r--r--   0        0        0    11415 2023-05-31 12:27:53.595831 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/season.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:27:37.135740 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/types/__init__.py
+-rw-r--r--   0        0        0      510 2023-05-31 07:27:37.136738 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/types/pydantic.py
+-rw-r--r--   0        0        0      736 2023-05-31 12:27:53.606829 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/user.py
+-rw-r--r--   0        0        0        0 2022-10-11 14:02:12.038461 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/__init__.py
+-rw-r--r--   0        0        0    18143 2023-05-31 16:17:02.535329 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py
+-rw-r--r--   0        0        0     1027 2023-05-31 12:27:53.572832 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py
+-rw-r--r--   0        0        0     4122 2023-05-31 13:43:41.683542 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py
+-rw-r--r--   0        0        0     4128 2023-05-31 12:27:53.612405 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py
+-rw-r--r--   0        0        0     3149 2023-05-31 13:41:23.034657 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py
+-rw-r--r--   0        0        0      356 2023-05-31 11:33:58.053326 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py
+-rw-r--r--   0        0        0        0 2022-10-25 10:53:45.022120 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/__init__.py
+-rw-r--r--   0        0        0      288 2022-10-25 10:55:21.893872 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/date.py
+-rw-r--r--   0        0        0     1240 2022-10-25 10:57:00.084086 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py
+-rw-r--r--   0        0        0      101 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/nonebot.py
+-rw-r--r--   0        0        0      482 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/rank.py
+-rw-r--r--   0        0        0      758 2023-05-31 13:06:45.885125 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/session.py
+-rw-r--r--   0        0        0      761 2023-03-13 11:15:04.268743 nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py
+-rw-r--r--   0        0        0     7733 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.4.0a1/PKG-INFO
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/LICENSE` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/pyproject.toml` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 [tool.poetry]
 name = "nonebot-plugin-mahjong-scoreboard"
-version = "0.3.1.post1"
+version = "0.4.0a1"
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
 nonebot2 = "^2.0.0rc4"
 nonebot-adapter-onebot = "^2.2.2"
-nonebot-plugin-sqlalchemy = "^0.2.0"
+nonebot_plugin_apscheduler = "^0.2.0"
+nonebot-plugin-sqlalchemy = "^0.2.1"
+nonebot-plugin-session = "^0.0.3"
+nonebot-plugin-gocqhttp-cross-machine-upload-file = "^0.1.5"
 aiosqlite = ">=0.17,<0.19"
 tzlocal = "^4.2"
-nonebot_plugin_apscheduler = "^0.2.0"
 cachetools = "^5.2.0"
-nonebot-plugin-gocqhttp-cross-machine-upload-file = "^0.1.4"
+nonebot-plugin-localstore = "^0.4.1"
 
 [tool.poetry.group.dev.dependencies]
+nonebot2 = { extras = ["httpx", "fastapi"], version = "^2.0.0rc3" }
+nonebot-adapter-qqguild = "^0.2.2"
 nonebug = "^0.2.1"
 flake8 = "^5.0.4"
-nonebot2 = {extras = ["fastapi"], version = "^2.0.0rc3"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/README.MD` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/README.MD`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 """
 nonebot-plugin-mahjong-scoreboard
 
 @Author         : ssttkkl
 @License        : MIT
 @GitHub         : https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard
 """
+from nonebot import require
+
+require("nonebot_plugin_localstore")
+require("nonebot_plugin_session")
+require("nonebot_plugin_sqlalchemy")
+require("nonebot_plugin_apscheduler")
+require("nonebot_plugin_gocqhttp_cross_machine_upload_file")
+
 from .utils.nonebot import default_cmd_start
 
 help_text = f"""
 对局：
 - {default_cmd_start}新建对局 [四人南|四人东]
 - {default_cmd_start}结算对局 <成绩> [对局<编号>] [@<用户>] [<自风>]
 - {default_cmd_start}撤销结算对局 [对局<编号>] [@<用户>]
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,163 +1,144 @@
-from datetime import date, timedelta, datetime, time
+from datetime import datetime, date, timedelta, time
 
-from nonebot import on_command
-from nonebot.adapters.onebot.v11 import Bot, Message, MessageSegment, MessageEvent
+from nonebot import on_command, Bot
+from nonebot.internal.adapter import Event
 from nonebot.internal.matcher import Matcher
 
-from nonebot_plugin_mahjong_scoreboard.controller.context import save_context
-from nonebot_plugin_mahjong_scoreboard.controller.general_handlers import require_parse_unary_at_arg, \
-    require_game_code_from_context, require_parse_unary_integer_arg, require_group_binding_qq, require_user_binding_qq
-from nonebot_plugin_mahjong_scoreboard.controller.interceptor import general_interceptor
-from nonebot_plugin_mahjong_scoreboard.controller.mapper.game_mapper import map_game
-from nonebot_plugin_mahjong_scoreboard.controller.utils.send_messages import send_msgs
-from nonebot_plugin_mahjong_scoreboard.errors import BadRequestError
-from nonebot_plugin_mahjong_scoreboard.service import group_service, game_service
-from nonebot_plugin_mahjong_scoreboard.service.group_service import get_group_by_binding_qq
-from nonebot_plugin_mahjong_scoreboard.service.user_service import get_user_by_binding_qq
+from .interceptor import handle_error
+from .mapper.game_mapper import map_game
+from .utils.dep import GroupDep, UnaryArg, UserDep
+from .utils.general_handlers import require_store_command_args, require_platform_group_id, require_platform_user_id
+from .utils.parse import parse_int_or_error
+from ..errors import BadRequestError
+from ..model import Group, User
+from ..platform.get_user_nickname import get_user_nickname
+from ..platform.send_messages import send_msgs
+from ..service import game_service
+from ..service.game_service import get_games
 
 # =============== 查询对局 ===============
 query_by_code_matcher = on_command("查询对局", aliases={"对局"}, priority=5)
 
-require_game_code_from_context(query_by_code_matcher)
-require_parse_unary_integer_arg(query_by_code_matcher, "game_code")
-require_group_binding_qq(query_by_code_matcher)
+require_store_command_args(query_by_code_matcher)
+require_platform_group_id(query_by_code_matcher)
 
 
 @query_by_code_matcher.handle()
-@general_interceptor(query_by_code_matcher)
-async def query_by_code(matcher: Matcher):
-    game_code = matcher.state.get("game_code", None)
+@handle_error()
+async def query_by_code(matcher: Matcher, group: Group = GroupDep(),
+                        game_code=UnaryArg(lookup_matcher_state=True, parser=lambda x: parse_int_or_error(x, '对局编号'))):
     if game_code is None:
         raise BadRequestError("请指定对局编号")
 
-    group = await group_service.get_group_by_binding_qq(matcher.state["binding_qq"])
-    game = await game_service.get_game_by_code(game_code, group)
+    game = await game_service.get_game(game_code, group.id)
     if game is None:
         raise BadRequestError("未找到指定对局")
 
     msg = await map_game(game, detailed=True)
-    send_result = await matcher.send(msg)
-    save_context(send_result["message_id"], game_code=game.code)
+    await matcher.send(msg)
 
 
 # ========== 个人最近对局 ==========
-query_user_recent_games_matcher = on_command("个人最近对局", aliases={"最近对局"}, priority=5)
+query_user_recent_games_matcher = on_command("个人最近对局", priority=5)
 
-require_parse_unary_at_arg(query_user_recent_games_matcher, "user_binding_qq")
-require_group_binding_qq(query_user_recent_games_matcher)
-require_user_binding_qq(query_user_recent_games_matcher)
+require_store_command_args(query_user_recent_games_matcher)
+require_platform_group_id(query_user_recent_games_matcher)
+require_platform_user_id(query_user_recent_games_matcher)
 
 
 @query_user_recent_games_matcher.handle()
-@general_interceptor(query_user_recent_games_matcher)
-async def query_user_recent_games(bot: Bot, event: MessageEvent, matcher: Matcher):
-    group_binding_qq = matcher.state["binding_qq"]
-    user_binding_qq = matcher.state["user_binding_qq"]
-
-    group = await get_group_by_binding_qq(group_binding_qq)
-    user = await get_user_by_binding_qq(user_binding_qq)
-
+@handle_error()
+async def query_user_recent_games(bot: Bot, event: Event, matcher: Matcher,
+                                  group: Group = GroupDep(),
+                                  user: User = UserDep(lookup_matcher_state=True)):
     end_time = datetime.combine(date.today() + timedelta(days=1), time())
     start_time = datetime.combine(end_time - timedelta(days=7), time())
 
-    games = await game_service.get_games(group, user, limit=30, reverse_order=True, time_span=(start_time, end_time))
+    games = await get_games(group.id, user.id, limit=5, reverse_order=True, time_span=(start_time, end_time))
     if len(games) != 0:
-        member_info = await bot.get_group_member_info(group_id=group.binding_qq, user_id=user.binding_qq)
-        header = Message([
-            MessageSegment.text("以下是"),
-            MessageSegment("at", {"qq": user.binding_qq, "name": member_info["nickname"]}),
-            MessageSegment.text("的最近对局")
-        ])
-        messages = [header]
+        msgs = []
+        msgs.append(f"以下是[{await get_user_nickname(bot, platform_user_id, group.platform_group_id)}]"
+                    f"的最近对局：")
+
         for g in games:
-            messages.append(await map_game(g, detailed=True))
+            msgs.append(await map_game(g, detailed=True))
 
-        await send_msgs(bot, event, messages)
+        await send_msgs(bot, event, msgs)
     else:
         await matcher.send("你还没有进行过对局")
 
 
 # ========== 群最近对局 ==========
-query_group_recent_games_matcher = on_command("群最近对局", priority=5)
+query_group_recent_games_matcher = on_command("群最近对局", aliases={"最近对局"}, priority=5)
 
-require_group_binding_qq(query_group_recent_games_matcher)
+require_store_command_args(query_group_recent_games_matcher)
+require_platform_group_id(query_group_recent_games_matcher)
 
 
 @query_group_recent_games_matcher.handle()
-@general_interceptor(query_group_recent_games_matcher)
-async def query_group_recent_games(bot: Bot, event: MessageEvent, matcher: Matcher):
-    group = await get_group_by_binding_qq(matcher.state["binding_qq"])
-
+@handle_error()
+async def query_group_recent_games(bot: Bot, event: Event, matcher: Matcher, group=GroupDep()):
     end_time = datetime.combine(date.today() + timedelta(days=1), time())
     start_time = datetime.combine(end_time - timedelta(days=7), time())
 
-    games = await game_service.get_games(group, limit=30, reverse_order=True, time_span=(start_time, end_time))
+    games = await get_games(group.id, limit=5, reverse_order=True, time_span=(start_time, end_time))
     if len(games) != 0:
-        header = Message(MessageSegment.text("以下是本群的最近对局"))
-        messages = [header]
+        msgs = []
+        msgs.append(f"以下是本群的最近对局：")
+
         for g in games:
-            messages.append(await map_game(g, detailed=True))
+            msgs.append(await map_game(g, detailed=True))
 
-        await send_msgs(bot, event, messages)
+        await send_msgs(bot, event, msgs)
     else:
         await matcher.send("本群还没有进行过对局")
 
 
 # ========== 个人未完成对局 ==========
-query_user_uncompleted_games_matcher = on_command("个人未完成对局", aliases={"未完成对局"}, priority=5)
+query_user_uncompleted_games_matcher = on_command("个人未完成对局", priority=5)
 
-require_parse_unary_at_arg(query_user_uncompleted_games_matcher, "user_binding_qq")
-require_group_binding_qq(query_user_uncompleted_games_matcher)
-require_user_binding_qq(query_user_uncompleted_games_matcher)
+require_store_command_args(query_user_uncompleted_games_matcher)
+require_platform_group_id(query_user_uncompleted_games_matcher)
+require_platform_user_id(query_user_uncompleted_games_matcher)
 
 
 @query_user_uncompleted_games_matcher.handle()
-@general_interceptor(query_user_uncompleted_games_matcher)
-async def query_user_uncompleted_games(bot: Bot, event: MessageEvent, matcher: Matcher):
-    group_binding_qq = matcher.state["binding_qq"]
-    user_binding_qq = matcher.state["user_binding_qq"]
-
-    group = await get_group_by_binding_qq(group_binding_qq)
-    user = await get_user_by_binding_qq(user_binding_qq)
-
-    games = await game_service.get_games(group, user, uncompleted_only=True, limit=30, reverse_order=True)
+@handle_error()
+async def query_user_uncompleted_games(bot: Bot, event: Event, matcher: Matcher,
+                                       group=GroupDep(),
+                                       user: User = UserDep(lookup_matcher_state=True)):
+    games = await get_games(group.id, user.id, uncompleted_only=True, limit=10, reverse_order=True)
     if len(games) != 0:
-        member_info = await bot.get_group_member_info(group_id=group.binding_qq, user_id=user.binding_qq)
-        header = Message([
-            MessageSegment.text("以下是"),
-            MessageSegment("at", {"qq": user.binding_qq, "name": member_info["nickname"]}),
-            MessageSegment.text("的未完成对局")
-        ])
+        msgs = []
+        msgs.append(f"以下是[{await get_user_nickname(bot, user.platform_user_id, group.platform_group_id)}]"
+                    f"的未完成对局：")
 
-        messages = [header]
         for g in games:
-            messages.append(await map_game(g, detailed=True))
+            msgs.append(await map_game(g, detailed=True))
 
-        await send_msgs(bot, event, messages)
+        await send_msgs(bot, event, msgs)
     else:
         await matcher.send("你还没有未完成的对局")
 
 
 # ========== 群未完成对局 ==========
-query_group_uncompleted_games_matcher = on_command("群未完成对局", priority=5)
+query_group_uncompleted_games_matcher = on_command("群未完成对局", aliases={"未完成对局"}, priority=5)
 
-require_group_binding_qq(query_group_uncompleted_games_matcher)
+require_store_command_args(query_group_uncompleted_games_matcher)
+require_platform_group_id(query_group_uncompleted_games_matcher)
 
 
 @query_group_uncompleted_games_matcher.handle()
-@general_interceptor(query_group_uncompleted_games_matcher)
-async def query_group_uncompleted_games(bot: Bot, event: MessageEvent, matcher: Matcher):
-    group_binding_qq = matcher.state["binding_qq"]
-
-    group = await get_group_by_binding_qq(group_binding_qq)
-
-    games = await game_service.get_games(group, uncompleted_only=True, limit=30, reverse_order=True)
+@handle_error()
+async def query_group_uncompleted_games(bot: Bot, event: Event, matcher: Matcher, group=GroupDep()):
+    games = await get_games(group.id, uncompleted_only=True, limit=10, reverse_order=True)
     if len(games) != 0:
-        header = Message(MessageSegment.text("以下是本群的未完成对局"))
-        messages = [header]
+        msgs = []
+        msgs.append(f"以下是本群的未完成对局：")
+
         for g in games:
-            messages.append(await map_game(g, detailed=True))
+            msgs.append(await map_game(g, detailed=True))
 
-        await send_msgs(bot, event, messages)
+        await send_msgs(bot, event, msgs)
     else:
         await matcher.send("本群还没有未完成的对局")
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,102 @@
 # ========== 查询最近走势 ==========
-from nonebot import on_command
-from nonebot.adapters.onebot.v11 import Message
-from nonebot.internal.matcher import Matcher
-
-from nonebot_plugin_mahjong_scoreboard.controller.general_handlers import require_parse_unary_at_arg, \
-    require_group_binding_qq, require_user_binding_qq, require_running_season
-from nonebot_plugin_mahjong_scoreboard.controller.interceptor import general_interceptor
-from nonebot_plugin_mahjong_scoreboard.controller.mapper.game_statistics_mapper import map_season_user_trend, \
-    map_game_statistics
-from nonebot_plugin_mahjong_scoreboard.controller.utils.message import SplitCommandArgs
-from nonebot_plugin_mahjong_scoreboard.errors import BadRequestError
-from nonebot_plugin_mahjong_scoreboard.service import season_user_point_service
-from nonebot_plugin_mahjong_scoreboard.service.game_service import get_game_statistics
-from nonebot_plugin_mahjong_scoreboard.service.group_service import get_group_by_binding_qq
-from nonebot_plugin_mahjong_scoreboard.service.season_service import get_season_by_id, get_season_by_code
-from nonebot_plugin_mahjong_scoreboard.service.user_service import get_user_by_binding_qq
+from io import StringIO
+
+from nonebot import on_command, Bot
+from nonebot.internal.matcher import Matcher, current_bot
+from nonebot_plugin_session import Session
+
+from .interceptor import handle_error
+from .mapper import map_point, digit_mapping, percentile_str, map_real_point
+from .utils.dep import GroupDep, SessionDep, RunningSeasonDep, UserDep, SeasonFromUnaryArgOrRunningSeason
+from .utils.general_handlers import require_store_command_args, require_platform_group_id, require_platform_user_id
+from ..errors import BadRequestError
+from ..model import GameStatistics, Group, Season, User
+from ..platform.get_user_nickname import get_user_nickname
+from ..service.game_service import get_game_statistics, get_games, get_season_game_statistics
+from ..utils.session import get_platform_group_id
 
 # ============ 查询最近走势 ============
 query_season_user_trend_matcher = on_command("查询最近走势", aliases={"最近走势", "走势"}, priority=5)
 
-require_parse_unary_at_arg(query_season_user_trend_matcher, "user_binding_qq")
-require_group_binding_qq(query_season_user_trend_matcher)
-require_user_binding_qq(query_season_user_trend_matcher)
-require_running_season(query_season_user_trend_matcher)
+require_store_command_args(query_season_user_trend_matcher)
+require_platform_group_id(query_season_user_trend_matcher)
+require_platform_user_id(query_season_user_trend_matcher)
 
 
 @query_season_user_trend_matcher.handle()
-@general_interceptor(query_season_user_trend_matcher)
-async def query_season_user_trend(matcher: Matcher):
-    group_binding_qq = matcher.state["binding_qq"]
-    user_binding_qq = matcher.state["user_binding_qq"]
-
-    group = await get_group_by_binding_qq(group_binding_qq)
-    user = await get_user_by_binding_qq(user_binding_qq)
-
-    season = await get_season_by_id(matcher.state["running_season_id"])
-    logs = await season_user_point_service.get_season_user_point_change_logs(season, user,
-                                                                             limit=10, reverse_order=True,
-                                                                             join_game_and_record=True)
-    if len(logs) != 0:
-        msg = await map_season_user_trend(group, user, season, logs)
-        await matcher.send(msg)
+@handle_error()
+async def query_season_user_trend(bot: Bot, matcher: Matcher, group: Group = GroupDep(),
+                                  session: Session = SessionDep(),
+                                  user: User = UserDep(lookup_matcher_state=True),
+                                  season: Season = RunningSeasonDep()):
+    games = await get_games(group.id, user.id, season.id, limit=10, reverse_order=True, completed_only=True)
+
+    if len(games) != 0:
+        with StringIO() as sio:
+            sio.write(f"用户[{await get_user_nickname(bot, user.platform_user_id, get_platform_group_id(session))}]"
+                      f"的最近走势如下：\n")
+
+            for game in games:
+                record = game.records[0]
+                for r in game.records:
+                    if r.user.id == user.id:
+                        record = r
+
+                sio.write(f"  {record.rank}位    {record.score}点  "
+                          f"({map_point(record.raw_point, record.point_scale)})  "
+                          f"对局{game.code}\n")
+
+            await matcher.send(sio.getvalue().strip())
     else:
         raise BadRequestError("你还没有参加过对局")
 
 
 # ============ 对战数据 ============
-query_user_statistics_matcher = on_command("对战数据", priority=5)
+async def map_game_statistics(game_statistics: GameStatistics, user: User, group: Group) -> str:
+    bot = current_bot.get()
+    with StringIO() as sio:
+        sio.write(f"用户[{await get_user_nickname(bot, user.platform_user_id, group.platform_group_id)}]的对战数据：\n")
+
+        sio.write(f"  对局数：{game_statistics.total} （半庄：{game_statistics.total_south}、东风：{game_statistics.total_east}）\n")
+        for i, rate in enumerate(game_statistics.rates):
+            sio.write(f"  {digit_mapping[i + 1]}位率：{percentile_str(rate)}\n")
+        sio.write(f"  平均顺位：{round(game_statistics.avg_rank, 2)}\n")
+        if game_statistics.pt_expectation is not None:
+            sio.write(f"  PT期望：{map_real_point(game_statistics.pt_expectation, 2)}\n")
+        sio.write(f"  被飞率：{percentile_str(game_statistics.flying_rate)}")
 
-require_parse_unary_at_arg(query_user_statistics_matcher, "user_binding_qq")
-require_group_binding_qq(query_user_statistics_matcher)
-require_user_binding_qq(query_user_statistics_matcher)
+        return sio.getvalue().strip()
 
 
-@query_user_statistics_matcher.handle()
-@general_interceptor(query_user_statistics_matcher)
-async def query_user_statistics(matcher: Matcher):
-    group_binding_qq = matcher.state["binding_qq"]
-    user_binding_qq = matcher.state["user_binding_qq"]
+query_user_statistics_matcher = on_command("对战数据", priority=5)
+
+require_store_command_args(query_user_statistics_matcher)
+require_platform_group_id(query_user_statistics_matcher)
+require_platform_user_id(query_user_statistics_matcher)
 
-    group = await get_group_by_binding_qq(group_binding_qq)
-    user = await get_user_by_binding_qq(user_binding_qq)
 
-    game_statistics = await get_game_statistics(group, user)
-    msg = await map_game_statistics(group, user, None, game_statistics)
+@query_user_statistics_matcher.handle()
+@handle_error()
+async def query_user_statistics(matcher: Matcher, group: Group = GroupDep(),
+                                user: User = UserDep(lookup_matcher_state=True)):
+    game_statistics = await get_game_statistics(group.id, user.id)
+    msg = await map_game_statistics(game_statistics, user, group)
     await matcher.send(msg)
 
 
 # ============ 赛季对战数据 ============
 query_season_user_statistics_matcher = on_command("赛季对战数据", priority=5)
 
-
-@query_season_user_statistics_matcher.handle()
-@general_interceptor(query_season_user_statistics_matcher)
-async def parse_query_season_user_statistics_args(matcher: Matcher, args: Message = SplitCommandArgs()):
-    user_id = None
-    season_code = None
-
-    for arg in args:
-        if arg.type == "at":
-            user_id = int(arg.data["qq"])
-        elif arg.type == "text":
-            season_code = arg.data["text"]
-
-    if user_id is not None:
-        matcher.state["user_binding_qq"] = user_id
-
-    if season_code is not None:
-        matcher.state["season_code"] = season_code
-
-
-require_parse_unary_at_arg(query_season_user_statistics_matcher, "user_binding_qq")
-require_group_binding_qq(query_season_user_statistics_matcher)
-require_user_binding_qq(query_season_user_statistics_matcher)
+require_store_command_args(query_season_user_statistics_matcher)
+require_platform_group_id(query_season_user_statistics_matcher)
+require_platform_user_id(query_season_user_statistics_matcher)
 
 
 @query_season_user_statistics_matcher.handle()
-@general_interceptor(query_season_user_statistics_matcher)
-async def query_season_user_statistics(matcher: Matcher):
-    group_binding_qq = matcher.state["binding_qq"]
-    user_binding_qq = matcher.state["user_binding_qq"]
-
-    group = await get_group_by_binding_qq(group_binding_qq)
-    user = await get_user_by_binding_qq(user_binding_qq)
-
-    season_code = matcher.state.get("season_code", None)
-    if season_code:
-        season = await get_season_by_code(season_code, group)
-        if season is None:
-            raise BadRequestError("找不到指定赛季")
-    else:
-        if group.running_season_id:
-            season = await get_season_by_id(group.running_season_id)
-        else:
-            raise BadRequestError("当前没有运行中的赛季")
-
-    game_statistics = await get_game_statistics(group, user, season)
-    msg = await map_game_statistics(group, user, season, game_statistics)
+@handle_error()
+async def query_season_user_statistics(matcher: Matcher, group: Group = GroupDep(),
+                                       user: User = UserDep(lookup_matcher_state=True),
+                                       season: Season = SeasonFromUnaryArgOrRunningSeason()):
+    game_statistics = await get_season_game_statistics(group.id, user.id, season.id)
+    msg = await  map_game_statistics(game_statistics, user, group)
     await matcher.send(msg)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_error_impl.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 from functools import wraps
-from typing import Type
 
 from nonebot import logger
-from nonebot.adapters.onebot.v11 import ActionFailed
-from nonebot.exception import MatcherException
-from nonebot.internal.matcher import Matcher
+from nonebot.exception import MatcherException, ActionFailed
+from nonebot.internal.matcher import current_event, current_matcher
 
-from nonebot_plugin_mahjong_scoreboard.errors import BadRequestError
+from ...errors import BadRequestError
 
 
-def handle_error(matcher: Type[Matcher]):
+def handle_error():
     def decorator(func):
         @wraps(func)
         async def wrapped_func(*args, **kwargs):
+            matcher = current_matcher.get()
             try:
                 return await func(*args, **kwargs)
             except MatcherException as e:
                 raise e
             except BadRequestError as e:
                 await matcher.finish(e.message)
             except ActionFailed as e:
-                logger.exception(e)
                 # 避免当发送消息错误时再尝试发送
-                if e.info['msg'] != 'SEND_MSG_API_ERROR':
-                    await matcher.finish(f"内部错误：{type(e)}{str(e)}")
+                logger.exception(e)
             except Exception as e:
                 logger.exception(e)
                 await matcher.finish(f"内部错误：{type(e)}{str(e)}")
 
         return wrapped_func
 
     return decorator
+
+
+def handle_interruption():
+    def decorator(func):
+        @wraps(func)
+        async def wrapped_func(*args, **kwargs):
+            event = current_event.get()
+            matcher = current_matcher.get()
+            if event and event.get_plaintext() == '/q':
+                await matcher.finish("中止流程")
+
+            return await func(*args, **kwargs)
+
+        return wrapped_func
+
+    return decorator
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import csv
 from typing import TextIO, Iterable
 
+from nonebot.internal.matcher import current_bot
+
 from nonebot_plugin_mahjong_scoreboard.controller.mapper import game_state_mapping, \
     player_and_wind_mapping, map_datetime, map_point
 from nonebot_plugin_mahjong_scoreboard.controller.mapper.game_mapper import map_game_progress
+from nonebot_plugin_mahjong_scoreboard.model import Game
 from nonebot_plugin_mahjong_scoreboard.model.enums import GameState
-from nonebot_plugin_mahjong_scoreboard.model.orm import data_source
-from nonebot_plugin_mahjong_scoreboard.model.orm.game import GameOrm, GameProgressOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.group import GroupOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.season import SeasonOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.user import UserOrm
-from nonebot_plugin_mahjong_scoreboard.service.group_service import get_user_nickname
+from nonebot_plugin_mahjong_scoreboard.platform.get_user_nickname import get_user_nickname
+from nonebot_plugin_mahjong_scoreboard.utils.session import get_real_id
 
 
-async def map_games_as_csv(f: TextIO, games: Iterable[GameOrm]):
-    session = data_source.session()
+async def write_games_csv(f: TextIO, games: Iterable[Game]):
+    bot = current_bot.get()
 
     writer = csv.writer(f)
     writer.writerow(['对局编号', '对局类型', '状态', '完成时间',
                      '所属赛季', '发起者',
                      '一位', '一位分数', '一位PT收支',
                      '二位', '二位分数', '二位PT收支',
                      '三位', '三位分数', '三位PT收支',
@@ -31,36 +30,32 @@
         ]
 
         if g.state == GameState.completed:
             row.append(map_datetime(g.complete_time))
         else:
             row.append("")
 
-        group = await session.get(GroupOrm, g.group_id)
-
-        if g.season_id is not None:
-            season = await session.get(SeasonOrm, g.season_id)
-            row.append(season.name)
+        if g.season is not None:
+            row.append(g.season.name)
         else:
             row.append("")
 
-        if g.promoter_user_id is not None:
-            promoter = await session.get(UserOrm, g.promoter_user_id)
-            row.append(f"{await get_user_nickname(promoter, group)} ({promoter.binding_qq})")
+        if g.promoter is not None:
+            row.append(f"{await get_user_nickname(bot, g.promoter.platform_user_id, g.group.platform_group_id)}"
+                       f" ({get_real_id(g.promoter.platform_user_id)})")
         else:
             row.append("")
 
         for r in sorted(g.records, key=lambda x: x.raw_point, reverse=True):
-            user = await session.get(UserOrm, r.user_id)
-            row.extend([f"{await get_user_nickname(user, group)} ({user.binding_qq})",
+            row.extend([f"{await get_user_nickname(bot, r.user.platform_user_id, g.group.platform_group_id)}"
+                        f" ({get_real_id(r.user.platform_user_id)})",
                         r.score,
                         map_point(r.raw_point, r.point_scale)])
 
-        progress = await session.get(GameProgressOrm, g.id)
-        if progress is not None:
-            row.append(map_game_progress(progress))
+        if g.progress is not None:
+            row.append(map_game_progress(g.progress))
         else:
             row.append("")
 
         row.append(g.comment)
 
         writer.writerow(row)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,80 @@
 from io import StringIO
 
-from nonebot.adapters.onebot.v11 import MessageSegment, Message
+from nonebot.internal.matcher import current_bot
 
-from nonebot_plugin_mahjong_scoreboard.controller.mapper import player_and_wind_mapping, game_state_mapping, \
-    digit_mapping, \
-    wind_mapping, map_datetime, map_point
-from nonebot_plugin_mahjong_scoreboard.model.enums import GameState
-from nonebot_plugin_mahjong_scoreboard.model.orm import data_source
-from nonebot_plugin_mahjong_scoreboard.model.orm.game import GameOrm, GameProgressOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.group import GroupOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.season import SeasonOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.user import UserOrm
-from nonebot_plugin_mahjong_scoreboard.service.group_service import get_user_nickname
-from nonebot_plugin_mahjong_scoreboard.utils.rank import ranked
+from . import player_and_wind_mapping, game_state_mapping, digit_mapping, wind_mapping, map_datetime, map_point
+from ...model import Game, GameProgress
+from ...model.enums import GameState
+from ...platform.get_user_nickname import get_user_nickname
+from ...utils.rank import ranked
 
 
-def map_game_progress(progress: GameProgressOrm) -> str:
+def map_game_progress(progress: GameProgress) -> str:
     with StringIO() as io:
         if progress.round <= 4:
             io.write('东')
             io.write(digit_mapping[progress.round])
         else:
             io.write('南')
             io.write(digit_mapping[progress.round - 4])
         io.write('局')
         io.write(str(progress.honba))
         io.write('本场')
 
         return io.getvalue()
 
 
-async def map_game(game: GameOrm, *, detailed: bool = False) -> Message:
-    session = data_source.session()
-
-    group = await session.get(GroupOrm, game.group_id)
-
+async def map_game(game: Game, *, detailed: bool = False) -> str:
+    bot = current_bot.get()
     with StringIO() as io:
         # 对局22090901  四人南
         io.write(f'对局{game.code}  {player_and_wind_mapping[game.player_and_wind]}\n')
 
         if detailed:
             # 所属赛季：Season Name
             season_name = '无'
-            if game.season_id is not None:
-                season = await session.get(SeasonOrm, game.season_id)
-                season_name = season.name
+            if game.season is not None:
+                season_name = game.season.name
             io.write(f'所属赛季：{season_name}\n')
 
-            promoter = await session.get(UserOrm, game.promoter_user_id)
-            io.write(f'创建者：{await get_user_nickname(promoter, group)}\n')
+            io.write(f'创建者：{game.promoter.platform_user_id}\n')
 
         # 状态：未完成
         io.write(f'状态：{game_state_mapping[GameState(game.state)]}')
         if game.state != GameState.completed:
             sum_score = sum(map(lambda r: r.score, game.records))
             io.write(f"  （合计{sum_score}点）")
         io.write('\n')
 
         if detailed and game.state == GameState.completed:
             io.write(f'完成时间：{map_datetime(game.complete_time)}\n')
 
-        progress = await session.get(GameProgressOrm, game.id)
-        if progress is not None:
-            io.write(f'进度：{map_game_progress(progress)}\n')
+        if game.progress is not None:
+            io.write(f'进度：{map_game_progress(game.progress)}\n')
 
         if len(game.records) > 0:
             # [空行]
             io.write('\n')
 
             # #1 [东]    Player Name    10000点  (+5)
             # [...]
             for rank, r in ranked(game.records, key=lambda r: r.raw_point, reverse=True):
-                user = await session.get(UserOrm, r.user_id)
-                name = await get_user_nickname(user, group)
                 io.write(f'#{rank}')
                 if r.wind is not None:
                     io.write(f' [{wind_mapping[r.wind]}]')
-                io.write(f'    {name}    {r.score}点')
+                io.write(f'    {await get_user_nickname(bot, r.user.platform_user_id, game.group.platform_group_id)}'
+                         f'    {r.score}点')
 
                 if game.state == GameState.completed:
                     point_text = map_point(r.raw_point, r.point_scale)
                     io.write(f'  ({point_text})')
 
                 io.write('\n')
 
         if game.comment:
             io.write('\n')
             io.write("备注：")
             io.write(game.comment)
             io.write('\n')
 
-        return Message(MessageSegment.text(io.getvalue().strip()))
+        return io.getvalue().strip()
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,24 @@
 from io import StringIO
-from typing import Optional
 
-from nonebot.adapters.onebot.v11 import Message, MessageSegment
+from . import season_state_mapping, map_datetime
+from ...model import Season
 
-from nonebot_plugin_mahjong_scoreboard.controller.mapper import season_state_mapping, map_datetime
-from nonebot_plugin_mahjong_scoreboard.model.orm.season import SeasonOrm
 
-
-def map_season(season: SeasonOrm, *, group_info: Optional[dict] = None) -> Message:
+def map_season(season: Season) -> str:
     with StringIO() as io:
         # {season.name}
         io.write(season.name)
         io.write('\n')
 
         # 代号：{season.code}
         io.write('代号：')
         io.write(season.code)
         io.write('\n')
 
-        if group_info is not None:
-            # 群组：义已死吾亦死 (114514)
-            io.write('群组：')
-            io.write(group_info["group_name"])
-            io.write(' (')
-            io.write(str(group_info["group_id"]))
-            io.write(')\n')
-
         if season.state:
             io.write('状态：')
             io.write(season_state_mapping[season.state])
             io.write('\n')
 
         if season.start_time:
             io.write('开始时间：')
@@ -68,8 +57,8 @@
         io.write('\n')
 
         # PT精度：1
         io.write('PT精度：')
         io.write(str(10 ** season.config.point_precision))
         io.write('\n')
 
-        return Message(MessageSegment.text(io.getvalue().strip()))
+        return io.getvalue().strip()
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 import csv
 from typing import TextIO, Iterable, List
 
+from nonebot.internal.matcher import current_bot
+
 from nonebot_plugin_mahjong_scoreboard.controller.mapper import map_datetime
+from nonebot_plugin_mahjong_scoreboard.model import Season, SeasonUserPointChangeLog
 from nonebot_plugin_mahjong_scoreboard.model.enums import SeasonUserPointChangeType
-from nonebot_plugin_mahjong_scoreboard.model.orm import data_source
-from nonebot_plugin_mahjong_scoreboard.model.orm.game import GameOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.group import GroupOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.season import SeasonOrm, SeasonUserPointChangeLogOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.user import UserOrm
-from nonebot_plugin_mahjong_scoreboard.service.group_service import get_user_nickname
+from nonebot_plugin_mahjong_scoreboard.platform.get_user_nickname import get_user_nickname
+from nonebot_plugin_mahjong_scoreboard.utils.session import get_real_id
 
 
 def _ensure_size(li: list, new_size: int, default):
     while len(li) < new_size:
         li.append(default)
 
 
-async def map_season_user_point_change_logs_as_csv(f: TextIO, logs: Iterable[SeasonUserPointChangeLogOrm],
-                                                   season: SeasonOrm):
-    session = data_source.session()
-    group = await session.get(GroupOrm, season.group_id)
+async def write_season_user_point_change_logs_csv(f: TextIO, logs: Iterable[SeasonUserPointChangeLog],
+                                                  season: Season):
+    bot = current_bot.get()
 
     header = ['', '合计PT']
     table: List[List[str]] = []
 
     user_idx = {}
     game_idx = {}
 
     user_point = {}
 
     # 初步绘制表格
     for log in logs:
-        user = await session.get(UserOrm, log.user_id)
-        if user.id not in user_idx:
-            table.append([f"{await get_user_nickname(user, group)} ({user.binding_qq})", ""])
-            user_idx[user.id] = len(table) - 1
+        if log.user.id not in user_idx:
+            table.append([f"{await get_user_nickname(bot, log.user.platform_user_id, season.group.platform_group_id)}"
+                          f" ({get_real_id(log.user.platform_user_id)})", ""])
+            user_idx[log.user.id] = len(table) - 1
 
         if log.change_type == SeasonUserPointChangeType.game:
-            related_game = await session.get(GameOrm, log.related_game_id)
-            if related_game.id not in game_idx:
-                header.append(str(related_game.code))
-                game_idx[related_game.id] = len(header) - 1
+            if log.related_game.id not in game_idx:
+                header.append(str(log.related_game.code))
+                game_idx[log.related_game.id] = len(header) - 1
 
-            _ensure_size(table[user_idx[user.id]], game_idx[related_game.id] + 1, '')
-            table[user_idx[user.id]][game_idx[related_game.id]] = str(log.change_point)
+            _ensure_size(table[user_idx[log.user.id]], game_idx[log.related_game.id] + 1, '')
+            table[user_idx[log.user.id]][game_idx[log.related_game.id]] = str(log.change_point)
 
-            user_point[user.id] = user_point.get(user.id, 0) + log.change_point
+            user_point[log.user.id] = user_point.get(log.user.id, 0) + log.change_point
         elif log.change_type == SeasonUserPointChangeType.manually:
             header.append(f"手动设置 {map_datetime(log.create_time)}")
 
-            _ensure_size(table[user_idx[user.id]], len(header), '')
-            table[user_idx[user.id]][-1] = str(log.change_point)
+            _ensure_size(table[user_idx[log.user.id]], len(header), '')
+            table[user_idx[log.user.id]][-1] = str(log.change_point)
 
-            user_point[user.id] = log.change_point
+            user_point[log.user.id] = log.change_point
 
     # 将行（用户）按pt排序
     ordered_user_idx = []
     for user_id, idx in user_idx.items():
         ordered_user_idx.append((user_id, idx, user_point[user_id]))
     ordered_user_idx.sort(key=lambda x: x[2], reverse=True)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,87 @@
 import re
 
 from nonebot import on_command
-from nonebot.adapters.onebot.v11 import MessageEvent, Message, MessageSegment
+from nonebot.internal.adapter import Event
 from nonebot.internal.matcher import Matcher
 from nonebot.internal.params import ArgPlainText
 
-from nonebot_plugin_mahjong_scoreboard.controller.general_handlers import require_group_binding_qq, \
-    require_parse_unary_text_arg, require_str, hint_for_question_flow_on_first
-from nonebot_plugin_mahjong_scoreboard.controller.interceptor import general_interceptor
-from nonebot_plugin_mahjong_scoreboard.controller.mapper.season_mapper import map_season
-from nonebot_plugin_mahjong_scoreboard.controller.utils.parse import parse_int_or_reject
-from nonebot_plugin_mahjong_scoreboard.errors import BadRequestError
-from nonebot_plugin_mahjong_scoreboard.model.enums import SeasonState
-from nonebot_plugin_mahjong_scoreboard.model.orm.season import SeasonOrm, SeasonConfig
-from nonebot_plugin_mahjong_scoreboard.service import season_service
-from nonebot_plugin_mahjong_scoreboard.service.group_service import get_group_by_binding_qq
-from nonebot_plugin_mahjong_scoreboard.service.user_service import get_user_by_binding_qq
+from .interceptor import handle_interruption, handle_error
+from .mapper.season_mapper import map_season
+from .utils.dep import GroupDep, UserDep, UnaryArg, RunningSeasonDep
+from .utils.general_handlers import hint_for_question_flow_on_first
+from .utils.parse import parse_int_or_reject
+from ..errors import BadRequestError
+from ..model import Group, Season, User, SeasonConfig
+from ..model.enums import SeasonState
+from ..service import season_service
+from ..service.season_service import get_season_by_code, new_season, start_season, finish_season
 
 # ========== 新赛季 ==========
 new_season_matcher = on_command("新建赛季", aliases={"新赛季"}, priority=5)
 
-require_group_binding_qq(new_season_matcher, True)
-
 new_season_matcher.append_handler(hint_for_question_flow_on_first)
 
 
 @new_season_matcher.got("code", "赛季代号？")
-@general_interceptor(new_season_matcher)
+@handle_error()
+@handle_interruption()
 async def new_season_got_code(matcher: Matcher,
-                              raw_arg=ArgPlainText("code")):
-    match_result = re.match(r"[_a-zA-Z][_a-zA-Z0-9]*", raw_arg)
+                              raw_arg=ArgPlainText("code"),
+                              group: Group = GroupDep()):
+    match_result = re.match(r"[_a-zA-Z]\w*", raw_arg)
     if match_result is None:
         await matcher.reject("赛季代号不合法。请重新输入。（赛季代号只允许包含字母、数字和下划线，且必须以字母或下划线开头）")
 
-    group = await get_group_by_binding_qq(matcher.state["binding_qq"])
-    season = await season_service.get_season_by_code(raw_arg, group)
+    season = await get_season_by_code(raw_arg, group.id)
     if season is not None:
         await matcher.reject("该赛季代号已被使用。请重新输入")
 
     matcher.state["code"] = raw_arg
 
 
 @new_season_matcher.got("name", "赛季名称？")
-@general_interceptor(new_season_matcher)
+@handle_error()
+@handle_interruption()
 async def new_season_got_name(matcher: Matcher,
                               raw_arg=ArgPlainText("name")):
     matcher.state["name"] = raw_arg
 
 
 @new_season_matcher.got("south_game_enabled", "是否开启半庄战？(y/n)")
-@general_interceptor(new_season_matcher)
+@handle_error()
+@handle_interruption()
 async def new_season_got_east_game_enabled(matcher: Matcher,
+                                           event: Event,
                                            raw_arg=ArgPlainText("south_game_enabled")):
+    Message = type(event.get_message())
     if raw_arg == 'y':
         matcher.state["south_game_enabled"] = True
     else:
         matcher.state["south_game_enabled"] = False
         matcher.set_arg("south_game_origin_point", Message())
         matcher.set_arg("south_game_horse_point", Message())
 
 
 @new_season_matcher.got("south_game_origin_point", "半庄战返点？")
-@general_interceptor(new_season_matcher)
+@handle_error()
+@handle_interruption()
 async def new_season_got_south_game_origin_point(matcher: Matcher,
                                                  raw_arg=ArgPlainText("south_game_origin_point")):
     if not matcher.state["south_game_enabled"]:
         matcher.state["south_game_origin_point"] = None
         return
 
     pt = await parse_int_or_reject(raw_arg, "半庄战返点")
     matcher.state["south_game_origin_point"] = pt
 
 
 @new_season_matcher.got("south_game_horse_point", "半庄战马点？通过空格分割")
-@general_interceptor(new_season_matcher)
+@handle_error()
+@handle_interruption()
 async def new_season_got_south_game_horse_point(matcher: Matcher,
                                                 raw_arg=ArgPlainText("south_game_horse_point")):
     if not matcher.state["south_game_enabled"]:
         return
 
     try:
         li = list(map(float, raw_arg.split(' ')))
@@ -87,42 +91,47 @@
 
     if len(li) != 4:
         await matcher.reject("输入的半庄战马点不合法。请重新输入")
     matcher.state["south_game_horse_point"] = li
 
 
 @new_season_matcher.got("east_game_enabled", "是否开启东风战？(y/n)")
-@general_interceptor(new_season_matcher)
+@handle_error()
+@handle_interruption()
 async def new_season_got_east_game_enabled(matcher: Matcher,
+                                           event: Event,
                                            raw_arg=ArgPlainText("east_game_enabled")):
+    Message = type(event.get_message())
     if raw_arg == 'y':
         matcher.state["east_game_enabled"] = True
     else:
         matcher.state["east_game_enabled"] = False
         matcher.set_arg("east_game_origin_point", Message())
         matcher.set_arg("east_game_horse_point", Message())
 
     if not matcher.state["south_game_enabled"] and not matcher.state["east_game_enabled"]:
         raise BadRequestError("半庄战、东风战至少需要开启一种")
 
 
 @new_season_matcher.got("east_game_origin_point", "东风战返点？")
-@general_interceptor(new_season_matcher)
+@handle_error()
+@handle_interruption()
 async def new_season_got_south_game_origin_point(matcher: Matcher,
                                                  raw_arg=ArgPlainText("east_game_origin_point")):
     if not matcher.state["east_game_enabled"]:
         matcher.state["east_game_origin_point"] = None
         return
 
     pt = await parse_int_or_reject(raw_arg, "东风战返点")
     matcher.state["east_game_origin_point"] = pt
 
 
 @new_season_matcher.got("east_game_horse_point", "东风战马点？通过空格分割")
-@general_interceptor(new_season_matcher)
+@handle_error()
+@handle_interruption()
 async def new_season_got_east_game_horse_point(matcher: Matcher,
                                                raw_arg=ArgPlainText("east_game_horse_point")):
     if not matcher.state["east_game_enabled"]:
         return
 
     try:
         li = list(map(float, raw_arg.split(' ')))
@@ -132,173 +141,157 @@
 
     if len(li) != 4:
         await matcher.reject("输入的东风战马点不合法。请重新输入")
     matcher.state["east_game_horse_point"] = li
 
 
 @new_season_matcher.got("point_precision", "PT精度？（输入x，则精度为10^x。例如：输入0，保留整数部分；输入-1，保留小数点后一位）")
-@general_interceptor(new_season_matcher)
+@handle_error()
+@handle_interruption()
 async def new_season_got_point_precision(matcher: Matcher,
                                          raw_arg=ArgPlainText("point_precision")):
     precision = await parse_int_or_reject(raw_arg, "PT精度", max=4, min=-1)
     matcher.state["point_precision"] = precision
 
 
 @new_season_matcher.handle()
-@general_interceptor(new_season_matcher)
-async def new_season_confirm(matcher: Matcher):
-    season = SeasonOrm(code=matcher.state["code"],
-                       name=matcher.state["name"],
-                       config=SeasonConfig({
-                           "south_game_enabled": matcher.state["south_game_enabled"],
-                           "south_game_origin_point": matcher.state.get("south_game_origin_point"),
-                           "south_game_horse_point": matcher.state.get("south_game_horse_point"),
-                           "east_game_enabled": matcher.state["east_game_enabled"],
-                           "east_game_origin_point": matcher.state.get("east_game_origin_point"),
-                           "east_game_horse_point": matcher.state.get("east_game_horse_point"),
-                           "point_precision": matcher.state["point_precision"]
-                       }))
-    matcher.state["season"] = season
+@handle_error()
+@handle_interruption()
+async def new_season_confirm(matcher: Matcher, group: Group = GroupDep()):
+    matcher.state["season_config"] = SeasonConfig(
+        south_game_enabled=matcher.state["south_game_enabled"],
+        south_game_origin_point=matcher.state.get("south_game_origin_point"),
+        south_game_horse_point=matcher.state.get("south_game_horse_point"),
+        east_game_enabled=matcher.state["east_game_enabled"],
+        east_game_origin_point=matcher.state.get("east_game_origin_point"),
+        east_game_horse_point=matcher.state.get("east_game_horse_point"),
+        point_precision=matcher.state["point_precision"]
+    )
+
+    season = Season(id=0,
+                    group=group,
+                    state=SeasonState.initial,
+                    code=matcher.state["code"],
+                    name=matcher.state["name"],
+                    config=matcher.state["season_config"])
 
-    msg = map_season(season, group_info=matcher.state["group_info"])
-    msg.append(MessageSegment.text("\n\n确定创建赛季吗？(y/n)"))
+    msg = map_season(season)
+    msg += "\n\n确定创建赛季吗？(y/n)"
     await matcher.pause(msg)
 
 
 @new_season_matcher.handle()
-@general_interceptor(new_season_matcher)
-async def new_season_handle(event: MessageEvent, matcher: Matcher):
-    if event.message.extract_plain_text() == 'y':
-        season = matcher.state["season"]
-        season.group = await get_group_by_binding_qq(matcher.state["binding_qq"])
-        season = await season_service.new_season(season)
-        matcher.state["season_id"] = season
+@handle_error()
+async def new_season_handle(event: Event, matcher: Matcher, group: Group = GroupDep()):
+    if event.get_message().extract_plain_text() == 'y':
+        season = await new_season(group.id, code=matcher.state["code"],
+                                  name=matcher.state["name"],
+                                  config=matcher.state["season_config"])
+        matcher.state["season"] = season
         await matcher.pause("赛季创建成功。是否立刻开启该赛季？(y/n)")
     else:
         await matcher.finish("取消赛季创建")
 
 
 @new_season_matcher.handle()
-@general_interceptor(new_season_matcher)
-async def new_season_start(event: MessageEvent, matcher: Matcher):
-    if event.message.extract_plain_text() == 'y':
-        # 因为session不同，所以需要重新获取season
-        season = await season_service.get_season_by_id(matcher.state["season"].id)
-        operator = await get_user_by_binding_qq(event.user_id)
-        await season_service.start_season(season, operator)
+@handle_error()
+async def new_season_start(event: Event, matcher: Matcher, operator: User = UserDep()):
+    if event.get_message().extract_plain_text() == 'y':
+        await start_season(matcher.state["season"].id, operator.id)
         await matcher.send("赛季开启成功")
     else:
         await matcher.send(f"稍后可以使用“/开启赛季 {matcher.state['season'].code}”命令开启赛季")
 
 
 # ========== 开启赛季 ==========
 start_season_matcher = on_command("开启赛季", priority=5)
 
-require_parse_unary_text_arg(start_season_matcher, "season_code")
-require_group_binding_qq(start_season_matcher, True)
-require_str(start_season_matcher, "season_code", "赛季代号")
-
 
 @start_season_matcher.handle()
-@general_interceptor(start_season_matcher)
-async def start_season_matcher_confirm(matcher: Matcher):
-    season_code = matcher.state["season_code"]
+@handle_error()
+async def start_season_matcher_confirm(matcher: Matcher, group: Group = GroupDep(),
+                                       season_code=UnaryArg()):
+    if season_code is None:
+        raise BadRequestError("请指定赛季编号。使用“/新赛季”指令创建赛季")
 
-    group = await get_group_by_binding_qq(matcher.state["binding_qq"])
-    season = await season_service.get_season_by_code(season_code, group)
+    season = await get_season_by_code(season_code, group.id)
     if season is None:
-        raise BadRequestError("找不到赛季。使用“/新赛季”指令创建赛季")
+        raise BadRequestError("找不到该赛季。使用“/新赛季”指令创建赛季")
 
-    matcher.state["season_id"] = season.id
+    matcher.state["season"] = season
 
-    msg = map_season(season, group_info=matcher.state["group_info"])
-    msg.append(MessageSegment.text("\n\n确定开启赛季吗？(y/n)"))
-    await matcher.pause(msg)
+    msg = map_season(season)
+    if season.state != SeasonState.initial:
+        msg += "\n\n赛季未处于初始状态，操作失败"
+        await matcher.finish(msg)
+    else:
+        msg += "\n\n确定开启赛季吗？(y/n)"
+        await matcher.pause(msg)
 
 
 @start_season_matcher.handle()
-@general_interceptor(start_season_matcher)
-async def start_season_end(event: MessageEvent, matcher: Matcher):
-    if event.message.extract_plain_text() == 'y':
-        # 因为session不同，所以需要重新获取season
-        season = await season_service.get_season_by_id(matcher.state["season_id"])
-        operator = await get_user_by_binding_qq(event.user_id)
-        await season_service.start_season(season, operator)
+@handle_error()
+async def start_season_end(event: Event, matcher: Matcher, operator: User = UserDep()):
+    if event.get_message().extract_plain_text() == 'y':
+        await season_service.start_season(matcher.state["season"].id, operator.id)
         await matcher.send("赛季开启成功")
     else:
         await matcher.send("取消开启赛季")
 
 
 # ========== 结束赛季 ==========
 finish_season_matcher = on_command("结束赛季", priority=5)
 
-require_group_binding_qq(finish_season_matcher, True)
-
 
 @finish_season_matcher.handle()
-@general_interceptor(finish_season_matcher)
-async def finish_season_confirm(matcher: Matcher):
-    group = await get_group_by_binding_qq(matcher.state["binding_qq"])
-    season = await season_service.get_season_by_id(group.running_season_id)
-    matcher.state["season_id"] = season.id
-
-    if season is None:
-        raise BadRequestError("当前没有运行中的赛季")
-
-    msg = map_season(season, group_info=matcher.state["group_info"])
-    msg.append(MessageSegment.text("\n\n结束赛季将删除赛季的所有未完成对局，并且无法再修改赛季的已完成对局。\n确定结束赛季吗？(y/n)"))
+@handle_error()
+async def finish_season_confirm(matcher: Matcher, season: Season = RunningSeasonDep()):
+    matcher.state["season"] = season
+    msg = map_season(season)
+    msg += "\n\n结束赛季将删除赛季的所有未完成对局，并且无法再修改赛季的已完成对局。\n确定结束赛季吗？(y/n)"
     await matcher.pause(msg)
 
 
 @finish_season_matcher.handle()
-@general_interceptor(finish_season_matcher)
-async def finish_season_end(event: MessageEvent, matcher: Matcher):
-    if event.message.extract_plain_text() == 'y':
-        # 因为session不同，所以需要重新获取season
-        season = await season_service.get_season_by_id(matcher.state["season_id"])
-        operator = await get_user_by_binding_qq(event.user_id)
-        await season_service.finish_season(season, operator)
+@handle_error()
+async def finish_season_end(event: Event, matcher: Matcher, operator: User = UserDep()):
+    if event.get_message().extract_plain_text() == 'y':
+        await finish_season(matcher.state["season"].id, operator.id)
         await matcher.send("赛季结束成功")
     else:
         await matcher.send("取消结束赛季")
 
 
 # ========== 删除赛季 ==========
 remove_season_matcher = on_command("删除赛季", priority=5)
 
-require_parse_unary_text_arg(remove_season_matcher, "season_code")
-require_group_binding_qq(remove_season_matcher, True)
-require_str(remove_season_matcher, "season_code", "赛季代号")
-
 
 @remove_season_matcher.handle()
-@general_interceptor(remove_season_matcher)
-async def remove_season_confirm(matcher: Matcher):
-    season_code = matcher.state["season_code"]
+@handle_error()
+async def remove_season_confirm(matcher: Matcher, group: Group = GroupDep(),
+                                season_code=UnaryArg()):
+    if season_code is None:
+        raise BadRequestError("请指定赛季编号")
 
-    group = await get_group_by_binding_qq(matcher.state["binding_qq"])
-    season = await season_service.get_season_by_code(season_code, group)
+    season = await get_season_by_code(season_code, group.id)
     if season is None:
-        raise BadRequestError("找不到赛季。使用“/新赛季”指令创建赛季")
+        raise BadRequestError("找不到该赛季")
 
-    matcher.state["season_id"] = season.id
+    matcher.state["season"] = season
 
-    msg = map_season(season, group_info=matcher.state["group_info"])
+    msg = map_season(season)
     if season.state != SeasonState.initial:
-        msg.append(MessageSegment.text("\n\n赛季未处于初始状态，操作失败"))
+        msg += "\n\n赛季未处于初始状态，操作失败"
         await matcher.finish(msg)
     else:
-        msg.append(MessageSegment.text("\n\n确定删除赛季吗？(y/n)"))
+        msg += "\n\n确定删除赛季吗？(y/n)"
         await matcher.pause(msg)
 
 
 @remove_season_matcher.handle()
-@general_interceptor(remove_season_matcher)
-async def remove_season_end(event: MessageEvent, matcher: Matcher):
-    if event.message.extract_plain_text() == 'y':
-        # 因为session不同，所以需要重新获取season
-        season = await season_service.get_season_by_id(matcher.state["season_id"])
-        operator = await get_user_by_binding_qq(event.user_id)
-        await season_service.remove_season(season, operator)
+@handle_error()
+async def remove_season_end(event: Event, matcher: Matcher, operator: User = UserDep()):
+    if event.get_message().extract_plain_text() == 'y':
+        await season_service.remove_season(matcher.state["season"].id, operator.id)
         await matcher.send("赛季删除成功")
     else:
         await matcher.send("取消删除赛季")
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 from datetime import datetime
 from io import StringIO
 
 import tzlocal
 from nonebot import on_command
-from nonebot.adapters.onebot.v11 import GroupMessageEvent, Bot, MessageEvent
-from nonebot.internal.matcher import Matcher
+from nonebot.adapters.onebot.v11 import Bot, MessageEvent
 
-from nonebot_plugin_mahjong_scoreboard.controller.general_handlers import require_group_binding_qq, \
-    require_parse_unary_text_arg
-from nonebot_plugin_mahjong_scoreboard.controller.interceptor import general_interceptor
-from nonebot_plugin_mahjong_scoreboard.controller.mapper.season_user_point_csv_mapper import \
-    map_season_user_point_change_logs_as_csv
-from nonebot_plugin_mahjong_scoreboard.errors import BadRequestError
-from nonebot_plugin_mahjong_scoreboard.model.enums import SeasonState
-from nonebot_plugin_mahjong_scoreboard.service import season_user_point_service, season_service
-from nonebot_plugin_mahjong_scoreboard.service.group_service import get_group_by_binding_qq
-from nonebot_plugin_mahjong_scoreboard.utils.date import encode_date
-from nonebot_plugin_mahjong_scoreboard.utils.upload_file import upload_group_file, upload_private_file
-
-# ========== 导出榜单 ==========
-export_season_ranking_matcher = on_command("导出榜单", priority=5)
-
-require_parse_unary_text_arg(export_season_ranking_matcher, "season_code")
-require_group_binding_qq(export_season_ranking_matcher)
-
-
-@export_season_ranking_matcher.handle()
-@general_interceptor(export_season_ranking_matcher)
-async def export_season_ranking(bot: Bot, event: MessageEvent, matcher: Matcher):
-    group = await get_group_by_binding_qq(matcher.state["binding_qq"])
-
-    season_code = matcher.state.get("season_code", None)
-    if season_code:
-        season = await season_service.get_season_by_code(season_code, group)
-        if season is None:
-            raise BadRequestError("找不到指定赛季")
-    else:
-        if group.running_season_id:
-            season = await season_service.get_season_by_id(group.running_season_id)
-        else:
-            raise BadRequestError("当前没有运行中的赛季")
-
-    logs = await season_user_point_service.get_season_user_point_change_logs(season)
+from .interceptor import handle_error
+from .mapper.game_csv_mapper import write_games_csv
+from .utils.dep import GroupDep, SeasonFromUnaryArgOrRunningSeason
+from .utils.general_handlers import require_store_command_args, require_platform_group_id
+from ..model import Group, Season
+from ..model.enums import SeasonState
+from ..platform.upload_file import upload_file
+from ..service.game_service import get_games
+from ..utils.date import encode_date
+
+# ========== 导出赛季对局 ==========
+export_season_games_matcher = on_command("导出赛季对局", aliases={"导出对局"}, priority=5)
+
+require_store_command_args(export_season_games_matcher)
+require_platform_group_id(export_season_games_matcher)
+
+
+@export_season_games_matcher.handle()
+@handle_error()
+async def export_season_games(bot: Bot, event: MessageEvent, group: Group = GroupDep(),
+                              season: Season = SeasonFromUnaryArgOrRunningSeason()):
+    games = await get_games(group_id=group.id, season_id=season.id)
 
-    filename = f"赛季榜单 {season.name}"
+    filename = f"赛季对局 {season.name}"
     if season.state == SeasonState.finished:
         filename += "（已结束）"
     else:
         now = datetime.now(tzlocal.get_localzone())
         filename += f"（截至{encode_date(now)}）"
     filename += ".csv"
 
     with StringIO() as sio:
-        await map_season_user_point_change_logs_as_csv(sio, logs, season)
+        await write_games_csv(sio, games)
+
+        data = sio.getvalue().encode("utf_8_sig")
+        await upload_file(bot, event, filename, data)
+
+
+# ========== 导出所有对局 ==========
+export_group_games_matcher = on_command("导出所有对局", priority=5)
+
+require_store_command_args(export_season_games_matcher)
+require_platform_group_id(export_season_games_matcher)
+
+
+@export_group_games_matcher.handle()
+@handle_error()
+async def export_group_games(bot: Bot, event: MessageEvent, group: Group = GroupDep()):
+    games = await get_games(group.id)
+
+    now = datetime.now(tzlocal.get_localzone())
+    filename = f"所有对局（截至{encode_date(now)}）.csv"
+
+    with StringIO() as sio:
+        await write_games_csv(sio, games)
 
         data = sio.getvalue().encode("utf_8_sig")
-        if isinstance(event, GroupMessageEvent):
-            await upload_group_file(bot, event.group_id, filename, data)
-        else:
-            await upload_private_file(bot, event.user_id, filename, data)
+        await upload_file(bot, event, filename, data)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 from typing import List, Optional
 
-from nonebot.adapters.onebot.v11 import Message, MessageSegment, MessageEvent
+from nonebot.adapters.qqguild import Message, MessageSegment
+from nonebot.internal.matcher import Matcher
 from nonebot.internal.params import Depends
 from nonebot.params import CommandArg
 
 
-def get_reply_message_id(event: MessageEvent) -> Optional[int]:
-    message_id = None
-    for seg in event.original_message:
-        if seg.type == "reply":
-            message_id = int(seg.data["id"])
-            break
-    return message_id
-
-
 def split_message(message: Message, ignore_empty: bool = True) -> List[MessageSegment]:
     result = []
     for seg in message:
         if seg.type == "text":
             for text in seg.data["text"].split(" "):
                 if not ignore_empty or text:
                     result.append(MessageSegment.text(text))
         else:
             result.append(seg)
 
     return result
 
 
-def SplitCommandArgs(ignore_empty: bool = True):
-    def dep(raw_args=CommandArg()):
-        return split_message(raw_args, ignore_empty)
+def SplitCommandArgs(*, lookup_matcher_state: bool = False,
+                     lookup_matcher_state_key: Optional[str] = "command_args_store",
+                     ignore_empty: bool = True):
+    def dep(matcher: Matcher, command_arg=CommandArg()):
+        if lookup_matcher_state:
+            command_arg = matcher.state[lookup_matcher_state_key]
+        return split_message(command_arg, ignore_empty)
 
     return Depends(dep)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/send_messages.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
-from nonebot.adapters.onebot.v11 import Message, MessageEvent, Bot, GroupMessageEvent
+from nonebot.adapters.onebot.v11 import Message, Bot, Event
 
-from nonebot_plugin_mahjong_scoreboard.config import conf
+from ...config import conf
 
 
 async def send_group_forward_msg(bot: Bot, group_id: int, messages: List[Message]):
     self_info = await bot.get_login_info()
 
     msg_li = []
 
@@ -37,20 +37,22 @@
                 "content": msg
             }
         })
 
     await bot.send_private_forward_msg(user_id=user_id, messages=msg_li)
 
 
-async def send_forward_msg(bot: Bot, event: MessageEvent, messages: List[Message]):
-    if isinstance(event, GroupMessageEvent):
-        await send_group_forward_msg(bot, event.group_id, messages)
+async def send_forward_msg(bot: Bot, event: Event, messages: List[Message]):
+    user_id = getattr(event, "user_id", None)
+    group_id = getattr(event, "group_id", None)
+    if group_id is not None:
+        await send_group_forward_msg(bot, group_id, messages)
     else:
-        await send_private_forward_msg(bot, event.user_id, messages)
+        await send_private_forward_msg(bot, user_id, messages)
 
 
-async def send_msgs(bot: Bot, event: MessageEvent, messages: List[Message]):
+async def send_msgs(bot: Bot, event: Event, messages: List[Message]):
     if len(messages) > 1 and conf.mahjong_scoreboard_send_forward_message:
         await send_forward_msg(bot, event, messages)
     else:
         for msg in messages:
             await bot.send(event, msg)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/metainfo.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sqlalchemy import JSON, inspect, select
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import Mapped, mapped_column
 
-from .src import data_source
+from .data_source import data_source
 
-APP_DB_VERSION = 2
+APP_DB_VERSION = 3
 
 
 @data_source.registry.mapped
 class MetaInfoOrm:
     __tablename__ = 'metainfo'
 
     key: Mapped[str] = mapped_column(primary_key=True)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,238 +1,169 @@
 from datetime import datetime, timedelta
 from math import ceil
 from typing import List, Optional, Tuple, overload
 
 import tzlocal
-from nonebot import logger, require
-from sqlalchemy import select, update, delete
+from nonebot import logger
+from nonebot_plugin_apscheduler import scheduler
+from sqlalchemy import delete
 from sqlalchemy.ext.asyncio import AsyncSession
-from sqlalchemy.orm import selectinload
-from sqlalchemy.sql import Select
-
-from nonebot_plugin_mahjong_scoreboard.errors import BadRequestError
-from nonebot_plugin_mahjong_scoreboard.model.enums import GameState, PlayerAndWind, Wind, SeasonState
-from nonebot_plugin_mahjong_scoreboard.model.game_statistics import GameStatistics
-from nonebot_plugin_mahjong_scoreboard.model.orm import data_source
-from nonebot_plugin_mahjong_scoreboard.model.orm.game import GameOrm, GameRecordOrm, GameProgressOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.group import GroupOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.season import SeasonOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.user import UserOrm
-from nonebot_plugin_mahjong_scoreboard.service.group_service import is_group_admin
-from nonebot_plugin_mahjong_scoreboard.service.season_user_point_service import revert_season_user_point_by_game, \
-    change_season_user_point_by_game
-from nonebot_plugin_mahjong_scoreboard.utils.date import encode_date
-from nonebot_plugin_mahjong_scoreboard.utils.integer import count_digit
 
-require("nonebot_plugin_apscheduler")
-from nonebot_plugin_apscheduler import scheduler
+from .group_service import is_group_admin
+from .mapper import map_game
+from ..errors import BadRequestError
+from ..model import Game, GameStatistics
+from ..model.enums import GameState, PlayerAndWind, Wind, SeasonState
+from ..repository import data_source
+from ..repository.data_model import GroupOrm, GameOrm, GameRecordOrm, GameProgressOrm, SeasonOrm
+from ..repository.game import GameRepository
+from ..repository.season import SeasonRepository
+from ..utils.date import encode_date
+from ..utils.integer import count_digit
 
 
 @scheduler.scheduled_job("cron", hour="*/2", id="delete_all_uncompleted_game")
 async def _delete_all_uncompleted_game():
     async with AsyncSession(data_source.engine) as session:
-        now = datetime.utcnow()
-        one_day_ago = now - timedelta(days=1)
-        stmt = (update(GameOrm)
-                .where(GameOrm.state != GameState.completed,
-                       GameOrm.create_time < one_day_ago,
-                       GameOrm.progress == None,
-                       GameOrm.accessible)
-                .values(accessible=False, delete_time=now, update_time=now)
-                .execution_options(synchronize_session=False))
-        result = await session.execute(stmt)
-        await session.commit()
-        logger.success(f"deleted {result.rowcount} outdated uncompleted game(s)")
-
-
-async def new_game(promoter: UserOrm,
-                   group: GroupOrm,
-                   player_and_wind: Optional[PlayerAndWind]) -> GameOrm:
+        repo = GameRepository(session)
+        rowcount = await repo.delete_all_uncompleted_game()
+        logger.success(f"deleted {rowcount} outdated uncompleted game(s)")
+
+
+async def _ensure_updatable(game: GameOrm):
+    session = data_source.session()
+    repo = SeasonRepository(session)
+
+    if game.season_id is not None:
+        season = await repo.get_by_pk(game.season_id)
+        if season.state != SeasonState.running:
+            raise BadRequestError("赛季已经结束，无法再修改对局")
+
+
+async def _ensure_permission(game: GameOrm, group_id: int, operator_user_id: int):
+    if game.state == GameState.completed:
+        completed_before_24h = datetime.utcnow() - game.complete_time >= timedelta(days=1)
+
+        if not completed_before_24h or await is_group_admin(operator_user_id, group_id):
+            return
+
+        raise BadRequestError("对局已完成超过24小时，需要管理员权限才能操作")
+
+
+async def new_game(promoter_user_id: int,
+                   group_id: int,
+                   player_and_wind: Optional[PlayerAndWind]) -> Game:
     session = data_source.session()
 
+    season_repo = SeasonRepository(session)
+
+    group = await session.get(GroupOrm, group_id)
+
+    # game_code
     now = datetime.now(tzlocal.get_localzone())
     game_code_base = encode_date(now)
     if game_code_base != group.prev_game_code_base:
         group.prev_game_code_base = game_code_base
         group.prev_game_code_identifier = 0
 
     group.prev_game_code_identifier += 1
 
     digit = max(2, count_digit(group.prev_game_code_identifier))
     game_code = group.prev_game_code_base * (10 ** digit) + group.prev_game_code_identifier
 
     # 未指定player_and_wind时，若赛季启用了半庄则默认为半庄，否则为东风
     if player_and_wind is None:
         if group.running_season_id is not None:
-            season = await session.get(SeasonOrm, group.running_season_id)
-            if season.config["south_game_enabled"]:
+            season = await season_repo.get_by_pk(group.running_season_id)
+            if season.config.south_game_enabled:
                 player_and_wind = PlayerAndWind.four_men_south
             else:
                 player_and_wind = PlayerAndWind.four_men_east
         else:
             player_and_wind = PlayerAndWind.four_men_south
     else:
         if group.running_season_id is not None:
-            season = await session.get(SeasonOrm, group.running_season_id)
-            if player_and_wind == PlayerAndWind.four_men_south and not season.config["south_game_enabled"] \
-                    or player_and_wind == PlayerAndWind.four_men_east and not season.config["east_game_enabled"]:
+            season = await season_repo.get_by_pk(group.running_season_id)
+            if player_and_wind == PlayerAndWind.four_men_south and not season.config.south_game_enabled \
+                    or player_and_wind == PlayerAndWind.four_men_east and not season.config.east_game_enabled:
                 raise BadRequestError("当前赛季未开放此类型对局")
 
     game = GameOrm(code=game_code,
-                   group_id=group.id,
-                   promoter_user_id=promoter.id,
+                   group_id=group_id,
+                   promoter_user_id=promoter_user_id,
                    player_and_wind=player_and_wind,
                    season_id=group.running_season_id,
                    records=[])
 
     session.add(game)
     await session.commit()
-    return game
-
-
-def _build_game_query(stmt: Select,
-                      *, offset: Optional[int] = None,
-                      limit: Optional[int] = None,
-                      uncompleted_only: bool = False,
-                      completed_only: bool = False,
-                      reverse_order: bool = False,
-                      time_span: Optional[Tuple[datetime, datetime]] = None) -> Select:
-    if uncompleted_only:
-        stmt = stmt.where(GameOrm.state != GameState.completed)
-    elif completed_only:
-        stmt = stmt.where(GameOrm.state == GameState.completed)
-
-    if reverse_order:
-        stmt = stmt.order_by(GameOrm.id.desc())
-    else:
-        stmt = stmt.order_by(GameOrm.id)
-
-    if time_span:
-        stmt = stmt.where(GameOrm.create_time >= time_span[0])
-        stmt = stmt.where(GameOrm.create_time < time_span[1])
-
-    stmt = stmt.where(GameOrm.accessible)
-
-    stmt = (stmt.offset(offset).limit(limit)
-            .options(selectinload(GameOrm.records)))
-
-    return stmt
-
-
-async def get_game_by_code(game_code: int, group: GroupOrm) -> Optional[GameOrm]:
-    session = data_source.session()
-
-    stmt = select(GameOrm).where(
-        GameOrm.group == group, GameOrm.code == game_code
-    )
-    stmt = _build_game_query(stmt, limit=1)
-    game = (await session.execute(stmt)).scalar_one_or_none()
-    return game
-
-
-@overload
-async def get_games(group: Optional[GroupOrm] = ...,
-                    user: Optional[UserOrm] = ...,
-                    season: Optional[SeasonOrm] = ...,
-                    *, uncompleted_only: bool = False,
-                    completed_only: bool = False,
-                    offset: Optional[int] = None,
-                    limit: Optional[int] = None,
-                    reverse_order: bool = False,
-                    time_span: Optional[Tuple[datetime, datetime]] = None) -> List[GameOrm]:
-    ...
-
-
-async def get_games(group: Optional[GroupOrm] = None,
-                    user: Optional[UserOrm] = None,
-                    season: Optional[SeasonOrm] = None,
-                    **kwargs) -> List[GameOrm]:
-    session = data_source.session()
+    await session.refresh(game)
 
-    stmt = select(GameOrm)
+    return await map_game(game, session)
 
-    if group is not None:
-        stmt = stmt.where(GameOrm.group == group)
 
-    if user is not None:
-        stmt = stmt.join(GameRecordOrm).where(GameRecordOrm.user == user)
-
-    if season is not None:
-        stmt = stmt.where(GameOrm.season == season)
-
-    stmt = _build_game_query(stmt, **kwargs)
-
-    result = await session.execute(stmt)
-    return [row[0] for row in result]
-
-
-async def _ensure_updatable(game: GameOrm):
+async def get_game(game_code: int, group_id: int) -> Game:
     session = data_source.session()
-    if game.season_id is not None:
-        season = await session.get(SeasonOrm, game.season_id)
-        if season.state != SeasonState.running:
-            raise BadRequestError("赛季已经结束，无法再修改对局")
-
-
-async def _ensure_permission(game: GameOrm, group: GroupOrm, operator: UserOrm):
-    if game.state == GameState.completed:
-        completed_before_24h = datetime.utcnow() - game.complete_time >= timedelta(days=1)
-
-        if not completed_before_24h or await is_group_admin(operator, group):
-            return
-
-        raise BadRequestError("对局已完成超过24小时，需要管理员权限才能操作")
+    game_repo = GameRepository(session)
+    game = await game_repo.get_by_code(game_code, group_id)
+    return await map_game(game, session)
 
 
 async def record_game(game_code: int,
-                      group: GroupOrm,
-                      user: UserOrm,
+                      group_id: int,
+                      user_id: int,
                       score: int,
                       wind: Optional[Wind],
-                      operator: UserOrm) -> GameOrm:
+                      operator_user_id: int) -> Game:
     session = data_source.session()
 
-    game = await get_game_by_code(game_code, group)
+    game_repo = GameRepository(session)
+    season_repo = SeasonRepository(session)
+
+    game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
         raise BadRequestError("未找到指定对局")
 
     await _ensure_updatable(game)
-    await _ensure_permission(game, group, operator)
+    await _ensure_permission(game, group_id, operator_user_id)
 
     for r in game.records:
-        if r.user_id == user.id:
+        if r.user_id == user_id:
             record = r
             break
     else:
         if len(game.records) == 4:
             raise BadRequestError("这场对局已经存在4人记录")
 
-        record = GameRecordOrm(game_id=game.id, user_id=user.id)
+        record = GameRecordOrm(game_id=game.id, user_id=user_id)
         session.add(record)
         game.records.append(record)
 
     if game.state == GameState.completed and game.season_id:
-        await revert_season_user_point_by_game(game)
+        await season_repo.revert_season_user_point_by_game(game)
 
     game.state = GameState.uncompleted
     record.score = score
     record.wind = wind
 
     if len(game.records) == 4:
         await _handle_full_recorded_game(game)
 
     game.update_time = datetime.utcnow()
     await session.commit()
-    return game
+    return await map_game(game, session)
 
 
 async def _handle_full_recorded_game(game: GameOrm):
     session = data_source.session()
 
-    progress = await session.get(GameProgressOrm, game.id)
+    game_repo = GameRepository(session)
+    season_repo = SeasonRepository(session)
+
+    progress = await game_repo.get_progress(game.id)
     if progress is not None:
         return
 
     # 总分校验
     sum_score = sum(map(lambda r: r.score, game.records))
     if sum_score != 25000 * 4:
         game.state = GameState.invalid_total_point
@@ -241,15 +172,15 @@
     game.state = GameState.completed
     game.complete_time = datetime.utcnow()
 
     # 计算pt
     if not game.season_id:
         return
 
-    season = await session.get(SeasonOrm, game.season_id)
+    season = await season_repo.get_by_pk(game.season_id)
     if game.player_and_wind == PlayerAndWind.four_men_east:
         horse_point = season.config.east_game_horse_point
         origin_point = season.config.east_game_origin_point
     elif game.player_and_wind == PlayerAndWind.four_men_south:
         horse_point = season.config.south_game_horse_point
         origin_point = season.config.south_game_origin_point
     else:
@@ -294,15 +225,15 @@
         r.raw_point = ceil(horse_point[i] + (r.score - origin_point) * (10 ** (-point_scale - 3)))
         r.point_scale = point_scale
 
         if i == 0 or indexed_record[i - 1][0].raw_point != r.raw_point:
             rank += 1
         r.rank = rank
 
-    await change_season_user_point_by_game(game)
+    await season_repo.change_season_user_point_by_game(game)
 
 
 def _divide_horse_point(horse_point: List[int], start: int, end: int):
     sum_horse_point = sum(horse_point[start:end + 1])
     divided_horse_point = sum_horse_point // (end - start + 1)
 
     for i in range(start, end + 1):
@@ -311,187 +242,216 @@
     # 除不尽的部分给第一个
     if divided_horse_point * (end - start + 1) != sum_horse_point:
         rest_horse_point = sum_horse_point - divided_horse_point * (end - start + 1)
         horse_point[start] += rest_horse_point
 
 
 async def revert_record(game_code: int,
-                        group: GroupOrm,
-                        user: UserOrm,
-                        operator: UserOrm) -> GameOrm:
+                        group_id: int,
+                        user_id: int,
+                        operator_user_id: int) -> Game:
     session = data_source.session()
 
-    game = await get_game_by_code(game_code, group)
+    game_repo = GameRepository(session)
+    season_repo = SeasonRepository(session)
+
+    game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
         raise BadRequestError("未找到指定对局")
 
     await _ensure_updatable(game)
-    await _ensure_permission(game, group, operator)
+    await _ensure_permission(game, group_id, operator_user_id)
 
     for r in game.records:
-        if r.user_id == user.id:
+        if r.user_id == user_id:
             record = r
             break
     else:
         raise BadRequestError("你还没有记录过这场对局")
 
     if game.state == GameState.completed and game.season_id:
-        await revert_season_user_point_by_game(game)
+        await season_repo.revert_season_user_point_by_game(game)
 
     game.state = GameState.uncompleted
     game.records.remove(record)
     await session.delete(record)
 
     game.update_time = datetime.utcnow()
     await session.commit()
-    return game
+    return await map_game(game, session)
 
 
 async def delete_game(game_code: int,
-                      group: GroupOrm,
-                      operator: UserOrm):
+                      group_id: int,
+                      operator_user_id: int):
     session = data_source.session()
 
-    game = await get_game_by_code(game_code, group)
+    game_repo = GameRepository(session)
+    season_repo = SeasonRepository(session)
+
+    game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
         raise BadRequestError("未找到指定对局")
 
     await _ensure_updatable(game)
 
-    if not await is_group_admin(operator, group):
+    if not await is_group_admin(operator_user_id, group_id):
         raise BadRequestError("需要管理员权限进行该操作")
 
     if game.state == GameState.completed and game.season_id:
-        await revert_season_user_point_by_game(game)
+        await season_repo.revert_season_user_point_by_game(game)
 
     game.accessible = False
     game.delete_time = datetime.utcnow()
     game.update_time = datetime.utcnow()
     await session.commit()
 
 
-async def delete_uncompleted_season_games(season: SeasonOrm):
+async def delete_uncompleted_season_games(season_id: int):
     session = data_source.session()
-    now = datetime.utcnow()
-    stmt = (update(GameOrm)
-            .where(GameOrm.season == season, GameOrm.state != GameState.completed, GameOrm.accessible)
-            .values(accessible=False, delete_time=now, update_time=now)
-            .execution_options(synchronize_session=False))
-    await session.execute(stmt)
-    await session.commit()
+    repo = SeasonRepository(session)
+    await repo.delete_uncompleted_games(season_id)
 
 
 async def make_game_progress(game_code: int, round: int, honba: int,
-                             group: GroupOrm, operator: UserOrm):
+                             group_id: int, operator_user_id: int):
     session = data_source.session()
 
-    game = await get_game_by_code(game_code, group)
+    game_repo = GameRepository(session)
+    season_repo = SeasonRepository(session)
+
+    game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
         raise BadRequestError("未找到指定对局")
 
     await _ensure_updatable(game)
-    await _ensure_permission(game, group, operator)
+    await _ensure_permission(game, group_id, operator_user_id)
 
     if game.state == GameState.completed and game.season_id:
-        await revert_season_user_point_by_game(game)
+        await season_repo.revert_season_user_point_by_game(game)
 
     game.state = GameState.uncompleted
 
-    progress = await session.get(GameProgressOrm, game.id)
+    progress = await game_repo.get_progress(game.id)
     if progress is None:
         progress = GameProgressOrm(game_id=game.id)
         session.add(progress)
 
     progress.round = round
     progress.honba = honba
 
     game.update_time = datetime.utcnow()
     await session.commit()
-    return game
+    return await map_game(game, session)
 
 
-async def remove_game_progress(game_code: int, group: GroupOrm):
+async def remove_game_progress(game_code: int, group_id: int):
     session = data_source.session()
 
-    game = await get_game_by_code(game_code, group)
+    game_repo = GameRepository(session)
+
+    game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
         raise BadRequestError("未找到指定对局")
 
     await _ensure_updatable(game)
 
-    progress = await session.get(GameProgressOrm, game.id)
+    progress = await game_repo.get_progress(game.id)
     if progress is not None:
         # 不能用session.delete，否则之后session.get还能获取到
         stmt = delete(GameProgressOrm).where(GameProgressOrm.game_id == game.id)
         await session.execute(stmt)
 
         if len(game.records) == 4:
             await _handle_full_recorded_game(game)
 
     game.update_time = datetime.utcnow()
     await session.commit()
-    return game
+    return await map_game(game, session)
 
 
-async def set_record_point(game_code: int, group: GroupOrm, user: UserOrm, point: float, operator: UserOrm):
+async def set_record_point(game_code: int, group_id: int, user_id: int, point: float, operator_user_id: int):
     session = data_source.session()
 
-    game = await get_game_by_code(game_code, group)
+    game_repo = GameRepository(session)
+    season_repo = SeasonRepository(session)
+
+    game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
         raise BadRequestError("未找到指定对局")
 
     await _ensure_updatable(game)
-    await _ensure_permission(game, group, operator)
+    await _ensure_permission(game, group_id, operator_user_id)
 
     for r in game.records:
-        if r.user_id == user.id:
+        if r.user_id == user_id:
             record = r
             break
     else:
-        raise BadRequestError("你还没有记录过这场对局")
+        raise BadRequestError("用户还没有记录过这场对局")
 
     if game.state != GameState.completed:
         raise BadRequestError("这场对局未处于完成状态")
 
     if game.season_id is None:
         raise BadRequestError("这场对局不属于赛季")
 
-    await revert_season_user_point_by_game(game)
+    await season_repo.revert_season_user_point_by_game(game)
 
-    season = await session.get(SeasonOrm, group.season_id)
+    season = await season_repo.get_by_pk(game.season_id)
     record.point_scale = season.config.point_precision
     record.raw_point = int(point * (10 ** -season.config.point_precision))
 
-    await change_season_user_point_by_game(game)
+    await season_repo.change_season_user_point_by_game(game)
 
     game.update_time = datetime.utcnow()
     await session.commit()
-    return game
+    return await map_game(game, session)
 
 
-async def set_game_comment(game_code: int, group: GroupOrm, comment: str, operator: UserOrm):
+async def set_game_comment(game_code: int, group_id: int, comment: str, operator_user_id: int):
     session = data_source.session()
 
-    game = await get_game_by_code(game_code, group)
+    game_repo = GameRepository(session)
+
+    game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
         raise BadRequestError("未找到指定对局")
 
     await _ensure_updatable(game)
-    await _ensure_permission(game, group, operator)
+    await _ensure_permission(game, group_id, operator_user_id)
 
     game.comment = comment
 
     game.update_time = datetime.utcnow()
     await session.commit()
-    return game
+    return await map_game(game, session)
 
 
-async def get_game_statistics(group: GroupOrm, user: UserOrm, season: Optional[SeasonOrm] = None):
-    games = await get_games(group, user, season, completed_only=True)
+@overload
+async def get_games(group_id: int, user_id: Optional[int] = None, season_id: Optional[int] = None,
+                    *, uncompleted_only: bool = ...,
+                    completed_only: bool = ...,
+                    offset: Optional[int] = ...,
+                    limit: Optional[int] = ...,
+                    reverse_order: bool = ...,
+                    time_span: Optional[Tuple[datetime, datetime]] = ...) -> List[Game]:
+    ...
+
+
+async def get_games(group_id: int, user_id: Optional[int] = None, season_id: Optional[int] = None, **kwargs) -> \
+        List[Game]:
+    session = data_source.session()
+    game_repo = GameRepository(session)
+    games = await game_repo.get(group_id, user_id, season_id, **kwargs)
+    return [await map_game(g, session) for g in games]
 
+
+def _get_game_statistics_by_games(games: List[GameOrm], user_id: int,
+                                  is_same_season: bool = False) -> GameStatistics:
     if len(games) == 0:
         raise BadRequestError("你还没有进行对局")
 
     total = len(games)
 
     total_east = 0
     total_south = 0
@@ -506,35 +466,52 @@
 
     sum_point = 0.0
 
     flying = 0
 
     for g in games:
         for r in g.records:
-            if r.user_id == user.id:
+            if r.user_id == user_id:
                 cnt[r.rank - 1] += 1
 
                 if r.score < 0:
                     flying += 1
 
                 sum_point += r.point
 
                 break
 
     rates = list(map(lambda x: x / total, cnt))
 
     avg_rank = (cnt[0] * 1 + cnt[1] * 2 + cnt[2] * 3 + cnt[3] * 4) / total
 
-    if season is not None:
+    if is_same_season:
         pt_expectation = sum_point / total
     else:
         pt_expectation = None
 
     flying_rate = flying / total
 
     return GameStatistics(total, total_east, total_south, rates, avg_rank, pt_expectation, flying_rate)
 
 
-__all__ = ("get_game_by_code", "get_games",
-           "new_game", "delete_game", "record_game", "revert_record", "set_record_point",
+async def get_game_statistics(group_id: int, user_id: int):
+    session = data_source.session()
+
+    game_repo = GameRepository(session)
+    games = await game_repo.get(group_id, user_id, completed_only=True)
+    return _get_game_statistics_by_games(games, user_id)
+
+
+async def get_season_game_statistics(group_id: int, user_id: int, season_id: int):
+    session = data_source.session()
+
+    season = await session.get(SeasonOrm, season_id)
+
+    game_repo = GameRepository(session)
+    games = await game_repo.get(group_id, user_id, season.id, completed_only=True)
+    return _get_game_statistics_by_games(games, user_id, is_same_season=True)
+
+
+__all__ = ("new_game", "delete_game", "record_game", "revert_record", "set_record_point",
            "make_game_progress", "remove_game_progress",
            "delete_uncompleted_season_games")
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/repository/season.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,239 +1,241 @@
 from datetime import datetime
-from operator import and_
-from typing import Optional, List, Literal, overload, Tuple, Union
+from typing import Optional, List, overload, Literal, Tuple, Union
 
-from sqlalchemy import delete
-from sqlalchemy.future import select
-from sqlalchemy.sql.functions import count, func
-
-from nonebot_plugin_mahjong_scoreboard.errors import BadRequestError
-from nonebot_plugin_mahjong_scoreboard.model.enums import SeasonUserPointChangeType
-from nonebot_plugin_mahjong_scoreboard.model.orm import data_source
-from nonebot_plugin_mahjong_scoreboard.model.orm.game import GameOrm, GameRecordOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.group import GroupOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.season import SeasonOrm, SeasonUserPointOrm, \
-    SeasonUserPointChangeLogOrm
-from nonebot_plugin_mahjong_scoreboard.model.orm.user import UserOrm
-from nonebot_plugin_mahjong_scoreboard.service.group_service import is_group_admin
-from nonebot_plugin_mahjong_scoreboard.utils.rank import ranked
-
-
-async def get_season_user_points(season: SeasonOrm) -> List[SeasonUserPointOrm]:
-    session = data_source.session()
-
-    stmt = select(SeasonUserPointOrm).where(
-        SeasonUserPointOrm.season == season
-    ).order_by(SeasonUserPointOrm.point.desc())
-    sup = (await session.execute(stmt)).scalars().all()
-    return sup
-
-
-@overload
-async def get_season_user_point_change_logs(season: Optional[SeasonOrm],
-                                            user: Optional[UserOrm] = ...,
-                                            *, offset: Optional[int] = ...,
-                                            limit: Optional[int] = ...,
-                                            reverse_order: bool = ...,
-                                            join_game_and_record: Literal[False] = ...) \
-        -> List[SeasonUserPointChangeLogOrm]:
-    ...
-
-
-@overload
-async def get_season_user_point_change_logs(season: Optional[SeasonOrm],
-                                            user: Optional[UserOrm] = ...,
-                                            *, offset: Optional[int] = ...,
-                                            limit: Optional[int] = ...,
-                                            reverse_order: bool = ...,
-                                            join_game_and_record: Literal[True] = ...) \
-        -> List[Tuple[SeasonUserPointChangeLogOrm, GameOrm, GameRecordOrm]]:
-    ...
-
-
-async def get_season_user_point_change_logs(season: Optional[SeasonOrm] = None,
-                                            user: Optional[UserOrm] = None,
-                                            *, offset: Optional[int] = None,
-                                            limit: Optional[int] = None,
-                                            reverse_order: bool = False,
-                                            join_game_and_record: bool = False) \
-        -> Union[List[SeasonUserPointChangeLogOrm], List[Tuple[SeasonUserPointChangeLogOrm, GameOrm, GameRecordOrm]]]:
-    session = data_source.session()
-
-    if not join_game_and_record:
-        stmt = select(SeasonUserPointChangeLogOrm)
-    else:
-        stmt = (select(SeasonUserPointChangeLogOrm, GameOrm, GameRecordOrm)
-                .join_from(SeasonUserPointChangeLogOrm, GameOrm,
-                           SeasonUserPointChangeLogOrm.related_game_id == GameOrm.id)
-                .join_from(SeasonUserPointChangeLogOrm, GameRecordOrm,
-                           and_(
-                               SeasonUserPointChangeLogOrm.related_game_id == GameRecordOrm.game_id,
-                               SeasonUserPointChangeLogOrm.user_id == GameRecordOrm.user_id
-                           )))
-
-    if season is not None:
-        stmt = stmt.where(SeasonUserPointChangeLogOrm.season == season)
-
-    if user is not None:
-        stmt = stmt.where(SeasonUserPointChangeLogOrm.user == user)
-
-    if reverse_order:
-        stmt = stmt.order_by(SeasonUserPointChangeLogOrm.id.desc())
-    else:
-        stmt = stmt.order_by(SeasonUserPointChangeLogOrm.id)
-
-    stmt = stmt.offset(offset).limit(limit)
-
-    result = (await session.execute(stmt)).all()
-    if join_game_and_record:
-        return [(a, b, c) for (a, b, c) in result]
-    else:
-        return [x for (x,) in result]
-
-
-async def get_season_user_point(season: SeasonOrm, user: UserOrm) -> Optional[SeasonUserPointOrm]:
-    session = data_source.session()
-
-    stmt = select(SeasonUserPointOrm).where(
-        SeasonUserPointOrm.season == season, SeasonUserPointOrm.user == user
-    ).limit(1)
-    sup: Optional[SeasonUserPointOrm] = (await session.execute(stmt)).scalar_one_or_none()
-    return sup
-
-
-async def get_season_user_point_rank(sup: SeasonUserPointOrm) -> int:
-    session = data_source.session()
-    stmt = select(count(SeasonUserPointOrm.user_id)).where(
-        SeasonUserPointOrm.season_id == sup.season_id, SeasonUserPointOrm.point > sup.point
-    )
-    result = (await session.execute(stmt)).scalar_one_or_none()
-    return result + 1
-
-
-async def count_season_user_point(season: SeasonOrm) -> Optional[SeasonUserPointOrm]:
-    session = data_source.session()
-
-    stmt = select(count(SeasonUserPointOrm.user_id)).where(
-        SeasonUserPointOrm.season == season
-    )
-    result = (await session.execute(stmt)).scalar_one_or_none()
-    return result
-
-
-async def reset_season_user_point(season: SeasonOrm,
-                                  user: UserOrm,
-                                  operator: UserOrm):
-    session = data_source.session()
-
-    group = await session.get(GroupOrm, season.group_id)
-    if not await is_group_admin(operator, group):
-        raise BadRequestError("没有权限")
-
-    sup = await get_season_user_point(season, user)
-    if sup is None:
-        return
-
-    stmt = delete(SeasonUserPointChangeLogOrm).where(
-        SeasonUserPointChangeLogOrm.season_id == sup.season_id,
-        SeasonUserPointChangeLogOrm.user_id == sup.user_id
-    )
-    await session.execute(stmt)
-
-    await session.delete(sup)
-    await session.commit()
-
-
-async def change_season_user_point_manually(season: SeasonOrm,
-                                            user: UserOrm,
-                                            point: float,
-                                            operator: UserOrm) -> SeasonUserPointOrm:
-    session = data_source.session()
-    group = await session.get(GroupOrm, season.group_id)
-    if not await is_group_admin(operator, group):
-        raise BadRequestError("没有权限")
-
-    sup = await get_season_user_point(season, user)
-    if sup is None:
-        sup = SeasonUserPointOrm(season=season, user=user)
-        session.add(sup)
-
-    sup.point = int(point * (10 ** -season.config.point_precision))
-
-    log = SeasonUserPointChangeLogOrm(season=season, user=user,
-                                      change_type=SeasonUserPointChangeType.manually,
-                                      change_point=point)
-    session.add(log)
-
-    sup.update_time = datetime.utcnow()
-    await session.commit()
-    return sup
+from sqlalchemy import update, select, and_, delete, func
+from sqlalchemy.sql.functions import count
 
+from .base import Repository
+from .data_model import GameOrm, GameRecordOrm, SeasonOrm, SeasonUserPointOrm, SeasonUserPointChangeLogOrm
+from ..errors import BadRequestError
+from ..model.enums import GameState, SeasonUserPointChangeType
+from ..utils.rank import ranked
+
+
+class SeasonRepository(Repository[SeasonOrm]):
+    async def get_by_pk(self, pk: int) -> Optional[SeasonOrm]:
+        stmt = select(SeasonOrm).where(
+            SeasonOrm.id == pk,
+            SeasonOrm.accessible
+        ).limit(1)
+        season = (await self.session.execute(stmt)).scalar_one_or_none()
+        return season
 
-async def change_season_user_point_by_game(game: GameOrm):
-    session = data_source.session()
-
-    for rank, r in ranked(game.records, key=lambda r: r.raw_point, reverse=True):
-        # 记录SeasonUserPoint
-        stmt = select(SeasonUserPointOrm).where(
-            SeasonUserPointOrm.season_id == game.season_id,
-            SeasonUserPointOrm.user_id == r.user_id
+    async def get_by_code(self, season_code: str, group_id: int) -> Optional[SeasonOrm]:
+        stmt = select(SeasonOrm).where(
+            SeasonOrm.group_id == group_id,
+            SeasonOrm.code == season_code,
+            SeasonOrm.accessible
         ).limit(1)
-        user_point = (await session.execute(stmt)).scalar_one_or_none()
+        season = (await self.session.execute(stmt)).scalar_one_or_none()
+        return season
 
-        if user_point is None:
-            user_point = SeasonUserPointOrm(season_id=game.season_id,
-                                            user_id=r.user_id,
-                                            point=0)
-            session.add(user_point)
-
-        user_point.point += r.raw_point
-
-        # 记录SeasonUserPointChangeLog
-        change_log = SeasonUserPointChangeLogOrm(user_id=r.user_id,
-                                                 season_id=game.season_id,
-                                                 change_type=SeasonUserPointChangeType.game,
-                                                 change_point=r.raw_point,
-                                                 related_game_id=game.id)
-        session.add(change_log)
-
-    await session.commit()
-
-
-async def revert_season_user_point_by_game(game: GameOrm):
-    session = data_source.session()
-
-    stmt = select(SeasonUserPointChangeLogOrm, SeasonUserPointOrm).join_from(
-        SeasonUserPointChangeLogOrm, SeasonUserPointOrm, and_(
-            SeasonUserPointChangeLogOrm.season_id == SeasonUserPointOrm.season_id,
-            SeasonUserPointChangeLogOrm.user_id == SeasonUserPointOrm.user_id,
+    async def get_group_seasons(self, group_id: int) -> List[SeasonOrm]:
+        stmt = select(SeasonOrm).where(
+            SeasonOrm.group_id == group_id,
+            SeasonOrm.accessible
         )
-    ).where(
-        SeasonUserPointChangeLogOrm.related_game_id == game.id
-    )
-
-    for change_log, user_point in await session.execute(stmt):
-        # 判断在此之后是否还变动过PT
-        stmt = select(func.count(SeasonUserPointChangeLogOrm.id)).where(
-            SeasonUserPointChangeLogOrm.season_id == change_log.season_id,
-            SeasonUserPointChangeLogOrm.user_id == change_log.user_id,
-            SeasonUserPointChangeLogOrm.id > change_log.id
+        result = await self.session.execute(stmt)
+        return [row[0] for row in result]
+
+    async def delete_uncompleted_games(self, season_id: int) -> int:
+        now = datetime.utcnow()
+        stmt = (update(GameOrm)
+                .where(GameOrm.season_id == season_id, GameOrm.state != GameState.completed, GameOrm.accessible)
+                .values(accessible=False, delete_time=now, update_time=now)
+                .execution_options(synchronize_session=False))
+        result = await self.session.execute(stmt)
+        await self.session.commit()
+        return result.rowcount
+
+    async def get_season_user_point(self, season_id: int, user_id: int,
+                                    *, insert_on_missing: bool = False) -> Optional[SeasonUserPointOrm]:
+        stmt = select(SeasonUserPointOrm).where(
+            SeasonUserPointOrm.season_id == season_id, SeasonUserPointOrm.user_id == user_id
+        ).limit(1)
+        sup = (await self.session.execute(stmt)).scalar_one_or_none()
+        if sup is None and insert_on_missing:
+            sup = SeasonUserPointOrm(season_id=season_id, user_id=user_id)
+            self.session.add(sup)
+            await self.session.commit()
+        return sup
+
+    async def get_season_user_point_rank(self, season_id: int, point: int) -> int:
+        stmt = select(count(SeasonUserPointOrm.user_id)).where(
+            SeasonUserPointOrm.season_id == season_id, SeasonUserPointOrm.point > point
         )
-        cnt = (await session.execute(stmt)).scalar_one()
+        result = (await self.session.execute(stmt)).scalar_one_or_none()
+        return result + 1
 
-        if cnt != 0:
-            raise BadRequestError("撤销结算失败，在该对局之后该用户PT发生了改变")
+    async def count_season_user_point(self, season_id: int) -> Optional[SeasonUserPointOrm]:
+        stmt = select(count(SeasonUserPointOrm.user_id)).where(
+            SeasonUserPointOrm.season_id == season_id
+        )
+        result = (await self.session.execute(stmt)).scalar_one_or_none()
+        return result
 
-        user_point.point -= change_log.change_point
-        await session.delete(change_log)
+    async def get_season_user_points(self, season_id: int) -> List[SeasonUserPointOrm]:
+        stmt = select(SeasonUserPointOrm).where(
+            SeasonUserPointOrm.season_id == season_id
+        ).order_by(SeasonUserPointOrm.point.desc())
+        sup = (await self.session.execute(stmt)).scalars().all()
+        return sup
+
+    @overload
+    async def get_season_user_point_change_logs(self, season_id: Optional[int] = ...,
+                                                user_id: Optional[int] = ...,
+                                                *, offset: Optional[int] = ...,
+                                                limit: Optional[int] = ...,
+                                                reverse_order: bool = ...,
+                                                join_game_and_record: Literal[False] = ...) \
+            -> List[SeasonUserPointChangeLogOrm]:
+        ...
+
+    @overload
+    async def get_season_user_point_change_logs(self, season_id: Optional[int] = ...,
+                                                user_id: Optional[int] = ...,
+                                                *, offset: Optional[int] = ...,
+                                                limit: Optional[int] = ...,
+                                                reverse_order: bool = ...,
+                                                join_game_and_record: Literal[True] = ...) \
+            -> List[Tuple[SeasonUserPointChangeLogOrm, GameOrm, GameRecordOrm]]:
+        ...
+
+    async def get_season_user_point_change_logs(self, season_id: Optional[int] = None,
+                                                user_id: Optional[int] = None,
+                                                *, offset: Optional[int] = None,
+                                                limit: Optional[int] = None,
+                                                reverse_order: bool = False,
+                                                join_game_and_record: bool = False) \
+            -> Union[
+                List[SeasonUserPointChangeLogOrm],
+                List[Tuple[SeasonUserPointChangeLogOrm, GameOrm, GameRecordOrm]]
+            ]:
+        if not join_game_and_record:
+            stmt = select(SeasonUserPointChangeLogOrm)
+        else:
+            stmt = (select(SeasonUserPointChangeLogOrm, GameOrm, GameRecordOrm)
+                    .join_from(SeasonUserPointChangeLogOrm, GameOrm,
+                               SeasonUserPointChangeLogOrm.related_game_id == GameOrm.id)
+                    .join_from(SeasonUserPointChangeLogOrm, GameRecordOrm,
+                               and_(
+                                   SeasonUserPointChangeLogOrm.related_game_id == GameRecordOrm.game_id,
+                                   SeasonUserPointChangeLogOrm.user_id == GameRecordOrm.user_id
+                               )))
+
+        if season_id is not None:
+            stmt = stmt.where(SeasonUserPointChangeLogOrm.season_id == season_id)
+
+        if user_id is not None:
+            stmt = stmt.where(SeasonUserPointChangeLogOrm.user_id == user_id)
+
+        if reverse_order:
+            stmt = stmt.order_by(SeasonUserPointChangeLogOrm.id.desc())
+        else:
+            stmt = stmt.order_by(SeasonUserPointChangeLogOrm.id)
+
+        stmt = stmt.offset(offset).limit(limit)
+
+        result = (await self.session.execute(stmt)).all()
+        if join_game_and_record:
+            return [(a, b, c) for (a, b, c) in result]
+        else:
+            return [x for (x,) in result]
+
+    async def change_season_user_point_manually(self, season_id: int,
+                                                user_id: int,
+                                                point: float) -> SeasonUserPointOrm:
+        season = await self.get_by_pk(season_id)
+        sup = await self.get_season_user_point(season_id, user_id, insert_on_missing=True)
+
+        sup.point = int(point * (10 ** -season.config.point_precision))
+
+        log = SeasonUserPointChangeLogOrm(season_id=season.id, user_id=user_id,
+                                          change_type=SeasonUserPointChangeType.manually,
+                                          change_point=point)
+        self.session.add(log)
+
+        sup.update_time = datetime.utcnow()
+        await self.session.commit()
+
+        return sup
+
+    async def change_season_user_point_by_game(self, game: GameOrm):
+        for rank, r in ranked(game.records, key=lambda r: r.raw_point, reverse=True):
+            # 记录SeasonUserPoint
+            stmt = select(SeasonUserPointOrm).where(
+                SeasonUserPointOrm.season_id == game.season_id,
+                SeasonUserPointOrm.user_id == r.user_id
+            ).limit(1)
+            user_point = (await self.session.execute(stmt)).scalar_one_or_none()
+
+            if user_point is None:
+                user_point = SeasonUserPointOrm(season_id=game.season_id,
+                                                user_id=r.user_id,
+                                                point=0)
+                self.session.add(user_point)
+
+            user_point.point += r.raw_point
+
+            # 记录SeasonUserPointChangeLog
+            change_log = SeasonUserPointChangeLogOrm(user_id=r.user_id,
+                                                     season_id=game.season_id,
+                                                     change_type=SeasonUserPointChangeType.game,
+                                                     change_point=r.raw_point,
+                                                     related_game_id=game.id)
+            self.session.add(change_log)
+
+        await self.session.commit()
+
+    async def revert_season_user_point_by_game(self, game: GameOrm):
+        stmt = select(SeasonUserPointChangeLogOrm, SeasonUserPointOrm).join_from(
+            SeasonUserPointChangeLogOrm, SeasonUserPointOrm, and_(
+                SeasonUserPointChangeLogOrm.season_id == SeasonUserPointOrm.season_id,
+                SeasonUserPointChangeLogOrm.user_id == SeasonUserPointOrm.user_id,
+            )
+        ).where(
+            SeasonUserPointChangeLogOrm.related_game_id == game.id
+        )
 
-        # 若用户只有这一次PT变动，则删除PT记录
-        stmt = select(func.count(SeasonUserPointChangeLogOrm.id)).where(
-            SeasonUserPointChangeLogOrm.season_id == user_point.season_id,
-            SeasonUserPointChangeLogOrm.user_id == user_point.user_id,
+        for change_log, user_point in await self.session.execute(stmt):
+            # 判断在此之后是否还变动过PT
+            stmt = select(func.count(SeasonUserPointChangeLogOrm.id)).where(
+                SeasonUserPointChangeLogOrm.season_id == change_log.season_id,
+                SeasonUserPointChangeLogOrm.user_id == change_log.user_id,
+                SeasonUserPointChangeLogOrm.id > change_log.id
+            )
+            cnt = (await self.session.execute(stmt)).scalar_one()
+
+            if cnt != 0:
+                raise BadRequestError("撤销结算失败，在该对局之后该用户PT发生了改变")
+
+            user_point.point -= change_log.change_point
+            await self.session.delete(change_log)
+
+            # 若用户只有这一次PT变动，则删除PT记录
+            stmt = select(func.count(SeasonUserPointChangeLogOrm.id)).where(
+                SeasonUserPointChangeLogOrm.season_id == user_point.season_id,
+                SeasonUserPointChangeLogOrm.user_id == user_point.user_id,
+            )
+            cnt = (await self.session.execute(stmt)).scalar_one()
+
+            if cnt == 0:
+                await self.session.delete(user_point)
+
+        await self.session.commit()
+
+    async def reset_season_user_point(self, season_id: int, user_id: int):
+        sup = await self.get_season_user_point(season_id, user_id)
+        if sup is None:
+            return
+
+        stmt = delete(SeasonUserPointChangeLogOrm).where(
+            SeasonUserPointChangeLogOrm.season_id == sup.season_id,
+            SeasonUserPointChangeLogOrm.user_id == sup.user_id
         )
-        cnt = (await session.execute(stmt)).scalar_one()
+        await self.session.execute(stmt)
+
+        await self.session.delete(sup)
+        await self.session.commit()
 
-        if cnt == 0:
-            await session.delete(user_point)
 
-    await session.commit()
+__all__ = ("SeasonOrm", "SeasonUserPointOrm", "SeasonUserPointChangeLogOrm")
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/PKG-INFO` & `nonebot_plugin_mahjong_scoreboard-0.4.0a1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mahjong-scoreboard
-Version: 0.3.1.post1
+Version: 0.4.0a1
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
-Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-file (>=0.1.4,<0.2.0)
-Requires-Dist: nonebot-plugin-sqlalchemy (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-file (>=0.1.5,<0.2.0)
+Requires-Dist: nonebot-plugin-localstore (>=0.4.1,<0.5.0)
+Requires-Dist: nonebot-plugin-session (>=0.0.3,<0.0.4)
+Requires-Dist: nonebot-plugin-sqlalchemy (>=0.2.1,<0.3.0)
 Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: tzlocal (>=4.2,<5.0)
 Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard
 Description-Content-Type: text/plain
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mahjong-scoreboard Version:
-0.3.1.post1 Summary: æ¥éº»å¯åå¨ï¼NoneBotæä»¶ï¼ Home-page: https://
-github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard License: MIT Author:
-ssttkkl Author-email: huang.wen.long@hotmail.com Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: aiosqlite (>=0.17,<0.19) Requires-
-Dist: cachetools (>=5.2.0,<6.0.0) Requires-Dist: nonebot-adapter-onebot
+Metadata-Version: 2.1 Name: nonebot-plugin-mahjong-scoreboard Version: 0.4.0a1
+Summary: æ¥éº»å¯åå¨ï¼NoneBotæä»¶ï¼ Home-page: https://github.com/
+ssttkkl/nonebot-plugin-mahjong-scoreboard License: MIT Author: ssttkkl Author-
+email: huang.wen.long@hotmail.com Requires-Python: >=3.9,<4.0 Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: aiosqlite (>=0.17,<0.19) Requires-Dist:
+cachetools (>=5.2.0,<6.0.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-
-file (>=0.1.4,<0.2.0) Requires-Dist: nonebot-plugin-sqlalchemy (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Requires-Dist:
-nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist: tzlocal (>=4.2,<5.0)
-Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-mahjong-
-scoreboard Description-Content-Type: text/plain
+file (>=0.1.5,<0.2.0) Requires-Dist: nonebot-plugin-localstore (>=0.4.1,<0.5.0)
+Requires-Dist: nonebot-plugin-session (>=0.0.3,<0.0.4) Requires-Dist: nonebot-
+plugin-sqlalchemy (>=0.2.1,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
+Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
+tzlocal (>=4.2,<5.0) Project-URL: Repository, https://github.com/ssttkkl/
+nonebot-plugin-mahjong-scoreboard Description-Content-Type: text/plain
                                    [nonebot]
           nonebot-plugin-mahjong-scoreboard ============ _â¨ NoneBot
                           æ¥éº»è®°åå¨æä»¶ â¨_
                            [license] [pypi] [python]
 æ¯æééå¨ï¼[OneBot V11](https://onebot.adapters.nonebot.dev/
 ) æ¯æé©±å¨å¨ï¼[FastAPI](https://v2.nonebot.dev/docs/tutorial/choose-
 driver) ## åè½
```

