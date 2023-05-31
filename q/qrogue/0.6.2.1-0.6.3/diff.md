# Comparing `tmp/qrogue-0.6.2.1.tar.gz` & `tmp/qrogue-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qrogue-0.6.2.1.tar", last modified: Tue Mar 28 10:39:01 2023, max compression
+gzip compressed data, was "qrogue-0.6.3.tar", last modified: Wed May 31 12:45:44 2023, max compression
```

## Comparing `qrogue-0.6.2.1.tar` & `qrogue-0.6.3.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.801449 qrogue-0.6.2.1/
--rw-rw-rw-   0        0        0       38 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5311 2023-03-28 10:39:01.801449 qrogue-0.6.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3675 2023-03-28 10:35:45.000000 qrogue-0.6.2.1/Readme.md
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:00.669013 qrogue-0.6.2.1/qrogue/
--rw-rw-rw-   0        0        0      289 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:00.715843 qrogue-0.6.2.1/qrogue/data/
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:00.898487 qrogue-0.6.2.1/qrogue/data/dungeons/
--rw-rw-rw-   0        0        0     4477 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/data/dungeons/l0exam.qrdg
--rw-rw-rw-   0        0        0     6419 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/data/dungeons/l0training.qrdg
--rw-rw-rw-   0        0        0     4159 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/data/dungeons/l0v0.qrdg
--rw-rw-rw-   0        0        0     3609 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/data/dungeons/l0v1.qrdg
--rw-rw-rw-   0        0        0     3677 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/data/dungeons/l0v2.qrdg
--rw-rw-rw-   0        0        0     4950 2023-03-20 11:36:39.000000 qrogue-0.6.2.1/qrogue/data/dungeons/l0v3.qrdg
--rw-rw-rw-   0        0        0     6458 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/data/dungeons/l0v4.qrdg
--rw-rw-rw-   0        0        0    10077 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/data/dungeons/l0v5.qrdg
--rw-rw-rw-   0        0        0     1885 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/data/dungeons/w0.qrw
--rw-rw-rw-   0        0        0     1275 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/data/dungeons/w1.qrw
--rw-rw-rw-   0        0        0      786 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/data/dungeons/worlds.qrw
--rw-rw-rw-   0        0        0      160 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/data/fresh.qrsave
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:00.914109 qrogue-0.6.2.1/qrogue/data/hallways/
--rw-rw-rw-   0        0        0        0 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/data/hallways/templates.txt
--rw-rw-rw-   0        0        0        6 2022-07-06 10:26:02.000000 qrogue-0.6.2.1/qrogue/data/qrogue_launch.config
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:00.929728 qrogue-0.6.2.1/qrogue/game/
--rw-rw-rw-   0        0        0      212 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:00.945350 qrogue-0.6.2.1/qrogue/game/logic/
--rw-rw-rw-   0        0        0      208 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:00.960974 qrogue-0.6.2.1/qrogue/game/logic/actors/
--rw-rw-rw-   0        0        0      267 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.007837 qrogue-0.6.2.1/qrogue/game/logic/actors/controllables/
--rw-rw-rw-   0        0        0      191 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/controllables/__init__.py
--rw-rw-rw-   0        0        0     2848 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/controllables/controllable.py
--rw-rw-rw-   0        0        0     1511 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/controllables/player.py
--rw-rw-rw-   0        0        0     2002 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/controllables/qubit.py
--rw-rw-rw-   0        0        0    29165 2023-03-28 10:31:00.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/controllables/robot.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.054699 qrogue-0.6.2.1/qrogue/game/logic/actors/puzzles/
--rw-rw-rw-   0        0        0      210 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/puzzles/__init__.py
--rw-rw-rw-   0        0        0     1343 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/puzzles/boss.py
--rw-rw-rw-   0        0        0     1273 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/puzzles/challenge.py
--rw-rw-rw-   0        0        0     1529 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/puzzles/enemy.py
--rw-rw-rw-   0        0        0     2091 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/puzzles/riddle.py
--rw-rw-rw-   0        0        0     2413 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/puzzles/target.py
--rw-rw-rw-   0        0        0    12329 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/actors/state_vector.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.101563 qrogue-0.6.2.1/qrogue/game/logic/collectibles/
--rw-rw-rw-   0        0        0      534 2023-03-28 10:31:00.000000 qrogue-0.6.2.1/qrogue/game/logic/collectibles/__init__.py
--rw-rw-rw-   0        0        0     2572 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/collectibles/collectible.py
--rw-rw-rw-   0        0        0     7438 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/collectibles/collectible_factory.py
--rw-rw-rw-   0        0        0     2029 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/collectibles/consumable.py
--rw-rw-rw-   0        0        0     8459 2023-03-28 10:31:00.000000 qrogue-0.6.2.1/qrogue/game/logic/collectibles/instruction.py
--rw-rw-rw-   0        0        0     2149 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/collectibles/pickup.py
--rw-rw-rw-   0        0        0      954 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/collectibles/qubit.py
--rw-rw-rw-   0        0        0     3350 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/logic/message.py
--rw-rw-rw-   0        0        0     9533 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/target_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.101563 qrogue-0.6.2.1/qrogue/game/world/
--rw-rw-rw-   0        0        0      286 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.179670 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/
--rw-rw-rw-   0        0        0    49157 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/QrogueLevelGenerator.py
--rw-rw-rw-   0        0        0    16607 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/QrogueWorldGenerator.py
--rw-rw-rw-   0        0        0      382 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.242154 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/dungeon_parser/
--rw-rw-rw-   0        0        0    37933 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonLexer.py
--rw-rw-rw-   0        0        0    11800 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonListener.py
--rw-rw-rw-   0        0        0   157830 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonParser.py
--rw-rw-rw-   0        0        0     7341 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonVisitor.py
--rw-rw-rw-   0        0        0      744 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/generator.py
--rw-rw-rw-   0        0        0     7173 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/parser_util.py
--rw-rw-rw-   0        0        0    45168 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/random_generator.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.289019 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/wave_function_collapse/
--rw-rw-rw-   0        0        0      197 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/wave_function_collapse/__init__.py
--rw-rw-rw-   0        0        0     2593 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/wave_function_collapse/learnables.py
--rw-rw-rw-   0        0        0     2936 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/wave_function_collapse/wave_function.py
--rw-rw-rw-   0        0        0    10188 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/wave_function_collapse/wfc_generator.py
--rw-rw-rw-   0        0        0     3192 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/wave_function_collapse/wfc_learner.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.351504 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/world_parser/
--rw-rw-rw-   0        0        0    21993 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldLexer.py
--rw-rw-rw-   0        0        0     4780 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldListener.py
--rw-rw-rw-   0        0        0    65975 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldParser.py
--rw-rw-rw-   0        0        0     3072 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldVisitor.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.426514 qrogue-0.6.2.1/qrogue/game/world/map/
--rw-rw-rw-   0        0        0      469 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/map/__init__.py
--rw-rw-rw-   0        0        0     2481 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/map/callbacks.py
--rw-rw-rw-   0        0        0      955 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/map/expedition_map.py
--rw-rw-rw-   0        0        0      748 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/map/level_map.py
--rw-rw-rw-   0        0        0    11948 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/map/map.py
--rw-rw-rw-   0        0        0    37005 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/map/rooms.py
--rw-rw-rw-   0        0        0    13912 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/map/spaceship_map.py
--rw-rw-rw-   0        0        0     1206 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/map/world_map.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.442135 qrogue-0.6.2.1/qrogue/game/world/navigation/
--rw-rw-rw-   0        0        0       84 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/navigation/__init__.py
--rw-rw-rw-   0        0        0     4868 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/navigation/navigation.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.473377 qrogue-0.6.2.1/qrogue/game/world/tiles/
--rw-rw-rw-   0        0        0      579 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/tiles/__init__.py
--rw-rw-rw-   0        0        0     9250 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/tiles/door_tiles.py
--rw-rw-rw-   0        0        0     6183 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/game/world/tiles/puzzle_tiles.py
--rw-rw-rw-   0        0        0     8526 2023-03-28 10:31:00.000000 qrogue-0.6.2.1/qrogue/game/world/tiles/tiles.py
--rw-rw-rw-   0        0        0    13276 2023-03-28 10:31:00.000000 qrogue-0.6.2.1/qrogue/game/world/tiles/walk_trigger_tiles.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.489011 qrogue-0.6.2.1/qrogue/graphics/
--rw-rw-rw-   0        0        0      371 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/graphics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.504620 qrogue-0.6.2.1/qrogue/graphics/popups/
--rw-rw-rw-   0        0        0      146 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/graphics/popups/__init__.py
--rw-rw-rw-   0        0        0    11063 2023-03-28 10:31:00.000000 qrogue-0.6.2.1/qrogue/graphics/popups/multiline_popup.py
--rw-rw-rw-   0        0        0     9120 2023-03-20 11:39:13.000000 qrogue-0.6.2.1/qrogue/graphics/popups/my_popups.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.535865 qrogue-0.6.2.1/qrogue/graphics/rendering/
--rw-rw-rw-   0        0        0      237 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/graphics/rendering/__init__.py
--rw-rw-rw-   0        0        0     5227 2023-03-28 10:31:00.000000 qrogue-0.6.2.1/qrogue/graphics/rendering/color_rules.py
--rw-rw-rw-   0        0        0     6927 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/graphics/rendering/renderer.py
--rw-rw-rw-   0        0        0     1886 2023-03-28 10:31:00.000000 qrogue-0.6.2.1/qrogue/graphics/widget_base.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.567105 qrogue-0.6.2.1/qrogue/graphics/widgets/
--rw-rw-rw-   0        0        0      695 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/graphics/widgets/__init__.py
--rw-rw-rw-   0        0        0    38814 2023-03-28 10:35:46.000000 qrogue-0.6.2.1/qrogue/graphics/widgets/my_widgets.py
--rw-rw-rw-   0        0        0      459 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/graphics/widgets/renderable.py
--rw-rw-rw-   0        0        0     3058 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/graphics/widgets/spaceship.py
--rw-rw-rw-   0        0        0    65669 2023-03-28 10:35:46.000000 qrogue-0.6.2.1/qrogue/graphics/widgets/widget_sets.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.629649 qrogue-0.6.2.1/qrogue/management/
--rw-rw-rw-   0        0        0      491 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/management/__init__.py
--rw-rw-rw-   0        0        0    15127 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/management/map_management.py
--rw-rw-rw-   0        0        0      372 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/management/pause.py
--rw-rw-rw-   0        0        0    32737 2023-03-28 10:31:00.000000 qrogue-0.6.2.1/qrogue/management/qrogue_pycui.py
--rw-rw-rw-   0        0        0     3938 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/management/save_data.py
--rw-rw-rw-   0        0        0     3140 2023-03-18 15:45:59.000000 qrogue-0.6.2.1/qrogue/management/story.py
--rw-rw-rw-   0        0        0     9953 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/qrogue.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.738941 qrogue-0.6.2.1/qrogue/util/
--rw-rw-rw-   0        0        0      376 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/__init__.py
--rw-rw-rw-   0        0        0    12301 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/achievements.py
--rw-rw-rw-   0        0        0     5750 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/common_messages.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:01.801449 qrogue-0.6.2.1/qrogue/util/config/
--rw-rw-rw-   0        0        0      447 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/config/__init__.py
--rw-rw-rw-   0        0        0     5130 2023-03-28 10:35:45.000000 qrogue-0.6.2.1/qrogue/util/config/config.py
--rw-rw-rw-   0        0        0      448 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/config/error_config.py
--rw-rw-rw-   0        0        0    14204 2023-03-28 10:31:00.000000 qrogue-0.6.2.1/qrogue/util/config/gameplay_config.py
--rw-rw-rw-   0        0        0    10930 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/config/path_config.py
--rw-rw-rw-   0        0        0     1033 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/config/py_cui_config.py
--rw-rw-rw-   0        0        0     1353 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/config/test_config.py
--rw-rw-rw-   0        0        0    10031 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/config/visual_config.py
--rw-rw-rw-   0        0        0     6243 2023-03-28 10:31:00.000000 qrogue-0.6.2.1/qrogue/util/controls.py
--rw-rw-rw-   0        0        0     6754 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/game_simulator.py
--rw-rw-rw-   0        0        0    15543 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/help_texts.py
--rw-rw-rw-   0        0        0     3529 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/key_logger.py
--rw-rw-rw-   0        0        0     4605 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/logger.py
--rw-rw-rw-   0        0        0     4791 2023-02-16 19:23:39.000000 qrogue-0.6.2.1/qrogue/util/my_random.py
--rw-rw-rw-   0        0        0     3669 2023-03-28 10:31:00.000000 qrogue-0.6.2.1/qrogue/util/util_functions.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:39:00.700217 qrogue-0.6.2.1/qrogue.egg-info/
--rw-rw-rw-   0        0        0     5311 2023-03-28 10:39:00.000000 qrogue-0.6.2.1/qrogue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4762 2023-03-28 10:39:00.000000 qrogue-0.6.2.1/qrogue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 10:39:00.000000 qrogue-0.6.2.1/qrogue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-03-28 10:39:00.000000 qrogue-0.6.2.1/qrogue.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       72 2023-03-28 10:39:00.000000 qrogue-0.6.2.1/qrogue.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-28 10:39:00.000000 qrogue-0.6.2.1/qrogue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-28 10:39:01.801449 qrogue-0.6.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2255 2023-03-28 10:35:45.000000 qrogue-0.6.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:44.174126 qrogue-0.6.3/
+-rw-rw-rw-   0        0        0     1092 2023-02-16 19:23:39.000000 qrogue-0.6.3/License.md
+-rw-rw-rw-   0        0        0       38 2023-02-16 19:23:39.000000 qrogue-0.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4387 2023-05-31 12:45:44.172150 qrogue-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3673 2023-05-31 12:30:35.000000 qrogue-0.6.3/Readme.md
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:42.737581 qrogue-0.6.3/qrogue/
+-rw-rw-rw-   0        0        0      289 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:42.781975 qrogue-0.6.3/qrogue/data/
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:42.852492 qrogue-0.6.3/qrogue/data/dungeons/
+-rw-rw-rw-   0        0        0     4477 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/data/dungeons/l0exam.qrdg
+-rw-rw-rw-   0        0        0     6419 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/data/dungeons/l0training.qrdg
+-rw-rw-rw-   0        0        0     4159 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/data/dungeons/l0v0.qrdg
+-rw-rw-rw-   0        0        0     3609 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/data/dungeons/l0v1.qrdg
+-rw-rw-rw-   0        0        0     3677 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/data/dungeons/l0v2.qrdg
+-rw-rw-rw-   0        0        0     4950 2023-03-20 11:36:39.000000 qrogue-0.6.3/qrogue/data/dungeons/l0v3.qrdg
+-rw-rw-rw-   0        0        0     6458 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/data/dungeons/l0v4.qrdg
+-rw-rw-rw-   0        0        0    10077 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/data/dungeons/l0v5.qrdg
+-rw-rw-rw-   0        0        0     1885 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/data/dungeons/w0.qrw
+-rw-rw-rw-   0        0        0     1275 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/data/dungeons/w1.qrw
+-rw-rw-rw-   0        0        0      786 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/data/dungeons/worlds.qrw
+-rw-rw-rw-   0        0        0      160 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/data/fresh.qrsave
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:42.854670 qrogue-0.6.3/qrogue/data/hallways/
+-rw-rw-rw-   0        0        0        0 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/data/hallways/templates.txt
+-rw-rw-rw-   0        0        0       12 2023-05-28 12:28:12.000000 qrogue-0.6.3/qrogue/data/qrogue_launch.config
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:42.880322 qrogue-0.6.3/qrogue/game/
+-rw-rw-rw-   0        0        0      212 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:42.899147 qrogue-0.6.3/qrogue/game/logic/
+-rw-rw-rw-   0        0        0      208 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:42.919432 qrogue-0.6.3/qrogue/game/logic/actors/
+-rw-rw-rw-   0        0        0      267 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/actors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.007142 qrogue-0.6.3/qrogue/game/logic/actors/controllables/
+-rw-rw-rw-   0        0        0      191 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/actors/controllables/__init__.py
+-rw-rw-rw-   0        0        0     2848 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/actors/controllables/controllable.py
+-rw-rw-rw-   0        0        0     1511 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/actors/controllables/player.py
+-rw-rw-rw-   0        0        0     2002 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/actors/controllables/qubit.py
+-rw-rw-rw-   0        0        0    29165 2023-05-28 11:31:02.000000 qrogue-0.6.3/qrogue/game/logic/actors/controllables/robot.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.065845 qrogue-0.6.3/qrogue/game/logic/actors/puzzles/
+-rw-rw-rw-   0        0        0      210 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/actors/puzzles/__init__.py
+-rw-rw-rw-   0        0        0     1343 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/actors/puzzles/boss.py
+-rw-rw-rw-   0        0        0     1273 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/actors/puzzles/challenge.py
+-rw-rw-rw-   0        0        0     1529 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/actors/puzzles/enemy.py
+-rw-rw-rw-   0        0        0     2091 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/actors/puzzles/riddle.py
+-rw-rw-rw-   0        0        0     2413 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/actors/puzzles/target.py
+-rw-rw-rw-   0        0        0    12329 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/actors/state_vector.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.145991 qrogue-0.6.3/qrogue/game/logic/collectibles/
+-rw-rw-rw-   0        0        0      534 2023-05-28 11:31:02.000000 qrogue-0.6.3/qrogue/game/logic/collectibles/__init__.py
+-rw-rw-rw-   0        0        0     2572 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/collectibles/collectible.py
+-rw-rw-rw-   0        0        0     7438 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/collectibles/collectible_factory.py
+-rw-rw-rw-   0        0        0     2029 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/collectibles/consumable.py
+-rw-rw-rw-   0        0        0     8459 2023-05-28 11:31:02.000000 qrogue-0.6.3/qrogue/game/logic/collectibles/instruction.py
+-rw-rw-rw-   0        0        0     2149 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/collectibles/pickup.py
+-rw-rw-rw-   0        0        0      954 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/collectibles/qubit.py
+-rw-rw-rw-   0        0        0     3350 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/logic/message.py
+-rw-rw-rw-   0        0        0     9533 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/target_factory.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.155138 qrogue-0.6.3/qrogue/game/world/
+-rw-rw-rw-   0        0        0      286 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.271629 qrogue-0.6.3/qrogue/game/world/dungeon_generator/
+-rw-rw-rw-   0        0        0    49157 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/QrogueLevelGenerator.py
+-rw-rw-rw-   0        0        0    16607 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/QrogueWorldGenerator.py
+-rw-rw-rw-   0        0        0      382 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.337193 qrogue-0.6.3/qrogue/game/world/dungeon_generator/dungeon_parser/
+-rw-rw-rw-   0        0        0    37933 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonLexer.py
+-rw-rw-rw-   0        0        0    11800 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonListener.py
+-rw-rw-rw-   0        0        0   157830 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonParser.py
+-rw-rw-rw-   0        0        0     7341 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonVisitor.py
+-rw-rw-rw-   0        0        0      744 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/generator.py
+-rw-rw-rw-   0        0        0     7173 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/parser_util.py
+-rw-rw-rw-   0        0        0    45168 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/random_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.392155 qrogue-0.6.3/qrogue/game/world/dungeon_generator/wave_function_collapse/
+-rw-rw-rw-   0        0        0      197 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/wave_function_collapse/__init__.py
+-rw-rw-rw-   0        0        0     2593 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/wave_function_collapse/learnables.py
+-rw-rw-rw-   0        0        0     2936 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/wave_function_collapse/wave_function.py
+-rw-rw-rw-   0        0        0    10188 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/wave_function_collapse/wfc_generator.py
+-rw-rw-rw-   0        0        0     3192 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/wave_function_collapse/wfc_learner.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.471390 qrogue-0.6.3/qrogue/game/world/dungeon_generator/world_parser/
+-rw-rw-rw-   0        0        0    21993 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldLexer.py
+-rw-rw-rw-   0        0        0     4780 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldListener.py
+-rw-rw-rw-   0        0        0    65975 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldParser.py
+-rw-rw-rw-   0        0        0     3072 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldVisitor.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.565941 qrogue-0.6.3/qrogue/game/world/map/
+-rw-rw-rw-   0        0        0      469 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/map/__init__.py
+-rw-rw-rw-   0        0        0     2481 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/map/callbacks.py
+-rw-rw-rw-   0        0        0      955 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/map/expedition_map.py
+-rw-rw-rw-   0        0        0      748 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/map/level_map.py
+-rw-rw-rw-   0        0        0    11948 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/map/map.py
+-rw-rw-rw-   0        0        0    37005 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/map/rooms.py
+-rw-rw-rw-   0        0        0    13912 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/map/spaceship_map.py
+-rw-rw-rw-   0        0        0     1206 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/map/world_map.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.585589 qrogue-0.6.3/qrogue/game/world/navigation/
+-rw-rw-rw-   0        0        0       84 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/navigation/__init__.py
+-rw-rw-rw-   0        0        0     4868 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/navigation/navigation.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.666842 qrogue-0.6.3/qrogue/game/world/tiles/
+-rw-rw-rw-   0        0        0      579 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/tiles/__init__.py
+-rw-rw-rw-   0        0        0     9250 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/tiles/door_tiles.py
+-rw-rw-rw-   0        0        0     6183 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/game/world/tiles/puzzle_tiles.py
+-rw-rw-rw-   0        0        0     8600 2023-03-28 10:41:57.000000 qrogue-0.6.3/qrogue/game/world/tiles/tiles.py
+-rw-rw-rw-   0        0        0    13377 2023-03-28 10:41:57.000000 qrogue-0.6.3/qrogue/game/world/tiles/walk_trigger_tiles.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.685419 qrogue-0.6.3/qrogue/graphics/
+-rw-rw-rw-   0        0        0      371 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/graphics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.727973 qrogue-0.6.3/qrogue/graphics/popups/
+-rw-rw-rw-   0        0        0      146 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/graphics/popups/__init__.py
+-rw-rw-rw-   0        0        0    11063 2023-05-28 11:31:02.000000 qrogue-0.6.3/qrogue/graphics/popups/multiline_popup.py
+-rw-rw-rw-   0        0        0     9120 2023-03-20 11:39:13.000000 qrogue-0.6.3/qrogue/graphics/popups/my_popups.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.774051 qrogue-0.6.3/qrogue/graphics/rendering/
+-rw-rw-rw-   0        0        0      237 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/graphics/rendering/__init__.py
+-rw-rw-rw-   0        0        0     5469 2023-03-28 10:41:57.000000 qrogue-0.6.3/qrogue/graphics/rendering/color_rules.py
+-rw-rw-rw-   0        0        0     6927 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/graphics/rendering/renderer.py
+-rw-rw-rw-   0        0        0     1886 2023-05-28 11:31:02.000000 qrogue-0.6.3/qrogue/graphics/widget_base.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.852561 qrogue-0.6.3/qrogue/graphics/widgets/
+-rw-rw-rw-   0        0        0      695 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/graphics/widgets/__init__.py
+-rw-rw-rw-   0        0        0    38781 2023-05-28 11:31:02.000000 qrogue-0.6.3/qrogue/graphics/widgets/my_widgets.py
+-rw-rw-rw-   0        0        0      459 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/graphics/widgets/renderable.py
+-rw-rw-rw-   0        0        0     3058 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/graphics/widgets/spaceship.py
+-rw-rw-rw-   0        0        0    65879 2023-05-28 11:31:02.000000 qrogue-0.6.3/qrogue/graphics/widgets/widget_sets.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:43.930120 qrogue-0.6.3/qrogue/management/
+-rw-rw-rw-   0        0        0      491 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/management/__init__.py
+-rw-rw-rw-   0        0        0    15127 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/management/map_management.py
+-rw-rw-rw-   0        0        0      372 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/management/pause.py
+-rw-rw-rw-   0        0        0    33663 2023-05-28 12:04:53.000000 qrogue-0.6.3/qrogue/management/qrogue_pycui.py
+-rw-rw-rw-   0        0        0     3938 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/management/save_data.py
+-rw-rw-rw-   0        0        0     3140 2023-03-18 15:45:59.000000 qrogue-0.6.3/qrogue/management/story.py
+-rw-rw-rw-   0        0        0     9953 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/qrogue.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:44.080808 qrogue-0.6.3/qrogue/util/
+-rw-rw-rw-   0        0        0      376 2023-05-28 11:31:02.000000 qrogue-0.6.3/qrogue/util/__init__.py
+-rw-rw-rw-   0        0        0    12356 2023-05-28 12:09:12.000000 qrogue-0.6.3/qrogue/util/achievements.py
+-rw-rw-rw-   0        0        0     5750 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/util/common_messages.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:44.170135 qrogue-0.6.3/qrogue/util/config/
+-rw-rw-rw-   0        0        0      447 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/util/config/__init__.py
+-rw-rw-rw-   0        0        0     5128 2023-05-31 12:30:35.000000 qrogue-0.6.3/qrogue/util/config/config.py
+-rw-rw-rw-   0        0        0      448 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/util/config/error_config.py
+-rw-rw-rw-   0        0        0    14204 2023-05-28 11:31:02.000000 qrogue-0.6.3/qrogue/util/config/gameplay_config.py
+-rw-rw-rw-   0        0        0    10930 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/util/config/path_config.py
+-rw-rw-rw-   0        0        0     1033 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/util/config/py_cui_config.py
+-rw-rw-rw-   0        0        0     1353 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/util/config/test_config.py
+-rw-rw-rw-   0        0        0    10031 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/util/config/visual_config.py
+-rw-rw-rw-   0        0        0     6243 2023-05-28 11:31:02.000000 qrogue-0.6.3/qrogue/util/controls.py
+-rw-rw-rw-   0        0        0     6754 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/util/game_simulator.py
+-rw-rw-rw-   0        0        0    15516 2023-05-31 12:20:06.000000 qrogue-0.6.3/qrogue/util/help_texts.py
+-rw-rw-rw-   0        0        0     3529 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/util/key_logger.py
+-rw-rw-rw-   0        0        0     4605 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/util/logger.py
+-rw-rw-rw-   0        0        0     4791 2023-02-16 19:23:39.000000 qrogue-0.6.3/qrogue/util/my_random.py
+-rw-rw-rw-   0        0        0     3669 2023-05-28 11:31:02.000000 qrogue-0.6.3/qrogue/util/util_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:45:42.778276 qrogue-0.6.3/qrogue.egg-info/
+-rw-rw-rw-   0        0        0     4387 2023-05-31 12:45:41.000000 qrogue-0.6.3/qrogue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4773 2023-05-31 12:45:41.000000 qrogue-0.6.3/qrogue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 12:45:41.000000 qrogue-0.6.3/qrogue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-31 12:45:41.000000 qrogue-0.6.3/qrogue.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       72 2023-05-31 12:45:41.000000 qrogue-0.6.3/qrogue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 12:45:41.000000 qrogue-0.6.3/qrogue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 12:45:44.174126 qrogue-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     2186 2023-05-31 12:30:35.000000 qrogue-0.6.3/setup.py
```

### Comparing `qrogue-0.6.2.1/Readme.md` & `qrogue-0.6.3/Readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 >         | |     | |  | '__/ _ \ / _` | | | |/ _ \
 >         | |_____| |  | | | (_) | (_| | |_| |  __/    
 >          \______\_\  |_|  \___/ \__, |\__,_|\___|   
 >                                  __/ |            
 >                                 |___/ 
 ASCII-Art generated by https://www.ascii-art-generator.org/
 
