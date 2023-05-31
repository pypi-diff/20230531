# Comparing `tmp/textworld-1.5.4rc3.tar.gz` & `tmp/textworld-1.5.4rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/textworld-1.5.4rc3.tar", last modified: Wed May 31 14:44:43 2023, max compression
+gzip compressed data, was "dist/textworld-1.5.4rc4.tar", last modified: Wed May 31 15:29:16 2023, max compression
```

## Comparing `textworld-1.5.4rc3.tar` & `textworld-1.5.4rc4.tar`

### file list

```diff
@@ -1,352 +1,352 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/
--rw-r--r--   0 vsts      (1001) docker     (123)     9811 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/CHANGELOG.md
--rw-r--r--   0 vsts      (1001) docker     (123)      915 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/CONTRIBUTING.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      944 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     9180 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     7522 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/glk_build.py
--rw-r--r--   0 vsts      (1001) docker     (123)      385 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/requirements-full.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      160 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/requirements-vis.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      224 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/requirements.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/scripts/
--rwxr-xr-x   0 vsts      (1001) docker     (123)      809 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/scripts/tw-data
--rw-r--r--   0 vsts      (1001) docker     (123)     7207 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/scripts/tw-extract
--rwxr-xr-x   0 vsts      (1001) docker     (123)    12269 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/scripts/tw-make
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2698 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/scripts/tw-play
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1741 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/scripts/tw-stats
--rwxr-xr-x   0 vsts      (1001) docker     (123)      895 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/scripts/tw-view
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     2078 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/setup.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2475 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/setup.sh
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/src/
--rw-r--r--   0 vsts      (1001) docker     (123)     6142 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/src/glk_comm.c
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/
--rw-r--r--   0 vsts      (1001) docker     (123)      573 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/agents/
--rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/agents/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2369 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/agents/human.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1506 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/agents/random.py
--rw-r--r--   0 vsts      (1001) docker     (123)      965 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/agents/simple.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1128 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/agents/walkthrough.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/
--rw-r--r--   0 vsts      (1001) docker     (123)      398 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1380 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/registration.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6704 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/coin_collector.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/logic/
--rw-r--r--   0 vsts      (1001) docker     (123)      787 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/logic/inventory.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      278 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/logic/object.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      236 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/logic/player.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     2288 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/logic/room.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/logic/thing.twl
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/
--rw-r--r--   0 vsts      (1001) docker     (123)    13249 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/house_instruction.twg
--rw-r--r--   0 vsts      (1001) docker     (123)    16075 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/house_obj.twg
--rw-r--r--   0 vsts      (1001) docker     (123)    34339 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/house_room.twg
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    49637 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/cooking.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/
--rw-r--r--   0 vsts      (1001) docker     (123)     1424 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/container.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/door.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     9734 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/food.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     1627 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/inventory.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/key.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     6333 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/meal.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/object.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     1882 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/oven.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      236 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/player.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      176 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/pot.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     2932 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/room.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      932 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/stove.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/supporter.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     1249 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/thing.twl
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/
--rw-r--r--   0 vsts      (1001) docker     (123)     1424 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/container.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/door.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     9786 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/food.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     2212 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/inventory.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/key.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     6688 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/meal.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/object.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     1882 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/oven.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      324 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/player.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      176 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/pot.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     2932 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/room.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      932 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/stove.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/supporter.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     1249 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/thing.twl
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/text_grammars/
--rw-r--r--   0 vsts      (1001) docker     (123)     1059 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_ext_cook.twg
--rw-r--r--   0 vsts      (1001) docker     (123)    13548 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_instruction.twg
--rw-r--r--   0 vsts      (1001) docker     (123)    16270 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_obj.twg
--rw-r--r--   0 vsts      (1001) docker     (123)    34301 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_room.twg
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12409 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/simple.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/
--rw-r--r--   0 vsts      (1001) docker     (123)     1424 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/container.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     2909 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/door.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      682 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/food.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     1805 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/inventory.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/key.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/object.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      236 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/player.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     2902 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/room.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/supporter.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/thing.twl
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/text_grammars/
--rw-r--r--   0 vsts      (1001) docker     (123)    13249 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/text_grammars/house_instruction.twg
--rw-r--r--   0 vsts      (1001) docker     (123)    16075 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/text_grammars/house_obj.twg
--rw-r--r--   0 vsts      (1001) docker     (123)    34339 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/text_grammars/house_room.twg
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/
--rw-r--r--   0 vsts      (1001) docker     (123)     1424 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/container.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     2909 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/door.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      682 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/food.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     1805 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/inventory.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/key.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/object.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      236 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/player.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     2902 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/room.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/supporter.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/thing.twl
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/
--rw-r--r--   0 vsts      (1001) docker     (123)    13249 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/house_instruction.twg
--rw-r--r--   0 vsts      (1001) docker     (123)    16075 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/house_obj.twg
--rw-r--r--   0 vsts      (1001) docker     (123)    34339 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/house_room.twg
--rw-r--r--   0 vsts      (1001) docker     (123)     9383 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/treasure_hunter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1636 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/challenges/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15836 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/core.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/envs/
--rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/envs/batch/
--rw-r--r--   0 vsts      (1001) docker     (123)     1647 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/batch/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8463 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/batch/batch_env.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/envs/glulx/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/glulx/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4952 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/glulx/git_glulx.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6850 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/tw.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/envs/wrappers/
--rw-r--r--   0 vsts      (1001) docker     (123)      422 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/wrappers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2125 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/wrappers/filter.py
--rw-r--r--   0 vsts      (1001) docker     (123)      447 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/wrappers/generic.py
--rw-r--r--   0 vsts      (1001) docker     (123)      843 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/wrappers/limit.py
--rw-r--r--   0 vsts      (1001) docker     (123)      813 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/wrappers/recorder.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14864 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/wrappers/tw_inform7.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2945 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/wrappers/viewer.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/envs/zmachine/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/zmachine/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4768 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/envs/zmachine/jericho.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/generator/
--rw-r--r--   0 vsts      (1001) docker     (123)     8349 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19691 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/chaining.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/generator/data/
--rw-r--r--   0 vsts      (1001) docker     (123)     6309 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/generator/data/logic/
--rw-r--r--   0 vsts      (1001) docker     (123)     1424 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/logic/container.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     2909 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/logic/door.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      682 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/logic/food.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     1805 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/logic/inventory.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/logic/key.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/logic/object.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      236 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/logic/player.twl
--rw-r--r--   0 vsts      (1001) docker     (123)     2902 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/logic/room.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/logic/supporter.twl
--rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/logic/thing.twl
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/generator/data/text_grammars/
--rw-r--r--   0 vsts      (1001) docker     (123)     1421 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/text_grammars/basic_instruction.twg
--rw-r--r--   0 vsts      (1001) docker     (123)     2266 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/text_grammars/basic_obj.twg
--rw-r--r--   0 vsts      (1001) docker     (123)     1704 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/text_grammars/basic_room.twg
--rw-r--r--   0 vsts      (1001) docker     (123)    13249 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/text_grammars/house_instruction.twg
--rw-r--r--   0 vsts      (1001) docker     (123)    16075 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/text_grammars/house_obj.twg
--rw-r--r--   0 vsts      (1001) docker     (123)    34339 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/data/text_grammars/house_room.twg
--rw-r--r--   0 vsts      (1001) docker     (123)     6085 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/dependency_tree.py
--rw-r--r--   0 vsts      (1001) docker     (123)    45392 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/game.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/graph_networks.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/generator/inform7/
--rw-r--r--   0 vsts      (1001) docker     (123)      394 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/inform7/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    48073 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/inform7/world2inform7.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7522 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)    29865 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/maker.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4688 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/testing.py
--rw-r--r--   0 vsts      (1001) docker     (123)    23051 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/text_generation.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19456 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/text_grammar.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7916 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/vtypes.py
--rw-r--r--   0 vsts      (1001) docker     (123)    23755 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/generator/world.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/gym/
--rw-r--r--   0 vsts      (1001) docker     (123)      101 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/gym/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1957 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/gym/core.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/gym/envs/
--rw-r--r--   0 vsts      (1001) docker     (123)      125 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/gym/envs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3245 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/gym/envs/textworld.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8771 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/gym/envs/textworld_batch.py
--rw-r--r--   0 vsts      (1001) docker     (123)      835 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/gym/envs/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/gym/spaces/
--rw-r--r--   0 vsts      (1001) docker     (123)      100 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/gym/spaces/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6214 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/gym/spaces/text_spaces.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7901 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/gym/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3866 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/helpers.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/logic/
--rw-r--r--   0 vsts      (1001) docker     (123)    60283 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/logic/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2671 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/logic/logic.ebnf
--rw-r--r--   0 vsts      (1001) docker     (123)     2464 2023-05-31 14:44:37.000000 textworld-1.5.4rc3/textworld/logic/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18302 2023-05-31 14:44:37.000000 textworld-1.5.4rc3/textworld/logic/parser.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/render/
--rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6386 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/graph.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16522 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/render.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10482 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/serve.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/render/tmpl/
--rw-r--r--   0 vsts      (1001) docker     (123)     1175 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/slideshow.handlebars
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/
--rw-r--r--   0 vsts      (1001) docker     (123)   144877 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/bootstrap.min.css
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/
--rw-r--r--   0 vsts      (1001) docker     (123)     1745 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Chevron.png
--rw-r--r--   0 vsts      (1001) docker     (123)     4156 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Container.png
--rw-r--r--   0 vsts      (1001) docker     (123)    33814 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_ContainerOpen.png
--rw-r--r--   0 vsts      (1001) docker     (123)     3402 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Cooked.png
--rw-r--r--   0 vsts      (1001) docker     (123)     1696 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Door.png
--rw-r--r--   0 vsts      (1001) docker     (123)     3028 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_DoorOpen.png
--rw-r--r--   0 vsts      (1001) docker     (123)     5570 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Fixed.png
--rw-r--r--   0 vsts      (1001) docker     (123)     5748 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Food.png
--rw-r--r--   0 vsts      (1001) docker     (123)     7467 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Key.png
--rw-r--r--   0 vsts      (1001) docker     (123)     4329 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_LightOff.png
--rw-r--r--   0 vsts      (1001) docker     (123)     5679 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_LightOn.png
--rw-r--r--   0 vsts      (1001) docker     (123)     3297 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Locked.png
--rw-r--r--   0 vsts      (1001) docker     (123)     4560 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Object.png
--rw-r--r--   0 vsts      (1001) docker     (123)     5869 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Player.png
--rw-r--r--   0 vsts      (1001) docker     (123)     4792 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Portable.png
--rw-r--r--   0 vsts      (1001) docker     (123)     2527 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Supporter.png
--rw-r--r--   0 vsts      (1001) docker     (123)     4693 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Uncooked.png
--rw-r--r--   0 vsts      (1001) docker     (123)     3273 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Unlocked.png
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/js/
--rw-r--r--   0 vsts      (1001) docker     (123)    48944 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/js/bootstrap.min.js
--rw-r--r--   0 vsts      (1001) docker     (123)   236270 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/js/d3.v5.min.js
--rw-r--r--   0 vsts      (1001) docker     (123)    89493 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/js/jquery-3.5.0.min.js
--rw-r--r--   0 vsts      (1001) docker     (123)    21789 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/js/visualization.js
--rw-r--r--   0 vsts      (1001) docker     (123)     3771 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/render/tmpl/static/style.css
--rw-r--r--   0 vsts      (1001) docker     (123)     2939 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/testing.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1954 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/text_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/textgen/
--rw-r--r--   0 vsts      (1001) docker     (123)     3134 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/textgen/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-05-31 14:44:37.000000 textworld-1.5.4rc3/textworld/textgen/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6169 2023-05-31 14:44:37.000000 textworld-1.5.4rc3/textworld/textgen/parser.py
--rw-r--r--   0 vsts      (1001) docker     (123)      628 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/textgen/textgen.ebnf
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/thirdparty/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (123)     2859 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/Makefile
--rw-r--r--   0 vsts      (1001) docker     (123)      876 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/Makefile.win
--rw-r--r--   0 vsts      (1001) docker     (123)    14938 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/README.txt
--rw-r--r--   0 vsts      (1001) docker     (123)    17006 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/accel.c
--rw-r--r--   0 vsts      (1001) docker     (123)    16278 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/compiler.c
--rw-r--r--   0 vsts      (1001) docker     (123)     3289 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/compiler.h
--rw-r--r--   0 vsts      (1001) docker     (123)     2709 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/config.h
--rw-r--r--   0 vsts      (1001) docker     (123)     1210 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/gestalt.c
--rw-r--r--   0 vsts      (1001) docker     (123)     5332 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/git.c
--rw-r--r--   0 vsts      (1001) docker     (123)     4587 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/git.h
--rw-r--r--   0 vsts      (1001) docker     (123)     2044 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/git_mac.c
--rw-r--r--   0 vsts      (1001) docker     (123)     2215 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/git_unix.c
--rw-r--r--   0 vsts      (1001) docker     (123)     2721 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/git_windows.c
--rw-r--r--   0 vsts      (1001) docker     (123)    39624 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/glkop.c
--rw-r--r--   0 vsts      (1001) docker     (123)     9266 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/heap.c
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/
--rw-r--r--   0 vsts      (1001) docker     (123)      174 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/Git.css
--rw-r--r--   0 vsts      (1001) docker     (123)     2518 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/Git.hhc
--rw-r--r--   0 vsts      (1001) docker     (123)      382 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/Git.hhp
--rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/about.png
--rw-r--r--   0 vsts      (1001) docker     (123)     1499 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/archive.htm
--rw-r--r--   0 vsts      (1001) docker     (123)      872 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/autorun.htm
--rw-r--r--   0 vsts      (1001) docker     (123)     1456 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/blorb.htm
--rw-r--r--   0 vsts      (1001) docker     (123)     2773 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/config.htm
--rw-r--r--   0 vsts      (1001) docker     (123)     3357 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/credits.htm
--rw-r--r--   0 vsts      (1001) docker     (123)     2391 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/editing_keys.htm
--rw-r--r--   0 vsts      (1001) docker     (123)      290 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/fixed.png
--rw-r--r--   0 vsts      (1001) docker     (123)     1791 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/getting_started.htm
--rw-r--r--   0 vsts      (1001) docker     (123)     1630 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/gfx_sound.htm
--rw-r--r--   0 vsts      (1001) docker     (123)      994 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/glk.htm
--rw-r--r--   0 vsts      (1001) docker     (123)      800 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/glulx.htm
--rw-r--r--   0 vsts      (1001) docker     (123)      302 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/help.png
--rw-r--r--   0 vsts      (1001) docker     (123)     1716 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/license_ogg.htm
--rw-r--r--   0 vsts      (1001) docker     (123)     1222 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/menus_toolbar.htm
--rw-r--r--   0 vsts      (1001) docker     (123)     3791 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/options.htm
--rw-r--r--   0 vsts      (1001) docker     (123)      275 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/options.png
--rw-r--r--   0 vsts      (1001) docker     (123)     1950 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/overview.htm
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/prop.png
--rw-r--r--   0 vsts      (1001) docker     (123)     5726 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/revision.htm
--rw-r--r--   0 vsts      (1001) docker     (123)      241 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/scroll.png
--rw-r--r--   0 vsts      (1001) docker     (123)     4296 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/labels.inc
--rw-r--r--   0 vsts      (1001) docker     (123)     4176 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/memory.c
--rw-r--r--   0 vsts      (1001) docker     (123)     5008 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/memory.h
--rw-r--r--   0 vsts      (1001) docker     (123)    17253 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/opcodes.c
--rw-r--r--   0 vsts      (1001) docker     (123)     3945 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/opcodes.h
--rw-r--r--   0 vsts      (1001) docker     (123)    12167 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/operands.c
--rw-r--r--   0 vsts      (1001) docker     (123)     5983 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/peephole.c
--rw-r--r--   0 vsts      (1001) docker     (123)     8408 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/savefile.c
--rw-r--r--   0 vsts      (1001) docker     (123)     9316 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/saveundo.c
--rw-r--r--   0 vsts      (1001) docker     (123)     9082 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/search.c
--rw-r--r--   0 vsts      (1001) docker     (123)    44041 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/terp.c
--rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/test.sh
--rw-r--r--   0 vsts      (1001) docker     (123)       45 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/user_agent.py
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-05-31 14:44:39.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/version.h
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/win/
--rw-r--r--   0 vsts      (1001) docker     (123)      281 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/win/git.rc
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/win/res/
--rw-r--r--   0 vsts      (1001) docker     (123)    25214 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/win/res/Blorb.ico
--rw-r--r--   0 vsts      (1001) docker     (123)      857 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/win/res/Git.manifest
--rw-r--r--   0 vsts      (1001) docker     (123)    25214 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/win/res/Glulx.ico
--rw-r--r--   0 vsts      (1001) docker     (123)    25214 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/win/res/Ulx.ico
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/
--rw-r--r--   0 vsts      (1001) docker     (123)       42 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (123)     1081 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)     1307 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/Makefile
--rw-r--r--   0 vsts      (1001) docker     (123)    11194 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/README.txt
--rw-r--r--   0 vsts      (1001) docker     (123)     5070 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/agent.c
--rw-r--r--   0 vsts      (1001) docker     (123)      786 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/agent.h
--rw-r--r--   0 vsts      (1001) docker     (123)    23329 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/casemap.py
--rw-r--r--   0 vsts      (1001) docker     (123)      574 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgblorb.c
--rw-r--r--   0 vsts      (1001) docker     (123)     9499 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgdate.c
--rw-r--r--   0 vsts      (1001) docker     (123)     8323 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgfref.c
--rw-r--r--   0 vsts      (1001) docker     (123)     3405 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cggestal.c
--rw-r--r--   0 vsts      (1001) docker     (123)    10757 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgmisc.c
--rw-r--r--   0 vsts      (1001) docker     (123)     1953 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgschan.c
--rw-r--r--   0 vsts      (1001) docker     (123)    50195 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgstream.c
--rw-r--r--   0 vsts      (1001) docker     (123)      623 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgstyle.c
--rw-r--r--   0 vsts      (1001) docker     (123)    15997 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgunicod.c
--rw-r--r--   0 vsts      (1001) docker     (123)   304820 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgunigen.c
--rw-r--r--   0 vsts      (1001) docker     (123)    13655 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgwindow.c
--rw-r--r--   0 vsts      (1001) docker     (123)     7686 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cheapglk.h
--rw-r--r--   0 vsts      (1001) docker     (123)    21573 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/gi_blorb.c
--rw-r--r--   0 vsts      (1001) docker     (123)     3718 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/gi_blorb.h
--rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/gi_debug.c
--rw-r--r--   0 vsts      (1001) docker     (123)     8233 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/gi_debug.h
--rw-r--r--   0 vsts      (1001) docker     (123)    60442 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/gi_dispa.c
--rw-r--r--   0 vsts      (1001) docker     (123)     4276 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/gi_dispa.h
--rw-r--r--   0 vsts      (1001) docker     (123)    16272 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/glk.h
--rw-r--r--   0 vsts      (1001) docker     (123)      694 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/glkstart.c
--rw-r--r--   0 vsts      (1001) docker     (123)     1636 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/glkstart.h
--rw-r--r--   0 vsts      (1001) docker     (123)     9047 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/main.c
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/thirdparty/inform7/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/thirdparty/inform7/share/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/thirdparty/inform7/share/inform7/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/thirdparty/inform7/share/inform7/Internal/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld/thirdparty/inform7/share/inform7/Internal/I6T/
--rw-r--r--   0 vsts      (1001) docker     (123)    27940 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/thirdparty/inform7/share/inform7/Internal/I6T/Actions.i6t
--rw-r--r--   0 vsts      (1001) docker     (123)     6138 2023-05-31 14:43:48.000000 textworld-1.5.4rc3/textworld/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-31 14:44:41.000000 textworld-1.5.4rc3/textworld/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     9180 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    14039 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      619 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       14 2023-05-31 14:44:43.000000 textworld-1.5.4rc3/textworld.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/
+-rw-r--r--   0 vsts      (1001) docker     (123)     9811 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/CHANGELOG.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      915 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/CONTRIBUTING.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      944 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     9180 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     7522 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/glk_build.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      373 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/requirements-full.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      160 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/requirements-vis.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      212 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/requirements.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/scripts/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      809 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/scripts/tw-data
+-rw-r--r--   0 vsts      (1001) docker     (123)     7207 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/scripts/tw-extract
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    12269 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/scripts/tw-make
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2698 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/scripts/tw-play
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1741 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/scripts/tw-stats
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      895 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/scripts/tw-view
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2078 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/setup.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2475 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/setup.sh
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/src/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6142 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/src/glk_comm.c
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/
+-rw-r--r--   0 vsts      (1001) docker     (123)      573 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/agents/
+-rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/agents/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2369 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/agents/human.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1506 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/agents/random.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      965 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/agents/simple.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1128 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/agents/walkthrough.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/
+-rw-r--r--   0 vsts      (1001) docker     (123)      398 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1380 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/registration.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6704 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/coin_collector.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/logic/
+-rw-r--r--   0 vsts      (1001) docker     (123)      787 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/logic/inventory.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      278 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/logic/object.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      236 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/logic/player.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     2288 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/logic/room.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/logic/thing.twl
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/
+-rw-r--r--   0 vsts      (1001) docker     (123)    13249 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/house_instruction.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)    16075 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/house_obj.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)    34339 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/house_room.twg
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    49637 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/cooking.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1424 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/container.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/door.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     9734 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/food.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     1627 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/inventory.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/key.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     6333 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/meal.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/object.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     1882 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/oven.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      236 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/player.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      176 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/pot.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     2932 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/room.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      932 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/stove.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/supporter.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     1249 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/thing.twl
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1424 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/container.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/door.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     9786 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/food.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     2212 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/inventory.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/key.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     6688 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/meal.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/object.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     1882 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/oven.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      324 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/player.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      176 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/pot.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     2932 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/room.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      932 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/stove.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/supporter.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     1249 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/thing.twl
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/text_grammars/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1059 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_ext_cook.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)    13548 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_instruction.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)    16270 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_obj.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)    34301 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_room.twg
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12409 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/simple.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1424 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/container.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     2909 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/door.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      682 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/food.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     1805 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/inventory.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/key.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/object.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      236 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/player.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     2902 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/room.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/supporter.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/thing.twl
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/text_grammars/
+-rw-r--r--   0 vsts      (1001) docker     (123)    13249 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/text_grammars/house_instruction.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)    16075 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/text_grammars/house_obj.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)    34339 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/text_grammars/house_room.twg
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1424 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/container.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     2909 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/door.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      682 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/food.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     1805 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/inventory.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/key.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/object.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      236 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/player.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     2902 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/room.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/supporter.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/thing.twl
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/
+-rw-r--r--   0 vsts      (1001) docker     (123)    13249 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/house_instruction.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)    16075 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/house_obj.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)    34339 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/house_room.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)     9383 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/treasure_hunter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1636 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/challenges/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15836 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/core.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/envs/
+-rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/envs/batch/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1647 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/batch/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8463 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/batch/batch_env.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/envs/glulx/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/glulx/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4952 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/glulx/git_glulx.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6850 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/tw.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/envs/wrappers/
+-rw-r--r--   0 vsts      (1001) docker     (123)      422 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/wrappers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2125 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/wrappers/filter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      447 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/wrappers/generic.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      843 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/wrappers/limit.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      813 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/wrappers/recorder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14864 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/wrappers/tw_inform7.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2945 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/wrappers/viewer.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/envs/zmachine/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/zmachine/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4768 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/envs/zmachine/jericho.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/generator/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8349 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19691 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/chaining.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/generator/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6309 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/generator/data/logic/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1424 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/logic/container.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     2909 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/logic/door.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      682 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/logic/food.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     1805 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/logic/inventory.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/logic/key.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/logic/object.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      236 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/logic/player.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)     2902 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/logic/room.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/logic/supporter.twl
+-rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/logic/thing.twl
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/generator/data/text_grammars/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1421 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/text_grammars/basic_instruction.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2266 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/text_grammars/basic_obj.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1704 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/text_grammars/basic_room.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)    13249 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/text_grammars/house_instruction.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)    16075 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/text_grammars/house_obj.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)    34339 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/data/text_grammars/house_room.twg
+-rw-r--r--   0 vsts      (1001) docker     (123)     6085 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/dependency_tree.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    45392 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/game.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/graph_networks.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/generator/inform7/
+-rw-r--r--   0 vsts      (1001) docker     (123)      394 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/inform7/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    48073 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/inform7/world2inform7.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7522 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    29865 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/maker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4688 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/testing.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    23051 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/text_generation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19456 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/text_grammar.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7916 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/vtypes.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    23755 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/generator/world.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/gym/
+-rw-r--r--   0 vsts      (1001) docker     (123)      101 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/gym/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1957 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/gym/core.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/gym/envs/
+-rw-r--r--   0 vsts      (1001) docker     (123)      125 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/gym/envs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3245 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/gym/envs/textworld.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8771 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/gym/envs/textworld_batch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      835 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/gym/envs/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/gym/spaces/
+-rw-r--r--   0 vsts      (1001) docker     (123)      100 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/gym/spaces/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6214 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/gym/spaces/text_spaces.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7901 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/gym/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3866 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/helpers.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/logic/
+-rw-r--r--   0 vsts      (1001) docker     (123)    60283 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/logic/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2671 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/logic/logic.ebnf
+-rw-r--r--   0 vsts      (1001) docker     (123)     2464 2023-05-31 15:29:10.000000 textworld-1.5.4rc4/textworld/logic/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18302 2023-05-31 15:29:10.000000 textworld-1.5.4rc4/textworld/logic/parser.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/render/
+-rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6386 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16522 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/render.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10482 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/serve.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/render/tmpl/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1175 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/slideshow.handlebars
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/
+-rw-r--r--   0 vsts      (1001) docker     (123)   144877 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/bootstrap.min.css
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1745 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Chevron.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     4156 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Container.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    33814 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_ContainerOpen.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     3402 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Cooked.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     1696 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Door.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     3028 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_DoorOpen.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     5570 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Fixed.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     5748 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Food.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     7467 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Key.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     4329 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_LightOff.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     5679 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_LightOn.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     3297 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Locked.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     4560 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Object.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     5869 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Player.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     4792 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Portable.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     2527 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Supporter.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     4693 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Uncooked.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     3273 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Unlocked.png
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/js/
+-rw-r--r--   0 vsts      (1001) docker     (123)    48944 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/js/bootstrap.min.js
+-rw-r--r--   0 vsts      (1001) docker     (123)   236270 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/js/d3.v5.min.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    89493 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/js/jquery-3.5.0.min.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    21789 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/js/visualization.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     3771 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/render/tmpl/static/style.css
+-rw-r--r--   0 vsts      (1001) docker     (123)     2939 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/testing.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1954 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/text_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/textgen/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3134 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/textgen/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-05-31 15:29:10.000000 textworld-1.5.4rc4/textworld/textgen/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6169 2023-05-31 15:29:10.000000 textworld-1.5.4rc4/textworld/textgen/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      628 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/textgen/textgen.ebnf
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/thirdparty/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (123)     2859 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/Makefile
+-rw-r--r--   0 vsts      (1001) docker     (123)      876 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/Makefile.win
+-rw-r--r--   0 vsts      (1001) docker     (123)    14938 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/README.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)    17006 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/accel.c
+-rw-r--r--   0 vsts      (1001) docker     (123)    16278 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/compiler.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     3289 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/compiler.h
+-rw-r--r--   0 vsts      (1001) docker     (123)     2709 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/config.h
+-rw-r--r--   0 vsts      (1001) docker     (123)     1210 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/gestalt.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     5332 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/git.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     4587 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/git.h
+-rw-r--r--   0 vsts      (1001) docker     (123)     2044 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/git_mac.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     2215 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/git_unix.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     2721 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/git_windows.c
+-rw-r--r--   0 vsts      (1001) docker     (123)    39624 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/glkop.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     9266 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/heap.c
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/
+-rw-r--r--   0 vsts      (1001) docker     (123)      174 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/Git.css
+-rw-r--r--   0 vsts      (1001) docker     (123)     2518 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/Git.hhc
+-rw-r--r--   0 vsts      (1001) docker     (123)      382 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/Git.hhp
+-rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/about.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     1499 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/archive.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)      872 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/autorun.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)     1456 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/blorb.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)     2773 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/config.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)     3357 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/credits.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)     2391 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/editing_keys.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)      290 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/fixed.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     1791 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/getting_started.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)     1630 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/gfx_sound.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)      994 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/glk.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)      800 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/glulx.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)      302 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/help.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     1716 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/license_ogg.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)     1222 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/menus_toolbar.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)     3791 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/options.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)      275 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/options.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     1950 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/overview.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/prop.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     5726 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/revision.htm
+-rw-r--r--   0 vsts      (1001) docker     (123)      241 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/scroll.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     4296 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/labels.inc
+-rw-r--r--   0 vsts      (1001) docker     (123)     4176 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/memory.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     5008 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/memory.h
+-rw-r--r--   0 vsts      (1001) docker     (123)    17253 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/opcodes.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     3945 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/opcodes.h
+-rw-r--r--   0 vsts      (1001) docker     (123)    12167 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/operands.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     5983 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/peephole.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     8408 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/savefile.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     9316 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/saveundo.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     9082 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/search.c
+-rw-r--r--   0 vsts      (1001) docker     (123)    44041 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/terp.c
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/test.sh
+-rw-r--r--   0 vsts      (1001) docker     (123)       45 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/user_agent.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-05-31 15:29:13.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/version.h
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/win/
+-rw-r--r--   0 vsts      (1001) docker     (123)      281 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/win/git.rc
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/win/res/
+-rw-r--r--   0 vsts      (1001) docker     (123)    25214 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/win/res/Blorb.ico
+-rw-r--r--   0 vsts      (1001) docker     (123)      857 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/win/res/Git.manifest
+-rw-r--r--   0 vsts      (1001) docker     (123)    25214 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/win/res/Glulx.ico
+-rw-r--r--   0 vsts      (1001) docker     (123)    25214 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/win/res/Ulx.ico
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/
+-rw-r--r--   0 vsts      (1001) docker     (123)       42 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (123)     1081 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)     1307 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/Makefile
+-rw-r--r--   0 vsts      (1001) docker     (123)    11194 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/README.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     5070 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/agent.c
+-rw-r--r--   0 vsts      (1001) docker     (123)      786 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/agent.h
+-rw-r--r--   0 vsts      (1001) docker     (123)    23329 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/casemap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      574 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgblorb.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     9499 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgdate.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     8323 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgfref.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     3405 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cggestal.c
+-rw-r--r--   0 vsts      (1001) docker     (123)    10757 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgmisc.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     1953 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgschan.c
+-rw-r--r--   0 vsts      (1001) docker     (123)    50195 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgstream.c
+-rw-r--r--   0 vsts      (1001) docker     (123)      623 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgstyle.c
+-rw-r--r--   0 vsts      (1001) docker     (123)    15997 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgunicod.c
+-rw-r--r--   0 vsts      (1001) docker     (123)   304820 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgunigen.c
+-rw-r--r--   0 vsts      (1001) docker     (123)    13655 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgwindow.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     7686 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cheapglk.h
+-rw-r--r--   0 vsts      (1001) docker     (123)    21573 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/gi_blorb.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     3718 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/gi_blorb.h
+-rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/gi_debug.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     8233 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/gi_debug.h
+-rw-r--r--   0 vsts      (1001) docker     (123)    60442 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/gi_dispa.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     4276 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/gi_dispa.h
+-rw-r--r--   0 vsts      (1001) docker     (123)    16272 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/glk.h
+-rw-r--r--   0 vsts      (1001) docker     (123)      694 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/glkstart.c
+-rw-r--r--   0 vsts      (1001) docker     (123)     1636 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/glkstart.h
+-rw-r--r--   0 vsts      (1001) docker     (123)     9047 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/main.c
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/thirdparty/inform7/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/thirdparty/inform7/share/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/thirdparty/inform7/share/inform7/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/thirdparty/inform7/share/inform7/Internal/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld/thirdparty/inform7/share/inform7/Internal/I6T/
+-rw-r--r--   0 vsts      (1001) docker     (123)    27940 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/thirdparty/inform7/share/inform7/Internal/I6T/Actions.i6t
+-rw-r--r--   0 vsts      (1001) docker     (123)     6138 2023-05-31 15:28:19.000000 textworld-1.5.4rc4/textworld/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-31 15:29:15.000000 textworld-1.5.4rc4/textworld/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     9180 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)    14039 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      595 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       14 2023-05-31 15:29:16.000000 textworld-1.5.4rc4/textworld.egg-info/top_level.txt
```

### Comparing `textworld-1.5.4rc3/CHANGELOG.md` & `textworld-1.5.4rc4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/CONTRIBUTING.md` & `textworld-1.5.4rc4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/LICENSE.txt` & `textworld-1.5.4rc4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/MANIFEST.in` & `textworld-1.5.4rc4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/PKG-INFO` & `textworld-1.5.4rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textworld
-Version: 1.5.4rc3
+Version: 1.5.4rc4
 Summary: Microsoft Textworld - A Text-based Learning Environment.
 Home-page: https://github.com/microsoft/TextWorld
 Author: Microsoft Textworld
 License: UNKNOWN
 Description: # TextWorld
         
         [![Build Status](https://dev.azure.com/maluuba/TextWorld/_apis/build/status/microsoft.TextWorld?branchName=main)](https://dev.azure.com/maluuba/TextWorld/_build/latest?definitionId=180&branchName=main) [![PyPI version](https://badge.fury.io/py/textworld.svg)](https://badge.fury.io/py/textworld) [![Documentation Status](https://readthedocs.org/projects/textworld/badge/?version=latest)](https://textworld.readthedocs.io/en/stable/?badge=stable) [![Join the chat at https://gitter.im/Microsoft/TextWorld](https://badges.gitter.im/Microsoft/TextWorld.svg)](https://gitter.im/Microsoft/TextWorld?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
```

### Comparing `textworld-1.5.4rc3/README.md` & `textworld-1.5.4rc4/README.md`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/glk_build.py` & `textworld-1.5.4rc4/glk_build.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/scripts/tw-data` & `textworld-1.5.4rc4/scripts/tw-data`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/scripts/tw-extract` & `textworld-1.5.4rc4/scripts/tw-extract`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/scripts/tw-make` & `textworld-1.5.4rc4/scripts/tw-make`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/scripts/tw-play` & `textworld-1.5.4rc4/scripts/tw-play`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/scripts/tw-stats` & `textworld-1.5.4rc4/scripts/tw-stats`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/scripts/tw-view` & `textworld-1.5.4rc4/scripts/tw-view`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/setup.py` & `textworld-1.5.4rc4/setup.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/setup.sh` & `textworld-1.5.4rc4/setup.sh`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/src/glk_comm.c` & `textworld-1.5.4rc4/src/glk_comm.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/__init__.py` & `textworld-1.5.4rc4/textworld/__init__.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/agents/human.py` & `textworld-1.5.4rc4/textworld/agents/human.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/agents/random.py` & `textworld-1.5.4rc4/textworld/agents/random.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/agents/simple.py` & `textworld-1.5.4rc4/textworld/agents/simple.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/agents/walkthrough.py` & `textworld-1.5.4rc4/textworld/agents/walkthrough.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/registration.py` & `textworld-1.5.4rc4/textworld/challenges/registration.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/coin_collector.py` & `textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/coin_collector.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/logic/inventory.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/logic/inventory.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/logic/room.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/logic/room.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/house_instruction.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/house_instruction.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/house_obj.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/house_obj.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/house_room.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_coin_collector/textworld_data/text_grammars/house_room.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/cooking.py` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/cooking.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/container.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/container.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/door.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/door.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/food.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/food.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/inventory.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/inventory.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/key.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/key.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/meal.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/meal.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/object.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/object.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/oven.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/oven.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/room.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/room.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/stove.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/stove.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic/thing.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic/thing.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/container.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/container.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/door.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/door.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/food.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/food.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/inventory.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/inventory.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/key.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/key.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/meal.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/meal.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/object.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/object.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/oven.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/oven.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/room.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/room.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/stove.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/stove.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/logic_drop/thing.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/logic_drop/thing.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_ext_cook.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_ext_cook.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_instruction.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_instruction.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_obj.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_obj.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_room.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_cooking/textworld_data/text_grammars/house_room.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_simple/simple.py` & `textworld-1.5.4rc4/textworld/challenges/tw_simple/simple.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/container.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/container.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/door.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/door.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/food.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/food.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/inventory.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/inventory.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/key.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/key.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/object.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/object.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/logic/room.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/logic/room.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/text_grammars/house_instruction.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/text_grammars/house_instruction.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/text_grammars/house_obj.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/text_grammars/house_obj.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_simple/textworld_data/text_grammars/house_room.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_simple/textworld_data/text_grammars/house_room.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/container.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/container.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/door.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/door.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/food.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/food.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/inventory.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/inventory.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/key.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/key.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/object.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/object.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/logic/room.twl` & `textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/logic/room.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/house_instruction.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/house_instruction.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/house_obj.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/house_obj.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/house_room.twg` & `textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/textworld_data/text_grammars/house_room.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/tw_treasure_hunter/treasure_hunter.py` & `textworld-1.5.4rc4/textworld/challenges/tw_treasure_hunter/treasure_hunter.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/challenges/utils.py` & `textworld-1.5.4rc4/textworld/challenges/utils.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/core.py` & `textworld-1.5.4rc4/textworld/core.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/envs/batch/__init__.py` & `textworld-1.5.4rc4/textworld/envs/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/envs/batch/batch_env.py` & `textworld-1.5.4rc4/textworld/envs/batch/batch_env.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/envs/glulx/git_glulx.py` & `textworld-1.5.4rc4/textworld/envs/glulx/git_glulx.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/envs/tw.py` & `textworld-1.5.4rc4/textworld/envs/tw.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/envs/wrappers/filter.py` & `textworld-1.5.4rc4/textworld/envs/wrappers/filter.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/envs/wrappers/limit.py` & `textworld-1.5.4rc4/textworld/envs/wrappers/limit.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/envs/wrappers/recorder.py` & `textworld-1.5.4rc4/textworld/envs/wrappers/recorder.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/envs/wrappers/tw_inform7.py` & `textworld-1.5.4rc4/textworld/envs/wrappers/tw_inform7.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/envs/wrappers/viewer.py` & `textworld-1.5.4rc4/textworld/envs/wrappers/viewer.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/envs/zmachine/jericho.py` & `textworld-1.5.4rc4/textworld/envs/zmachine/jericho.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/__init__.py` & `textworld-1.5.4rc4/textworld/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/chaining.py` & `textworld-1.5.4rc4/textworld/generator/chaining.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/__init__.py` & `textworld-1.5.4rc4/textworld/generator/data/__init__.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/logic/container.twl` & `textworld-1.5.4rc4/textworld/generator/data/logic/container.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/logic/door.twl` & `textworld-1.5.4rc4/textworld/generator/data/logic/door.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/logic/food.twl` & `textworld-1.5.4rc4/textworld/generator/data/logic/food.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/logic/inventory.twl` & `textworld-1.5.4rc4/textworld/generator/data/logic/inventory.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/logic/key.twl` & `textworld-1.5.4rc4/textworld/generator/data/logic/key.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/logic/object.twl` & `textworld-1.5.4rc4/textworld/generator/data/logic/object.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/logic/room.twl` & `textworld-1.5.4rc4/textworld/generator/data/logic/room.twl`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/text_grammars/basic_instruction.twg` & `textworld-1.5.4rc4/textworld/generator/data/text_grammars/basic_instruction.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/text_grammars/basic_obj.twg` & `textworld-1.5.4rc4/textworld/generator/data/text_grammars/basic_obj.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/text_grammars/basic_room.twg` & `textworld-1.5.4rc4/textworld/generator/data/text_grammars/basic_room.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/text_grammars/house_instruction.twg` & `textworld-1.5.4rc4/textworld/generator/data/text_grammars/house_instruction.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/text_grammars/house_obj.twg` & `textworld-1.5.4rc4/textworld/generator/data/text_grammars/house_obj.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/data/text_grammars/house_room.twg` & `textworld-1.5.4rc4/textworld/generator/data/text_grammars/house_room.twg`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/dependency_tree.py` & `textworld-1.5.4rc4/textworld/generator/dependency_tree.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/game.py` & `textworld-1.5.4rc4/textworld/generator/game.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/graph_networks.py` & `textworld-1.5.4rc4/textworld/generator/graph_networks.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/inform7/world2inform7.py` & `textworld-1.5.4rc4/textworld/generator/inform7/world2inform7.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/logger.py` & `textworld-1.5.4rc4/textworld/generator/logger.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/maker.py` & `textworld-1.5.4rc4/textworld/generator/maker.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/testing.py` & `textworld-1.5.4rc4/textworld/generator/testing.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/text_generation.py` & `textworld-1.5.4rc4/textworld/generator/text_generation.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/text_grammar.py` & `textworld-1.5.4rc4/textworld/generator/text_grammar.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/vtypes.py` & `textworld-1.5.4rc4/textworld/generator/vtypes.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/generator/world.py` & `textworld-1.5.4rc4/textworld/generator/world.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/gym/core.py` & `textworld-1.5.4rc4/textworld/gym/core.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/gym/envs/textworld.py` & `textworld-1.5.4rc4/textworld/gym/envs/textworld.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/gym/envs/textworld_batch.py` & `textworld-1.5.4rc4/textworld/gym/envs/textworld_batch.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/gym/envs/utils.py` & `textworld-1.5.4rc4/textworld/gym/envs/utils.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/gym/spaces/text_spaces.py` & `textworld-1.5.4rc4/textworld/gym/spaces/text_spaces.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/gym/utils.py` & `textworld-1.5.4rc4/textworld/gym/utils.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/helpers.py` & `textworld-1.5.4rc4/textworld/helpers.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/logic/__init__.py` & `textworld-1.5.4rc4/textworld/logic/__init__.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/logic/logic.ebnf` & `textworld-1.5.4rc4/textworld/logic/logic.ebnf`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/logic/model.py` & `textworld-1.5.4rc4/textworld/logic/model.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/logic/parser.py` & `textworld-1.5.4rc4/textworld/logic/parser.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/graph.py` & `textworld-1.5.4rc4/textworld/render/graph.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/render.py` & `textworld-1.5.4rc4/textworld/render/render.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/serve.py` & `textworld-1.5.4rc4/textworld/render/serve.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/slideshow.handlebars` & `textworld-1.5.4rc4/textworld/render/tmpl/slideshow.handlebars`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/bootstrap.min.css` & `textworld-1.5.4rc4/textworld/render/tmpl/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Chevron.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Chevron.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Container.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Container.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_ContainerOpen.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_ContainerOpen.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Cooked.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Cooked.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Door.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Door.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_DoorOpen.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_DoorOpen.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Fixed.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Fixed.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Food.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Food.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Key.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Key.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_LightOff.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_LightOff.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_LightOn.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_LightOn.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Locked.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Locked.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Object.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Object.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Player.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Player.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Portable.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Portable.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Supporter.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Supporter.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Uncooked.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Uncooked.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/images/TextWorldIcons_Unlocked.png` & `textworld-1.5.4rc4/textworld/render/tmpl/static/images/TextWorldIcons_Unlocked.png`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/js/bootstrap.min.js` & `textworld-1.5.4rc4/textworld/render/tmpl/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/js/d3.v5.min.js` & `textworld-1.5.4rc4/textworld/render/tmpl/static/js/d3.v5.min.js`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/js/jquery-3.5.0.min.js` & `textworld-1.5.4rc4/textworld/render/tmpl/static/js/jquery-3.5.0.min.js`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/js/visualization.js` & `textworld-1.5.4rc4/textworld/render/tmpl/static/js/visualization.js`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/render/tmpl/static/style.css` & `textworld-1.5.4rc4/textworld/render/tmpl/static/style.css`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/testing.py` & `textworld-1.5.4rc4/textworld/testing.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/text_utils.py` & `textworld-1.5.4rc4/textworld/text_utils.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/textgen/__init__.py` & `textworld-1.5.4rc4/textworld/textgen/__init__.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/textgen/model.py` & `textworld-1.5.4rc4/textworld/textgen/model.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/textgen/parser.py` & `textworld-1.5.4rc4/textworld/textgen/parser.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/textgen/textgen.ebnf` & `textworld-1.5.4rc4/textworld/textgen/textgen.ebnf`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/Makefile` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/Makefile`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/Makefile.win` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/Makefile.win`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/README.txt` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/README.txt`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/accel.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/accel.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/compiler.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/compiler.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/compiler.h` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/compiler.h`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/config.h` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/config.h`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/gestalt.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/gestalt.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/git.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/git.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/git.h` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/git.h`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/git_mac.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/git_mac.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/git_unix.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/git_unix.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/git_windows.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/git_windows.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/glkop.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/glkop.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/heap.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/heap.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/Git.hhc` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/Git.hhc`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/archive.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/archive.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/autorun.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/autorun.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/blorb.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/blorb.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/config.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/config.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/credits.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/credits.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/editing_keys.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/editing_keys.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/getting_started.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/getting_started.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/gfx_sound.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/gfx_sound.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/glk.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/glk.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/glulx.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/glulx.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/license_ogg.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/license_ogg.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/menus_toolbar.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/menus_toolbar.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/options.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/options.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/overview.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/overview.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/help/revision.htm` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/help/revision.htm`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/labels.inc` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/labels.inc`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/memory.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/memory.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/memory.h` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/memory.h`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/opcodes.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/opcodes.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/opcodes.h` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/opcodes.h`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/operands.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/operands.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/peephole.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/peephole.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/savefile.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/savefile.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/saveundo.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/saveundo.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/search.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/search.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/terp.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/terp.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/win/res/Blorb.ico` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/win/res/Blorb.ico`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/win/res/Git.manifest` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/win/res/Git.manifest`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/win/res/Glulx.ico` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/win/res/Glulx.ico`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/Git-Glulx/win/res/Ulx.ico` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/Git-Glulx/win/res/Ulx.ico`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/LICENSE` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/LICENSE`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/Makefile` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/Makefile`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/README.txt` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/README.txt`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/agent.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/agent.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/agent.h` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/agent.h`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/casemap.py` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/casemap.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgblorb.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgblorb.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgdate.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgdate.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgfref.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgfref.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cggestal.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cggestal.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgmisc.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgmisc.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgschan.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgschan.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgstream.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgstream.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgstyle.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgstyle.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgunicod.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgunicod.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgunigen.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgunigen.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cgwindow.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cgwindow.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/cheapglk.h` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/cheapglk.h`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/gi_blorb.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/gi_blorb.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/gi_blorb.h` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/gi_blorb.h`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/gi_debug.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/gi_debug.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/gi_debug.h` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/gi_debug.h`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/gi_dispa.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/gi_dispa.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/gi_dispa.h` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/gi_dispa.h`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/glk.h` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/glk.h`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/glkstart.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/glkstart.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/glkstart.h` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/glkstart.h`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/glulx/cheapglk/main.c` & `textworld-1.5.4rc4/textworld/thirdparty/glulx/cheapglk/main.c`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/thirdparty/inform7/share/inform7/Internal/I6T/Actions.i6t` & `textworld-1.5.4rc4/textworld/thirdparty/inform7/share/inform7/Internal/I6T/Actions.i6t`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld/utils.py` & `textworld-1.5.4rc4/textworld/utils.py`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld.egg-info/PKG-INFO` & `textworld-1.5.4rc4/textworld.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textworld
-Version: 1.5.4rc3
+Version: 1.5.4rc4
 Summary: Microsoft Textworld - A Text-based Learning Environment.
 Home-page: https://github.com/microsoft/TextWorld
 Author: Microsoft Textworld
 License: UNKNOWN
 Description: # TextWorld
         
         [![Build Status](https://dev.azure.com/maluuba/TextWorld/_apis/build/status/microsoft.TextWorld?branchName=main)](https://dev.azure.com/maluuba/TextWorld/_build/latest?definitionId=180&branchName=main) [![PyPI version](https://badge.fury.io/py/textworld.svg)](https://badge.fury.io/py/textworld) [![Documentation Status](https://readthedocs.org/projects/textworld/badge/?version=latest)](https://textworld.readthedocs.io/en/stable/?badge=stable) [![Join the chat at https://gitter.im/Microsoft/TextWorld](https://badges.gitter.im/Microsoft/TextWorld.svg)](https://gitter.im/Microsoft/TextWorld?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
```

### Comparing `textworld-1.5.4rc3/textworld.egg-info/SOURCES.txt` & `textworld-1.5.4rc4/textworld.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `textworld-1.5.4rc3/textworld.egg-info/requires.txt` & `textworld-1.5.4rc4/textworld.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 numpy>=1.14.5
 tqdm>=4.17.1
-cffi>=1.0.0
 networkx>=2
 more_itertools
 tatsu<5,>=4.3.0
 hashids>=1.2.0
 jericho>=3.0.3
 mementos>=1.3.1
 prompt_toolkit
 gym<0.26,>=0.10.11
 
 [full]
 numpy>=1.14.5
 tqdm>=4.17.1
-cffi>=1.0.0
 networkx>=2
 more_itertools
 tatsu<5,>=4.3.0
 hashids>=1.2.0
 jericho>=2.2.0
 mementos>=1.3.1
 prompt_toolkit
```

