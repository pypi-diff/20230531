# Comparing `tmp/nonebot_plugin_tetris_stats-0.4.0.post1.tar.gz` & `tmp/nonebot_plugin_tetris_stats-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tetris_stats-0.4.0.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_tetris_stats-0.4.1.tar", max compression
```

## Comparing `nonebot_plugin_tetris_stats-0.4.0.post1.tar` & `nonebot_plugin_tetris_stats-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/LICENSE
--rw-r--r--   0        0        0     1043 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/README.md
--rw-r--r--   0        0        0       34 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/__init__.py
--rw-r--r--   0        0        0       72 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
--rw-r--r--   0        0        0     1135 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
--rw-r--r--   0        0        0    12834 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py
--rw-r--r--   0        0        0     5296 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/request.py
--rw-r--r--   0        0        0     8908 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor.py
--rw-r--r--   0        0        0     7272 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor.py
--rw-r--r--   0        0        0       49 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/utils/__init__.py
--rw-r--r--   0        0        0      204 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/utils/config.py
--rw-r--r--   0        0        0     4609 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/utils/database.py
--rw-r--r--   0        0        0     3981 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/utils/message_analyzer.py
--rw-r--r--   0        0        0      895 2023-05-29 22:15:33.854264 nonebot_plugin_tetris_stats-0.4.0.post1/pyproject.toml
--rw-r--r--   0        0        0     2086 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-0.4.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-30 22:25:48.055532 nonebot_plugin_tetris_stats-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1043 2023-05-30 22:25:48.055532 nonebot_plugin_tetris_stats-0.4.1/README.md
+-rw-r--r--   0        0        0       34 2023-05-30 22:25:48.055532 nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/__init__.py
+-rw-r--r--   0        0        0       72 2023-05-30 22:25:48.055532 nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
+-rw-r--r--   0        0        0     1135 2023-05-30 22:25:48.055532 nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
+-rw-r--r--   0        0        0    12834 2023-05-30 22:25:48.059532 nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py
+-rw-r--r--   0        0        0     5296 2023-05-30 22:25:48.059532 nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/request.py
+-rw-r--r--   0        0        0     8908 2023-05-30 22:25:48.059532 nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor.py
+-rw-r--r--   0        0        0     7272 2023-05-30 22:25:48.059532 nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor.py
+-rw-r--r--   0        0        0       49 2023-05-30 22:25:48.059532 nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/utils/__init__.py
+-rw-r--r--   0        0        0      204 2023-05-30 22:25:48.059532 nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/utils/config.py
+-rw-r--r--   0        0        0     4638 2023-05-30 22:25:48.059532 nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/utils/database.py
+-rw-r--r--   0        0        0     3981 2023-05-30 22:25:48.059532 nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/utils/message_analyzer.py
+-rw-r--r--   0        0        0      889 2023-05-30 22:25:48.059532 nonebot_plugin_tetris_stats-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2080 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-0.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_tetris_stats-0.4.0.post1/LICENSE` & `nonebot_plugin_tetris_stats-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.4.0.post1/README.md` & `nonebot_plugin_tetris_stats-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py` & `nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/request.py` & `nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor.py` & `nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor.py` & `nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/utils/database.py` & `nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/utils/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     async def write_rank_info_today(cls, rank: str, trline: int, playercount: int, avgapm: float, avgpps: float, avgvs: float):
         '''写入段位信息'''
 
         db = await cls._get_db()
         cursor = db.cursor()
         cursor.execute('''SELECT TRLINE
                         FROM IORANK
-                        WHERE RANK = ? AND DATE = ?''', (rank, datetime.date.today()))
+                        WHERE RANK = ? AND DATE = ?''', (rank, datetime.date.today() - datetime.timedelta(days=1)))
 
         result = cursor.fetchone()
 
         if result is None:
             trending = '?'
         else:
             if result[0] > trline:
```

### Comparing `nonebot_plugin_tetris_stats-0.4.0.post1/nonebot_plugin_tetris_stats/utils/message_analyzer.py` & `nonebot_plugin_tetris_stats-0.4.1/nonebot_plugin_tetris_stats/utils/message_analyzer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.4.0.post1/pyproject.toml` & `nonebot_plugin_tetris_stats-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-tetris-stats"
-version = "0.4.0.post1"
+version = "0.4.1"
 description = "一个基于nonebot2的用于查询TETRIS相关游戏玩家数据的插件"
 authors = ["scdhh <wallfjjd@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats"
 repository = "https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats"
 license = "MIT"
```

### Comparing `nonebot_plugin_tetris_stats-0.4.0.post1/PKG-INFO` & `nonebot_plugin_tetris_stats-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tetris-stats
-Version: 0.4.0.post1
+Version: 0.4.1
 Summary: 一个基于nonebot2的用于查询TETRIS相关游戏玩家数据的插件
 Home-page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats
 License: MIT
 Author: scdhh
 Author-email: wallfjjd@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