-# Qrogue v0.6.2.1 #
+# Qrogue v0.6.3 #
 
 Qrogue is a modernized Quantum Computing take of the classical game 
 [Rogue](https://en.wikipedia.org/wiki/Rogue_%28video_game%29). 
 
 You will play as a student whose dream is to travel through the galaxy. 
 As they hear about "Mission Quniverse" they immediately apply for its 
 training program to be able to join this fascinating Quantum Computing
```

### Comparing `qrogue-0.6.2.1/qrogue/data/dungeons/l0exam.qrdg` & `qrogue-0.6.3/qrogue/data/dungeons/l0exam.qrdg`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/data/dungeons/l0training.qrdg` & `qrogue-0.6.3/qrogue/data/dungeons/l0training.qrdg`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/data/dungeons/l0v0.qrdg` & `qrogue-0.6.3/qrogue/data/dungeons/l0v0.qrdg`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/data/dungeons/l0v1.qrdg` & `qrogue-0.6.3/qrogue/data/dungeons/l0v1.qrdg`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/data/dungeons/l0v2.qrdg` & `qrogue-0.6.3/qrogue/data/dungeons/l0v2.qrdg`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/data/dungeons/l0v3.qrdg` & `qrogue-0.6.3/qrogue/data/dungeons/l0v3.qrdg`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/data/dungeons/l0v4.qrdg` & `qrogue-0.6.3/qrogue/data/dungeons/l0v4.qrdg`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/data/dungeons/l0v5.qrdg` & `qrogue-0.6.3/qrogue/data/dungeons/l0v5.qrdg`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/data/dungeons/w0.qrw` & `qrogue-0.6.3/qrogue/data/dungeons/w0.qrw`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/data/dungeons/w1.qrw` & `qrogue-0.6.3/qrogue/data/dungeons/w1.qrw`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/data/dungeons/worlds.qrw` & `qrogue-0.6.3/qrogue/data/dungeons/worlds.qrw`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/actors/controllables/controllable.py` & `qrogue-0.6.3/qrogue/game/logic/actors/controllables/controllable.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/actors/controllables/player.py` & `qrogue-0.6.3/qrogue/game/logic/actors/controllables/player.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/actors/controllables/qubit.py` & `qrogue-0.6.3/qrogue/game/logic/actors/controllables/qubit.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/actors/controllables/robot.py` & `qrogue-0.6.3/qrogue/game/logic/actors/controllables/robot.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/actors/puzzles/boss.py` & `qrogue-0.6.3/qrogue/game/logic/actors/puzzles/boss.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/actors/puzzles/challenge.py` & `qrogue-0.6.3/qrogue/game/logic/actors/puzzles/challenge.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/actors/puzzles/enemy.py` & `qrogue-0.6.3/qrogue/game/logic/actors/puzzles/enemy.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/actors/puzzles/riddle.py` & `qrogue-0.6.3/qrogue/game/logic/actors/puzzles/riddle.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/actors/puzzles/target.py` & `qrogue-0.6.3/qrogue/game/logic/actors/puzzles/target.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/actors/state_vector.py` & `qrogue-0.6.3/qrogue/game/logic/actors/state_vector.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/collectibles/__init__.py` & `qrogue-0.6.3/qrogue/game/logic/collectibles/__init__.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/collectibles/collectible.py` & `qrogue-0.6.3/qrogue/game/logic/collectibles/collectible.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/collectibles/collectible_factory.py` & `qrogue-0.6.3/qrogue/game/logic/collectibles/collectible_factory.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/collectibles/consumable.py` & `qrogue-0.6.3/qrogue/game/logic/collectibles/consumable.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/collectibles/instruction.py` & `qrogue-0.6.3/qrogue/game/logic/collectibles/instruction.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/collectibles/pickup.py` & `qrogue-0.6.3/qrogue/game/logic/collectibles/pickup.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/collectibles/qubit.py` & `qrogue-0.6.3/qrogue/game/logic/collectibles/qubit.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/logic/message.py` & `qrogue-0.6.3/qrogue/game/logic/message.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/target_factory.py` & `qrogue-0.6.3/qrogue/game/target_factory.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/QrogueLevelGenerator.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/QrogueLevelGenerator.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/QrogueWorldGenerator.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/QrogueWorldGenerator.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonLexer.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonLexer.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonListener.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonListener.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonParser.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonParser.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonVisitor.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/dungeon_parser/QrogueDungeonVisitor.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/generator.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/generator.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/parser_util.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/parser_util.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/random_generator.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/random_generator.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/wave_function_collapse/learnables.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/wave_function_collapse/learnables.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/wave_function_collapse/wave_function.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/wave_function_collapse/wave_function.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/wave_function_collapse/wfc_generator.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/wave_function_collapse/wfc_generator.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/wave_function_collapse/wfc_learner.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/wave_function_collapse/wfc_learner.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldLexer.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldLexer.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldListener.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldListener.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldParser.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldParser.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldVisitor.py` & `qrogue-0.6.3/qrogue/game/world/dungeon_generator/world_parser/QrogueWorldVisitor.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/map/callbacks.py` & `qrogue-0.6.3/qrogue/game/world/map/callbacks.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/map/expedition_map.py` & `qrogue-0.6.3/qrogue/game/world/map/expedition_map.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/map/level_map.py` & `qrogue-0.6.3/qrogue/game/world/map/level_map.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/map/map.py` & `qrogue-0.6.3/qrogue/game/world/map/map.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/map/rooms.py` & `qrogue-0.6.3/qrogue/game/world/map/rooms.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/map/spaceship_map.py` & `qrogue-0.6.3/qrogue/game/world/map/spaceship_map.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/map/world_map.py` & `qrogue-0.6.3/qrogue/game/world/map/world_map.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/navigation/navigation.py` & `qrogue-0.6.3/qrogue/game/world/navigation/navigation.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/tiles/__init__.py` & `qrogue-0.6.3/qrogue/game/world/tiles/__init__.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/tiles/door_tiles.py` & `qrogue-0.6.3/qrogue/game/world/tiles/door_tiles.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/tiles/puzzle_tiles.py` & `qrogue-0.6.3/qrogue/game/world/tiles/puzzle_tiles.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/game/world/tiles/tiles.py` & `qrogue-0.6.3/qrogue/game/world/tiles/tiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,489 +45,494 @@
 000002c0: 2020 2320 7469 6c65 206f 6620 6120 706c    # tile of a pl
 000002d0: 6163 6520 7765 2063 616e 6e6f 7420 7365  ace we cannot se
 000002e0: 6520 7965 740d 0a0d 0a20 2020 204d 6573  e yet....    Mes
 000002f0: 7361 6765 203d 2028 362c 2022 2e22 2920  sage = (6, ".") 
 00000300: 2020 2020 2020 2020 2320 7469 6c65 2066          # tile f
 00000310: 6f72 2064 6973 706c 6179 696e 6720 6120  or displaying a 
 00000320: 706f 7075 7020 6d65 7373 6167 650d 0a20  popup message.. 
-00000330: 2020 2054 7269 6767 6572 203d 2028 392c     Trigger = (9,
-00000340: 2022 5422 2920 2020 2020 2020 2020 2320   "T")         # 
-00000350: 7469 6c65 2074 6861 7420 6361 6c6c 7320  tile that calls 
-00000360: 6120 6675 6e63 7469 6f6e 206f 6e20 7761  a function on wa
-00000370: 6c6b 2c20 692e 652e 2065 7665 6e74 2074  lk, i.e. event t
-00000380: 696c 650d 0a20 2020 2054 656c 6570 6f72  ile..    Telepor
-00000390: 7420 3d20 2839 312c 2022 7422 2920 2020  t = (91, "t")   
-000003a0: 2020 2020 2320 7370 6563 6961 6c20 7472      # special tr
-000003b0: 6967 6765 7220 666f 7220 7465 6c65 706f  igger for telepo
-000003c0: 7274 696e 6720 6265 7477 6565 6e20 6d61  rting between ma
-000003d0: 7073 0d0a 2020 2020 4465 636f 7261 7469  ps..    Decorati
-000003e0: 6f6e 203d 2028 3131 2c20 2264 2229 2020  on = (11, "d")  
-000003f0: 2020 2023 2073 696d 706c 7920 6469 7370     # simply disp
-00000400: 6c61 7973 2061 2073 7065 6369 6669 6564  lays a specified
-00000410: 2063 6861 7261 6374 6572 0d0a 0d0a 2020   character....  
-00000420: 2020 5761 6c6c 203d 2028 312c 2022 2322    Wall = (1, "#"
-00000430: 290d 0a20 2020 204f 6273 7461 636c 6520  )..    Obstacle 
-00000440: 3d20 2832 2c20 226f 2229 0d0a 2020 2020  = (2, "o")..    
-00000450: 446f 6f72 203d 2028 342c 2022 7c22 290d  Door = (4, "|").
-00000460: 0a0d 0a20 2020 2043 6f6e 7472 6f6c 6c61  ...    Controlla
-00000470: 626c 6520 3d20 2832 302c 2022 4322 290d  ble = (20, "C").
-00000480: 0a20 2020 204e 7063 203d 2028 3235 2c20  .    Npc = (25, 
-00000490: 224e 2229 0d0a 2020 2020 456e 656d 7920  "N")..    Enemy 
-000004a0: 3d20 2833 302c 2022 4522 290d 0a20 2020  = (30, "E")..   
-000004b0: 2042 6f73 7320 3d20 2834 302c 2022 4222   Boss = (40, "B"
-000004c0: 290d 0a0d 0a20 2020 2043 6f6c 6c65 6374  )....    Collect
-000004d0: 6962 6c65 203d 2028 3530 2c20 2263 2229  ible = (50, "c")
-000004e0: 0d0a 2020 2020 5269 6464 6c65 7220 3d20  ..    Riddler = 
-000004f0: 2835 312c 2022 3f22 290d 0a20 2020 2053  (51, "?")..    S
-00000500: 686f 704b 6565 7065 7220 3d20 2835 322c  hopKeeper = (52,
-00000510: 2022 2422 290d 0a20 2020 2045 6e65 7267   "$")..    Energ
-00000520: 7920 3d20 2835 332c 2022 6522 290d 0a20  y = (53, "e").. 
-00000530: 2020 2043 6861 6c6c 656e 6765 7220 3d20     Challenger = 
-00000540: 2835 342c 2022 2122 290d 0a0d 0a20 2020  (54, "!")....   
-00000550: 2053 7061 6365 7368 6970 426c 6f63 6b20   SpaceshipBlock 
-00000560: 3d20 2837 302c 2022 2f22 290d 0a20 2020  = (70, "/")..   
-00000570: 2053 7061 6365 7368 6970 5761 6c6b 203d   SpaceshipWalk =
-00000580: 2028 3731 2c20 222e 2229 0d0a 2020 2020   (71, ".")..    
-00000590: 5370 6163 6573 6869 7054 7269 6767 6572  SpaceshipTrigger
-000005a0: 203d 2028 3732 2c20 2254 2229 0d0a 2020   = (72, "T")..  
-000005b0: 2020 4f75 7465 7253 7061 6365 203d 2028    OuterSpace = (
-000005c0: 3733 2c20 222a 2229 0d0a 0d0a 2020 2020  73, "*")....    
-000005d0: 436f 6c6c 6563 7469 626c 654b 6579 203d  CollectibleKey =
-000005e0: 2028 3530 312c 2022 6b22 290d 0a20 2020   (501, "k")..   
-000005f0: 2043 6f6c 6c65 6374 6962 6c65 436f 696e   CollectibleCoin
-00000600: 203d 2028 3530 322c 2022 e282 ac22 290d   = (502, "...").
-00000610: 0a20 2020 2043 6f6c 6c65 6374 6962 6c65  .    Collectible
-00000620: 456e 6572 6779 203d 2028 3530 332c 2022  Energy = (503, "
-00000630: 6522 290d 0a20 2020 2043 6f6c 6c65 6374  e")..    Collect
-00000640: 6962 6c65 4761 7465 203d 2028 3532 302c  ibleGate = (520,
-00000650: 2022 6722 290d 0a20 2020 2043 6f6c 6c65   "g")..    Colle
-00000660: 6374 6962 6c65 5175 6269 7420 3d20 2835  ctibleQubit = (5
-00000670: 3630 2c20 2271 2229 0d0a 0d0a 2020 2020  60, "q")....    
-00000680: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00000690: 662c 2069 643a 2069 6e74 2c20 7265 7072  f, id: int, repr
-000006a0: 6573 656e 7461 7469 6f6e 3a20 7374 7229  esentation: str)
-000006b0: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-000006c0: 5f5f 6964 203d 2069 640d 0a20 2020 2020  __id = id..     
-000006d0: 2020 2073 656c 662e 5f5f 7265 7072 6573     self.__repres
-000006e0: 656e 7461 7469 6f6e 203d 2072 6570 7265  entation = repre
-000006f0: 7365 6e74 6174 696f 6e0d 0a0d 0a20 2020  sentation....   
-00000700: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-00000710: 6465 6620 6964 2873 656c 6629 202d 3e20  def id(self) -> 
-00000720: 696e 743a 0d0a 2020 2020 2020 2020 7265  int:..        re
-00000730: 7475 726e 2073 656c 662e 5f5f 6964 0d0a  turn self.__id..
-00000740: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-00000750: 0a20 2020 2064 6566 2072 6570 7265 7365  .    def represe
-00000760: 6e74 6174 696f 6e28 7365 6c66 2920 2d3e  ntation(self) ->
-00000770: 2073 7472 3a0d 0a20 2020 2020 2020 2072   str:..        r
-00000780: 6574 7572 6e20 7365 6c66 2e5f 5f72 6570  eturn self.__rep
-00000790: 7265 7365 6e74 6174 696f 6e0d 0a0d 0a20  resentation.... 
-000007a0: 2020 2064 6566 205f 5f73 7472 5f5f 2873     def __str__(s
-000007b0: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-000007c0: 6574 7572 6e20 7365 6c66 2e72 6570 7265  eturn self.repre
-000007d0: 7365 6e74 6174 696f 6e0d 0a0d 0a20 2020  sentation....   
-000007e0: 2040 7374 6174 6963 6d65 7468 6f64 0d0a   @staticmethod..
-000007f0: 2020 2020 6465 6620 7370 6563 6961 6c5f      def special_
-00000800: 7661 6c75 6573 2829 202d 3e20 4c69 7374  values() -> List
-00000810: 5b22 5469 6c65 436f 6465 225d 3a0d 0a20  ["TileCode"]:.. 
-00000820: 2020 2020 2020 2072 6574 7572 6e20 5b0d         return [.
-00000830: 0a20 2020 2020 2020 2020 2020 2054 696c  .            Til
-00000840: 6543 6f64 652e 496e 7661 6c69 642c 2054  eCode.Invalid, T
-00000850: 696c 6543 6f64 652e 4465 6275 672c 2054  ileCode.Debug, T
-00000860: 696c 6543 6f64 652e 566f 6964 2c20 5469  ileCode.Void, Ti
-00000870: 6c65 436f 6465 2e46 6f67 4f66 5761 722c  leCode.FogOfWar,
-00000880: 0d0a 2020 2020 2020 2020 2020 2020 5469  ..            Ti
-00000890: 6c65 436f 6465 2e4d 6573 7361 6765 2c20  leCode.Message, 
-000008a0: 5469 6c65 436f 6465 2e54 7269 6767 6572  TileCode.Trigger
-000008b0: 2c20 5469 6c65 436f 6465 2e54 656c 6570  , TileCode.Telep
-000008c0: 6f72 742c 2054 696c 6543 6f64 652e 4465  ort, TileCode.De
-000008d0: 636f 7261 7469 6f6e 2c0d 0a20 2020 2020  coration,..     
-000008e0: 2020 205d 0d0a 0d0a 2020 2020 4073 7461     ]....    @sta
-000008f0: 7469 636d 6574 686f 640d 0a20 2020 2064  ticmethod..    d
-00000900: 6566 2063 6f6c 6c65 6374 6962 6c65 5f73  ef collectible_s
-00000910: 7562 7479 7065 7328 2920 2d3e 204c 6973  ubtypes() -> Lis
-00000920: 745b 2254 696c 6543 6f64 6522 5d3a 0d0a  t["TileCode"]:..
-00000930: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-00000940: 0d0a 2020 2020 2020 2020 2020 2020 5469  ..            Ti
-00000950: 6c65 436f 6465 2e43 6f6c 6c65 6374 6962  leCode.Collectib
-00000960: 6c65 2c0d 0a20 2020 2020 2020 2020 2020  le,..           
-00000970: 2054 696c 6543 6f64 652e 436f 6c6c 6563   TileCode.Collec
-00000980: 7469 626c 654b 6579 2c20 5469 6c65 436f  tibleKey, TileCo
-00000990: 6465 2e43 6f6c 6c65 6374 6962 6c65 436f  de.CollectibleCo
-000009a0: 696e 2c20 5469 6c65 436f 6465 2e43 6f6c  in, TileCode.Col
-000009b0: 6c65 6374 6962 6c65 456e 6572 6779 2c0d  lectibleEnergy,.
-000009c0: 0a20 2020 2020 2020 2020 2020 2054 696c  .            Til
-000009d0: 6543 6f64 652e 436f 6c6c 6563 7469 626c  eCode.Collectibl
-000009e0: 6547 6174 652c 2054 696c 6543 6f64 652e  eGate, TileCode.
-000009f0: 436f 6c6c 6563 7469 626c 6551 7562 6974  CollectibleQubit
-00000a00: 2c0d 0a20 2020 2020 2020 205d 0d0a 0d0a  ,..        ]....
-00000a10: 0d0a 636c 6173 7320 5469 6c65 2841 4243  ..class Tile(ABC
-00000a20: 293a 0d0a 2020 2020 4073 7461 7469 636d  ):..    @staticm
-00000a30: 6574 686f 640d 0a20 2020 2064 6566 205f  ethod..    def _
-00000a40: 696e 7669 7369 626c 655f 7469 6c65 2829  invisible_tile()
-00000a50: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00000a60: 6e20 2220 220d 0a0d 0a20 2020 2064 6566  n " "....    def
-00000a70: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00000a80: 636f 6465 3a20 5469 6c65 436f 6465 293a  code: TileCode):
-00000a90: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00000aa0: 5f63 6f64 6520 3d20 636f 6465 0d0a 0d0a  _code = code....
-00000ab0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-00000ac0: 2020 2064 6566 2064 6174 6128 7365 6c66     def data(self
-00000ad0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
-00000ae0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00000af0: 2045 2e67 2e20 616d 6f75 6e74 2066 6f72   E.g. amount for
-00000b00: 2045 6e65 7267 792c 206c 6f67 6963 616c   Energy, logical
-00000b10: 2043 6f6c 6c65 6374 6962 6c65 2066 6f72   Collectible for
-00000b20: 2043 6f6c 6c65 6374 6962 6c65 732c 2065   Collectibles, e
-00000b30: 6964 2066 6f72 2045 6e65 6d69 6573 206f  id for Enemies o
-00000b40: 7220 4e6f 6e65 2066 6f72 2074 696c 6573  r None for tiles
-00000b50: 2077 6974 686f 7574 2061 6e79 0d0a 2020   without any..  
-00000b60: 2020 2020 2020 6479 6e61 6d69 6320 7661        dynamic va
-00000b70: 6c75 6573 2028 5761 6c6c 732c 2046 6c6f  lues (Walls, Flo
-00000b80: 6f72 2c20 2e2e 2e29 0d0a 0d0a 2020 2020  or, ...)....    
-00000b90: 2020 2020 3a72 6574 7572 6e3a 2061 2072      :return: a r
-00000ba0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-00000bb0: 2074 6865 2073 7065 6369 6669 6320 7469   the specific ti
-00000bc0: 6c65 2773 2064 6174 610d 0a20 2020 2020  le's data..     
-00000bd0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00000be0: 7265 7475 726e 204e 6f6e 650d 0a0d 0a20  return None.... 
-00000bf0: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
-00000c00: 2020 6465 6620 636f 6465 2873 656c 6629    def code(self)
-00000c10: 202d 3e20 5469 6c65 436f 6465 3a0d 0a20   -> TileCode:.. 
-00000c20: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00000c30: 6c66 2e5f 5f63 6f64 650d 0a0d 0a20 2020  lf.__code....   
-00000c40: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-00000c50: 6465 6620 5f69 6e76 6973 6962 6c65 2873  def _invisible(s
-00000c60: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00000c70: 6574 7572 6e20 5469 6c65 2e5f 696e 7669  eturn Tile._invi
-00000c80: 7369 626c 655f 7469 6c65 2829 0d0a 0d0a  sible_tile()....
-00000c90: 2020 2020 4061 6273 7472 6163 746d 6574      @abstractmet
-00000ca0: 686f 640d 0a20 2020 2064 6566 2067 6574  hod..    def get
-00000cb0: 5f69 6d67 2873 656c 6629 3a0d 0a20 2020  _img(self):..   
-00000cc0: 2020 2020 2070 6173 730d 0a0d 0a20 2020       pass....   
-00000cd0: 2040 6162 7374 7261 6374 6d65 7468 6f64   @abstractmethod
-00000ce0: 0d0a 2020 2020 6465 6620 6973 5f77 616c  ..    def is_wal
-00000cf0: 6b61 626c 6528 7365 6c66 2c20 6469 7265  kable(self, dire
-00000d00: 6374 696f 6e3a 2044 6972 6563 7469 6f6e  ction: Direction
-00000d10: 2c20 636f 6e74 726f 6c6c 6162 6c65 3a20  , controllable: 
-00000d20: 436f 6e74 726f 6c6c 6162 6c65 2920 2d3e  Controllable) ->
-00000d30: 2062 6f6f 6c3a 0d0a 2020 2020 2020 2020   bool:..        
-00000d40: 7061 7373 0d0a 0d0a 2020 2020 4061 6273  pass....    @abs
-00000d50: 7472 6163 746d 6574 686f 640d 0a20 2020  tractmethod..   
-00000d60: 2064 6566 2063 6f70 7928 7365 6c66 2920   def copy(self) 
-00000d70: 2d3e 2022 5469 6c65 223a 0d0a 2020 2020  -> "Tile":..    
-00000d80: 2020 2020 7061 7373 0d0a 0d0a 2020 2020      pass....    
-00000d90: 6465 6620 5f5f 7374 725f 5f28 7365 6c66  def __str__(self
-00000da0: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-00000db0: 726e 2073 656c 662e 6765 745f 696d 6728  rn self.get_img(
-00000dc0: 290d 0a0d 0a0d 0a63 6c61 7373 2049 6e76  )......class Inv
-00000dd0: 616c 6964 2854 696c 6529 3a0d 0a20 2020  alid(Tile):..   
-00000de0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00000df0: 6c66 293a 0d0a 2020 2020 2020 2020 7375  lf):..        su
-00000e00: 7065 7228 292e 5f5f 696e 6974 5f5f 2854  per().__init__(T
-00000e10: 696c 6543 6f64 652e 496e 7661 6c69 6429  ileCode.Invalid)
-00000e20: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
-00000e30: 790d 0a20 2020 2064 6566 2064 6174 6128  y..    def data(
-00000e40: 7365 6c66 2920 2d3e 204e 6f6e 653a 0d0a  self) -> None:..
-00000e50: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00000e60: 6f6e 650d 0a0d 0a20 2020 2064 6566 2067  one....    def g
-00000e70: 6574 5f69 6d67 2873 656c 6629 3a0d 0a20  et_img(self):.. 
-00000e80: 2020 2020 2020 2072 6574 7572 6e20 5469         return Ti
-00000e90: 6c65 436f 6465 2e49 6e76 616c 6964 2e72  leCode.Invalid.r
-00000ea0: 6570 7265 7365 6e74 6174 696f 6e0d 0a0d  epresentation...
-00000eb0: 0a20 2020 2064 6566 2069 735f 7761 6c6b  .    def is_walk
-00000ec0: 6162 6c65 2873 656c 662c 2064 6972 6563  able(self, direc
-00000ed0: 7469 6f6e 3a20 4469 7265 6374 696f 6e2c  tion: Direction,
-00000ee0: 2063 6f6e 7472 6f6c 6c61 626c 653a 2043   controllable: C
-00000ef0: 6f6e 7472 6f6c 6c61 626c 6529 202d 3e20  ontrollable) -> 
-00000f00: 626f 6f6c 3a0d 0a20 2020 2020 2020 2072  bool:..        r
-00000f10: 6574 7572 6e20 4661 6c73 650d 0a0d 0a20  eturn False.... 
-00000f20: 2020 2064 6566 2063 6f70 7928 7365 6c66     def copy(self
-00000f30: 2920 2d3e 2022 5469 6c65 223a 0d0a 2020  ) -> "Tile":..  
-00000f40: 2020 2020 2020 7265 7475 726e 2049 6e76        return Inv
-00000f50: 616c 6964 2829 0d0a 0d0a 0d0a 636c 6173  alid()......clas
-00000f60: 7320 4465 6275 6728 5469 6c65 293a 0d0a  s Debug(Tile):..
-00000f70: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00000f80: 2873 656c 662c 206e 756d 3a20 696e 7429  (self, num: int)
-00000f90: 3a0d 0a20 2020 2020 2020 2073 7570 6572  :..        super
-00000fa0: 2844 6562 7567 2c20 7365 6c66 292e 5f5f  (Debug, self).__
-00000fb0: 696e 6974 5f5f 2854 696c 6543 6f64 652e  init__(TileCode.
-00000fc0: 4465 6275 6729 0d0a 2020 2020 2020 2020  Debug)..        
-00000fd0: 7365 6c66 2e5f 5f6e 756d 203d 2073 7472  self.__num = str
-00000fe0: 286e 756d 295b 305d 0d0a 0d0a 2020 2020  (num)[0]....    
-00000ff0: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
-00001000: 6566 2064 6174 6128 7365 6c66 2920 2d3e  ef data(self) ->
-00001010: 2069 6e74 3a0d 0a20 2020 2020 2020 2072   int:..        r
-00001020: 6574 7572 6e20 7365 6c66 2e5f 5f6e 756d  eturn self.__num
-00001030: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
-00001040: 696d 6728 7365 6c66 2920 2d3e 2073 7472  img(self) -> str
-00001050: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00001060: 6e20 7365 6c66 2e5f 5f6e 756d 0d0a 0d0a  n self.__num....
-00001070: 2020 2020 6465 6620 6973 5f77 616c 6b61      def is_walka
-00001080: 626c 6528 7365 6c66 2c20 6469 7265 6374  ble(self, direct
-00001090: 696f 6e3a 2044 6972 6563 7469 6f6e 2c20  ion: Direction, 
-000010a0: 636f 6e74 726f 6c6c 6162 6c65 3a20 436f  controllable: Co
-000010b0: 6e74 726f 6c6c 6162 6c65 2920 2d3e 2062  ntrollable) -> b
-000010c0: 6f6f 6c3a 0d0a 2020 2020 2020 2020 7265  ool:..        re
-000010d0: 7475 726e 2046 616c 7365 0d0a 0d0a 2020  turn False....  
-000010e0: 2020 6465 6620 636f 7079 2873 656c 6629    def copy(self)
-000010f0: 202d 3e20 2254 696c 6522 3a0d 0a20 2020   -> "Tile":..   
-00001100: 2020 2020 2072 6574 7572 6e20 4465 6275       return Debu
-00001110: 6728 696e 7428 7365 6c66 2e5f 5f6e 756d  g(int(self.__num
-00001120: 2929 0d0a 0d0a 0d0a 636c 6173 7320 566f  ))......class Vo
-00001130: 6964 2854 696c 6529 3a0d 0a20 2020 2064  id(Tile):..    d
-00001140: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00001150: 293a 0d0a 2020 2020 2020 2020 7375 7065  ):..        supe
-00001160: 7228 292e 5f5f 696e 6974 5f5f 2854 696c  r().__init__(Til
-00001170: 6543 6f64 652e 466c 6f6f 7229 0d0a 0d0a  eCode.Floor)....
-00001180: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-00001190: 2020 2064 6566 2064 6174 6128 7365 6c66     def data(self
-000011a0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
-000011b0: 2020 2020 7265 7475 726e 204e 6f6e 650d      return None.
-000011c0: 0a0d 0a20 2020 2064 6566 2067 6574 5f69  ...    def get_i
-000011d0: 6d67 2873 656c 6629 3a0d 0a20 2020 2020  mg(self):..     
-000011e0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000011f0: 696e 7669 7369 626c 650d 0a0d 0a20 2020  invisible....   
-00001200: 2064 6566 2069 735f 7761 6c6b 6162 6c65   def is_walkable
-00001210: 2873 656c 662c 2064 6972 6563 7469 6f6e  (self, direction
-00001220: 3a20 4469 7265 6374 696f 6e2c 2063 6f6e  : Direction, con
-00001230: 7472 6f6c 6c61 626c 653a 2043 6f6e 7472  trollable: Contr
-00001240: 6f6c 6c61 626c 6529 202d 3e20 626f 6f6c  ollable) -> bool
-00001250: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00001260: 6e20 4661 6c73 650d 0a0d 0a20 2020 2064  n False....    d
-00001270: 6566 2063 6f70 7928 7365 6c66 2920 2d3e  ef copy(self) ->
-00001280: 2022 5469 6c65 223a 0d0a 2020 2020 2020   "Tile":..      
-00001290: 2020 7265 7475 726e 2056 6f69 6428 290d    return Void().
-000012a0: 0a0d 0a0d 0a63 6c61 7373 2046 6c6f 6f72  .....class Floor
-000012b0: 2854 696c 6529 3a0d 0a20 2020 2040 7374  (Tile):..    @st
-000012c0: 6174 6963 6d65 7468 6f64 0d0a 2020 2020  aticmethod..    
-000012d0: 6465 6620 696d 6728 293a 0d0a 2020 2020  def img():..    
-000012e0: 2020 2020 7265 7475 726e 2054 696c 652e      return Tile.
-000012f0: 5f69 6e76 6973 6962 6c65 5f74 696c 6528  _invisible_tile(
-00001300: 290d 0a0d 0a20 2020 2064 6566 205f 5f69  )....    def __i
-00001310: 6e69 745f 5f28 7365 6c66 293a 0d0a 2020  nit__(self):..  
-00001320: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
-00001330: 696e 6974 5f5f 2854 696c 6543 6f64 652e  init__(TileCode.
-00001340: 466c 6f6f 7229 0d0a 0d0a 2020 2020 4070  Floor)....    @p
-00001350: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
-00001360: 2064 6174 6128 7365 6c66 2920 2d3e 204e   data(self) -> N
-00001370: 6f6e 653a 0d0a 2020 2020 2020 2020 7265  one:..        re
-00001380: 7475 726e 204e 6f6e 650d 0a0d 0a20 2020  turn None....   
-00001390: 2064 6566 2067 6574 5f69 6d67 2873 656c   def get_img(sel
-000013a0: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-000013b0: 7572 6e20 466c 6f6f 722e 696d 6728 290d  urn Floor.img().
-000013c0: 0a0d 0a20 2020 2064 6566 2069 735f 7761  ...    def is_wa
-000013d0: 6c6b 6162 6c65 2873 656c 662c 2064 6972  lkable(self, dir
-000013e0: 6563 7469 6f6e 3a20 4469 7265 6374 696f  ection: Directio
-000013f0: 6e2c 2063 6f6e 7472 6f6c 6c61 626c 653a  n, controllable:
-00001400: 2043 6f6e 7472 6f6c 6c61 626c 6529 202d   Controllable) -
-00001410: 3e20 626f 6f6c 3a0d 0a20 2020 2020 2020  > bool:..       
-00001420: 2072 6574 7572 6e20 5472 7565 0d0a 0d0a   return True....
-00001430: 2020 2020 6465 6620 636f 7079 2873 656c      def copy(sel
-00001440: 6629 202d 3e20 2254 696c 6522 3a0d 0a20  f) -> "Tile":.. 
-00001450: 2020 2020 2020 2072 6574 7572 6e20 466c         return Fl
-00001460: 6f6f 7228 290d 0a0d 0a0d 0a63 6c61 7373  oor()......class
-00001470: 2057 616c 6c28 5469 6c65 293a 0d0a 2020   Wall(Tile):..  
-00001480: 2020 4073 7461 7469 636d 6574 686f 640d    @staticmethod.
-00001490: 0a20 2020 2064 6566 2069 6d67 2829 3a0d  .    def img():.
-000014a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000014b0: 5469 6c65 436f 6465 2e57 616c 6c2e 7265  TileCode.Wall.re
-000014c0: 7072 6573 656e 7461 7469 6f6e 0d0a 0d0a  presentation....
-000014d0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000014e0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-000014f0: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
-00001500: 5f28 5469 6c65 436f 6465 2e57 616c 6c29  _(TileCode.Wall)
-00001510: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
-00001520: 790d 0a20 2020 2064 6566 2064 6174 6128  y..    def data(
-00001530: 7365 6c66 2920 2d3e 204e 6f6e 653a 0d0a  self) -> None:..
-00001540: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00001550: 6f6e 650d 0a0d 0a20 2020 2064 6566 2067  one....    def g
-00001560: 6574 5f69 6d67 2873 656c 6629 3a0d 0a20  et_img(self):.. 
-00001570: 2020 2020 2020 2072 6574 7572 6e20 5761         return Wa
-00001580: 6c6c 2e69 6d67 2829 0d0a 0d0a 2020 2020  ll.img()....    
-00001590: 6465 6620 6973 5f77 616c 6b61 626c 6528  def is_walkable(
-000015a0: 7365 6c66 2c20 6469 7265 6374 696f 6e3a  self, direction:
-000015b0: 2044 6972 6563 7469 6f6e 2c20 636f 6e74   Direction, cont
-000015c0: 726f 6c6c 6162 6c65 3a20 436f 6e74 726f  rollable: Contro
-000015d0: 6c6c 6162 6c65 2920 2d3e 2062 6f6f 6c3a  llable) -> bool:
-000015e0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000015f0: 2046 616c 7365 0d0a 0d0a 2020 2020 6465   False....    de
-00001600: 6620 636f 7079 2873 656c 6629 202d 3e20  f copy(self) -> 
-00001610: 2254 696c 6522 3a0d 0a20 2020 2020 2020  "Tile":..       
-00001620: 2072 6574 7572 6e20 5761 6c6c 2829 0d0a   return Wall()..
-00001630: 0d0a 0d0a 636c 6173 7320 4f62 7374 6163  ....class Obstac
-00001640: 6c65 2854 696c 6529 3a0d 0a20 2020 2064  le(Tile):..    d
-00001650: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00001660: 293a 0d0a 2020 2020 2020 2020 7375 7065  ):..        supe
-00001670: 7228 292e 5f5f 696e 6974 5f5f 2854 696c  r().__init__(Til
-00001680: 6543 6f64 652e 4f62 7374 6163 6c65 290d  eCode.Obstacle).
-00001690: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-000016a0: 0d0a 2020 2020 6465 6620 6461 7461 2873  ..    def data(s
-000016b0: 656c 6629 202d 3e20 4e6f 6e65 3a0d 0a20  elf) -> None:.. 
-000016c0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-000016d0: 6e65 0d0a 0d0a 2020 2020 6465 6620 6765  ne....    def ge
-000016e0: 745f 696d 6728 7365 6c66 293a 0d0a 2020  t_img(self):..  
-000016f0: 2020 2020 2020 7265 7475 726e 2054 696c        return Til
-00001700: 6543 6f64 652e 4f62 7374 6163 6c65 2e72  eCode.Obstacle.r
-00001710: 6570 7265 7365 6e74 6174 696f 6e0d 0a0d  epresentation...
-00001720: 0a20 2020 2064 6566 2069 735f 7761 6c6b  .    def is_walk
-00001730: 6162 6c65 2873 656c 662c 2064 6972 6563  able(self, direc
-00001740: 7469 6f6e 3a20 4469 7265 6374 696f 6e2c  tion: Direction,
-00001750: 2063 6f6e 7472 6f6c 6c61 626c 653a 2043   controllable: C
-00001760: 6f6e 7472 6f6c 6c61 626c 6529 202d 3e20  ontrollable) -> 
-00001770: 626f 6f6c 3a0d 0a20 2020 2020 2020 2072  bool:..        r
-00001780: 6574 7572 6e20 4661 6c73 6520 6f72 2043  eturn False or C
-00001790: 6865 6174 436f 6e66 6967 2e69 676e 6f72  heatConfig.ignor
-000017a0: 655f 6f62 7374 6163 6c65 7328 290d 0a0d  e_obstacles()...
-000017b0: 0a20 2020 2064 6566 2063 6f70 7928 7365  .    def copy(se
-000017c0: 6c66 2920 2d3e 2022 5469 6c65 223a 0d0a  lf) -> "Tile":..
-000017d0: 2020 2020 2020 2020 7265 7475 726e 204f          return O
-000017e0: 6273 7461 636c 6528 290d 0a0d 0a0d 0a63  bstacle()......c
-000017f0: 6c61 7373 2046 6f67 4f66 5761 7228 5469  lass FogOfWar(Ti
-00001800: 6c65 293a 0d0a 2020 2020 6465 6620 5f5f  le):..    def __
-00001810: 696e 6974 5f5f 2873 656c 6629 3a0d 0a20  init__(self):.. 
-00001820: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
-00001830: 5f69 6e69 745f 5f28 5469 6c65 436f 6465  _init__(TileCode
-00001840: 2e4f 6273 7461 636c 6529 0d0a 0d0a 2020  .Obstacle)....  
-00001850: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
-00001860: 2064 6566 2064 6174 6128 7365 6c66 2920   def data(self) 
-00001870: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
-00001880: 2020 7265 7475 726e 204e 6f6e 650d 0a0d    return None...
-00001890: 0a20 2020 2064 6566 2067 6574 5f69 6d67  .    def get_img
-000018a0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-000018b0: 2072 6574 7572 6e20 5469 6c65 436f 6465   return TileCode
-000018c0: 2e46 6f67 4f66 5761 722e 7265 7072 6573  .FogOfWar.repres
-000018d0: 656e 7461 7469 6f6e 0d0a 0d0a 2020 2020  entation....    
-000018e0: 6465 6620 6973 5f77 616c 6b61 626c 6528  def is_walkable(
-000018f0: 7365 6c66 2c20 6469 7265 6374 696f 6e3a  self, direction:
-00001900: 2044 6972 6563 7469 6f6e 2c20 636f 6e74   Direction, cont
-00001910: 726f 6c6c 6162 6c65 3a20 436f 6e74 726f  rollable: Contro
-00001920: 6c6c 6162 6c65 2920 2d3e 2062 6f6f 6c3a  llable) -> bool:
-00001930: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001940: 2054 7275 650d 0a0d 0a20 2020 2064 6566   True....    def
-00001950: 2063 6f70 7928 7365 6c66 2920 2d3e 2022   copy(self) -> "
-00001960: 5469 6c65 223a 0d0a 2020 2020 2020 2020  Tile":..        
-00001970: 7265 7475 726e 2046 6f67 4f66 5761 7228  return FogOfWar(
-00001980: 290d 0a0d 0a0d 0a63 6c61 7373 2044 6563  )......class Dec
-00001990: 6f72 6174 696f 6e28 5469 6c65 293a 0d0a  oration(Tile):..
-000019a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000019b0: 2873 656c 662c 2064 6563 6f72 6174 696f  (self, decoratio
-000019c0: 6e3a 2073 7472 2c20 626c 6f63 6b69 6e67  n: str, blocking
-000019d0: 3a20 626f 6f6c 203d 2046 616c 7365 293a  : bool = False):
-000019e0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-000019f0: 4465 636f 7261 7469 6f6e 2c20 7365 6c66  Decoration, self
-00001a00: 292e 5f5f 696e 6974 5f5f 2854 696c 6543  ).__init__(TileC
-00001a10: 6f64 652e 4465 636f 7261 7469 6f6e 290d  ode.Decoration).
-00001a20: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
-00001a30: 6465 636f 7261 7469 6f6e 203d 2064 6563  decoration = dec
-00001a40: 6f72 6174 696f 6e0d 0a20 2020 2020 2020  oration..       
-00001a50: 2073 656c 662e 5f5f 626c 6f63 6b69 6e67   self.__blocking
-00001a60: 203d 2062 6c6f 636b 696e 670d 0a0d 0a20   = blocking.... 
-00001a70: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
-00001a80: 2020 6465 6620 6461 7461 2873 656c 6629    def data(self)
-00001a90: 202d 3e20 626f 6f6c 3a0d 0a20 2020 2020   -> bool:..     
-00001aa0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00001ab0: 5f62 6c6f 636b 696e 670d 0a0d 0a20 2020  _blocking....   
-00001ac0: 2064 6566 2067 6574 5f69 6d67 2873 656c   def get_img(sel
-00001ad0: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-00001ae0: 7572 6e20 7365 6c66 2e5f 5f64 6563 6f72  urn self.__decor
-00001af0: 6174 696f 6e0d 0a0d 0a20 2020 2064 6566  ation....    def
-00001b00: 2069 735f 7761 6c6b 6162 6c65 2873 656c   is_walkable(sel
-00001b10: 662c 2064 6972 6563 7469 6f6e 3a20 4469  f, direction: Di
-00001b20: 7265 6374 696f 6e2c 2063 6f6e 7472 6f6c  rection, control
-00001b30: 6c61 626c 653a 2043 6f6e 7472 6f6c 6c61  lable: Controlla
-00001b40: 626c 6529 202d 3e20 626f 6f6c 3a0d 0a20  ble) -> bool:.. 
-00001b50: 2020 2020 2020 2072 6574 7572 6e20 6e6f         return no
-00001b60: 7420 7365 6c66 2e5f 5f62 6c6f 636b 696e  t self.__blockin
-00001b70: 670d 0a0d 0a20 2020 2064 6566 2063 6f70  g....    def cop
-00001b80: 7928 7365 6c66 2920 2d3e 2022 5469 6c65  y(self) -> "Tile
-00001b90: 223a 0d0a 2020 2020 2020 2020 7265 7475  ":..        retu
-00001ba0: 726e 2044 6563 6f72 6174 696f 6e28 7365  rn Decoration(se
-00001bb0: 6c66 2e5f 5f64 6563 6f72 6174 696f 6e2c  lf.__decoration,
-00001bc0: 2073 656c 662e 5f5f 626c 6f63 6b69 6e67   self.__blocking
-00001bd0: 290d 0a0d 0a0d 0a63 6c61 7373 2043 6f6e  )......class Con
-00001be0: 7472 6f6c 6c61 626c 6554 696c 6528 5469  trollableTile(Ti
-00001bf0: 6c65 293a 0d0a 2020 2020 6465 6620 5f5f  le):..    def __
-00001c00: 696e 6974 5f5f 2873 656c 662c 2063 6f6e  init__(self, con
-00001c10: 7472 6f6c 6c61 626c 653a 2043 6f6e 7472  trollable: Contr
-00001c20: 6f6c 6c61 626c 6529 3a0d 0a20 2020 2020  ollable):..     
-00001c30: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-00001c40: 745f 5f28 5469 6c65 436f 6465 2e43 6f6e  t__(TileCode.Con
-00001c50: 7472 6f6c 6c61 626c 6529 0d0a 2020 2020  trollable)..    
-00001c60: 2020 2020 7365 6c66 2e5f 5f63 6f6e 7472      self.__contr
-00001c70: 6f6c 6c61 626c 6520 3d20 636f 6e74 726f  ollable = contro
-00001c80: 6c6c 6162 6c65 0d0a 0d0a 2020 2020 4070  llable....    @p
-00001c90: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
-00001ca0: 2064 6174 6128 7365 6c66 2920 2d3e 2073   data(self) -> s
-00001cb0: 7472 3a0d 0a20 2020 2020 2020 2072 6574  tr:..        ret
-00001cc0: 7572 6e20 7365 6c66 2e5f 5f63 6f6e 7472  urn self.__contr
-00001cd0: 6f6c 6c61 626c 652e 6e61 6d65 0d0a 0d0a  ollable.name....
-00001ce0: 2020 2020 6465 6620 6765 745f 696d 6728      def get_img(
-00001cf0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00001d00: 7265 7475 726e 2073 656c 662e 5f5f 636f  return self.__co
-00001d10: 6e74 726f 6c6c 6162 6c65 2e67 6574 5f69  ntrollable.get_i
-00001d20: 6d67 2829 0d0a 0d0a 2020 2020 6465 6620  mg()....    def 
-00001d30: 6973 5f77 616c 6b61 626c 6528 7365 6c66  is_walkable(self
-00001d40: 2c20 6469 7265 6374 696f 6e3a 2044 6972  , direction: Dir
-00001d50: 6563 7469 6f6e 2c20 636f 6e74 726f 6c6c  ection, controll
-00001d60: 6162 6c65 3a20 436f 6e74 726f 6c6c 6162  able: Controllab
-00001d70: 6c65 2920 2d3e 2062 6f6f 6c3a 0d0a 2020  le) -> bool:..  
-00001d80: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00001d90: 6520 2320 746f 646f 2063 6865 636b 0d0a  e # todo check..
-00001da0: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-00001db0: 0a20 2020 2064 6566 2063 6f6e 7472 6f6c  .    def control
-00001dc0: 6c61 626c 6528 7365 6c66 2920 2d3e 2043  lable(self) -> C
-00001dd0: 6f6e 7472 6f6c 6c61 626c 653a 0d0a 2020  ontrollable:..  
-00001de0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00001df0: 662e 5f5f 636f 6e74 726f 6c6c 6162 6c65  f.__controllable
-00001e00: 0d0a 0d0a 2020 2020 6465 6620 636f 7079  ....    def copy
-00001e10: 2873 656c 6629 202d 3e20 2254 696c 6522  (self) -> "Tile"
-00001e20: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00001e30: 6e20 436f 6e74 726f 6c6c 6162 6c65 5469  n ControllableTi
-00001e40: 6c65 2873 656c 662e 5f5f 636f 6e74 726f  le(self.__contro
-00001e50: 6c6c 6162 6c65 290d 0a0d 0a0d 0a63 6c61  llable)......cla
-00001e60: 7373 204e 7063 5469 6c65 2854 696c 6529  ss NpcTile(Tile)
-00001e70: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
-00001e80: 745f 5f28 7365 6c66 2c20 6e61 6d65 3a20  t__(self, name: 
-00001e90: 7374 722c 2073 686f 775f 6d65 7373 6167  str, show_messag
-00001ea0: 655f 6361 6c6c 6261 636b 3a20 4361 6c6c  e_callback: Call
-00001eb0: 6162 6c65 5b5b 7374 722c 2073 7472 5d2c  able[[str, str],
-00001ec0: 204e 6f6e 655d 2c0d 0a20 2020 2020 2020   None],..       
-00001ed0: 2020 2020 2020 2020 2020 6765 745f 7465            get_te
-00001ee0: 7874 5f63 616c 6c62 6163 6b3a 2043 616c  xt_callback: Cal
-00001ef0: 6c61 626c 655b 5b5d 2c20 7374 725d 293a  lable[[], str]):
-00001f00: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-00001f10: 4e70 6354 696c 652c 2073 656c 6629 2e5f  NpcTile, self)._
-00001f20: 5f69 6e69 745f 5f28 5469 6c65 436f 6465  _init__(TileCode
-00001f30: 2e4e 7063 290d 0a20 2020 2020 2020 2073  .Npc)..        s
-00001f40: 656c 662e 5f5f 6e61 6d65 203d 206e 616d  elf.__name = nam
-00001f50: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00001f60: 5f5f 7368 6f77 5f6d 6573 7361 6765 203d  __show_message =
-00001f70: 2073 686f 775f 6d65 7373 6167 655f 6361   show_message_ca
-00001f80: 6c6c 6261 636b 0d0a 2020 2020 2020 2020  llback..        
-00001f90: 7365 6c66 2e5f 5f67 6574 5f74 6578 7420  self.__get_text 
-00001fa0: 3d20 6765 745f 7465 7874 5f63 616c 6c62  = get_text_callb
-00001fb0: 6163 6b0d 0a0d 0a20 2020 2040 7072 6f70  ack....    @prop
-00001fc0: 6572 7479 0d0a 2020 2020 6465 6620 6461  erty..    def da
-00001fd0: 7461 2873 656c 6629 202d 3e20 7374 723a  ta(self) -> str:
-00001fe0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001ff0: 2073 656c 662e 5f5f 6e61 6d65 0d0a 0d0a   self.__name....
-00002000: 2020 2020 6465 6620 6765 745f 696d 6728      def get_img(
-00002010: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00002020: 7265 7475 726e 2073 656c 662e 5f5f 6e61  return self.__na
-00002030: 6d65 5b30 5d0d 0a0d 0a20 2020 2064 6566  me[0]....    def
-00002040: 2069 735f 7761 6c6b 6162 6c65 2873 656c   is_walkable(sel
-00002050: 662c 2064 6972 6563 7469 6f6e 3a20 4469  f, direction: Di
-00002060: 7265 6374 696f 6e2c 2063 6f6e 7472 6f6c  rection, control
-00002070: 6c61 626c 653a 2043 6f6e 7472 6f6c 6c61  lable: Controlla
-00002080: 626c 6529 202d 3e20 626f 6f6c 3a0d 0a20  ble) -> bool:.. 
-00002090: 2020 2020 2020 2073 656c 662e 5f5f 7368         self.__sh
-000020a0: 6f77 5f6d 6573 7361 6765 2873 656c 662e  ow_message(self.
-000020b0: 5f5f 6e61 6d65 2c20 7365 6c66 2e5f 5f67  __name, self.__g
-000020c0: 6574 5f74 6578 7428 2929 0d0a 2020 2020  et_text())..    
-000020d0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000020e0: 0d0a 0d0a 2020 2020 6465 6620 636f 7079  ....    def copy
-000020f0: 2873 656c 6629 202d 3e20 2254 696c 6522  (self) -> "Tile"
-00002100: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00002110: 6e20 4e70 6354 696c 6528 7365 6c66 2e5f  n NpcTile(self._
-00002120: 5f6e 616d 652c 2073 656c 662e 5f5f 7368  _name, self.__sh
-00002130: 6f77 5f6d 6573 7361 6765 2c20 7365 6c66  ow_message, self
-00002140: 2e5f 5f67 6574 5f74 6578 7429 0d0a       .__get_text)..
+00000330: 2020 2047 6f61 6c20 3d20 2836 312c 2022     Goal = (61, "
+00000340: 4722 2920 2020 2020 2020 2020 2020 2023  G")            #
+00000350: 2074 696c 6520 666f 7220 7468 6520 676f   tile for the go
+00000360: 616c 2c20 692e 652e 2065 6e64 206f 6620  al, i.e. end of 
+00000370: 6120 6c65 7665 6c0d 0a20 2020 2054 7269  a level..    Tri
+00000380: 6767 6572 203d 2028 392c 2022 5422 2920  gger = (9, "T") 
+00000390: 2020 2020 2020 2020 2320 7469 6c65 2074          # tile t
+000003a0: 6861 7420 6361 6c6c 7320 6120 6675 6e63  hat calls a func
+000003b0: 7469 6f6e 206f 6e20 7761 6c6b 2c20 692e  tion on walk, i.
+000003c0: 652e 2065 7665 6e74 2074 696c 650d 0a20  e. event tile.. 
+000003d0: 2020 2054 656c 6570 6f72 7420 3d20 2839     Teleport = (9
+000003e0: 312c 2022 7422 2920 2020 2020 2020 2320  1, "t")       # 
+000003f0: 7370 6563 6961 6c20 7472 6967 6765 7220  special trigger 
+00000400: 666f 7220 7465 6c65 706f 7274 696e 6720  for teleporting 
+00000410: 6265 7477 6565 6e20 6d61 7073 0d0a 2020  between maps..  
+00000420: 2020 4465 636f 7261 7469 6f6e 203d 2028    Decoration = (
+00000430: 3131 2c20 2264 2229 2020 2020 2023 2073  11, "d")     # s
+00000440: 696d 706c 7920 6469 7370 6c61 7973 2061  imply displays a
+00000450: 2073 7065 6369 6669 6564 2063 6861 7261   specified chara
+00000460: 6374 6572 0d0a 0d0a 2020 2020 5761 6c6c  cter....    Wall
+00000470: 203d 2028 312c 2022 2322 290d 0a20 2020   = (1, "#")..   
+00000480: 204f 6273 7461 636c 6520 3d20 2832 2c20   Obstacle = (2, 
+00000490: 226f 2229 0d0a 2020 2020 446f 6f72 203d  "o")..    Door =
+000004a0: 2028 342c 2022 7c22 290d 0a0d 0a20 2020   (4, "|")....   
+000004b0: 2043 6f6e 7472 6f6c 6c61 626c 6520 3d20   Controllable = 
+000004c0: 2832 302c 2022 4322 290d 0a20 2020 204e  (20, "C")..    N
+000004d0: 7063 203d 2028 3235 2c20 224e 2229 0d0a  pc = (25, "N")..
+000004e0: 2020 2020 456e 656d 7920 3d20 2833 302c      Enemy = (30,
+000004f0: 2022 4522 290d 0a20 2020 2042 6f73 7320   "E")..    Boss 
+00000500: 3d20 2834 302c 2022 4222 290d 0a0d 0a20  = (40, "B").... 
+00000510: 2020 2043 6f6c 6c65 6374 6962 6c65 203d     Collectible =
+00000520: 2028 3530 2c20 2263 2229 0d0a 2020 2020   (50, "c")..    
+00000530: 5269 6464 6c65 7220 3d20 2835 312c 2022  Riddler = (51, "
+00000540: 3f22 290d 0a20 2020 2053 686f 704b 6565  ?")..    ShopKee
+00000550: 7065 7220 3d20 2835 322c 2022 2422 290d  per = (52, "$").
+00000560: 0a20 2020 2045 6e65 7267 7920 3d20 2835  .    Energy = (5
+00000570: 332c 2022 6522 290d 0a20 2020 2043 6861  3, "e")..    Cha
+00000580: 6c6c 656e 6765 7220 3d20 2835 342c 2022  llenger = (54, "
+00000590: 2122 290d 0a0d 0a20 2020 2053 7061 6365  !")....    Space
+000005a0: 7368 6970 426c 6f63 6b20 3d20 2837 302c  shipBlock = (70,
+000005b0: 2022 2f22 290d 0a20 2020 2053 7061 6365   "/")..    Space
+000005c0: 7368 6970 5761 6c6b 203d 2028 3731 2c20  shipWalk = (71, 
+000005d0: 222e 2229 0d0a 2020 2020 5370 6163 6573  ".")..    Spaces
+000005e0: 6869 7054 7269 6767 6572 203d 2028 3732  hipTrigger = (72
+000005f0: 2c20 2254 2229 0d0a 2020 2020 4f75 7465  , "T")..    Oute
+00000600: 7253 7061 6365 203d 2028 3733 2c20 222a  rSpace = (73, "*
+00000610: 2229 0d0a 0d0a 2020 2020 436f 6c6c 6563  ")....    Collec
+00000620: 7469 626c 654b 6579 203d 2028 3530 312c  tibleKey = (501,
+00000630: 2022 6b22 290d 0a20 2020 2043 6f6c 6c65   "k")..    Colle
+00000640: 6374 6962 6c65 436f 696e 203d 2028 3530  ctibleCoin = (50
+00000650: 322c 2022 e282 ac22 290d 0a20 2020 2043  2, "...")..    C
+00000660: 6f6c 6c65 6374 6962 6c65 456e 6572 6779  ollectibleEnergy
+00000670: 203d 2028 3530 332c 2022 6522 290d 0a20   = (503, "e").. 
+00000680: 2020 2043 6f6c 6c65 6374 6962 6c65 4761     CollectibleGa
+00000690: 7465 203d 2028 3532 302c 2022 6722 290d  te = (520, "g").
+000006a0: 0a20 2020 2043 6f6c 6c65 6374 6962 6c65  .    Collectible
+000006b0: 5175 6269 7420 3d20 2835 3630 2c20 2271  Qubit = (560, "q
+000006c0: 2229 0d0a 0d0a 2020 2020 6465 6620 5f5f  ")....    def __
+000006d0: 696e 6974 5f5f 2873 656c 662c 2069 643a  init__(self, id:
+000006e0: 2069 6e74 2c20 7265 7072 6573 656e 7461   int, representa
+000006f0: 7469 6f6e 3a20 7374 7229 3a0d 0a20 2020  tion: str):..   
+00000700: 2020 2020 2073 656c 662e 5f5f 6964 203d       self.__id =
+00000710: 2069 640d 0a20 2020 2020 2020 2073 656c   id..        sel
+00000720: 662e 5f5f 7265 7072 6573 656e 7461 7469  f.__representati
+00000730: 6f6e 203d 2072 6570 7265 7365 6e74 6174  on = representat
+00000740: 696f 6e0d 0a0d 0a20 2020 2040 7072 6f70  ion....    @prop
+00000750: 6572 7479 0d0a 2020 2020 6465 6620 6964  erty..    def id
+00000760: 2873 656c 6629 202d 3e20 696e 743a 0d0a  (self) -> int:..
+00000770: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00000780: 656c 662e 5f5f 6964 0d0a 0d0a 2020 2020  elf.__id....    
+00000790: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+000007a0: 6566 2072 6570 7265 7365 6e74 6174 696f  ef representatio
+000007b0: 6e28 7365 6c66 2920 2d3e 2073 7472 3a0d  n(self) -> str:.
+000007c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000007d0: 7365 6c66 2e5f 5f72 6570 7265 7365 6e74  self.__represent
+000007e0: 6174 696f 6e0d 0a0d 0a20 2020 2064 6566  ation....    def
+000007f0: 205f 5f73 7472 5f5f 2873 656c 6629 3a0d   __str__(self):.
+00000800: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000810: 7365 6c66 2e72 6570 7265 7365 6e74 6174  self.representat
+00000820: 696f 6e0d 0a0d 0a20 2020 2040 7374 6174  ion....    @stat
+00000830: 6963 6d65 7468 6f64 0d0a 2020 2020 6465  icmethod..    de
+00000840: 6620 7370 6563 6961 6c5f 7661 6c75 6573  f special_values
+00000850: 2829 202d 3e20 4c69 7374 5b22 5469 6c65  () -> List["Tile
+00000860: 436f 6465 225d 3a0d 0a20 2020 2020 2020  Code"]:..       
+00000870: 2072 6574 7572 6e20 5b0d 0a20 2020 2020   return [..     
+00000880: 2020 2020 2020 2054 696c 6543 6f64 652e         TileCode.
+00000890: 496e 7661 6c69 642c 2054 696c 6543 6f64  Invalid, TileCod
+000008a0: 652e 4465 6275 672c 2054 696c 6543 6f64  e.Debug, TileCod
+000008b0: 652e 566f 6964 2c20 5469 6c65 436f 6465  e.Void, TileCode
+000008c0: 2e46 6f67 4f66 5761 722c 0d0a 2020 2020  .FogOfWar,..    
+000008d0: 2020 2020 2020 2020 5469 6c65 436f 6465          TileCode
+000008e0: 2e4d 6573 7361 6765 2c20 5469 6c65 436f  .Message, TileCo
+000008f0: 6465 2e54 7269 6767 6572 2c20 5469 6c65  de.Trigger, Tile
+00000900: 436f 6465 2e54 656c 6570 6f72 742c 2054  Code.Teleport, T
+00000910: 696c 6543 6f64 652e 4465 636f 7261 7469  ileCode.Decorati
+00000920: 6f6e 2c0d 0a20 2020 2020 2020 205d 0d0a  on,..        ]..
+00000930: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00000940: 686f 640d 0a20 2020 2064 6566 2063 6f6c  hod..    def col
+00000950: 6c65 6374 6962 6c65 5f73 7562 7479 7065  lectible_subtype
+00000960: 7328 2920 2d3e 204c 6973 745b 2254 696c  s() -> List["Til
+00000970: 6543 6f64 6522 5d3a 0d0a 2020 2020 2020  eCode"]:..      
+00000980: 2020 7265 7475 726e 205b 0d0a 2020 2020    return [..    
+00000990: 2020 2020 2020 2020 5469 6c65 436f 6465          TileCode
+000009a0: 2e43 6f6c 6c65 6374 6962 6c65 2c0d 0a20  .Collectible,.. 
+000009b0: 2020 2020 2020 2020 2020 2054 696c 6543             TileC
+000009c0: 6f64 652e 436f 6c6c 6563 7469 626c 654b  ode.CollectibleK
+000009d0: 6579 2c20 5469 6c65 436f 6465 2e43 6f6c  ey, TileCode.Col
+000009e0: 6c65 6374 6962 6c65 436f 696e 2c20 5469  lectibleCoin, Ti
+000009f0: 6c65 436f 6465 2e43 6f6c 6c65 6374 6962  leCode.Collectib
+00000a00: 6c65 456e 6572 6779 2c0d 0a20 2020 2020  leEnergy,..     
+00000a10: 2020 2020 2020 2054 696c 6543 6f64 652e         TileCode.
+00000a20: 436f 6c6c 6563 7469 626c 6547 6174 652c  CollectibleGate,
+00000a30: 2054 696c 6543 6f64 652e 436f 6c6c 6563   TileCode.Collec
+00000a40: 7469 626c 6551 7562 6974 2c0d 0a20 2020  tibleQubit,..   
+00000a50: 2020 2020 205d 0d0a 0d0a 0d0a 636c 6173       ]......clas
+00000a60: 7320 5469 6c65 2841 4243 293a 0d0a 2020  s Tile(ABC):..  
+00000a70: 2020 4073 7461 7469 636d 6574 686f 640d    @staticmethod.
+00000a80: 0a20 2020 2064 6566 205f 696e 7669 7369  .    def _invisi
+00000a90: 626c 655f 7469 6c65 2829 3a0d 0a20 2020  ble_tile():..   
+00000aa0: 2020 2020 2072 6574 7572 6e20 2220 220d       return " ".
+00000ab0: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
+00000ac0: 745f 5f28 7365 6c66 2c20 636f 6465 3a20  t__(self, code: 
+00000ad0: 5469 6c65 436f 6465 293a 0d0a 2020 2020  TileCode):..    
+00000ae0: 2020 2020 7365 6c66 2e5f 5f63 6f64 6520      self.__code 
+00000af0: 3d20 636f 6465 0d0a 0d0a 2020 2020 4070  = code....    @p
+00000b00: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00000b10: 2064 6174 6128 7365 6c66 2920 2d3e 204e   data(self) -> N
+00000b20: 6f6e 653a 0d0a 2020 2020 2020 2020 2222  one:..        ""
+00000b30: 220d 0a20 2020 2020 2020 2045 2e67 2e20  "..        E.g. 
+00000b40: 616d 6f75 6e74 2066 6f72 2045 6e65 7267  amount for Energ
+00000b50: 792c 206c 6f67 6963 616c 2043 6f6c 6c65  y, logical Colle
+00000b60: 6374 6962 6c65 2066 6f72 2043 6f6c 6c65  ctible for Colle
+00000b70: 6374 6962 6c65 732c 2065 6964 2066 6f72  ctibles, eid for
+00000b80: 2045 6e65 6d69 6573 206f 7220 4e6f 6e65   Enemies or None
+00000b90: 2066 6f72 2074 696c 6573 2077 6974 686f   for tiles witho
+00000ba0: 7574 2061 6e79 0d0a 2020 2020 2020 2020  ut any..        
+00000bb0: 6479 6e61 6d69 6320 7661 6c75 6573 2028  dynamic values (
+00000bc0: 5761 6c6c 732c 2046 6c6f 6f72 2c20 2e2e  Walls, Floor, ..
+00000bd0: 2e29 0d0a 0d0a 2020 2020 2020 2020 3a72  .)....        :r
+00000be0: 6574 7572 6e3a 2061 2072 6570 7265 7365  eturn: a represe
+00000bf0: 6e74 6174 696f 6e20 6f66 2074 6865 2073  ntation of the s
+00000c00: 7065 6369 6669 6320 7469 6c65 2773 2064  pecific tile's d
+00000c10: 6174 610d 0a20 2020 2020 2020 2022 2222  ata..        """
+00000c20: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000c30: 204e 6f6e 650d 0a0d 0a20 2020 2040 7072   None....    @pr
+00000c40: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
+00000c50: 636f 6465 2873 656c 6629 202d 3e20 5469  code(self) -> Ti
+00000c60: 6c65 436f 6465 3a0d 0a20 2020 2020 2020  leCode:..       
+00000c70: 2072 6574 7572 6e20 7365 6c66 2e5f 5f63   return self.__c
+00000c80: 6f64 650d 0a0d 0a20 2020 2040 7072 6f70  ode....    @prop
+00000c90: 6572 7479 0d0a 2020 2020 6465 6620 5f69  erty..    def _i
+00000ca0: 6e76 6973 6962 6c65 2873 656c 6629 3a0d  nvisible(self):.
+00000cb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000cc0: 5469 6c65 2e5f 696e 7669 7369 626c 655f  Tile._invisible_
+00000cd0: 7469 6c65 2829 0d0a 0d0a 2020 2020 4061  tile()....    @a
+00000ce0: 6273 7472 6163 746d 6574 686f 640d 0a20  bstractmethod.. 
+00000cf0: 2020 2064 6566 2067 6574 5f69 6d67 2873     def get_img(s
+00000d00: 656c 6629 3a0d 0a20 2020 2020 2020 2070  elf):..        p
+00000d10: 6173 730d 0a0d 0a20 2020 2040 6162 7374  ass....    @abst
+00000d20: 7261 6374 6d65 7468 6f64 0d0a 2020 2020  ractmethod..    
+00000d30: 6465 6620 6973 5f77 616c 6b61 626c 6528  def is_walkable(
+00000d40: 7365 6c66 2c20 6469 7265 6374 696f 6e3a  self, direction:
+00000d50: 2044 6972 6563 7469 6f6e 2c20 636f 6e74   Direction, cont
+00000d60: 726f 6c6c 6162 6c65 3a20 436f 6e74 726f  rollable: Contro
+00000d70: 6c6c 6162 6c65 2920 2d3e 2062 6f6f 6c3a  llable) -> bool:
+00000d80: 0d0a 2020 2020 2020 2020 7061 7373 0d0a  ..        pass..
+00000d90: 0d0a 2020 2020 4061 6273 7472 6163 746d  ..    @abstractm
+00000da0: 6574 686f 640d 0a20 2020 2064 6566 2063  ethod..    def c
+00000db0: 6f70 7928 7365 6c66 2920 2d3e 2022 5469  opy(self) -> "Ti
+00000dc0: 6c65 223a 0d0a 2020 2020 2020 2020 7061  le":..        pa
+00000dd0: 7373 0d0a 0d0a 2020 2020 6465 6620 5f5f  ss....    def __
+00000de0: 7374 725f 5f28 7365 6c66 293a 0d0a 2020  str__(self):..  
+00000df0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00000e00: 662e 6765 745f 696d 6728 290d 0a0d 0a0d  f.get_img().....
+00000e10: 0a63 6c61 7373 2049 6e76 616c 6964 2854  .class Invalid(T
+00000e20: 696c 6529 3a0d 0a20 2020 2064 6566 205f  ile):..    def _
+00000e30: 5f69 6e69 745f 5f28 7365 6c66 293a 0d0a  _init__(self):..
+00000e40: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00000e50: 5f5f 696e 6974 5f5f 2854 696c 6543 6f64  __init__(TileCod
+00000e60: 652e 496e 7661 6c69 6429 0d0a 0d0a 2020  e.Invalid)....  
+00000e70: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00000e80: 2064 6566 2064 6174 6128 7365 6c66 2920   def data(self) 
+00000e90: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
+00000ea0: 2020 7265 7475 726e 204e 6f6e 650d 0a0d    return None...
+00000eb0: 0a20 2020 2064 6566 2067 6574 5f69 6d67  .    def get_img
+00000ec0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00000ed0: 2072 6574 7572 6e20 5469 6c65 436f 6465   return TileCode
+00000ee0: 2e49 6e76 616c 6964 2e72 6570 7265 7365  .Invalid.represe
+00000ef0: 6e74 6174 696f 6e0d 0a0d 0a20 2020 2064  ntation....    d
+00000f00: 6566 2069 735f 7761 6c6b 6162 6c65 2873  ef is_walkable(s
+00000f10: 656c 662c 2064 6972 6563 7469 6f6e 3a20  elf, direction: 
+00000f20: 4469 7265 6374 696f 6e2c 2063 6f6e 7472  Direction, contr
+00000f30: 6f6c 6c61 626c 653a 2043 6f6e 7472 6f6c  ollable: Control
+00000f40: 6c61 626c 6529 202d 3e20 626f 6f6c 3a0d  lable) -> bool:.
+00000f50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000f60: 4661 6c73 650d 0a0d 0a20 2020 2064 6566  False....    def
+00000f70: 2063 6f70 7928 7365 6c66 2920 2d3e 2022   copy(self) -> "
+00000f80: 5469 6c65 223a 0d0a 2020 2020 2020 2020  Tile":..        
+00000f90: 7265 7475 726e 2049 6e76 616c 6964 2829  return Invalid()
+00000fa0: 0d0a 0d0a 0d0a 636c 6173 7320 4465 6275  ......class Debu
+00000fb0: 6728 5469 6c65 293a 0d0a 2020 2020 6465  g(Tile):..    de
+00000fc0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00000fd0: 206e 756d 3a20 696e 7429 3a0d 0a20 2020   num: int):..   
+00000fe0: 2020 2020 2073 7570 6572 2844 6562 7567       super(Debug
+00000ff0: 2c20 7365 6c66 292e 5f5f 696e 6974 5f5f  , self).__init__
+00001000: 2854 696c 6543 6f64 652e 4465 6275 6729  (TileCode.Debug)
+00001010: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00001020: 5f6e 756d 203d 2073 7472 286e 756d 295b  _num = str(num)[
+00001030: 305d 0d0a 0d0a 2020 2020 4070 726f 7065  0]....    @prope
+00001040: 7274 790d 0a20 2020 2064 6566 2064 6174  rty..    def dat
+00001050: 6128 7365 6c66 2920 2d3e 2069 6e74 3a0d  a(self) -> int:.
+00001060: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001070: 7365 6c66 2e5f 5f6e 756d 0d0a 0d0a 2020  self.__num....  
+00001080: 2020 6465 6620 6765 745f 696d 6728 7365    def get_img(se
+00001090: 6c66 2920 2d3e 2073 7472 3a0d 0a20 2020  lf) -> str:..   
+000010a0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000010b0: 2e5f 5f6e 756d 0d0a 0d0a 2020 2020 6465  .__num....    de
+000010c0: 6620 6973 5f77 616c 6b61 626c 6528 7365  f is_walkable(se
+000010d0: 6c66 2c20 6469 7265 6374 696f 6e3a 2044  lf, direction: D
+000010e0: 6972 6563 7469 6f6e 2c20 636f 6e74 726f  irection, contro
+000010f0: 6c6c 6162 6c65 3a20 436f 6e74 726f 6c6c  llable: Controll
+00001100: 6162 6c65 2920 2d3e 2062 6f6f 6c3a 0d0a  able) -> bool:..
+00001110: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00001120: 616c 7365 0d0a 0d0a 2020 2020 6465 6620  alse....    def 
+00001130: 636f 7079 2873 656c 6629 202d 3e20 2254  copy(self) -> "T
+00001140: 696c 6522 3a0d 0a20 2020 2020 2020 2072  ile":..        r
+00001150: 6574 7572 6e20 4465 6275 6728 696e 7428  eturn Debug(int(
+00001160: 7365 6c66 2e5f 5f6e 756d 2929 0d0a 0d0a  self.__num))....
+00001170: 0d0a 636c 6173 7320 566f 6964 2854 696c  ..class Void(Til
+00001180: 6529 3a0d 0a20 2020 2064 6566 205f 5f69  e):..    def __i
+00001190: 6e69 745f 5f28 7365 6c66 293a 0d0a 2020  nit__(self):..  
+000011a0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+000011b0: 696e 6974 5f5f 2854 696c 6543 6f64 652e  init__(TileCode.
+000011c0: 466c 6f6f 7229 0d0a 0d0a 2020 2020 4070  Floor)....    @p
+000011d0: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+000011e0: 2064 6174 6128 7365 6c66 2920 2d3e 204e   data(self) -> N
+000011f0: 6f6e 653a 0d0a 2020 2020 2020 2020 7265  one:..        re
+00001200: 7475 726e 204e 6f6e 650d 0a0d 0a20 2020  turn None....   
+00001210: 2064 6566 2067 6574 5f69 6d67 2873 656c   def get_img(sel
+00001220: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
+00001230: 7572 6e20 7365 6c66 2e5f 696e 7669 7369  urn self._invisi
+00001240: 626c 650d 0a0d 0a20 2020 2064 6566 2069  ble....    def i
+00001250: 735f 7761 6c6b 6162 6c65 2873 656c 662c  s_walkable(self,
+00001260: 2064 6972 6563 7469 6f6e 3a20 4469 7265   direction: Dire
+00001270: 6374 696f 6e2c 2063 6f6e 7472 6f6c 6c61  ction, controlla
+00001280: 626c 653a 2043 6f6e 7472 6f6c 6c61 626c  ble: Controllabl
+00001290: 6529 202d 3e20 626f 6f6c 3a0d 0a20 2020  e) -> bool:..   
+000012a0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+000012b0: 650d 0a0d 0a20 2020 2064 6566 2063 6f70  e....    def cop
+000012c0: 7928 7365 6c66 2920 2d3e 2022 5469 6c65  y(self) -> "Tile
+000012d0: 223a 0d0a 2020 2020 2020 2020 7265 7475  ":..        retu
+000012e0: 726e 2056 6f69 6428 290d 0a0d 0a0d 0a63  rn Void()......c
+000012f0: 6c61 7373 2046 6c6f 6f72 2854 696c 6529  lass Floor(Tile)
+00001300: 3a0d 0a20 2020 2040 7374 6174 6963 6d65  :..    @staticme
+00001310: 7468 6f64 0d0a 2020 2020 6465 6620 696d  thod..    def im
+00001320: 6728 293a 0d0a 2020 2020 2020 2020 7265  g():..        re
+00001330: 7475 726e 2054 696c 652e 5f69 6e76 6973  turn Tile._invis
+00001340: 6962 6c65 5f74 696c 6528 290d 0a0d 0a20  ible_tile().... 
+00001350: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00001360: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00001370: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00001380: 2854 696c 6543 6f64 652e 466c 6f6f 7229  (TileCode.Floor)
+00001390: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
+000013a0: 790d 0a20 2020 2064 6566 2064 6174 6128  y..    def data(
+000013b0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0d0a  self) -> None:..
+000013c0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+000013d0: 6f6e 650d 0a0d 0a20 2020 2064 6566 2067  one....    def g
+000013e0: 6574 5f69 6d67 2873 656c 6629 3a0d 0a20  et_img(self):.. 
+000013f0: 2020 2020 2020 2072 6574 7572 6e20 466c         return Fl
+00001400: 6f6f 722e 696d 6728 290d 0a0d 0a20 2020  oor.img()....   
+00001410: 2064 6566 2069 735f 7761 6c6b 6162 6c65   def is_walkable
+00001420: 2873 656c 662c 2064 6972 6563 7469 6f6e  (self, direction
+00001430: 3a20 4469 7265 6374 696f 6e2c 2063 6f6e  : Direction, con
+00001440: 7472 6f6c 6c61 626c 653a 2043 6f6e 7472  trollable: Contr
+00001450: 6f6c 6c61 626c 6529 202d 3e20 626f 6f6c  ollable) -> bool
+00001460: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+00001470: 6e20 5472 7565 0d0a 0d0a 2020 2020 6465  n True....    de
+00001480: 6620 636f 7079 2873 656c 6629 202d 3e20  f copy(self) -> 
+00001490: 2254 696c 6522 3a0d 0a20 2020 2020 2020  "Tile":..       
+000014a0: 2072 6574 7572 6e20 466c 6f6f 7228 290d   return Floor().
+000014b0: 0a0d 0a0d 0a63 6c61 7373 2057 616c 6c28  .....class Wall(
+000014c0: 5469 6c65 293a 0d0a 2020 2020 4073 7461  Tile):..    @sta
+000014d0: 7469 636d 6574 686f 640d 0a20 2020 2064  ticmethod..    d
+000014e0: 6566 2069 6d67 2829 3a0d 0a20 2020 2020  ef img():..     
+000014f0: 2020 2072 6574 7572 6e20 5469 6c65 436f     return TileCo
+00001500: 6465 2e57 616c 6c2e 7265 7072 6573 656e  de.Wall.represen
+00001510: 7461 7469 6f6e 0d0a 0d0a 2020 2020 6465  tation....    de
+00001520: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
+00001530: 3a0d 0a20 2020 2020 2020 2073 7570 6572  :..        super
+00001540: 2829 2e5f 5f69 6e69 745f 5f28 5469 6c65  ().__init__(Tile
+00001550: 436f 6465 2e57 616c 6c29 0d0a 0d0a 2020  Code.Wall)....  
+00001560: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00001570: 2064 6566 2064 6174 6128 7365 6c66 2920   def data(self) 
+00001580: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
+00001590: 2020 7265 7475 726e 204e 6f6e 650d 0a0d    return None...
+000015a0: 0a20 2020 2064 6566 2067 6574 5f69 6d67  .    def get_img
+000015b0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000015c0: 2072 6574 7572 6e20 5761 6c6c 2e69 6d67   return Wall.img
+000015d0: 2829 0d0a 0d0a 2020 2020 6465 6620 6973  ()....    def is
+000015e0: 5f77 616c 6b61 626c 6528 7365 6c66 2c20  _walkable(self, 
+000015f0: 6469 7265 6374 696f 6e3a 2044 6972 6563  direction: Direc
+00001600: 7469 6f6e 2c20 636f 6e74 726f 6c6c 6162  tion, controllab
+00001610: 6c65 3a20 436f 6e74 726f 6c6c 6162 6c65  le: Controllable
+00001620: 2920 2d3e 2062 6f6f 6c3a 0d0a 2020 2020  ) -> bool:..    
+00001630: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00001640: 0d0a 0d0a 2020 2020 6465 6620 636f 7079  ....    def copy
+00001650: 2873 656c 6629 202d 3e20 2254 696c 6522  (self) -> "Tile"
+00001660: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+00001670: 6e20 5761 6c6c 2829 0d0a 0d0a 0d0a 636c  n Wall()......cl
+00001680: 6173 7320 4f62 7374 6163 6c65 2854 696c  ass Obstacle(Til
+00001690: 6529 3a0d 0a20 2020 2064 6566 205f 5f69  e):..    def __i
+000016a0: 6e69 745f 5f28 7365 6c66 293a 0d0a 2020  nit__(self):..  
+000016b0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+000016c0: 696e 6974 5f5f 2854 696c 6543 6f64 652e  init__(TileCode.
+000016d0: 4f62 7374 6163 6c65 290d 0a0d 0a20 2020  Obstacle)....   
+000016e0: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
+000016f0: 6465 6620 6461 7461 2873 656c 6629 202d  def data(self) -
+00001700: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
+00001710: 2072 6574 7572 6e20 4e6f 6e65 0d0a 0d0a   return None....
+00001720: 2020 2020 6465 6620 6765 745f 696d 6728      def get_img(
+00001730: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00001740: 7265 7475 726e 2054 696c 6543 6f64 652e  return TileCode.
+00001750: 4f62 7374 6163 6c65 2e72 6570 7265 7365  Obstacle.represe
+00001760: 6e74 6174 696f 6e0d 0a0d 0a20 2020 2064  ntation....    d
+00001770: 6566 2069 735f 7761 6c6b 6162 6c65 2873  ef is_walkable(s
+00001780: 656c 662c 2064 6972 6563 7469 6f6e 3a20  elf, direction: 
+00001790: 4469 7265 6374 696f 6e2c 2063 6f6e 7472  Direction, contr
+000017a0: 6f6c 6c61 626c 653a 2043 6f6e 7472 6f6c  ollable: Control
+000017b0: 6c61 626c 6529 202d 3e20 626f 6f6c 3a0d  lable) -> bool:.
+000017c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000017d0: 4661 6c73 6520 6f72 2043 6865 6174 436f  False or CheatCo
+000017e0: 6e66 6967 2e69 676e 6f72 655f 6f62 7374  nfig.ignore_obst
+000017f0: 6163 6c65 7328 290d 0a0d 0a20 2020 2064  acles()....    d
+00001800: 6566 2063 6f70 7928 7365 6c66 2920 2d3e  ef copy(self) ->
+00001810: 2022 5469 6c65 223a 0d0a 2020 2020 2020   "Tile":..      
+00001820: 2020 7265 7475 726e 204f 6273 7461 636c    return Obstacl
+00001830: 6528 290d 0a0d 0a0d 0a63 6c61 7373 2046  e()......class F
+00001840: 6f67 4f66 5761 7228 5469 6c65 293a 0d0a  ogOfWar(Tile):..
+00001850: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00001860: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00001870: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+00001880: 5f28 5469 6c65 436f 6465 2e4f 6273 7461  _(TileCode.Obsta
+00001890: 636c 6529 0d0a 0d0a 2020 2020 4070 726f  cle)....    @pro
+000018a0: 7065 7274 790d 0a20 2020 2064 6566 2064  perty..    def d
+000018b0: 6174 6128 7365 6c66 2920 2d3e 204e 6f6e  ata(self) -> Non
+000018c0: 653a 0d0a 2020 2020 2020 2020 7265 7475  e:..        retu
+000018d0: 726e 204e 6f6e 650d 0a0d 0a20 2020 2064  rn None....    d
+000018e0: 6566 2067 6574 5f69 6d67 2873 656c 6629  ef get_img(self)
+000018f0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+00001900: 6e20 5469 6c65 436f 6465 2e46 6f67 4f66  n TileCode.FogOf
+00001910: 5761 722e 7265 7072 6573 656e 7461 7469  War.representati
+00001920: 6f6e 0d0a 0d0a 2020 2020 6465 6620 6973  on....    def is
+00001930: 5f77 616c 6b61 626c 6528 7365 6c66 2c20  _walkable(self, 
+00001940: 6469 7265 6374 696f 6e3a 2044 6972 6563  direction: Direc
+00001950: 7469 6f6e 2c20 636f 6e74 726f 6c6c 6162  tion, controllab
+00001960: 6c65 3a20 436f 6e74 726f 6c6c 6162 6c65  le: Controllable
+00001970: 2920 2d3e 2062 6f6f 6c3a 0d0a 2020 2020  ) -> bool:..    
+00001980: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
+00001990: 0a0d 0a20 2020 2064 6566 2063 6f70 7928  ...    def copy(
+000019a0: 7365 6c66 2920 2d3e 2022 5469 6c65 223a  self) -> "Tile":
+000019b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000019c0: 2046 6f67 4f66 5761 7228 290d 0a0d 0a0d   FogOfWar().....
+000019d0: 0a63 6c61 7373 2044 6563 6f72 6174 696f  .class Decoratio
+000019e0: 6e28 5469 6c65 293a 0d0a 2020 2020 6465  n(Tile):..    de
+000019f0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00001a00: 2064 6563 6f72 6174 696f 6e3a 2073 7472   decoration: str
+00001a10: 2c20 626c 6f63 6b69 6e67 3a20 626f 6f6c  , blocking: bool
+00001a20: 203d 2046 616c 7365 293a 0d0a 2020 2020   = False):..    
+00001a30: 2020 2020 7375 7065 7228 4465 636f 7261      super(Decora
+00001a40: 7469 6f6e 2c20 7365 6c66 292e 5f5f 696e  tion, self).__in
+00001a50: 6974 5f5f 2854 696c 6543 6f64 652e 4465  it__(TileCode.De
+00001a60: 636f 7261 7469 6f6e 290d 0a20 2020 2020  coration)..     
+00001a70: 2020 2073 656c 662e 5f5f 6465 636f 7261     self.__decora
+00001a80: 7469 6f6e 203d 2064 6563 6f72 6174 696f  tion = decoratio
+00001a90: 6e0d 0a20 2020 2020 2020 2073 656c 662e  n..        self.
+00001aa0: 5f5f 626c 6f63 6b69 6e67 203d 2062 6c6f  __blocking = blo
+00001ab0: 636b 696e 670d 0a0d 0a20 2020 2040 7072  cking....    @pr
+00001ac0: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
+00001ad0: 6461 7461 2873 656c 6629 202d 3e20 626f  data(self) -> bo
+00001ae0: 6f6c 3a0d 0a20 2020 2020 2020 2072 6574  ol:..        ret
+00001af0: 7572 6e20 7365 6c66 2e5f 5f62 6c6f 636b  urn self.__block
+00001b00: 696e 670d 0a0d 0a20 2020 2064 6566 2067  ing....    def g
+00001b10: 6574 5f69 6d67 2873 656c 6629 3a0d 0a20  et_img(self):.. 
+00001b20: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00001b30: 6c66 2e5f 5f64 6563 6f72 6174 696f 6e0d  lf.__decoration.
+00001b40: 0a0d 0a20 2020 2064 6566 2069 735f 7761  ...    def is_wa
+00001b50: 6c6b 6162 6c65 2873 656c 662c 2064 6972  lkable(self, dir
+00001b60: 6563 7469 6f6e 3a20 4469 7265 6374 696f  ection: Directio
+00001b70: 6e2c 2063 6f6e 7472 6f6c 6c61 626c 653a  n, controllable:
+00001b80: 2043 6f6e 7472 6f6c 6c61 626c 6529 202d   Controllable) -
+00001b90: 3e20 626f 6f6c 3a0d 0a20 2020 2020 2020  > bool:..       
+00001ba0: 2072 6574 7572 6e20 6e6f 7420 7365 6c66   return not self
+00001bb0: 2e5f 5f62 6c6f 636b 696e 670d 0a0d 0a20  .__blocking.... 
+00001bc0: 2020 2064 6566 2063 6f70 7928 7365 6c66     def copy(self
+00001bd0: 2920 2d3e 2022 5469 6c65 223a 0d0a 2020  ) -> "Tile":..  
+00001be0: 2020 2020 2020 7265 7475 726e 2044 6563        return Dec
+00001bf0: 6f72 6174 696f 6e28 7365 6c66 2e5f 5f64  oration(self.__d
+00001c00: 6563 6f72 6174 696f 6e2c 2073 656c 662e  ecoration, self.
+00001c10: 5f5f 626c 6f63 6b69 6e67 290d 0a0d 0a0d  __blocking).....
+00001c20: 0a63 6c61 7373 2043 6f6e 7472 6f6c 6c61  .class Controlla
+00001c30: 626c 6554 696c 6528 5469 6c65 293a 0d0a  bleTile(Tile):..
+00001c40: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00001c50: 2873 656c 662c 2063 6f6e 7472 6f6c 6c61  (self, controlla
+00001c60: 626c 653a 2043 6f6e 7472 6f6c 6c61 626c  ble: Controllabl
+00001c70: 6529 3a0d 0a20 2020 2020 2020 2073 7570  e):..        sup
+00001c80: 6572 2829 2e5f 5f69 6e69 745f 5f28 5469  er().__init__(Ti
+00001c90: 6c65 436f 6465 2e43 6f6e 7472 6f6c 6c61  leCode.Controlla
+00001ca0: 626c 6529 0d0a 2020 2020 2020 2020 7365  ble)..        se
+00001cb0: 6c66 2e5f 5f63 6f6e 7472 6f6c 6c61 626c  lf.__controllabl
+00001cc0: 6520 3d20 636f 6e74 726f 6c6c 6162 6c65  e = controllable
+00001cd0: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
+00001ce0: 790d 0a20 2020 2064 6566 2064 6174 6128  y..    def data(
+00001cf0: 7365 6c66 2920 2d3e 2073 7472 3a0d 0a20  self) -> str:.. 
+00001d00: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00001d10: 6c66 2e5f 5f63 6f6e 7472 6f6c 6c61 626c  lf.__controllabl
+00001d20: 652e 6e61 6d65 0d0a 0d0a 2020 2020 6465  e.name....    de
+00001d30: 6620 6765 745f 696d 6728 7365 6c66 293a  f get_img(self):
+00001d40: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001d50: 2073 656c 662e 5f5f 636f 6e74 726f 6c6c   self.__controll
+00001d60: 6162 6c65 2e67 6574 5f69 6d67 2829 0d0a  able.get_img()..
+00001d70: 0d0a 2020 2020 6465 6620 6973 5f77 616c  ..    def is_wal
+00001d80: 6b61 626c 6528 7365 6c66 2c20 6469 7265  kable(self, dire
+00001d90: 6374 696f 6e3a 2044 6972 6563 7469 6f6e  ction: Direction
+00001da0: 2c20 636f 6e74 726f 6c6c 6162 6c65 3a20  , controllable: 
+00001db0: 436f 6e74 726f 6c6c 6162 6c65 2920 2d3e  Controllable) ->
+00001dc0: 2062 6f6f 6c3a 0d0a 2020 2020 2020 2020   bool:..        
+00001dd0: 7265 7475 726e 2054 7275 6520 2320 746f  return True # to
+00001de0: 646f 2063 6865 636b 0d0a 0d0a 2020 2020  do check....    
+00001df0: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00001e00: 6566 2063 6f6e 7472 6f6c 6c61 626c 6528  ef controllable(
+00001e10: 7365 6c66 2920 2d3e 2043 6f6e 7472 6f6c  self) -> Control
+00001e20: 6c61 626c 653a 0d0a 2020 2020 2020 2020  lable:..        
+00001e30: 7265 7475 726e 2073 656c 662e 5f5f 636f  return self.__co
+00001e40: 6e74 726f 6c6c 6162 6c65 0d0a 0d0a 2020  ntrollable....  
+00001e50: 2020 6465 6620 636f 7079 2873 656c 6629    def copy(self)
+00001e60: 202d 3e20 2254 696c 6522 3a0d 0a20 2020   -> "Tile":..   
+00001e70: 2020 2020 2072 6574 7572 6e20 436f 6e74       return Cont
+00001e80: 726f 6c6c 6162 6c65 5469 6c65 2873 656c  rollableTile(sel
+00001e90: 662e 5f5f 636f 6e74 726f 6c6c 6162 6c65  f.__controllable
+00001ea0: 290d 0a0d 0a0d 0a63 6c61 7373 204e 7063  )......class Npc
+00001eb0: 5469 6c65 2854 696c 6529 3a0d 0a20 2020  Tile(Tile):..   
+00001ec0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00001ed0: 6c66 2c20 6e61 6d65 3a20 7374 722c 2073  lf, name: str, s
+00001ee0: 686f 775f 6d65 7373 6167 655f 6361 6c6c  how_message_call
+00001ef0: 6261 636b 3a20 4361 6c6c 6162 6c65 5b5b  back: Callable[[
+00001f00: 7374 722c 2073 7472 5d2c 204e 6f6e 655d  str, str], None]
+00001f10: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001f20: 2020 2020 6765 745f 7465 7874 5f63 616c      get_text_cal
+00001f30: 6c62 6163 6b3a 2043 616c 6c61 626c 655b  lback: Callable[
+00001f40: 5b5d 2c20 7374 725d 293a 0d0a 2020 2020  [], str]):..    
+00001f50: 2020 2020 7375 7065 7228 4e70 6354 696c      super(NpcTil
+00001f60: 652c 2073 656c 6629 2e5f 5f69 6e69 745f  e, self).__init_
+00001f70: 5f28 5469 6c65 436f 6465 2e4e 7063 290d  _(TileCode.Npc).
+00001f80: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
+00001f90: 6e61 6d65 203d 206e 616d 650d 0a20 2020  name = name..   
+00001fa0: 2020 2020 2073 656c 662e 5f5f 7368 6f77       self.__show
+00001fb0: 5f6d 6573 7361 6765 203d 2073 686f 775f  _message = show_
+00001fc0: 6d65 7373 6167 655f 6361 6c6c 6261 636b  message_callback
+00001fd0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00001fe0: 5f67 6574 5f74 6578 7420 3d20 6765 745f  _get_text = get_
+00001ff0: 7465 7874 5f63 616c 6c62 6163 6b0d 0a0d  text_callback...
+00002000: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
+00002010: 2020 2020 6465 6620 6461 7461 2873 656c      def data(sel
+00002020: 6629 202d 3e20 7374 723a 0d0a 2020 2020  f) -> str:..    
+00002030: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00002040: 5f5f 6e61 6d65 0d0a 0d0a 2020 2020 6465  __name....    de
+00002050: 6620 6765 745f 696d 6728 7365 6c66 293a  f get_img(self):
+00002060: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00002070: 2073 656c 662e 5f5f 6e61 6d65 5b30 5d0d   self.__name[0].
+00002080: 0a0d 0a20 2020 2064 6566 2069 735f 7761  ...    def is_wa
+00002090: 6c6b 6162 6c65 2873 656c 662c 2064 6972  lkable(self, dir
+000020a0: 6563 7469 6f6e 3a20 4469 7265 6374 696f  ection: Directio
+000020b0: 6e2c 2063 6f6e 7472 6f6c 6c61 626c 653a  n, controllable:
+000020c0: 2043 6f6e 7472 6f6c 6c61 626c 6529 202d   Controllable) -
+000020d0: 3e20 626f 6f6c 3a0d 0a20 2020 2020 2020  > bool:..       
+000020e0: 2073 656c 662e 5f5f 7368 6f77 5f6d 6573   self.__show_mes
+000020f0: 7361 6765 2873 656c 662e 5f5f 6e61 6d65  sage(self.__name
+00002100: 2c20 7365 6c66 2e5f 5f67 6574 5f74 6578  , self.__get_tex
+00002110: 7428 2929 0d0a 2020 2020 2020 2020 7265  t())..        re
+00002120: 7475 726e 2046 616c 7365 0d0a 0d0a 2020  turn False....  
+00002130: 2020 6465 6620 636f 7079 2873 656c 6629    def copy(self)
+00002140: 202d 3e20 2254 696c 6522 3a0d 0a20 2020   -> "Tile":..   
+00002150: 2020 2020 2072 6574 7572 6e20 4e70 6354       return NpcT
+00002160: 696c 6528 7365 6c66 2e5f 5f6e 616d 652c  ile(self.__name,
+00002170: 2073 656c 662e 5f5f 7368 6f77 5f6d 6573   self.__show_mes
+00002180: 7361 6765 2c20 7365 6c66 2e5f 5f67 6574  sage, self.__get
+00002190: 5f74 6578 7429 0d0a                      _text)..
```

### Comparing `qrogue-0.6.2.1/qrogue/game/world/tiles/walk_trigger_tiles.py` & `qrogue-0.6.3/qrogue/game/world/tiles/walk_trigger_tiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,14 +164,16 @@
         self.__message = message
         if popup_times < 0:
             popup_times = 99999     # display "everytime" the controllable steps on it
         self.__times = popup_times
 
     def get_img(self):
         if self.__times > 0:
+            if self.__message.id == "donemsg":
+                return TileCode.Goal.representation
             return "."
         else:
             return self._invisible
 
     def is_walkable(self, direction: Direction, controllable: Controllable) -> bool:
         return True
```

### Comparing `qrogue-0.6.2.1/qrogue/graphics/popups/multiline_popup.py` & `qrogue-0.6.3/qrogue/graphics/popups/multiline_popup.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/graphics/popups/my_popups.py` & `qrogue-0.6.3/qrogue/graphics/popups/my_popups.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/graphics/rendering/color_rules.py` & `qrogue-0.6.3/qrogue/graphics/rendering/color_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         TileCode.Wall: PyCuiColors.BLACK_ON_WHITE,
         TileCode.Obstacle: PyCuiColors.BLACK_ON_WHITE,
         TileCode.Door: PyCuiColors.CYAN_ON_BLACK,
 
         TileCode.Collectible: PyCuiColors.CYAN_ON_BLACK,
         TileCode.Teleport: PyCuiColors.CYAN_ON_BLACK,
         TileCode.Message: PyCuiColors.CYAN_ON_BLACK,
+        TileCode.Goal: PyCuiColors.GREEN_ON_BLACK,
 
         TileCode.Controllable: PyCuiColors.WHITE_ON_GREEN,
         TileCode.Npc: PyCuiColors.BLUE_ON_BLACK,
         TileCode.Enemy: PyCuiColors.RED_ON_BLACK,
         TileCode.Boss: PyCuiColors.BLACK_ON_RED,
 
         TileCode.SpaceshipWalk: PyCuiColors.BLACK_ON_WHITE,
@@ -62,14 +63,18 @@
                                    'contains', match_type='regex')
 
         # collectibles
         for ct in TileCode.collectible_subtypes():
             widget.add_text_color_rule(ct.representation, TileColorer.get_color(TileCode.Collectible), 'contains',
                                        match_type='regex')
 
+        # goal
+        widget.add_text_color_rule(TileCode.Goal.representation, TileColorer.get_color(TileCode.Goal),
+                                   'contains', match_type='regex')
+
     @staticmethod
     def apply_spaceship_rules(widget: WidgetWrapper):
         widget.add_text_color_rule('\.', TileColorer.get_color(TileCode.SpaceshipWalk), 'contains', match_type='regex')
         widget.add_text_color_rule('M', TileColorer.get_color(TileCode.Controllable), 'contains', match_type='regex')
         widget.add_text_color_rule('R', TileColorer.get_color(TileCode.Npc), 'contains', match_type='regex')
         widget.add_text_color_rule('(B|W|N|G)', TileColorer.get_color(TileCode.SpaceshipWalk), 'contains',
                                    match_type='regex')
```

### Comparing `qrogue-0.6.2.1/qrogue/graphics/rendering/renderer.py` & `qrogue-0.6.3/qrogue/graphics/rendering/renderer.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/graphics/widget_base.py` & `qrogue-0.6.3/qrogue/graphics/widget_base.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/graphics/widgets/__init__.py` & `qrogue-0.6.3/qrogue/graphics/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/graphics/widgets/my_widgets.py` & `qrogue-0.6.3/qrogue/graphics/widgets/my_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -768,15 +768,15 @@
         self.widget.add_key_command(controls.get_keys(Keys.SelectionUp), self._up)
         self.widget.add_key_command(controls.get_keys(Keys.SelectionRight), self._right)
         self.widget.add_key_command(controls.get_keys(Keys.SelectionDown), self._down)
         self.widget.add_key_command(controls.get_keys(Keys.SelectionLeft), self._left)
 
         # sadly cannot use a loop here because of how lambda expressions work the index would be the same for all calls
         # instead we use a list of indices to still be flexible without changing much code
-        indices = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]        # todo: make more pretty?
+        indices = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
         hotkeys = [
             controls.get_keys(Keys.HotKey0),
             controls.get_keys(Keys.HotKey1),
             controls.get_keys(Keys.HotKey2),
             controls.get_keys(Keys.HotKey3),
             controls.get_keys(Keys.HotKey4),
             controls.get_keys(Keys.HotKey5),
```

### Comparing `qrogue-0.6.2.1/qrogue/graphics/widgets/spaceship.py` & `qrogue-0.6.3/qrogue/graphics/widgets/spaceship.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/graphics/widgets/widget_sets.py` & `qrogue-0.6.3/qrogue/graphics/widgets/widget_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -907,14 +907,15 @@
         self.__flee_choice = flee_choice
         self._continue_exploration_callback = continue_exploration_callback
         self._robot: Optional[Robot] = None
         self._target: Optional[Target] = None
         self.__num_of_qubits = -1   # needs to be an illegal value because we definitely want to reposition all
         # dependent widgets for the first usage of this WidgetSet
         self._details_content = None
+        self._block_details_back = False
         self.__in_expedition = False
 
         posy = 0
         posx = 0
         row_span = UIConfig.stv_height(2)   # doesn't matter since we reposition the dependent widgets anyway
         matrix_width = UIConfig.WINDOW_WIDTH - (UIConfig.INPUT_STV_WIDTH + UIConfig.OUTPUT_STV_WIDTH +
                                                 UIConfig.TARGET_STV_WIDTH + 1 * 3)  # + width of the three signs
@@ -1020,26 +1021,27 @@
             self.render()
         self.__circuit.widget.add_key_command(controls.get_keys(Keys.Cancel), cancel_circuit)
 
     def __init_choices(self):
         texts = ["Edit", "Gate Guide"]
         callbacks = [self.__choices_adapt, self.__choices_help]
 
-        # todo: do we need this?
         if self.__in_expedition or Ach.check_unlocks(Unlocks.CircuitReset, self._progress):
             texts.append("Reset")
             callbacks.append(self.__choices_reset)
 
         if self.__in_expedition or Ach.check_unlocks(Unlocks.PuzzleFlee, self._progress):
             texts.append(self.__flee_choice)
             callbacks.append(self._choices_flee)
 
         self._choices.set_data(data=(texts, callbacks))
 
     def __details_back(self):
+        if self._block_details_back: return
+
         Widget.move_focus(self._choices, self)
         self._choices.validate_index()
         self._details.render_reset()
         self.render()
 
     @property
     def _sign_offset(self) -> str:
@@ -1203,27 +1205,28 @@
             Logger.instance().error("Error! Target is not set!", from_pycui=False)
             return False
         self._robot.update_statevector()
         success, reward = self._target.is_reached(self._robot.state_vector)
         self.__update_calculation(success)
         self.render()
         if success:
+            def give_reward_and_continue():
+                if reward is not None: self._robot.give_collectible(reward)
+                self._block_details_back = False    # undo the blocking since the success notification is over
+                self._continue_exploration_callback()
+            self._block_details_back = True
             if reward is None:
                 self._details.set_data(data=(
                     [f"Congratulations, you solved the "
                      f"{ColorConfig.highlight_object('Puzzle')}!"],
-                    [self._continue_exploration_callback]
+                    [give_reward_and_continue]
                 ))
             else:
                 Logger.instance().assertion(isinstance(reward, Collectible),
                                             f"Error! Reward is not a Collectible: {reward}")
-
-                def give_reward_and_continue():
-                    self._robot.give_collectible(reward)
-                    self._continue_exploration_callback()
                 self._details.set_data(data=(
                     [f"Congratulations! Your reward: {ColorConfig.highlight_object(reward.to_string())}"],
                     [give_reward_and_continue]
                 ))
 
             self._details_content = self._DETAILS_INFO_THEN_CHOICES
         else:
```

### Comparing `qrogue-0.6.2.1/qrogue/management/map_management.py` & `qrogue-0.6.3/qrogue/management/map_management.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/management/qrogue_pycui.py` & `qrogue-0.6.3/qrogue/management/qrogue_pycui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 from enum import Enum
+from threading import Thread
 from typing import List, Callable, Optional, Any, Tuple
 
 from py_cui import PyCUI
 from py_cui import popups
 from py_cui.widget_set import WidgetSet
 
 from qrogue.game.logic import StateVector, collectibles
@@ -29,14 +30,17 @@
 from qrogue.util.game_simulator import GameSimulator
 from qrogue.util.key_logger import KeyLogger, OverWorldKeyLogger
 
 from qrogue.management import MapManager, Pausing, SaveData, StoryNarration, TransitionText
 
 
 class QrogueCUI(PyCUI):
+    # how many seconds to wait after starting to mark initialization as complete (relevant for input handling)
+    __INIT_DELAY = 0.1
+
     class _State(Enum):
         Menu = 0
         Pause = 1
         Explore = 2
         Fight = 3
         Shop = 4
         Riddle = 5
@@ -130,14 +134,15 @@
 
             qrogue_cui.start()
             return True
         except FileNotFoundError:
             return False
 
     def __init__(self, seed: int, width: int = UIConfig.WINDOW_WIDTH, height: int = UIConfig.WINDOW_HEIGHT):
+        self.__init_complete = False
         super().__init__(width, height)
         self.set_title(f"Qrogue {Config.version()}")
         self.__controls = Controls(self._handle_key_presses)
         self.__seed = seed
         Logger(seed)
         RandomManager(seed)
         OverWorldKeyLogger().reinit(seed, "meta")
@@ -307,14 +312,24 @@
                 self._stdscr.refresh()
 
             # since _draw is only called once, we have to set the timeout manually for the screen
             self._stdscr.timeout(self._refresh_timeout)
 
     def start(self):
         self.__render([self.__cur_widget_set])
+
+        # We don't want to handle accidental input on startup of the game (e.g., during play-testing this once closed
+        # the introduction popup before it even was visible to the player) so we set our init_complete-flag to True
+        # after a short delay. Needs to be in an extra thread so _handle_key_presses() can try to handle the accidental
+        # input. Otherwise, the input queue would not be cleared and the problem only delayed.
+        def call_me():
+            time.sleep(QrogueCUI.__INIT_DELAY)
+            self.__init_complete = True
+        Thread(target=call_me).start()
+
         super(QrogueCUI, self).start()
 
     def __choose_simulation(self):
         title = f"Enter the path to the {FileTypes.KeyLog.value}-file to simulate:"
         self.__show_input_popup(title, PyCuiColors.WHITE_ON_CYAN, self.__start_simulation)
 
     def __start_simulation(self, path: str):
@@ -353,14 +368,17 @@
         now_time = time.time()
         if now_time - self.__last_input >= pause:
             self.__last_input = now_time
             return True
         return False
 
     def _handle_key_presses(self, key_pressed):
+        # ignore all input before we completed initialization
+        if not self.__init_complete: return
+
         if key_pressed == 0:    # skips the "empty" key press during initialization
             return
         if key_pressed == PyCuiConfig.KEY_CTRL_Q:
             super(QrogueCUI, self)._handle_key_presses(PyCuiConfig.KEY_ESCAPE)
         if self.__simulator is None:
             if self._ready_for_input(key_pressed, gameplay=True):
                 if key_pressed == PyCuiConfig.KEY_ESCAPE:
```

### Comparing `qrogue-0.6.2.1/qrogue/management/save_data.py` & `qrogue-0.6.3/qrogue/management/save_data.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/management/story.py` & `qrogue-0.6.3/qrogue/management/story.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/qrogue.py` & `qrogue-0.6.3/qrogue/qrogue.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/util/achievements.py` & `qrogue-0.6.3/qrogue/util/achievements.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             # from now on we can choose with which level we want to to continue
             return progress > Ach.__EXAM_DONE_PROGRESS + 1
 
         elif unlock is Unlocks.ShowEnergy:
             return progress > 0     # Lesson 0 completed
 
         elif unlock is Unlocks.GateRemove:
-            return progress >= 4    # we are at least in Lesson 4
+            return True     # unlock from the beginning to avoid confusion and complicated implicit removal (via cancel)
         elif unlock is Unlocks.CircuitReset:
             return progress >= MapConfig.num_of_lessons()    # all lessons completed
         elif unlock is Unlocks.PuzzleFlee:
             return progress >= MapConfig.num_of_lessons()
 
         elif unlock is Unlocks.ProceedChoice:
             # instead of automatically proceeding to the next level we now have a choice
```

### Comparing `qrogue-0.6.2.1/qrogue/util/common_messages.py` & `qrogue-0.6.3/qrogue/util/common_messages.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/util/config/config.py` & `qrogue-0.6.3/qrogue/util/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from qrogue.util.config import CheatConfig, GameplayConfig, PathConfig, TestConfig
 
 
 class Config:   # todo make singleton and handle access to other configs?
     __frame_count = 0
     MAX_SEED = 1000000
-    __VERSION = "v0.6.2.1"
+    __VERSION = "v0.6.3"
     __GAME_CONFIG = "qrogue_game.config"
     __GAMEPLAY_HEAD = "[Gameplay]\n"
     __DEBUG = False
     __TEST_LEVEL = False
 
     __HEADER = "Qrogue "
     __SEED_HEAD = "Seed="
```

### Comparing `qrogue-0.6.2.1/qrogue/util/config/gameplay_config.py` & `qrogue-0.6.3/qrogue/util/config/gameplay_config.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/util/config/path_config.py` & `qrogue-0.6.3/qrogue/util/config/path_config.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/util/config/py_cui_config.py` & `qrogue-0.6.3/qrogue/util/config/py_cui_config.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/util/config/test_config.py` & `qrogue-0.6.3/qrogue/util/config/test_config.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/util/config/visual_config.py` & `qrogue-0.6.3/qrogue/util/config/visual_config.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/util/controls.py` & `qrogue-0.6.3/qrogue/util/controls.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/util/game_simulator.py` & `qrogue-0.6.3/qrogue/util/game_simulator.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/util/help_texts.py` & `qrogue-0.6.3/qrogue/util/help_texts.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 
         HelpTextType.Pause:
             "In the Pause Menu you can do several things:\n"
             f"{_HL.continue_} - Leave the Pause Menu and continue where you stopped.\n"
             f"{_HL.help_} - If you ever feel stuck and don't remember how certain stuff in the game works select "
             f"this menu and we will try to help you.\n"
             f"{_HL.options} - Configure some Options of the game, like font size or coloring.\n"
-            f"{_HL.exit_} - Exit the current Level or Expedition and return to the Spaceship.\n",
+            f"{_HL.exit_} - Exit the current Level or Expedition .\n",
 
         HelpTextType.Options:
             "",
 
     }
 
     @staticmethod
```

### Comparing `qrogue-0.6.2.1/qrogue/util/key_logger.py` & `qrogue-0.6.3/qrogue/util/key_logger.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/util/logger.py` & `qrogue-0.6.3/qrogue/util/logger.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/util/my_random.py` & `qrogue-0.6.3/qrogue/util/my_random.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue/util/util_functions.py` & `qrogue-0.6.3/qrogue/util/util_functions.py`

 * *Files identical despite different names*

### Comparing `qrogue-0.6.2.1/qrogue.egg-info/SOURCES.txt` & `qrogue-0.6.3/qrogue.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+License.md
 MANIFEST.in
 Readme.md
 setup.py
 qrogue/__init__.py
 qrogue/qrogue.py
 qrogue.egg-info/PKG-INFO
 qrogue.egg-info/SOURCES.txt
```

### Comparing `qrogue-0.6.2.1/setup.py` & `qrogue-0.6.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,32 +22,31 @@
 		'qrogue.game.world',
 		'qrogue.game.world.navigation',
 		'qrogue.game.world.tiles',
 		'qrogue.game.world.map',
 		'qrogue.game.world.dungeon_generator',
 		'qrogue.game.world.dungeon_generator.dungeon_parser',
 		'qrogue.game.world.dungeon_generator.world_parser',
-		'qrogue.game.world.dungeon_generator.wave_function_collapse',
 		'qrogue.graphics',
 		'qrogue.graphics.rendering',
 		'qrogue.graphics.popups',
 		'qrogue.graphics.widgets',
 		'qrogue.management',
 	],
 	package_data={"data": ["qrogue/data"]},
 	include_package_data=True,
-	version='0.6.2.1',
+	version='0.6.3',
 	license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
 	description='Qrogue is a modernized Quantum Computing take of the classical game Rogue.',
 	long_description=README,
 	long_description_content_type="text/markdown",
 	author='Michael Artner',
 	author_email='michael.artner@jku.at',
 	url='https://github.com/7Magic7Mike7/Qrogue',
-	download_url='https://github.com/7Magic7Mike7/Qrogue/releases/tag/0.6.2.1',  # link to Release on GitHub
+	download_url='https://github.com/7Magic7Mike7/Qrogue/releases/tag/0.6.3',  # link to Release on GitHub
 	keywords=['Quantum Computing', 'Gamification', 'Video Game', 'PyCUI'],
 	install_requires=[
 		'py-cui==0.1.4',
 		'numpy==1.22.3',
 		'qiskit==0.34.2',
 		'antlr4-python3-runtime==4.10',
 	],
```

