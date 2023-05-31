# Comparing `tmp/revolution-eda-0.4.1.tar.gz` & `tmp/revolution-eda-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revolution-eda-0.4.1.tar", last modified: Fri Feb 10 22:17:27 2023, max compression
+gzip compressed data, was "revolution-eda-0.5.0.tar", last modified: Wed May 31 12:21:04 2023, max compression
```

## Comparing `revolution-eda-0.4.1.tar` & `revolution-eda-0.5.0.tar`

### file list

```diff
@@ -1,50 +1,158 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 22:17:27.210817 revolution-eda-0.4.1/
--rw-rw-rw-   0        0        0     1087 2023-02-09 16:47:29.000000 revolution-eda-0.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1441 2023-02-10 22:17:27.209818 revolution-eda-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      987 2023-02-10 22:14:19.000000 revolution-eda-0.4.1/README_pypi.md
-drwxrwxrwx   0        0        0        0 2023-02-10 22:17:27.140161 revolution-eda-0.4.1/api/
--rw-rw-rw-   0        0        0     2820 2023-01-22 11:57:00.000000 revolution-eda-0.4.1/api/ui.py
-drwxrwxrwx   0        0        0        0 2023-02-10 22:17:27.145787 revolution-eda-0.4.1/backend/
--rw-rw-rw-   0        0        0     1071 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/backend/__init__.py
--rw-rw-rw-   0        0        0     5691 2022-12-25 21:30:50.000000 revolution-eda-0.4.1/backend/hdlBackEnd.py
--rw-rw-rw-   0        0        0     2279 2023-01-22 12:02:02.000000 revolution-eda-0.4.1/backend/libraryMethods.py
--rw-rw-rw-   0        0        0     8865 2023-01-10 20:27:51.000000 revolution-eda-0.4.1/backend/schBackEnd.py
--rw-rw-rw-   0        0        0     3026 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/backend/undoStack.py
-drwxrwxrwx   0        0        0        0 2023-02-10 22:17:27.156412 revolution-eda-0.4.1/common/
--rw-rw-rw-   0        0        0     2103 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/common/Point.py
--rw-rw-rw-   0        0        0     1830 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/common/Vector.py
--rw-rw-rw-   0        0        0     1072 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/common/__init__.py
--rw-rw-rw-   0        0        0     1229 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/common/cellview.py
--rw-rw-rw-   0        0        0     2650 2022-12-16 16:29:49.000000 revolution-eda-0.4.1/common/fonts.py
--rw-rw-rw-   0        0        0     2649 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/common/layers.py
--rw-rw-rw-   0        0        0     6737 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/common/net.py
--rw-rw-rw-   0        0        0     2653 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/common/pens.py
--rw-rw-rw-   0        0        0    57737 2023-02-10 20:15:17.000000 revolution-eda-0.4.1/common/shape.py
-drwxrwxrwx   0        0        0        0 2023-02-10 22:17:27.160407 revolution-eda-0.4.1/fileio/
--rw-rw-rw-   0        0        0     1072 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/fileio/__init__.py
--rw-rw-rw-   0        0        0     8617 2023-02-10 21:52:21.000000 revolution-eda-0.4.1/fileio/loadJSON.py
--rw-rw-rw-   0        0        0     7179 2023-02-10 21:47:17.000000 revolution-eda-0.4.1/fileio/symbolEncoder.py
-drwxrwxrwx   0        0        0        0 2023-02-10 22:17:27.170410 revolution-eda-0.4.1/gui/
--rw-rw-rw-   0        0        0     1072 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/gui/__init__.py
--rw-rw-rw-   0        0        0    21009 2023-02-10 11:48:36.000000 revolution-eda-0.4.1/gui/appWindow.py
--rw-rw-rw-   0        0        0     1617 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/gui/editFunctions.py
--rw-rw-rw-   0        0        0   162199 2023-02-10 21:17:30.000000 revolution-eda-0.4.1/gui/editorWindows.py
--rw-rw-rw-   0        0        0    26947 2023-01-30 11:24:48.000000 revolution-eda-0.4.1/gui/fileDialogues.py
--rw-rw-rw-   0        0        0    34635 2023-02-08 12:02:01.000000 revolution-eda-0.4.1/gui/propertyDialogues.py
--rw-rw-rw-   0        0        0     6784 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/gui/pythonConsole.py
-drwxrwxrwx   0        0        0        0 2023-02-10 22:17:27.173411 revolution-eda-0.4.1/pdk/
--rw-rw-rw-   0        0        0     1071 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/pdk/__init__.py
--rw-rw-rw-   0        0        0     1972 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/pdk/callbacks.py
--rw-rw-rw-   0        0        0      759 2023-02-10 22:15:05.000000 revolution-eda-0.4.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-02-10 22:17:27.174880 revolution-eda-0.4.1/resources/
--rw-rw-rw-   0        0        0   124102 2022-12-15 12:57:33.000000 revolution-eda-0.4.1/resources/resources.py
--rw-rw-rw-   0        0        0     1143 2023-02-10 22:17:11.000000 revolution-eda-0.4.1/revinit.py
-drwxrwxrwx   0        0        0        0 2023-02-10 22:17:27.208818 revolution-eda-0.4.1/revolution_eda.egg-info/
--rw-rw-rw-   0        0        0     1441 2023-02-10 22:17:27.000000 revolution-eda-0.4.1/revolution_eda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      821 2023-02-10 22:17:27.000000 revolution-eda-0.4.1/revolution_eda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 22:17:27.000000 revolution-eda-0.4.1/revolution_eda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-02-10 22:17:27.000000 revolution-eda-0.4.1/revolution_eda.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       31 2023-02-10 22:17:27.000000 revolution-eda-0.4.1/revolution_eda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       52 2023-02-10 22:17:27.000000 revolution-eda-0.4.1/revolution_eda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-10 22:17:27.210817 revolution-eda-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 16:48:55.000000 revolution-eda-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.779193 revolution-eda-0.5.0/
+-rw-rw-rw-   0        0        0      114 2023-05-23 10:07:51.000000 revolution-eda-0.5.0/.env
+-rw-rw-rw-   0        0        0     1087 2023-02-09 16:47:29.000000 revolution-eda-0.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      139 2023-05-31 12:16:47.000000 revolution-eda-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2203 2023-05-31 12:21:04.778401 revolution-eda-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1763 2023-05-23 10:07:51.000000 revolution-eda-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.376326 revolution-eda-0.5.0/docs/
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.476967 revolution-eda-0.5.0/docs/assets/
+-rw-rw-rw-   0        0        0     8942 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230209_082011.png
+-rw-rw-rw-   0        0        0   475487 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230210_113658.png
+-rw-rw-rw-   0        0        0    70438 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230210_142342.png
+-rw-rw-rw-   0        0        0    63865 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230210_142507.png
+-rw-rw-rw-   0        0        0    83180 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_204024.png
+-rw-rw-rw-   0        0        0    82595 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_204324.png
+-rw-rw-rw-   0        0        0    45362 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_210207.png
+-rw-rw-rw-   0        0        0    33070 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_211158.png
+-rw-rw-rw-   0        0        0    27216 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_212122.png
+-rw-rw-rw-   0        0        0    26926 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_213352.png
+-rw-rw-rw-   0        0        0    25662 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_213448.png
+-rw-rw-rw-   0        0        0    23583 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_213534.png
+-rw-rw-rw-   0        0        0    19764 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_214328.png
+-rw-rw-rw-   0        0        0    52005 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_214720.png
+-rw-rw-rw-   0        0        0    55425 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_215123.png
+-rw-rw-rw-   0        0        0    33406 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_215437.png
+-rw-rw-rw-   0        0        0    49907 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_215836.png
+-rw-rw-rw-   0        0        0   105491 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_220729.png
+-rw-rw-rw-   0        0        0   160790 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_221911.png
+-rw-rw-rw-   0        0        0   139162 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230214_225857.png
+-rw-rw-rw-   0        0        0    56372 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_104815.png
+-rw-rw-rw-   0        0        0    52976 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_113354.png
+-rw-rw-rw-   0        0        0    12448 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_113556.png
+-rw-rw-rw-   0        0        0    27513 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_113949.png
+-rw-rw-rw-   0        0        0    31774 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_114312.png
+-rw-rw-rw-   0        0        0    62743 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_114438.png
+-rw-rw-rw-   0        0        0    20453 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_152849.png
+-rw-rw-rw-   0        0        0    43440 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_153445.png
+-rw-rw-rw-   0        0        0    26210 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_153909.png
+-rw-rw-rw-   0        0        0    68838 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_154320.png
+-rw-rw-rw-   0        0        0    35198 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_154633.png
+-rw-rw-rw-   0        0        0    35993 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_154905.png
+-rw-rw-rw-   0        0        0    75895 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_155308.png
+-rw-rw-rw-   0        0        0    68774 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_163913.png
+-rw-rw-rw-   0        0        0    72575 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_164434.png
+-rw-rw-rw-   0        0        0    41952 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_172217.png
+-rw-rw-rw-   0        0        0    31943 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_172655.png
+-rw-rw-rw-   0        0        0    38087 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230215_173829.png
+-rw-rw-rw-   0        0        0   262766 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230216_100322.png
+-rw-rw-rw-   0        0        0    49810 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230216_101413-1676540084030-7.png
+-rw-rw-rw-   0        0        0    49810 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230216_101413.png
+-rw-rw-rw-   0        0        0    45971 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230216_103427.png
+-rw-rw-rw-   0        0        0    17810 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230216_120741.png
+-rw-rw-rw-   0        0        0    22104 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230216_123430.png
+-rw-rw-rw-   0        0        0    16465 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230216_123713.png
+-rw-rw-rw-   0        0        0    66178 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/Screenshot_20230216_124059.png
+-rw-rw-rw-   0        0        0     8675 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/image-20230209082042521.png
+-rw-rw-rw-   0        0        0     8675 2023-05-11 16:50:24.000000 revolution-eda-0.5.0/docs/assets/image-20230209082047928.png
+-rw-rw-rw-   0        0        0    32212 2023-05-26 11:27:21.000000 revolution-eda-0.5.0/docs/index.md
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.338559 revolution-eda-0.5.0/exampleLibraries/
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.478395 revolution-eda-0.5.0/exampleLibraries/analogLib/
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.480409 revolution-eda-0.5.0/exampleLibraries/analogLib/cap/
+-rw-rw-rw-   0        0        0     3244 2023-05-23 19:09:34.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/cap/symbol.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.494651 revolution-eda-0.5.0/exampleLibraries/analogLib/capVa/
+-rw-rw-rw-   0        0        0      825 2023-05-23 14:57:45.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/capVa/cap.va
+-rw-rw-rw-   0        0        0     5055 2023-05-23 21:07:53.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/capVa/symbol.json
+-rw-rw-rw-   0        0        0      247 2023-05-23 14:57:45.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/capVa/veriloga.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.502698 revolution-eda-0.5.0/exampleLibraries/analogLib/gnd/
+-rw-rw-rw-   0        0        0     2017 2023-05-23 21:04:41.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/gnd/symbol.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.511745 revolution-eda-0.5.0/exampleLibraries/analogLib/ind/
+-rw-rw-rw-   0        0        0     4485 2023-05-23 19:09:06.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/ind/symbol.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.519867 revolution-eda-0.5.0/exampleLibraries/analogLib/nmos/
+-rw-rw-rw-   0        0        0     6697 2023-05-26 19:16:57.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/nmos/symbol.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.528969 revolution-eda-0.5.0/exampleLibraries/analogLib/res/
+-rw-rw-rw-   0        0        0     3054 2023-05-25 12:55:41.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/res/symbol.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.552640 revolution-eda-0.5.0/exampleLibraries/analogLib/resVa/
+-rw-rw-rw-   0        0        0      662 2023-04-01 17:10:48.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/resVa/res.va
+-rw-rw-rw-   0        0        0      222 2023-02-19 22:52:34.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/resVa/veriloga.json
+-rw-rw-rw-   0        0        0        0 2023-05-30 10:13:56.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/reveda.lib
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.568801 revolution-eda-0.5.0/exampleLibraries/analogLib/vaVco/
+-rw-rw-rw-   0        0        0     6194 2023-05-25 11:37:58.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/vaVco/symbol.json
+-rw-rw-rw-   0        0        0     1063 2023-05-22 11:34:55.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/vaVco/vaVco.va
+-rw-rw-rw-   0        0        0      349 2023-05-22 11:34:55.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/vaVco/veriloga.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.579322 revolution-eda-0.5.0/exampleLibraries/analogLib/vdc/
+-rw-rw-rw-   0        0        0     4044 2023-05-23 21:01:26.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/vdc/symbol.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.588491 revolution-eda-0.5.0/exampleLibraries/analogLib/vdd/
+-rw-rw-rw-   0        0        0     1457 2023-05-23 21:08:20.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/vdd/symbol.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.593162 revolution-eda-0.5.0/exampleLibraries/analogLib/vpat/
+-rw-rw-rw-   0        0        0     3132 2023-05-24 07:13:18.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/vpat/symbol.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.602576 revolution-eda-0.5.0/exampleLibraries/analogLib/vsin/
+-rw-rw-rw-   0        0        0     5111 2023-05-23 20:43:36.000000 revolution-eda-0.5.0/exampleLibraries/analogLib/vsin/symbol.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.605279 revolution-eda-0.5.0/exampleLibraries/designs/
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.617718 revolution-eda-0.5.0/exampleLibraries/designs/LCFilter/
+-rw-rw-rw-   0        0        0     1150 2023-05-23 21:17:16.000000 revolution-eda-0.5.0/exampleLibraries/designs/LCFilter/schematic.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.639988 revolution-eda-0.5.0/exampleLibraries/designs/anotherFilter/
+-rw-rw-rw-   0        0        0     5252 2023-05-25 15:26:55.000000 revolution-eda-0.5.0/exampleLibraries/designs/anotherFilter/schematic.json
+-rw-rw-rw-   0        0        0     3044 2023-05-23 21:11:05.000000 revolution-eda-0.5.0/exampleLibraries/designs/anotherFilter/symbol.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.651608 revolution-eda-0.5.0/exampleLibraries/designs/cascadedFilter/
+-rw-rw-rw-   0        0        0       47 2023-05-30 20:37:11.000000 revolution-eda-0.5.0/exampleLibraries/designs/cascadedFilter/schematic.json
+-rw-rw-rw-   0        0        0     2880 2022-12-13 11:37:24.000000 revolution-eda-0.5.0/exampleLibraries/designs/cascadedFilter/symbol.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.671922 revolution-eda-0.5.0/exampleLibraries/designs/complexFilter/
+-rw-rw-rw-   0        0        0      727 2023-05-22 09:41:48.000000 revolution-eda-0.5.0/exampleLibraries/designs/complexFilter/config.json
+-rw-rw-rw-   0        0        0     8530 2023-05-25 15:03:54.000000 revolution-eda-0.5.0/exampleLibraries/designs/complexFilter/schematic.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.684579 revolution-eda-0.5.0/exampleLibraries/designs/highPassFilter/
+-rw-rw-rw-   0        0        0     4282 2023-05-25 18:22:47.000000 revolution-eda-0.5.0/exampleLibraries/designs/highPassFilter/schematic.json
+-rw-rw-rw-   0        0        0     2874 2023-05-20 22:11:19.000000 revolution-eda-0.5.0/exampleLibraries/designs/highPassFilter/symbol.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.693045 revolution-eda-0.5.0/exampleLibraries/designs/higherOrderFilter/
+-rw-rw-rw-   0        0        0     6567 2023-05-25 13:10:16.000000 revolution-eda-0.5.0/exampleLibraries/designs/higherOrderFilter/schematic.json
+-rw-rw-rw-   0        0        0     2479 2023-05-23 15:10:23.000000 revolution-eda-0.5.0/exampleLibraries/designs/higherOrderFilter/symbol.json
+-rw-rw-rw-   0        0        0        0 2023-05-09 20:31:10.000000 revolution-eda-0.5.0/exampleLibraries/designs/reveda.lib
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.704349 revolution-eda-0.5.0/exampleLibraries/designs/tb_anotherFilter/
+-rw-rw-rw-   0        0        0      690 2023-05-24 17:45:31.000000 revolution-eda-0.5.0/exampleLibraries/designs/tb_anotherFilter/config.json
+-rw-rw-rw-   0        0        0      662 2023-05-23 18:57:10.000000 revolution-eda-0.5.0/exampleLibraries/designs/tb_anotherFilter/res.va
+-rw-rw-rw-   0        0        0     6277 2023-05-24 22:02:28.000000 revolution-eda-0.5.0/exampleLibraries/designs/tb_anotherFilter/schematic.json
+-rw-rw-rw-   0        0        0    16727 2023-02-11 12:22:24.000000 revolution-eda-0.5.0/mozillaPublicLicense.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.708592 revolution-eda-0.5.0/pdk/
+-rw-rw-rw-   0        0        0     1071 2022-12-15 13:57:32.000000 revolution-eda-0.5.0/pdk/__init__.py
+-rw-rw-rw-   0        0        0     1972 2022-12-15 13:57:32.000000 revolution-eda-0.5.0/pdk/callbacks.py
+-rw-rw-rw-   0        0        0      812 2023-05-31 08:16:47.000000 revolution-eda-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0     3842 2023-05-23 10:07:51.000000 revolution-eda-0.5.0/reveda.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.344660 revolution-eda-0.5.0/revedaEditor/
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.723147 revolution-eda-0.5.0/revedaEditor/backend/
+-rw-rw-rw-   0        0        0     1071 2022-12-15 13:57:32.000000 revolution-eda-0.5.0/revedaEditor/backend/__init__.py
+-rw-rw-rw-   0        0        0     1865 2023-05-28 21:01:30.000000 revolution-eda-0.5.0/revedaEditor/backend/dataDefinitions.py
+-rw-rw-rw-   0        0        0     5918 2023-05-20 22:11:14.000000 revolution-eda-0.5.0/revedaEditor/backend/hdlBackEnd.py
+-rw-rw-rw-   0        0        0    11682 2023-05-20 21:55:29.000000 revolution-eda-0.5.0/revedaEditor/backend/importViews.py
+-rw-rw-rw-   0        0        0     2292 2023-03-31 22:24:42.000000 revolution-eda-0.5.0/revedaEditor/backend/libraryMethods.py
+-rw-rw-rw-   0        0        0     9097 2023-05-23 12:11:02.000000 revolution-eda-0.5.0/revedaEditor/backend/schBackEnd.py
+-rw-rw-rw-   0        0        0     3503 2023-05-11 17:00:40.000000 revolution-eda-0.5.0/revedaEditor/backend/undoStack.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.732696 revolution-eda-0.5.0/revedaEditor/common/
+-rw-rw-rw-   0        0        0     1072 2023-05-13 22:43:30.000000 revolution-eda-0.5.0/revedaEditor/common/__init__.py
+-rw-rw-rw-   0        0        0     2650 2022-12-16 17:29:48.000000 revolution-eda-0.5.0/revedaEditor/common/fonts.py
+-rw-rw-rw-   0        0        0     2649 2022-12-15 13:57:32.000000 revolution-eda-0.5.0/revedaEditor/common/layers.py
+-rw-rw-rw-   0        0        0    16666 2023-05-29 20:37:24.000000 revolution-eda-0.5.0/revedaEditor/common/net.py
+-rw-rw-rw-   0        0        0     2848 2023-05-11 21:06:35.000000 revolution-eda-0.5.0/revedaEditor/common/pens.py
+-rw-rw-rw-   0        0        0    61965 2023-05-28 21:54:20.000000 revolution-eda-0.5.0/revedaEditor/common/shape.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.737469 revolution-eda-0.5.0/revedaEditor/fileio/
+-rw-rw-rw-   0        0        0     1072 2022-12-15 13:57:32.000000 revolution-eda-0.5.0/revedaEditor/fileio/__init__.py
+-rw-rw-rw-   0        0        0     8844 2023-05-24 19:51:52.000000 revolution-eda-0.5.0/revedaEditor/fileio/loadJSON.py
+-rw-rw-rw-   0        0        0     7358 2023-05-09 11:54:17.000000 revolution-eda-0.5.0/revedaEditor/fileio/symbolEncoder.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.749103 revolution-eda-0.5.0/revedaEditor/gui/
+-rw-rw-rw-   0        0        0     1070 2023-05-22 14:30:52.000000 revolution-eda-0.5.0/revedaEditor/gui/__init__.py
+-rw-rw-rw-   0        0        0     1617 2022-12-15 13:57:32.000000 revolution-eda-0.5.0/revedaEditor/gui/editFunctions.py
+-rw-rw-rw-   0        0        0   173562 2023-05-30 11:14:11.000000 revolution-eda-0.5.0/revedaEditor/gui/editorWindows.py
+-rw-rw-rw-   0        0        0    27142 2023-05-16 14:45:24.000000 revolution-eda-0.5.0/revedaEditor/gui/fileDialogues.py
+-rw-rw-rw-   0        0        0    37119 2023-05-25 13:01:33.000000 revolution-eda-0.5.0/revedaEditor/gui/propertyDialogues.py
+-rw-rw-rw-   0        0        0     6723 2023-03-31 22:24:42.000000 revolution-eda-0.5.0/revedaEditor/gui/pythonConsole.py
+-rw-rw-rw-   0        0        0    10579 2023-05-23 18:44:24.000000 revolution-eda-0.5.0/revedaEditor/gui/revedaMain.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.749725 revolution-eda-0.5.0/revedaEditor/resources/
+-rw-rw-rw-   0        0        0   158489 2023-02-13 11:31:30.000000 revolution-eda-0.5.0/revedaEditor/resources/resources.py
+-rw-rw-rw-   0        0        0     1102 2023-05-30 11:14:11.000000 revolution-eda-0.5.0/revinit.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:21:04.776376 revolution-eda-0.5.0/revolution_eda.egg-info/
+-rw-rw-rw-   0        0        0     2203 2023-05-31 12:21:04.000000 revolution-eda-0.5.0/revolution_eda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6565 2023-05-31 12:21:04.000000 revolution-eda-0.5.0/revolution_eda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 12:21:04.000000 revolution-eda-0.5.0/revolution_eda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-31 12:21:04.000000 revolution-eda-0.5.0/revolution_eda.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       31 2023-05-31 12:21:04.000000 revolution-eda-0.5.0/revolution_eda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-05-31 12:21:04.000000 revolution-eda-0.5.0/revolution_eda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 12:21:04.779340 revolution-eda-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-02-11 13:22:24.000000 revolution-eda-0.5.0/setup.py
```

### Comparing `revolution-eda-0.4.1/LICENSE.txt` & `revolution-eda-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.4.1/backend/__init__.py` & `revolution-eda-0.5.0/pdk/__init__.py`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.4.1/backend/hdlBackEnd.py` & `revolution-eda-0.5.0/revedaEditor/backend/hdlBackEnd.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         self.instanceParams = dict()
         self.modelParams = dict()
         self.inPins = list()
         self.inoutPins = list()
         self.outPins = list()
         self._netlistLine = ''
         self.statementLines = list()
+        self._pinOrder = ''
 
         with open(self._pathObj) as f:
             self.fileLines = f.readlines()
         self.stripComments()
         self.oneLiners()
         # splitLines=[fileline.split() for fileline in fileLines]
 
@@ -84,14 +85,15 @@
                         self.inPins.extend([pin.strip() for pin in pinsList])
                     elif splitLine[0] == 'out' or splitLine[0] == 'output':
                         pinsList = splitLine[1].split(';')[0].split(',')
                         self.outPins.extend([pin.strip() for pin in pinsList])
                     elif splitLine[0] == 'inout':
                         pinsList = splitLine[1].split(';')[0].split(',')
                         self.inoutPins.extend([pin.strip() for pin in pinsList])
+
                     elif splitLine[0] == "parameter":
                         paramDefPart = tempLine.split('*(')[0]
                         paramName = paramDefPart.split('=')[0].split()[-1].strip()
                         paramValue = paramDefPart.split('=')[1].split()[0].strip()
 
                         try:
                             paramAttr = tempLine.strip().split("(*")[1]
@@ -112,21 +114,31 @@
 
     @pathObj.setter
     def pathObj(self, value:pathlib.Path):
         assert isinstance(value,pathlib.Path)
         self._pathObj = value
 
     @property
+    def pinOrder(self):
+        return self._pinOrder
+
+    @pinOrder.setter
+    def pinOrder(self, value:str):
+        assert isinstance(value,str)
+        self._pinOrder = value
+
+    @property
     def netlistLine(self):
-        pinsString = ' '.join([f'[|{pin}:%]' for pin in self.pins])
+        self._pinOrder = ','.join(self.pins)
+        print(f'pinOrder : {self.pinOrder}')
         instParamString = ' '.join(
             [f'[@{key}:{key}=%:{key}={item}]' for key, item in
              self.instanceParams.items()])
-        self._netlistLine = f'Y{self._vaModule} [@instName] {pinsString} ' \
-                f'[@vaModel:vaModel=%:vaModel={self._vaModule}Model] {instParamString}'
+        self._netlistLine = f'Y{self._vaModule} [@instName] [@pinList]  ' \
+                            f'{self._vaModule}Model {instParamString}'
         return self._netlistLine
 
     @netlistLine.setter
     def netListLine(self, value:str):
         assert isinstance(value,str)
         self._netlistLine = value
```

### Comparing `revolution-eda-0.4.1/backend/libraryMethods.py` & `revolution-eda-0.5.0/revedaEditor/backend/libraryMethods.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #    Software: Revolution EDA
 #    License: Mozilla Public License 2.0
 #    Licensor: Revolution Semiconductor (Registered in the Netherlands)
 
 from PySide6.QtCore import (Qt, )
 from PySide6.QtGui import (QStandardItemModel)
 
-import backend.schBackEnd as scb
+import revedaEditor.backend.schBackEnd as scb
 
 
 def getLibItem(libraryModel: QStandardItemModel, libName: str) -> scb.libraryItem:
     libItem = [item for item in libraryModel.findItems(libName) if
                item.data(Qt.UserRole + 1) == 'library'][0]
     return libItem
```

### Comparing `revolution-eda-0.4.1/backend/schBackEnd.py` & `revolution-eda-0.5.0/revedaEditor/backend/schBackEnd.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,240 +1,243 @@
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-# schematic editor backend
-import pathlib
-import shutil
-from pathlib import Path
-
-from PySide6.QtCore import (Qt, )
-from PySide6.QtGui import (QStandardItem, )
-from PySide6.QtWidgets import (QMessageBox, QGroupBox, QVBoxLayout, QDialog,
-                               QDialogButtonBox, QFormLayout)
-# from ruamel.yaml import YAML
-import json
-import fileio.symbolEncoder as se
-import gui.editFunctions as edf
-
-
-class libraryItem(QStandardItem):
-    def __init__(self, libraryPath: pathlib.Path):  # path is a pathlib.Path object
-        self._libraryPath = libraryPath
-        self._libraryName = libraryPath.name
-        super().__init__(self.libraryName)
-        self.setEditable(False)
-        self.setData(libraryPath, Qt.UserRole + 2)
-        self.setData("library", Qt.UserRole + 1)
-
-    def type(self):
-        return Qt.StandardItem.UserType
-
-    @property
-    def libraryPath(self):
-        return self._libraryPath
-
-    @libraryPath.setter
-    def libraryPath(self, value):
-        if isinstance(value, pathlib.Path):
-            self._libraryPath = value
-
-    @property
-    def libraryName(self):
-        return self._libraryName
-
-
-class cellItem(QStandardItem):
-    def __init__(self, cellPath: pathlib.Path) -> None:
-        self._cellName = cellPath.stem
-        # self._libName = self.parent.libraryName
-        super().__init__(self.cellName)
-        self.setEditable(False)
-        self.setData("cell", Qt.UserRole + 1)
-        self.setData(cellPath, Qt.UserRole + 2)
-
-    def type(self):
-        return QStandardItem.UserType + 1
-
-    @property
-    def cellName(self):
-        return self._cellName
-
-
-class viewItem(QStandardItem):
-    def __init__(self, viewPath: pathlib.Path) -> None:
-        self.viewPath = viewPath
-        super().__init__(self.viewPath.stem)
-        self.setEditable(False)
-        self.setData('view', Qt.UserRole + 1)
-        # set the data to the item to be the path to the view.
-        self.setData(viewPath, Qt.UserRole + 2)
-
-    def type(self):
-        return QStandardItem.UserType + 1
-
-    def delete(self):
-        '''
-        delete the view file and remove the row.
-        '''
-        self.viewPath.unlink()
-        viewRow = self.row()
-        parent = self.parent()
-        parent.removeRow(viewRow)
-
-    @property
-    def viewType(self):
-        if 'schematic' in self.viewPath.stem:
-            return 'schematic'
-        elif 'symbol' in self.viewPath.stem:
-            return 'symbol'
-        elif 'veriloga' in self.viewPath.stem:
-            return 'veriloga'
-        elif 'config' in self.viewPath.stem:
-            return 'config'
-        elif 'xyce' in self.viewPath.stem:
-            return 'xyce'
-        elif 'spice' in self.viewPath.stem:
-            return 'spice'
-        else:
-            return None
-
-    @property
-    def viewName(self):
-        return self.viewPath.stem
-
-
-def createLibrary(parent, model, libraryDir, libraryName) -> libraryItem:
-    if libraryName.strip() == "":
-        QMessageBox.warning(parent, "Error", "Please enter a library name")
-    else:
-        libraryPath = Path(libraryDir).joinpath(libraryName)
-        if libraryPath.exists():
-            QMessageBox.warning(parent, "Error", "Library already exits.")
-        else:
-            libraryPath.mkdir()
-            newLibraryItem = libraryItem(libraryPath)
-            newLibraryItem.setData(libraryPath, Qt.UserRole + 2)
-            newLibraryItem.setData("library", Qt.UserRole + 1)
-            model.appendRow(newLibraryItem)
-            print(f"Created {libraryPath}")
-    return newLibraryItem
-
-
-def createCell(parent, model, selectedLib, cellName) -> cellItem:
-    # assert isinstance(selectedLib, libraryItem)
-    if selectedLib.data(Qt.UserRole + 1) == "library":
-        selectedLibPath = selectedLib.data(Qt.UserRole + 2)
-        cellPath = selectedLibPath.joinpath(cellName)
-        if cellName.strip() == "":
-            QMessageBox.warning(parent, "Error", "Please enter a cell name")
-            return None
-        elif cellPath.exists():
-            QMessageBox.warning(parent, "Error", "Cell already exits. Delete cell first.")
-            return None
-        else:
-            cellPath.mkdir()
-            # parentLibrary = model.findItems(selectedLibPath.stem,
-            #                                 flags=Qt.MatchExactly)[0]
-            newCellItem = cellItem(cellPath)
-            selectedLib.appendRow(newCellItem)
-            parent.logger.warning(f"Created {cellName} cell at {str(cellPath)}")
-            return newCellItem
-
-
-def createCellView(parent, viewName, cellItem: cellItem) -> viewItem:
-    if viewName.strip() == "":
-        QMessageBox.warning(parent, "Error", "Please enter a view name")
-        return None
-    viewPath = cellItem.data(Qt.UserRole + 2).joinpath(f'{viewName}.json')
-    if viewPath.exists():
-        parent.logger.warning('Replacing the cell view.')
-        oldView = [cellItem.child(row) for row in range(cellItem.rowCount()) if
-                   cellItem.child(row).viewName == viewName][0]
-        oldView.delete()
-    newViewItem = viewItem(viewPath)
-    viewPath.touch()  # create empty cell view
-    items = list()
-    if 'schematic' in viewName:
-        items.insert(0, {'viewName': 'schematic'})
-    elif 'symbol' in viewName:
-        items.insert(0, {'viewName': 'symbol'})
-    elif 'veriloga' in viewName:
-        items.insert(0, {'viewName': 'veriloga'})
-    elif 'config' in viewName:
-        items.insert(0, {'viewName': 'config'})
-    with viewPath.open(mode='w') as f:
-        json.dump(items, f, indent=4)
-    parent.logger.warning(f'Created {viewName} at {str(viewPath)}')
-    cellItem.appendRow(newViewItem)
-
-    return newViewItem
-
-
-# function for copying a cell
-def copyCell(parent, model, origCellItem: cellItem, copyName, selectedLibPath) -> bool:
-    """
-    parent: the parent widget
-    model: the model
-    cellItem: the cell item in the model
-    copyName: the name of the new cell
-    selectedLibPath: the path of the selected library
-    """
-    cellPath = origCellItem.data(Qt.UserRole + 2)  # get the cell path from item user data
-    if copyName == "":  # assign a default name for the cell
-        copyName = "newCell"
-    copyPath = selectedLibPath.joinpath(copyName)
-    if copyPath.exists():
-        QMessageBox.warning(parent, "Error", "Cell already exits.")
-        return False
-    else:
-        assert cellPath.exists()
-        shutil.copytree(cellPath, copyPath)  # copied the cell
-        libraryItem = model.findItems(selectedLibPath.cellName, flags=Qt.MatchExactly)[
-            0]  # find the library item
-        # create new cell item
-        newCellItem = cellItem(copyPath.cellName)
-        newCellItem.setEditable(False)
-        newCellItem.setData("cell", Qt.UserRole + 1)
-        newCellItem.setData(copyPath, Qt.UserRole + 2)
-        # go through view list and add to cell item
-        viewList = [str(view.stem) for view in copyPath.iterdir() if
-                    view.suffix == ".json"]
-
-        for view in viewList:
-            addedView = viewItem(copyPath.joinpath(view).with_suffix(".json"))
-            addedView.setData("view", Qt.UserRole + 1)
-            # set the data to the item to be the path to the view.
-            addedView.setData(copyPath.joinpath(view).with_suffix(".json"),
-                              Qt.UserRole + 2, )
-            addedView.setEditable(False)
-            cellItem.appendRow(addedView)
-        libraryItem.appendRow(cellItem)
-        return True
-
-
-def renameCell(parent, oldCell, newName) -> bool:
-    cellPath = oldCell.data(Qt.UserRole + 2)
-    if newName.strip() == "":
-        QMessageBox.warning(parent, "Error", "Please enter a cell name")
-        return False
-    else:
-        cellPath.rename(cellPath.parent / newName)
-        oldCell.setText(newName)
-        return True
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+# from ruamel.yaml import YAML
+import json
+# schematic editor backend
+import pathlib
+import shutil
+from pathlib import Path
+
+from PySide6.QtCore import (Qt, )
+from PySide6.QtGui import (QStandardItem, )
+from PySide6.QtWidgets import (QMessageBox)
+
+
+class libraryItem(QStandardItem):
+    def __init__(self, libraryPath: pathlib.Path):  # path is a pathlib.Path object
+        self._libraryPath = libraryPath
+        self._libraryName = libraryPath.name
+        super().__init__(self.libraryName)
+        self.setEditable(False)
+        self.setData(libraryPath, Qt.UserRole + 2)
+        self.setData("library", Qt.UserRole + 1)
+
+    def type(self):
+        return Qt.StandardItem.UserType
+
+    def __repr__(self):
+        return f"library item path: {self.libraryPath}, \nlibrary item name: {self.libraryName}"
+
+    @property
+    def libraryPath(self):
+        return self._libraryPath
+
+    @libraryPath.setter
+    def libraryPath(self, value):
+        if isinstance(value, pathlib.Path):
+            self._libraryPath = value
+
+    @property
+    def libraryName(self):
+        return self._libraryName
+
+
+class cellItem(QStandardItem):
+    def __init__(self, cellPath: pathlib.Path) -> None:
+        self._cellName = cellPath.stem
+        # self._libName = self.parent.libraryName
+        super().__init__(self.cellName)
+        self.setEditable(False)
+        self.setData("cell", Qt.UserRole + 1)
+        self.setData(cellPath, Qt.UserRole + 2)
+
+    def type(self):
+        return QStandardItem.UserType + 1
+
+    def __repr__(self):
+        return f"cell item path: {self.cellPath}, \ncell item name: {self.cellName}"
+
+    @property
+    def cellName(self):
+        return self._cellName
+
+
+class viewItem(QStandardItem):
+    def __init__(self, viewPath: pathlib.Path) -> None:
+        self.viewPath = viewPath
+        super().__init__(self.viewPath.stem)
+        self.setEditable(False)
+        self.setData('view', Qt.UserRole + 1)
+        # set the data to the item to be the path to the view.
+        self.setData(viewPath, Qt.UserRole + 2)
+
+    def type(self):
+        return QStandardItem.UserType + 1
+
+    def __repr__(self):
+        return f"view item path: {self.viewPath}, \nview item name: {self.viewName}"
+
+    def delete(self):
+        '''
+        delete the view file and remove the row.
+        '''
+        self.viewPath.unlink()
+        viewRow = self.row()
+        parent = self.parent()
+        parent.removeRow(viewRow)
+
+    @property
+    def viewType(self):
+        if 'schematic' in self.viewPath.stem:
+            return 'schematic'
+        elif 'symbol' in self.viewPath.stem:
+            return 'symbol'
+        elif 'veriloga' in self.viewPath.stem:
+            return 'veriloga'
+        elif 'config' in self.viewPath.stem:
+            return 'config'
+        elif 'xyce' in self.viewPath.stem:
+            return 'xyce'
+        elif 'spice' in self.viewPath.stem:
+            return 'spice'
+        elif 'myhdl'  in self.viewPath.stem:
+            return 'myhdl'
+        else:
+            return None
+
+    @property
+    def viewName(self):
+        return self.viewPath.stem
+
+
+def createLibrary(parent, model, libraryDir, libraryName) -> libraryItem:
+    if libraryName.strip() == "":
+        QMessageBox.warning(parent, "Error", "Please enter a library name")
+    else:
+        libraryPath = Path(libraryDir).joinpath(libraryName)
+        if libraryPath.exists():
+            QMessageBox.warning(parent, "Error", "Library already exits.")
+        else:
+            libraryPath.mkdir()
+            newLibraryItem = libraryItem(libraryPath)
+            newLibraryItem.setData(libraryPath, Qt.UserRole + 2)
+            newLibraryItem.setData("library", Qt.UserRole + 1)
+            model.appendRow(newLibraryItem)
+            print(f"Created {libraryPath}")
+    return newLibraryItem
+
+
+def createCell(parent, model, selectedLib, cellName) -> cellItem:
+    # assert isinstance(selectedLib, libraryItem)
+    if selectedLib.data(Qt.UserRole + 1) == "library":
+        selectedLibPath = selectedLib.data(Qt.UserRole + 2)
+        cellPath = selectedLibPath.joinpath(cellName)
+        if cellName.strip() == "":
+            QMessageBox.warning(parent, "Error", "Please enter a cell name")
+            return None
+        elif cellPath.exists():
+            QMessageBox.warning(parent, "Error", "Cell already exits. Delete cell first.")
+            return None
+        else:
+            cellPath.mkdir()
+            # parentLibrary = model.findItems(selectedLibPath.stem,
+            #                                 flags=Qt.MatchExactly)[0]
+            newCellItem = cellItem(cellPath)
+            selectedLib.appendRow(newCellItem)
+            parent.logger.warning(f"Created {cellName} cell at {str(cellPath)}")
+            return newCellItem
+
+
+def createCellView(parent, viewName, cellItem: cellItem) -> viewItem:
+    if viewName.strip() == "":
+        QMessageBox.warning(parent, "Error", "Please enter a view name")
+        return None
+    viewPath = cellItem.data(Qt.UserRole + 2).joinpath(f'{viewName}.json')
+    if viewPath.exists():
+        parent.logger.warning('Replacing the cell view.')
+        oldView = [cellItem.child(row) for row in range(cellItem.rowCount()) if
+                   cellItem.child(row).viewName == viewName][0]
+        oldView.delete()
+    newViewItem = viewItem(viewPath)
+    viewPath.touch()  # create empty cell view
+    items = list()
+    if 'schematic' in viewName:
+        items.insert(0, {'viewName': 'schematic'})
+    elif 'symbol' in viewName:
+        items.insert(0, {'viewName': 'symbol'})
+    elif 'veriloga' in viewName:
+        items.insert(0, {'viewName': 'veriloga'})
+    elif 'config' in viewName:
+        items.insert(0, {'viewName': 'config'})
+    with viewPath.open(mode='w') as f:
+        json.dump(items, f, indent=4)
+    parent.logger.warning(f'Created {viewName} at {str(viewPath)}')
+    cellItem.appendRow(newViewItem)
+
+    return newViewItem
+
+
+# function for copying a cell
+def copyCell(parent, model, origCellItem: cellItem, copyName, selectedLibPath) -> bool:
+    """
+    parent: the parent widget
+    model: the model
+    cellItem: the cell item in the model
+    copyName: the name of the new cell
+    selectedLibPath: the path of the selected library
+    """
+    cellPath = origCellItem.data(Qt.UserRole + 2)  # get the cell path from item user data
+    if copyName == "":  # assign a default name for the cell
+        copyName = "newCell"
+    copyPath = selectedLibPath.joinpath(copyName)
+    if copyPath.exists():
+        QMessageBox.warning(parent, "Error", "Cell already exits.")
+        return False
+    else:
+        assert cellPath.exists()
+        shutil.copytree(cellPath, copyPath)  # copied the cell
+        libraryItem = model.findItems(selectedLibPath.name, flags=Qt.MatchExactly)[
+            0]  # find the library item
+        # create new cell item
+        newCellItem = cellItem(copyPath)
+        newCellItem.setEditable(False)
+        newCellItem.setData("cell", Qt.UserRole + 1)
+        newCellItem.setData(copyPath, Qt.UserRole + 2)
+        # go through view list and add to cell item
+        addedViewList = [viewItem(viewPath) for viewPath in copyPath.iterdir() if
+                    viewPath.suffix == ".json"]
+        [addedView.setEditable(False) for addedView in addedViewList]
+
+        newCellItem.appendRows(addedViewList)
+        # add the new cell item to the library item
+        libraryItem.appendRow(newCellItem)
+        return True
+
+
+def renameCell(parent, oldCell, newName) -> bool:
+    cellPath = oldCell.data(Qt.UserRole + 2)
+    if newName.strip() == "":
+        QMessageBox.warning(parent, "Error", "Please enter a cell name")
+        return False
+    else:
+        cellPath.rename(cellPath.parent / newName)
+        oldCell.setText(newName)
+        return True
```

### Comparing `revolution-eda-0.4.1/common/Vector.py` & `revolution-eda-0.5.0/revedaEditor/gui/editFunctions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+
 #   “Commons Clause” License Condition v1.0
 #  #
 #   The Software is provided to you by the Licensor under the License, as defined
 #   below, subject to the following condition.
 #  #
 #   Without limiting other conditions in the License, the grant of rights under the
 #   License will not include, and the License does not grant to you, the right to
@@ -16,37 +17,27 @@
 #   license notice or attribution required by the License must also include this
 #   Commons Clause License Condition notice.
 #  #
 #   Software: Revolution EDA
 #   License: Mozilla Public License 2.0
 #   Licensor: Revolution Semiconductor (Registered in the Netherlands)
 
-# vector class
-# (C) Revolution Semiconductor, 2021
-# All rights reserved
-import math
-from PySide6.QtGui import QVector2D as QVec2
-
-class Vector(QVec2):
-    def __init__(self, *args):
-        if len(args) == 4:
-            self.x = args[2] - args[0]
-            self.y = args[3] - args[1]
-        elif len(args) == 2:
-            self.x = args[0]
-            self.y = args[1]  
-        elif len(args) == 0:
-            self.x = 0
-            self.y = 0
-        else:
-            raise ValueError("Vector: wrong number of arguments")
-        if hasattr(self,'x') and hasattr(self,'y'): # check if dx and dy are defined
-            super().__init__(self.x,self.y)
-        
-    def normal(self):
-        return Vector(self.x, self.y).normalized()
-
-
-        
-
- 
+from PySide6.QtCore import (Qt, )
+from PySide6.QtWidgets import (QLineEdit, QLabel, QWidget)
 
+class shortLineEdit(QLineEdit):
+    def __init__(self):
+        super().__init__(None)
+        self.setMaximumWidth(80)
+
+
+class boldLabel(QLabel):
+    def __init__(self, text: str, parent: QWidget = None):
+        super().__init__(text, parent)
+        self.setTextFormat(Qt.RichText)
+        self.setText("<b>" + text + "</b>")
+
+
+class longLineEdit(QLineEdit):
+    def __init__(self):
+        super().__init__(None)
+        self.setMaximumWidth(500)
```

### Comparing `revolution-eda-0.4.1/common/__init__.py` & `revolution-eda-0.5.0/revedaEditor/common/__init__.py`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.4.1/common/fonts.py` & `revolution-eda-0.5.0/revedaEditor/common/fonts.py`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.4.1/common/layers.py` & `revolution-eda-0.5.0/revedaEditor/common/layers.py`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.4.1/common/pens.py` & `revolution-eda-0.5.0/revedaEditor/common/pens.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,68 @@
-
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-from PySide6.QtCore import (Qt)
-from PySide6.QtGui import (QPen, QColor)
-from common.layers import (wireLayer,symbolLayer,selectedWireLayer,pinLayer,labelLayer,
-                           textLayer, draftLayer)
-
-
-class pen(QPen):
-    def __init__(self,pname:str,pcolor:QColor, pwidth:int,
-                 plinestyle:Qt.PenStyle=Qt.SolidLine):
-        super().__init__()
-        self._pname = pname
-        self._pcolor = pcolor
-        self._pwidth = pwidth
-        self._plinestyle = plinestyle
-        self.setWidth(self._pwidth)
-        self.setColor(self._pcolor)
-        self.setStyle(self._plinestyle)
-
-    @property
-    def pname(self):
-        return self._pname
-    @classmethod
-    def returnPen(cls,penName):
-        match penName:
-            case 'wirePen':
-                rpen = cls('wirePen',wireLayer.color,2)
-                rpen.setCosmetic(True)
-            case 'symbolPen':
-                rpen = cls("symbolPen",symbolLayer.color, 3)
-                rpen.setCosmetic(True)
-            case 'selectedWirePen':
-                rpen = cls("selectedWirePen",selectedWireLayer.color, 2)
-            case 'pinPen':
-                rpen = cls('pinPen', pinLayer.color, 2)
-            case 'labelPen':
-                rpen = cls('labelPen',labelLayer.color, 1)
-            case 'textPen':
-                rpen = cls('textPen',textLayer.color, 1)
-            case 'draftPen':
-                rpen = cls('draftPen',draftLayer.color, 1, Qt.DashLine)
-            case other:
-                rpen = cls('otherPen', QColor('darkGray'), 1, Qt.DotLine )
-        return rpen
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+from PySide6.QtCore import (Qt)
+from PySide6.QtGui import (QPen, QColor)
+
+from revedaEditor.common.layers import (wireLayer, symbolLayer,
+                                        selectedWireLayer, pinLayer,
+                                        labelLayer,
+                                        textLayer, draftLayer)
+
+
+class sPen(QPen):
+    def __init__(self, pname: str, pcolor: QColor, pwidth: int,
+                 plinestyle: Qt.PenStyle = Qt.SolidLine):
+        super().__init__()
+        self._pname = pname
+        self._pcolor = pcolor
+        self._pwidth = pwidth
+        self._plinestyle = plinestyle
+        self.setWidth(self._pwidth)
+        self.setColor(self._pcolor)
+        self.setStyle(self._plinestyle)
+
+    @property
+    def pname(self):
+        return self._pname
+
+    @classmethod
+    def returnPen(cls, penName):
+        match penName:
+            case 'wirePen':
+                rpen = cls('wirePen', wireLayer.color, 2)
+                rpen.setCosmetic(True)
+            case 'symbolPen':
+                rpen = cls("symbolPen", symbolLayer.color, 2)
+                rpen.setCosmetic(True)
+            case 'selectedWirePen':
+                rpen = cls("selectedWirePen", selectedWireLayer.color, 2)
+            case 'pinPen':
+                rpen = cls('pinPen', pinLayer.color, 2)
+            case 'labelPen':
+                rpen = cls('labelPen', labelLayer.color, 1)
+            case 'textPen':
+                rpen = cls('textPen', textLayer.color, 1)
+            case 'draftPen':
+                rpen = cls('draftPen', draftLayer.color, 2, Qt.DashLine)
+            case other:
+                rpen = cls('otherPen', QColor('darkGray'), 2, Qt.DotLine)
+        return rpen
```

### Comparing `revolution-eda-0.4.1/common/shape.py` & `revolution-eda-0.5.0/revedaEditor/common/shape.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,25 @@
 #   license notice or attribution required by the License must also include this
 #   Commons Clause License Condition notice.
 #  #
 #   Software: Revolution EDA
 #   License: Mozilla Public License 2.0
 #   Licensor: Revolution Semiconductor (Registered in the Netherlands)
 
+import math
+
 # shape class definition for symbol editor.
 # base class for all shapes: rectangle, circle, line
-from PySide6.QtCore import (QPoint, QPointF, QRect, QRectF, Qt, QLine, QLineF)
-from PySide6.QtGui import (QPen, QFont, QFontMetrics, QColor, QPainterPath,
-                           QTextOption, QFontDatabase, QTransform)
+from PySide6.QtCore import QPoint, QRect, QRectF, Qt, QLine, QLineF
+from PySide6.QtGui import (QPen, QFont, QFontMetrics, QPainterPath, QTextOption,
+                           QFontDatabase, )
 from PySide6.QtWidgets import (QGraphicsItem, QGraphicsSceneMouseEvent, )
-import math
 from quantiphy import Quantity
+import revedaEditor.common.net as net
+import revedaEditor.backend.dataDefinitions as ddef
 import pdk.callbacks as cb
 
 
 class shape(QGraphicsItem):
     def __init__(self, pen: QPen, gridTuple: tuple) -> None:
         super().__init__()
         self.setFlag(QGraphicsItem.ItemIsMovable, True)
@@ -111,17 +114,17 @@
             self.setFlag(QGraphicsItem.ItemIsMovable, False)
             self.setFlag(QGraphicsItem.ItemIsSelectable, False)
         else:
             self.setFlag(QGraphicsItem.ItemIsMovable, True)
             self.setFlag(QGraphicsItem.ItemIsSelectable, True)
 
     def sceneEvent(self, event):
-        '''
+        """
         Do not propagate event if shape needs to keep still.
-        '''
+        """
 
         if self.scene() and (self.scene().changeOrigin or self.scene().drawMode):
             return False
         else:
             super().sceneEvent(event)
             return True
 
@@ -143,62 +146,63 @@
         self.setOpacity(1)
         self.clearFocus()
 
     def contextMenuEvent(self, event):
         self.scene().itemContextMenu.exec_(event.screenPos())
 
     def snapToBase(self, number, base):
-        '''
+        """
         Restrict a number to the multiples of base
-        '''
+        """
         return base * int(round(number / base))
 
     def snapToGrid(self, point: QPoint, gridTuple: tuple[int, int]):
         """
         snap point to grid. Divides and multiplies by grid size.
         """
         return QPoint(gridTuple[0] * int(round(point.x() / gridTuple[0])),
                       gridTuple[1] * int(round(point.y() / gridTuple[1])), )
 
 
 class rectangle(shape):
     """
     rect: QRect defined by top left corner and bottom right corner. QRect(Point1,Point2)
     """
-    sides = ['Left', 'Right', 'Top', 'Bottom']
+
+    sides = ["Left", "Right", "Top", "Bottom"]
 
     def __init__(self, start: QPoint, end: QPoint, pen: QPen, grid: tuple, ):
         super().__init__(pen, grid)
         self._rect = QRectF(start, end).normalized()
         self._start = self._rect.topLeft()
         self._end = self._rect.bottomRight()
         self._stretchSide = None
 
     def boundingRect(self):
-        return self.rect.normalized().adjusted(-2, -2, 2, 2)
+        return self._rect.normalized().adjusted(-2, -2, 2, 2)
 
     def paint(self, painter, option, widget):
         if self.isSelected():
             painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
-            painter.drawRect(self.rect)
+            painter.drawRect(self._rect)
             if self.stretch:
                 painter.setPen(QPen(Qt.red, 2, Qt.SolidLine))
                 if self._stretchSide == rectangle.sides[0]:
                     painter.drawLine(self.rect.topLeft(), self.rect.bottomLeft())
                 elif self._stretchSide == rectangle.sides[1]:
                     painter.drawLine(self.rect.topRight(),
                                      self.rect.bottomRight())
                 elif self._stretchSide == rectangle.sides[2]:
                     painter.drawLine(self.rect.topLeft(), self.rect.topRight())
                 elif self._stretchSide == rectangle.sides[3]:
                     painter.drawLine(self.rect.bottomLeft(),
                                      self.rect.bottomRight())
         else:
-            painter.setPen(self.pen)
-            painter.drawRect(self.rect)
+            painter.setPen(self._pen)
+            painter.drawRect(self._rect)
 
     @property
     def rect(self):
         return self._rect
 
     @rect.setter
     def rect(self, rect: QRect):
@@ -208,23 +212,25 @@
     @property
     def start(self):
         return self._start
 
     @start.setter
     def start(self, start: QPoint):
         self.prepareGeometryChange()
+        self._rect = QRectF(start, self.end).normalized()
         self._start = start
 
     @property
     def end(self):
         return self._end
 
     @end.setter
     def end(self, end: QPoint):
         self.prepareGeometryChange()
+        self._rect = QRectF(self.start, end).normalized()
         self._end = end
 
     @property
     def centre(self):
         return QPoint(int(self._rect.x() + self._rect.width() / 2),
                       int(self._rect.y() + self._rect.height() / 2), )
 
@@ -250,65 +256,61 @@
     def objName(self):
         return "RECTANGLE"
 
     @property
     def left(self):
         return self.rect.left()
 
-    @property
-    def right(self):
-        return self.rect.right()
-
-    @property
-    def top(self):
-        return self.rect.top()
-
-    @property
-    def bottom(self):
-        return self.rect.bottom()
-
     @left.setter
     def left(self, left: int):
         self.rect.setLeft(left)
 
+    @property
+    def right(self):
+        return self.rect.right()
+
     @right.setter
     def right(self, right: int):
+        self.prepareGeometryChange()
         self.rect.setRight(right)
 
+    @property
+    def top(self):
+        return self.rect.top()
+
     @top.setter
     def top(self, top: int):
+        self.prepareGeometryChange()
         self.rect.setTop(top)
 
+    @property
+    def bottom(self):
+        return self.rect.bottom()
+
     @bottom.setter
     def bottom(self, bottom: int):
+        self.prepareGeometryChange()
         self.rect.setBottom(bottom)
 
-    @height.setter
-    def height(self, height: int):
-        self.rect.setHeight(height)
-
-    @width.setter
-    def width(self, width: int):
-        self.rect.setWidth(width)
-
     @property
     def origin(self):
         return self.rect.bottomLeft()
 
     @property
     def stretchSide(self):
         return self._stretchSide
 
     @stretchSide.setter
     def stretchSide(self, value: str):
+        self.prepareGeometryChange()
         self._stretchSide = value
 
     def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
         super().mousePressEvent(event)
-        eventPos = self.snapToGrid(event.pos(), self.gridTuple)
+        eventPos = event.pos().toPoint()
         if self._stretch:
             self.setFlag(QGraphicsItem.ItemIsMovable, False)
             if eventPos.x() == self.snapToBase(self._rect.left(),
                                                self.gridTuple[0]):
                 if self._rect.top() <= eventPos.y() <= self._rect.bottom():
                     self.setCursor(Qt.SizeHorCursor)
                     self._stretchSide = rectangle.sides[0]
@@ -325,15 +327,15 @@
             elif eventPos.y() == self.snapToBase(self._rect.bottom(),
                                                  self.gridTuple[1]):
                 if self._rect.left() <= eventPos.x() <= self._rect.right():
                     self.setCursor(Qt.SizeVerCursor)
                     self._stretchSide = rectangle.sides[3]
 
     def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        eventPos = self.snapToGrid(event.pos(), self.gridTuple)
+        eventPos = event.pos().toPoint()
         if self.stretch:
             self.prepareGeometryChange()
             if self.stretchSide == rectangle.sides[0]:
                 self.setCursor(Qt.SizeHorCursor)
                 self.rect.setLeft(eventPos.x())
             elif self.stretchSide == rectangle.sides[1]:
                 self.setCursor(Qt.SizeHorCursor)
@@ -347,16 +349,16 @@
             self.update()
         else:
             super().mouseMoveEvent(event)
 
     def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
         self.setFlag(QGraphicsItem.ItemIsMovable, True)
         super().mouseReleaseEvent(event)
-        self.start = self.rect.topLeft()
-        self.end = self.rect.bottomRight()
+        # self.start = self.rect.topLeft()
+        # self.end = self.rect.bottomRight()
         if self.stretch:
             self._stretch = False
             self._stretchSide = None
             self.setCursor(Qt.ArrowCursor)
 
 
 class circle(shape):
@@ -372,14 +374,15 @@
         self._end = self._centre + QPoint(self._radius, 0)  # along x-axis
         self._stretch = False
         self._startStretch = False
 
     def paint(self, painter, option, widget) -> None:
         if self.isSelected():
             painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
+            painter.drawEllipse(self._centre, 1, 1)
             if self._stretch:
                 painter.setPen(QPen(Qt.red, 2, Qt.SolidLine))
         else:
             painter.setPen(self._pen)
         painter.drawEllipse(self._centre, self._radius, self._radius)
 
     @property
@@ -398,17 +401,17 @@
     def radius(self):
         return self._radius
 
     @radius.setter
     def radius(self, radius: int):
         self.prepareGeometryChange()
         self._radius = self.snapToBase(radius, self._gridTuple[0])
-        # self.topLeft = self._centre - QPoint(self._radius, self._radius)
-        # self.rightBottom = self._centre + QPoint(self._radius, self._radius)
         self._end = self._centre + QPoint(self._radius, 0)
+        self._topLeft = self._centre - QPoint(self._radius, self._radius)
+        self._rightBottom = self._centre + QPoint(self._radius, self._radius)
 
     @property
     def centre(self):
         return self._centre
 
     @centre.setter
     def centre(self, value: QPoint):
@@ -419,14 +422,15 @@
     @property
     def end(self):
         return self._end
 
     @end.setter
     def end(self, value: QPoint):
         if isinstance(value, QPoint):
+            self.prepareGeometryChange()
             self._end = value
 
     @property
     def rightBottom(self):
         return self._rightBottom
 
     @rightBottom.setter
@@ -444,39 +448,40 @@
             self._topLeft = value
 
     @property
     def objName(self):
         return "CIRCLE"
 
     def boundingRect(self):
-        return QRectF(self._topLeft, self._rightBottom).normalized().adjusted(-2,
-            -2, 2, 2)
+        return (
+            QRectF(self._topLeft, self._rightBottom).normalized().adjusted(-2, -2,
+                                                                           2, 2))
 
     def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
         super().mousePressEvent(event)
         if self.isSelected() and self._stretch:
             self.setFlag(QGraphicsItem.ItemIsMovable, False)
             # eventPos = self.snap2grid(event.pos(), self._gridTuple)
-            eventPos = event.pos()
+            eventPos = event.pos().toPoint()
             distance = self.snapToBase(math.sqrt(
                 (eventPos.x() - self._centre.x()) ** 2 + (
                         eventPos.y() - self._centre.y()) ** 2),
-                self._gridTuple[0])
+                                       self._gridTuple[0], )
             if distance == self._radius:
                 self._startStretch = True
                 self.setCursor(Qt.DragMoveCursor)
 
     def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
         super().mouseMoveEvent(event)
         if self._startStretch:
-            eventPos = self.snapToGrid(event.pos(), self._gridTuple)
+            eventPos = event.pos().toPoint()
             distance = self.snapToBase(math.sqrt(
                 (eventPos.x() - self._centre.x()) ** 2 + (
                         eventPos.y() - self._centre.y()) ** 2),
-                self._gridTuple[0])
+                                       self._gridTuple[0], )
             self.prepareGeometryChange()
             self._radius = distance
 
     def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
         super().mouseReleaseEvent(event)
         if self._startStretch:
             self._startStretch = False
@@ -488,28 +493,33 @@
             self.setCursor(Qt.ArrowCursor)
 
 
 class arc(shape):
     """
     Class to draw arc shapes. Can have four directions.
     """
-    arcTypes = ['Up', 'Right', 'Down', 'Left']
-    sides = ['Left', 'Right', 'Top', 'Bottom']
+
+    arcTypes = ["Up", "Right", "Down", "Left"]
+    sides = ["Left", "Right", "Top", "Bottom"]
 
     def __init__(self, start: QPoint, end: QPoint, pen: QPen, gridTuple: tuple):
         super().__init__(pen, gridTuple)
         self._start = start
         self._end = end
         self._rect = QRectF(self._start, self._end).normalized()
         self._arcLine = QLineF(self._start, self._end)
-        self._arcAngle = self._arcLine.angle()
+        self._arcAngle = 0
         self._width = self._rect.width()
         self._height = self._rect.height()
         self._adjustment = int(self.pen.width() / 2)
         self._stretchSide = None
+        self.findAngle()
+
+    def findAngle(self):
+        self._arcAngle = self._arcLine.angle()
         if 90 >= self._arcAngle >= 0:
             self._arcType = arc.arcTypes[0]
         elif 180 >= self._arcAngle > 90:
             self._arcType = arc.arcTypes[1]
         elif 270 >= self._arcAngle > 180:
             self._arcType = arc.arcTypes[2]
         elif 360 > self._arcAngle > 270:
@@ -567,24 +577,30 @@
     @property
     def start(self):
         return self._start
 
     @start.setter
     def start(self, point: QPoint):
         assert isinstance(point, QPoint)
+        self.prepareGeometryChange()
         self._start = self.snapToGrid(point, self.gridTuple)
 
     @property
     def end(self):
         return self._end
 
     @end.setter
     def end(self, point: QPoint):
         assert isinstance(point, QPoint)
-        self._end = self.snapToGrid(point, self.gridTuple)
+        self.prepareGeometryChange()
+        self._end = point
+        self._arcLine = QLineF(self._start, self._end)
+        self._arcAngle = self._arcLine.angle()
+        self.findAngle()
+        self._rect = QRectF(self._start, self._end).normalized()
 
     @property
     def width(self):
         return self._width
 
     @width.setter
     def width(self, width):
@@ -600,42 +616,42 @@
     def height(self, height):
         self._height = height
         self.prepareGeometryChange()
         self.rect.setHeight(self._height)
 
     def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
         super().mousePressEvent(event)
-        eventPos = self.snapToGrid(event.pos(), self.gridTuple)
+        eventPos = event.pos().toPoint()
         if self._stretch:
             self.setFlag(QGraphicsItem.ItemIsMovable, False)
             if eventPos.x() == self.snapToBase(self._rect.left(),
                                                self.gridTuple[0]):
-                if (self._rect.top() <= eventPos.y() <= self._rect.bottom()):
+                if self._rect.top() <= eventPos.y() <= self._rect.bottom():
                     self.setCursor(Qt.SizeHorCursor)
                     self._stretchSide = arc.sides[0]
             elif eventPos.x() == self.snapToBase(self._rect.right(),
                                                  self.gridTuple[0]):
-                if (self._rect.top() <= eventPos.y() <= self._rect.bottom()):
+                if self._rect.top() <= eventPos.y() <= self._rect.bottom():
                     self.setCursor(Qt.SizeHorCursor)
                     self._stretchSide = arc.sides[1]
             elif eventPos.y() == self.snapToBase(self._rect.top(),
                                                  self.gridTuple[1]):
-                if (self._rect.left() <= eventPos.x() <= self._rect.right()):
+                if self._rect.left() <= eventPos.x() <= self._rect.right():
                     self.setCursor(Qt.SizeVerCursor)
                     self._stretchSide = arc.sides[2]
             elif eventPos.y() == self.snapToBase(self._rect.bottom(),
                                                  self.gridTuple[1]):
-                if (self._rect.left() <= eventPos.x() <= self._rect.right()):
+                if self._rect.left() <= eventPos.x() <= self._rect.right():
                     self.setCursor(Qt.SizeVerCursor)
                     self._stretchSide = arc.sides[3]
 
     def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
         super().mouseMoveEvent(event)
 
-        eventPos = self.snapToGrid(event.pos(), self.gridTuple)
+        eventPos = event.pos().toPoint()
         if self._stretch:
             self.prepareGeometryChange()
             if self._stretchSide == arc.sides[0]:
                 self.setCursor(Qt.SizeHorCursor)
                 self._rect.setLeft(eventPos.x())
             elif self._stretchSide == arc.sides[1]:
                 self.setCursor(Qt.SizeHorCursor)
@@ -677,15 +693,16 @@
             self._rect = QRectF(self._start, self._end).normalized()
 
 
 class line(shape):
     """
     line class definition for symbol drawing.
     """
-    stretchSides = ['start', 'end']
+
+    stretchSides = ["start", "end"]
 
     def __init__(self, start: QPoint, end: QPoint, pen: QPen, grid: tuple, ):
         super().__init__(pen, grid)
         self._end = end
         self._start = start
         self._pen = pen
         self._stretch = False
@@ -698,14 +715,19 @@
         return self._rect.adjusted(-2, -2, 2, 2)
 
     def shape(self):
         path = QPainterPath()
         path.addRect(self._rect.adjusted(-2, -2, 2, 2))
         return path
 
+    def shape(self):
+        path = QPainterPath()
+        path.addRect(self._rect.adjusted(-2, -2, 2, 2))
+        return path
+
     def paint(self, painter, option, widget):
         if self.isSelected():
             painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
             if self._stretch:
                 painter.setPen(QPen(Qt.red, 2, Qt.SolidLine))
                 if self._stretchSide == line.stretchSides[0]:
                     painter.drawEllipse(self._start, self.gridTuple[0],
@@ -733,24 +755,26 @@
         return self._start
 
     @start.setter
     def start(self, start: QPoint):
         self.prepareGeometryChange()
         self._start = start
         self._line = QLine(self._start, self._end)
+        self._rect = QRect(self._start, self._end).normalized()
 
     @property
     def end(self):
         return self._end
 
     @end.setter
     def end(self, end: QPoint):
         self.prepareGeometryChange()
         self._end = end
         self._line = QLine(self._start, self._end)
+        self._rect = QRect(self._start, self._end).normalized()
 
     @property
     def pen(self):
         return self._pen
 
     @pen.setter
     def pen(self, pen: QPen):
@@ -776,47 +800,48 @@
         return math.sqrt((self.start.x() - self._end.x()) ** 2 + (
                     self.start.y() - self._end.y()) ** 2)
 
     def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
         super().mousePressEvent(event)
         if self.isSelected() and self._stretch:
             self.setFlag(QGraphicsItem.ItemIsMovable, False)
-            eventPos = self.snapToGrid(event.pos(), self._gridTuple)
+            eventPos = event.pos().toPoint()
             if eventPos == self.start:
                 self._stretchSide = line.stretchSides[0]
             elif eventPos == self._end:
                 self._stretchSide = line.stretchSides[1]
 
     def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        eventPos = self.snapToGrid(event.pos(), self._gridTuple)
+        eventPos = event.pos().toPoint()
         if self._stretchSide == line.stretchSides[0]:
             self.prepareGeometryChange()
             self.start = eventPos
             self._line = QLine(self.start, self._end)
             self._rect = QRect(self.start, self._end).normalized()
         elif self._stretchSide == line.stretchSides[1]:
             self.prepareGeometryChange()
             self._end = eventPos
             self._line = QLine(self.start, self._end)
             self._rect = QRect(self.start, self._end).normalized()
 
         super().mouseMoveEvent(event)
 
     def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseReleaseEvent(event)
         self._stretch = False
         self.setFlag(QGraphicsItem.ItemIsMovable, True)
         self.setFlag(QGraphicsItem.ItemIsSelectable, True)
         self._stretchSide = ""
-        super().mouseReleaseEvent(event)
 
 
 class pin(shape):
     """
     symbol pin class definition for symbol drawing.
     """
+
     pinDirs = ["Input", "Output", "Inout"]
     pinTypes = ["Signal", "Ground", "Power", "Clock", "Digital", "Analog"]
 
     def __init__(self, start: QPoint, pen: QPen, pinName: str = "",
                  pinDir: str = pinDirs[0], pinType: str = pinTypes[0],
                  grid: tuple = (10, 10), ):
         super().__init__(pen, grid)
@@ -824,14 +849,17 @@
         self._start = start  # centre of pin
         self._pinName = pinName
         self._pinDir = pinDir
         self._pinType = pinType
         self._connected = False  # True if the pin is connected to a net.
         self._rect = QRect(self._start.x() - 5, self._start.y() - 5, 10, 10)
 
+    def __repr__(self):
+        return f"pin: {self._pinName} {self.mapToScene(self._start)}"
+
     def boundingRect(self):
         return self._rect  #
 
     def paint(self, painter, option, widget):
         painter.setPen(self._pen)
         painter.setBrush(self._pen.color())
         painter.drawRect(self._rect)
@@ -895,21 +923,22 @@
                             gridTuple)
 
 
 class text(shape):
     """
     This class is for text annotations on symbol or schematics.
     """
+
     textAlignments = ["Left", "Center", "Right"]
     textOrients = ["R0", "R90", "R180", "R270"]
 
     def __init__(self, start: QPoint, pen: QPen, textContent: str = "",
-                 grid: tuple = (10, 10), fontFamily='Helvetica',
-                 fontStyle='Regular', textHeight: str = "12",
-                 textAlign: str = "Left", textOrient: str = "R0"):
+                 grid: tuple = (10, 10), fontFamily="Helvetica",
+                 fontStyle="Regular", textHeight: str = "12",
+                 textAlign: str = "Left", textOrient: str = "R0", ):
         super().__init__(pen, grid)
 
         self._start = start
         self._pen = pen
         self._textContent = textContent
         self._textHeight = textHeight
         self._textAlign = textAlign
@@ -938,15 +967,15 @@
                                                Qt.AlignmentFlag.AlignCenter,
                                                self._textContent)
         elif self._textAlign == text.textAlignments[2]:
             self._rect = self._fm.boundingRect(QRect(0, 0, 400, 400),
                                                Qt.AlignmentFlag.AlignRight,
                                                self._textContent)
         return QRect(self._start.x(), self._start.y() - self._rect.height(),
-                     self._rect.width(), self._rect.height())
+                     self._rect.width(), self._rect.height(), )
 
     def paint(self, painter, option, widget):
         painter.setFont(self._textFont)
         if self.isSelected():
             painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
             painter.drawRect(self.boundingRect())
         else:
@@ -967,55 +996,55 @@
         return self._textContent
 
     @textContent.setter
     def textContent(self, inputText: str):
         if isinstance(inputText, str):
             self._textContent = inputText
         else:
-            self.scene().logger.error(f'Not a string: {inputText}')
+            self.scene().logger.error(f"Not a string: {inputText}")
 
     @property
     def fontFamily(self) -> str:
         return self._textFont.family()
 
     @fontFamily.setter
     def fontFamily(self, familyName):
         fontFamilies = QFontDatabase.families(QFontDatabase.Latin)
         fixedFamilies = [family for family in fontFamilies if
                          QFontDatabase.isFixedPitch(family)]
         if familyName in fixedFamilies:
             self._textFont.setFamily(familyName)
         else:
-            self.scene().logger.error(f'Not a valid font name: {familyName}')
+            self.scene().logger.error(f"Not a valid font name: {familyName}")
 
     @property
     def fontStyle(self) -> str:
         return self._textFont.styleName()
 
     @fontStyle.setter
     def fontStyle(self, value: str):
         if value in QFontDatabase.styles(self._textFont.family()):
             self._textFont.setStyleName(value)
         else:
-            self.scene().logger.error(f'Not a valid font style: {value}')
+            self.scene().logger.error(f"Not a valid font style: {value}")
 
     @property
     def textHeight(self) -> int:
         return self._textHeight
 
     @textHeight.setter
     def textHeight(self, value: int):
         fontSizes = [str(size) for size in
                      QFontDatabase.pointSizes(self._textFont.family(),
                                               self._textFont.styleName())]
         if value in fontSizes:
             self._textHeight = value
         else:
-            self.scene().logger.error(f'Not a valid font height: {value}')
-            self.scene().logger.warning(f'Valid font heights are: {fontSizes}')
+            self.scene().logger.error(f"Not a valid font height: {value}")
+            self.scene().logger.warning(f"Valid font heights are: {fontSizes}")
 
     @property
     def textFont(self) -> QFont:
         return self._textFont
 
     @textFont.setter
     def textFont(self, value: QFont):
@@ -1028,51 +1057,52 @@
 
     @textAlignment.setter
     def textAlignment(self, value):
         if value in text.textAlignments:
             self._textAlign = value
         else:
             self.scene().logger.error(
-                f'Not a valid text alignment value: {value}')
+                f"Not a valid text alignment value: {value}")
 
     @property
     def textOrient(self):
         return self._textOrient
 
     @textOrient.setter
     def textOrient(self, value):
         if value in text.textOrients:
             self._textOrient = value
         else:
-            self.scene().logger.error(f'Not a valid text orientation: {value}')
+            self.scene().logger.error(f"Not a valid text orientation: {value}")
 
 
 class label(shape):
     """
     label: text class definition for symbol drawing.
     labelText is what is shown on the symbol in a schematic
     """
 
     labelAlignments = ["Left", "Center", "Right"]
     labelOrients = ["R0", "R90", "R180", "R270", "MX", "MX90", "MY", "MY90"]
     labelUses = ["Normal", "Instance", "Pin", "Device", "Annotation"]
     labelTypes = ["Normal", "NLPLabel", "PyLabel"]
     predefinedLabels = ["[@libName]", "[@cellName]", "[@viewName]", "[@instName]",
-                        "[@modelName]"]
+                        "[@modelName]", "[@elementNum]"]
 
     def __init__(self, start: QPoint, pen: QPen, labelDefinition: str = "",
                  grid: tuple = (10, 10), labelType: str = "Normal",
                  labelHeight: str = "12", labelAlign: str = "Left",
                  labelOrient: str = "R0", labelUse: str = "Normal", ):
         super().__init__(pen, grid)
         self._start = start  # top left corner
         self._pen = pen
-        self._labelDefinition = labelDefinition  # label definition
+        self._labelDefinition = labelDefinition  # label definition is what is
+        # entered in the symbol editor
         self._labelName = None  # label Name
-        self._labelValue = "?"  # label value
+        self._labelValue = None  # label value
         self._labelText = None  # Displayed label
         self._labelHeight = labelHeight
         self._labelAlign = labelAlign
         self._labelOrient = labelOrient
         self._labelUse = labelUse
         self._labelType = labelType
         self._labelFont = QFont("Arial")
@@ -1081,17 +1111,26 @@
         self._labelVisible: bool = False
         self._labelValueSet: bool = False
         # labels are visible by default
         self.setOpacity(1)
         self._fm = QFontMetrics(self._labelFont)
         self._rect = self._fm.boundingRect(self._labelDefinition)
 
+    def __repr__(self):
+        return f"label: {self._labelText} for {self._labelDefinition} at {self._start}, " \
+               f"value =  {self._labelValue}"
+
     def boundingRect(self):
         return QRect(self._start.x(), self._start.y(), self._rect.width(),
-                     self._rect.height())  #
+                     self._rect.height()).normalized().adjusted(0, 0, 0,5)  #
+
+    def shape(self) -> QPainterPath:
+        path = QPainterPath()
+        path.addRect(self.boundingRect())
+        return path
 
     def paint(self, painter, option, widget):
         # self._rect = self.fm.boundingRect(self.labelName)
         self._labelFont.setPointSize(int(self._labelHeight))
         painter.setFont(self._labelFont)
         if self.isSelected():
             painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
@@ -1142,32 +1181,35 @@
         return self.boundingRect().height()
 
     @property
     def labelName(self):
         return self._labelName
 
     @labelName.setter
-    def labelName(self, labelName):
+    def labelName(self, labelName: str):
         self._labelName = labelName
 
     @property
     def labelDefinition(self):
         return self._labelDefinition
 
     @labelDefinition.setter
-    def labelDefinition(self, labelDefinition):
-        self._labelDefinition = labelDefinition
+    def labelDefinition(self, labelDefinition: str):
+        if isinstance(labelDefinition, str):
+            self._labelDefinition = labelDefinition.strip()
 
     @property
     def labelValue(self):
         return self._labelValue
 
     @labelValue.setter
     def labelValue(self, labelValue):
         self._labelValue = labelValue
+        self._labelValueSet = True
+        # self.labelDefs()
 
     @property
     def labelValueSet(self) -> bool:
         return self._labelValueSet
 
     @labelValueSet.setter
     def labelValueSet(self, value: bool):
@@ -1185,40 +1227,40 @@
     @property
     def labelText(self):
         return self._labelText
 
     @labelText.setter
     def labelText(self, labelText):
         self._labelText = labelText
-        self._rect = self._fm.boundingRect(self._labelText)
+        self._rect = self._fm.boundingRect(self._labelText).normalized().adjusted(0, 0, 0, 5)
 
     def objName(self):
         return "LABEL"
 
     @property
     def labelType(self):
         return self._labelType
 
     @labelType.setter
     def labelType(self, labelType):
         if labelType in self.labelTypes:
             self._labelType = labelType
-        else:
+        elif self.scene():
             self.scene().logger.error("Invalid label type")
 
     @property
     def labelAlign(self):
         return self._labelAlign
 
     @labelAlign.setter
     def labelAlign(self, labelAlignment):
         if labelAlignment in self.labelAlignments:
             self._labelAlign = labelAlignment
-        else:
-            print("Invalid label alignment")
+        elif self.scene():
+            self.scene().logger.error("Invalid label alignment")
 
     @property
     def labelOrient(self):
         return self._labelOrient
 
     @labelOrient.setter
     def labelOrient(self, labelOrient):
@@ -1231,16 +1273,16 @@
     def labelUse(self):
         return self._labelUse
 
     @labelUse.setter
     def labelUse(self, labelUse):
         if labelUse in self.labelUses:
             self._labelUse = labelUse
-        else:
-            print("Invalid label use")
+        elif self.scene():
+            self.scene().logger.error("Invalid label use")
 
     @property
     def labelFont(self):
         return self._labelFont
 
     @labelFont.setter
     def labelFont(self, labelFont: QFont):
@@ -1259,123 +1301,102 @@
         else:
             self.setOpacity(0.001)
             self._labelVisible = False
 
     def moveBy(self, delta: QPoint):
         self._start += delta
 
-    def setLabelName(self):
-        """
-        Creates a label name from label definition, such as [@w:w=%:] becomes
-        w. Label names are used in instance.labelDict to identify each label.
-        """
-        # if label type is normal, label name is the label definition and also label text
-        if self._labelType == "Normal":
-            self._labelName = self._labelDefinition
-
-        elif self._labelType == "NLPLabel":
-            # if label type is NLPLabel, it is a bit more complicated.
-            # here we only define label names to display when symbol is instantiated.
-            try:
-                if self._labelDefinition.strip() == "[@cellName]":
-                    self._labelName = "cellName"
-                elif self.labelDefinition.strip() == "[@instName]":
-                    self._labelName = "instName"
-                elif self._labelDefinition.strip() == "[@libName]":
-                    self._labelName = "libName"
-                elif self._labelDefinition.strip() == "[@viewName]":
-                    self._labelName = "viewName"
-                elif self._labelDefinition.strip() == "[@modelName]":
-                    self._labelName = "modelName"
-                elif self._labelDefinition.strip() == "[@elementNum]":
-                    self._labelName = "elementNum"
-                else:
-                    if self._labelDefinition[:2] == '[@' and \
-                            self._labelDefinition[
-                                -1] == "]":  # check if it is a correct start and end
-                        self._labelName = \
-                            self._labelDefinition.lstrip('[@').rstrip(']').rstrip(
-                                ':').split(':')[0].strip()
-                    else:
-                        self.scene().logger.error('Error in label definition.')
-            except Exception as e:
-                print(e)
-        elif self._labelType == "PyLabel":
-            self._labelName = \
-                [string.strip() for string in self.labelDefinition.split("=")][0]
-
     def labelDefs(self):
         """
-        This method will create label name and text from label definition. It
-        should be only run during the label initiation.
+        This method will create label name, value andtext from label
+        definition. It should be run label is defined or redefined.
         """
+        self.prepareGeometryChange()
         if self._labelType == label.labelTypes[0]:
+            self._labelName = self._labelDefinition
             self._labelText = self._labelDefinition
-        elif self._labelType == label.labelTypes[1]:
+            self._labelValue = None
+            self._labelValueSet = True
+        elif self.labelType == label.labelTypes[1]:
             try:
-                match self._labelDefinition:
-                    case "[@cellName]":
-                        self._labelValue = self.parentItem().cellName
-                        self._labelText = self._labelValue
-                    case "[@instName]":
-                        self._labelValue = f"I{self.parentItem().counter}"
-                        self._labelText = self._labelValue
-                    case "[@libName]":
-                        self._labelValue = self.parentItem().libraryName
-                        self._labelText = self._labelValue
-                    case "[@viewName]":
-                        self._labelValue = self.parentItem().viewName
-                        self._labelText = self._labelValue
-                    case "[@modelName]":
-                        if self.parentItem().attr.get("ModelName"):
-                            self._labelValue = self.parentItem().attr["modelName"]
-                        else:
-                            self._labelValue = ""
-                        self._labelText = self._labelValue
-                    case "[@elementNum]":
-                        self._labelValue = f'{self.parentItem().counter}'
-                        self._labelText = self._labelValue
-                    case other:
-                        labelFields = self._labelDefinition.lstrip('[@').rstrip(
-                            ']').rstrip(':').split(':')
-                        match len(labelFields):
-                            case 1:
-                                self._labelText = self._labelValue
-                            case 2:
-                                self._labelText = labelFields[1].strip().replace(
-                                    '%', self._labelValue)
-                            case 3:
-                                tempLabelValue = \
-                                    labelFields[2].strip().split('=')[-1].split()[
-                                        -1]
-                                if self._labelValueSet:
-                                    self._labelText = labelFields[2].replace(
-                                        tempLabelValue, self._labelValue)
-                                else:
-                                    self._labelText = labelFields[2]
-                                    self._labelValue = tempLabelValue
+                if self._labelDefinition in label.predefinedLabels:
+                    self._labelValueSet = True
+                    match self.labelDefinition:
+                        case "[@cellName]":
+                            self._labelName = "cellName"
+                            self._labelValue = self.parentItem().cellName
+                            self._labelText = self._labelValue
+                        case "[@instName]":
+                            self._labelName = "instName"
+                            self._labelValue = f"I{self.parentItem().counter}"
+                            self._labelText = self._labelValue
+                        case "[@libName]":
+                            self._labelName = "libName"
+                            self._labelValue = self.parentItem().libraryName
+                            self._labelText = self._labelValue
+                        case "[@viewName]":
+                            self._viewName = "viewName"
+                            self._labelValue = self.parentItem().viewName
+                            self._labelText = self._labelValue
+                        case "[@modelName]":
+                            self._labelName = "modelName"
+                            self._labelValue = self.parentItem().attr.get(
+                                "modelName", "")
+                            self._labelText = self._labelValue
+                        case "[@elementNum]":
+                            self._labelName = "elementNum"
+                            self._labelValue = f"{self.parentItem().counter}"
+                            self._labelText = self._labelValue
+                else:
+                    labelFields = (
+                        self._labelDefinition.lstrip("[@").rstrip("]").rstrip(
+                            ":").split(":"))
+                    self._labelName = labelFields[0].strip()
+                    match len(labelFields):
+                        case 1:
+                            if not self._labelValueSet:
+                                self._labelValue = "?"
+                            self._labelText = self._labelValue
+                        case 2:
+                            if self._labelValueSet:
+                                self._labelText = (
+                                    labelFields[1].strip().replace("%",
+                                                                   self._labelValue))
+                            else:
+                                self._labelValue = "?"
+                        case 3:
+                            tempLabelValue = (
+                                labelFields[2].strip().split("=")[-1].split()[-1])
+                            if self.labelValueSet:
+                                self._labelText = labelFields[2].replace(
+                                    tempLabelValue, self._labelValue)
+                            else:
+                                self._labelText = labelFields[2]
+                                self._labelValue = tempLabelValue
+
             except Exception as e:
-                print(e)
+                if self.scene():
+                    self.scene().logger.error(e)
         elif self._labelType == label.labelTypes[2]:  # pyLabel
             try:
-                labelFields = self._labelDefinition.strip().split('=')
+                labelFields = self._labelDefinition.strip().split("=")
                 self._labelName = labelFields[0].strip()
                 labelFunction = labelFields[1].strip()
                 # pass the PDK callback class named with "cellName" the labels
-                # dictionary of instance.
-                expression = f'cb.{self.parentItem().cellName}(self.parentItem(' \
-                             f').labels).{labelFunction}'
+                # dictionary of instance.w
+                expression = (
+                    f"cb.{self.parentItem().cellName}(self.parentItem().labels).{labelFunction}")
                 self._labelValue = Quantity(eval(expression)).render(prec=3)
-                self._labelText = f'{self._labelName}={self._labelValue}'
+                self._labelText = f"{self._labelName}={self._labelValue}"
             except Exception as e:
-                print(e)
+                if self.scene():
+                    self.scene().logger.error(e)
 
 
 class symbolShape(shape):
-
     def __init__(self, pen: QPen, gridTuple: tuple, shapes: list, attr: dict):
         super().__init__(pen, gridTuple)
         assert shapes is not None  # must not be an empty list
         self.shapes = shapes  # list of shapes in the symbol
         self.attr = attr  # parameters common to all instances of symbol
         self._counter = 0  # item's number on schematic
         self._libraryName = ""
@@ -1386,14 +1407,15 @@
         # self._simViewName = None
         self._angle = 0.0
         self._drawings = list()
         self._labels = dict()  # dict of labels
         self._pins = dict()  # dict of pins
         self.pinLocations = dict()  # pinName: pinRect
         self.pinNetMap = dict()  # pinName: netName
+        self.pinNetTupleList = list()  # list of pinNetTuple
         for item in self.shapes:
             item.setFlag(QGraphicsItem.ItemIsSelectable, False)
             item.setFlag(QGraphicsItem.ItemStacksBehindParent, True)
             item.setParentItem(self)
             if type(item) is pin:
                 self._pins[item.pinName] = item
             elif type(item) is label:
@@ -1403,14 +1425,20 @@
         self.setFiltersChildEvents(True)
         self.setHandlesChildEvents(True)
         self.setFlag(QGraphicsItem.ItemContainsChildrenInShape, True)
         self.borderRect = self._drawings[0].sceneBoundingRect()
         if self._drawings[1:]:
             for draw in self._drawings[1:]:
                 self.borderRect = self.borderRect.united(draw.sceneBoundingRect())
+        self.dashLines = dict()
+
+    def __repr__(self):
+        return (
+            f"symbolShape(name={self.cellName}, scene position= {self.scenePos()}, "
+            f"pins = {self.pins}, labels = {self.labels}, ")
 
     def paint(self, painter, option, widget):
         if self.isSelected():
             painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
             painter.drawRect(self.borderRect)
 
     def boundingRect(self):
@@ -1422,14 +1450,61 @@
                 return False
             else:
                 super().sceneEvent(event)
                 return True
         except AttributeError:
             return False
 
+    def itemChange(self, change, value):
+
+        if self.scene() and change == QGraphicsItem.ItemPositionHasChanged:
+            # item's position has changed
+            # do something here
+            for item in self.pinNetTupleList:
+                if item.start == 1:
+                    item.net.start = item.pin.mapToScene(item.pin.start)
+                elif item.start == 0:
+                    item.net.end = item.pin.mapToScene(item.pin.start)
+
+        return super().itemChange(change, value)
+
+    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        self.pinNetTupleList = list()
+        # create a named tuple to record whether the pin is located at the start or at
+        # the end of the net.
+        pins = [item for item in self.pins.values()]
+        for pinItem in pins:
+            for pinNet in self.scene().items(pinItem.sceneBoundingRect().adjusted(
+                    -2, -2, 2, 2), Qt.IntersectsItemShape):
+                if isinstance(pinNet, net.schematicNet):
+                    if pinItem.sceneBoundingRect().adjusted(-2, -2, 2, 2).contains(
+                            pinNet.mapToScene(pinNet.start)):
+                        self.pinNetTupleList.append(ddef.pinNetTuple(pinItem, pinNet, 1))
+                    elif pinItem.sceneBoundingRect().adjusted(-2, -2, 2, 2).contains(
+                            pinNet.mapToScene(pinNet.end)):
+                        self.pinNetTupleList.append(ddef.pinNetTuple(pinItem, pinNet, 0))
+        for item in self.pinNetTupleList:
+            pinSceneLoc = item.pin.mapToScene(item.pin.start)
+            if item.start == 1:
+                item.net.start = pinSceneLoc
+            else:
+                item.net.end = pinSceneLoc
+            item.net.pen = self.scene().otherPen
+        super().mousePressEvent(event)
+
+    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseReleaseEvent(event)
+
+        for item in self.pinNetTupleList:
+            lines = self.scene().addWires(item.net.start, self.scene().wirePen)
+            self.scene().extendWires(lines,item.net.start,item.net.end)
+            self.scene().pruneWires(lines,self.scene().wirePen)
+            self.scene().removeItem(item.net)
+
+
     @property
     def libraryName(self):
         return self._libraryName
 
     @libraryName.setter
     def libraryName(self, value):
         self._libraryName = value
@@ -1452,15 +1527,22 @@
 
     @property
     def instanceName(self):
         return self._instanceName
 
     @instanceName.setter
     def instanceName(self, value: str):
+        '''
+        If instance name is changed and [@instName] label exists, change it too.
+        '''
         self._instanceName = value
+        if self.labels.get('instanceName', None):
+            self.labels['instanceName'].labelValue = value
+            self.labels['instanceName'].labelValueSet = True
+            self.labels['instanceName'].update()
 
     @property
     def counter(self) -> int:
         return self._counter
 
     @counter.setter
     def counter(self, value: int):
@@ -1474,119 +1556,141 @@
     @angle.setter
     def angle(self, value: float):
         self.setRotation(value)
         self._angle = value
 
     @property
     def labels(self):
-        return self._labels
-
-    # labels setter works a bit differently
-    @labels.setter
-    def labels(self, item: label):
-        assert isinstance(item, label)
-        self._labels[item.labelName] = item
+        return self._labels  # dictionary
 
     @property
     def pins(self):
         return self._pins
 
-    @pins.setter
-    def pins(self, item: pin):
-        assert isinstance(item, pin)
-        self._pins[item.pinName] = item
-
-    def createNetlistLine(self):
-        """
-        Create a netlist line from a nlp device format line.
-        """
-        try:
-            nlpDeviceFormatLine = self.attr["NLPDeviceFormat"].strip()
-            nlpDeviceFormatLine.replace("[@instName]", f'{self.instanceName}')
-            for labelItem in self.labels.values():
-                if labelItem.labelDefinition in nlpDeviceFormatLine:
-                    nlpDeviceFormatLine = nlpDeviceFormatLine.replace(
-                        labelItem.labelDefinition, labelItem.labelText)
-            for pinName, netName in self.pinNetMap.items():
-                if pinName in nlpDeviceFormatLine:
-                    nlpDeviceFormatLine = nlpDeviceFormatLine.replace(
-                        f'[|{pinName}:%]', netName)
-            return nlpDeviceFormatLine
-        except KeyError:
-            self.scene().parent.parent.logger.error(
-                f'Netlist line is not defined for '
-                f'{self.instanceName}')
-            # if there is no NLPDeviceFormat line, create a warning line
-            return f"*Netlist line is not defined for symbol of {self.instanceName}"  # return empty string
+    @property
+    def drawings(self):
+        return self._drawings
 
 
 class schematicPin(shape):
-    '''
+    """
     schematic pin class.
-    '''
+    """
+
     pinDirs = ["Input", "Output", "Inout"]
     pinTypes = ["Signal", "Ground", "Power", "Clock", "Digital", "Analog"]
 
     def __init__(self, start: QPoint, pen: QPen, pinName, pinDir, pinType,
                  gridTuple: tuple):
         super().__init__(pen, gridTuple)
         self._start = start
         self._pinName = pinName
         self._pinDir = pinDir
         self._pinType = pinType
+        self._netTupleSet = set()
+
+    def __repr__(self):
+        return f"schematicPin({self._start}, {self._pen}, {self._pinName}, {self._pinDir}, {self._pinType})"
 
     def paint(self, painter, option, widget):
 
         painter.setPen(self._pen)
         painter.setBrush(self._pen.color())
         painter.setFont(QFont("Arial", 12))
         match self.pinDir:
             case "Input":
                 painter.drawPolygon(
                     [QPoint(self._start.x() - 10, self._start.y() - 10),
                      QPoint(self._start.x() + 10, self._start.y() - 10),
                      QPoint(self._start.x() + 20, self._start.y()),
                      QPoint(self._start.x() + 10, self._start.y() + 10),
-                     QPoint(self._start.x() - 10, self._start.y() + 10)])
+                     QPoint(self._start.x() - 10, self._start.y() + 10), ])
             case "Output":
                 painter.drawPolygon(
                     [QPoint(self._start.x() - 20, self._start.y()),
                      QPoint(self._start.x() - 10, self._start.y() - 10),
                      QPoint(self._start.x() + 10, self._start.y() - 10),
                      QPoint(self._start.x() + 10, self._start.y() + 10),
-                     QPoint(self._start.x() - 10, self._start.y() + 10)])
+                     QPoint(self._start.x() - 10, self._start.y() + 10), ])
             case "Inout":
                 painter.drawPolygon(
                     [QPoint(self._start.x() - 20, self._start.y()),
                      QPoint(self._start.x() - 10, self._start.y() - 10),
                      QPoint(self._start.x() + 10, self._start.y() - 10),
                      QPoint(self._start.x() + 20, self._start.y()),
                      QPoint(self._start.x() + 10, self._start.y() + 10),
-                     QPoint(self._start.x() - 10, self._start.y() + 10)])
+                     QPoint(self._start.x() - 10, self._start.y() + 10), ])
         painter.drawText(self._start.x(), self._start.y() - 20, self.pinName)
         if self.isSelected():
             painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
             # painter.setBrush(Qt.yellow)
             painter.drawRect(
                 QRect.span(QPoint(self._start.x() - 10, self._start.y() - 10),
-                           QPoint(self._start.x() + 10, self._start.y() + 10)))
+                           QPoint(self._start.x() + 10, self._start.y() + 10), ))
 
     def boundingRect(self):
         return QRect(self._start.x() - 10, self._start.y() - 10, 30, 20).adjusted(
             -5, -10, 5, 5)
 
     def sceneEvent(self, event):
         if self.scene().drawWire:
             return False
         else:
             super().sceneEvent(event)
             return True
+    #
+    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mousePressEvent(event)
+        # create a named tuple to record whether the pin is located at the start or at
+        # the end of the net.
 
-    def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        self.setPos(event.scenePos() - event.buttonDownPos(Qt.LeftButton))
+        for pinNet in self.scene().items(self.sceneBoundingRect().adjusted(
+                -2, -2, 2, 2), Qt.IntersectsItemShape):
+            if isinstance(pinNet, net.schematicNet):
+                if self.sceneBoundingRect().adjusted(-2, -2, 2, 2).contains(
+                        pinNet.mapToScene(pinNet.start)):
+                    self._netTupleSet.add(ddef.netTuple(pinNet, 1))
+                elif self.sceneBoundingRect().adjusted(-2, -2, 2, 2).contains(
+                        pinNet.mapToScene(pinNet.end)):
+                    self._netTupleSet.addd(ddef.netTuple(pinNet, 0))
+        for item in self._netTupleSet:
+            pinSceneLoc = self.mapToScene(self.start)
+            if item.start == 1:
+                item.net.start = pinSceneLoc
+            else:
+                item.net.end = pinSceneLoc
+            item.net.pen = self.scene().otherPen
+        super().mousePressEvent(event)
+    #
+    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseReleaseEvent(event)
+
+        for item in self._netTupleSet:
+            lines = self.scene().addWires(item.net.start, self.scene().wirePen)
+            self.scene().extendWires(lines,item.net.start,item.net.end)
+            self.scene().pruneWires(lines,self.scene().wirePen)
+            self.scene().removeItem(item.net)
+        self._netTupleSet = set()
+
+    def itemChange(self, change, value):
+
+
+        if self.scene() and change == QGraphicsItem.ItemPositionHasChanged:
+            # item's position has changed
+            # do something here
+            for item in self._netTupleSet:
+                if item.start == 1:
+                    item.net.start = self.mapToScene(self.start)
+                elif item.start == 0:
+                    item.net.end = self.mapToScene(self.start)
+        return super().itemChange(change, value)
+
+    # def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+    #     super().mouseMoveEvent(event)
+    #     self.setPos(event.scenePos() - event.buttonDownPos(Qt.LeftButton))
 
     def toSymbolPin(self, start: QPoint, pen: QPen, gridTuple: tuple):
         return pin(start, pen, self.pinName, self.pinDir, self.pinType, gridTuple)
 
     @property
     def start(self):
         return self._start
```

### Comparing `revolution-eda-0.4.1/fileio/__init__.py` & `revolution-eda-0.5.0/revedaEditor/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.4.1/fileio/loadJSON.py` & `revolution-eda-0.5.0/revedaEditor/fileio/loadJSON.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,224 +1,222 @@
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-# Load symbol and maybe later schematic from json file.
-# import pathlib
-
-import json
-
-from PySide6.QtCore import (QPoint, Qt, )  # QtCore
-from PySide6.QtGui import (QColor, QPen, )
-
-import common.shape as shp
-import fileio.symbolEncoder as se
-import common.net as net
-import common.pens as pens
-
-
-def createSymbolItems(item, gridTuple):
-    """
-    Create symbol items from json file.
-    """
-    if item["type"] == "rect":
-        return createRectItem(item, gridTuple)
-    elif item["type"] == "circle":
-        return createCircleItem(item, gridTuple)
-    elif item["type"] == "arc":
-        return createArcItem(item, gridTuple)
-    elif item["type"] == "line":
-        return createLineItem(item, gridTuple)
-    elif item["type"] == "pin":
-        return createPinItem(item, gridTuple)
-    elif item["type"] == "label":
-        return createLabelItem(item, gridTuple)
-
-
-def createRectItem(item, gridTuple):
-    """
-    Create symbol items from json file.
-    """
-    start = QPoint(item["rect"][0], item["rect"][1])
-    end = QPoint(item["rect"][2], item["rect"][3])
-    pen = pens.pen.returnPen(item['pen'])
-    rect = shp.rectangle(start, end, pen,
-                         gridTuple)  # note that we are using grid values for scene
-    rect.setPos(QPoint(item["loc"][0], item["loc"][1]), )
-    rect.angle = item["ang"]
-    return rect
-
-
-def createCircleItem(item, gridTuple):
-    centre = QPoint(item["cen"][0], item["cen"][1])
-    end = QPoint(item["end"][0], item["end"][1])
-    pen = pens.pen.returnPen(item['pen'])
-    circle = shp.circle(centre, end, pen,
-                        gridTuple)  # note that we are using grid values for scene
-    circle.setPos(QPoint(item["loc"][0], item["loc"][1]), )
-    circle.angle = item["ang"]
-    return circle
-
-
-def createArcItem(item, gridTuple):
-    start = QPoint(item["st"][0], item["st"][1])
-    end = QPoint(item["end"][0], item["end"][1])
-    pen = pens.pen.returnPen(item['pen'])
-    arc = shp.arc(start, end, pen,
-                  gridTuple)  # note that we are using grid values for scene
-    arc.setPos(QPoint(item["loc"][0], item["loc"][1]))
-    arc.angle = item["ang"]
-    return arc
-
-
-def createLineItem(item, gridTuple):
-    start = QPoint(item["st"][0], item["st"][1])
-    end = QPoint(item["end"][0], item["end"][1])
-    pen = pens.pen.returnPen(item['pen'])
-    line = shp.line(start, end, pen, gridTuple)
-    line.setPos(QPoint(item["loc"][0], item["loc"][1]))
-    line.angle = item["ang"]
-    return line
-
-
-def createPinItem(item, gridTuple):
-    start = QPoint(item["st"][0], item["st"][1])
-    pen = pens.pen.returnPen(item['pen'])
-    pin = shp.pin(start, pen, item["nam"], item["pd"], item["pt"], gridTuple, )
-    pin.setPos(QPoint(item["loc"][0], item["loc"][1]))
-    pin.angle = item["ang"]
-    return pin
-
-
-def createLabelItem(item, gridTuple):
-    start = QPoint(item["st"][0], item["st"][1])
-    pen = pens.pen.returnPen(item['pen'])
-    label = shp.label(start, pen, item["def"], gridTuple, item["lt"], item["ht"],
-                      item["al"], item["or"], item["use"], )
-    label.setPos(QPoint(item["loc"][0], item["loc"][1]))
-    label.angle = item["ang"]
-    label.labelName = item["nam"]
-    label.labelText = item["txt"]
-    label.labelVisible = item["vis"]
-    label.labelValue = item["val"]
-    return label
-
-
-def createTextItem(item, gridTuple: (int, int)):
-    start = QPoint(item["st"][0], item["st"][1])
-    pen = pens.pen.returnPen(item['pen'])
-    text = shp.text(start, pen, item['tc'], gridTuple, item['ff'], item['fs'],
-                    item['th'], item['ta'], item['to'])
-    text.setPos(QPoint(item["loc"][0], item["loc"][1]))
-    return text
-
-
-def createSymbolAttribute(item):
-    if item["type"] == "attr":
-        return se.symbolAttribute(item["nam"], item["def"])
-
-
-def createSchematicItems(item, libraryDict, viewName: str, gridTuple: (int, int)):
-    """
-    Create schematic items from json file.
-    """
-    if item["type"] == "symbolShape":
-        libraryPath = libraryDict.get(item["lib"])
-        if libraryPath is None:
-            print(f'{item["lib"]} cannot be found.')
-            return None
-        cell = item["cell"]
-        instCounter = item["ic"]
-        itemShapes = list()
-        symbolAttributes = dict()
-        labelDict = item["ld"]
-        draftPen = pens.pen.returnPen('draftPen')
-        # find the symbol file
-        file = libraryPath.joinpath(cell, viewName + ".json")
-        # load json file and create shapes
-        with open(file, "r") as temp:
-            try:
-                shapes = json.load(temp)
-                for shape in shapes[1:]:
-                    if shape["type"] == "rect":
-                        itemShapes.append(createRectItem(shape, gridTuple))
-                    elif shape["type"] == "circle":
-                        itemShapes.append(createCircleItem(shape, gridTuple))
-                    elif shape["type"] == "arc":
-                        itemShapes.append(createArcItem(shape, gridTuple))
-                    elif shape["type"] == "line":
-                        itemShapes.append(createLineItem(shape, gridTuple))
-                    elif shape["type"] == "pin":
-                        itemShapes.append(createPinItem(shape, gridTuple))
-                    elif shape["type"] == "label":
-                        itemShapes.append(createLabelItem(shape, gridTuple))
-                    # just recreate attributes dictionary
-                    elif shape["type"] == "attr":
-                        symbolAttributes[shape["nam"]] = shape["def"]
-            except json.decoder.JSONDecodeError:
-                print("Error: Invalid Symbol file")
-        symbolInstance = shp.symbolShape(draftPen, gridTuple, itemShapes,
-                                         symbolAttributes)
-        symbolInstance.libraryName = item["lib"]
-        symbolInstance.cellName = item["cell"]
-        symbolInstance.counter = instCounter
-        symbolInstance.instanceName = item["nam"]
-        symbolInstance.angle = item["ang"]
-        symbolInstance.viewName = "symbol"
-        symbolInstance.attributes = symbolAttributes
-        for label in symbolInstance.labels.values():
-            if label.labelName in labelDict.keys():
-                label.labelValue = labelDict[label.labelName][0]
-                label.labelVisible = labelDict[label.labelName][1]
-                label.labelDefs()
-        symbolInstance.setPos(item["loc"][0], item["loc"][1])
-        return symbolInstance
-
-
-def createSchematicNets(item):
-    """
-    Create schematic items from json file.
-    """
-    if item["type"] == "schematicNet":
-        start = QPoint(item["st"][0], item["st"][1])
-        end = QPoint(item["end"][0], item["end"][1])
-        position = QPoint(item["loc"][0], item["loc"][1])
-        pen = pens.pen.returnPen(item['pen'])
-        netItem = net.schematicNet(start, end, pen)
-        netItem.name = item["nam"]
-        netItem.nameSet = item["ns"]
-        netItem.setPos(position)
-        return netItem
-
-
-def createSchematicPins(item, gridTuple):
-    """
-    Create schematic items from json file.
-    """
-    if item["type"] == "schematicPin":
-        start = QPoint(item["st"][0], item["st"][1])
-        pen = pens.pen.returnPen(item['pen'])
-        pinName = item["pn"]
-        pinDir = item["pd"]
-        pinType = item["pt"]
-        pinItem = shp.schematicPin(start, pen, pinName, pinDir, pinType,
-                                   gridTuple)
-        pinItem.setPos(QPoint(item["loc"][0], item["loc"][1]))
-        pinItem.angle = item["ang"]
-        return pinItem
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+# Load symbol and maybe later schematic from json file.
+# import pathlib
+
+import json
+
+from PySide6.QtCore import (QPoint, )  # QtCore
+
+import revedaEditor.common.net as net
+import revedaEditor.common.pens as pens
+import revedaEditor.common.shape as shp
+import revedaEditor.fileio.symbolEncoder as se
+
+
+def createSymbolItems(item, gridTuple):
+    """
+    Create symbol items from json file.
+    """
+    if item["type"] == "rect":
+        return createRectItem(item, gridTuple)
+    elif item["type"] == "circle":
+        return createCircleItem(item, gridTuple)
+    elif item["type"] == "arc":
+        return createArcItem(item, gridTuple)
+    elif item["type"] == "line":
+        return createLineItem(item, gridTuple)
+    elif item["type"] == "pin":
+        return createPinItem(item, gridTuple)
+    elif item["type"] == "label":
+        return createLabelItem(item, gridTuple)
+
+
+def createRectItem(item, gridTuple):
+    """
+    Create symbol items from json file.
+    """
+    start = QPoint(item["rect"][0], item["rect"][1])
+    end = QPoint(item["rect"][2], item["rect"][3])
+    pen = pens.sPen.returnPen(item['pen'])
+    rect = shp.rectangle(start, end, pen,
+                         gridTuple)  # note that we are using grid values for scene
+    rect.setPos(QPoint(item["loc"][0], item["loc"][1]), )
+    rect.angle = item["ang"]
+    return rect
+
+
+def createCircleItem(item, gridTuple):
+    centre = QPoint(item["cen"][0], item["cen"][1])
+    end = QPoint(item["end"][0], item["end"][1])
+    pen = pens.sPen.returnPen(item['pen'])
+    circle = shp.circle(centre, end, pen,
+                        gridTuple)  # note that we are using grid values for scene
+    circle.setPos(QPoint(item["loc"][0], item["loc"][1]), )
+    circle.angle = item["ang"]
+    return circle
+
+
+def createArcItem(item, gridTuple):
+    start = QPoint(item["st"][0], item["st"][1])
+    end = QPoint(item["end"][0], item["end"][1])
+    pen = pens.sPen.returnPen(item['pen'])
+    arc = shp.arc(start, end, pen,
+                  gridTuple)  # note that we are using grid values for scene
+    arc.setPos(QPoint(item["loc"][0], item["loc"][1]))
+    arc.angle = item["ang"]
+    return arc
+
+
+def createLineItem(item, gridTuple):
+    start = QPoint(item["st"][0], item["st"][1])
+    end = QPoint(item["end"][0], item["end"][1])
+    pen = pens.sPen.returnPen(item['pen'])
+    line = shp.line(start, end, pen, gridTuple)
+    line.setPos(QPoint(item["loc"][0], item["loc"][1]))
+    line.angle = item["ang"]
+    return line
+
+
+def createPinItem(item, gridTuple):
+    start = QPoint(item["st"][0], item["st"][1])
+    pen = pens.sPen.returnPen(item['pen'])
+    pin = shp.pin(start, pen, item["nam"], item["pd"], item["pt"], gridTuple, )
+    pin.setPos(QPoint(item["loc"][0], item["loc"][1]))
+    pin.angle = item["ang"]
+    return pin
+
+
+def createLabelItem(item, gridTuple):
+    start = QPoint(item["st"][0], item["st"][1])
+    pen = pens.sPen.returnPen(item['pen'])
+    label = shp.label(start, pen, item["def"], gridTuple, item["lt"], item["ht"],
+                      item["al"], item["or"], item["use"], )
+    label.setPos(QPoint(item["loc"][0], item["loc"][1]))
+    label.angle = item["ang"]
+    label.labelName = item["nam"]
+    label.labelText = item["txt"]
+    label.labelVisible = item["vis"]
+    label.labelValue = item["val"]
+    return label
+
+
+def createTextItem(item, gridTuple: (int, int)):
+    start = QPoint(item["st"][0], item["st"][1])
+    pen = pens.sPen.returnPen(item['pen'])
+    text = shp.text(start, pen, item['tc'], gridTuple, item['ff'], item['fs'],
+                    item['th'], item['ta'], item['to'])
+    text.setPos(QPoint(item["loc"][0], item["loc"][1]))
+    return text
+
+
+def createSymbolAttribute(item):
+    if item["type"] == "attr":
+        return se.symbolAttribute(item["nam"], item["def"])
+
+
+def createSchematicItems(item, libraryDict, viewName: str, gridTuple: (int, int)):
+    """
+    Create schematic items from json file.
+    """
+    if item["type"] == "symbolShape":
+        libraryPath = libraryDict.get(item["lib"])
+        if libraryPath is None:
+            print(f'{item["lib"]} cannot be found.')
+            return None
+        cell = item["cell"]
+        instCounter = item["ic"]
+        itemShapes = list()
+        symbolAttributes = dict()
+        labelDict = item["ld"]
+        draftPen = pens.sPen.returnPen('draftPen')
+        # find the symbol file
+        file = libraryPath.joinpath(cell, viewName + ".json")
+        # load json file and create shapes
+        with open(file, "r") as temp:
+            try:
+                shapes = json.load(temp)
+                for shape in shapes[1:]:
+                    if shape["type"] == "rect":
+                        itemShapes.append(createRectItem(shape, gridTuple))
+                    elif shape["type"] == "circle":
+                        itemShapes.append(createCircleItem(shape, gridTuple))
+                    elif shape["type"] == "arc":
+                        itemShapes.append(createArcItem(shape, gridTuple))
+                    elif shape["type"] == "line":
+                        itemShapes.append(createLineItem(shape, gridTuple))
+                    elif shape["type"] == "pin":
+                        itemShapes.append(createPinItem(shape, gridTuple))
+                    elif shape["type"] == "label":
+                        itemShapes.append(createLabelItem(shape, gridTuple))
+                    # just recreate attributes dictionary
+                    elif shape["type"] == "attr":
+                        symbolAttributes[shape["nam"]] = shape["def"]
+            except json.decoder.JSONDecodeError:
+                print("Error: Invalid Symbol file")
+        symbolInstance = shp.symbolShape(draftPen, gridTuple, itemShapes,
+                                         symbolAttributes)
+        symbolInstance.libraryName = item["lib"]
+        symbolInstance.cellName = item["cell"]
+        symbolInstance.counter = instCounter
+        symbolInstance.instanceName = item["nam"]
+        symbolInstance.angle = item["ang"]
+        symbolInstance.viewName = viewName
+        symbolInstance.attributes = symbolAttributes
+        for labelItem in symbolInstance.labels.values():
+            if labelItem.labelName in labelDict.keys():
+                labelItem.labelValue = labelDict[labelItem.labelName][0]
+                labelItem.labelVisible = labelDict[labelItem.labelName][1]
+        symbolInstance.setPos(item["loc"][0], item["loc"][1])
+        return symbolInstance
+
+
+def createSchematicNets(item):
+    """
+    Create schematic items from json file.
+    """
+    if item["type"] == "schematicNet":
+        start = QPoint(item["st"][0], item["st"][1])
+        end = QPoint(item["end"][0], item["end"][1])
+        position = QPoint(item["loc"][0], item["loc"][1])
+        pen = pens.sPen.returnPen(item['pen'])
+        netItem = net.schematicNet(start, end, pen)
+        netItem.name = item["nam"]
+        netItem.nameSet = item["ns"]
+        netItem.setPos(position)
+        return netItem
+
+
+def createSchematicPins(item, gridTuple):
+    """
+    Create schematic items from json file.
+    """
+    if item["type"] == "schematicPin":
+        start = QPoint(item["st"][0], item["st"][1])
+        pen = pens.sPen.returnPen(item['pen'])
+        pinName = item["pn"]
+        pinDir = item["pd"]
+        pinType = item["pt"]
+        pinItem = shp.schematicPin(start, pen, pinName, pinDir, pinType,
+                                   gridTuple)
+        pinItem.setPos(QPoint(item["loc"][0], item["loc"][1]))
+        pinItem.angle = item["ang"]
+        return pinItem
```

### Comparing `revolution-eda-0.4.1/gui/__init__.py` & `revolution-eda-0.5.0/revedaEditor/backend/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,7 @@
 #   license notice or attribution required by the License must also include this
 #   Commons Clause License Condition notice.
 #  #
 #   Software: Revolution EDA
 #   License: Mozilla Public License 2.0
 #   Licensor: Revolution Semiconductor (Registered in the Netherlands)
 
-
```

### Comparing `revolution-eda-0.4.1/gui/editFunctions.py` & `revolution-eda-0.5.0/pdk/callbacks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 
-
 #   “Commons Clause” License Condition v1.0
 #  #
 #   The Software is provided to you by the Licensor under the License, as defined
 #   below, subject to the following condition.
 #  #
 #   Without limiting other conditions in the License, the grant of rights under the
 #   License will not include, and the License does not grant to you, the right to
@@ -17,27 +16,35 @@
 #   license notice or attribution required by the License must also include this
 #   Commons Clause License Condition notice.
 #  #
 #   Software: Revolution EDA
 #   License: Mozilla Public License 2.0
 #   Licensor: Revolution Semiconductor (Registered in the Netherlands)
 
-from PySide6.QtCore import (Qt, )
-from PySide6.QtWidgets import (QLineEdit, QLabel, QWidget)
+from quantiphy import Quantity
+
+class baseInst():
+    def __init__(self, labels_dict: dict):
+        self._labelsDict = labels_dict
+
+class res(baseInst):
+    def __init__(self,labels_dict:dict):
+        super().__init__(labels_dict)
+
+    def doubleR(self):
+        Rvalue = self._labelsDict.get('R').labelValue
+        if Rvalue.isalnum():
+            return str(2*Quantity(Rvalue))
+        return '?'
+
+class nmos(baseInst):
+    def __init__(self,labels_dict:dict):
+        super().__init__(labels_dict)
+        self.w = Quantity(self._labelsDict['w'].labelValue)
+        self.l = Quantity(self._labelsDict['l'].labelValue)
+        self.nf= Quantity(self._labelsDict['nf'].labelValue)
+        self.sd1p8v = 0.28
+        self.sa1p8v = sb1p8v = 0.265
+        self.sourceDiffs = lambda nf: int(int(nf) / 2 + 1)
 
-class shortLineEdit(QLineEdit):
-    def __init__(self):
-        super().__init__(None)
-        self.setMaximumWidth(80)
-
-
-class boldLabel(QLabel):
-    def __init__(self, text: str, parent: QWidget = None):
-        super().__init__(text, parent)
-        self.setTextFormat(Qt.RichText)
-        self.setText("<b>" + text + "</b>")
-
-
-class longLineEdit(QLineEdit):
-    def __init__(self):
-        super().__init__(None)
-        self.setMaximumWidth(500)
+    def asparm(self):
+        return self.sourceDiffs(self.nf)*(self.w/self.nf)*self.sd1p8v
```

### Comparing `revolution-eda-0.4.1/gui/editorWindows.py` & `revolution-eda-0.5.0/revedaEditor/gui/editorWindows.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,3459 +1,3734 @@
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-from copy import deepcopy
-import datetime
-import json
-import math
-
-# from hashlib import new
-import pathlib
-import shutil
-
-# import numpy as np
-from PySide6.QtCore import (QDir, Qt, QRect, QPoint, QMargins, QRectF, QProcess,
-                            QRunnable, Signal, Slot)
-from PySide6.QtGui import (QAction, QKeySequence, QColor, QIcon, QPainter, QPen,
-                           QImage, QStandardItemModel, QCursor, QUndoStack,
-                           QTextDocument, QGuiApplication, QCloseEvent, QFont,
-                           QStandardItem)
-from PySide6.QtPrintSupport import (QPrintDialog, )
-from PySide6.QtWidgets import (QDialog, QDialogButtonBox, QFileDialog,
-                               QFormLayout, QGraphicsScene, QHBoxLayout, QLabel,
-                               QLineEdit, QMainWindow, QMenu, QMessageBox,
-                               QToolBar, QTreeView, QVBoxLayout, QWidget,
-                               QGraphicsRectItem, QGraphicsEllipseItem,
-                               QGraphicsView, QGridLayout,
-                               QGraphicsSceneMouseEvent, QAbstractItemView,
-                               QTableView, QGroupBox, QComboBox)
-
-import backend.schBackEnd as scb
-import backend.undoStack as us
-import backend.libraryMethods as libm
-import common.layers as cel
-import common.net as net
-import common.pens as pens  # import pens
-import common.shape as shp  # import the shapes
-import fileio.loadJSON as lj
-import fileio.symbolEncoder as se
-import gui.fileDialogues as fd
-import gui.propertyDialogues as pdlg
-import gui.editFunctions as edf
-
-
-class editorWindow(QMainWindow):
-    """
-    Base class for editor windows.
-    """
-
-    def __init__(self, viewItem: scb.viewItem, libraryDict: dict,
-                 libraryView):  # file is a pathlib.Path object
-        super().__init__()
-        self.viewItem = viewItem
-        self.file = self.viewItem.data(Qt.UserRole + 2)
-        self.cellItem = self.viewItem.parent()
-        self.cellName = self.cellItem.cellName
-        self.libItem = self.cellItem.parent()
-        self.libName = self.libItem.libraryName
-        self.viewName = self.viewItem.viewName
-        self.libraryDict = libraryDict
-        self.libraryView = libraryView
-        self.parentView = None
-        self._createActions()
-        self._createTriggers()
-        self._createShortcuts()
-        self.appMainW = self.libraryView.parent.parent.appMainW
-        self.logger = self.appMainW.logger
-        self.switchViewList = self.appMainW.switchViewList
-        self.stopViewList = self.appMainW.stopViewList
-        self.statusLine = self.statusBar()
-        self.messageLine = QLabel()  # message line
-        self.statusLine.addPermanentWidget(self.messageLine)
-        self.majorGrid = 10  # snapping grid size
-        self.gridTuple = (self.majorGrid, self.majorGrid)
-        self.init_UI()
-
-    def init_UI(self):
-        """
-        Placeholder for child classes init_UI function.
-        """
-        ...
-
-    def _createMenuBar(self):
-        self.editorMenuBar = self.menuBar()
-        self.editorMenuBar.setNativeMenuBar(False)
-        # Returns QMenu object.
-        self.menuFile = self.editorMenuBar.addMenu("&File")
-        self.menuView = self.editorMenuBar.addMenu("&View")
-        self.menuEdit = self.editorMenuBar.addMenu("&Edit")
-        self.menuCreate = self.editorMenuBar.addMenu("C&reate")
-        self.menuCheck = self.editorMenuBar.addMenu("&Check")
-        self.menuTools = self.editorMenuBar.addMenu("&Tools")
-        self.menuWindow = self.editorMenuBar.addMenu("&Window")
-        self.menuUtilities = self.editorMenuBar.addMenu("&Utilities")
-
-    def _createActions(self):
-        checkCellIcon = QIcon(":/icons/document-task.png")
-        self.checkCellAction = QAction(checkCellIcon, "Check-Save", self)
-
-        self.readOnlyCellIcon = QIcon(":/icons/lock.png")
-        self.readOnlyCellAction = QAction(self.readOnlyCellIcon, "Make Read Only",
-                                          self)
-
-        printIcon = QIcon(":/icons/printer--arrow.png")
-        self.printAction = QAction(printIcon, "Print...", self)
-
-        printPreviewIcon = QIcon(":/icons/printer--arrow.png")
-        self.printPreviewAction = QAction(printPreviewIcon, "Print Preview...",
-                                          self)
-
-        exportImageIcon = QIcon(":/icons/image-export.png")
-        self.exportImageAction = QAction(exportImageIcon, "Export...", self)
-
-        exitIcon = QIcon(":/icons/external.png")
-        self.exitAction = QAction(exitIcon, "Close Window", self)
-        self.exitAction.setShortcut("Ctrl+Q")
-
-        fitIcon = QIcon(":/icons/zone.png")
-        self.fitAction = QAction(fitIcon, "Fit to Window", self)
-
-        zoomInIcon = QIcon(":/icons/zone-resize.png")
-        self.zoomInAction = QAction(zoomInIcon, "Zoom In", self)
-
-        zoomOutIcon = QIcon(":/icons/zone-resize-actual.png")
-        self.zoomOutAction = QAction(zoomOutIcon, "Zoom Out", self)
-
-        panIcon = QIcon(":/icons/zone--arrow.png")
-        self.panAction = QAction(panIcon, "Pan View", self)
-
-        redrawIcon = QIcon(":/icons/arrow-circle.png")
-        self.redrawAction = QAction(redrawIcon, "Redraw", self)
-
-        # rulerIcon = QIcon(":/icons/ruler.png")
-        # self.rulerAction = QAction(rulerIcon, 'Ruler', self)
-        # self.menuView.addAction(self.rulerAction)
-        # delRulerIcon = QIcon.fromTheme('delete')
-        # self.delRulerAction = QAction(delRulerIcon, 'Delete Rulers', self)
-        # self.menuView.addAction(self.delRulerAction)
-
-        # display options
-        dispConfigIcon = QIcon(":/icons/resource-monitor.png")
-        self.dispConfigAction = QAction(dispConfigIcon, "Display Config...", self)
-
-        selectConfigIcon = QIcon(":/icons/zone-select.png")
-        self.selectConfigAction = QAction(selectConfigIcon, "Selection Config...",
-                                          self)
-
-        panZoomConfigIcon = QIcon(":/icons/selection-resize.png")
-        self.panZoomConfigAction = QAction(panZoomConfigIcon,
-                                           "Pan/Zoom Config...", self)
-
-        undoIcon = QIcon(":/icons/arrow-circle-315-left.png")
-        self.undoAction = QAction(undoIcon, "Undo", self)
-
-        redoIcon = QIcon(":/icons/arrow-circle-225.png")
-        self.redoAction = QAction(redoIcon, "Redo", self)
-
-        yankIcon = QIcon(":/icons/node-insert.png")
-        self.yankAction = QAction(yankIcon, "Yank", self)
-
-        pasteIcon = QIcon(":/icons/clipboard-paste.png")
-        self.pasteAction = QAction(pasteIcon, "Paste", self)
-
-        deleteIcon = QIcon(":/icons/node-delete.png")
-        self.deleteAction = QAction(deleteIcon, "Delete", self)
-
-        copyIcon = QIcon(":/icons/document-copy.png")
-        self.copyAction = QAction(copyIcon, "Copy", self)
-
-        moveIcon = QIcon(":/icons/arrow-move.png")
-        self.moveAction = QAction(moveIcon, "Move", self)
-
-        moveByIcon = QIcon(":/icons/arrow-transition.png")
-        self.moveByAction = QAction(moveByIcon, "Move By ...", self)
-
-        moveOriginIcon = QIcon(":/icons/arrow-skip.png")
-        self.moveOriginAction = QAction(moveOriginIcon, "Move Origin", self)
-
-        stretchIcon = QIcon(":/icons/fill.png")
-        self.stretchAction = QAction(stretchIcon, "Stretch", self)
-
-        rotateIcon = QIcon(":/icons/arrow-circle.png")
-        self.rotateAction = QAction(rotateIcon, "Rotate...", self)
-
-        scaleIcon = QIcon(":/icons/selection-resize.png")
-        self.scaleAction = QAction(scaleIcon, "Scale...", self)
-
-        netNameIcon = QIcon(":/icons/node-design.png")
-        self.netNameAction = QAction(netNameIcon, "Net Name...", self)
-
-        # create label action but do not add to any menu.
-        createLabelIcon = QIcon(":/icons/tag-label-yellow.png")
-        self.createLabelAction = QAction(createLabelIcon, "Create Label...", self)
-
-        createPinIcon = QIcon(":/icons/pin--plus.png")
-        self.createPinAction = QAction(createPinIcon, "Create Pin...", self)
-
-        goUpIcon = QIcon(":/icons/arrow-step-out.png")
-        self.goUpAction = QAction(goUpIcon, "Go Up   ↑", self)
-
-        goDownIcon = QIcon(":/icons/arrow-step.png")
-        self.goDownAction = QAction(goDownIcon, "Go Down ↓", self)
-
-        self.selectAllIcon = QIcon(":/icons/node-select-all.png")
-        self.selectAllAction = QAction(self.selectAllIcon, "Select All", self)
-
-        deselectAllIcon = QIcon(":/icons/node.png")
-        self.deselectAllAction = QAction(deselectAllIcon, "Unselect All", self)
-
-        objPropIcon = QIcon(":/icons/property-blue.png")
-        self.objPropAction = QAction(objPropIcon, "Object Properties...", self)
-
-        viewPropIcon = QIcon(":/icons/property.png")
-        self.viewPropAction = QAction(viewPropIcon, "Cellview Properties...",
-                                      self)
-
-        viewCheckIcon = QIcon(":/icons/ui-check-box.png")
-        self.viewCheckAction = QAction(viewCheckIcon, "Check CellView", self)
-
-        viewErrorsIcon = QIcon(":/icons/report--exclamation.png")
-        self.viewErrorsAction = QAction(viewErrorsIcon, "View Errors...", self)
-
-        deleteErrorsIcon = QIcon(":/icons/report--minus.png")
-        self.deleteErrorsAction = QAction(deleteErrorsIcon, "Delete Errors...",
-                                          self)
-
-        netlistIcon = QIcon(":/icons/script-text.png")
-        self.netlistAction = QAction(netlistIcon, "Create Netlist...", self)
-
-        simulateIcon = QIcon(":/icons/application-wave.png")
-        self.simulateAction = QAction(simulateIcon, "Run RevEDA Sim GUI", self)
-
-        createLineIcon = QIcon(":/icons/layer-shape-line.png")
-        self.createLineAction = QAction(createLineIcon, "Create Line...", self)
-
-        createRectIcon = QIcon(":/icons/layer-shape.png")
-        self.createRectAction = QAction(createRectIcon, "Create Rectangle...",
-                                        self)
-
-        createPolyIcon = QIcon(":/icons/layer-shape-polygon.png")
-        self.createPolyAction = QAction(createPolyIcon, "Create Polygon...", self)
-
-        createCircleIcon = QIcon(":/icons/layer-shape-ellipse.png")
-        self.createCircleAction = QAction(createCircleIcon, "Create Circle...",
-                                          self)
-
-        createArcIcon = QIcon(":/icons/layer-shape-polyline.png")
-        self.createArcAction = QAction(createArcIcon, "Create Arc...", self)
-
-        createInstIcon = QIcon(":/icons/block--plus.png")
-        self.createInstAction = QAction(createInstIcon, "Create Instance...",
-                                        self)
-
-        createWireIcon = QIcon(":/icons/node-insert.png")
-        self.createWireAction = QAction(createWireIcon, "Create Wire...", self)
-
-        createBusIcon = QIcon(":/icons/node-select-all.png")
-        self.createBusAction = QAction(createBusIcon, "Create Bus...", self)
-
-        createLabelIcon = QIcon(":/icons/tag-label-yellow.png")
-        self.createLabelAction = QAction(createLabelIcon, "Create Label...", self)
-
-        createPinIcon = QIcon(":/icons/pin--plus.png")
-        self.createPinAction = QAction(createPinIcon, "Create Pin...", self)
-
-        createSymbolIcon = QIcon(":/icons/application-block.png")
-        self.createSymbolAction = QAction(createSymbolIcon, "Create Symbol...",
-                                          self)
-
-        createTextIcon = QIcon(":icons/sticky-note-text.png")
-        self.createTextAction = QAction(createTextIcon, "Create Text...", self)
-
-    def _createToolBars(self):
-        # Create tools bar called "main toolbar"
-        self.toolbar = QToolBar("Main Toolbar", self)
-        # place toolbar at top
-        self.addToolBar(self.toolbar)
-        self.toolbar.addAction(self.printAction)
-        self.toolbar.addAction(self.exportImageAction)
-        self.toolbar.addSeparator()
-        self.toolbar.addAction(self.undoAction)
-        self.toolbar.addAction(self.redoAction)
-        self.toolbar.addSeparator()
-        self.toolbar.addAction(self.deleteAction)
-        self.toolbar.addAction(self.moveAction)
-        self.toolbar.addAction(self.copyAction)
-        self.toolbar.addAction(self.stretchAction)
-        self.toolbar.addAction(self.rotateAction)
-        self.toolbar.addSeparator()
-        self.toolbar.addAction(self.fitAction)
-        self.toolbar.addAction(self.zoomInAction)
-        self.toolbar.addAction(self.zoomOutAction)
-        self.toolbar.addSeparator()
-        self.toolbar.addAction(self.objPropAction)
-
-    def _addActions(self):
-        # file menu
-        self.menuFile.addAction(self.checkCellAction)
-        self.menuFile.addAction(self.readOnlyCellAction)
-        self.menuFile.addAction(self.printAction)
-        self.menuFile.addAction(self.printPreviewAction)
-        self.menuFile.addAction(self.exportImageAction)
-        self.menuFile.addAction(self.exitAction)
-        # view menu
-        self.menuView.addAction(self.fitAction)
-        self.menuView.addAction(self.zoomInAction)
-        self.menuView.addAction(self.zoomOutAction)
-        self.menuView.addAction(self.panAction)
-        self.menuView.addAction(self.redrawAction)
-        self.menuView.addAction(self.dispConfigAction)
-        self.menuView.addAction(self.selectConfigAction)
-        self.menuView.addAction(self.panZoomConfigAction)
-        # edit menu
-        self.menuEdit.addAction(self.undoAction)
-        self.menuEdit.addAction(self.redoAction)
-        self.menuEdit.addAction(self.yankAction)
-        self.menuEdit.addAction(self.pasteAction)
-        self.menuEdit.addAction(self.deleteAction)
-        self.menuEdit.addAction(self.copyAction)
-        self.menuEdit.addAction(self.moveAction)
-        self.menuEdit.addAction(self.moveByAction)
-        self.menuEdit.addAction(self.moveOriginAction)
-        self.menuEdit.addAction(self.stretchAction)
-        self.menuEdit.addAction(self.rotateAction)
-
-        self.menuCheck.addAction(self.viewCheckAction)
-
-    def _createTriggers(self):
-        self.printAction.triggered.connect(self.printClick)
-        # self.printPreviewAction.triggered.connect(self.printPreviewClick)
-        self.exportImageAction.triggered.connect(self.imageExportClick)
-        self.exitAction.triggered.connect(self.closeWindow)
-        self.fitAction.triggered.connect(self.fitToWindow)
-        self.zoomInAction.triggered.connect(self.zoomIn)
-        self.zoomOutAction.triggered.connect(self.zoomOut)
-        self.dispConfigAction.triggered.connect(self.dispConfDialog)
-        self.moveOriginAction.triggered.connect(self.moveOrigin)
-
-    def _createShortcuts(self):
-        self.redoAction.setShortcut("Shift+U")
-        self.undoAction.setShortcut(Qt.Key_U)
-        self.objPropAction.setShortcut(Qt.Key_Q)
-        self.copyAction.setShortcut("C")
-        self.rotateAction.setShortcut("Ctrl+R")
-        self.createTextAction.setShortcut("Shift+L")
-        self.deleteAction.setShortcut(QKeySequence.Delete)
-
-    def dispConfDialog(self):
-        dcd = pdlg.displayConfigDialog(self)
-        dlg.majorGridEntry.setText(str(self.majorGrid))
-        if dcd.exec() == QDialog.Accepted:
-            self.majorGrid = int(float(dcd.majorGridEntry.text()))
-
-    def printClick(self):
-        dlg = QPrintDialog(self)
-        if dlg.exec() == QDialog.Accepted:
-            printer = dlg.printer()
-            self.centralW.view.printView(printer)
-
-    # def printPreviewClick(self):
-    #     # dlg = QPrintDialog(self)
-    #     # if dlg.exec() == QDialog.Accepted:
-    #     #     printer = dlg.printer()
-    #     printer = QPrinter(QPrinter.ScreenResolution)
-    #
-    #     ppdlg = QPrintPreviewDialog(self)
-    #     ppdlg.paintRequested.connect(self.centralW.scene.render(QPainter(printer)))
-    #     ppdlg.exec()
-    def imageExportClick(self):
-        image = QImage(self.centralW.view.viewport().size(),
-                       QImage.Format_ARGB32_Premultiplied)
-        self.centralW.view.printView(image)
-        fdlg = QFileDialog(self, caption="Select or create an image file")
-        fdlg.setDefaultSuffix("png")
-        fdlg.setFileMode(QFileDialog.AnyFile)
-        fdlg.setViewMode(QFileDialog.Detail)
-        fdlg.setNameFilter("Image Files (*.png *.jpg *.bmp *.gif *.jpeg")
-        if fdlg.exec() == QDialog.Accepted:
-            imageFile = fdlg.selectedFiles()[0]
-        image.save(imageFile)
-
-    def fitToWindow(self):
-        self.centralW.view.fitToView()
-
-    def zoomIn(self):
-        self.centralW.view.scale(1.25, 1.25)
-
-    def zoomOut(self):
-        self.centralW.view.scale(0.8, 0.8)
-
-    def closeWindow(self):
-        self.close()
-
-    def _createMenu(self):
-        pass
-
-    def moveOrigin(self):
-        self.centralW.scene.changeOrigin = True
-
-
-class schematicEditor(editorWindow):
-    def __init__(self, viewItem: scb.viewItem, libraryDict: dict,
-                 libraryView) -> None:
-        super().__init__(viewItem, libraryDict, libraryView)
-        self.setWindowTitle(f"Schematic Editor - {self.cellName}")
-        self.setWindowIcon(QIcon(":/icons/layer-shape.png"))
-        self.configDict = dict()
-        self.netlistedCells = list()
-        self.symbolChooser = None
-        self.cellViews = [
-            "symbol"]  # only symbol can be instantiated in the schematic window.
-        self._schematicActions()
-
-    def init_UI(self):
-        self.resize(1600, 800)
-        self._createMenuBar()
-        self._createToolBars()
-        # create container to position all widgets
-        self.centralW = schematicContainer(self)
-        self.setCentralWidget(self.centralW)
-
-    def _createTriggers(self):
-        super()._createTriggers()
-        self.checkCellAction.triggered.connect(self.checkSaveCell)
-        self.createWireAction.triggered.connect(self.createWireClick)
-        self.createInstAction.triggered.connect(self.createInstClick)
-        self.createPinAction.triggered.connect(self.createPinClick)
-        self.createTextAction.triggered.connect(self.createNoteClick)
-        self.createSymbolAction.triggered.connect(self.createSymbolClick)
-        self.copyAction.triggered.connect(self.copyClick)
-        self.deleteAction.triggered.connect(self.deleteClick)
-        self.objPropAction.triggered.connect(self.objPropClick)
-        self.undoAction.triggered.connect(self.undoClick)
-        self.redoAction.triggered.connect(self.redoClick)
-        self.netlistAction.triggered.connect(self.createNetlistClick)
-        self.rotateAction.triggered.connect(self.rotateItemClick)
-        self.simulateAction.triggered.connect(self.startSimClick)
-        self.goDownAction.triggered.connect(self.goDownClick)
-        self.goUpAction.triggered.connect(self.goUpClick)
-
-    def _createMenuBar(self):
-        super()._createMenuBar()
-        self.menuSimulation = self.editorMenuBar.addMenu("&Simulation")
-        self.menuHelp = self.editorMenuBar.addMenu("&Help")
-        self._addActions()
-
-    def _addActions(self):
-        super()._addActions()
-        # edit menu
-
-        self.menuEdit.addAction(self.netNameAction)
-
-        self.propertyMenu = self.menuEdit.addMenu("Properties")
-        self.propertyMenu.addAction(self.objPropAction)
-
-        self.selectMenu = self.menuEdit.addMenu("Select")
-        self.selectMenu.addAction(self.selectAllAction)
-        self.selectMenu.addAction(self.deselectAllAction)
-
-        # hierarchy submenu
-        self.hierMenu = self.menuEdit.addMenu("Hierarchy")
-        self.hierMenu.addAction(self.goUpAction)
-        self.hierMenu.addAction(self.goDownAction)
-
-        # create menu
-        self.menuCreate.addAction(self.createInstAction)
-        self.menuCreate.addAction(self.createWireAction)
-        self.menuCreate.addAction(self.createBusAction)
-        self.menuCreate.addAction(self.createLabelAction)
-        self.menuCreate.addAction(self.createPinAction)
-        self.menuCreate.addAction(self.createTextAction)
-        self.menuCreate.addAction(self.createSymbolAction)
-
-        # check menu
-        self.menuCheck.addAction(self.viewErrorsAction)
-        self.menuCheck.addAction(self.deleteErrorsAction)
-
-        self.menuSimulation.addAction(self.netlistAction)
-        self.menuSimulation.addAction(self.simulateAction)
-
-    def _createToolBars(self):
-        super()._createToolBars()
-        # toolbar.addAction(self.rulerAction)
-        # toolbar.addAction(self.delRulerAction)
-        self.toolbar.addAction(self.objPropAction)
-        self.toolbar.addAction(self.viewPropAction)
-
-        self.schematicToolbar = QToolBar("Schematic Toolbar", self)
-        self.addToolBar(self.schematicToolbar)
-        self.schematicToolbar.addAction(self.createInstAction)
-        self.schematicToolbar.addAction(self.createWireAction)
-        self.schematicToolbar.addAction(self.createBusAction)
-        self.schematicToolbar.addAction(self.createPinAction)
-        # self.schematicToolbar.addAction(self.createLabelAction)
-        self.schematicToolbar.addAction(self.createSymbolAction)
-        self.schematicToolbar.addSeparator()
-        self.schematicToolbar.addAction(self.viewCheckAction)
-
-    def _schematicActions(self):
-        self.centralW.scene.itemContextMenu.addAction(self.copyAction)
-        self.centralW.scene.itemContextMenu.addAction(self.moveAction)
-        self.centralW.scene.itemContextMenu.addAction(self.rotateAction)
-        self.centralW.scene.itemContextMenu.addAction(self.deleteAction)
-        self.centralW.scene.itemContextMenu.addAction(self.objPropAction)
-        self.centralW.scene.itemContextMenu.addAction(self.goDownAction)
-        if self.parentView is not None:
-            self.centralW.scene.itemContextMenu.addAction(self.goUpAction)
-
-    def _createShortcuts(self):
-        super()._createShortcuts()
-        self.createInstAction.setShortcut(Qt.Key_I)
-        self.createWireAction.setShortcut(Qt.Key_W)
-        self.createPinAction.setShortcut(Qt.Key_P)
-
-    def createWireClick(self, s):
-        self.centralW.scene.drawWire = True
-
-    def deleteClick(self, s):
-        self.centralW.scene.deleteSelectedItems()
-
-    def createInstClick(self, s):
-
-        # create a designLibrariesView
-        libraryModel = symbolViewsModel(self.libraryDict)
-        if self.symbolChooser is None:
-            self.symbolChooser = fd.selectCellViewDialog(self, libraryModel)
-            self.symbolChooser.show()
-        else:
-            self.symbolChooser.raise_()
-        if self.symbolChooser.exec() == QDialog.Accepted:
-            self.centralW.scene.addInstance = True
-            libItem = libm.getLibItem(libraryModel,
-                                      self.symbolChooser.libNamesCB.currentText())
-            cellItem = libm.getCellItem(libItem,
-                                        self.symbolChooser.cellCB.currentText())
-            viewItem = libm.getViewItem(cellItem,
-                                        self.symbolChooser.viewCB.currentText())
-            self.centralW.scene.instanceSymbolFile = viewItem.data(
-                Qt.UserRole + 2)
-
-    def createPinClick(self, s):
-        createPinDlg = pdlg.createSchematicPinDialog(self)
-        if createPinDlg.exec() == QDialog.Accepted:
-            self.centralW.scene.pinName = createPinDlg.pinName.text()
-            self.centralW.scene.pinType = createPinDlg.pinType.currentText()
-            self.centralW.scene.pinDir = createPinDlg.pinDir.currentText()
-            self.centralW.scene.drawPin = True
-
-    def createNoteClick(self, s):
-        textDlg = pdlg.noteTextEdit(self)
-        if textDlg.exec() == QDialog.Accepted:
-            self.centralW.scene.noteText = textDlg.plainTextEdit.toPlainText()
-            self.centralW.scene.noteFontFamily = textDlg.familyCB.currentText()
-            self.centralW.scene.noteFontSize = textDlg.fontsizeCB.currentText()
-            self.centralW.scene.noteFontStyle = textDlg.fontStyleCB.currentText()
-            self.centralW.scene.noteAlign = textDlg.textAlignmCB.currentText()
-            self.centralW.scene.noteOrient = textDlg.textOrientCB.currentText()
-            self.centralW.scene.drawText = True
-
-    def createSymbolClick(self, s):
-        self.centralW.scene.createSymbol()
-
-    def undoClick(self, s):
-        self.centralW.scene.undoStack.undo()
-
-    def redoClick(self, s):
-        self.centralW.scene.undoStack.redo()
-
-    def objPropClick(self, s):
-        self.centralW.scene.viewObjProperties()
-
-    def copyClick(self, s):
-        self.centralW.scene.copySelectedItems()
-
-    def rotateItemClick(self, s):
-        self.centralW.scene.rotateItem = True
-        self.centralW.scene.itemSelect = False
-
-    def startSimClick(self, s):
-        simguiw = revedasim.simGUImainWindow(self)
-        simguiw.show()
-
-    def checkSaveCell(self):
-        self.centralW.scene.saveSchematicCell(self.file)
-
-    def loadSchematic(self):
-        with open(self.file) as tempFile:
-            items = json.load(tempFile)
-        self.centralW.scene.loadSchematicCell(items)
-
-    def createConfigView(self, configItem: scb.viewItem, configDict: dict,
-                         newConfigDict: dict, netlistedCells: set):
-
-        sceneSymbolSet = self.centralW.scene.findSceneSymbolSet()
-        for item in sceneSymbolSet:
-            libItem = libm.getLibItem(self.libraryView.libraryModel,
-                                      item.libraryName)
-            cellItem = libm.getCellItem(libItem, item.cellName)
-            viewItems = [cellItem.child(row) for row in
-                         range(cellItem.rowCount())]
-            viewNames = [viewItem.viewName for viewItem in viewItems]
-            netlistableViews = [viewItemName for viewItemName in
-                                self.switchViewList if viewItemName in viewNames]
-            itemSwitchViewList = deepcopy(netlistableViews)
-            viewDict = dict(zip(viewNames, viewItems))
-            if cellItem.cellName not in netlistedCells:
-                cellLine = configDict.get(cellItem.cellName)
-                if cellLine:
-                    netlistableViews = [cellLine[1]]
-                for viewName in netlistableViews:
-                    match viewDict[viewName].viewType:
-                        case "schematic":
-                            newConfigDict.update({
-                                cellItem.cellName: [libItem.libraryName, viewName,
-                                                    itemSwitchViewList, ]})
-                            schematicObj = schematicEditor(viewDict[viewName],
-                                                           self.libraryDict,
-                                                           self.libraryView, )
-                            schematicObj.loadSchematic()
-                            schematicObj.createConfigView(configItem, configDict,
-                                                          newConfigDict,
-                                                          netlistedCells)
-                            break
-                        case other:
-                            newConfigDict.update({
-                                cellItem.cellName: [libItem.libraryName, viewName,
-                                                    itemSwitchViewList, ]})
-                            break
-                netlistedCells.append(cellItem.cellName)
-
-    def closeEvent(self, event):
-        self.centralW.scene.saveSchematicCell(self.file)
-        self.libraryView.openViews.pop(
-            f"{self.libName}_{self.cellName}_{self.viewName}")
-        event.accept()
-
-    def createNetlistClick(self, s):
-        dlg = fd.netlistExportDialogue(self)
-        dlg.libNameEdit.setText(self.libName)
-        dlg.cellNameEdit.setText(self.cellName)
-        configViewItems = [self.cellItem.child(row) for row in
-                           range(self.cellItem.rowCount()) if
-                           self.cellItem.child(row).viewType == 'config']
-        netlistableViews = [self.viewItem.viewName]
-        for item in configViewItems:
-            # is there a better way of doing it?
-            with item.data(Qt.UserRole + 2).open(mode='r') as f:
-                configItems = json.load(f)
-                if configItems[1]['reference'] == self.viewItem.viewName:
-                    netlistableViews.append(item.viewName)
-        dlg.viewNameCombo.addItems(netlistableViews)
-        if hasattr(self.appMainW, "simulationPath"):
-            dlg.netlistDirEdit.setText(str(self.appMainW.simulationPath))
-        if dlg.exec() == QDialog.Accepted:
-            self.netlistDir = dlg.netlistDirEdit.text()
-            selectedViewName = dlg.viewNameCombo.currentText()
-            self.switchViewList = [item.strip() for item in
-                                   dlg.switchViewEdit.text().split(",")]
-            self.stopViewList = [dlg.stopViewEdit.text().strip()]
-            simDirPathObj = pathlib.Path(self.netlistDir)
-            subDirPathObj = simDirPathObj.joinpath(self.cellName)
-            subDirPathObj.mkdir(parents=True, exist_ok=True)
-            netlistFilePathObj = subDirPathObj.joinpath(f'{self.cellName}_'
-                                                        f'{selectedViewName}').with_suffix(
-                '.cir')
-            if 'schematic' in dlg.viewNameCombo.currentText():
-                netlistObj = xyceNetlist(self, netlistFilePathObj)
-            else:
-                netlistObj = xyceNetlist(self, netlistFilePathObj, True)
-                configItem = libm.findViewItem(self.libraryView.libraryModel,
-                                               self.libName, self.cellName,
-                                               dlg.viewNameCombo.currentText())
-                with configItem.data(Qt.UserRole + 2).open(mode='r') as f:
-                    netlistObj.configDict = json.load(f)[2]
-            xyceNetlRunner = runXNetlistThread(netlistObj, self)
-            self.logger.info('Writing netlist')
-            self.appMainW.threadPool.start(xyceNetlRunner)
-
-    def goDownClick(self, s):
-        self.centralW.scene.goDownHier()
-
-    def goUpClick(self, s):
-        self.centralW.scene.goUpHier()
-
-
-class symbolEditor(editorWindow):
-    def __init__(self, viewItem: scb.viewItem, libraryDict: dict, libraryView):
-        super().__init__(viewItem, libraryDict, libraryView)
-        self.setWindowTitle(f"Symbol Editor - {self.cellName}")
-        self._symbolActions()
-
-    def init_UI(self):
-        self.resize(1600, 800)
-        self._createMenuBar()
-        self._createToolBars()
-        # create container to position all widgets
-        self.centralW = symbolContainer(self)
-        self.setCentralWidget(self.centralW)
-
-    def _createActions(self):
-        super()._createActions()
-
-    def _createShortcuts(self):
-        super()._createShortcuts()
-        self.stretchAction.setShortcut(Qt.Key_M)
-        self.createRectAction.setShortcut(Qt.Key_R)
-        self.createLineAction.setShortcut(Qt.Key_W)
-        self.createLabelAction.setShortcut(Qt.Key_L)
-
-    def _createMenuBar(self):
-        super()._createMenuBar()
-        self.menuHelp = self.editorMenuBar.addMenu("&Help")
-        self._addActions()
-
-    def _createToolBars(self):  # redefine the toolbar in the editorWindow class
-        super()._createToolBars()
-        self.symbolToolbar = QToolBar("Symbol Toolbar", self)
-        self.addToolBar(self.symbolToolbar)
-        self.symbolToolbar.addAction(self.createLineAction)
-        self.symbolToolbar.addAction(self.createRectAction)
-        self.symbolToolbar.addAction(self.createPolyAction)
-        self.symbolToolbar.addAction(self.createCircleAction)
-        self.symbolToolbar.addAction(self.createArcAction)
-        self.symbolToolbar.addAction(self.createLabelAction)
-        self.symbolToolbar.addAction(self.createPinAction)
-
-    def _addActions(self):
-        super()._addActions()
-        self.menuEdit.addAction(self.stretchAction)
-        self.menuEdit.addAction(self.viewPropAction)
-        self.menuCreate.addAction(self.createLineAction)
-        self.menuCreate.addAction(self.createRectAction)
-        self.menuCreate.addAction(self.createPolyAction)
-        self.menuCreate.addAction(self.createCircleAction)
-        self.menuCreate.addAction(self.createArcAction)
-        self.menuCreate.addAction(self.createLabelAction)
-        self.menuCreate.addAction(self.createPinAction)
-
-    def _createTriggers(self):
-
-        self.checkCellAction.triggered.connect(self.checkSaveCell)
-        self.createLineAction.triggered.connect(self.createLineClick)
-        self.createRectAction.triggered.connect(self.createRectClick)
-        self.createPolyAction.triggered.connect(self.createPolyClick)
-        self.createArcAction.triggered.connect(self.createArcClick)
-        self.createCircleAction.triggered.connect(self.createCircleClick)
-        self.createLabelAction.triggered.connect(self.createSymbolLabelDialogue)
-        self.createPinAction.triggered.connect(self.createPinClick)
-        self.objPropAction.triggered.connect(self.objPropClick)
-        self.copyAction.triggered.connect(self.copyClick)
-        self.redoAction.triggered.connect(self.redoClick)
-        self.undoAction.triggered.connect(self.undoClick)
-        self.rotateAction.triggered.connect(self.rotateItemClick)
-        self.deleteAction.triggered.connect(self.deleteClick)
-        self.stretchAction.triggered.connect(self.stretchClick)
-        self.viewPropAction.triggered.connect(self.viewPropClick)
-        super()._createTriggers()
-
-    def _symbolActions(self):
-        self.centralW.scene.itemContextMenu.addAction(self.copyAction)
-        self.centralW.scene.itemContextMenu.addAction(self.moveAction)
-        self.centralW.scene.itemContextMenu.addAction(self.rotateAction)
-        self.centralW.scene.itemContextMenu.addAction(self.stretchAction)
-        self.centralW.scene.itemContextMenu.addAction(self.deleteAction)
-        self.centralW.scene.itemContextMenu.addAction(self.objPropAction)
-
-    def objPropClick(self):
-        self.centralW.scene.itemProperties()
-
-    def checkSaveCell(self):
-        self.centralW.scene.saveSymbolCell(self.file)
-
-    def createRectClick(self, s):
-        self.setDrawMode(False, False, False, True, False, False, False)
-
-    def createLineClick(self, s):
-        self.setDrawMode(False, False, False, False, True, False, False)
-
-    def createPolyClick(self, s):
-        pass
-
-    def createArcClick(self, s):
-        self.setDrawMode(False, False, True, False, False, False, False)
-
-    def createCircleClick(self, s):
-        self.setDrawMode(False, False, False, False, False, False, True)
-
-    def createPinClick(self, s):
-        createPinDlg = pdlg.createPinDialog(self)
-        if createPinDlg.exec() == QDialog.Accepted:
-            self.centralW.scene.pinName = createPinDlg.pinName.text()
-            self.centralW.scene.pinType = createPinDlg.pinType.currentText()
-            self.centralW.scene.pinDir = createPinDlg.pinDir.currentText()
-            self.setDrawMode(True, False, False, False, False, False, False)
-
-    def rotateItemClick(self, s):
-        self.centralW.scene.rotateItem = True
-        self.centralW.scene.selectItem = False
-        self.messageLine.setText("Click on an item to rotate CW 90 degrees.")
-
-    def undoClick(self, s):
-        self.centralW.scene.undoStack.undo()
-
-    def redoClick(self, s):
-        self.centralW.scene.undoStack.redo()
-
-    def deleteClick(self, s):
-        self.centralW.scene.deleteSelectedItems()
-
-    def copyClick(self, s):
-        self.centralW.scene.copySelectedItems()
-
-    def stretchClick(self, s):
-        self.centralW.scene.stretchSelectedItem()
-
-    def viewPropClick(self, s):
-        self.centralW.scene.viewSymbolProperties()
-
-    def setDrawMode(self, *args):
-        """
-        Sets the drawing mode in the symbol editor.
-        """
-        self.centralW.scene.drawPin = args[0]
-        self.centralW.scene.selectItem = args[1]
-        self.centralW.scene.drawArc = args[2]  # draw arc
-        self.centralW.scene.drawRect = args[3]  # draw rect
-        self.centralW.scene.drawLine = args[4]  # draw line
-        self.centralW.scene.addLabel = args[5]
-        self.centralW.scene.drawCircle = args[6]
-        if hasattr(self.centralW.scene, "start"):
-            del self.centralW.scene.start
-
-    def loadSymbol(self):
-        """
-        symbol is loaded to the scene.
-        """
-        with open(self.file) as tempFile:
-            items = json.load(tempFile)
-        self.centralW.scene.loadSymbol(items)
-
-    def createSymbolLabelDialogue(self):
-        createLabelDlg = pdlg.createSymbolLabelDialog(self)
-        if createLabelDlg.exec() == QDialog.Accepted:
-            self.setDrawMode(False, False, False, False, False, True, False)
-            # directly setting scene class attributes here to pass the information.
-            self.centralW.scene.labelDefinition = createLabelDlg.labelDefinition.text()
-            self.centralW.scene.labelHeight = (
-                createLabelDlg.labelHeightEdit.text().strip())
-            self.centralW.scene.labelAlignment = (
-                createLabelDlg.labelAlignCombo.currentText())
-            self.centralW.scene.labelOrient = (
-                createLabelDlg.labelOrientCombo.currentText())
-            self.centralW.scene.labelUse = createLabelDlg.labelUseCombo.currentText()
-            if createLabelDlg.labelVisiCombo.currentText() == "Yes":
-                self.centralW.scene.labelOpaque = True
-            else:
-                self.centralW.scene.labelOpaque = False
-            self.centralW.scene.labelType = "Normal"  # default button
-            if createLabelDlg.normalType.isChecked():
-                self.centralW.scene.labelType = "Normal"
-            elif createLabelDlg.NLPType.isChecked():
-                self.centralW.scene.labelType = "NLPLabel"
-            elif createLabelDlg.pyLType.isChecked():
-                self.centralW.scene.labelType = "PyLabel"
-
-    def closeEvent(self, event):
-        """
-        Closes the application.
-        """
-        self.centralW.scene.saveSymbolCell(self.file)
-        self.appMainW.openViews.pop(
-            f"{self.libName}_{self.cellName}_{self.viewName}")
-        event.accept()
-
-
-class symbolContainer(QWidget):
-    def __init__(self, parent):
-        super().__init__(parent=parent)
-        self.parent = parent
-        self.scene = symbol_scene(self)
-        self.view = symbol_view(self.scene, self)
-        self.init_UI()
-
-    def init_UI(self):
-        # layout statements, using a grid layout
-        gLayout = QGridLayout()
-        gLayout.setSpacing(10)
-        gLayout.addWidget(self.view, 0, 0)
-        # ratio of first column to second column is 5
-        gLayout.setColumnStretch(0, 5)
-        gLayout.setRowStretch(0, 6)
-        self.setLayout(gLayout)
-
-
-class schematicContainer(QWidget):
-    def __init__(self, parent: schematicEditor):
-        super().__init__(parent=parent)
-        assert isinstance(parent, schematicEditor)
-        self.parent = parent
-        self.scene = schematic_scene(self)
-        self.view = schematic_view(self.scene, self)
-        self.init_UI()
-
-    def init_UI(self):
-        # layout statements, using a grid layout
-        gLayout = QGridLayout()
-        gLayout.setSpacing(10)
-        gLayout.addWidget(self.view, 0, 0)
-        # ratio of first column to second column is 5
-        gLayout.setColumnStretch(0, 5)
-        gLayout.setRowStretch(0, 6)
-        self.setLayout(gLayout)
-
-
-class editor_scene(QGraphicsScene):
-    def __init__(self, parent):
-        super().__init__(parent)
-        self.parent = parent
-        self.editor = self.parent.parent
-        self.majorGrid = self.editor.majorGrid
-        self.gridTuple = self.editor.gridTuple
-        self.selectedItems = None  # selected item
-        self.defineSceneLayers()
-        self.setPens()
-        self.undoStack = QUndoStack()
-        self.changeOrigin = False
-        self.origin = QPoint(0, 0)
-        self.cellName = self.editor.file.parent.stem
-        self.libraryDict = self.editor.libraryDict
-        self.rotateItem = False
-        self.itemContextMenu = QMenu()
-        self.appMainW = self.editor.appMainW
-        self.logger = self.appMainW.logger
-        self.messageLine = self.editor.messageLine
-        self.statusLine = self.editor.statusLine
-
-    def setPens(self):
-        self.wirePen = pens.pen.returnPen("wirePen")
-        self.symbolPen = pens.pen.returnPen("symbolPen")
-        self.selectedWirePen = pens.pen.returnPen("selectedWirePen")
-        self.pinPen = pens.pen.returnPen("pinPen")
-        self.labelPen = pens.pen.returnPen("labelPen")
-        self.textPen = pens.pen.returnPen("textPen")
-
-    def defineSceneLayers(self):
-        self.wireLayer = cel.wireLayer
-        self.symbolLayer = cel.symbolLayer
-        self.guideLineLayer = cel.guideLineLayer
-        self.selectedWireLayer = cel.selectedWireLayer
-        self.pinLayer = cel.pinLayer
-        self.labelLayer = cel.labelLayer
-        self.textLayer = cel.textLayer
-
-    def snapToBase(self, number, base):
-        '''
-        Restrict a number to the multiples of base
-        '''
-        return int(base * int(round(number / base)))
-
-    def snapToGrid(self, point: QPoint, gridTuple: tuple[int, int]):
-        """
-        snap point to grid. Divides and multiplies by grid size.
-        """
-        return QPoint(int(gridTuple[0] * int(round(point.x() / gridTuple[0]))),
-                      int(gridTuple[1] * int(round(point.y() / gridTuple[1]))))
-
-    def rotateSelectedItems(self, point: QPoint):
-        """
-        Rotate selected items by 90 degree.
-        """
-        for item in self.selectedItems:
-            self.rotateAnItem(point, item, 90)
-        self.rotateItem = False
-        self.itemSelect = True
-
-    def rotateAnItem(self, point: QPoint, item, angle):
-        rotationOriginPoint = item.mapFromScene(point)
-        item.setTransformOriginPoint(rotationOriginPoint)
-        item.angle += angle
-        item.setRotation(item.angle)
-        undoCommand = us.undoRotateShape(self, item, item.angle)
-        self.undoStack.push(undoCommand)
-
-
-class symbol_scene(editor_scene):
-    """
-    Scene for Symbol editor.
-    """
-
-    def __init__(self, parent):
-        super().__init__(parent)
-        # drawing switches
-        self.resetSceneMode()  # reset to select mode
-        # pen definitions
-        self.setPens()
-        self.draftPen = QPen(self.guideLineLayer.color, 1)
-        self.drawPin = False
-        self.itemSelect = True
-        self.drawArc = False  # draw arc
-        self.drawRect = False
-        self.drawLine = False
-        self.addLabel = False
-        self.drawCircle = False
-        self.drawMode = (
-                self.drawLine or self.drawArc or self.drawRect or self.drawCircle)
-        self.symbolShapes = ["line", "arc", "rect", "circle", "pin", "label"]
-        self.changeOrigin = False
-        self.origin = QPoint(0, 0)
-        # some default attributes
-        self.pinName = ""
-        self.pinType = shp.pin.pinTypes[0]
-        self.pinDir = shp.pin.pinDirs[0]
-        self.labelDefinition = ""
-        self.labelType = shp.label.labelTypes[0]
-        self.labelOrient = shp.label.labelOrients[0]
-        self.labelAlignment = shp.label.labelAlignments[0]
-        self.labelUse = shp.label.labelUses[0]
-        self.labelVisible = False
-        self.labelHeight = "12"
-        self.labelOpaque = True
-
-    def mousePressEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
-        super().mousePressEvent(mouse_event)
-        if mouse_event.button() == Qt.LeftButton:
-            eventScenePos = mouse_event.scenePos()
-            self.start = self.snapToGrid(eventScenePos.toPoint(), self.gridTuple)
-            if self.changeOrigin:  # change origin of the symbol
-                self.origin = self.start
-            if self.itemSelect:
-                self.messageLine.setText("Select an item")
-                #     # find the view rectangle every time mouse is pressed.
-                self.viewRect = self.parent.view.mapToScene(
-                    self.parent.view.viewport().rect()).boundingRect()
-                itemsAtMousePress = self.items(eventScenePos)
-                if itemsAtMousePress:
-                    self.selectedItems = [item for item in itemsAtMousePress if
-                                          item.isSelected()]
-                    self.messageLine.setText("Item selected")
-                else:
-                    self.selectedItems = None
-                    self.parent.parent.messageLine.setText("Nothing selected")
-            if self.drawPin:
-                if hasattr(self, "draftPin"):
-                    self.removeItem(self.draftPin)
-                self.draftPin = shp.pin(self.start, self.draftPen, "", "Input",
-                                        "Signal", self.gridTuple, )
-                self.addItem(self.draftPin)
-                self.draftPin.setSelected(True)
-            if self.addLabel:
-                if hasattr(self, "draftLabel"):
-                    self.removeItem(self.draftLabel)
-                self.draftLabel = shp.label(self.start, self.draftPen, "12",
-                                            self.gridTuple, )
-                self.addItem(self.draftLabel)
-                self.draftLabel.setSelected(True)
-            if self.rotateItem:
-                if self.selectedItems:
-                    self.rotateSelectedItems(self.start)
-
-    def mouseMoveEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
-        super().mouseMoveEvent(mouse_event)
-        eventScenePos = mouse_event.scenePos()
-        self.current = self.snapToGrid(eventScenePos.toPoint(), self.gridTuple)
-        modifiers = QGuiApplication.keyboardModifiers()
-        if mouse_event.buttons() == Qt.LeftButton:
-            if hasattr(self, "draftItem"):
-                self.removeItem(self.draftItem)
-                del self.draftItem
-            # if hasattr(self, "draftRect"):
-            #     self.removeItem(self.draftRect)
-            if self.drawLine and hasattr(self, "start"):
-                self.parent.parent.messageLine.setText("Line Mode")
-                self.draftItem = shp.line(self.start, self.current, self.draftPen,
-                                          self.gridTuple)
-                self.addItem(self.draftItem)
-            if self.drawRect and hasattr(self, "start"):
-                self.draftItem = shp.rectangle(self.start, self.current,
-                                               self.draftPen, self.gridTuple)
-                self.addItem(self.draftItem)
-            if self.drawCircle and hasattr(self, "start"):
-                xlen = abs(self.current.x() - self.start.x())
-                ylen = abs(self.current.y() - self.start.y())
-                length = math.sqrt(xlen ** 2 + ylen ** 2)
-                self.draftItem = QGraphicsEllipseItem(
-                    QRectF(self.start - QPoint(int(length), int(length)),
-                           self.start + QPoint(int(length), int(length)), ))
-                self.draftItem.setPen(self.draftPen)
-                self.addItem(self.draftItem)
-            if self.drawArc and hasattr(self, "start"):
-                self.draftItem = shp.arc(self.start, self.current, self.draftPen,
-                                         self.gridTuple)
-                # self.draftRect = shp.rectangle(self.start,self.current, self.draftPen,
-                #                                self.gridTuple)
-                self.addItem(self.draftItem)  # self.addItem(self.draftRect)
-            if self.itemSelect:
-                if modifiers == Qt.ShiftModifier:
-                    self.draftItem = QGraphicsRectItem(
-                        QRect.span(self.start, self.current))
-                    self.draftItem.setPen(self.draftPen)
-                    self.addItem(self.draftItem)
-                    self.messageLine.setText("Select an Area")
-
-        self.statusLine.showMessage(
-            "Cursor Position: " + str((self.current - self.origin).toTuple()))
-
-    def mouseReleaseEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
-        super().mouseReleaseEvent(mouse_event)
-        eventScenePos = mouse_event.scenePos()
-        self.current = self.snapToGrid(eventScenePos.toPoint(), self.gridTuple)
-        if mouse_event.button() == Qt.LeftButton:
-            if (self.itemSelect and hasattr(self, "draftItem") and isinstance(
-                    self.draftItem, QGraphicsRectItem)):
-                self.selectedItems = [item for item in
-                                      self.items(self.draftItem.rect(),
-                                                 mode=Qt.IntersectsItemBoundingRect)]
-                for item in self.selectedItems:
-                    item.setSelected(True)
-            if self.drawLine and hasattr(self, "start"):
-                self.lineDraw(self.start, self.current, self.symbolPen,
-                              self.gridTuple)
-
-            if self.drawRect and hasattr(self, "start"):
-                self.rectDraw(self.start, self.current, self.symbolPen,
-                              self.gridTuple)
-
-            if self.drawCircle and hasattr(self, "start"):
-                self.circleDraw(self.start, self.current, self.symbolPen,
-                                self.gridTuple)
-
-            if self.drawArc and hasattr(self, 'start'):
-                self.arcDraw(self.start, self.current, self.symbolPen,
-                             self.gridTuple)
-            if self.drawPin and hasattr(self, "draftPin"):
-                self.pinDraw(self.current, self.pinPen, self.pinName, self.pinDir,
-                             self.pinType, self.gridTuple, )  # draw pin
-
-            if self.addLabel and hasattr(self, "draftLabel"):
-                self.labelDraw(self.current, self.labelPen, self.labelDefinition,
-                               self.gridTuple, self.labelType, self.labelHeight,
-                               self.labelAlignment, self.labelOrient,
-                               self.labelUse, )  # draw label
-
-            if hasattr(self, "draftItem"):
-                self.removeItem(self.draftItem)
-                del self.draftItem
-            elif hasattr(self, "draftPin"):
-                self.removeItem(self.draftPin)
-                del self.draftPin
-            elif hasattr(self, "draftLabel"):
-                self.removeItem(self.draftLabel)
-                del self.draftLabel  # if hasattr(self,"draftRect"):  #     self.removeItem(self.draftRect)  # del self.draftRect
-            if self.changeOrigin:
-                self.changeOrigin = False
-            self.itemSelect = True
-
-    def lineDraw(self, start: QPoint, current: QPoint, pen: QPen,
-                 gridTuple: tuple):
-        line = shp.line(start, current, pen, gridTuple)
-        self.addItem(line)
-        undoCommand = us.addShapeUndo(self, line)
-        self.undoStack.push(undoCommand)
-        self.drawLine = False
-        return line
-
-    def rectDraw(self, start: QPoint, end: QPoint, pen: QPen, gridTuple: tuple):
-        """
-        Draws a rectangle on the scene
-        """
-        rect = shp.rectangle(start,
-                             end - QPoint(pen.width() / 2, pen.width() / 2), pen,
-                             gridTuple)
-        self.addItem(rect)
-        undoCommand = us.addShapeUndo(self, rect)
-        self.undoStack.push(undoCommand)
-        self.drawRect = False
-        return rect
-
-    def circleDraw(self, start: QPoint, end: QPoint, pen: QPen,
-                   gridTuple: tuple[int, int]):
-        """
-        Draws a circle on the scene
-        """
-        snappedEnd = self.snapToGrid(end, gridTuple)
-        circle = shp.circle(start, snappedEnd, pen, gridTuple)
-        self.addItem(circle)
-        undoCommand = us.addShapeUndo(self, circle)
-        self.undoStack.push(undoCommand)
-        self.drawCircle = False
-        return circle
-
-    def arcDraw(self, start: QPoint, end: QPoint, pen: QPen,
-                gridTuple: tuple[int, int]):
-        '''
-        Draws an arc inside the rectangle defined by start and end points.
-        '''
-        arc = shp.arc(start, end, pen, gridTuple)
-        self.addItem(arc)
-        undoCommand = us.addShapeUndo(self, arc)
-        self.undoStack.push(undoCommand)
-        self.drawArc = False
-        return arc
-
-    def pinDraw(self, current, pen: QPen, pinName: str, pinDir, pinType,
-                gridTuple: tuple):
-        pin = shp.pin(current, pen, pinName, pinDir, pinType, gridTuple)
-        self.addItem(pin)
-        undoCommand = us.addShapeUndo(self, pin)
-        self.undoStack.push(undoCommand)
-        self.drawPin = False
-        return pin
-
-    def labelDraw(self, current, pen: QPen, labelDefinition, gridTuple, labelType,
-                  labelHeight, labelAlignment, labelOrient, labelUse, ):
-        label = shp.label(current, pen, labelDefinition, gridTuple, labelType,
-                          labelHeight, labelAlignment, labelOrient, labelUse, )
-        label.labelVisible = self.labelOpaque
-        label.setLabelName()  # set the name
-        label.setOpacity(1)
-        self.addItem(label)
-        undoCommand = us.addShapeUndo(self, label)
-        self.undoStack.push(undoCommand)
-        self.addLabel = False
-        return label
-
-    def keyPressEvent(self, key_event):
-        super().keyPressEvent(key_event)
-        if key_event.key() == Qt.Key_Escape:
-            self.resetSceneMode()
-        elif key_event.key() == Qt.Key_C:
-            self.copySelectedItems()
-        elif key_event.key() == Qt.Key_M:
-            self.stretchSelectedItem()  # elif key_event.key() == Qt.Key_Up:  #     selectedItemsCount = len(self.itemsAtMousePress)  #     if self.selectCount == selectedItemsCount:  #         self.selectCount = 0  #         self.changeSelection(self.selectCount)  #         self.selectCount += 1  #     elif self.selectCount < selectedItemsCount:  #         self.changeSelection(self.selectCount)  #         self.selectCount += 1
-
-    # def changeSelection(self, i):
-    #     """
-    #     Change the selected item.
-    #     """
-    #     self.selectedItem.setSelected(False)
-    #     self.selectedItem = self.itemsAtMousePress[i]
-    #     self.selectedItem.setSelected(True)
-
-    def resetSceneMode(self):
-        """
-        Reset the scene mode to default. Select mode is set to True.
-        """
-        self.drawItem = False  # flag to indicate if an item is being drawn
-        self.drawLine = False  # flag to indicate if a line is being drawn
-        self.drawArc = False  # flag to indicate if an arc is being drawn
-        self.drawPin = False  # flag to indicate if a pin is being drawn
-        self.drawRect = False  # flag to indicate if a rectangle is being drawn
-        self.addLabel = False  # flag to indicate if a label is being drawn
-        self.selectCount = 0  # index of item selected
-        self.selectedItems = None
-        if hasattr(self, "draftItem"):
-            self.removeItem(self.draftItem)
-        self.itemSelect = True
-
-    def deleteSelectedItems(self):
-        if self.selectedItems:
-            for item in self.selectedItems:
-                self.removeItem(item)
-            del self.selectedItems
-            self.update()
-            self.itemSelect = True
-
-    def copySelectedItems(self):
-        if hasattr(self, "selectedItems"):
-            for item in self.selectedItems:
-                selectedItemJson = json.dumps(item, cls=se.symbolEncoder)
-                itemCopyDict = json.loads(selectedItemJson)
-                shape = lj.createSymbolItems(itemCopyDict, self.gridTuple)
-                self.addItem(shape)
-                undoCommand = us.addShapeUndo(self, shape)
-                self.undoStack.push(undoCommand)
-                # shift position by one grid unit to right and down
-                shape.setPos(QPoint(item.pos().x() + 2 * self.gridTuple[0],
-                                    item.pos().y() + 2 * self.gridTuple[1], ))
-
-    def itemProperties(self):
-        """
-        When item properties is queried.
-        """
-        if self.selectedItems:
-            for item in self.selectedItems:
-                if isinstance(item, shp.rectangle):
-                    self.queryDlg = pdlg.rectPropertyDialog(self.editor, item)
-                    if self.queryDlg.exec() == QDialog.Accepted:
-                        self.updateRectangleShape(item)
-                if isinstance(item, shp.circle):
-                    self.queryDlg = pdlg.circlePropertyDialog(self.editor, item)
-                    if self.queryDlg.exec() == QDialog.Accepted:
-                        self.updateCircleShape(item)
-                if isinstance(item, shp.arc):
-                    self.queryDlg = pdlg.arcPropertyDialog(self.editor, item)
-                    if self.queryDlg.exec() == QDialog.Accepted:
-                        self.updateArcShape(item)
-                elif isinstance(item, shp.line):
-                    self.queryDlg = pdlg.linePropertyDialog(self.editor, item)
-                    if self.queryDlg.exec() == QDialog.Accepted:
-                        self.updateLineShape(item)
-                elif isinstance(item, shp.pin):
-                    self.queryDlg = pdlg.pinPropertyDialog(self.editor, item)
-                    if self.queryDlg.exec() == QDialog.Accepted:
-                        self.updatePinShape(item)
-                elif isinstance(item, shp.label):
-                    self.queryDlg = pdlg.labelPropertyDialog(self.editor, item)
-                    if self.queryDlg.exec() == QDialog.Accepted:
-                        self.updateLabelShape(item)
-
-    def updateRectangleShape(self, item: shp.rectangle):
-        left = self.snapToBase(float(self.queryDlg.rectLeftLine.text()),
-                               self.gridTuple[0])
-        top = self.snapToBase(float(self.queryDlg.rectTopLine.text()),
-                              self.gridTuple[1])
-        width = self.snapToBase(float(self.queryDlg.rectWidthLine.text()),
-                                self.gridTuple[0])
-        height = self.snapToBase(float(self.queryDlg.rectHeightLine.text()),
-                                 self.gridTuple[1])
-        topLeft = item.mapFromScene(QPoint(left, top))
-        # undoUpdateRectangle = us.updateShapeUndo()
-        # us.keepOriginalShape(self, item, self.gridTuple, parent=undoUpdateRectangle)
-        item.rect = QRect(topLeft.x(), topLeft.y(), width, height)
-
-        # us.changeOriginalShape(self, item, parent=undoUpdateRectangle)
-        # self.undoStack.push(undoUpdateRectangle)
-        # self.selectedItem.update()
-
-    def updateCircleShape(self, item: shp.circle):
-
-        centerX = self.snapToBase(float(self.queryDlg.centerXEdit.text()),
-                                  self.gridTuple[0])
-        centerY = self.snapToBase(float(self.queryDlg.centerYEdit.text()),
-                                  self.gridTuple[1])
-        radius = self.snapToBase(float(self.queryDlg.radiusEdit.text()),
-                                 self.gridTuple[0])
-        centerPoint = self.snapToGrid(QPoint(centerX, centerY), self.gridTuple)
-        item.centre(self.selectedItem.mapFromScene(centerPoint))
-        item.radius(radius)
-
-    def updateArcShape(self, item: shp.arc):
-
-        startX = self.snapToBase(float(self.queryDlg.startXEdit.text()),
-                                 self.gridTuple[0])
-        startY = self.snapToBase(float(self.queryDlg.startYEdit.text()),
-                                 self.gridTuple[1])
-        item.start = item.mapFromScene(QPoint(startX, startY)).toPoint()
-        item.width = self.snapToBase(float(self.queryDlg.widthEdit.text()),
-                                     self.gridTuple[0])
-        item.height = self.snapToBase(float(self.queryDlg.heightEdit.text()),
-                                      self.gridTuple[1])
-
-    def updateLineShape(self, item: shp.line):
-        """
-        Updates line shape from dialogue entries.
-        """
-        startEntry = QPoint(int(float(self.queryDlg.startXLine.text())),
-                            int(float(self.queryDlg.startYLine.text())), )
-        item.start = item.mapFromScene(startEntry).toPoint()
-        endEntry = QPoint(int(float(self.queryDlg.endXLine.text())),
-                          int(float(self.queryDlg.endYLine.text())), )
-        item.end = item.mapFromScene(endEntry).toPoint()
-
-    def updatePinShape(self, item: shp.pin):
-        location = item.scenePos().toTuple()
-        item.start = self.snapToGrid(
-            QPoint(int(float(self.queryDlg.pinXLine.text()) - float(location[0])),
-                   int(float(self.queryDlg.pinYLine.text()) - float(
-                       location[1])), ), self.gridTuple, )
-        item.rect = QRect(self.selectedItem.start.x() - 5,
-                          self.selectedItem.start.y() - 5, 10, 10)
-        item.pinName = self.queryDlg.pinName.text()
-        item.pinType = self.queryDlg.pinType.currentText()
-        item.pinDir = self.queryDlg.pinDir.currentText()
-        item.update()
-
-    def updateLabelShape(self, item: shp.label):
-        """
-        update pin shape with new values.
-        """
-        location = item.scenePos().toTuple()
-        item.start = self.snapToGrid(
-            QPoint(int(float(self.queryDlg.labelXLine.text()) - float(location[0])),
-                   int(float(self.queryDlg.labelYLine.text()) - float(
-                       location[1])), ), self.gridTuple, )
-        item.labelDefinition = self.queryDlg.labelDefinition.text()
-        item.labelHeight = self.queryDlg.labelHeightEdit.text()
-        item.labelAlign = self.queryDlg.labelAlignCombo.currentText()
-        item.labelOrient = self.queryDlg.labelOrientCombo.currentText()
-        item.labelUse = self.queryDlg.labelUseCombo.currentText()
-        if self.queryDlg.labelVisiCombo.currentText() == "Yes":
-            item.labelVisible = True
-        else:
-            item.labelVisible = False
-        if self.queryDlg.normalType.isChecked():
-            item.labelType = shp.label.labelTypes[0]
-        elif self.queryDlg.NLPType.isChecked():
-            item.labelType = shp.label.labelTypes[1]
-        elif self.queryDlg.pyLType.isChecked():
-            item.labelType = shp.label.labelTypes[2]
-        # set opacity to 1 so that the label is still visible on symbol editor
-        item.setOpacity(1)
-        item.setLabelName()
-        item.update()
-
-    def loadSymbol(self, itemsList: list):
-        self.attributeList = []
-        for item in itemsList[1:]:
-            if item is not None:
-                if item["type"] in self.symbolShapes:
-                    itemShape = lj.createSymbolItems(item, self.gridTuple)
-                    # items should be always visible in symbol view
-                    if isinstance(itemShape, shp.label):
-                        itemShape.setOpacity(1)
-                    print(item['type'])
-                    self.addItem(itemShape)
-                elif item["type"] == "attr":
-                    attr = lj.createSymbolAttribute(item)
-                    self.attributeList.append(attr)
-
-    def saveSymbolCell(self, fileName):
-        # items = self.items(self.sceneRect())  # get items in scene rect
-        items = self.items()
-        items.insert(0, {"cellView": "symbol"})
-        if hasattr(self, "attributeList"):
-            items.extend(self.attributeList)  # add attribute list to list
-        with open(fileName, "w") as f:
-            try:
-                json.dump(items, f, cls=se.symbolEncoder, indent=4)
-            except Exception as e:
-                self.logger.error(e)
-
-    def stretchSelectedItem(self):
-        if self.selectedItems is not None:
-            try:
-                for item in self.selectedItems:
-                    if hasattr(item, 'stretch'):
-                        item.stretch = True
-
-            except AttributeError:
-                self.messageLine.setText("Nothing selected")
-
-    def viewSymbolProperties(self):
-        """
-        View symbol properties dialog.
-        """
-        # copy symbol attribute list to another list by deepcopy to be safe
-        attributeListCopy = deepcopy(self.attributeList)
-        symbolPropDialogue = pdlg.symbolLabelsDialogue(self.parent.parent,
-                                                       self.items(),
-                                                       attributeListCopy)
-        if symbolPropDialogue.exec() == QDialog.Accepted:
-            for i, item in enumerate(symbolPropDialogue.labelItemList):
-                # label name is not changed.
-                item.labelHeight = symbolPropDialogue.labelHeightList[i].text()
-                item.labelAlign = symbolPropDialogue.labelAlignmentList[
-                    i].currentText()
-                item.labelOrient = symbolPropDialogue.labelOrientationList[
-                    i].currentText()
-                item.labelUse = symbolPropDialogue.labelUseList[i].currentText()
-                item.labelType = symbolPropDialogue.labelTypeList[i].currentText()
-                item.update(item.boundingRect())
-            # create an empty attribute list. If the dialog is OK, the local attribute list
-            # will be copied to the symbol attribute list.
-            localAttributeList = []
-            for i, item in enumerate(symbolPropDialogue.attributeNameList):
-                if item.text().strip() != "":
-                    localAttributeList.append(se.symbolAttribute(item.text(),
-                                                                 symbolPropDialogue.attributeDefList[
-                                                                     i].text()))
-                self.attributeList = deepcopy(localAttributeList)
-
-
-class schematic_scene(editor_scene):
-    def __init__(self, parent):
-        super().__init__(parent)
-        self.parent = parent
-        self.schematicWindow = self.parent.parent
-        self.instCounter = 0
-        self.mousePressLoc = QPoint(0, 0)
-        self.mouseMoveLoc = QPoint(0, 0)
-        self.mouseReleaseLoc = QPoint(0, 0)
-        self.start = QPoint(0, 0)
-        self.current = QPoint(0, 0)
-        self.selectedItems = None
-        self.itemsAtMousePress = list()
-        self.itemContextMenu = QMenu()
-        self.drawWire = False  # flag to add wire
-        self.drawPin = False  # flag to add pin
-        self.drawText = False  # flat to add text
-        self.itemSelect = True  # flag to select item
-        self.drawMode = self.drawWire or self.drawPin
-        self.draftPen = QPen(self.guideLineLayer.color, 1)
-        self.draftPen.setStyle(Qt.DashLine)
-        self.draftPin = None
-        self.draftText = None
-        self.itemCounter = 0
-        self.netCounter = 0
-        # self.pinLocations = self.pinLocs()  # dictionary to store pin locations
-        self.schematicNets = {}  # netName: list of nets with the same name
-        self.crossDots = set()  # list of cross dots
-        self.draftItem = None
-        self.viewRect = QRect(0, 0, 0, 0)
-        self.viewportCrossDots = (
-            set())  # an empty set of crossing points in the viewport
-        self.sceneCrossDots = set()  # an empty set of all crossing points in the scene
-        self.crossDotsMousePress = (
-            set())  # a temporary set to hold the crossdots locations
-        # add instance attributes
-        self.addInstance = False
-        self.instanceSymbolFile = None
-        # pin attribute defaults
-        self.pinName = ""
-        self.pinType = "Signal"
-        self.pinDir = "Input"
-        self.parentView = None
-
-    def mousePressEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
-        super().mousePressEvent(mouse_event)
-        if mouse_event.button() == Qt.LeftButton:
-            self.mousePressLoc = mouse_event.scenePos().toPoint()
-            self.start = self.snapToGrid(self.mousePressLoc, self.gridTuple)
-            if self.changeOrigin:  # change origin of the symbol
-                self.origin = self.start
-            elif self.itemSelect:
-                self.parent.parent.messageLine.setText("Select an item")
-                #     # find the view rectangle every time mouse is pressed.
-                self.viewRect = self.parent.view.mapToScene(
-                    self.parent.view.viewport().rect()).boundingRect()
-                itemsAtMousePress = self.items(mouse_event.scenePos())
-                if itemsAtMousePress:
-                    # normally only one item is selected
-                    self.selectedItems = [item for item in itemsAtMousePress if
-                                          item.isSelected()]
-                    self.parent.parent.messageLine.setText("Item selected")
-                else:
-                    self.selectedItems = None
-                    self.parent.parent.messageLine.setText("Nothing selected")
-            elif self.drawPin:
-                self.draftPin = shp.schematicPin(self.start, self.draftPen,
-                                                 self.pinName, self.pinDir,
-                                                 self.pinType, self.gridTuple, )
-                self.addItem(self.draftPin)
-            elif self.drawText:
-                self.draftText = shp.text(self.start, self.draftPen,
-                                          self.noteText, self.gridTuple,
-                                          self.noteFontFamily, self.noteFontStyle,
-                                          self.noteFontSize, self.noteAlign,
-                                          self.noteOrient, )
-                self.rotateAnItem(self.start, self.draftText,
-                                  float(self.noteOrient[1:]))
-                self.addItem(self.draftText)
-            elif self.rotateItem:
-                if self.selectedItems:
-                    self.rotateSelectedItems(self.start)
-
-    def mouseMoveEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
-        super().mouseMoveEvent(mouse_event)
-        self.mouseMoveLoc = mouse_event.scenePos().toPoint()
-        self.current = self.snapToGrid(self.mouseMoveLoc, self.gridTuple)
-        modifiers = QGuiApplication.keyboardModifiers()
-        if mouse_event.buttons() == Qt.LeftButton:
-            if hasattr(self, "draftItem"):
-                self.removeItem(self.draftItem)
-                del self.draftItem
-            if self.drawWire and hasattr(self, "start"):
-                self.parent.parent.messageLine.setText("Wire Mode")
-                self.draftItem = net.schematicNet(self.start, self.current,
-                                                  self.draftPen)
-                self.addItem(self.draftItem)
-            elif self.itemSelect:
-                if modifiers == Qt.ShiftModifier:
-                    self.draftItem = QGraphicsRectItem(
-                        QRect.span(self.start, self.current))
-                    self.draftItem.setPen(self.draftPen)
-                    self.addItem(self.draftItem)
-                    self.parent.parent.messageLine.setText("Select an Area")
-            elif self.drawPin:
-                self.draftPin.setPos(
-                    self.snapToGrid(self.mouseMoveLoc - self.mousePressLoc,
-                                    self.gridTuple))
-            elif self.drawText:
-                self.draftText.setPos(
-                    self.snapToGrid(self.mouseMoveLoc - self.mousePressLoc,
-                                    self.gridTuple))
-        self.parent.parent.statusLine.showMessage(
-            "Cursor Position: " + str(self.current.toTuple()))
-
-    def mouseReleaseEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
-        super().mouseReleaseEvent(mouse_event)
-        self.mouseReleaseLoc = mouse_event.scenePos().toPoint()
-        self.current = self.snapToGrid(self.mouseReleaseLoc, self.gridTuple)
-
-        if mouse_event.button() == Qt.LeftButton:
-            if self.addInstance:
-                instance = self.drawInstance(self.current)
-                instance.setSelected(True)
-                self.itemSelect = False
-                self.addInstance = False
-            elif self.drawText:
-                self.removeItem(self.draftText)
-                note = self.addNote(
-                    self.snapToGrid(self.mouseReleaseLoc, self.gridTuple))
-                self.rotateAnItem(self.current, note, float(self.noteOrient[1:]))
-                self.addItem(note)
-                note.setSelected(True)
-                self.parent.parent.messageLine.setText("Note added.")
-                self.drawText = False
-            elif self.drawPin:
-                self.removeItem(self.draftPin)
-                pin = self.addPin(
-                    self.snapToGrid(self.mouseReleaseLoc, self.gridTuple))
-                self.addItem(pin)
-                pin.setSelected(True)
-                self.parent.parent.messageLine.setText("Pin added")
-                self.drawPin = False
-            elif hasattr(self, "draftItem") and hasattr(self, "start"):
-                if self.itemSelect and isinstance(self.draftItem,
-                                                  QGraphicsRectItem):
-                    self.selectedItems = [item for item in
-                                          self.items(self.draftItem.rect(),
-                                                     mode=Qt.IntersectsItemBoundingRect)
-                                          if (item.childItems() or isinstance(
-                            item, net.schematicNet))]
-                    for item in self.selectedItems:
-                        item.setSelected(True)
-                if self.drawWire:
-                    drawnNet = self.netDraw(self.start, self.current,
-                                            self.wirePen)
-                    self.removeDotsInView(self.viewRect)
-                    self.mergeNets(drawnNet, self.viewRect)
-                    self.splitNets(self.viewRect)
-                    self.findDotPoints(self.viewRect)
-                    self.drawWire = False
-                self.removeItem(self.draftItem)
-                del self.draftItem
-                del self.start
-
-    def removeDotsInView(self, viewRect: QRect) -> None:
-        dotsInView = {item for item in self.items(viewRect) if
-                      isinstance(item, net.crossingDot)}
-        for dot in dotsInView:
-            self.removeItem(dot)
-            del dot
-        self.viewportCrossDots = set()
-
-    def findDotPoints(self, viewRect: QRect) -> None:
-        self.viewportCrossDots = set()  # empty the set.
-        netsInView = {item for item in self.items(viewRect) if
-                      isinstance(item, net.schematicNet)}
-        for netItem in netsInView:
-            netItemEnd = netItem.mapToScene(netItem.end)
-            for netItem2 in netsInView.difference({netItem, }):
-                netItem2Start = netItem.mapToScene(netItem2.start)
-                if ((netItem.horizontal and netItem2.horizontal) and (
-                        netItemEnd == netItem2Start) or (
-                        not (netItem.horizontal or netItem2.horizontal) and (
-                        netItemEnd == netItem2Start))):
-                    for netItem3 in netsInView.difference({netItem, }).difference(
-                            {netItem2, }):
-                        netItem3End = netItem3.mapToScene(netItem3.end)
-                        netItem3Start = netItem3.mapToScene(netItem3.start)
-                        if (netItemEnd == netItem3End) or (
-                                netItemEnd == netItem3Start):
-                            cornerPoint = netItemEnd.toPoint()
-                            self.viewportCrossDots.add(cornerPoint)
-
-        for cornerPoint in self.viewportCrossDots:
-            self.createCrossDot(cornerPoint, 3)
-
-    def mergeNets(self, drawnNet, viewRect: QRect) -> None:
-        # check any overlapping nets in the view
-        # editing is done in the view and thus there is no need to check all nets in the scene
-        horizontalNetsInView = {item for item in self.items(viewRect) if (
-                isinstance(item, net.schematicNet) and item.horizontal)}
-        verticalNetsInView = {item for item in self.items(viewRect) if (
-                isinstance(item, net.schematicNet) and not item.horizontal)}
-        dBNetRect = drawnNet.sceneBoundingRect()
-        if len(horizontalNetsInView) > 1 and drawnNet.horizontal:
-            for netItem in horizontalNetsInView - {drawnNet, }:
-                netItemBRect = netItem.sceneBoundingRect()
-                if dBNetRect.intersects(netItemBRect):
-                    mergedRect = dBNetRect.united(netItemBRect).toRect()
-                    self.removeItem(netItem)  # remove the old net from the scene
-                    self.removeItem(
-                        drawnNet)  # remove the drawn net from the scene
-                    mergedNet = self.netDraw(
-                        self.snapToGrid(mergedRect.bottomLeft(), self.gridTuple),
-                        self.snapToGrid(mergedRect.bottomRight(), self.gridTuple),
-                        self.wirePen, )
-                    horizontalNetsInView.discard(netItem)
-                    self.mergeNets(mergedNet, viewRect)
-                    self.parent.parent.messageLine.setText("Merged Nets")
-        elif len(verticalNetsInView) > 1 and not drawnNet.horizontal:
-            for netItem in verticalNetsInView - {drawnNet, }:
-                netItemBRect = netItem.sceneBoundingRect()
-                if dBNetRect.intersects(netItemBRect):
-                    mergedRect = dBNetRect.united(netItemBRect).toRect()
-                    self.removeItem(netItem)  # remove the old net from the scene
-                    self.removeItem(
-                        drawnNet)  # remove the drawn net from the scene
-                    mergedNet = self.netDraw(
-                        self.snapToGrid(mergedRect.bottomRight(), self.gridTuple),
-                        self.snapToGrid(mergedRect.topRight(), self.gridTuple),
-                        self.wirePen, )  # create a new net with the merged rectangle
-                    verticalNetsInView.discard(netItem)
-                    self.mergeNets(mergedNet, viewRect)
-                    self.parent.parent.messageLine.setText("Net merged")
-
-    def splitNets(self, viewRect: QRect) -> None:
-        horizontalNetsInView = {item for item in self.items(viewRect) if (
-                isinstance(item, net.schematicNet) and item.horizontal)}
-        verticalNetsInView = {item for item in self.items(viewRect) if (
-                isinstance(item, net.schematicNet) and not item.horizontal)}
-        addedNets = set()
-        for hNetItem in horizontalNetsInView:
-            verticalNetsInView = {item for item in self.items(viewRect) if (
-                    isinstance(item, net.schematicNet) and not item.horizontal)}
-            hNetBRect = hNetItem.sceneBoundingRect().toRect()
-            for vNetItem in verticalNetsInView:
-                vNetBRect = vNetItem.sceneBoundingRect().toRect()
-                if vNetBRect.intersects(hNetBRect):
-                    crossPoint = self.snapToGrid(
-                        vNetBRect.intersected(hNetBRect).center(), self.gridTuple)
-                    if crossPoint != vNetItem.end and crossPoint != vNetItem.start:
-                        addedNets.add((
-                            vNetItem.mapToScene(vNetItem.start).toPoint(),
-                            crossPoint))
-                        addedNets.add((crossPoint, vNetItem.mapToScene(
-                            vNetItem.end).toPoint()))
-                        self.removeItem(vNetItem)
-                        del vNetItem
-                        break
-        for vNetItem in verticalNetsInView:
-            horizontalNetsInView = {item for item in self.items(viewRect) if (
-                    isinstance(item, net.schematicNet) and item.horizontal)}
-            vNetBRect = vNetItem.sceneBoundingRect().toRect()
-            for hNetItem in horizontalNetsInView:
-                hNetBRect = hNetItem.sceneBoundingRect().toRect()
-                if hNetBRect.intersects(vNetBRect):
-                    crossPoint = self.snapToGrid(
-                        hNetBRect.intersected(vNetBRect).center(), self.gridTuple)
-                    if crossPoint != hNetItem.end and crossPoint != hNetItem.start:
-                        addedNets.add((
-                            hNetItem.mapToScene(hNetItem.start).toPoint(),
-                            crossPoint))
-                        addedNets.add((crossPoint, hNetItem.mapToScene(
-                            hNetItem.end).toPoint()))
-                        self.removeItem(hNetItem)
-                        del hNetItem
-                        break
-        for addedNet in addedNets:
-            self.netDraw(addedNet[0], addedNet[1], self.wirePen)
-
-    def createNetlist(self, netlistFile, writeNetlist: bool) -> None:
-        """
-        Creates a netlist from the schematic.
-        """
-        pass
-
-    def groupAllNets(self) -> None:
-        """
-        This method starting from nets connected to pins, then named nets and unnamed
-        nets, groups all the nets in the schematic.
-        """
-        # all the nets in the schematic in a set to remove duplicates
-        netsSceneSet = self.findSceneNetsSet()
-        # create a separate set of named nets.
-        # namedNetsSet = set()
-        # nets connected to pins. Netlisting will start from those nets
-        pinConNetsSet = set()
-        # first start from schematic pins
-        scenePinsSet = self.findScenePinsSet()
-
-        for scenePin in scenePinsSet:
-            for sceneNet in netsSceneSet:
-                if self.checkPinNetConnect(scenePin, sceneNet):
-                    if sceneNet.nameSet:
-                        if sceneNet.name == scenePin.pinName:
-                            pinConNetsSet.add(sceneNet)
-                        else:
-                            sceneNet.nameConflict = True
-                            self.parent.parent.logger.error(
-                                f"Net name conflict at {scenePin.pinName} of "
-                                f"{scenePin.parent.instanceName}.")
-                    else:
-                        pinConNetsSet.add(sceneNet)
-                        sceneNet.name = scenePin.pinName
-                    sceneNet.update()
-
-        # first propagate the net names to the nets connected to pins.
-        # first net set is left over nets.
-        notPinConnNets = self.groupNamedNets(pinConNetsSet,
-                                             netsSceneSet - pinConNetsSet)
-
-        # find all nets with nets set through net dialogue.
-        namedNetsSet = set([netItem for netItem in netsSceneSet - pinConNetsSet if
-                            netItem.nameSet])
-        # now remove already named net set from firstNetSet
-        unnamedNets = self.groupNamedNets(namedNetsSet,
-                                          notPinConnNets - namedNetsSet)
-        # for netItem in unnamedNets:
-        #     if not netItem.nameSet:
-        #         netItem.name = None  # empty all net names not set by the user
-        # now start netlisting from the unnamed nets
-        self.groupUnnamedNets(unnamedNets, self.netCounter)
-
-    def generatePinNetMap(self, sceneSymbolSet):
-        """
-        For symbols in sceneSymbolSet, find which pin is connected to which net. If a
-        pin is not connected, assign to it a default net starting with d prefix.
-        """
-        netCounter = 0
-        for symbolItem in sceneSymbolSet:
-            for pinName, pinItem in symbolItem.pins.items():
-                pinItem.connected = False  # clear connections
-                # find each symbol its pin locations and save it in pinLocations
-                # directory.
-                # symbolItem.pinLocations[pinName] = pinItem.sceneBoundingRect()
-                for netName, netItemSet in self.schematicNets.items():
-                    for netItem in netItemSet:
-                        if self.checkPinNetConnect(pinItem, netItem):
-                            symbolItem.pinNetMap[pinName] = netName
-                            pinItem.connected = True  # print(f'{symbolItem.instanceName}, {pinItem.pinName}')
-                if not pinItem.connected:
-                    # assign a default net name prefixed with d(efault).
-                    symbolItem.pinNetMap[pinName] = f"dnet{netCounter}"
-                    self.logger.error(
-                        f"left unconnected:{symbolItem.pinNetMap[pinName]}")
-                    netCounter += 1
-
-    def findSceneCells(self, symbolSet):
-        """
-        This function just goes through set of symbol items in the scene and
-        checks if that symbol's cell is encountered first time. If so, it adds
-        it to a dictionary   cell_name:symbol
-        """
-        symbolGroupDict = dict()
-        for symbolItem in symbolSet:
-            if symbolItem.cellName not in symbolGroupDict.keys():
-                symbolGroupDict[symbolItem.cellName] = symbolItem
-        return symbolGroupDict
-
-    def findSceneSymbolSet(self) -> set[shp.symbolShape]:
-        """
-        Find all the symbols on the scene as a set.
-        """
-        symbolSceneSet = {item for item in self.items() if
-                          isinstance(item, shp.symbolShape)}
-        return symbolSceneSet
-
-    def findSceneNetsSet(self) -> set[net.schematicNet]:
-        netsSceneSet = {item for item in self.items() if
-                        isinstance(item, net.schematicNet)}
-        return netsSceneSet
-
-    def findScenePinsSet(self) -> set[shp.schematicPin]:
-        pinsSceneSet = {item for item in self.items() if
-                        isinstance(item, shp.schematicPin)}
-        if pinsSceneSet:  # check pinsSceneSet is empty
-            return pinsSceneSet
-        else:
-            return set()
-
-    def findSceneTextSet(self) -> set[shp.text]:
-        textSceneSet = {item for item in self.items() if
-                        isinstance(item, shp.text)}
-        if textSceneSet:  # check textSceneSet is empty
-            return textSceneSet
-        else:
-            return set()
-
-    def groupNamedNets(self, namedNetsSet, unnamedNetsSet):
-        """
-        Groups nets with the same name.
-        """
-        for netItem in namedNetsSet:
-            if self.schematicNets.get(netItem.name) is None:
-                self.schematicNets[netItem.name] = set()
-            connectedNets, unnamedNetsSet = self.traverseNets({netItem, },
-                                                              unnamedNetsSet, )
-            self.schematicNets[netItem.name] |= connectedNets
-        # These are the nets not connected to any named net
-        return unnamedNetsSet
-
-    def groupUnnamedNets(self, unnamedNetsSet: set[net.schematicNet],
-                         nameCounter: int):
-        """
-        Groups nets together if they are connected and assign them default names
-        if they don't have a name assigned.
-        """
-        # select a net from the set and remove it from the set
-        try:
-            initialNet = (
-                unnamedNetsSet.pop())  # assign it a name, net0, net1, net2, etc.
-        except KeyError:  # initialNet set is empty
-            pass
-        else:
-            initialNet.name = "net" + str(nameCounter)
-            # now go through the set and see if any of the
-            # nets are connected to the initial net
-            # remove them from the set and add them to the initial net's set
-            self.schematicNets[
-                initialNet.name], unnamedNetsSet = self.traverseNets(
-                {initialNet, }, unnamedNetsSet, )
-            nameCounter += 1
-            if len(unnamedNetsSet) > 1:
-                self.groupUnnamedNets(unnamedNetsSet, nameCounter)
-            elif len(unnamedNetsSet) == 1:
-                lastNet = unnamedNetsSet.pop()
-                lastNet.name = "net" + str(nameCounter)
-                self.schematicNets[lastNet.name] = {lastNet}
-
-    def traverseNets(self, connectedSet, otherNetsSet):
-        """
-        Start from a net and traverse the schematic to find all connected nets. If the connected net search
-        is exhausted, remove those nets from the scene nets set and start again in another net until all
-        the nets in the scene are exhausted.
-        """
-        newFoundConnectedSet = set()
-        for netItem in connectedSet:
-            for netItem2 in otherNetsSet:
-                if self.checkConnect(netItem, netItem2):
-                    if (
-                            netItem2.nameSet and netItem.nameSet and netItem.name != netItem2.name):
-                        self.parent.parent.messageLine.setText(
-                            "Error: multiple names assigned to same net")
-                        netItem2.nameConflict = True
-                        netItem.nameConflict = True
-                        break
-                    else:
-                        netItem2.name = netItem.name
-                        netItem.nameConflict = False
-                        netItem2.nameConflict = False
-                    newFoundConnectedSet.add(netItem2)
-        # keep searching if you already found a net connected to the initial net
-        if len(newFoundConnectedSet) > 0:
-            connectedSet.update(newFoundConnectedSet)
-            otherNetsSet -= newFoundConnectedSet
-            self.traverseNets(connectedSet, otherNetsSet)
-        return connectedSet, otherNetsSet
-
-    def checkPinNetConnect(self, pinItem: shp.pin, netItem: net.schematicNet):
-        if pinItem.sceneBoundingRect().intersects(netItem.sceneBoundingRect()):
-            return True
-        else:
-            return False
-
-    def checkConnect(self, netItem, otherNetItem):
-        """
-        Determine if a net is connected to netItem.
-        """
-        netBRect = netItem.sceneBoundingRect()
-        if otherNetItem is not netItem:
-            otherBRect = otherNetItem.sceneBoundingRect()
-            if otherBRect.contains(
-                    netItem.mapToScene(netItem.start)) or otherBRect.contains(
-                netItem.mapToScene(netItem.end)):
-                return True
-            elif netBRect.contains(otherNetItem.mapToScene(
-                    otherNetItem.start)) or netBRect.contains(
-                otherNetItem.mapToScene(otherNetItem.end)):
-                return True
-            else:
-                return False
-
-    def createCrossDot(self, center: QPoint, radius: int):
-        crossDot = net.crossingDot(center, radius, self.wirePen)
-        self.addItem(crossDot)
-        return crossDot
-
-    def keyPressEvent(self, key_event):
-        if key_event.key() == Qt.Key_Escape:
-            self.resetSceneMode()
-        super().keyPressEvent(key_event)
-
-    def resetSceneMode(self):
-        self.itemSelect = True
-        self.drawWire = False
-        self.drawPin = False
-        self.selectedItems = []
-        self.parent.parent.messageLine.setText("Select Mode")
-
-    def netDraw(self, start: QPoint, current: QPoint,
-                pen: QPen) -> net.schematicNet:
-        line = net.schematicNet(start, current, pen)
-        self.addItem(line)
-        undoCommand = us.addShapeUndo(self, line)
-        self.undoStack.push(undoCommand)
-        return line
-
-    def addPin(self, pos: QPoint):
-        pin = shp.schematicPin(pos, self.pinPen, self.pinName, self.pinDir,
-                               self.pinType, self.gridTuple)
-        undoCommand = us.addShapeUndo(self, pin)
-        self.undoStack.push(undoCommand)
-        return pin
-
-    def addNote(self, pos: QPoint):
-        """
-        Changed the method name not to clash with qgraphicsscene addText method.
-        """
-        text = shp.text(pos, self.textPen, self.noteText, self.gridTuple,
-                        self.noteFontFamily, self.noteFontStyle,
-                        self.noteFontSize, self.noteAlign, self.noteOrient, )
-        undoCommand = us.addShapeUndo(self, text)
-        self.undoStack.push(undoCommand)
-        return text
-
-    def drawInstance(self, pos: QPoint):
-        """
-        Add an instance of a symbol to the scene.
-        """
-        instance = self.instSymbol(self.instanceSymbolFile, pos)
-        self.addItem(instance)
-        undoCommand = us.addShapeUndo(self, instance)
-        self.undoStack.push(undoCommand)
-        return instance
-
-    def instSymbol(self, file: pathlib.Path, pos: QPoint):
-        """
-        Read a symbol file and create symbolShape objects from it.
-        """
-        assert isinstance(file, pathlib.Path)
-        itemShapes = []
-        itemAttributes = {}
-        draftPen = QPen(self.guideLineLayer.color, 1)
-        with open(file, "r") as temp:
-            try:
-                items = json.load(temp)
-                if items[0]["cellView"] == "symbol":
-                    for item in items[1:]:
-                        if item["type"] == 'attr':
-                            itemAttributes[item["nam"]] = item["def"]
-                        else:
-                            itemShapes.append(lj.createSymbolItems(item,
-                                                               self.gridTuple))
-                        # if (item["type"] == "rect" or item["type"] == "line" or
-                        #         item["type"] == "pin" or item[
-                        #             "type"] == "label" or item[
-                        #             "type"] == "circle" or item["type"] == "arc"):
-                        #     # append recreated shapes to shapes list
-                        #     itemShapes.append(
-                        #         lj.createSymbolItems(item, self.gridTuple))
-                        # elif item["type"] == "attr":
-                        #     itemAttributes[item["nam"]] = item["def"]
-                else:
-                    self.logger.error("Not a symbol!")
-
-                # create a symbol instance passing item shapes and attributes as
-                # arguments
-                symbolInstance = shp.symbolShape(draftPen, self.gridTuple,
-                                                 itemShapes, itemAttributes)
-                symbolInstance.setPos(pos)
-                # For each instance assign a counter number from the scene
-                symbolInstance.counter = self.itemCounter
-                symbolInstance.instanceName = f"I{symbolInstance.counter}"
-                symbolInstance.libraryName = file.parent.parent.stem
-                symbolInstance.cellName = file.parent.stem
-                symbolInstance.viewName = "symbol"
-                for item in symbolInstance.labels.values():
-                    item.labelDefs()
-                return symbolInstance
-            except json.JSONDecodeError:
-                # print("Invalid JSON file")
-                self.logger.warning("Invalid JSON File")
-
-    def deleteSelectedItems(self):
-        try:
-            for item in self.selectedItems:
-                self.removeItem(item)
-            del self.selectedItems
-            self.update()
-            self.itemSelect = True
-        except TypeError:
-            pass
-
-    def copySelectedItems(self):
-        if self.selectedItems is not None:
-            for item in self.selectedItems:
-                selectedItemJson = json.dumps(item, cls=se.schematicEncoder)
-                itemCopyDict = json.loads(selectedItemJson)
-                print(itemCopyDict)
-                if isinstance(item, shp.symbolShape):
-                    self.itemCounter += 1
-                    itemCopyDict["name"] = f"I{self.itemCounter}"
-                    itemCopyDict["labelDict"]["instName"] = ["@instName",
-                                                             f"I{self.itemCounter}", ]
-                    shape = lj.createSchematicItems(itemCopyDict,
-                                                    self.libraryDict,
-                                                    item.viewName, self.gridTuple)
-
-                elif isinstance(item, net.schematicNet):
-                    shape = lj.createSchematicNets(itemCopyDict)
-                elif isinstance(item, shp.schematicPin):
-                    shape = lj.createSchematicPins(itemCopyDict, self.gridTuple)
-                self.addItem(shape)
-                # shift position by one grid unit to right and down
-                shape.setPos(QPoint(item.pos().x() + 4 * self.gridTuple[0],
-                                    item.pos().y() + 4 * self.gridTuple[1], ))
-                undoCommand = us.addShapeUndo(self, shape)
-                self.undoStack.push(undoCommand)
-
-    def saveSchematicCell(self, file: pathlib.Path):
-        self.sceneR = self.sceneRect()  # get scene rect
-        # items = self.items(self.sceneR)  # get items in scene rect
-        # only save symbol shapes
-        symbolItems = self.findSceneSymbolSet()
-        netItems = self.findSceneNetsSet()
-        pinItems = self.findScenePinsSet()
-        textItems = self.findSceneTextSet()
-        items = list(symbolItems | netItems | pinItems | textItems)
-        items.insert(0, {"cellView": "schematic"})
-        with open(file, "w") as f:
-            json.dump(items, f, cls=se.schematicEncoder, indent=4)
-        if self.parent.parent.parentView is not None:
-            if type(self.parentView) == schematicEditor:
-                self.parent.parent.parentView.loadSchematic()
-            elif type(self.parentView) == symbolEditor:
-                self.parent.parent.parentView.loadSymbol()
-
-    def loadSchematicCell(self, itemsList):
-        """
-        load schematic from item list
-        """
-        for item in itemsList[1:]:
-            if item is not None:
-                if item["type"] == "symbolShape":
-                    itemShape = lj.createSchematicItems(item, self.libraryDict,
-                                                        "symbol", self.gridTuple)
-                    self.addItem(itemShape)
-                    if itemShape.counter > self.itemCounter:
-                        self.itemCounter = itemShape.counter
-                elif item["type"] == "schematicNet":
-                    netShape = lj.createSchematicNets(item)
-                    self.addItem(netShape)
-                elif item["type"] == "schematicPin":
-                    pinShape = lj.createSchematicPins(item, self.gridTuple)
-                    self.addItem(pinShape)
-                elif item["type"] == "text":
-                    text = lj.createTextItem(item, self.gridTuple)
-                    self.addItem(text)
-
-        # increment item counter for next symbol
-        self.itemCounter += 1
-        self.findDotPoints(self.sceneRect())
-        # self.addItem(shp.text(QPoint(0, 200), self.textPen, 'Revolution EDA'))
-        self.update()
-
-    def viewObjProperties(self):
-        """
-        Display the properties of the selected object.
-        """
-
-        if self.selectedItems is not None:
-            for item in self.selectedItems:
-                if isinstance(item, shp.symbolShape):
-                    dlg = pdlg.instanceProperties(self.parent.parent, item)
-                    if dlg.exec() == QDialog.Accepted:
-                        item.libraryName = dlg.libNameEdit.text().strip()
-                        item.cellName = dlg.cellNameEdit.text().strip()
-                        item.viewName = dlg.viewNameEdit.text().strip()
-                        filePath = pathlib.Path(
-                            self.libraryDict[item.libraryName].joinpath(
-                                item.cellName, item.viewName + ".json"))
-                        item.instanceName = dlg.instNameEdit.text().strip()
-                        item.angle = float(dlg.angleEdit.text().strip())
-                        for label in item.labels.values():
-                            if label.labelDefinition == "[@instName]":
-                                label.labelValue = item.instanceName
-                            elif label.labelDefinition == "[@cellName]":
-                                label.labelValue = item.cellName
-                        location = self.snapToGrid(
-                            QPoint(float(dlg.xLocationEdit.text().strip()),
-                                   float(dlg.yLocationEdit.text().strip()), ),
-                            self.gridTuple, )
-                        item.setPos(location)
-                        tempDoc = QTextDocument()
-                        for i in range(dlg.instanceLabelsLayout.rowCount()):
-                            # first create label name document with HTML annotations
-                            tempDoc.setHtml(
-                                dlg.instanceLabelsLayout.itemAtPosition(i,
-                                                                        0).widget().text())
-                            # now strip html annotations
-                            tempLabelName = tempDoc.toPlainText().strip()
-                            # check if label name is in label dictionary of item.
-                            if tempLabelName in item.labels.keys():
-                                item.labels[tempLabelName].labelValue = (
-                                    dlg.instanceLabelsLayout.itemAtPosition(i,
-                                                                            1).widget().text())
-                                item.labels[tempLabelName].labelValueSet = True
-                                visible = (
-                                    dlg.instanceLabelsLayout.itemAtPosition(i,
-                                                                            2).widget().currentText())
-                                if visible == "True":
-                                    item.labels[tempLabelName].labelVisible = True
-                                else:
-                                    item.labels[
-                                        tempLabelName].labelVisible = False
-                                item.labels[tempLabelName].labelDefs()
-                        item.update()
-                elif isinstance(item, net.schematicNet):
-                    dlg = pdlg.netProperties(self.parent.parent, item)
-                    if dlg.exec() == QDialog.Accepted:
-                        item.name = dlg.netNameEdit.text().strip()
-                        if item.name == "":
-                            item.nameSet = False
-                        else:
-                            item.nameSet = True  # self.createNetlist()
-                        item.update()
-                elif isinstance(item, shp.text):
-                    dlg = pdlg.noteTextEditProperties(self.parent.parent, item)
-                    if dlg.exec() == QDialog.Accepted:
-                        # item.prepareGeometryChange()
-                        start = item.start
-                        self.removeItem(item)
-                        item = shp.text(start, self.textPen,
-                                        dlg.plainTextEdit.toPlainText(),
-                                        self.gridTuple,
-                                        dlg.familyCB.currentText(),
-                                        dlg.fontStyleCB.currentText(),
-                                        dlg.fontsizeCB.currentText(),
-                                        dlg.textAlignmCB.currentText(),
-                                        dlg.textOrientCB.currentText(), )
-                        self.rotateAnItem(start, item, float(item.textOrient[1:]))
-                        self.addItem(item)
-
-    def createSymbol(self):
-        """
-        Create a symbol view for a schematic.
-        """
-        oldSymbolItem = False
-
-        askViewNameDlg = pdlg.symbolNameDialog(self.parent.parent.file.parent,
-                                               self.parent.parent.cellName,
-                                               self.parent.parent, )
-        if askViewNameDlg.exec() == QDialog.Accepted:
-            symbolViewName = askViewNameDlg.symbolViewsCB.currentText()
-            if symbolViewName in askViewNameDlg.symbolViewNames:
-                oldSymbolItem = True
-
-        if oldSymbolItem:
-            deleteSymViewDlg = fd.deleteSymbolDialog(self.parent.parent.cellName,
-                                                     symbolViewName,
-                                                     self.parent.parent)
-            if deleteSymViewDlg.exec() == QDialog.Accepted:
-                self.generateSymbol(symbolViewName)
-        else:
-            self.generateSymbol(symbolViewName)
-
-    def generateSymbol(self, symbolViewName: str):
-        # openPath = pathlib.Path(cellItem.data(Qt.UserRole + 2))
-        cellPath = self.schematicWindow.file.parent
-        libName = self.schematicWindow.libName
-        cellName = self.schematicWindow.cellName
-        libItem = libm.getLibItem(self.schematicWindow.libraryView.libraryModel,
-                                  libName)
-        cellItem = libm.getCellItem(libItem, cellName)
-        libraryView = self.schematicWindow.libraryView
-        schematicPins = list(self.findScenePinsSet())
-
-        schematicPinNames = [pinItem.pinName for pinItem in schematicPins]
-
-        inputPins = [pinItem.pinName for pinItem in schematicPins if
-                     pinItem.pinDir == shp.schematicPin.pinDirs[0]]
-
-        outputPins = [pinItem.pinName for pinItem in schematicPins if
-                      pinItem.pinDir == shp.schematicPin.pinDirs[1]]
-
-        inoutPins = [pinItem.pinName for pinItem in schematicPins if
-                     pinItem.pinDir == shp.schematicPin.pinDirs[2]]
-
-        dlg = pdlg.symbolCreateDialog(self.parent.parent, inputPins, outputPins,
-                                      inoutPins)
-        if dlg.exec() == QDialog.Accepted:
-            symbolViewItem = scb.createCellView(self.parent.parent,
-                                                symbolViewName, cellItem)
-            libraryDict = self.parent.parent.libraryDict
-            # create symbol editor window with an empty items list
-            symbolWindow = symbolEditor(symbolViewItem, libraryDict, libraryView)
-            try:
-                leftPinNames = list(filter(None, [pinName.strip() for pinName in
-                                                  dlg.leftPinsEdit.text().split(
-                                                      ",")], ))
-                rightPinNames = list(filter(None, [pinName.strip() for pinName in
-                                                   dlg.rightPinsEdit.text().split(
-                                                       ",")], ))
-                topPinNames = list(filter(None, [pinName.strip() for pinName in
-                                                 dlg.topPinsEdit.text().split(
-                                                     ",")], ))
-                bottomPinNames = list(filter(None, [pinName.strip() for pinName in
-                                                    dlg.bottomPinsEdit.text().split(
-                                                        ",")], ))
-                stubLength = int(float(dlg.stubLengthEdit.text().strip()))
-                pinDistance = int(float(dlg.pinDistanceEdit.text().strip()))
-                rectXDim = (max(len(topPinNames),
-                                len(bottomPinNames)) + 1) * pinDistance
-                rectYDim = (max(len(leftPinNames),
-                                len(rightPinNames)) + 1) * pinDistance
-            except ValueError:
-                print("Enter valid value")
-
-        # add window to open windows list
-        libraryView.openViews[
-            f"{libName}_{cellName}_{symbolViewName}"] = symbolWindow
-        symbolScene = symbolWindow.centralW.scene
-        symbolScene.rectDraw(QPoint(0, 0), QPoint(rectXDim, rectYDim),
-                             self.symbolPen, self.gridTuple)
-        symbolScene.labelDraw(QPoint(int(0.25 * rectXDim), int(0.4 * rectYDim)),
-                              self.labelPen, "[@cellName]", self.gridTuple,
-                              "NLPLabel", "12", "Center", "R0", "Instance", )
-        symbolScene.labelDraw(QPoint(int(rectXDim), int(-0.2 * rectYDim)),
-                              self.labelPen, "[@instName]", self.gridTuple,
-                              "NLPLabel", "12", "Center", "R0", "Instance", )
-        leftPinLocs = [QPoint(-stubLength, (i + 1) * pinDistance) for i in
-                       range(len(leftPinNames))]
-        rightPinLocs = [QPoint(rectXDim + stubLength, (i + 1) * pinDistance) for i
-                        in range(len(rightPinNames))]
-        bottomPinLocs = [QPoint((i + 1) * pinDistance, rectYDim + stubLength) for
-                         i in range(len(bottomPinNames))]
-        topPinLocs = [QPoint((i + 1) * pinDistance, -stubLength) for i in
-                      range(len(topPinNames))]
-        for i in range(len(leftPinNames)):
-            symbolScene.lineDraw(leftPinLocs[i],
-                                 leftPinLocs[i] + QPoint(stubLength, 0),
-                                 symbolScene.symbolPen, symbolScene.gridTuple, )
-            symbolScene.addItem(schematicPins[
-                schematicPinNames.index(leftPinNames[i])].toSymbolPin(
-                leftPinLocs[i], symbolScene.pinPen, symbolScene.gridTuple))
-        for i in range(len(rightPinNames)):
-            symbolScene.lineDraw(rightPinLocs[i],
-                                 rightPinLocs[i] + QPoint(-stubLength, 0),
-                                 symbolScene.symbolPen, symbolScene.gridTuple, )
-            symbolScene.addItem(schematicPins[
-                schematicPinNames.index(rightPinNames[i])].toSymbolPin(
-                rightPinLocs[i], symbolScene.pinPen, symbolScene.gridTuple))
-        for i in range(len(topPinNames)):
-            symbolScene.lineDraw(topPinLocs[i],
-                                 topPinLocs[i] + QPoint(0, stubLength),
-                                 symbolScene.symbolPen, symbolScene.gridTuple, )
-            symbolScene.addItem(schematicPins[
-                schematicPinNames.index(topPinNames[i])].toSymbolPin(
-                topPinLocs[i], symbolScene.pinPen, symbolScene.gridTuple))
-        for i in range(len(bottomPinNames)):
-            symbolScene.lineDraw(bottomPinLocs[i],
-                                 bottomPinLocs[i] + QPoint(0, -stubLength),
-                                 symbolScene.symbolPen, symbolScene.gridTuple, )
-            symbolScene.addItem(schematicPins[
-                schematicPinNames.index(bottomPinNames[i])].toSymbolPin(
-                bottomPinLocs[i], symbolScene.pinPen,
-                symbolScene.gridTuple))  # symbol attribute generation for netlisting.
-        symbolScene.attributeList = list()  # empty attribute list
-        nlpPinNames = ""
-        for pinName in schematicPinNames:
-            nlpPinNames += f" [|{pinName}:%]"
-        symbolScene.attributeList.append(se.symbolAttribute("NLPDeviceFormat",
-                                                            f"X[@instName] {nlpPinNames} [@cellName]"))
-        symbolWindow.show()
-        libraryView.reworkDesignLibrariesView()
-        return symbolViewItem
-
-    def goDownHier(self):
-        if self.selectedItems is not None:
-            for item in self.selectedItems:
-                if isinstance(item, shp.symbolShape):
-                    dlg = fd.goDownHierDialogue(item,
-                                                self.parent.parent.libraryDict, )
-                    if dlg.exec() == QDialog.Accepted:
-                        selectedView = dlg.viewNameCB.currentText()
-                        libName = item.libraryName
-                        cellName = item.cellName
-                        libraryView = self.parent.parent.libraryView
-                        libraryModel = libraryView.libraryModel
-                        libraryDict = libraryView.libraryDict
-                        viewItem = libm.findViewItem(libraryModel, libName,
-                                                     cellName, selectedView)
-
-                        if "symbol" in selectedView:
-                            symbolWindow = symbolEditor(viewItem, libraryDict,
-                                                        libraryView, )
-                            symbolWindow.loadSymbol()
-                            symbolWindow.parentView = self.parent.parent
-                            symbolWindow.show()
-                            libraryView.openViews[
-                                f"{libName}_{cellName}_{selectedView}"] = symbolWindow
-                        elif "schematic" in selectedView:
-                            schematicWindow = schematicEditor(viewItem,
-                                                              libraryDict,
-                                                              libraryView, )
-                            schematicWindow.loadSchematic()
-                            schematicWindow.parentView = self.parent.parent
-                            schematicWindow.show()
-                            libraryView.openViews[
-                                f"{libName}_{cellName}_{selectedView}"] = schematicWindow
-
-    def goUpHier(self):
-        print("Up baby up")
-
-
-class editor_view(QGraphicsView):
-    """
-    The qgraphicsview for qgraphicsscene. It is used for both schematic and layout editors.
-    """
-
-    def __init__(self, scene, parent):
-        super().__init__(scene, parent)
-        self.parent = parent
-        self.editor = self.parent.parent
-        self.scene = scene
-        self.majorGrid = self.editor.majorGrid
-        self.gridTuple = self.editor.gridTuple
-        self.gridbackg = True
-        self.init_UI()
-
-    def init_UI(self):
-        self.setViewportUpdateMode(QGraphicsView.FullViewportUpdate)
-        # self.setCacheMode(QGraphicsView.CacheBackground)
-        self.standardCursor = QCursor(Qt.CrossCursor)
-        self.setCursor(self.standardCursor)  # set cursor to standard arrow
-        self.setRenderHint(QPainter.Antialiasing)
-        self.setRenderHint(QPainter.TextAntialiasing)
-        self.setMouseTracking(True)
-
-    def wheelEvent(self, mouse_event):
-        factor = 1.1
-        if mouse_event.angleDelta().y() < 0:
-            factor = 0.9
-        view_pos = QPoint(int(mouse_event.globalPosition().x()),
-                          int(mouse_event.globalPosition().y()))
-        scene_pos = self.mapToScene(view_pos)
-        self.centerOn(scene_pos)
-        self.scale(factor, factor)
-        delta = self.mapToScene(view_pos) - self.mapToScene(
-            self.viewport().rect().center())
-        self.centerOn(scene_pos - delta)
-        super().wheelEvent(mouse_event)
-
-    def snapToBase(self, number, base):
-        return base * int(math.floor(number / base))
-
-    def drawBackground(self, painter, rect):
-
-        if self.gridbackg:
-            rectCoord = rect.getRect()
-            painter.fillRect(rect, QColor("black"))
-            painter.setPen(QColor("gray"))
-            grid_x_start = math.ceil(
-                rectCoord[0] / self.majorGrid) * self.majorGrid
-            grid_y_start = math.ceil(
-                rectCoord[1] / self.majorGrid) * self.majorGrid
-            num_x_points = math.floor(rectCoord[2] / self.majorGrid)
-            num_y_points = math.floor(rectCoord[3] / self.majorGrid)
-            for i in range(int(num_x_points)):  # rect width
-                for j in range(int(num_y_points)):  # rect length
-                    painter.drawPoint(grid_x_start + i * self.majorGrid,
-                                      grid_y_start + j * self.majorGrid, )
-        else:
-            super().drawBackground(painter, rect)
-
-    def keyPressEvent(self, key_event):
-        if key_event.key() == Qt.Key_F:
-            self.fitToView()
-        super().keyPressEvent(key_event)
-
-    def fitToView(self):
-        viewRect = self.scene.itemsBoundingRect().marginsAdded(
-            QMargins(40, 40, 40, 40))
-        self.fitInView(viewRect, Qt.AspectRatioMode.KeepAspectRatio)
-        self.show()
-
-    def printView(self, printer):
-        """
-        Print view using selected Printer.
-        """
-        painter = QPainter(printer)
-        painter.setFont(QFont("Helvetica"))
-        self.gridbackg = False
-        self.drawBackground(painter, self.viewport().geometry())
-        painter.drawText(self.viewport().geometry(), "Revolution EDA")
-        self.render(painter)
-        self.gridbackg = True
-        painter.end()
-
-
-class symbol_view(editor_view):
-    def __init__(self, scene, parent):
-        self.scene = scene
-        self.parent = parent
-        super().__init__(self.scene, self.parent)
-        self.visibleRect = QRect(0, 0, 0, 0)  # initialize to an empty rectangle
-
-
-class schematic_view(editor_view):
-    def __init__(self, scene, parent):
-        self.scene = scene
-        self.parent = parent
-        super().__init__(self.scene, self.parent)
-        self.visibleRect = QRect(0, 0, 0, 0)  # initialize to an empty rectangle
-        self.viewItems = []
-        self.netItems = []
-
-    def mouseReleaseEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
-        if mouse_event.button() == Qt.LeftButton:
-            if self.scene.drawWire:
-                self.visibleRect = self.viewport().geometry()
-                self.viewItems = [item for item in self.items(self.visibleRect,
-                                                              mode=Qt.IntersectsItemShape)
-                                  if isinstance(item, shp.symbolShape)]
-                self.netItems = [item for item in self.items(self.visibleRect,
-                                                             mode=Qt.IntersectsItemShape)
-                                 if isinstance(item, net.schematicNet)]
-        super().mouseReleaseEvent(mouse_event)
-
-
-class libraryBrowser(QMainWindow):
-    def __init__(self, appMainW: QMainWindow) -> None:
-        super().__init__()
-        self.appMainW = appMainW
-        self.libraryDict = self.appMainW.libraryDict
-        self.cellViews = self.appMainW.cellViews
-        self.setWindowTitle("Library Browser")
-        self._createMenuBar()
-        self._createActions()
-        self._createToolBars()
-        self.logger = self.appMainW.logger
-        self.libFilePath = self.appMainW.libraryPathObj
-        self.libBrowserCont = libraryBrowserContainer(self)
-        self.setCentralWidget(self.libBrowserCont)
-        self.designView = self.libBrowserCont.designView
-        self.libraryModel = self.designView.libraryModel
-
-    def _createMenuBar(self):
-        self.browserMenubar = self.menuBar()
-        self.browserMenubar.setNativeMenuBar(False)
-        self.libraryMenu = self.browserMenubar.addMenu("&Library")
-
-    def _createActions(self):
-        openLibIcon = QIcon(":/icons/database--plus.png")
-        self.openLibAction = QAction(openLibIcon, "Create/Open Lib...", self)
-        self.openLibAction.setToolTip("Create/Open Lib...")
-        self.libraryMenu.addAction(self.openLibAction)
-        self.openLibAction.triggered.connect(self.openLibClick)
-
-        libraryEditIcon = QIcon(":/icons/application-dialog.png")
-        self.libraryEditorAction = QAction(libraryEditIcon, "Library Editor",
-                                           self)
-        self.libraryMenu.addAction(self.libraryEditorAction)
-        self.libraryEditorAction.setToolTip("Open Library Editor...")
-        self.libraryEditorAction.triggered.connect(self.libraryEditorClick)
-
-        closeLibIcon = QIcon(":/icons/database-delete.png")
-        self.closeLibAction = QAction(closeLibIcon, "Close Lib...", self)
-        self.closeLibAction.setToolTip("Close Lib")
-        self.libraryMenu.addAction(self.closeLibAction)
-        self.closeLibAction.triggered.connect(self.closeLibClick)
-
-        self.libraryMenu.addSeparator()
-
-        newCellIcon = QIcon(":/icons/document--plus.png")
-        self.newCellAction = QAction(newCellIcon, "New Cell...", self)
-        self.newCellAction.setToolTip("Create New Cell")
-        self.libraryMenu.addAction(self.newCellAction)
-        self.newCellAction.triggered.connect(self.newCellClick)
-
-        deleteCellIcon = QIcon(":/icons/node-delete.png")
-        self.deleteCellAction = QAction(deleteCellIcon, "Delete Cell...", self)
-        self.deleteCellAction.setToolTip("Delete Cell")
-        self.libraryMenu.addAction(self.deleteCellAction)
-        self.deleteCellAction.triggered.connect(self.deleteCellClick)
-
-        self.libraryMenu.addSeparator()
-
-        newCellViewIcon = QIcon(":/icons/document--pencil.png")
-        self.newCellViewAction = QAction(newCellViewIcon,
-                                         "Create New CellView...", self)
-        self.newCellViewAction.setToolTip("Create New Cellview")
-        self.libraryMenu.addAction(self.newCellViewAction)
-        self.newCellViewAction.triggered.connect(self.newCellViewClick)
-
-        openCellViewIcon = QIcon(":/icons/document--pencil.png")
-        self.openCellViewAction = QAction(openCellViewIcon, "Open CellView...",
-                                          self)
-        self.openCellViewAction.setToolTip("Open CellView")
-        self.libraryMenu.addAction(self.openCellViewAction)
-        self.openCellViewAction.triggered.connect(self.openCellViewClick)
-
-        deleteCellViewIcon = QIcon(":/icons/node-delete.png")
-        self.deleteCellViewAction = QAction(deleteCellViewIcon,
-                                            "Delete CellView...", self)
-        self.deleteCellViewAction.setToolTip("Delete Cellview")
-        self.libraryMenu.addAction(self.deleteCellViewAction)
-        self.deleteCellViewAction.triggered.connect(self.deleteCellViewClick)
-
-    def _createToolBars(self):
-        # Create tools bar called "main toolbar"
-        toolbar = QToolBar("Main Toolbar", self)
-        # place toolbar at top
-        self.addToolBar(toolbar)
-        toolbar.addAction(self.openLibAction)
-        toolbar.addAction(self.closeLibAction)
-        toolbar.addSeparator()
-        toolbar.addAction(self.newCellAction)
-        toolbar.addAction(self.deleteCellAction)
-        toolbar.addSeparator()
-        toolbar.addAction(self.newCellViewAction)
-        toolbar.addAction(self.openCellViewAction)
-        toolbar.addAction(self.deleteCellViewAction)
-
-    def writeLibDefFile(self, libPathDict: dict,
-                        libFilePath: pathlib.Path) -> None:
-
-        libTempDict = dict(
-            zip(libPathDict.keys(), map(str, libPathDict.values())))
-        try:
-            with libFilePath.open(mode="w") as f:
-                json.dump({"libdefs": libTempDict}, f, indent=4)
-            self.logger.info(f'Wrote library definition file in {libFilePath}')
-        except IOError:
-            self.logger.error(f"Cannot save library definitions in {libFilePath}")
-
-    def openLibClick(self):
-        """
-        Open a directory and add a 'reveda.lib' file to designate it as a library.
-        """
-        home_dir = str(pathlib.Path.cwd())
-        libDialog = QFileDialog(self, "Create/Open Library", home_dir)
-        libDialog.setFileMode(QFileDialog.Directory)
-        # libDialog.Option(QFileDialog.ShowDirsOnly)
-        if libDialog.exec() == QDialog.Accepted:
-            libPathObj = pathlib.Path(libDialog.selectedFiles()[0])
-            self.libraryDict[libPathObj.stem] = libPathObj
-            # create an empty file to denote it is a design library.
-            # TODO: add some library information to this file.
-            libPathObj.joinpath("reveda.lib").touch(exist_ok=True)
-            # self.designView.reworkDesignLibrariesView()
-            self.libraryModel.populateLibrary(libPathObj)
-            self.writeLibDefFile(self.libraryDict, self.libFilePath)
-
-    def closeLibClick(self):
-        libCloseDialog = fd.closeLibDialog(self.libraryDict, self)
-        if libCloseDialog.exec() == QDialog.Accepted:
-            libName = libCloseDialog.libNamesCB.currentText()
-            libItem = libm.getLibItem(self.libraryModel, libName)
-            try:
-                self.libraryDict.pop(libName)
-            except KeyError:
-                self.logger.error(f"{libName} not found.")
-            finally:
-                self.libraryModel.rootItem.removeRow(
-                    libItem)  # self.designView.reworkDesignLibrariesView()
-
-    def libraryEditorClick(self, s):
-        """
-        Open library editor dialogue.
-        """
-        tempDict = deepcopy(self.libraryDict)
-        pathEditDlg = fd.libraryPathEditorDialog(self, tempDict)
-        self.libraryDict.clear()
-        if pathEditDlg.exec() == QDialog.Accepted:
-            model = pathEditDlg.pathsModel
-            for row in range(model.rowCount()):
-
-                if model.itemFromIndex(model.index(row, 1)).text().strip():
-                    self.libraryDict[model.itemFromIndex(
-                        model.index(row, 0)).text().strip()] = pathlib.Path(
-                        model.itemFromIndex(model.index(row, 1)).text().strip())
-        self.writeLibDefFile(self.libraryDict,
-                             pathlib.Path.cwd().joinpath('library.json'))
-        self.designView.reworkDesignLibrariesView()
-
-    def newCellClick(self, s):
-        dlg = fd.createCellDialog(self, self.libraryModel)
-        if dlg.exec() == QDialog.Accepted:
-            libName = dlg.libNamesCB.currentText()
-            cellName = dlg.cellCB.currentText()
-            self.createNewCell(self, self.libraryModel, cellName, libName)
-
-    def createNewCell(self, parent, libraryModel, cellName, libName):
-        libItem = libm.getLibItem(self.libraryModel, libName)
-        if cellName.strip() == "":
-            self.logger.error("Please enter a cell name.")
-        else:
-            scb.createCell(parent, libraryModel, libItem, cellName)
-
-    def deleteCellClick(self, s):
-        dlg = fd.deleteCellDialog(self, self.libraryModel)
-        if dlg.exec() == QDialog.Accepted:
-            libItem = libm.getLibItem(self.libraryModel,
-                                      dlg.libNamesCB.currentText())
-            if dlg.cellCB.currentText().strip() == "":
-                self.logger.error("Please enter a cell name.")
-            else:
-                # cellItemsLib = {libItem.child(i).cellName: libItem.child(i) for i in
-                #                 range(libItem.rowCount())}
-                # cellItem = cellItemsLib.get(dlg.cellCB.currentText())
-                cellItem = libm.getCellItem(libItem, dlg.cellCB.currentText())
-                # remove the directory
-                shutil.rmtree(cellItem.data(Qt.UserRole + 2))
-                cellItem.parent().removeRow(cellItem.row())
-
-    def newCellViewClick(self, s):
-        dlg = fd.newCellViewDialog(self, self.libraryModel)
-        dlg.viewType.addItems(self.cellViews)
-        if dlg.exec() == QDialog.Accepted:
-            # cellPath = dlg.selectedLibPath.joinpath(dlg.cellCB.currentText())
-            libItem = libm.getLibItem(self.libraryModel,
-                                      dlg.libNamesCB.currentText())
-            cellItem = libm.getCellItem(libItem, dlg.cellCB.currentText())
-            viewItem = scb.createCellView(self.appMainW,
-                                          dlg.viewName.text().strip(), cellItem)
-            self.createNewCellView(libItem, cellItem, viewItem)
-
-    def createNewCellView(self, libItem, cellItem, viewItem):
-        match viewItem.viewType:
-            case "config":
-                schViewsList = [cellItem.child(row).viewName for row in
-                                range(cellItem.rowCount()) if
-                                cellItem.child(row).viewType == "schematic"]
-
-                dlg = fd.createConfigViewDialogue(self.appMainW)
-                dlg.libraryNameEdit.setText(libItem.libraryName)
-                dlg.cellNameEdit.setText(cellItem.cellName)
-                dlg.viewNameCB.addItems(schViewsList)
-                dlg.switchViews.setText(", ".join(self.appMainW.switchViewList))
-                dlg.stopViews.setText(", ".join(self.appMainW.stopViewList))
-                # dlg.switchViews.setText(self.)
-                if dlg.exec() == QDialog.Accepted:
-                    selectedSchName = dlg.viewNameCB.currentText()
-                    selectedSchItem = libm.getViewItem(cellItem, selectedSchName)
-                    schematicWindow = schematicEditor(selectedSchItem,
-                                                      self.libraryDict,
-                                                      self.libBrowserCont.designView, )
-                    schematicWindow.loadSchematic()
-                    switchViewList = [viewName.strip() for viewName in
-                                      dlg.switchViews.text().split(",")]
-                    stopViewList = [viewName.strip() for viewName in
-                                    dlg.stopViews.text().split(",")]
-                    schematicWindow.switchViewList = switchViewList
-                    schematicWindow.stopViewList = stopViewList
-                    schematicWindow.configDict = dict()  # clear config dictionary
-                    schematicWindow.netlistedCells = list()
-                    # clear netlisted cells list
-                    newConfigDict = dict()  # create an empty newconfig dict
-                    schematicWindow.createConfigView(viewItem,
-                                                     schematicWindow.configDict,
-                                                     newConfigDict,
-                                                     schematicWindow.netlistedCells, )
-                    configFilePathObj = viewItem.data(Qt.UserRole + 2)
-                    items = list()
-                    items.insert(0, {"cellView": "config"})
-                    items.insert(1, {"reference": selectedSchName})
-                    items.insert(2, schematicWindow.configDict)
-                    with configFilePathObj.open(mode="w+") as configFile:
-                        json.dump(items, configFile, indent=4)
-
-                    self.openConfigEditWindow(schematicWindow.configDict,
-                                              selectedSchItem, viewItem)
-            case "schematic":
-                # scb.createCellView(self.appMainW, viewItem.viewName, cellItem)
-                schematicWindow = schematicEditor(viewItem, self.libraryDict,
-                                                  self.libBrowserCont.designView)
-                schematicWindow.loadSchematic()
-                schematicWindow.show()
-            case "symbol":
-                # scb.createCellView(self.appMainW, viewItem.viewName, cellItem)
-                symbolWindow = symbolEditor(viewItem, self.libraryDict,
-                                            self.libBrowserCont.designView)
-                symbolWindow.loadSymbol()
-                symbolWindow.show()
-            case "veriloga":
-                # scb.createCellView(self.appMainW, viewItem.viewName, cellItem)
-                p = QProcess(self.appMainW)
-                p.finished.connect(self.appMainW.importVerilogaClick)
-                p.start(str(self.appMainW.textEditorPath), [])
-
-    def openConfigEditWindow(self, configDict, schViewItem, viewItem):
-        schematicName = schViewItem.viewName
-        libItem = schViewItem.parent().parent()
-        configWindow = configViewEdit(self.appMainW, schViewItem, configDict,
-                                      viewItem)
-        configWindow.centralWidget.libraryNameEdit.setText(libItem.libraryName)
-        cellItem = viewItem.parent()
-        configWindow.centralWidget.cellNameEdit.setText(cellItem.cellName)
-        schViewsList = [cellItem.child(row).viewName for row in
-                        range(cellItem.rowCount()) if
-                        cellItem.child(row).viewType == "schematic"]
-        configWindow.centralWidget.viewNameCB.addItems(schViewsList)
-        configWindow.centralWidget.viewNameCB.setCurrentText(schematicName)
-        configWindow.centralWidget.switchViewsEdit.setText(
-            ", ".join(self.appMainW.switchViewList))
-        configWindow.centralWidget.stopViewsEdit.setText(
-            ", ".join(self.appMainW.stopViewList))
-        configWindow.show()
-
-    def selectCellView(self, libModel) -> scb.viewItem:
-        dlg = fd.selectCellViewDialog(self, libModel)
-        if dlg.exec() == QDialog.Accepted:
-            libItem = libm.getLibItem(libModel, dlg.libNamesCB.currentText())
-            try:
-                cellItem = libm.getCellItem(libItem, dlg.cellCB.currentText())
-            except IndexError:
-                cellItem = libItem.child(0)
-            try:
-                viewItem = libm.getViewItem(cellItem, dlg.viewCB.currentText())
-                return viewItem
-            except IndexError:
-                viewItem = cellItem.child(0)
-                return None
-
-    def openCellViewClick(self):
-        viewItem = self.selectCellView(self.libraryModel)
-        cellItem = viewItem.parent()
-        libItem = cellItem.parent()
-        self.openCellView(viewItem, cellItem, libItem)
-
-    def openCellView(self, viewItem, cellItem, libItem):
-        viewName = viewItem.viewName
-        cellName = cellItem.cellName
-        libName = libItem.libraryName
-
-        if f"{libName}_{cellName}_{viewName}" in self.appMainW.openViews.keys():
-            self.appMainW.openViews[
-                f"{libName}_{cellName}_" f"{viewName}"].raise_()
-        else:
-            if viewItem.viewType == "schematic":
-                schematicWindow = schematicEditor(viewItem, self.libraryDict,
-                                                  self.libBrowserCont.designView)
-                schematicWindow.loadSchematic()
-                schematicWindow.show()
-                self.appMainW.openViews[
-                    f"{libName}_{cellName}_" f"{viewName}"] = schematicWindow
-            elif viewItem.viewType == "symbol":
-                symbolWindow = symbolEditor(viewItem, self.libraryDict,
-                                            self.libBrowserCont.designView)
-                symbolWindow.loadSymbol()
-                symbolWindow.show()
-                self.appMainW.openViews[
-                    f"{libName}_{cellName}_" f"{viewName}"] = symbolWindow
-            elif viewItem.viewType == "veriloga":
-                with open(viewItem.viewPath) as tempFile:
-                    items = json.load(tempFile)
-                if items[1]["filePath"]:
-                    p = QProcess(self.appMainW)
-                    p.finished.connect(self.appMainW.importVerilogaClick)
-                    p.start(str(self.appMainW.textEditorPath), [
-                        str(viewItem.viewPath.parent.joinpath(
-                            items[1]["filePath"]))])
-
-                else:
-                    self.logger.warning("File path not defined.")
-            elif viewItem.viewType == "config":
-                with open(viewItem.viewPath) as tempFile:
-                    items = json.load(tempFile)
-                viewName = items[0]["viewName"]
-                schematicName = items[1]["reference"]
-                schViewItem = libm.getViewItem(cellItem, schematicName)
-                configDict = items[2]
-                self.openConfigEditWindow(configDict, schViewItem, viewItem)
-
-    def deleteCellViewClick(self, s):
-        viewItem = self.selectCellView(self.libraryModel)
-        try:
-            viewItem.data(Qt.UserRole + 2).unlink()  # delete the file.
-            viewItem.parent().removeRow(viewItem.row())
-        except OSError as e:
-            # print(f"Error:{e.strerror}")
-            self.logger.warning(f"Error:{e.strerror}")
-
-    def closeEvent(self, event: QCloseEvent) -> None:
-        self.appMainW.libraryBrowser = None
-        event.accept()
-
-
-class libraryBrowserContainer(QWidget):
-    def __init__(self, parent) -> None:
-        super().__init__(parent)
-        self.parent = parent
-        self.initUI()
-
-    def initUI(self):
-        self.layout = QVBoxLayout()
-        self.designView = designLibrariesView(self)
-        self.layout.addWidget(self.designView)
-        self.setLayout(self.layout)
-
-
-class designLibrariesView(QTreeView):
-    def __init__(self, parent):
-        super().__init__(parent=parent)  # QTreeView
-        self.parent = parent  # type: QMainWindow
-        self.setSelectionMode(QAbstractItemView.SingleSelection)
-        self.viewCounter = 0
-        self.libBrowsW = self.parent.parent
-        self.appMainW = self.libBrowsW.appMainW
-        self.libraryDict = self.appMainW.libraryDict  # type: dict
-        self.cellViews = self.appMainW.cellViews  # type: list
-        self.openViews = self.appMainW.openViews  # type: dict
-        self.logger = self.appMainW.logger
-        self.selectedItem = None
-        # library model is based on qstandarditemmodel
-        self.libraryModel = designLibrariesModel(self.libraryDict)
-        self.setSortingEnabled(True)
-        self.setUniformRowHeights(True)
-        self.expandAll()
-        # iterate design library directories. Designpath is the path of library
-        # obtained from libraryDict
-        # for designPath in self.libraryDict.values():  # type: Path
-        #     self.populateLibrary(designPath)
-        self.setModel(self.libraryModel)
-
-    def removeLibrary(self):
-        button = QMessageBox.question(self, "Library Deletion",
-                                      "Are you sure to delete " "this library? This action cannot be undone.", )
-        if button == QMessageBox.Yes:
-            shutil.rmtree(self.selectedItem.data(Qt.UserRole + 2))
-            self.libraryModel.removeRow(self.selectedItem.row())
-
-    def saveLibAs(self):
-        pass
-
-    def renameLib(self):
-        oldLibraryName = self.selectedItem.libraryName
-        dlg = fd.renameLibDialog(self, oldLibraryName)
-        if dlg.exec() == QDialog.Accepted:
-            newLibraryName = dlg.newLibraryName.text().strip()
-            libraryItem = libm.getLibItem(self.libraryModel, oldLibraryName)
-            libraryItem.setText(newLibraryName)
-            oldLibraryPath = libraryItem.data(Qt.UserRole + 2)
-            newLibraryPath = oldLibraryPath.parent.joinpath(newLibraryName)
-            oldLibraryPath.rename(newLibraryPath)
-
-    def createCell(self):
-        dlg = fd.createCellDialog(self, self.libraryModel)
-        assert isinstance(self.selectedItem, scb.libraryItem)
-        dlg.libNamesCB.setCurrentText(self.selectedItem.libraryName)
-        if dlg.exec() == QDialog.Accepted:
-            cellName = dlg.cellCB.currentText()
-            if cellName.strip() != '':
-                scb.createCell(self, self.libraryModel, self.selectedItem,
-                               cellName)
-            else:
-                self.logger.error("Please enter a cell name.")
-
-    def copyCell(self):
-        dlg = fd.copyCellDialog(self, self.libraryModel, self.selectedItem)
-
-        if dlg.exec() == QDialog.Accepted:
-            scb.copyCell(self, dlg.model, dlg.cellItem, dlg.copyName.text(),
-                         dlg.selectedLibPath)
-
-    def renameCell(self):
-        dlg = fd.renameCellDialog(self, self.selectedItem)
-        if dlg.exec() == QDialog.Accepted:
-            scb.renameCell(self, dlg.cellItem, dlg.nameEdit.text())
-
-    def deleteCell(self):
-        try:
-            shutil.rmtree(self.selectedItem.data(Qt.UserRole + 2))
-            self.selectedItem.parent().removeRow(self.selectedItem.row())
-        except OSError as e:
-            # print(f"Error:{e.strerror}")
-            self.logger.warning(f"Error:{e}")
-
-    def createCellView(self):
-        dlg = fd.createCellViewDialog(self, self.libraryModel, self.selectedItem)
-        if dlg.exec() == QDialog.Accepted:
-            viewItem = scb.createCellView(self.appMainW, dlg.nameEdit.text(),
-                                          self.selectedItem)
-            self.libBrowsW.createNewCellView(self.selectedItem.parent(),
-                                             self.selectedItem, viewItem)
-
-    def openView(self):
-        viewItem = self.selectedItem
-        cellItem = viewItem.parent()
-        libItem = cellItem.parent()
-        self.libBrowsW.openCellView(viewItem, cellItem, libItem)
-
-    def copyView(self):
-        dlg = fd.copyViewDialog(self, self.libraryModel)
-        if dlg.exec() == QDialog.Accepted:
-            if self.selectedItem.data(Qt.UserRole + 1) == "view":
-                viewPath = self.selectedItem.data(Qt.UserRole + 2)
-                selectedLibItem = libm.getLibItem(self.libraryModel,
-                                                  dlg.libNamesCB.currentText())
-                selectedLibPath = selectedLibItem.libraryPath
-                cellName = dlg.cellCB.currentText()
-                libCellNames = [selectedLibItem.child(row).cellName for row in
-                                range(selectedLibItem.rowCount())]
-                if (
-                        cellName in libCellNames):  # check if there is the cell in the library
-                    cellItem = libm.getCellItem(selectedLibItem,
-                                                dlg.cellCB.currentText())
-                else:
-                    cellItem = scb.createCell(self.libBrowsW, self.libraryModel,
-                                              selectedLibItem,
-                                              dlg.cellCB.currentText(), )
-                cellViewNames = [cellItem.child(row).viewName for row in
-                                 range(cellItem.rowCount())]
-                newViewName = dlg.viewName.text()
-                if newViewName in cellViewNames:
-                    self.logger.warning(
-                        "View already exists. Delete cellview and try " "again.")
-                else:
-                    newViewPath = cellItem.data(Qt.UserRole + 2).joinpath(
-                        f"{newViewName}.json")
-                    shutil.copy(viewPath, newViewPath)
-                    cellItem.appendRow(scb.viewItem(newViewPath))
-
-    def renameView(self):
-        oldViewName = self.selectedItem.viewName
-        dlg = fd.renameViewDialog(self.libBrowsW, oldViewName)
-        if dlg.exec() == QDialog.Accepted:
-            newName = dlg.newViewNameEdit.text()
-            try:
-                viewPathObj = self.selectedItem.data(Qt.UserRole + 2)
-                newPathObj = self.selectedItem.data(Qt.UserRole + 2).rename(
-                    viewPathObj.parent.joinpath(f"{newName}.json"))
-                self.selectedItem.parent().appendRow(scb.viewItem(newPathObj))
-                self.selectedItem.parent().removeRow(self.selectedItem.row())
-            except FileExistsError:
-                self.logger.error("Cellview exists.")
-
-    def deleteView(self):
-        try:
-            self.selectedItem.data(Qt.UserRole + 2).unlink()
-            itemRow = self.selectedItem.row()
-            parent = self.selectedItem.parent()
-            parent.removeRow(itemRow)
-        except OSError as e:
-            # print(f"Error:{e.strerror}")
-            self.logger.warning(f"Error:{e.strerror}")
-
-    def reworkDesignLibrariesView(self):
-        """
-        Recreate library model from libraryDict.
-        """
-        self.libraryModel.clear()
-        self.libraryModel = designLibrariesModel(self.appMainW.libraryDict)
-        self.setModel(self.libraryModel)
-
-    # context menu
-    def contextMenuEvent(self, event):
-        menu = QMenu(self)
-        try:
-            index = self.selectedIndexes()[0]
-        except IndexError:
-            pass
-        try:
-            self.selectedItem = self.libraryModel.itemFromIndex(index)
-            if self.selectedItem.data(Qt.UserRole + 1) == "library":
-                menu.addAction("Rename Library", self.renameLib)
-                menu.addAction("Remove Library", self.removeLibrary)
-                menu.addAction("Create Cell", self.createCell)
-            elif self.selectedItem.data(Qt.UserRole + 1) == "cell":
-                menu.addAction(QAction("Create CellView...", self,
-                                       triggered=self.createCellView))
-                menu.addAction(
-                    QAction("Copy Cell...", self, triggered=self.copyCell))
-                menu.addAction(
-                    QAction("Rename Cell...", self, triggered=self.renameCell))
-                menu.addAction(
-                    QAction("Delete Cell...", self, triggered=self.deleteCell))
-            elif self.selectedItem.data(Qt.UserRole + 1) == "view":
-                menu.addAction(
-                    QAction("Open View", self, triggered=self.openView))
-                menu.addAction(
-                    QAction("Copy View...", self, triggered=self.copyView))
-                menu.addAction(
-                    QAction("Rename View...", self, triggered=self.renameView))
-                menu.addAction(
-                    QAction("Delete View...", self, triggered=self.deleteView))
-            menu.exec(event.globalPos())
-        except UnboundLocalError:
-            pass
-
-
-class designLibrariesModel(QStandardItemModel):
-    def __init__(self, libraryDict):
-        self.libraryDict = libraryDict
-        super().__init__()
-        self.rootItem = self.invisibleRootItem()
-        self.setHorizontalHeaderLabels(["Libraries"])
-        for designPath in self.libraryDict.values():
-            self.populateLibrary(designPath)
-
-    def populateLibrary(self, designPath):  # designPath: Path
-        """
-        Populate library view.
-        """
-        if designPath.joinpath("reveda.lib").exists():
-            libraryItem = self.addLibraryToModel(designPath)
-            cellList = [cell.name for cell in designPath.iterdir() if
-                        cell.is_dir()]
-            for cell in cellList:  # type: str
-                cellItem = self.addCellToModel(designPath.joinpath(cell),
-                                               libraryItem)
-                viewList = [view.name for view in
-                            designPath.joinpath(cell).iterdir() if
-                            view.suffix == ".json"]
-                for view in viewList:
-                    self.addViewToModel(designPath.joinpath(cell, view), cellItem)
-
-    def addLibraryToModel(self, designPath):
-        libraryEntry = scb.libraryItem(designPath)
-        self.rootItem.appendRow(libraryEntry)
-        return libraryEntry
-
-    def addCellToModel(self, cellPath, parentItem):
-        cellEntry = scb.cellItem(cellPath)
-        parentItem.appendRow(cellEntry)
-        return cellEntry
-
-    def addViewToModel(self, viewPath, parentItem):
-        viewEntry = scb.viewItem(viewPath)
-        parentItem.appendRow(viewEntry)  # return viewEntry
-
-
-class libraryPathsModel(QStandardItemModel):
-    def __init__(self, libraryDict):
-        super().__init__()
-        self.libraryDict = libraryDict
-        self.setHorizontalHeaderLabels(['Library Name', 'Library Path'])
-        for key, value in self.libraryDict.items():
-            libName = QStandardItem(key)
-            libPath = QStandardItem(str(value))
-            self.appendRow(libName, libPath)
-        self.appendRow(QStandardItem('Click here...'), QStandardItem(''))
-
-
-class libraryPathsTableView(QTableView):
-    def __init__(self, model):
-        self.model = model
-        self.setModel(self.model)
-        self.setShowGrid(True)
-        self.setContextMenuPolicy(Qt.CustomContextMenu)
-
-    def contextMenuEvent(self, event) -> None:
-        self.menu = QMenu(self)
-        removePathAction = QAction('Remove Library Path...', self.menu)
-        removePathAction.triggered.connect(lambda: self.removeLibraryPath(event))
-        self.menu.addAction(removePathAction)
-        self.menu.popup(QCursor.pos())
-
-    def removeLibraryPath(self, event):
-        print('remove library path')
-
-
-class symbolViewsModel(designLibrariesModel):
-    def __init__(self, libraryDict):
-        super().__init__(libraryDict)
-
-    def populateLibrary(self, designPath):  # designPath: Path
-        """
-        Populate library view.
-        """
-        if designPath.joinpath("reveda.lib").exists():
-            libraryItem = self.addLibraryToModel(designPath)
-            cellList = [cell.name for cell in designPath.iterdir() if
-                        cell.is_dir()]
-            for cell in cellList:  # type: str
-                cellItem = self.addCellToModel(designPath.joinpath(cell),
-                                               libraryItem)
-                viewList = [view.name for view in
-                            designPath.joinpath(cell).iterdir() if
-                            view.suffix == ".json" and "symbol" in view.name]
-                for view in viewList:
-                    self.addViewToModel(designPath.joinpath(cell, view), cellItem)
-
-
-class xyceNetlist:
-    def __init__(self, schematic: schematicEditor, filePathObj: pathlib.Path,
-                 use_config: bool = False):
-        self.filePathObj = filePathObj
-        self.schematic = schematic
-        self.scene = self.schematic.centralW.scene
-        self.libraryDict = self.schematic.libraryDict
-        self.libraryView = self.schematic.libraryView
-        self._configDict = None
-        self.libItem = libm.getLibItem(self.schematic.libraryView.libraryModel,
-                                       self.schematic.libName, )
-        self.cellItem = libm.getCellItem(self.libItem, self.schematic.cellName)
-        self.use_config = use_config
-        self.switchViewList = schematic.switchViewList
-        self.netlistedViews = dict()
-
-    def writeNetlist(self):
-        with self.filePathObj.open(mode="w") as cirFile:
-            cirFile.write(f'{80 * "*"}\n')
-            cirFile.write("* Revolution EDA CDL Netlist\n")
-            cirFile.write(f"* Library: {self.schematic.libName}\n")
-            cirFile.write(f"* Top Cell Name: {self.schematic.cellName}\n")
-            cirFile.write(f"* View Name: {self.schematic.viewName}\n")
-            cirFile.write(f"* Date: {datetime.datetime.now()}\n")
-            cirFile.write(f'{80 * "*"}\n')
-            cirFile.write(".GLOBAL gnd!\n")
-            cirFile.write("\n")
-            self.recursiveNetlisting(self.schematic, cirFile, self.use_config)
-            cirFile.write(".END\n")
-
-    @property
-    def configDict(self):
-        return self._configDict
-
-    @configDict.setter
-    def configDict(self, value: dict):
-        if value:
-            self._configDict = value
-
-    def recursiveNetlisting(self, schematic: schematicEditor, cirFile,
-                            use_config: bool = False):
-        """
-        Recursively traverse all sub-circuits and netlist them.
-        """
-        # self.analyseSchematic(self.schematic)
-        scene = schematic.centralW.scene
-        scene.groupAllNets()  # name all nets in the schematic
-        sceneSymbolSet = scene.findSceneSymbolSet()
-        scene.generatePinNetMap(sceneSymbolSet)
-        for item in sceneSymbolSet:
-            libItem = libm.getLibItem(schematic.libraryView.libraryModel,
-                                      item.libraryName)
-            cellItem = libm.getCellItem(libItem, item.cellName)
-            viewItems = [cellItem.child(row) for row in
-                         range(cellItem.rowCount())]
-            viewNames = [view.viewName for view in viewItems]
-
-            viewDict = dict(zip(viewNames, viewItems))
-            if use_config:
-                netlistableViews = [self.configDict.get(item.cellName)[1]]
-            else:
-                netlistableViews = [viewItemName for viewItemName in
-                                    self.switchViewList if
-                                    viewItemName in viewNames]
-            self.createItemLine(cirFile, item, libItem, netlistableViews,
-                                viewDict)
-
-    def createItemLine(self, cirFile, item, libItem, netlistableViews, viewDict):
-        for view in netlistableViews:
-            if view in viewDict.keys():
-                if viewDict[view].viewType == "schematic":
-                    schematicObj = schematicEditor(viewDict[view],
-                                                   self.libraryDict,
-                                                   self.libraryView, )
-                    schematicObj.loadSchematic()
-                    pins = " ".join(list(item.pinNetMap.keys()))
-                    nets = " ".join(list(item.pinNetMap.values()))
-                    cirFile.write(
-                        f"X{item.instanceName} {nets} {item.cellName}\n")
-                    if item.cellName not in self.netlistedViews.keys():
-                        self.netlistedViews[item.cellName] = [libItem.libraryName,
-                                                              view, ]
-                        cirFile.write(f".SUBCKT {item.cellName} {pins}\n")
-                        self.recursiveNetlisting(schematicObj, cirFile)
-                        cirFile.write(".ENDS\n")
-                elif viewDict[view].viewType == "veriloga":
-                    with viewDict[view].data(Qt.UserRole + 2).open(
-                            mode="r") as vaview:
-                        items = json.load(vaview)
-                    netlistLine = items[3]['netlistLine']
-                    netlistLine = netlistLine.replace("[@instName]",
-                                                      f"{item.instanceName}")
-                    for pinName, netName in item.pinNetMap.items():
-                        netlistLine = netlistLine.replace(f"[|{pinName}:%]",
-                                                          f"{netName}")
-                    for labelItem in item.labels.values():
-                        if labelItem.labelDefinition in netlistLine:
-                            netlistLine = netlistLine.replace(
-                                labelItem.labelDefinition, labelItem.labelText)
-                    cirFile.write(f"{netlistLine}\n")
-                    modelParamsLine = ', '.join(
-                        ' = '.join((key, val)) for (key, val) in
-                        item.attr.items())
-                    modelLine = f'.MODEL {item.labels["vaModel"].labelValue} ' \
-                                f'{item.labels["vaModule"].labelValue} {modelParamsLine}'
-                    cirFile.write(f'{modelLine}\n')
-                    self.netlistedViews[item.cellName] = [libItem.libraryName,
-                                                          "veriloga", ]
-                elif viewDict[view].viewType == "symbol":
-                    cirFile.write(f"{item.createNetlistLine()}\n")
-                    self.netlistedViews[item.cellName] = [libItem.libraryName,
-                                                          "symbol", ]
-                break
-
-
-class configViewEdit(QMainWindow):
-    def __init__(self, appmainW, schViewItem, configDict, viewItem):
-        super().__init__(parent=appmainW)
-        self.appmainW = appmainW  # app mainwindow
-        self.schViewItem = schViewItem
-        self.configDict = configDict
-        self.viewItem = viewItem
-        self.setWindowTitle('Edit Config View')
-        self.setMinimumSize(500, 600)
-        self._createMenuBar()
-        self._createActions()
-        self._addActions()
-        self._createTriggers()
-        self.centralWidget = configViewEditContainer(self)
-        self.setCentralWidget(self.centralWidget)
-
-    def _createMenuBar(self):
-        self.mainMenu = self.menuBar()
-        self.fileMenu = self.mainMenu.addMenu("&File")
-        self.editMenu = self.mainMenu.addMenu("&Edit")
-        self.status_bar = self.statusBar()
-        self.status_bar.showMessage('Ready')
-
-    def _createActions(self):
-        updateIcon = QIcon(":/icons/arrow-circle.png")
-        self.updateAction = QAction(updateIcon, "Update", self)
-        saveIcon = QIcon(":/icons/database--plus.png")
-        self.saveAction = QAction(saveIcon, "Save", self)
-
-    def _addActions(self):
-        self.fileMenu.addAction(self.updateAction)
-        self.fileMenu.addAction(self.saveAction)
-
-    def _createTriggers(self):
-        self.updateAction.triggered.connect(self.updateClick)
-        self.saveAction.triggered.connect(self.saveClick)
-
-    def updateClick(self):
-        self.centralWidget.configViewTable.updateModel()
-        self.configDict = dict()
-        newConfigDict = dict()
-        model = self.centralWidget.confModel
-        for i in range(model.rowCount()):
-            viewList = [item.strip() for item in
-                        model.itemFromIndex(model.index(i, 3)).text().split(',')]
-            self.configDict[model.item(i, 1).text()] = [model.item(i, 0).text(),
-                                                        model.item(i, 2).text(),
-                                                        viewList]
-        if self.appmainW.libraryBrowser is None:
-            self.appmainW.createLibraryBrowser()
-        topSchematicWindow = schematicEditor(self.schViewItem,
-                                             self.appmainW.libraryDict,
-                                             self.appmainW.libraryBrowser.libBrowserCont.designView)
-        topSchematicWindow.loadSchematic()
-        topSchematicWindow.createConfigView(self.viewItem, self.configDict,
-                                            newConfigDict, [])
-        self.configDict = newConfigDict
-
-        self.centralWidget.confModel = configModel(self.configDict)
-        # self.centralWidget.configDictGroup.setVisible(False)
-        self.centralWidget.configDictLayout.removeWidget(
-            self.centralWidget.configViewTable)
-        self.centralWidget.configViewTable = configTable(
-            self.centralWidget.confModel)
-        self.centralWidget.configDictLayout.addWidget(
-            self.centralWidget.configViewTable)  # self.centralWidget.configDictGroup.setVisible(True)
-
-    def saveClick(self):
-        configFilePathObj = self.viewItem.data(Qt.UserRole + 2)
-        items = list()
-        items.insert(0, {"viewName": "config"})
-        items.insert(1, {"reference": self.schViewItem.viewName})
-        items.insert(2, self.configDict)
-        with configFilePathObj.open(mode="w+") as configFile:
-            json.dump(items, configFile, indent=4)
-
-
-class configViewEditContainer(QWidget):
-    def __init__(self, parent):
-        super().__init__(parent)
-        self.parent = parent
-        self.mainLayout = QVBoxLayout()
-        topCellGroup = QGroupBox('Top Cell')
-        topCellLayout = QFormLayout()
-        self.libraryNameEdit = edf.longLineEdit()
-        topCellLayout.addRow(edf.boldLabel('Library:'), self.libraryNameEdit)
-        self.cellNameEdit = edf.longLineEdit()
-        topCellLayout.addRow(edf.boldLabel('Cell:'), self.cellNameEdit)
-        self.viewNameCB = QComboBox()
-        topCellLayout.addRow(edf.boldLabel('View:'), self.viewNameCB)
-        topCellGroup.setLayout(topCellLayout)
-        self.mainLayout.addWidget(topCellGroup)
-        viewGroup = QGroupBox('Switch/Stop Views')
-        viewGroupLayout = QFormLayout()
-        viewGroup.setLayout(viewGroupLayout)
-        self.switchViewsEdit = edf.longLineEdit()
-        viewGroupLayout.addRow(edf.boldLabel('View List:'), self.switchViewsEdit)
-        self.stopViewsEdit = edf.longLineEdit()
-        viewGroupLayout.addRow(edf.boldLabel('Stop List:'), self.stopViewsEdit)
-        self.mainLayout.addWidget(viewGroup)
-        self.configDictGroup = QGroupBox('Cell View Configuration')
-        self.confModel = configModel(self.parent.configDict)
-        self.configDictLayout = QVBoxLayout()
-        self.configViewTable = configTable(self.confModel)
-        self.configDictLayout.addWidget(self.configViewTable)
-        self.configDictGroup.setLayout(self.configDictLayout)
-        self.mainLayout.addWidget(self.configDictGroup)
-        self.setLayout(self.mainLayout)
-
-
-class configModel(QStandardItemModel):
-    def __init__(self, configDict: dict):
-        row = len(configDict.keys())
-        column = 4
-        super().__init__(row, column)
-        self.setHorizontalHeaderLabels(
-            ['Library', 'Cell Name', 'View Found', 'View To '
-                                                   'Use'])
-        for i, (k, v) in enumerate(configDict.items()):
-            item = QStandardItem(v[0])
-            self.setItem(i, 0, item)
-            item = QStandardItem(k)
-            self.setItem(i, 1, item)
-            item = QStandardItem(v[1])
-            self.setItem(i, 2, item)
-            item = QStandardItem(', '.join(v[2]))
-            self.setItem(i, 3, item)
-
-
-class configTable(QTableView):
-    def __init__(self, model: configModel):
-        super().__init__()
-        self.model = model
-        self.setModel(self.model)
-        self.combos = list()
-        for row in range(self.model.rowCount()):
-            self.combos.append(QComboBox())
-            items = [item.strip() for item in self.model.itemFromIndex(
-                self.model.index(row, 3)).text().split(',')]
-            self.combos[-1].addItems(items)
-            self.combos[-1].setCurrentText(
-                self.model.itemFromIndex(self.model.index(row, 2)).text())
-            self.setIndexWidget(self.model.index(row, 3), self.combos[-1])
-
-    def updateModel(self):
-        for row in range(self.model.rowCount()):
-            item = QStandardItem(self.combos[row].currentText())
-            self.model.setItem(row, 2, item)
-
-
-class runXNetlistThread(QRunnable):
-    def __init__(self, netlistObj: xyceNetlist, parent):
-        super().__init__()
-        self.netlistObj = netlistObj
-        self.parent = parent
-
-    def run(self) -> None:
-        self.netlistObj.writeNetlist()
-        self.parent.logger.info('Netlisting finished')
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+import datetime
+import json
+import math
+# from hashlib import new
+import pathlib
+import shutil
+from copy import deepcopy
+import os
+# if os.environ.get('REVEDASIM_PATH'):
+#     import revedasim.simMainWindow as smw
+
+# import numpy as np
+from PySide6.QtCore import (QEvent, QMargins, QPoint, QPointF, QProcess, QRect,
+                            QRectF, QRunnable, Qt, Slot)
+from PySide6.QtGui import (QAction, QCloseEvent, QColor, QCursor, QFont,
+                           QGuiApplication, QIcon, QImage, QKeySequence, QPainter,
+                           QPen, QStandardItem, QStandardItemModel, QTextDocument,
+                           QUndoStack)
+from PySide6.QtPrintSupport import (QPrintDialog, QPrinter, QPrintPreviewDialog)
+from PySide6.QtWidgets import (QAbstractItemView, QApplication, QComboBox,
+                               QDialog, QFileDialog, QFormLayout,
+                               QGraphicsRectItem, QGraphicsScene,
+                               QGraphicsSceneMouseEvent, QGraphicsView,
+                               QGridLayout, QGroupBox, QLabel, QMainWindow, QMenu,
+                               QMessageBox, QTableView, QToolBar, QTreeView,
+                               QVBoxLayout, QWidget)
+
+import revedaEditor.backend.dataDefinitions as ddef
+import revedaEditor.backend.libraryMethods as libm
+import revedaEditor.backend.schBackEnd as scb
+import revedaEditor.backend.undoStack as us
+import revedaEditor.common.layers as cel
+import revedaEditor.common.net as net
+import revedaEditor.common.pens as pens  # import pens
+import revedaEditor.common.shape as shp  # import the shapes
+import revedaEditor.fileio.loadJSON as lj
+import revedaEditor.fileio.symbolEncoder as se
+import revedaEditor.gui.editFunctions as edf
+import revedaEditor.gui.fileDialogues as fd
+import revedaEditor.gui.propertyDialogues as pdlg
+import revedaEditor.resources.resources
+
+class editorWindow(QMainWindow):
+    """
+    Base class for editor windows.
+    """
+
+    def __init__(self, viewItem: scb.viewItem, libraryDict: dict,
+                 libraryView):  # file is a pathlib.Path object
+        super().__init__()
+        self.viewItem = viewItem
+        self.file = self.viewItem.data(Qt.UserRole + 2)
+        self.cellItem = self.viewItem.parent()
+        self.cellName = self.cellItem.cellName
+        self.libItem = self.cellItem.parent()
+        self.libName = self.libItem.libraryName
+        self.viewName = self.viewItem.viewName
+        self.libraryDict = libraryDict
+        self.libraryView = libraryView
+        self.parentView = None
+        self._app = QApplication.instance()
+        self._createActions()
+        self._createTriggers()
+        self._createShortcuts()
+        self.appMainW = self.libraryView.parent.parent.appMainW
+        self.logger = self.appMainW.logger
+        self.switchViewList = self.appMainW.switchViewList
+        self.stopViewList = self.appMainW.stopViewList
+        self.statusLine = self.statusBar()
+        self.messageLine = QLabel()  # message line
+        self.statusLine.addPermanentWidget(self.messageLine)
+        self.majorGrid = 10  # snapping grid size
+        self.gridTuple = (self.majorGrid, self.majorGrid)
+        self.snapDistance = 20
+        if self._app.revedasim_path:
+            import revedasim.simMainWindow as smw
+        self.init_UI()
+
+    def init_UI(self):
+        """
+        Placeholder for child classes init_UI function.
+        """
+        ...
+
+    def _createMenuBar(self):
+        self.editorMenuBar = self.menuBar()
+        self.editorMenuBar.setNativeMenuBar(False)
+        # Returns QMenu object.
+        self.menuFile = self.editorMenuBar.addMenu("&File")
+        self.menuView = self.editorMenuBar.addMenu("&View")
+        self.menuEdit = self.editorMenuBar.addMenu("&Edit")
+        self.menuCreate = self.editorMenuBar.addMenu("C&reate")
+        self.menuCheck = self.editorMenuBar.addMenu("&Check")
+        self.menuTools = self.editorMenuBar.addMenu("&Tools")
+        self.menuWindow = self.editorMenuBar.addMenu("&Window")
+        self.menuUtilities = self.editorMenuBar.addMenu("&Utilities")
+
+    def _createActions(self):
+        checkCellIcon = QIcon(":/icons/document-task.png")
+        self.checkCellAction = QAction(checkCellIcon, "Check-Save", self)
+
+        self.readOnlyCellIcon = QIcon(":/icons/lock.png")
+        self.readOnlyCellAction = QAction(self.readOnlyCellIcon, "Make Read Only",
+                                          self)
+
+        printIcon = QIcon(":/icons/printer--arrow.png")
+        self.printAction = QAction(printIcon, "Print...", self)
+
+        printPreviewIcon = QIcon(":/icons/printer--arrow.png")
+        self.printPreviewAction = QAction(printPreviewIcon, "Print Preview...",
+                                          self)
+
+        exportImageIcon = QIcon(":/icons/image-export.png")
+        self.exportImageAction = QAction(exportImageIcon, "Export...", self)
+
+        exitIcon = QIcon(":/icons/external.png")
+        self.exitAction = QAction(exitIcon, "Close Window", self)
+        self.exitAction.setShortcut("Ctrl+Q")
+
+        fitIcon = QIcon(":/icons/zone.png")
+        self.fitAction = QAction(fitIcon, "Fit to Window", self)
+
+        zoomInIcon = QIcon(":/icons/zone-resize.png")
+        self.zoomInAction = QAction(zoomInIcon, "Zoom In", self)
+
+        zoomOutIcon = QIcon(":/icons/zone-resize-actual.png")
+        self.zoomOutAction = QAction(zoomOutIcon, "Zoom Out", self)
+
+        panIcon = QIcon(":/icons/zone--arrow.png")
+        self.panAction = QAction(panIcon, "Pan View", self)
+
+        redrawIcon = QIcon(":/icons/arrow-circle.png")
+        self.redrawAction = QAction(redrawIcon, "Redraw", self)
+
+        # rulerIcon = QIcon(":/icons/ruler.png")
+        # self.rulerAction = QAction(rulerIcon, 'Ruler', self)
+        # self.menuView.addAction(self.rulerAction)
+        # delRulerIcon = QIcon.fromTheme('delete')
+        # self.delRulerAction = QAction(delRulerIcon, 'Delete Rulers', self)
+        # self.menuView.addAction(self.delRulerAction)
+
+        # display options
+        dispConfigIcon = QIcon(":/icons/resource-monitor.png")
+        self.dispConfigAction = QAction(dispConfigIcon, "Display Config...", self)
+
+        selectConfigIcon = QIcon(":/icons/zone-select.png")
+        self.selectConfigAction = QAction(selectConfigIcon, "Selection Config...",
+                                          self)
+
+        panZoomConfigIcon = QIcon(":/icons/selection-resize.png")
+        self.panZoomConfigAction = QAction(panZoomConfigIcon,
+                                           "Pan/Zoom Config...", self)
+
+        undoIcon = QIcon(":/icons/arrow-circle-315-left.png")
+        self.undoAction = QAction(undoIcon, "Undo", self)
+
+        redoIcon = QIcon(":/icons/arrow-circle-225.png")
+        self.redoAction = QAction(redoIcon, "Redo", self)
+
+        yankIcon = QIcon(":/icons/node-insert.png")
+        self.yankAction = QAction(yankIcon, "Yank", self)
+
+        pasteIcon = QIcon(":/icons/clipboard-paste.png")
+        self.pasteAction = QAction(pasteIcon, "Paste", self)
+
+        deleteIcon = QIcon(":/icons/node-delete.png")
+        self.deleteAction = QAction(deleteIcon, "Delete", self)
+
+        copyIcon = QIcon(":/icons/document-copy.png")
+        self.copyAction = QAction(copyIcon, "Copy", self)
+
+        moveIcon = QIcon(":/icons/arrow-move.png")
+        self.moveAction = QAction(moveIcon, "Move", self)
+
+        moveByIcon = QIcon(":/icons/arrow-transition.png")
+        self.moveByAction = QAction(moveByIcon, "Move By ...", self)
+
+        moveOriginIcon = QIcon(":/icons/arrow-skip.png")
+        self.moveOriginAction = QAction(moveOriginIcon, "Move Origin", self)
+
+        stretchIcon = QIcon(":/icons/fill.png")
+        self.stretchAction = QAction(stretchIcon, "Stretch", self)
+
+        rotateIcon = QIcon(":/icons/arrow-circle.png")
+        self.rotateAction = QAction(rotateIcon, "Rotate...", self)
+
+        scaleIcon = QIcon(":/icons/selection-resize.png")
+        self.scaleAction = QAction(scaleIcon, "Scale...", self)
+
+        netNameIcon = QIcon(":/icons/node-design.png")
+        self.netNameAction = QAction(netNameIcon, "Net Name...", self)
+
+        # create label action but do not add to any menu.
+        createLabelIcon = QIcon(":/icons/tag-label-yellow.png")
+        self.createLabelAction = QAction(createLabelIcon, "Create Label...", self)
+
+        createPinIcon = QIcon(":/icons/pin--plus.png")
+        self.createPinAction = QAction(createPinIcon, "Create Pin...", self)
+
+        goUpIcon = QIcon(":/icons/arrow-step-out.png")
+        self.goUpAction = QAction(goUpIcon, "Go Up", self)
+
+        goDownIcon = QIcon(":/icons/arrow-step.png")
+        self.goDownAction = QAction(goDownIcon, "Go Down", self)
+
+        self.selectAllIcon = QIcon(":/icons/node-select-all.png")
+        self.selectAllAction = QAction(self.selectAllIcon, "Select All", self)
+
+        deselectAllIcon = QIcon(":/icons/node.png")
+        self.deselectAllAction = QAction(deselectAllIcon, "Unselect All", self)
+
+        objPropIcon = QIcon(":/icons/property-blue.png")
+        self.objPropAction = QAction(objPropIcon, "Object Properties...", self)
+
+        viewPropIcon = QIcon(":/icons/property.png")
+        self.viewPropAction = QAction(viewPropIcon, "Cellview Properties...",
+                                      self)
+
+        viewCheckIcon = QIcon(":/icons/ui-check-box.png")
+        self.viewCheckAction = QAction(viewCheckIcon, "Check CellView", self)
+
+        viewErrorsIcon = QIcon(":/icons/report--exclamation.png")
+        self.viewErrorsAction = QAction(viewErrorsIcon, "View Errors...", self)
+
+        deleteErrorsIcon = QIcon(":/icons/report--minus.png")
+        self.deleteErrorsAction = QAction(deleteErrorsIcon, "Delete Errors...",
+                                          self)
+
+        netlistIcon = QIcon(":/icons/script-text.png")
+        self.netlistAction = QAction(netlistIcon, "Create Netlist...", self)
+
+        simulateIcon = QIcon(":/icons/application-wave.png")
+        self.simulateAction = QAction(simulateIcon, "Run RevEDA Sim GUI", self)
+
+        createLineIcon = QIcon(":/icons/layer-shape-line.png")
+        self.createLineAction = QAction(createLineIcon, "Create Line...", self)
+
+        createRectIcon = QIcon(":/icons/layer-shape.png")
+        self.createRectAction = QAction(createRectIcon, "Create Rectangle...",
+                                        self)
+
+        createPolyIcon = QIcon(":/icons/layer-shape-polygon.png")
+        self.createPolyAction = QAction(createPolyIcon, "Create Polygon...", self)
+
+        createCircleIcon = QIcon(":/icons/layer-shape-ellipse.png")
+        self.createCircleAction = QAction(createCircleIcon, "Create Circle...",
+                                          self)
+
+        createArcIcon = QIcon(":/icons/layer-shape-polyline.png")
+        self.createArcAction = QAction(createArcIcon, "Create Arc...", self)
+
+        createInstIcon = QIcon(":/icons/block--plus.png")
+        self.createInstAction = QAction(createInstIcon, "Create Instance...",
+                                        self)
+
+        createWireIcon = QIcon(":/icons/node-insert.png")
+        self.createWireAction = QAction(createWireIcon, "Create Wire...", self)
+
+        createBusIcon = QIcon(":/icons/node-select-all.png")
+        self.createBusAction = QAction(createBusIcon, "Create Bus...", self)
+
+        createLabelIcon = QIcon(":/icons/tag-label-yellow.png")
+        self.createLabelAction = QAction(createLabelIcon, "Create Label...", self)
+
+        createPinIcon = QIcon(":/icons/pin--plus.png")
+        self.createPinAction = QAction(createPinIcon, "Create Pin...", self)
+
+        createSymbolIcon = QIcon(":/icons/application-block.png")
+        self.createSymbolAction = QAction(createSymbolIcon, "Create Symbol...",
+                                          self)
+
+        createTextIcon = QIcon(":icons/sticky-note-text.png")
+        self.createTextAction = QAction(createTextIcon, "Create Text...", self)
+
+    def _createToolBars(self):
+        # Create tools bar called "main toolbar"
+        self.toolbar = QToolBar("Main Toolbar", self)
+        # place toolbar at top
+        self.addToolBar(self.toolbar)
+        self.toolbar.addAction(self.printAction)
+        self.toolbar.addAction(self.exportImageAction)
+        self.toolbar.addSeparator()
+        self.toolbar.addAction(self.undoAction)
+        self.toolbar.addAction(self.redoAction)
+        self.toolbar.addSeparator()
+        self.toolbar.addAction(self.deleteAction)
+        self.toolbar.addAction(self.moveAction)
+        self.toolbar.addAction(self.copyAction)
+        self.toolbar.addAction(self.stretchAction)
+        self.toolbar.addAction(self.rotateAction)
+        self.toolbar.addSeparator()
+        self.toolbar.addAction(self.fitAction)
+        self.toolbar.addAction(self.zoomInAction)
+        self.toolbar.addAction(self.zoomOutAction)
+        self.toolbar.addSeparator()
+        self.toolbar.addAction(self.objPropAction)
+
+    def _addActions(self):
+        # file menu
+        self.menuFile.addAction(self.checkCellAction)
+        self.menuFile.addAction(self.readOnlyCellAction)
+        self.menuFile.addAction(self.printAction)
+        self.menuFile.addAction(self.printPreviewAction)
+        self.menuFile.addAction(self.exportImageAction)
+        self.menuFile.addAction(self.exitAction)
+        # view menu
+        self.menuView.addAction(self.fitAction)
+        self.menuView.addAction(self.zoomInAction)
+        self.menuView.addAction(self.zoomOutAction)
+        self.menuView.addAction(self.panAction)
+        self.menuView.addAction(self.redrawAction)
+        self.menuView.addAction(self.dispConfigAction)
+        self.menuView.addAction(self.selectConfigAction)
+        self.menuView.addAction(self.panZoomConfigAction)
+        # edit menu
+        self.menuEdit.addAction(self.undoAction)
+        self.menuEdit.addAction(self.redoAction)
+        # self.menuEdit.addAction(self.yankAction)
+        self.menuEdit.addAction(self.pasteAction)
+        self.menuEdit.addAction(self.deleteAction)
+        self.menuEdit.addAction(self.copyAction)
+        self.menuEdit.addAction(self.moveAction)
+        self.menuEdit.addAction(self.moveByAction)
+        self.menuEdit.addAction(self.moveOriginAction)
+        self.menuEdit.addAction(self.stretchAction)
+        self.menuEdit.addAction(self.rotateAction)
+
+        self.menuCheck.addAction(self.viewCheckAction)
+
+    def _createTriggers(self):
+        self.printAction.triggered.connect(self.printClick)
+        self.printPreviewAction.triggered.connect(self.printPreviewClick)
+        self.exportImageAction.triggered.connect(self.imageExportClick)
+        self.exitAction.triggered.connect(self.closeWindow)
+        self.fitAction.triggered.connect(self.fitToWindow)
+        self.zoomInAction.triggered.connect(self.zoomIn)
+        self.zoomOutAction.triggered.connect(self.zoomOut)
+        self.dispConfigAction.triggered.connect(self.dispConfigEdit)
+        self.selectConfigAction.triggered.connect(self.selectConfigEdit)
+        self.moveOriginAction.triggered.connect(self.moveOrigin)
+        self.selectAllAction.triggered.connect(self.selectAllClick)
+        self.deselectAllAction.triggered.connect(self.deselectAllClick)
+
+    def _createShortcuts(self):
+        self.redoAction.setShortcut("Shift+U")
+        self.undoAction.setShortcut(Qt.Key_U)
+        self.objPropAction.setShortcut(Qt.Key_Q)
+        self.copyAction.setShortcut(Qt.Key_C)
+        self.rotateAction.setShortcut("Ctrl+R")
+        self.createTextAction.setShortcut("Shift+L")
+        self.fitAction.setShortcut(Qt.Key_F)
+        self.deleteAction.setShortcut(QKeySequence.Delete)
+        self.selectAllAction.setShortcut("Ctrl+A")
+
+    def dispConfigEdit(self):
+        dcd = pdlg.displayConfigDialog(self)
+        dcd.majorGridEntry.setText(str(self.majorGrid))
+        dcd.snapDistanceEntry.setText(str(self.snapDistance))
+        if dcd.exec() == QDialog.Accepted:
+            self.majorGrid = int(float(dcd.majorGridEntry.text()))
+            self.snapDistance = int(float(dcd.snapDistanceEntry.text()))
+            self.gridTuple = (self.majorGrid, self.majorGrid)
+
+            if dcd.dotType.isChecked():
+                self.centralW.view.gridbackg = True
+                self.centralW.view.linebackg = False
+            elif dcd.lineType.isChecked():
+                self.centralW.view.gridbackg = False
+                self.centralW.view.linebackg = True
+            else:
+                self.centralW.view.gridbackg = False
+                self.centralW.view.linebackg = False
+            self.centralW.view.resetCachedContent()
+
+    def selectConfigEdit(self):
+        scd = pdlg.selectConfigDialogue(self)
+        if self.centralW.scene.partialSelection:
+            scd.partialSelection.setChecked(True)
+        else:
+            scd.fullSelection.setChecked(True)
+        if scd.exec() == QDialog.Accepted:
+            if scd.partialSelection.isChecked():
+                self.centralW.scene.partialSelection = True
+            else:
+                self.centralW.scene.partialSelection = False
+
+    def printClick(self):
+        dlg = QPrintDialog(self)
+        if dlg.exec() == QDialog.Accepted:
+            printer = dlg.printer()
+            printRunner = startThread(self.centralW.view.printView(printer))
+            self.appMainW.threadPool.start(printRunner)
+            self.logger.info('Printing started')
+            # self.centralW.view.printView(printer)
+
+    def printPreviewClick(self):
+        printer = QPrinter(QPrinter.ScreenResolution)
+        printer.setOutputFormat(QPrinter.PdfFormat)
+        ppdlg = QPrintPreviewDialog(self)
+        ppdlg.paintRequested.connect(self.centralW.view.printView)
+        ppdlg.exec()
+
+
+
+    def imageExportClick(self):
+        image = QImage(self.centralW.view.viewport().size(),
+                       QImage.Format_ARGB32_Premultiplied)
+        self.centralW.view.printView(image)
+        fdlg = QFileDialog(self, caption="Select or create an image file")
+        fdlg.setDefaultSuffix("png")
+        fdlg.setFileMode(QFileDialog.AnyFile)
+        fdlg.setViewMode(QFileDialog.Detail)
+        fdlg.setNameFilter("Image Files (*.png *.jpg *.bmp *.gif *.jpeg")
+        if fdlg.exec() == QDialog.Accepted:
+            imageFile = fdlg.selectedFiles()[0]
+            image.save(imageFile)
+
+    def selectAllClick(self):
+        self.centralW.scene.selectAll()
+
+    def deselectAllClick(self):
+        self.centralW.scene.deselectAll()
+
+    def fitToWindow(self):
+        self.centralW.view.fitToView()
+
+    def zoomIn(self):
+        self.centralW.view.scale(1.25, 1.25)
+
+    def zoomOut(self):
+        self.centralW.view.scale(0.8, 0.8)
+
+    def closeWindow(self):
+        self.close()
+
+    def closeEvent(self, event):
+        cellViewTuple = ddef.viewTuple(self.libName, self.cellName, self.viewName)
+        self.appMainW.openViews.pop(cellViewTuple)
+        event.accept()
+
+    def _createMenu(self):
+        pass
+
+    def moveOrigin(self):
+        self.centralW.scene.changeOrigin = True
+
+
+class schematicEditor(editorWindow):
+    def __init__(self, viewItem: scb.viewItem, libraryDict: dict,
+                 libraryView) -> None:
+        super().__init__(viewItem, libraryDict, libraryView)
+        self.setWindowTitle(
+            f"Schematic Editor - {self.cellName} - {self.viewName}")
+        self.setWindowIcon(QIcon(":/icons/layer-shape.png"))
+        self.configDict = dict()
+        self.processedCells = set()  # cells included in config view
+        self.symbolChooser = None
+        self.cellViews = [
+            "symbol"]  # only symbol can be instantiated in the schematic window.
+        self._schematicActions()
+
+    def init_UI(self):
+        self.resize(1600, 800)
+        self._createMenuBar()
+        self._createToolBars()
+        # create container to position all widgets
+        self.centralW = schematicContainer(self)
+        self.setCentralWidget(self.centralW)
+
+    def _createTriggers(self):
+        super()._createTriggers()
+        self.checkCellAction.triggered.connect(self.checkSaveCell)
+        self.createWireAction.triggered.connect(self.createWireClick)
+        self.createInstAction.triggered.connect(self.createInstClick)
+        self.createPinAction.triggered.connect(self.createPinClick)
+        self.createTextAction.triggered.connect(self.createNoteClick)
+        self.createSymbolAction.triggered.connect(self.createSymbolClick)
+        self.copyAction.triggered.connect(self.copyClick)
+        self.deleteAction.triggered.connect(self.deleteClick)
+        self.objPropAction.triggered.connect(self.objPropClick)
+        self.undoAction.triggered.connect(self.undoClick)
+        self.redoAction.triggered.connect(self.redoClick)
+        self.netlistAction.triggered.connect(self.createNetlistClick)
+        self.rotateAction.triggered.connect(self.rotateItemClick)
+        self.simulateAction.triggered.connect(self.startSimClick)
+        self.goDownAction.triggered.connect(self.goDownClick)
+        self.goUpAction.triggered.connect(self.goUpClick)
+
+    def _createMenuBar(self):
+        super()._createMenuBar()
+        self.menuSimulation = self.editorMenuBar.addMenu("&Simulation")
+        self.menuHelp = self.editorMenuBar.addMenu("&Help")
+        self._addActions()
+
+    def _addActions(self):
+        super()._addActions()
+        # edit menu
+
+        self.menuEdit.addAction(self.netNameAction)
+
+        self.propertyMenu = self.menuEdit.addMenu("Properties")
+        self.propertyMenu.addAction(self.objPropAction)
+
+        self.selectMenu = self.menuEdit.addMenu("Select")
+        self.selectMenu.addAction(self.selectAllAction)
+        self.selectMenu.addAction(self.deselectAllAction)
+
+        # hierarchy submenu
+        self.hierMenu = self.menuEdit.addMenu("Hierarchy")
+        self.hierMenu.addAction(self.goUpAction)
+        self.hierMenu.addAction(self.goDownAction)
+
+        # create menu
+        self.menuCreate.addAction(self.createInstAction)
+        self.menuCreate.addAction(self.createWireAction)
+        self.menuCreate.addAction(self.createBusAction)
+        self.menuCreate.addAction(self.createLabelAction)
+        self.menuCreate.addAction(self.createPinAction)
+        self.menuCreate.addAction(self.createTextAction)
+        self.menuCreate.addAction(self.createSymbolAction)
+
+        # check menu
+        self.menuCheck.addAction(self.viewErrorsAction)
+        self.menuCheck.addAction(self.deleteErrorsAction)
+
+        self.menuSimulation.addAction(self.netlistAction)
+        if self._app.revedasim_path:
+            self.menuSimulation.addAction(self.simulateAction)
+
+    def _createToolBars(self):
+        super()._createToolBars()
+        # toolbar.addAction(self.rulerAction)
+        # toolbar.addAction(self.delRulerAction)
+        self.toolbar.addAction(self.objPropAction)
+        self.toolbar.addAction(self.viewPropAction)
+
+        self.schematicToolbar = QToolBar("Schematic Toolbar", self)
+        self.addToolBar(self.schematicToolbar)
+        self.schematicToolbar.addAction(self.createInstAction)
+        self.schematicToolbar.addAction(self.createWireAction)
+        self.schematicToolbar.addAction(self.createBusAction)
+        self.schematicToolbar.addAction(self.createPinAction)
+        # self.schematicToolbar.addAction(self.createLabelAction)
+        self.schematicToolbar.addAction(self.createSymbolAction)
+        self.schematicToolbar.addSeparator()
+        self.schematicToolbar.addAction(self.viewCheckAction)
+
+    def _schematicActions(self):
+        self.centralW.scene.itemContextMenu.addAction(self.copyAction)
+        self.centralW.scene.itemContextMenu.addAction(self.moveAction)
+        self.centralW.scene.itemContextMenu.addAction(self.rotateAction)
+        self.centralW.scene.itemContextMenu.addAction(self.deleteAction)
+        self.centralW.scene.itemContextMenu.addAction(self.objPropAction)
+        self.centralW.scene.itemContextMenu.addAction(self.goDownAction)
+        if self.parentView is not None:
+            self.centralW.scene.itemContextMenu.addAction(self.goUpAction)
+
+    def _createShortcuts(self):
+        super()._createShortcuts()
+        self.createInstAction.setShortcut(Qt.Key_I)
+        self.createWireAction.setShortcut(Qt.Key_W)
+        self.createPinAction.setShortcut(Qt.Key_P)
+        self.goDownAction.setShortcut("Shift+E")
+
+    def dispConfigEdit(self):
+        super().dispConfigEdit()
+        self.centralW.view.majorGrid = self.majorGrid
+        self.centralW.scene.majorGrid = self.majorGrid
+        self.centralW.scene.gridTuple = (self.majorGrid, self.majorGrid)
+        self.centralW.view.gridTuple = (self.majorGrid, self.majorGrid)
+
+    def createWireClick(self, s):
+        self.centralW.scene.drawWire = True
+
+    def deleteClick(self, s):
+        self.centralW.scene.deleteSelectedItems()
+
+    def createInstClick(self, s):
+
+        # create a designLibrariesView
+        libraryModel = symbolViewsModel(self.libraryDict)
+        if self.symbolChooser is None:
+            self.symbolChooser = fd.selectCellViewDialog(self, libraryModel)
+            self.symbolChooser.show()
+        else:
+            self.symbolChooser.raise_()
+        if self.symbolChooser.exec() == QDialog.Accepted:
+            self.centralW.scene.addInstance = True
+            libItem = libm.getLibItem(libraryModel,
+                                      self.symbolChooser.libNamesCB.currentText())
+            cellItem = libm.getCellItem(libItem,
+                                        self.symbolChooser.cellCB.currentText())
+            viewItem = libm.getViewItem(cellItem,
+                                        self.symbolChooser.viewCB.currentText())
+            self.centralW.scene.instanceSymbolFile = viewItem.data(
+                Qt.UserRole + 2)
+
+    def createPinClick(self, s):
+        createPinDlg = pdlg.createSchematicPinDialog(self)
+        if createPinDlg.exec() == QDialog.Accepted:
+            self.centralW.scene.pinName = createPinDlg.pinName.text()
+            self.centralW.scene.pinType = createPinDlg.pinType.currentText()
+            self.centralW.scene.pinDir = createPinDlg.pinDir.currentText()
+            self.centralW.scene.drawPin = True
+
+    def createNoteClick(self, s):
+        textDlg = pdlg.noteTextEdit(self)
+        if textDlg.exec() == QDialog.Accepted:
+            self.centralW.scene.noteText = textDlg.plainTextEdit.toPlainText()
+            self.centralW.scene.noteFontFamily = textDlg.familyCB.currentText()
+            self.centralW.scene.noteFontSize = textDlg.fontsizeCB.currentText()
+            self.centralW.scene.noteFontStyle = textDlg.fontStyleCB.currentText()
+            self.centralW.scene.noteAlign = textDlg.textAlignmCB.currentText()
+            self.centralW.scene.noteOrient = textDlg.textOrientCB.currentText()
+            self.centralW.scene.drawText = True
+
+    def createSymbolClick(self, s):
+        self.centralW.scene.createSymbol()
+
+    def undoClick(self, s):
+        self.centralW.scene.undoStack.undo()
+
+    def redoClick(self, s):
+        self.centralW.scene.undoStack.redo()
+
+    def objPropClick(self, s):
+        self.centralW.scene.viewObjProperties()
+
+    def copyClick(self, s):
+        self.centralW.scene.copySelectedItems()
+
+    def rotateItemClick(self, s):
+        self.centralW.scene.rotateItem = True
+        self.centralW.scene.itemSelect = False
+
+    def startSimClick(self, s):
+        import revedasim.simMainWindow as smw
+        simguiw = smw.simMainWindow(self)
+        simguiw.show()
+
+    def checkSaveCell(self):
+        self.centralW.scene.saveSchematicCell(self.file)
+
+    def loadSchematic(self):
+        with open(self.file) as tempFile:
+            items = json.load(tempFile)
+        self.centralW.scene.loadSchematicCell(items)
+        sceneNetsSet = self.centralW.scene.findSceneNetsSet()
+        # because do not save dot points, it is necessary to recreate them.
+        for netItem in sceneNetsSet:
+            netItem.findDotPoints()
+
+    def createConfigView(self, configItem: scb.viewItem, configDict: dict,
+                         newConfigDict: dict, processedCells: set):
+
+        sceneSymbolSet = self.centralW.scene.findSceneSymbolSet()
+        for item in sceneSymbolSet:
+            libItem = libm.getLibItem(self.libraryView.libraryModel,
+                                      item.libraryName)
+            cellItem = libm.getCellItem(libItem, item.cellName)
+            viewItems = [cellItem.child(row) for row in
+                         range(cellItem.rowCount())]
+            viewNames = [viewItem.viewName for viewItem in viewItems]
+            netlistableViews = [viewItemName for viewItemName in
+                                self.switchViewList if
+                                viewItemName in viewNames]
+            itemSwitchViewList = deepcopy(netlistableViews)
+            viewDict = dict(zip(viewNames, viewItems))
+            itemCellTuple = ddef.cellTuple(libItem.libraryName, cellItem.cellName)
+            if itemCellTuple not in processedCells:
+                cellLine = configDict.get(cellItem.cellName)
+                if cellLine:
+                    netlistableViews = [cellLine[1]]
+                for viewName in netlistableViews:
+                    match viewDict[viewName].viewType:
+                        case "schematic":
+                            newConfigDict.update({
+                                cellItem.cellName: [libItem.libraryName, viewName,
+                                                    itemSwitchViewList, ]})
+                            schematicObj = schematicEditor(viewDict[viewName],
+                                                           self.libraryDict,
+                                                           self.libraryView, )
+                            schematicObj.loadSchematic()
+                            schematicObj.createConfigView(configItem, configDict,
+                                                          newConfigDict,
+                                                          processedCells)
+                            break
+                        case other:
+                            newConfigDict.update({
+                                cellItem.cellName: [libItem.libraryName, viewName,
+                                                    itemSwitchViewList, ]})
+                            break
+                processedCells.add(itemCellTuple)
+
+    def closeEvent(self, event):
+        self.centralW.scene.saveSchematicCell(self.file)
+        super().closeEvent(event)
+        event.accept()
+
+    def createNetlistClick(self, s):
+        netlistObj = None
+        dlg = fd.netlistExportDialogue(self)
+        dlg.libNameEdit.setText(self.libName)
+        dlg.cellNameEdit.setText(self.cellName)
+        configViewItems = [self.cellItem.child(row) for row in
+                           range(self.cellItem.rowCount()) if
+                           self.cellItem.child(row).viewType == 'config']
+        netlistableViews = [self.viewItem.viewName]
+        for item in configViewItems:
+            # is there a better way of doing it?
+            with item.data(Qt.UserRole + 2).open(mode='r') as f:
+                configItems = json.load(f)
+                if configItems[1]['reference'] == self.viewItem.viewName:
+                    netlistableViews.append(item.viewName)
+        dlg.viewNameCombo.addItems(netlistableViews)
+        if hasattr(self.appMainW, "simulationPath"):
+            dlg.netlistDirEdit.setText(str(self.appMainW.simulationPath))
+        if dlg.exec() == QDialog.Accepted:
+            try:
+                self.appMainW.simulationPath = pathlib.Path(
+                    dlg.netlistDirEdit.text())
+                selectedViewName = dlg.viewNameCombo.currentText()
+                self.switchViewList = [item.strip() for item in
+                                       dlg.switchViewEdit.text().split(",")]
+                self.stopViewList = [dlg.stopViewEdit.text().strip()]
+                subDirPathObj = self.appMainW.simulationPath.joinpath(
+                    self.cellName)
+                subDirPathObj.mkdir(parents=True, exist_ok=True)
+                netlistFilePathObj = subDirPathObj.joinpath(f'{self.cellName}_'
+                                                            f'{selectedViewName}').with_suffix(
+                    '.cir')
+                simViewName = dlg.viewNameCombo.currentText()
+                if 'schematic' in simViewName:
+                    netlistObj = xyceNetlist(self, netlistFilePathObj)
+                elif 'config' in simViewName:
+                    netlistObj = xyceNetlist(self, netlistFilePathObj, True)
+                    configItem = libm.findViewItem(self.libraryView.libraryModel,
+                                                   self.libName, self.cellName,
+                                                   dlg.viewNameCombo.currentText())
+                    with configItem.data(Qt.UserRole + 2).open(mode='r') as f:
+                        netlistObj.configDict = json.load(f)[2]
+
+                if netlistObj:
+                    xyceNetlRunner = startThread(netlistObj.writeNetlist())
+                    self.appMainW.threadPool.start(xyceNetlRunner)
+                    # netlistObj.writeNetlist()
+                    self.logger.info('Netlisting finished.')
+            except Exception as e:
+                self.logger.error(f'Error in creating netlist: {e}')
+
+    def goDownClick(self, s):
+        self.centralW.scene.goDownHier()
+
+    def goUpClick(self, s):
+        self.centralW.scene.goUpHier()
+
+
+class symbolEditor(editorWindow):
+    def __init__(self, viewItem: scb.viewItem, libraryDict: dict, libraryView):
+        super().__init__(viewItem, libraryDict, libraryView)
+        self.setWindowTitle(f"Symbol Editor - {self.cellName} - {self.viewName}")
+        self._symbolActions()
+
+    def init_UI(self):
+        self.resize(1600, 800)
+        self._createMenuBar()
+        self._createToolBars()
+        # create container to position all widgets
+        self.centralW = symbolContainer(self)
+        self.setCentralWidget(self.centralW)
+
+    def _createActions(self):
+        super()._createActions()
+
+    def _createShortcuts(self):
+        super()._createShortcuts()
+        self.stretchAction.setShortcut(Qt.Key_M)
+        self.createRectAction.setShortcut(Qt.Key_R)
+        self.createLineAction.setShortcut(Qt.Key_W)
+        self.createLabelAction.setShortcut(Qt.Key_L)
+        self.createPinAction.setShortcut(Qt.Key_P)
+
+    def _createMenuBar(self):
+        super()._createMenuBar()
+        self.menuHelp = self.editorMenuBar.addMenu("&Help")
+        self._addActions()
+
+    def _createToolBars(self):  # redefine the toolbar in the editorWindow class
+        super()._createToolBars()
+        self.symbolToolbar = QToolBar("Symbol Toolbar", self)
+        self.addToolBar(self.symbolToolbar)
+        self.symbolToolbar.addAction(self.createLineAction)
+        self.symbolToolbar.addAction(self.createRectAction)
+        self.symbolToolbar.addAction(self.createPolyAction)
+        self.symbolToolbar.addAction(self.createCircleAction)
+        self.symbolToolbar.addAction(self.createArcAction)
+        self.symbolToolbar.addAction(self.createLabelAction)
+        self.symbolToolbar.addAction(self.createPinAction)
+
+    def _addActions(self):
+        super()._addActions()
+        self.menuEdit.addAction(self.stretchAction)
+        self.menuEdit.addAction(self.viewPropAction)
+        self.selectMenu = self.menuEdit.addMenu("Select")
+        self.selectMenu.addAction(self.selectAllAction)
+        self.selectMenu.addAction(self.deselectAllAction)
+        self.menuCreate.addAction(self.createLineAction)
+        self.menuCreate.addAction(self.createRectAction)
+        self.menuCreate.addAction(self.createPolyAction)
+        self.menuCreate.addAction(self.createCircleAction)
+        self.menuCreate.addAction(self.createArcAction)
+        self.menuCreate.addAction(self.createLabelAction)
+        self.menuCreate.addAction(self.createPinAction)
+
+    def _createTriggers(self):
+
+        self.checkCellAction.triggered.connect(self.checkSaveCell)
+        self.createLineAction.triggered.connect(self.createLineClick)
+        self.createRectAction.triggered.connect(self.createRectClick)
+        self.createPolyAction.triggered.connect(self.createPolyClick)
+        self.createArcAction.triggered.connect(self.createArcClick)
+        self.createCircleAction.triggered.connect(self.createCircleClick)
+        self.createLabelAction.triggered.connect(self.createLabelClick)
+        self.createPinAction.triggered.connect(self.createPinClick)
+        self.objPropAction.triggered.connect(self.objPropClick)
+        self.copyAction.triggered.connect(self.copyClick)
+        self.redoAction.triggered.connect(self.redoClick)
+        self.undoAction.triggered.connect(self.undoClick)
+        self.rotateAction.triggered.connect(self.rotateItemClick)
+        self.deleteAction.triggered.connect(self.deleteClick)
+        self.stretchAction.triggered.connect(self.stretchClick)
+        self.viewPropAction.triggered.connect(self.viewPropClick)
+        super()._createTriggers()
+
+    def _symbolActions(self):
+        self.centralW.scene.itemContextMenu.addAction(self.copyAction)
+        self.centralW.scene.itemContextMenu.addAction(self.moveAction)
+        self.centralW.scene.itemContextMenu.addAction(self.rotateAction)
+        self.centralW.scene.itemContextMenu.addAction(self.stretchAction)
+        self.centralW.scene.itemContextMenu.addAction(self.deleteAction)
+        self.centralW.scene.itemContextMenu.addAction(self.objPropAction)
+
+    # def dispConfigEdit(self):
+    #     super().dispConfigEdit()
+    #     self.centralW.view.majorGrid = self.majorGrid
+    #     self.centralW.scene.majorGrid = self.majorGrid
+    #     self.centralW.view.gridTuple = (self.majorGrid, self.majorGrid)
+    #     self.centralW.scene.gridTuple = (self.majorGrid, self.majorGrid)
+
+    def objPropClick(self):
+        self.centralW.scene.itemProperties()
+
+    def checkSaveCell(self):
+        self.centralW.scene.saveSymbolCell(self.file)
+
+    def setDrawMode(self, *args):
+        """
+        Sets the drawing mode in the symbol editor.
+        """
+        self.centralW.scene.drawPin = args[0]
+        self.centralW.scene.itemSelect = args[1]
+        self.centralW.scene.drawArc = args[2]  # draw arc
+        self.centralW.scene.drawRect = args[3]  # draw rect
+        self.centralW.scene.drawLine = args[4]  # draw line
+        self.centralW.scene.addLabel = args[5]
+        self.centralW.scene.drawCircle = args[6]
+        self.centralW.scene.rotateItem = args[7]
+
+    def createRectClick(self, s):
+        modeList = [False for i in range(8)]
+        modeList[3] = True
+        self.setDrawMode(*modeList)
+
+    def createLineClick(self, s):
+        modeList = [False for i in range(8)]
+        modeList[4] = True
+        self.setDrawMode(*modeList)
+
+    def createPolyClick(self, s):
+        pass
+
+    def createArcClick(self, s):
+        modeList = [False for i in range(8)]
+        modeList[2] = True
+        self.setDrawMode(*modeList)
+
+    def createCircleClick(self, s):
+        modeList = [False for i in range(8)]
+        modeList[6] = True
+        self.setDrawMode(*modeList)
+
+    def createPinClick(self, s):
+        createPinDlg = pdlg.createPinDialog(self)
+        if createPinDlg.exec() == QDialog.Accepted:
+            modeList = [False for i in range(8)]
+            modeList[0] = True
+            self.centralW.scene.pinName = createPinDlg.pinName.text()
+            self.centralW.scene.pinType = createPinDlg.pinType.currentText()
+            self.centralW.scene.pinDir = createPinDlg.pinDir.currentText()
+            self.setDrawMode(*modeList)
+
+    def rotateItemClick(self, s):
+        self.centralW.scene.rotateItem = True
+        modeList = [False for i in range(8)]
+        modeList[7] = True
+        self.setDrawMode(*modeList)
+        self.messageLine.setText("Click on an item to rotate CW 90 degrees.")
+
+    def undoClick(self, s):
+        self.centralW.scene.undoStack.undo()
+
+    def redoClick(self, s):
+        self.centralW.scene.undoStack.redo()
+
+    def deleteClick(self, s):
+        self.centralW.scene.deleteSelectedItems()
+
+    def copyClick(self, s):
+        self.centralW.scene.copySelectedItems()
+
+    def stretchClick(self, s):
+        self.centralW.scene.stretchSelectedItem()
+
+    def viewPropClick(self, s):
+        self.centralW.scene.viewSymbolProperties()
+
+    def loadSymbol(self):
+        """
+        symbol is loaded to the scene.
+        """
+        with open(self.file) as tempFile:
+            try:
+                items = json.load(tempFile)
+            except json.decoder.JSONDecodeError:
+                self.logger.error("Cannot load symbol. JSON Decode Error")
+        self.centralW.scene.loadSymbol(items)
+
+    def createLabelClick(self):
+        createLabelDlg = pdlg.createSymbolLabelDialog(self)
+        self.messageLine.setText('Place a label')
+        if createLabelDlg.exec() == QDialog.Accepted:
+            modeList = [False for i in range(8)]
+            modeList[5] = True
+            self.setDrawMode(*modeList)
+            # directly setting scene class attributes here to pass the information.
+            self.centralW.scene.labelDefinition = createLabelDlg.labelDefinition.text()
+            self.centralW.scene.labelHeight = (
+                createLabelDlg.labelHeightEdit.text().strip())
+            self.centralW.scene.labelAlignment = (
+                createLabelDlg.labelAlignCombo.currentText())
+            self.centralW.scene.labelOrient = (
+                createLabelDlg.labelOrientCombo.currentText())
+            self.centralW.scene.labelUse = createLabelDlg.labelUseCombo.currentText()
+            if createLabelDlg.labelVisiCombo.currentText() == "Yes":
+                self.centralW.scene.labelOpaque = True
+            else:
+                self.centralW.scene.labelOpaque = False
+            self.centralW.scene.labelType = "Normal"  # default button
+            if createLabelDlg.normalType.isChecked():
+                self.centralW.scene.labelType = "Normal"
+            elif createLabelDlg.NLPType.isChecked():
+                self.centralW.scene.labelType = "NLPLabel"
+            elif createLabelDlg.pyLType.isChecked():
+                self.centralW.scene.labelType = "PyLabel"
+
+    def closeEvent(self, event):
+        """
+        Closes the application.
+        """
+        super().closeEvent(event)
+        self.centralW.scene.saveSymbolCell(self.file)
+        event.accept()
+
+
+class symbolContainer(QWidget):
+    def __init__(self, parent):
+        super().__init__(parent=parent)
+        self.parent = parent
+        self.scene = symbol_scene(self)
+        self.view = symbol_view(self.scene, self)
+        self.init_UI()
+
+    def init_UI(self):
+        # layout statements, using a grid layout
+        gLayout = QGridLayout()
+        gLayout.setSpacing(10)
+        gLayout.addWidget(self.view, 0, 0)
+        # ratio of first column to second column is 5
+        gLayout.setColumnStretch(0, 5)
+        gLayout.setRowStretch(0, 6)
+        self.setLayout(gLayout)
+
+
+class schematicContainer(QWidget):
+    def __init__(self, parent: schematicEditor):
+        super().__init__(parent=parent)
+        assert isinstance(parent, schematicEditor)
+        self.parent = parent
+        self.scene = schematic_scene(self)
+        self.view = schematic_view(self.scene, self)
+        self.init_UI()
+
+    def init_UI(self):
+        # layout statements, using a grid layout
+        gLayout = QGridLayout()
+        gLayout.setSpacing(10)
+        gLayout.addWidget(self.view, 0, 0)
+        # ratio of first column to second column is 5
+        gLayout.setColumnStretch(0, 5)
+        gLayout.setRowStretch(0, 6)
+        self.setLayout(gLayout)
+
+
+class editor_scene(QGraphicsScene):
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.parent = parent
+        self.editorWindow = self.parent.parent
+        self.majorGrid = self.editorWindow.majorGrid
+        self.gridTuple = self.editorWindow.gridTuple
+        self.mousePressLoc = None
+        self.mouseMoveLoc = None
+        self.mouseReleaseLoc = None
+        self.selectedItems = None  # selected item
+        self.readOnly = False  # if the scene is not editable
+        self.defineSceneLayers()
+        self.setPens()
+        self.undoStack = QUndoStack()
+        self.changeOrigin = False
+        self.origin = QPoint(0, 0)
+        self.snapDistance = self.editorWindow.snapDistance
+        self.cellName = self.editorWindow.file.parent.stem
+        self.selectedItems = None
+        self.partialSelection = True
+        self.selectionRectItem = None
+        self.libraryDict = self.editorWindow.libraryDict
+        self.rotateItem = False
+        self.itemContextMenu = QMenu()
+        self.appMainW = self.editorWindow.appMainW
+        self.logger = self.appMainW.logger
+        self.messageLine = self.editorWindow.messageLine
+        self.statusLine = self.editorWindow.statusLine
+        self.installEventFilter(self)
+
+    def setPens(self):
+        self.wirePen = pens.sPen.returnPen("wirePen")
+        self.symbolPen = pens.sPen.returnPen("symbolPen")
+        self.selectedWirePen = pens.sPen.returnPen("selectedWirePen")
+        self.pinPen = pens.sPen.returnPen("pinPen")
+        self.labelPen = pens.sPen.returnPen("labelPen")
+        self.textPen = pens.sPen.returnPen("textPen")
+        self.otherPen = pens.sPen.returnPen("otherPen")
+
+    def defineSceneLayers(self):
+        self.wireLayer = cel.wireLayer
+        self.symbolLayer = cel.symbolLayer
+        self.guideLineLayer = cel.guideLineLayer
+        self.selectedWireLayer = cel.selectedWireLayer
+        self.pinLayer = cel.pinLayer
+        self.labelLayer = cel.labelLayer
+        self.textLayer = cel.textLayer
+
+    def snapToBase(self, number, base):
+        '''
+        Restrict a number to the multiples of base
+        '''
+        return int(base * int(round(number / base)))
+
+    def snapToGrid(self, point: QPoint, gridTuple: tuple[int, int]):
+        """
+        snap point to grid. Divides and multiplies by grid size.
+        """
+        return QPoint(self.snapToBase(point.x(), gridTuple[0]),
+                      self.snapToBase(point.y(), gridTuple[1]))
+
+    def rotateSelectedItems(self, point: QPoint):
+        """
+        Rotate selected items by 90 degree.
+        """
+        for item in self.selectedItems:
+            self.rotateAnItem(point, item, 90)
+        self.rotateItem = False
+        self.itemSelect = True
+
+    def rotateAnItem(self, point: QPoint, item, angle):
+        rotationOriginPoint = item.mapFromScene(point)
+        item.setTransformOriginPoint(rotationOriginPoint)
+        item.angle += angle
+        item.setRotation(item.angle)
+        undoCommand = us.undoRotateShape(self, item, item.angle)
+        self.undoStack.push(undoCommand)
+
+    def eventFilter(self, source, event):
+        '''
+        Mouse events should snap to background grid points.
+        '''
+        if self.readOnly:  # if read only do not propagate any mouse events
+            return True
+        elif (event.type() == QEvent.GraphicsSceneMouseMove or
+              event.type() == QEvent.GraphicsSceneMousePress or
+              event.type() == QEvent.GraphicsSceneMouseRelease):
+            event.setScenePos(
+                self.snapToGrid(event.scenePos(), self.gridTuple).toPointF())
+            return False
+        else:
+            return super().eventFilter(source, event)
+
+    def selectSceneItems(self, modifiers):
+        if modifiers == Qt.ShiftModifier:
+
+            self.editorWindow.messageLine.setText(
+                "Draw Selection Rectangle")
+            self.selectionRectItem = QGraphicsRectItem(
+                QRectF(self.mousePressLoc, self.mousePressLoc))
+            self.selectionRectItem.setPen(self.draftPen)
+            self.addItem(self.selectionRectItem)
+        else:
+            self.editorWindow.messageLine.setText("Select an item")
+            itemsAtMousePress = self.items(self.mousePressLoc)
+            if itemsAtMousePress:
+                self.selectedItems = [item for item in itemsAtMousePress
+                                      if
+                                      item.isSelected()]
+                self.editorWindow.messageLine.setText("Item selected")
+            else:
+                self.selectedItems = None
+                self.editorWindow.messageLine.setText("Nothing selected")
+
+    def selectInRectItems(self, selectionRect: QRect, partialSelection=False):
+        """
+        Select items in the scene.
+        """
+
+        if partialSelection:  # partial selection
+            selectedItems = self.items(selectionRect,
+                                            mode=Qt.IntersectsItemShape)
+        else:
+            # full selection
+            selectedItems = self.items(selectionRect,
+                                            mode=Qt.ContainsItemShape)
+        [item.setSelected(True) for item in selectedItems]
+        return selectedItems
+
+    def selectAll(self):
+        """
+        Select all items in the scene.
+        """
+        self.selectedItems = self.items()
+        [item.setSelected(True) for item in self.selectedItems]
+
+    def deselectAll(self):
+        """
+        Deselect all items in the scene.
+        """
+        [item.setSelected(False) for item in self.selectedItems]
+        self.selectedItems = None
+
+
+class symbol_scene(editor_scene):
+    """
+    Scene for Symbol editor.
+    """
+
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.parent = parent
+        # drawing switches
+        self.selectMode()  # reset to select mode
+        # pen definitions
+        self.setPens()
+        self.draftPen = QPen(self.guideLineLayer.color, 1)
+        self.drawPin = False
+        self.itemSelect = True
+        self.drawArc = False  # draw arc
+        self.drawRect = False
+        self.drawLine = False
+        self.addLabel = False
+        self.drawCircle = False
+        self.drawMode = (
+                    self.drawLine or self.drawArc or self.drawRect or self.drawCircle)
+        self.symbolShapes = ["line", "arc", "rect", "circle", "pin", "label"]
+        self.changeOrigin = False
+        self.origin = QPoint(0, 0)
+        # some default attributes
+        self.newPin = None
+        self.pinName = ""
+        self.pinType = shp.pin.pinTypes[0]
+        self.pinDir = shp.pin.pinDirs[0]
+        self.labelDefinition = ""
+        self.labelType = shp.label.labelTypes[0]
+        self.labelOrient = shp.label.labelOrients[0]
+        self.labelAlignment = shp.label.labelAlignments[0]
+        self.labelUse = shp.label.labelUses[0]
+        self.labelVisible = False
+        self.labelHeight = "12"
+        self.labelOpaque = True
+        self.newLine = None
+        self.newRect = None
+        self.newCirc = None
+        self.newArc = None
+
+    def mousePressEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
+        super().mousePressEvent(mouse_event)
+        try:
+            modifiers = QGuiApplication.keyboardModifiers()
+            self.viewRect = self.parent.view.mapToScene(
+                self.parent.view.viewport().rect()).boundingRect()
+            if mouse_event.button() == Qt.LeftButton:
+                self.mousePressLoc = mouse_event.scenePos().toPoint()
+                if self.changeOrigin:  # change origin of the symbol
+                    self.origin = self.mousePressLoc
+                    self.changeOrigin = False
+                if self.itemSelect:
+                    self.selectSceneItems(modifiers)
+                if self.drawPin:
+                    self.editorWindow.messageLine.setText("Add Symbol Pin")
+                    self.newPin = self.pinDraw(self.mousePressLoc, self.gridTuple)
+                    self.newPin.setSelected(True)
+                elif self.drawLine:
+                    self.editorWindow.messageLine.setText('Drawing a Line')
+                    self.newLine = self.lineDraw(self.mousePressLoc,
+                                                 self.mousePressLoc,
+                                                 self.symbolPen, self.gridTuple)
+                    self.newLine.setSelected(True)
+                elif self.addLabel:
+                    self.newLabel = self.labelDraw(self.mousePressLoc, self.labelPen,
+                                                   self.labelDefinition,
+                                                   self.labelType,
+                                                   self.labelHeight,
+                                                   self.labelAlignment,
+                                                   self.labelOrient, self.labelUse,
+                                                   self.gridTuple)
+                    self.newLabel.setSelected(True)
+                elif self.drawRect:
+                    self.newRect = self.rectDraw(self.mousePressLoc,
+                                                 self.mousePressLoc,
+                                                 self.symbolPen, self.gridTuple)
+                elif self.drawCircle:
+                    self.editorWindow.messageLine.setText(
+                        'Click on the center of the circle')
+                    self.newCircle = self.circleDraw(self.mousePressLoc,
+                                                     self.mousePressLoc,
+                                                     self.symbolPen, self.gridTuple)
+                elif self.drawArc:
+                    self.editorWindow.messageLine.setText('Start drawing an arc')
+                    self.newArc = self.arcDraw(self.mousePressLoc, self.mousePressLoc,
+                                               self.symbolPen, self.gridTuple)
+                if self.rotateItem and self.selectedItems:
+                    self.rotateSelectedItems(self.mousePressLoc)
+        except Exception as e:
+            print(e)
+
+    def mouseMoveEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
+
+        super().mouseMoveEvent(mouse_event)
+        self.mouseMoveLoc = mouse_event.scenePos().toPoint()
+        modifiers = QGuiApplication.keyboardModifiers()
+        if mouse_event.buttons() == Qt.LeftButton:
+            if self.drawLine:
+                self.editorWindow.messageLine.setText(
+                    "Release mouse on the end point")
+                self.newLine.end = self.mouseMoveLoc
+            elif self.drawPin and self.newPin.isSelected():
+                self.newPin.setPos(self.mouseMoveLoc - self.mousePressLoc)
+            elif self.drawRect:
+                self.editorWindow.messageLine.setText(
+                    "Release mouse on the bottom left point")
+                self.newRect.end = self.mouseMoveLoc
+            elif self.drawCircle:
+                self.editorWindow.messageLine.setText('Extend Circle')
+                radius = ((self.mouseMoveLoc.x() - self.mousePressLoc.x()) ** 2 + (
+                                self.mouseMoveLoc.y() - self.mousePressLoc.y()) ** 2) ** 0.5
+                self.newCircle.radius = radius
+            elif self.drawArc:
+                self.editorWindow.messageLine.setText('Extend Arc')
+                self.newArc.end = self.mouseMoveLoc
+            elif self.itemSelect and modifiers == Qt.ShiftModifier:
+                self.selectionRectItem.setRect(QRectF(self.mousePressLoc,self.mouseMoveLoc))
+        self.statusLine.showMessage(
+            "Cursor Position: " + str(
+                (self.mouseMoveLoc - self.origin).toTuple()))
+
+    def mouseReleaseEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseReleaseEvent(mouse_event)
+        try:
+            self.mouseReleaseLoc = mouse_event.scenePos().toPoint()
+            modifiers = QGuiApplication.keyboardModifiers()
+            if mouse_event.button() == Qt.LeftButton:
+                if self.drawLine:
+                    self.newLine.setSelected(False)
+                elif self.drawCircle:
+                    self.newCircle.setSelected(False)
+                    self.newCircle.update()
+                elif self.drawPin:
+                    self.newPin.setSelected(False)
+
+                elif self.drawRect:
+                    self.newRect.setSelected(False)
+                elif self.drawArc:
+                    self.newArc.setSelected(False)
+                elif self.addLabel:
+                    self.newLabel.setSelected(False)
+                elif self.itemSelect and modifiers == Qt.ShiftModifier:
+                    self.selectedItems = self.selectInRectItems(self.selectionRectItem.rect(
+                    ), self.partialSelection)
+                    self.removeItem(self.selectionRectItem)
+                    self.selectionRectItem = None
+        except Exception as e:
+            print(e)
+
+
+            self.selectMode()
+
+    def lineDraw(self, start: QPoint, current: QPoint, pen: pens.sPen,
+                 gridTuple: [int, int]):
+        line = shp.line(start, current, pen, gridTuple)
+        self.addItem(line)
+        undoCommand = us.addShapeUndo(self, line)
+        self.undoStack.push(undoCommand)
+        return line
+
+    def rectDraw(self, start: QPoint, end: QPoint, pen: pens.sPen,
+                 gridTuple: [int, int]):
+        """
+        Draws a rectangle on the scene
+        """
+        # rect = shp.rectangle(start, end - QPoint(pen.width() / 2, pen.width() / 2), pen,
+        #                      gridTuple)
+        rect = shp.rectangle(start, end, pen, gridTuple)
+        self.addItem(rect)
+        undoCommand = us.addShapeUndo(self, rect)
+        self.undoStack.push(undoCommand)
+        return rect
+
+    def circleDraw(self, start: QPoint, end: QPoint, pen: pens.sPen,
+                   gridTuple: [int, int]):
+        """
+        Draws a circle on the scene
+        """
+        snappedEnd = self.snapToGrid(end, gridTuple)
+        circle = shp.circle(start, snappedEnd, pen, gridTuple)
+        self.addItem(circle)
+        undoCommand = us.addShapeUndo(self, circle)
+        self.undoStack.push(undoCommand)
+        return circle
+
+    def arcDraw(self, start: QPoint, end: QPoint, pen: pens.sPen,
+                gridTuple: [int, int]):
+        '''
+        Draws an arc inside the rectangle defined by start and end points.
+        '''
+        arc = shp.arc(start, end, pen, self.gridTuple)
+        self.addItem(arc)
+        undoCommand = us.addShapeUndo(self, arc)
+        self.undoStack.push(undoCommand)
+        return arc
+
+    def pinDraw(self, current, gridTuple: [int, int]):
+        pin = shp.pin(current, self.pinPen, self.pinName, self.pinDir,
+                      self.pinType,
+                      gridTuple)
+        self.addItem(pin)
+        undoCommand = us.addShapeUndo(self, pin)
+        self.undoStack.push(undoCommand)
+        return pin
+
+    def labelDraw(self, current, pen: pens.sPen, labelDefinition, labelType,
+                  labelHeight,
+                  labelAlignment, labelOrient, labelUse, gridTuple: [int, int]):
+        label = shp.label(current, pen, labelDefinition, gridTuple, labelType,
+                          labelHeight,
+                          labelAlignment, labelOrient, labelUse, )
+        label.labelVisible = self.labelOpaque
+        label.labelDefs()
+        label.setOpacity(1)
+        self.addItem(label)
+        undoCommand = us.addShapeUndo(self, label)
+        self.undoStack.push(undoCommand)
+        return label
+
+    def keyPressEvent(self, key_event):
+        super().keyPressEvent(key_event)
+        if key_event.key() == Qt.Key_Escape:
+            self.selectMode()
+        elif key_event.key() == Qt.Key_C:
+            self.copySelectedItems()
+        elif key_event.key() == Qt.Key_M:
+            self.stretchSelectedItem()
+
+    def selectMode(self):
+        """
+        Reset the scene mode to default. Select mode is set to True.
+        """
+        self.editorWindow.messageLine.setText("Select Mode")
+        self.drawPin = False
+        self.itemSelect = True
+        self.drawArc = False  # draw arc
+        self.drawRect = False  # draw rect
+        self.drawLine = False  # draw line
+        self.addLabel = False
+        self.drawCircle = False
+        self.rotateItem = False
+
+    def deleteSelectedItems(self):
+        if self.selectedItems:
+            for item in self.selectedItems:
+                self.removeItem(item)
+                undoCommand = us.deleteShapeUndo(self, item)
+                self.undoStack.push(undoCommand)
+            del self.selectedItems
+            self.update()  # self.selectMode()
+
+    def copySelectedItems(self):
+        if hasattr(self, "selectedItems"):
+            for item in self.selectedItems:
+                selectedItemJson = json.dumps(item, cls=se.symbolEncoder)
+                itemCopyDict = json.loads(selectedItemJson)
+                shape = lj.createSymbolItems(itemCopyDict, self.gridTuple)
+                self.addItem(shape)
+                undoCommand = us.addShapeUndo(self, shape)
+                self.undoStack.push(undoCommand)
+                # shift position by one grid unit to right and down
+                shape.setPos(QPoint(item.pos().x() + 2 * self.gridTuple[0],
+                                    item.pos().y() + 2 * self.gridTuple[1], ))
+
+    def itemProperties(self):
+        """
+        When item properties is queried.
+        """
+        if self.selectedItems:
+            for item in self.selectedItems:
+                if isinstance(item, shp.rectangle):
+                    self.queryDlg = pdlg.rectPropertyDialog(self.editorWindow, item)
+                    if self.queryDlg.exec() == QDialog.Accepted:
+                        self.updateRectangleShape(item)
+                if isinstance(item, shp.circle):
+                    self.queryDlg = pdlg.circlePropertyDialog(self.editorWindow, item)
+                    if self.queryDlg.exec() == QDialog.Accepted:
+                        self.updateCircleShape(item)
+                if isinstance(item, shp.arc):
+                    self.queryDlg = pdlg.arcPropertyDialog(self.editorWindow, item)
+                    if self.queryDlg.exec() == QDialog.Accepted:
+                        self.updateArcShape(item)
+                elif isinstance(item, shp.line):
+                    self.queryDlg = pdlg.linePropertyDialog(self.editorWindow, item)
+                    if self.queryDlg.exec() == QDialog.Accepted:
+                        self.updateLineShape(item)
+                elif isinstance(item, shp.pin):
+                    self.queryDlg = pdlg.pinPropertyDialog(self.editorWindow, item)
+                    if self.queryDlg.exec() == QDialog.Accepted:
+                        self.updatePinShape(item)
+                elif isinstance(item, shp.label):
+                    self.queryDlg = pdlg.labelPropertyDialog(self.editorWindow, item)
+                    if self.queryDlg.exec() == QDialog.Accepted:
+                        self.updateLabelShape(item)
+
+    def updateRectangleShape(self, item: shp.rectangle):
+        left = self.snapToBase(float(self.queryDlg.rectLeftLine.text()),
+                               self.gridTuple[0])
+        top = self.snapToBase(float(self.queryDlg.rectTopLine.text()),
+                              self.gridTuple[1])
+        width = self.snapToBase(float(self.queryDlg.rectWidthLine.text()),
+                                self.gridTuple[0])
+        height = self.snapToBase(float(self.queryDlg.rectHeightLine.text()),
+                                 self.gridTuple[1])
+        topLeft = item.mapFromScene(QPoint(left, top))
+        # undoUpdateRectangle = us.updateShapeUndo()
+        # us.keepOriginalShape(self, item, self.gridTuple, parent=undoUpdateRectangle)
+        item.rect = QRect(topLeft.x(), topLeft.y(), width, height)
+
+        # us.changeOriginalShape(self, item, parent=undoUpdateRectangle)  # self.undoStack.push(undoUpdateRectangle)  # self.selectedItem.update()
+
+    def updateCircleShape(self, item: shp.circle):
+
+        centerX = self.snapToBase(float(self.queryDlg.centerXEdit.text()),
+                                  self.gridTuple[0])
+        centerY = self.snapToBase(float(self.queryDlg.centerYEdit.text()),
+                                  self.gridTuple[1])
+        radius = self.snapToBase(float(self.queryDlg.radiusEdit.text()),
+                                 self.gridTuple[0])
+        centerPoint = self.snapToGrid(QPoint(centerX, centerY), self.gridTuple)
+        item.centre(item.mapFromScene(centerPoint))
+        item.radius(radius)
+
+    def updateArcShape(self, item: shp.arc):
+
+        startX = self.snapToBase(float(self.queryDlg.startXEdit.text()),
+                                 self.gridTuple[0])
+        startY = self.snapToBase(float(self.queryDlg.startYEdit.text()),
+                                 self.gridTuple[1])
+        item.start = item.mapFromScene(QPoint(startX, startY)).toPoint()
+        item.width = self.snapToBase(float(self.queryDlg.widthEdit.text()),
+                                     self.gridTuple[0])
+        item.height = self.snapToBase(float(self.queryDlg.heightEdit.text()),
+                                      self.gridTuple[1])
+
+    def updateLineShape(self, item: shp.line):
+        """
+        Updates line shape from dialogue entries.
+        """
+        startEntry = QPoint(int(float(self.queryDlg.startXLine.text())),
+                            int(float(self.queryDlg.startYLine.text())), )
+        item.start = item.mapFromScene(startEntry).toPoint()
+        endEntry = QPoint(int(float(self.queryDlg.endXLine.text())),
+                          int(float(self.queryDlg.endYLine.text())), )
+        item.end = item.mapFromScene(endEntry).toPoint()
+
+    def updatePinShape(self, item: shp.pin):
+        location = item.scenePos().toTuple()
+        item.start = self.snapToGrid(
+            QPoint(int(float(self.queryDlg.pinXLine.text()) - float(location[0])),
+                   int(float(self.queryDlg.pinYLine.text()) - float(
+                       location[1])), ),
+            self.gridTuple, )
+        item.rect = QRect(self.item.start.x() - 5,
+                          self.item.start.y() - 5,
+                          10, 10)
+        item.pinName = self.queryDlg.pinName.text()
+        item.pinType = self.queryDlg.pinType.currentText()
+        item.pinDir = self.queryDlg.pinDir.currentText()
+        item.update()
+
+    def updateLabelShape(self, item: shp.label):
+        """
+        update pin shape with new values.
+        """
+        location = item.scenePos().toTuple()
+        item.start = self.snapToGrid(
+            QPoint(
+                int(float(self.queryDlg.labelXLine.text()) - float(location[0])),
+                int(float(self.queryDlg.labelYLine.text()) - float(
+                    location[1])), ),
+            self.gridTuple, )
+        item.labelDefinition = self.queryDlg.labelDefinition.text()
+        item.labelHeight = self.queryDlg.labelHeightEdit.text()
+        item.labelAlign = self.queryDlg.labelAlignCombo.currentText()
+        item.labelOrient = self.queryDlg.labelOrientCombo.currentText()
+        item.labelUse = self.queryDlg.labelUseCombo.currentText()
+        if self.queryDlg.labelVisiCombo.currentText() == "Yes":
+            item.labelVisible = True
+        else:
+            item.labelVisible = False
+        if self.queryDlg.normalType.isChecked():
+            item.labelType = shp.label.labelTypes[0]
+        elif self.queryDlg.NLPType.isChecked():
+            item.labelType = shp.label.labelTypes[1]
+        elif self.queryDlg.pyLType.isChecked():
+            item.labelType = shp.label.labelTypes[2]
+        # set opacity to 1 so that the label is still visible on symbol editor
+        item.setOpacity(1)
+        item.labelDefs()
+        item.update()
+
+    def loadSymbol(self, itemsList: list):
+        self.attributeList = []
+        for item in itemsList[1:]:
+            if item is not None:
+                if item["type"] in self.symbolShapes:
+                    itemShape = lj.createSymbolItems(item, self.gridTuple)
+                    # items should be always visible in symbol view
+                    if isinstance(itemShape, shp.label):
+                        itemShape.setOpacity(1)
+                    self.addItem(itemShape)
+                elif item["type"] == "attr":
+                    attr = lj.createSymbolAttribute(item)
+                    self.attributeList.append(attr)
+
+    def saveSymbolCell(self, fileName):
+        # items = self.items(self.sceneRect())  # get items in scene rect
+        items = self.items()
+        items.insert(0, {"cellView": "symbol"})
+        if hasattr(self, "attributeList"):
+            items.extend(self.attributeList)  # add attribute list to list
+        with open(fileName, "w") as f:
+            try:
+                json.dump(items, f, cls=se.symbolEncoder, indent=4)
+            except Exception as e:
+                self.logger.error(e)
+
+    def stretchSelectedItem(self):
+        if self.selectedItems is not None:
+            try:
+                for item in self.selectedItems:
+                    if hasattr(item, 'stretch'):
+                        item.stretch = True
+
+            except AttributeError:
+                self.messageLine.setText("Nothing selected")
+
+    def viewSymbolProperties(self):
+        """
+        View symbol properties dialog.
+        """
+        # copy symbol attribute list to another list by deepcopy to be safe
+        attributeListCopy = deepcopy(self.attributeList)
+        symbolPropDialogue = pdlg.symbolLabelsDialogue(self.parent.parent,
+                                                       self.items(),
+                                                       attributeListCopy)
+        if symbolPropDialogue.exec() == QDialog.Accepted:
+            for i, item in enumerate(symbolPropDialogue.labelItemList):
+                # label name is not changed.
+                item.labelHeight = symbolPropDialogue.labelHeightList[i].text()
+                item.labelAlign = symbolPropDialogue.labelAlignmentList[
+                    i].currentText()
+                item.labelOrient = symbolPropDialogue.labelOrientationList[
+                    i].currentText()
+                item.labelUse = symbolPropDialogue.labelUseList[i].currentText()
+                item.labelType = symbolPropDialogue.labelTypeList[i].currentText()
+                item.update(item.boundingRect())
+            # create an empty attribute list. If the dialog is OK, the local attribute list
+            # will be copied to the symbol attribute list.
+            localAttributeList = []
+            for i, item in enumerate(symbolPropDialogue.attributeNameList):
+                if item.text().strip() != "":
+                    localAttributeList.append(se.symbolAttribute(item.text(),
+                                                                 symbolPropDialogue.attributeDefList[
+                                                                     i].text()))
+                self.attributeList = deepcopy(localAttributeList)
+
+
+class schematic_scene(editor_scene):
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.parent = parent
+        self.instCounter = 0
+        self.start = QPoint(0, 0)
+        self.current = QPoint(0, 0)
+        self.selectedItems = None
+        self.itemsAtMousePress = list()
+        self.itemContextMenu = QMenu()
+        self.drawWire = False  # flag to add wire
+        self.drawPin = False  # flag to add pin
+        self.drawText = False  # flat to add text
+        self.itemSelect = True  # flag to select item
+        self.drawMode = self.drawWire or self.drawPin
+        self.draftPen = QPen(self.guideLineLayer.color, 1)
+        self.draftPen.setStyle(Qt.DashLine)
+        self.draftPin = None
+        self.draftText = None
+        self.itemCounter = 0
+        self.netCounter = 0
+        self.schematicNets = {}  # netName: list of nets with the same name
+        self.crossDots = set()  # list of cross dots
+        self.draftItem = None
+        self.viewRect = None
+        # add instance attributes
+        self.addInstance = False
+        self.instanceSymbolFile = None
+        # pin attribute defaults
+        self.pinName = ""
+        self.pinType = "Signal"
+        self.pinDir = "Input"
+        self.parentView = None
+        self.wires = None
+        self.newInstance = None
+        self.newPin = None
+        self.newText = None
+        self.snapPointRect = None
+
+    def mousePressEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
+
+        super().mousePressEvent(mouse_event)
+        try:
+            modifiers = QGuiApplication.keyboardModifiers()
+            self.viewRect = self.parent.view.mapToScene(
+                self.parent.view.viewport().rect()).boundingRect()
+
+            if mouse_event.button() == Qt.LeftButton:
+                self.mousePressLoc = mouse_event.scenePos().toPoint()
+
+                if self.addInstance:
+                    self.newInstance = self.drawInstance(self.mousePressLoc)
+                    self.newInstance.setSelected(True)
+
+                elif self.drawWire:
+                    self.editorWindow.messageLine.setText("Wire Mode")
+                    self.wires = self.addWires(self.mousePressLoc, self.wirePen)
+
+                elif self.changeOrigin:  # change origin of the symbol
+                    self.origin = self.mousePressLoc
+
+                elif self.drawPin:
+                    self.editorWindow.messageLine.setText("Add a pin")
+                    self.newPin = self.addPin(self.mousePressLoc)
+                    self.newPin.setSelected(True)
+
+                elif self.drawText:
+                    self.editorWindow.messageLine.setText('Add a text note')
+                    self.newText = self.addNote(self.mousePressLoc)
+                    self.rotateAnItem(self.mousePressLoc, self.newText,
+                                      float(self.noteOrient[1:]))
+                    self.newText.setSelected(True)
+                elif self.rotateItem:
+                    self.editorWindow.messageLine.setText("Rotate item")
+                    if self.selectedItems:
+                        self.rotateSelectedItems(self.mousePressLoc)
+
+                elif self.itemSelect:
+                    self.selectSceneItems(modifiers)
+        except Exception as e:
+            self.logger.error(e)
+
+    def mouseMoveEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseMoveEvent(mouse_event)
+        self.mouseMoveLoc = mouse_event.scenePos().toPoint()
+        modifiers = QGuiApplication.keyboardModifiers()
+        try:
+            if mouse_event.buttons() == Qt.LeftButton:
+                if self.addInstance:
+                    # TODO: think how to do it with mapFromScene
+                    self.newInstance.setPos(self.mouseMoveLoc - self.mousePressLoc)
+
+                elif self.drawWire:
+                    self.mouseMoveLoc = self.findSnapPoint(self.mouseMoveLoc,
+                                                           self.snapDistance,
+                                                           set(self.wires))
+                    if self.snapPointRect is None:
+                        rect = QRectF(QPointF(-5, -5), QPointF(5, 5))
+                        self.snapPointRect = QGraphicsRectItem(rect)
+                        self.snapPointRect.setPen(self.draftPen)
+                        self.addItem(self.snapPointRect)
+                    self.snapPointRect.setPos(self.mouseMoveLoc)
+
+                    self.extendWires(self.wires, self.mousePressLoc,
+                                     self.mouseMoveLoc)
+                elif self.drawPin and self.newPin.isSelected():
+                    self.newPin.setPos(self.mouseMoveLoc - self.mousePressLoc)
+
+                elif self.drawText and self.newText.isSelected():
+                    self.newText.setPos(self.mouseMoveLoc - self.mousePressLoc)
+
+                elif self.itemSelect and modifiers == Qt.ShiftModifier:
+                        self.selectionRectItem.setRect(
+                            QRectF(self.mousePressLoc, self.mouseMoveLoc))
+
+            self.editorWindow.statusLine.showMessage(
+                "Cursor Position: " + str(self.mouseMoveLoc.toTuple()))
+        except Exception as e:
+            self.logger.error(e)
+
+    def mouseReleaseEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseReleaseEvent(mouse_event)
+        try:
+            self.mouseReleaseLoc = mouse_event.scenePos().toPoint()
+            modifiers = QGuiApplication.keyboardModifiers()
+            if mouse_event.button() == Qt.LeftButton:
+                if self.drawWire and self.wires:
+                    self.mouseReleaseLoc = self.findSnapPoint(self.mouseReleaseLoc,
+                                                              self.snapDistance,
+                                                              set(self.wires))
+                    self.extendWires(self.wires, self.mousePressLoc,
+                                     self.mouseReleaseLoc)
+                    if self.snapPointRect:
+                        self.removeItem(self.snapPointRect)
+                        self.snapPointRect = None
+
+                    lines = self.pruneWires(self.wires, self.wirePen)
+                    if lines:
+                        for line in lines:
+                            line.mergeNets()
+                    self.wires = None  # self.mergeNets()
+                    viewNets = {netItem for netItem in
+                                self.editorWindow.centralW.view.items() if
+                                isinstance(netItem,net.schematicNet)}
+                    [netItem.findDotPoints() for netItem in viewNets]
+
+                elif self.addInstance:
+                    self.addInstance = False
+                    self.newInstance = None
+
+                elif self.drawText:
+                    self.parent.parent.messageLine.setText("Note added.")
+                    self.drawText = False
+                    self.newText = None
+                elif self.drawPin:
+                    self.parent.parent.messageLine.setText("Pin added")
+                    self.drawPin = False
+                    self.newPin = None
+                elif self.itemSelect and modifiers == Qt.ShiftModifier:
+                    self.selectedItems = self.selectInRectItems(self.selectionRectItem.rect(
+                    ), self.partialSelection)
+                    self.removeItem(self.selectionRectItem)
+                    self.selectionRectItem = None
+        except Exception as e:
+            print(e)
+
+    def findSnapPoint(self, eventLoc: QPoint, snapDistance: int,
+                      ignoredNetSet: set):
+        snapRect = QRect(eventLoc.x() - snapDistance, eventLoc.y() - snapDistance,
+                         2 * snapDistance, 2 * snapDistance)
+        snapItems = {item for item in self.items(snapRect) if
+                     isinstance(item, shp.pin) or isinstance(item,
+                                                             net.schematicNet)}
+
+        try:
+            snapItems -= ignoredNetSet
+            lengths = list()
+            points = list()
+            items = list()
+            if len(snapItems) > 0:
+                for item in snapItems:
+                    if isinstance(item, shp.pin):
+                        items.append(item)
+                        points.append(item.mapToScene(item.start))
+                        lengths.append(
+                            (item.mapToScene(
+                                item.start) - eventLoc).manhattanLength())
+                    elif isinstance(item, net.schematicNet):
+                        if snapRect.contains(item.line().p1().toPoint()):
+                            items.append(item)
+                            # print(f'net start:{item.start}')
+                            points.append(item.line().p1().toPoint())
+                            lengths.append((item.mapToScene(
+                                item.line().p1()) - eventLoc).manhattanLength())
+                        elif snapRect.contains(item.line().p2().toPoint()):
+                            items.append(item)
+                            points.append(item.line().p2().toPoint())
+                            # print(f'net end:{item.end}')
+                            lengths.append((item.mapToScene(
+                                item.line().p2()) - eventLoc).manhattanLength())
+                if len(lengths) > 0:
+                    indexClosestPoint = lengths.index(min(lengths))
+                    eventLoc = points[indexClosestPoint]
+
+            return eventLoc
+        except Exception as e:
+            self.logger.error(e)  # no items found
+            return eventLoc
+
+    def clearNetStatus(self, netsSet: set):
+        '''
+        Clear all assigned net names
+        '''
+        for netItem in netsSet:
+            netItem.nameAdded = False
+            netItem.nameConflict = False
+
+    def groupAllNets(self) -> None:
+        """
+        This method starting from nets connected to pins, then named nets and unnamed
+        nets, groups all the nets in the schematic.
+        """
+        try:
+            # all the nets in the schematic in a set to remove duplicates
+            sceneNetsSet = self.findSceneNetsSet()
+            self.clearNetStatus(sceneNetsSet)
+            # first find nets connected to pins designating global nets.
+            globalNetsSet = self.findGlobalNets()
+            sceneNetsSet -= globalNetsSet  # remove these nets from all nets set.
+            # now remove nets connected to global nets from this set.
+            sceneNetsSet = self.groupNamedNets(globalNetsSet, sceneNetsSet)
+            # now find nets connected to schematic pins
+            schemPinConNetsSet = self.findSchPinNets()
+            sceneNetsSet -= schemPinConNetsSet
+            # use these nets as starting nets to find other nets connected to them
+            sceneNetsSet = self.groupNamedNets(schemPinConNetsSet, sceneNetsSet)
+            # now find the set of nets whose name is set by the user
+            namedNetsSet = set(
+                [netItem for netItem in sceneNetsSet if netItem.nameSet])
+            sceneNetsSet -= namedNetsSet
+            # now remove already named net set from firstNetSet
+            unnamedNets = self.groupNamedNets(namedNetsSet, sceneNetsSet)
+            # now start netlisting from the unnamed nets
+            self.groupUnnamedNets(unnamedNets, self.netCounter)
+        except Exception as e:
+            self.logger.error(e)
+
+    def findGlobalNets(self) -> set:
+        """
+        This method finds all nets connected to global pins.
+        """
+        try:
+            globalPinsSet = set()
+            globalNetsSet = set()
+            for symbolItem in self.findSceneSymbolSet():
+                for pinName, pinItem in symbolItem.pins.items():
+                    if pinName[-1] == '!':
+                        globalPinsSet.add(pinItem)
+            # self.logger.warning(f'global pins:{globalPinsSet}')
+            for pinItem in globalPinsSet:
+                pinNetSet = {netItem for netItem in
+                             self.items(pinItem.sceneBoundingRect())
+                             if isinstance(netItem, net.schematicNet)}
+                for netItem in pinNetSet:
+                    if netItem.nameSet or netItem.nameAdded:
+                        # check if net is already named explicitly
+                        if netItem.name != pinItem.pinName:
+                            netItem.nameConflict = True
+                            self.logger.error(
+                                f"Net name conflict at {pinItem.pinName} of "
+                                f"{pinItem.parent.instanceName}.")
+                        else:
+                            globalNetsSet.add(netItem)
+                    else:
+                        globalNetsSet.add(netItem)
+                        netItem.name = pinItem.pinName
+                        netItem.nameAdded = True
+            return globalNetsSet
+        except Exception as e:
+            self.logger.error(e)
+
+    def findSchPinNets(self):
+        # nets connected to schematic pins.
+        schemPinConNetsSet = set()
+        # first start from schematic pins
+        sceneSchemPinsSet = self.findSceneSchemPinsSet()
+        for sceneSchemPin in sceneSchemPinsSet:
+            pinNetSet = {netItem for netItem in
+                         self.items(sceneSchemPin.sceneBoundingRect()) if
+                         isinstance(netItem, net.schematicNet)}
+            for netItem in pinNetSet:
+                if netItem.nameSet or netItem.nameAdded:  # check if net is named
+                    if netItem.name == sceneSchemPin.pinName:
+                        schemPinConNetsSet.add(netItem)
+                    else:
+                        netItem.nameConflict = True
+                        self.parent.parent.logger.error(
+                            f"Net name conflict at {sceneSchemPin.pinName} of "
+                            f"{sceneSchemPin.parent.instanceName}.")
+                else:
+                    schemPinConNetsSet.add(netItem)
+                    netItem.name = sceneSchemPin.pinName
+                    netItem.nameAdded = True
+                netItem.update()
+            schemPinConNetsSet.update(pinNetSet)
+        return schemPinConNetsSet
+
+    def groupNamedNets(self, namedNetsSet, unnamedNetsSet):
+        """
+        Groups nets with the same name using namedNetsSet members as seeds and going
+        through connections. Returns the set of still unnamed nets.
+        """
+        for netItem in namedNetsSet:
+            if self.schematicNets.get(netItem.name) is None:
+                self.schematicNets[netItem.name] = set()
+            connectedNets, unnamedNetsSet = self.traverseNets({netItem, },
+                                                              unnamedNetsSet, )
+            self.schematicNets[netItem.name] |= connectedNets
+        # These are the nets not connected to any named net
+        return unnamedNetsSet
+
+    def groupUnnamedNets(self, unnamedNetsSet: set[net.schematicNet],
+                         nameCounter: int):
+        """
+        Groups nets together if they are connected and assign them default names
+        if they don't have a name assigned.
+        """
+        # select a net from the set and remove it from the set
+        try:
+            initialNet = (
+                unnamedNetsSet.pop())  # assign it a name, net0, net1, net2, etc.
+        except KeyError:  # initialNet set is empty
+            pass
+        else:
+            initialNet.name = "net" + str(nameCounter)
+            # now go through the set and see if any of the
+            # nets are connected to the initial net
+            # remove them from the set and add them to the initial net's set
+            self.schematicNets[
+                initialNet.name], unnamedNetsSet = self.traverseNets(
+                {initialNet, }, unnamedNetsSet, )
+            nameCounter += 1
+            if len(unnamedNetsSet) > 1:
+                self.groupUnnamedNets(unnamedNetsSet, nameCounter)
+            elif len(unnamedNetsSet) == 1:
+                lastNet = unnamedNetsSet.pop()
+                lastNet.name = "net" + str(nameCounter)
+                self.schematicNets[lastNet.name] = {lastNet}
+
+    def traverseNets(self, connectedSet, otherNetsSet):
+        """
+        Start from a net and traverse the schematic to find all connected nets. If the connected net search
+        is exhausted, remove those nets from the scene nets set and start again in another net until all
+        the nets in the scene are exhausted.
+        """
+        newFoundConnectedSet = set()
+        for netItem in connectedSet:
+            for netItem2 in otherNetsSet:
+                if self.checkNetConnect(netItem, netItem2):
+                    if ((netItem2.nameSet or netItem2.nameAdded) and (
+                            netItem.nameSet or netItem.nameAdded) and (
+                            netItem.name != netItem2.name)):
+                        self.editorWindow.messageLine.setText(
+                            "Error: multiple names assigned to same net")
+                        netItem2.nameConflict = True
+                        netItem.nameConflict = True
+                        break
+                    else:
+                        netItem2.name = netItem.name
+                        netItem2.nameAdded = True
+                    newFoundConnectedSet.add(netItem2)
+        # keep searching if you already found a net connected to the initial net
+        if len(newFoundConnectedSet) > 0:
+            connectedSet.update(newFoundConnectedSet)
+            otherNetsSet -= newFoundConnectedSet
+            self.traverseNets(connectedSet, otherNetsSet)
+        return connectedSet, otherNetsSet
+
+    def checkPinNetConnect(self, pinItem: shp.schematicPin,
+                           netItem: net.schematicNet):
+        """
+        Determine if a pin is connected to a net.
+        """
+        if pinItem.sceneBoundingRect().intersects(netItem.sceneBoundingRect()):
+            return True
+        else:
+            return False
+
+    def checkNetConnect(self, netItem, otherNetItem):
+        """
+        Determine if a net is connected to another one. One net should end on the other net.
+        """
+        netBRect = netItem.sceneBoundingRect().adjusted(-2, -2, 2, 2)
+        if otherNetItem is not netItem:
+            otherBRect = otherNetItem.sceneBoundingRect().adjusted(-2, -2, 2, 2)
+            for endPoint in netItem.endPoints:
+                if otherBRect.contains(endPoint):
+                    return True
+            for endPoint in otherNetItem.endPoints:
+                if netBRect.contains(endPoint):
+                    return True
+        else:
+            return False
+
+    def generatePinNetMap(self, sceneSymbolSet):
+        """
+        For symbols in sceneSymbolSet, find which pin is connected to which net. If a
+        pin is not connected, assign to it a default net starting with d prefix.
+        """
+        netCounter = 0
+        for symbolItem in sceneSymbolSet:
+            for pinName, pinItem in symbolItem.pins.items():
+                pinItem.connected = False  # clear connections
+
+                pinConnectedNets = [netItem for netItem in self.items(
+                    pinItem.sceneBoundingRect().adjusted(-2, -2, 2, 2)) if
+                                    isinstance(netItem, net.schematicNet)]
+                # this will name the pin by first net it finds in the bounding rectangle of
+                # the pin. If there are multiple nets in the bounding rectangle, the first
+                # net in the list will be the one used.
+                if pinConnectedNets:
+                    symbolItem.pinNetMap[pinName] = pinConnectedNets[0].name
+                    pinItem.connected = True
+
+                if not pinItem.connected:
+                    # assign a default net name prefixed with d(efault).
+                    symbolItem.pinNetMap[pinName] = f"dnet{netCounter}"
+                    self.logger.warning(
+                        f"left unconnected:{symbolItem.pinNetMap[pinName]}")
+                    netCounter += 1
+            # now reorder pinNetMap according pinOrder attribute
+            if symbolItem.attr.get('pinOrder'):
+                pinOrderList = list()
+                [pinOrderList.append(item.strip()) for item in
+                 symbolItem.attr.get(
+                     'pinOrder').split(',')]
+                symbolItem.pinNetMap = {
+                    pinName: symbolItem.pinNetMap[pinName] for pinName in
+                    pinOrderList}
+
+    def findSceneCells(self, symbolSet):
+        """
+        This function just goes through set of symbol items in the scene and
+        checks if that symbol's cell is encountered first time. If so, it adds
+        it to a dictionary   cell_name:symbol
+        """
+        symbolGroupDict = dict()
+        for symbolItem in symbolSet:
+            if symbolItem.cellName not in symbolGroupDict.keys():
+                symbolGroupDict[symbolItem.cellName] = symbolItem
+        return symbolGroupDict
+
+    def findSceneSymbolSet(self) -> set[shp.symbolShape]:
+        """
+        Find all the symbols on the scene as a set.
+        """
+        symbolSceneSet = {item for item in self.items() if
+                          isinstance(item, shp.symbolShape)}
+        return symbolSceneSet
+
+    def findSceneNetsSet(self) -> set[net.schematicNet]:
+        return set(
+            item for item in self.items() if isinstance(item, net.schematicNet))
+
+    def findSceneSchemPinsSet(self) -> set[shp.schematicPin]:
+        pinsSceneSet = {item for item in self.items() if
+                        isinstance(item, shp.schematicPin)}
+        if pinsSceneSet:  # check pinsSceneSet is empty
+            return pinsSceneSet
+        else:
+            return set()
+
+    def findSceneTextSet(self) -> set[shp.text]:
+        textSceneSet = {item for item in self.items() if
+                        isinstance(item, shp.text)}
+        if textSceneSet:  # check textSceneSet is empty
+            return textSceneSet
+        else:
+            return set()
+
+    def keyPressEvent(self, key_event):
+        super().keyPressEvent(key_event)
+        if key_event.key() == Qt.Key_Escape:
+            self.resetSceneMode()
+
+    def resetSceneMode(self):
+        self.itemSelect = True
+        self.drawWire = False
+        self.drawPin = False
+        self.selectedItems = []
+        self.parent.parent.messageLine.setText("Select Mode")
+
+    def addWires(self, start: QPoint, pen: pens.sPen) -> net.schematicNet:
+        """
+        Add a net or nets to the scene.
+        """
+        lines = [net.schematicNet(start, start, pen),
+                 net.schematicNet(start, start, pen),
+                 net.schematicNet(start, start, pen)]
+        return lines
+
+    def extendWires(self, lines: list, start: QPoint, end: QPoint):
+        '''
+        This method is to shape the wires drawn using addWires method.
+        __|^^^
+        '''
+        try:
+            firstPointX = self.snapToBase((end.x() - start.x()) / 3 + start.x(),
+                                          self.gridTuple[0])
+            firstPointY = start.y()
+            firstPoint = QPoint(firstPointX, firstPointY)
+            secondPoint = QPoint(firstPointX, end.y())
+            [self.addItem(line) for line in lines if line.scene() is None]
+            lines[0].start = start
+            lines[0].end = firstPoint
+            lines[1].start = firstPoint
+            lines[1].end = secondPoint
+            lines[2].start = secondPoint
+            lines[2].end = end
+        except Exception as e:
+            self.logger.error(e)
+
+    def pruneWires(self, lines, pen):
+        if lines[0].start == lines[
+            2].end:  # if the first and last points are the same
+            for line in lines:
+                self.removeItem(line)
+                del line
+            return None
+        # if the line is vertical or horizontal
+        elif lines[0].start.x() == lines[2].end.x() or lines[0].start.y() == \
+                lines[
+                    2].end.y():
+            newLine = net.schematicNet(lines[0].start, lines[2].end, pen)
+            self.addItem(newLine)
+            undoCommand = us.addShapeUndo(self, newLine)
+            self.undoStack.push(undoCommand)
+            for line in lines:
+                self.removeItem(line)
+                del line
+            return [newLine]
+        else:
+            for line in lines:
+                if line.length == 0:
+                    self.removeItem(line)
+                    lines.remove(line)
+                    del line
+                else:
+                    undoCommand = us.addShapeUndo(self, line)
+                    self.undoStack.push(undoCommand)
+            return lines
+
+    def addPin(self, pos: QPoint):
+        try:
+            pin = shp.schematicPin(pos, self.pinPen, self.pinName, self.pinDir,
+                                   self.pinType,
+                                   self.gridTuple)
+            self.addItem(pin)
+            undoCommand = us.addShapeUndo(self, pin)
+            self.undoStack.push(undoCommand)
+            return pin
+        except Exception as e:
+            self.logger.error(e)
+
+    def addNote(self, pos: QPoint):
+        """
+        Changed the method name not to clash with qgraphicsscene addText method.
+        """
+        text = shp.text(pos, self.textPen, self.noteText, self.gridTuple,
+                        self.noteFontFamily, self.noteFontStyle,
+                        self.noteFontSize,
+                        self.noteAlign, self.noteOrient, )
+        self.addItem(text)
+        undoCommand = us.addShapeUndo(self, text)
+        self.undoStack.push(undoCommand)
+        return text
+
+    def drawInstance(self, pos: QPoint):
+        """
+        Add an instance of a symbol to the scene.
+        """
+        instance = self.instSymbol(self.instanceSymbolFile, pos)
+        self.addItem(instance)
+        self.itemCounter += 1
+        undoCommand = us.addShapeUndo(self, instance)
+        self.undoStack.push(undoCommand)
+        return instance
+
+    def instSymbol(self, file: pathlib.Path, pos: QPoint):
+        """
+        Read a symbol file and create symbolShape objects from it.
+        """
+        assert isinstance(file, pathlib.Path)
+        itemShapes = []
+        itemAttributes = {}
+        draftPen = QPen(self.guideLineLayer.color, 1)
+        with open(file, "r") as temp:
+            try:
+                items = json.load(temp)
+                if items[0]["cellView"] == "symbol":
+                    for item in items[1:]:
+                        if item["type"] == 'attr':
+                            itemAttributes[item["nam"]] = item["def"]
+                        else:
+                            itemShapes.append(
+                                lj.createSymbolItems(item, self.gridTuple))
+                else:
+                    self.logger.error("Not a symbol!")
+
+                # create a symbol instance passing item shapes and attributes as
+                # arguments
+                symbolInstance = shp.symbolShape(draftPen, self.gridTuple,
+                                                 itemShapes,
+                                                 itemAttributes)
+                symbolInstance.setPos(pos)
+                # For each instance assign a counter number from the scene
+                symbolInstance.counter = self.itemCounter
+
+                symbolInstance.instanceName = f"I{symbolInstance.counter}"
+                symbolInstance.libraryName = file.parent.parent.stem
+                symbolInstance.cellName = file.parent.stem
+                symbolInstance.viewName = "symbol"
+                for item in symbolInstance.labels.values():
+                    item.labelDefs()
+                return symbolInstance
+            except json.JSONDecodeError:
+                # print("Invalid JSON file")
+                self.logger.warning("Invalid JSON File")
+
+    def deleteSelectedItems(self):
+        try:
+            for item in self.selectedItems:
+                self.removeItem(item)
+            del self.selectedItems
+            self.update()
+            self.itemSelect = True
+        except TypeError:
+            pass
+
+    def copySelectedItems(self):
+        if self.selectedItems is not None:
+            for item in self.selectedItems:
+                selectedItemJson = json.dumps(item, cls=se.schematicEncoder)
+                itemCopyDict = json.loads(selectedItemJson)
+                if isinstance(item, shp.symbolShape):
+                    self.itemCounter += 1
+                    itemCopyDict["name"] = f"I{self.itemCounter}"
+                    itemCopyDict['ic'] = int(self.itemCounter)
+                    itemCopyDict["ld"]["instName"][0] = f"I{self.itemCounter}"
+                    shape = lj.createSchematicItems(itemCopyDict,
+                                                    self.libraryDict,
+                                                    item.viewName, self.gridTuple)
+                    [label.labelDefs() for label in shape.labels.values()]
+                elif isinstance(item, net.schematicNet):
+                    shape = lj.createSchematicNets(itemCopyDict)
+                elif isinstance(item, shp.schematicPin):
+                    shape = lj.createSchematicPins(itemCopyDict, self.gridTuple)
+                elif isinstance(item, shp.text):
+                    shape = lj.createTextItem(itemCopyDict, self.gridTuple)
+                if shape is not None:
+                    self.addItem(shape)
+                # shift position by one grid unit to right and down
+                shape.setPos(QPoint(item.pos().x() + 4 * self.gridTuple[0],
+                                    item.pos().y() + 4 * self.gridTuple[1], ))
+                undoCommand = us.addShapeUndo(self, shape)
+                self.undoStack.push(undoCommand)
+
+    def saveSchematicCell(self, file: pathlib.Path):
+        self.sceneR = self.sceneRect()  # get scene rect
+        # items = self.items(self.sceneR)  # get items in scene rect
+        # only save symbol shapes
+        symbolItems = self.findSceneSymbolSet()
+        netItems = self.findSceneNetsSet()
+        pinItems = self.findSceneSchemPinsSet()
+        textItems = self.findSceneTextSet()
+        items = list(symbolItems | netItems | pinItems | textItems)
+        items.insert(0, {"cellView": "schematic"})
+        with open(file, "w") as f:
+            json.dump(items, f, cls=se.schematicEncoder, indent=4)
+        if self.parent.parent.parentView is not None:
+            if type(self.parentView) == schematicEditor:
+                self.parent.parent.parentView.loadSchematic()
+            elif type(self.parentView) == symbolEditor:
+                self.parent.parent.parentView.loadSymbol()
+
+    def loadSchematicCell(self, itemsList):
+        """
+        load schematic from item list
+        """
+        for item in itemsList[1:]:
+            if item is not None:
+                if item["type"] == "symbolShape":
+                    itemShape = lj.createSchematicItems(item, self.libraryDict,
+                                                        "symbol",
+                                                        self.gridTuple)
+                    self.addItem(itemShape)
+                    if itemShape.counter > self.itemCounter:
+                        self.itemCounter = itemShape.counter
+                    [labelItem.labelDefs() for labelItem in itemShape.labels.values()]
+                elif item["type"] == "schematicNet":
+                    netShape = lj.createSchematicNets(item)
+                    self.addItem(netShape)
+                elif item["type"] == "schematicPin":
+                    pinShape = lj.createSchematicPins(item, self.gridTuple)
+                    self.addItem(pinShape)
+                elif item["type"] == "text":
+                    text = lj.createTextItem(item, self.gridTuple)
+                    self.addItem(text)
+
+        # increment item counter for next symbol
+        self.itemCounter += 1
+        # self.addItem(shp.text(QPoint(0, 200), self.textPen, 'Revolution EDA'))
+        self.update()
+
+    def viewObjProperties(self):
+        """
+        Display the properties of the selected object.
+        """
+        if self.selectedItems is not None:
+            for item in self.selectedItems:
+                if isinstance(item, shp.symbolShape):
+                    dlg = pdlg.instanceProperties(self.editorWindow, item)
+                    if dlg.exec() == QDialog.Accepted:
+                        item.instanceName = dlg.instNameEdit.text().strip()
+                        item.angle = float(dlg.angleEdit.text().strip())
+
+                        location = self.snapToGrid(
+                            QPoint(float(dlg.xLocationEdit.text().strip()),
+                                   float(dlg.yLocationEdit.text().strip()), ),
+                            self.gridTuple, )
+                        item.setPos(location)
+                        tempDoc = QTextDocument()
+                        for i in range(dlg.instanceLabelsLayout.rowCount()):
+                            # first create label name document with HTML annotations
+                            tempDoc.setHtml(
+                                dlg.instanceLabelsLayout.itemAtPosition(i,
+                                                                        0).widget().text())
+                            # now strip html annotations
+                            tempLabelName = tempDoc.toPlainText().strip()
+                            # check if label name is in label dictionary of item.
+                            if item.labels.get(tempLabelName):
+                                item.labels[tempLabelName].labelValue = (
+                                    dlg.instanceLabelsLayout.itemAtPosition(i,
+                                                                            1).widget().text())
+                                visible = (
+                                    dlg.instanceLabelsLayout.itemAtPosition(i,
+                                                                            2).widget().currentText())
+                                if visible == "True":
+                                    item.labels[tempLabelName].labelVisible = True
+                                else:
+                                    item.labels[
+                                        tempLabelName].labelVisible = False
+                        [labelItem.labelDefs() for labelItem in
+                         item.labels.values()]  # item.update()
+                elif isinstance(item, net.schematicNet):
+                    dlg = pdlg.netProperties(self.parent.parent, item)
+                    if dlg.exec() == QDialog.Accepted:
+                        item.name = dlg.netNameEdit.text().strip()
+                        item.nameSet = True
+                        item.update()
+                elif isinstance(item, shp.text):
+                    dlg = pdlg.noteTextEditProperties(self.parent.parent, item)
+                    if dlg.exec() == QDialog.Accepted:
+                        # item.prepareGeometryChange()
+                        start = item.start
+                        self.removeItem(item)
+                        item = shp.text(start, self.textPen,
+                                        dlg.plainTextEdit.toPlainText(),
+                                        self.gridTuple,
+                                        dlg.familyCB.currentText(),
+                                        dlg.fontStyleCB.currentText(),
+                                        dlg.fontsizeCB.currentText(),
+                                        dlg.textAlignmCB.currentText(),
+                                        dlg.textOrientCB.currentText(), )
+                        self.rotateAnItem(start, item, float(item.textOrient[1:]))
+                        self.addItem(item)
+
+    def createSymbol(self):
+        """
+        Create a symbol view for a schematic.
+        """
+        oldSymbolItem = False
+
+        askViewNameDlg = pdlg.symbolNameDialog(self.parent.parent.file.parent,
+                                               self.parent.parent.cellName,
+                                               self.parent.parent, )
+        if askViewNameDlg.exec() == QDialog.Accepted:
+            symbolViewName = askViewNameDlg.symbolViewsCB.currentText()
+            if symbolViewName in askViewNameDlg.symbolViewNames:
+                oldSymbolItem = True
+            if oldSymbolItem:
+                deleteSymViewDlg = fd.deleteSymbolDialog(
+                    self.parent.parent.cellName,
+                    symbolViewName, self.parent.parent)
+                if deleteSymViewDlg.exec() == QDialog.Accepted:
+                    symbolViewItem = self.generateSymbol(symbolViewName)
+                    self.editorWindow.appMainW.libraryBrowser.openCellView(
+                        symbolViewItem, self.editorWindow.cellItem,
+                        self.editorWindow.libItem)
+            else:
+                symbolViewItem = self.generateSymbol(symbolViewName)
+                self.editorWindow.appMainW.libraryBrowser.openCellView(
+                    symbolViewItem,
+                    self.editorWindow.cellItem, self.editorWindow.libItem)
+
+    def generateSymbol(self, symbolViewName: str):
+        # openPath = pathlib.Path(cellItem.data(Qt.UserRole + 2))
+        libName = self.editorWindow.libName
+        cellName = self.editorWindow.cellName
+        libItem = libm.getLibItem(self.editorWindow.libraryView.libraryModel,
+                                  libName)
+        cellItem = libm.getCellItem(libItem, cellName)
+        libraryView = self.editorWindow.libraryView
+        schematicPins = list(self.findSceneSchemPinsSet())
+
+        schematicPinNames = [pinItem.pinName for pinItem in schematicPins]
+
+        inputPins = [pinItem.pinName for pinItem in schematicPins if
+                     pinItem.pinDir == shp.schematicPin.pinDirs[0]]
+
+        outputPins = [pinItem.pinName for pinItem in schematicPins if
+                      pinItem.pinDir == shp.schematicPin.pinDirs[1]]
+
+        inoutPins = [pinItem.pinName for pinItem in schematicPins if
+                     pinItem.pinDir == shp.schematicPin.pinDirs[2]]
+
+        dlg = pdlg.symbolCreateDialog(self.parent.parent, inputPins, outputPins,
+                                      inoutPins)
+        if dlg.exec() == QDialog.Accepted:
+            symbolViewItem = scb.createCellView(self.parent.parent,
+                                                symbolViewName,
+                                                cellItem)
+            libraryDict = self.parent.parent.libraryDict
+            # create symbol editor window with an empty items list
+            symbolWindow = symbolEditor(symbolViewItem, libraryDict, libraryView)
+            try:
+                leftPinNames = list(filter(None, [pinName.strip() for pinName in
+                                                  dlg.leftPinsEdit.text().split(
+                                                      ",")], ))
+                rightPinNames = list(filter(None, [pinName.strip() for pinName in
+                                                   dlg.rightPinsEdit.text().split(
+                                                       ",")], ))
+                topPinNames = list(filter(None, [pinName.strip() for pinName in
+                                                 dlg.topPinsEdit.text().split(
+                                                     ",")], ))
+                bottomPinNames = list(filter(None, [pinName.strip() for pinName in
+                                                    dlg.bottomPinsEdit.text().split(
+                                                        ",")], ))
+                stubLength = int(float(dlg.stubLengthEdit.text().strip()))
+                pinDistance = int(float(dlg.pinDistanceEdit.text().strip()))
+                rectXDim = (max(len(topPinNames),
+                                len(bottomPinNames)) + 1) * pinDistance
+                rectYDim = (max(len(leftPinNames),
+                                len(rightPinNames)) + 1) * pinDistance
+            except ValueError:
+                self.logger.error("Enter valid value")
+
+        # add window to open windows list
+        libraryView.openViews[
+            f"{libName}_{cellName}_{symbolViewName}"] = symbolWindow
+        symbolScene = symbolWindow.centralW.scene
+        symbolScene.rectDraw(QPoint(0, 0), QPoint(rectXDim, rectYDim),
+                             self.symbolPen,
+                             symbolScene.gridTuple)
+        symbolScene.labelDraw(QPoint(int(0.25 * rectXDim), int(0.4 * rectYDim)),
+                              self.labelPen, "[@cellName]", "NLPLabel", "12",
+                              "Center",
+                              "R0", "Instance", symbolScene.gridTuple)
+        symbolScene.labelDraw(QPoint(int(rectXDim), int(-0.2 * rectYDim)),
+                              self.labelPen,
+                              "[@instName]", "NLPLabel", "12", "Center", "R0",
+                              "Instance",
+                              symbolScene.gridTuple)
+        leftPinLocs = [QPoint(-stubLength, (i + 1) * pinDistance) for i in
+                       range(len(leftPinNames))]
+        rightPinLocs = [QPoint(rectXDim + stubLength, (i + 1) * pinDistance) for i
+                        in
+                        range(len(rightPinNames))]
+        bottomPinLocs = [QPoint((i + 1) * pinDistance, rectYDim + stubLength) for
+                         i in
+                         range(len(bottomPinNames))]
+        topPinLocs = [QPoint((i + 1) * pinDistance, -stubLength) for i in
+                      range(len(topPinNames))]
+        for i in range(len(leftPinNames)):
+            symbolScene.lineDraw(leftPinLocs[i],
+                                 leftPinLocs[i] + QPoint(stubLength, 0),
+                                 symbolScene.symbolPen, symbolScene.gridTuple)
+            symbolScene.addItem(
+                schematicPins[
+                    schematicPinNames.index(leftPinNames[i])].toSymbolPin(
+                    leftPinLocs[i], symbolScene.pinPen, symbolScene.gridTuple))
+        for i in range(len(rightPinNames)):
+            symbolScene.lineDraw(rightPinLocs[i],
+                                 rightPinLocs[i] + QPoint(-stubLength, 0),
+                                 symbolScene.symbolPen, symbolScene.gridTuple)
+            symbolScene.addItem(
+                schematicPins[
+                    schematicPinNames.index(rightPinNames[i])].toSymbolPin(
+                    rightPinLocs[i], symbolScene.pinPen, symbolScene.gridTuple))
+        for i in range(len(topPinNames)):
+            symbolScene.lineDraw(topPinLocs[i],
+                                 topPinLocs[i] + QPoint(0, stubLength),
+                                 symbolScene.symbolPen, symbolScene.gridTuple)
+            symbolScene.addItem(
+                schematicPins[
+                    schematicPinNames.index(topPinNames[i])].toSymbolPin(
+                    topPinLocs[i], symbolScene.pinPen, symbolScene.gridTuple))
+        for i in range(len(bottomPinNames)):
+            symbolScene.lineDraw(bottomPinLocs[i],
+                                 bottomPinLocs[i] + QPoint(0, -stubLength),
+                                 symbolScene.symbolPen, symbolScene.gridTuple)
+            symbolScene.addItem(
+                schematicPins[
+                    schematicPinNames.index(bottomPinNames[i])].toSymbolPin(
+                    bottomPinLocs[i], symbolScene.pinPen,
+                    symbolScene.gridTuple))  # symbol attribute generation for netlisting.
+        symbolScene.attributeList = list()  # empty attribute list
+
+        symbolScene.attributeList.append(se.symbolAttribute("XyceNetlistLine",
+                                                            "X[@instName] [@cellName] [@pinList]"))
+
+        symbolWindow.checkSaveCell()
+        libraryView.reworkDesignLibrariesView(self.appMainW.libraryDict)
+        # symbolWindow.show()
+        return symbolViewItem
+
+    def goDownHier(self):
+        if self.selectedItems is not None:
+            for item in self.selectedItems:
+                if isinstance(item, shp.symbolShape):
+                    dlg = fd.goDownHierDialogue(self.editorWindow)
+                    libItem = libm.getLibItem(
+                        self.editorWindow.libraryView.libraryModel,
+                        item.libraryName)
+                    cellItem = libm.getCellItem(libItem, item.cellName)
+                    viewNames = [cellItem.child(i).text() for i in range(
+                        cellItem.rowCount()) if
+                                 cellItem.child(i).text() != item.viewName]
+                    dlg.viewListCB.addItems(viewNames)
+                    if dlg.exec() == QDialog.Accepted:
+                        libItem = libm.getLibItem(
+                            self.editorWindow.libraryView.libraryModel,
+                            item.libraryName)
+                        cellItem = libm.getCellItem(libItem, item.cellName)
+                        viewItem = libm.getViewItem(cellItem,
+                                                    dlg.viewListCB.currentText())
+                        openViewT = self.editorWindow.libraryView.libBrowsW.openCellView(
+                            viewItem, cellItem, libItem)
+                        if self.editorWindow.appMainW.openViews[openViewT]:
+                            childWindow = self.editorWindow.appMainW.openViews[
+                                openViewT]
+                            childWindow.parentView = self.editorWindow
+                            if dlg.buttonId == 2:
+                                childWindow.centralW.scene.readOnly = True
+
+    def goUpHier(self):
+        if self.editorWindow.parentView:
+            self.editorWindow.parentView.raise_()
+            self.editorWindow.close()
+
+
+class editor_view(QGraphicsView):
+    """
+    The qgraphicsview for qgraphicsscene. It is used for both schematic and layout editors.
+    """
+
+    def __init__(self, scene, parent):
+        super().__init__(scene, parent)
+        self.parent = parent
+        self.editor = self.parent.parent
+        self.scene = scene
+        self.logger = self.scene.logger
+        self.majorGrid = self.editor.majorGrid
+        self.gridTuple = self.editor.gridTuple
+        self.gridbackg = True
+        self.linebackg = False
+
+        self.init_UI()
+
+    def init_UI(self):
+        self.setViewportUpdateMode(QGraphicsView.FullViewportUpdate)
+        # self.setCacheMode(QGraphicsView.CacheBackground)
+        self.standardCursor = QCursor(Qt.CrossCursor)
+        self.setCursor(self.standardCursor)  # set cursor to standard arrow
+        self.setRenderHint(QPainter.Antialiasing)
+        self.setRenderHint(QPainter.TextAntialiasing)
+        self.setMouseTracking(True)
+
+    def wheelEvent(self, mouse_event):
+        factor = 1.1
+        if mouse_event.angleDelta().y() < 0:
+            factor = 0.9
+        view_pos = QPoint(int(mouse_event.globalPosition().x()),
+                          int(mouse_event.globalPosition().y()))
+        scene_pos = self.mapToScene(view_pos)
+        self.centerOn(scene_pos)
+        self.scale(factor, factor)
+        delta = self.mapToScene(view_pos) - self.mapToScene(
+            self.viewport().rect().center())
+        self.centerOn(scene_pos - delta)
+        super().wheelEvent(mouse_event)
+
+    def snapToBase(self, number, base):
+        '''
+        Restrict a number to the multiples of base
+        '''
+        return int(base * int(round(number / base)))
+
+    def snapToGrid(self, point: QPoint, gridTuple: tuple[int, int]):
+        """
+        snap point to grid. Divides and multiplies by grid size.
+        """
+        return QPoint(self.snapToBase(point.x(), gridTuple[0]),
+                      self.snapToBase(point.y(), gridTuple[1]))
+
+    def drawBackground(self, painter, rect):
+
+        rectCoord = rect.getRect()
+        if self.gridbackg:
+            painter.fillRect(rect, QColor("black"))
+            painter.setPen(QColor("gray"))
+            grid_x_start = math.ceil(rectCoord[0] / self.gridTuple[0]) * \
+                           self.gridTuple[0]
+            grid_y_start = math.ceil(rectCoord[1] / self.gridTuple[1]) * \
+                           self.gridTuple[1]
+            num_x_points = math.floor(rectCoord[2] / self.gridTuple[0])
+            num_y_points = math.floor(rectCoord[3] / self.gridTuple[1])
+            for i in range(int(num_x_points)):  # rect width
+                for j in range(int(num_y_points)):  # rect length
+                    painter.drawPoint(grid_x_start + i * self.gridTuple[0],
+                                      grid_y_start + j * self.gridTuple[1], )
+        elif self.linebackg:
+            painter.fillRect(rect, QColor("black"))
+            painter.setPen(QColor("gray"))
+            left = int(rect.left()) - (int(rect.left()) % self.gridTuple[0])
+            top = int(rect.top()) - (int(rect.top()) % self.gridTuple[1])
+
+            x = left
+            while x < rect.right():
+                painter.drawLine(x, rect.top(), x, rect.bottom())
+                x += self.gridTuple[0]
+
+            # Draw the horizontal grid lines
+            y = top
+            while y < rect.bottom():
+                painter.drawLine(rect.left(), y, rect.right(), y)
+                y += self.gridTuple[1]
+        else:
+            super().drawBackground(painter, rect)
+
+    def keyPressEvent(self, key_event):
+        if key_event.key() == Qt.Key_F:
+            self.fitToView()
+        super().keyPressEvent(key_event)
+
+    def fitToView(self):
+        viewRect = self.scene.itemsBoundingRect().marginsAdded(
+            QMargins(40, 40, 40, 40))
+        self.fitInView(viewRect, Qt.AspectRatioMode.KeepAspectRatio)
+        self.show()
+
+    def printView(self, printer):
+        """
+        Print view using selected Printer.
+        """
+        painter = QPainter(printer)
+        if self.gridbackg:
+            self.gridbackg = False
+            self.revedaPrint(painter)
+            self.gridbackg = True
+        else:
+            self.linebackg = False
+            self.revedaPrint(painter)
+            self.linebackg = True
+
+    def revedaPrint(self, painter):
+        self.drawBackground(painter, self.viewport().geometry())
+        painter.drawText(self.viewport().geometry(), "Revolution EDA")
+        self.render(painter)
+        painter.end()
+
+
+
+class symbol_view(editor_view):
+    def __init__(self, scene, parent):
+        self.scene = scene
+        self.parent = parent
+        super().__init__(self.scene, self.parent)
+        self.visibleRect = None
+
+
+class schematic_view(editor_view):
+    def __init__(self, scene, parent):
+        self.scene = scene
+        self.parent = parent
+        super().__init__(self.scene, self.parent)
+        self.visibleRect = None  # initialize to an empty rectangle
+
+
+class libraryBrowser(QMainWindow):
+    def __init__(self, appMainW: QMainWindow) -> None:
+        super().__init__()
+        self.resize(300,600)
+        self.appMainW = appMainW
+        self.libraryDict = self.appMainW.libraryDict
+        self.cellViews = self.appMainW.cellViews
+        self.setWindowTitle("Library Browser")
+        self._createMenuBar()
+        self._createActions()
+        self._createToolBars()
+        self.logger = self.appMainW.logger
+        self.libFilePath = self.appMainW.libraryPathObj
+        self.libBrowserCont = libraryBrowserContainer(self)
+        self.setCentralWidget(self.libBrowserCont)
+        self.designView = self.libBrowserCont.designView
+        self.libraryModel = self.designView.libraryModel
+        self.editProcess = None
+
+    def _createMenuBar(self):
+        self.browserMenubar = self.menuBar()
+        self.browserMenubar.setNativeMenuBar(False)
+        self.libraryMenu = self.browserMenubar.addMenu("&Library")
+
+    def _createActions(self):
+        openLibIcon = QIcon(":/icons/database--plus.png")
+        self.openLibAction = QAction(openLibIcon, "Create/Open Lib...", self)
+        self.openLibAction.setToolTip("Create/Open Lib...")
+        self.libraryMenu.addAction(self.openLibAction)
+        self.openLibAction.triggered.connect(self.openLibClick)
+
+        libraryEditIcon = QIcon(":/icons/application-dialog.png")
+        self.libraryEditorAction = QAction(libraryEditIcon, "Library Editor",
+                                           self)
+        self.libraryMenu.addAction(self.libraryEditorAction)
+        self.libraryEditorAction.setToolTip("Open Library Editor...")
+        self.libraryEditorAction.triggered.connect(self.libraryEditorClick)
+
+        closeLibIcon = QIcon(":/icons/database-delete.png")
+        self.closeLibAction = QAction(closeLibIcon, "Close Lib...", self)
+        self.closeLibAction.setToolTip("Close Lib")
+        self.libraryMenu.addAction(self.closeLibAction)
+        self.closeLibAction.triggered.connect(self.closeLibClick)
+
+        self.libraryMenu.addSeparator()
+
+        newCellIcon = QIcon(":/icons/document--plus.png")
+        self.newCellAction = QAction(newCellIcon, "New Cell...", self)
+        self.newCellAction.setToolTip("Create New Cell")
+        self.libraryMenu.addAction(self.newCellAction)
+        self.newCellAction.triggered.connect(self.newCellClick)
+
+        deleteCellIcon = QIcon(":/icons/node-delete.png")
+        self.deleteCellAction = QAction(deleteCellIcon, "Delete Cell...", self)
+        self.deleteCellAction.setToolTip("Delete Cell")
+        self.libraryMenu.addAction(self.deleteCellAction)
+        self.deleteCellAction.triggered.connect(self.deleteCellClick)
+
+        self.libraryMenu.addSeparator()
+
+        newCellViewIcon = QIcon(":/icons/document--pencil.png")
+        self.newCellViewAction = QAction(newCellViewIcon,
+                                         "Create New CellView...", self)
+        self.newCellViewAction.setToolTip("Create New Cellview")
+        self.libraryMenu.addAction(self.newCellViewAction)
+        self.newCellViewAction.triggered.connect(self.newCellViewClick)
+
+        openCellViewIcon = QIcon(":/icons/document--pencil.png")
+        self.openCellViewAction = QAction(openCellViewIcon, "Open CellView...",
+                                          self)
+        self.openCellViewAction.setToolTip("Open CellView")
+        self.libraryMenu.addAction(self.openCellViewAction)
+        self.openCellViewAction.triggered.connect(self.openCellViewClick)
+
+        deleteCellViewIcon = QIcon(":/icons/node-delete.png")
+        self.deleteCellViewAction = QAction(deleteCellViewIcon,
+                                            "Delete CellView...", self)
+        self.deleteCellViewAction.setToolTip("Delete Cellview")
+        self.libraryMenu.addAction(self.deleteCellViewAction)
+        self.deleteCellViewAction.triggered.connect(self.deleteCellViewClick)
+
+    def _createToolBars(self):
+        # Create tools bar called "main toolbar"
+        toolbar = QToolBar("Main Toolbar", self)
+        # place toolbar at top
+        self.addToolBar(toolbar)
+        toolbar.addAction(self.openLibAction)
+        toolbar.addAction(self.closeLibAction)
+        toolbar.addSeparator()
+        toolbar.addAction(self.newCellAction)
+        toolbar.addAction(self.deleteCellAction)
+        toolbar.addSeparator()
+        toolbar.addAction(self.newCellViewAction)
+        toolbar.addAction(self.openCellViewAction)
+        toolbar.addAction(self.deleteCellViewAction)
+
+    def writeLibDefFile(self, libPathDict: dict,
+                        libFilePath: pathlib.Path) -> None:
+
+        libTempDict = dict(
+            zip(libPathDict.keys(), map(str, libPathDict.values())))
+        try:
+            with libFilePath.open(mode="w") as f:
+                json.dump({"libdefs": libTempDict}, f, indent=4)
+            self.logger.info(f'Wrote library definition file in {libFilePath}')
+        except IOError:
+            self.logger.error(f"Cannot save library definitions in {libFilePath}")
+
+    def openLibClick(self):
+        """
+        Open a directory and add a 'reveda.lib' file to designate it as a library.
+        """
+        home_dir = str(pathlib.Path.cwd())
+        libDialog = QFileDialog(self, "Create/Open Library", home_dir)
+        libDialog.setFileMode(QFileDialog.Directory)
+        # libDialog.Option(QFileDialog.ShowDirsOnly)
+        if libDialog.exec() == QDialog.Accepted:
+            libPathObj = pathlib.Path(libDialog.selectedFiles()[0])
+            self.libraryDict[libPathObj.stem] = libPathObj
+            # create an empty file to denote it is a design library.
+            # TODO: add some library information to this file.
+            libPathObj.joinpath("reveda.lib").touch(exist_ok=True)
+            # self.designView.reworkDesignLibrariesView()
+            self.libraryModel.populateLibrary(libPathObj)
+            self.writeLibDefFile(self.libraryDict, self.libFilePath)
+
+    def closeLibClick(self):
+        libCloseDialog = fd.closeLibDialog(self.libraryDict, self)
+        if libCloseDialog.exec() == QDialog.Accepted:
+            libName = libCloseDialog.libNamesCB.currentText()
+            libItem = libm.getLibItem(self.libraryModel, libName)
+            try:
+                self.libraryDict.pop(libName)
+            except KeyError:
+                self.logger.error(f"{libName} not found.")
+            finally:
+                self.libraryModel.rootItem.removeRow(
+                    libItem)  # self.designView.reworkDesignLibrariesView()
+
+    def libraryEditorClick(self, s):
+        """
+        Open library editor dialogue.
+        """
+        tempDict = deepcopy(self.libraryDict)
+        pathEditDlg = fd.libraryPathEditorDialog(self, tempDict)
+        libDefFilePathObj = pathlib.Path.cwd().joinpath('library.json')
+        self.libraryDict.clear()
+        if pathEditDlg.exec() == QDialog.Accepted:
+            model = pathEditDlg.pathsModel
+            for row in range(model.rowCount()):
+                if model.itemFromIndex(model.index(row, 1)).text().strip():
+                    self.libraryDict[model.itemFromIndex(
+                        model.index(row, 0)).text().strip()] = pathlib.Path(
+                        model.itemFromIndex(model.index(row, 1)).text().strip())
+        self.writeLibDefFile(self.libraryDict, libDefFilePathObj)
+        self.appMainW.libraryDict = self.libraryDict
+        self.designView.reworkDesignLibrariesView(self.appMainW.libraryDict)
+
+    def newCellClick(self, s):
+        dlg = fd.createCellDialog(self, self.libraryModel)
+        if dlg.exec() == QDialog.Accepted:
+            libName = dlg.libNamesCB.currentText()
+            cellName = dlg.cellCB.currentText()
+            self.createNewCell(self, self.libraryModel, cellName, libName)
+
+    def createNewCell(self, parent, libraryModel, cellName, libName):
+        libItem = libm.getLibItem(self.libraryModel, libName)
+        if cellName.strip() == "":
+            self.logger.error("Please enter a cell name.")
+        else:
+            scb.createCell(parent, libraryModel, libItem, cellName)
+
+    def deleteCellClick(self, s):
+        dlg = fd.deleteCellDialog(self, self.libraryModel)
+        if dlg.exec() == QDialog.Accepted:
+            libItem = libm.getLibItem(self.libraryModel,
+                                      dlg.libNamesCB.currentText())
+            if dlg.cellCB.currentText().strip() == "":
+                self.logger.error("Please enter a cell name.")
+            else:
+                # cellItemsLib = {libItem.child(i).cellName: libItem.child(i) for i in
+                #                 range(libItem.rowCount())}
+                # cellItem = cellItemsLib.get(dlg.cellCB.currentText())
+                cellItem = libm.getCellItem(libItem, dlg.cellCB.currentText())
+                # remove the directory
+                shutil.rmtree(cellItem.data(Qt.UserRole + 2))
+                cellItem.parent().removeRow(cellItem.row())
+
+    def newCellViewClick(self, s):
+        dlg = fd.newCellViewDialog(self, self.libraryModel)
+        dlg.viewType.addItems(self.cellViews)
+        if dlg.exec() == QDialog.Accepted:
+            # cellPath = dlg.selectedLibPath.joinpath(dlg.cellCB.currentText())
+            libItem = libm.getLibItem(self.libraryModel,
+                                      dlg.libNamesCB.currentText())
+            cellItem = libm.getCellItem(libItem, dlg.cellCB.currentText())
+            viewItem = scb.createCellView(self.appMainW,
+                                          dlg.viewName.text().strip(),
+                                          cellItem)
+            self.createNewCellView(libItem, cellItem, viewItem)
+
+    def createNewCellView(self, libItem, cellItem, viewItem):
+        viewTuple = ddef.viewTuple(libItem.libraryName, cellItem.cellName,
+                                   viewItem.viewName)
+        match viewItem.viewType:
+            case "config":
+                schViewsList = [cellItem.child(row).viewName for row in
+                                range(cellItem.rowCount()) if
+                                cellItem.child(row).viewType == "schematic"]
+
+                dlg = fd.createConfigViewDialogue(self.appMainW)
+                dlg.libraryNameEdit.setText(libItem.libraryName)
+                dlg.cellNameEdit.setText(cellItem.cellName)
+                dlg.viewNameCB.addItems(schViewsList)
+                dlg.switchViews.setText(", ".join(self.appMainW.switchViewList))
+                dlg.stopViews.setText(", ".join(self.appMainW.stopViewList))
+                # dlg.switchViews.setText(self.)
+                if dlg.exec() == QDialog.Accepted:
+                    selectedSchName = dlg.viewNameCB.currentText()
+                    selectedSchItem = libm.getViewItem(cellItem, selectedSchName)
+                    schematicWindow = schematicEditor(selectedSchItem,
+                                                      self.libraryDict,
+                                                      self.libBrowserCont.designView, )
+                    schematicWindow.loadSchematic()
+                    switchViewList = [viewName.strip() for viewName in
+                                      dlg.switchViews.text().split(",")]
+                    stopViewList = [viewName.strip() for viewName in
+                                    dlg.stopViews.text().split(",")]
+                    schematicWindow.switchViewList = switchViewList
+                    schematicWindow.stopViewList = stopViewList
+                    schematicWindow.configDict = dict()  # clear config dictionary
+
+                    # clear netlisted cells list
+                    newConfigDict = dict()  # create an empty newconfig dict
+                    schematicWindow.createConfigView(viewItem,
+                                                     schematicWindow.configDict,
+                                                     newConfigDict,
+                                                     schematicWindow.processedCells)
+                    configFilePathObj = viewItem.data(Qt.UserRole + 2)
+                    items = list()
+                    items.insert(0, {"cellView": "config"})
+                    items.insert(1, {"reference": selectedSchName})
+                    items.insert(2, schematicWindow.configDict)
+                    with configFilePathObj.open(mode="w+") as configFile:
+                        json.dump(items, configFile, indent=4)
+
+                    configWindow = self.openConfigEditWindow(
+                        schematicWindow.configDict,
+                        selectedSchItem, viewItem)
+                    self.appMainW.openViews[viewTuple] = configWindow
+            case "schematic":
+                # scb.createCellView(self.appMainW, viewItem.viewName, cellItem)
+                schematicWindow = schematicEditor(viewItem, self.libraryDict,
+                                                  self.libBrowserCont.designView)
+                self.appMainW.openViews[viewTuple] = schematicWindow
+                schematicWindow.loadSchematic()
+                schematicWindow.show()
+            case "symbol":
+                # scb.createCellView(self.appMainW, viewItem.viewName, cellItem)
+                symbolWindow = symbolEditor(viewItem, self.libraryDict,
+                                            self.libBrowserCont.designView)
+                self.appMainW.openViews[viewTuple] = symbolWindow
+                symbolWindow.loadSymbol()
+                symbolWindow.show()
+            case "veriloga":
+                scb.createCellView(self.appMainW, viewItem.viewName, cellItem)
+                if self.editProcess is None:
+                    self.editProcess = QProcess()
+                    self.editProcess.finished.connect(self.editProcessFinished)
+                    self.editProcess.start(str(self.appMainW.textEditorPath), [])
+
+    def openConfigEditWindow(self, configDict, schViewItem, viewItem):
+        schematicName = schViewItem.viewName
+        libItem = schViewItem.parent().parent()
+        configWindow = configViewEdit(self.appMainW, schViewItem, configDict,
+                                      viewItem)
+        configWindow.centralWidget.libraryNameEdit.setText(libItem.libraryName)
+        cellItem = viewItem.parent()
+        configWindow.centralWidget.cellNameEdit.setText(cellItem.cellName)
+        schViewsList = [cellItem.child(row).viewName for row in
+                        range(cellItem.rowCount())
+                        if cellItem.child(row).viewType == "schematic"]
+        configWindow.centralWidget.viewNameCB.addItems(schViewsList)
+        configWindow.centralWidget.viewNameCB.setCurrentText(schematicName)
+        configWindow.centralWidget.switchViewsEdit.setText(
+            ", ".join(self.appMainW.switchViewList))
+        configWindow.centralWidget.stopViewsEdit.setText(
+            ", ".join(self.appMainW.stopViewList))
+        configWindow.show()
+        return configWindow
+
+    def selectCellView(self, libModel) -> scb.viewItem:
+        dlg = fd.selectCellViewDialog(self, libModel)
+        if dlg.exec() == QDialog.Accepted:
+            libItem = libm.getLibItem(libModel, dlg.libNamesCB.currentText())
+            try:
+                cellItem = libm.getCellItem(libItem, dlg.cellCB.currentText())
+            except IndexError:
+                cellItem = libItem.child(0)
+            try:
+                viewItem = libm.getViewItem(cellItem, dlg.viewCB.currentText())
+                return viewItem
+            except IndexError:
+                viewItem = cellItem.child(0)
+                return None
+
+    def openCellViewClick(self):
+        viewItem = self.selectCellView(self.libraryModel)
+        cellItem = viewItem.parent()
+        libItem = cellItem.parent()
+        self.openCellView(viewItem, cellItem, libItem)
+
+    def openCellView(self, viewItem, cellItem, libItem):
+        viewName = viewItem.viewName
+        cellName = cellItem.cellName
+        libName = libItem.libraryName
+        openCellViewTuple = ddef.viewTuple(libName, cellName, viewName)
+        if openCellViewTuple in self.appMainW.openViews.keys():
+            self.appMainW.openViews[openCellViewTuple].raise_()
+        else:
+            if viewItem.viewType == "schematic":
+                schematicWindow = schematicEditor(viewItem, self.libraryDict,
+                                                  self.libBrowserCont.designView)
+                schematicWindow.loadSchematic()
+                schematicWindow.show()
+                self.appMainW.openViews[openCellViewTuple] = schematicWindow
+            elif viewItem.viewType == "symbol":
+                symbolWindow = symbolEditor(viewItem, self.libraryDict,
+                                            self.libBrowserCont.designView)
+                symbolWindow.loadSymbol()
+                symbolWindow.show()
+                self.appMainW.openViews[openCellViewTuple] = symbolWindow
+            elif viewItem.viewType == "veriloga":
+                with open(viewItem.viewPath) as tempFile:
+                    items = json.load(tempFile)
+                if items[1]["filePath"]:
+                    if self.editProcess is None:
+                        self.editProcess = QProcess()
+                        VerilogafilePathObj = viewItem.parent().data(
+                            Qt.UserRole + 2).joinpath(items[1]["filePath"])
+                        self.editProcess.finished.connect(
+                            self.editProcessFinished)
+                        self.editProcess.start(self.appMainW.textEditorPath,
+                                               [str(VerilogafilePathObj)])
+                else:
+                    self.logger.warning("File path not defined.")
+            elif viewItem.viewType == "config":
+                with open(viewItem.viewPath) as tempFile:
+                    items = json.load(tempFile)
+                viewName = items[0]["viewName"]
+                schematicName = items[1]["reference"]
+                schViewItem = libm.getViewItem(cellItem, schematicName)
+                configDict = items[2]
+                configWindow = self.openConfigEditWindow(configDict, schViewItem,
+                                                         viewItem)
+                self.appMainW.openViews[openCellViewTuple] = configWindow
+        return openCellViewTuple
+
+    def editProcessFinished(self):
+        self.appMainW.importVerilogaClick()
+        self.editProcess = None
+
+    def deleteCellViewClick(self, s):
+        viewItem = self.selectCellView(self.libraryModel)
+        try:
+            viewItem.data(Qt.UserRole + 2).unlink()  # delete the file.
+            viewItem.parent().removeRow(viewItem.row())
+        except OSError as e:
+            # print(f"Error:{e.strerror}")
+            self.logger.warning(f"Error:{e.strerror}")
+
+    def closeEvent(self, event: QCloseEvent) -> None:
+        event.ignore()  # ignore the default close event
+        self.hide()  # hide the window instead
+
+
+class libraryBrowserContainer(QWidget):
+    def __init__(self, parent) -> None:
+        super().__init__(parent)
+        self.parent = parent
+        self.initUI()
+
+    def initUI(self):
+        self.layout = QVBoxLayout()
+        self.designView = designLibrariesView(self)
+        self.layout.addWidget(self.designView)
+        self.setLayout(self.layout)
+
+
+class designLibrariesView(QTreeView):
+    def __init__(self, parent):
+        super().__init__(parent=parent)  # QTreeView
+        self.parent = parent  # type: QWidget (libraryBrowserContainer)
+        self.setSelectionMode(QAbstractItemView.SingleSelection)
+        self.viewCounter = 0
+        self.libBrowsW = self.parent.parent
+        self.appMainW = self.libBrowsW.appMainW
+        self.libraryDict = self.appMainW.libraryDict  # type: dict
+        self.cellViews = self.appMainW.cellViews  # type: list
+        self.openViews = self.appMainW.openViews  # type: dict
+        self.logger = self.appMainW.logger
+        self.selectedItem = None
+        # library model is based on qstandarditemmodel
+        self.libraryModel = designLibrariesModel(self.libraryDict)
+        self.setSortingEnabled(True)
+        self.setUniformRowHeights(True)
+        self.expandAll()
+        self.setModel(self.libraryModel)
+
+    def removeLibrary(self):
+        button = QMessageBox.question(self, "Library Deletion",
+                                      "Are you sure to delete " "this library? This action cannot be undone.", )
+        if button == QMessageBox.Yes:
+            shutil.rmtree(self.selectedItem.data(Qt.UserRole + 2))
+            self.libraryModel.removeRow(self.selectedItem.row())
+
+    def renameLib(self):
+        oldLibraryName = self.selectedItem.libraryName
+        dlg = fd.renameLibDialog(self, oldLibraryName)
+        if dlg.exec() == QDialog.Accepted:
+            newLibraryName = dlg.newLibraryName.text().strip()
+            libraryItem = libm.getLibItem(self.libraryModel, oldLibraryName)
+            libraryItem.setText(newLibraryName)
+            oldLibraryPath = libraryItem.data(Qt.UserRole + 2)
+            newLibraryPath = oldLibraryPath.parent.joinpath(newLibraryName)
+            oldLibraryPath.rename(newLibraryPath)
+
+    def createCell(self):
+        dlg = fd.createCellDialog(self, self.libraryModel)
+        assert isinstance(self.selectedItem, scb.libraryItem)
+        dlg.libNamesCB.setCurrentText(self.selectedItem.libraryName)
+        if dlg.exec() == QDialog.Accepted:
+            cellName = dlg.cellCB.currentText()
+            if cellName.strip() != '':
+                scb.createCell(self, self.libraryModel, self.selectedItem,
+                               cellName)
+            else:
+                self.logger.error("Please enter a cell name.")
+
+    def copyCell(self):
+        dlg = fd.copyCellDialog(self, self.libraryModel, self.selectedItem)
+
+        if dlg.exec() == QDialog.Accepted:
+            scb.copyCell(self, dlg.model, dlg.cellItem, dlg.copyName.text(),
+                         dlg.selectedLibPath)
+
+    def renameCell(self):
+        dlg = fd.renameCellDialog(self, self.selectedItem)
+        if dlg.exec() == QDialog.Accepted:
+            scb.renameCell(self, dlg.cellItem, dlg.nameEdit.text())
+
+    def deleteCell(self):
+        try:
+            shutil.rmtree(self.selectedItem.data(Qt.UserRole + 2))
+            self.selectedItem.parent().removeRow(self.selectedItem.row())
+        except OSError as e:
+            # print(f"Error:{e.strerror}")
+            self.logger.warning(f"Error:{e}")
+
+    def createCellView(self):
+        dlg = fd.createCellViewDialog(self, self.libraryModel, self.selectedItem)
+        if dlg.exec() == QDialog.Accepted:
+            viewItem = scb.createCellView(self.appMainW, dlg.nameEdit.text(),
+                                          self.selectedItem)
+            self.libBrowsW.createNewCellView(self.selectedItem.parent(),
+                                             self.selectedItem,
+                                             viewItem)
+
+    def openView(self):
+        viewItem = self.selectedItem
+        cellItem = viewItem.parent()
+        libItem = cellItem.parent()
+        self.libBrowsW.openCellView(viewItem, cellItem, libItem)
+
+    def copyView(self):
+        dlg = fd.copyViewDialog(self, self.libraryModel)
+        if dlg.exec() == QDialog.Accepted:
+            if self.selectedItem.data(Qt.UserRole + 1) == "view":
+                viewPath = self.selectedItem.data(Qt.UserRole + 2)
+                selectedLibItem = libm.getLibItem(self.libraryModel,
+                                                  dlg.libNamesCB.currentText())
+                cellName = dlg.cellCB.currentText()
+                libCellNames = [selectedLibItem.child(row).cellName for row in
+                                range(selectedLibItem.rowCount())]
+                if (
+                        cellName in libCellNames):  # check if there is the cell in the library
+                    cellItem = libm.getCellItem(selectedLibItem,
+                                                dlg.cellCB.currentText())
+                else:
+                    cellItem = scb.createCell(self.libBrowsW, self.libraryModel,
+                                              selectedLibItem,
+                                              dlg.cellCB.currentText(), )
+                cellViewNames = [cellItem.child(row).viewName for row in
+                                 range(cellItem.rowCount())]
+                newViewName = dlg.viewName.text()
+                if newViewName in cellViewNames:
+                    self.logger.warning(
+                        "View already exists. Delete cellview and try again.")
+                else:
+                    newViewPath = cellItem.data(Qt.UserRole + 2).joinpath(
+                        f"{newViewName}.json")
+                    shutil.copy(viewPath, newViewPath)
+                    cellItem.appendRow(scb.viewItem(newViewPath))
+
+    def renameView(self):
+        oldViewName = self.selectedItem.viewName
+        dlg = fd.renameViewDialog(self.libBrowsW, oldViewName)
+        if dlg.exec() == QDialog.Accepted:
+            newName = dlg.newViewNameEdit.text()
+            try:
+                viewPathObj = self.selectedItem.data(Qt.UserRole + 2)
+                newPathObj = self.selectedItem.data(Qt.UserRole + 2).rename(
+                    viewPathObj.parent.joinpath(f"{newName}.json"))
+                self.selectedItem.parent().appendRow(scb.viewItem(newPathObj))
+                self.selectedItem.parent().removeRow(self.selectedItem.row())
+            except FileExistsError:
+                self.logger.error("Cellview exists.")
+
+    def deleteView(self):
+        try:
+            self.selectedItem.data(Qt.UserRole + 2).unlink()
+            itemRow = self.selectedItem.row()
+            parent = self.selectedItem.parent()
+            parent.removeRow(itemRow)
+        except OSError as e:
+            # print(f"Error:{e.strerror}")
+            self.logger.warning(f"Error:{e.strerror}")
+
+    def reworkDesignLibrariesView(self,libraryDict:dict):
+        """
+        Recreate library model from libraryDict.
+        """
+        self.libraryModel = designLibrariesModel(libraryDict)
+        self.setModel(self.libraryModel)
+        self.libBrowsW.libraryModel = self.libraryModel
+
+    # context menu
+    def contextMenuEvent(self, event):
+        menu = QMenu(self)
+        try:
+            index = self.selectedIndexes()[0]
+        except IndexError:
+            pass
+        try:
+            self.selectedItem = self.libraryModel.itemFromIndex(index)
+            if self.selectedItem.data(Qt.UserRole + 1) == "library":
+                menu.addAction("Rename Library", self.renameLib)
+                menu.addAction("Remove Library", self.removeLibrary)
+                menu.addAction("Create Cell", self.createCell)
+            elif self.selectedItem.data(Qt.UserRole + 1) == "cell":
+                menu.addAction(
+                    QAction("Create CellView...", self,
+                            triggered=self.createCellView))
+                menu.addAction(
+                    QAction("Copy Cell...", self, triggered=self.copyCell))
+                menu.addAction(
+                    QAction("Rename Cell...", self, triggered=self.renameCell))
+                menu.addAction(
+                    QAction("Delete Cell...", self, triggered=self.deleteCell))
+            elif self.selectedItem.data(Qt.UserRole + 1) == "view":
+                menu.addAction(
+                    QAction("Open View", self, triggered=self.openView))
+                menu.addAction(
+                    QAction("Copy View...", self, triggered=self.copyView))
+                menu.addAction(
+                    QAction("Rename View...", self, triggered=self.renameView))
+                menu.addAction(
+                    QAction("Delete View...", self, triggered=self.deleteView))
+            menu.exec(event.globalPos())
+        except UnboundLocalError:
+            pass
+
+
+class designLibrariesModel(QStandardItemModel):
+    def __init__(self, libraryDict):
+        self.libraryDict = libraryDict
+        super().__init__()
+        self.rootItem = self.invisibleRootItem()
+        self.setHorizontalHeaderLabels(["Libraries"])
+        self.initModel()
+
+    def initModel(self):
+        for designPath in self.libraryDict.values():
+            self.populateLibrary(designPath)
+
+    def populateLibrary(self, designPath):  # designPath: Path
+        """
+        Populate library view.
+        """
+        if designPath.joinpath("reveda.lib").exists():
+            libraryItem = self.addLibraryToModel(designPath)
+            cellList = [cell.name for cell in designPath.iterdir() if
+                        cell.is_dir()]
+            for cell in cellList:  # type: str
+                cellItem = self.addCellToModel(designPath.joinpath(cell),
+                                               libraryItem)
+                viewList = [view.name for view in
+                            designPath.joinpath(cell).iterdir() if
+                            view.suffix == ".json"]
+                for view in viewList:
+                    self.addViewToModel(designPath.joinpath(cell, view), cellItem)
+
+    def addLibraryToModel(self, designPath):
+        libraryEntry = scb.libraryItem(designPath)
+        self.rootItem.appendRow(libraryEntry)
+        return libraryEntry
+
+    def addCellToModel(self, cellPath, parentItem):
+        cellEntry = scb.cellItem(cellPath)
+        parentItem.appendRow(cellEntry)
+        return cellEntry
+
+    def addViewToModel(self, viewPath, parentItem):
+        viewEntry = scb.viewItem(viewPath)
+        parentItem.appendRow(viewEntry)
+
+
+class libraryPathsModel(QStandardItemModel):
+    def __init__(self, libraryDict):
+        super().__init__()
+        self.libraryDict = libraryDict
+        self.setHorizontalHeaderLabels(['Library Name', 'Library Path'])
+        for key, value in self.libraryDict.items():
+            libName = QStandardItem(key)
+            libPath = QStandardItem(str(value))
+            self.appendRow(libName, libPath)
+        self.appendRow(QStandardItem('Click here...'), QStandardItem(''))
+
+
+class libraryPathsTableView(QTableView):
+    def __init__(self, model):
+        self.model = model
+        self.setModel(self.model)
+        self.setShowGrid(True)
+        self.setContextMenuPolicy(Qt.CustomContextMenu)
+
+    def contextMenuEvent(self, event) -> None:
+        self.menu = QMenu(self)
+        removePathAction = QAction('Remove Library Path...', self.menu)
+        removePathAction.triggered.connect(lambda: self.removeLibraryPath(event))
+        self.menu.addAction(removePathAction)
+        self.menu.popup(QCursor.pos())
+
+    def removeLibraryPath(self, event):
+        print('remove library path')
+
+
+class symbolViewsModel(designLibrariesModel):
+    def __init__(self, libraryDict):
+        super().__init__(libraryDict)
+
+    def populateLibrary(self, designPath):  # designPath: Path
+        """
+        Populate library view.
+        """
+        if designPath.joinpath("reveda.lib").exists():
+            libraryItem = self.addLibraryToModel(designPath)
+            cellList = [cell.name for cell in designPath.iterdir() if
+                        cell.is_dir()]
+            for cell in cellList:  # type: str
+                cellItem = self.addCellToModel(designPath.joinpath(cell),
+                                               libraryItem)
+                viewList = [view.name for view in
+                            designPath.joinpath(cell).iterdir() if
+                            view.suffix == ".json" and "symbol" in view.name]
+                for view in viewList:
+                    self.addViewToModel(designPath.joinpath(cell, view), cellItem)
+
+
+class xyceNetlist:
+    def __init__(self, schematic: schematicEditor, filePathObj: pathlib.Path,
+                 use_config: bool = False):
+        self.filePathObj = filePathObj
+        self.schematic = schematic
+        self._use_config = use_config
+        self._scene = self.schematic.centralW.scene
+        self.libraryDict = self.schematic.libraryDict
+        self.libraryView = self.schematic.libraryView
+        self._configDict = None
+        self.libItem = libm.getLibItem(self.schematic.libraryView.libraryModel,
+                                       self.schematic.libName, )
+        self.cellItem = libm.getCellItem(self.libItem, self.schematic.cellName)
+
+        self.switchViewList = schematic.switchViewList
+        self.stopViewList = schematic.stopViewList
+        self.netlistedViewsSet = set()  # keeps track of netlisted views.
+
+    def writeNetlist(self):
+        with self.filePathObj.open(mode="w") as cirFile:
+            cirFile.write(
+                '*'.join(['\n', 80 * "*", "\n", "* Revolution EDA CDL Netlist\n",
+                          f"* Library: {self.schematic.libName}\n",
+                          f"* Top Cell Name: {self.schematic.cellName}\n",
+                          f"* View Name: {self.schematic.viewName}\n",
+                          f"* Date: {datetime.datetime.now()}\n", 80 * "*", "\n",
+                          ".GLOBAL gnd!\n\n"]))
+
+            # now go down the rabbit hole to track all circuit elements.
+            self.recursiveNetlisting(self.schematic, cirFile)
+
+            cirFile.write(".END\n")
+
+    @property
+    def configDict(self):
+        return self._configDict
+
+    @configDict.setter
+    def configDict(self, value: dict):
+        assert isinstance(value, dict)
+        self._configDict = value
+
+    def recursiveNetlisting(self, schematic: schematicEditor, cirFile):
+        """
+        Recursively traverse all sub-circuits and netlist them.
+        """
+        try:
+            schematicScene = schematic.centralW.scene
+            schematicScene.groupAllNets()  # name all nets in the
+            # schematic
+            sceneSymbolSet = schematicScene.findSceneSymbolSet()
+            schematicScene.generatePinNetMap(sceneSymbolSet)
+            for item in sceneSymbolSet:
+                if item.attr.get("XyceNetlistLine") and item.attr.get(
+                        "XyceNetlistPass") != '1':
+                    self.netlistedViewsSet.add(ddef.viewTuple(item.libraryName,
+                                                              item.cellName,
+                                                              item.viewName))
+                    libItem = libm.getLibItem(schematic.libraryView.libraryModel,
+                                              item.libraryName)
+                    cellItem = libm.getCellItem(libItem, item.cellName)
+                    viewItems = [cellItem.child(row) for row in
+                                 range(cellItem.rowCount())]
+                    viewNames = [view.viewName for view in viewItems]
+
+                    viewDict = dict(zip(viewNames, viewItems))
+                    if self._use_config:
+                        netlistableViews = [self.configDict.get(item.cellName)[1]]
+                    else:
+                        netlistableViews = [viewItemName for viewItemName in
+                                            self.switchViewList if
+                                            viewItemName in viewNames]
+                    # now create the netlist line for that item.
+
+                    self.createItemLine(cirFile, item, netlistableViews, viewDict)
+                elif not item.attr.get("XyceNetlistPass", False):
+                    cirFile.write(f'*{item.instanceName} has no '
+                                  f'XyceNetlistLine attribute\n')
+            # print(f'netlisted views: {self.netlistedViewsSet}')
+        except Exception as e:
+            self.schematic.logger.error(e)
+
+    def createItemLine(self, cirFile, item, netlistableViews: list,
+                       viewDict: dict):
+        for viewName in netlistableViews:
+            if viewName in viewDict.keys():
+                viewTuple = ddef.viewTuple(item.libraryName, item.cellName,
+                                           viewName)
+                # print(viewTuple)
+                if viewDict[viewName].viewType == "schematic":
+                    cirFile.write(self.createXyceSymbolLine(item))
+
+                    schematicObj = schematicEditor(viewDict[viewName],
+                                                   self.libraryDict,
+                                                   self.libraryView, )
+
+                    schematicObj.loadSchematic()
+                    if viewTuple not in self.netlistedViewsSet:
+                        self.netlistedViewsSet.add(viewTuple)
+                        # print(f'{schematicObj.cellName} {schematicObj.viewName}')
+                        pinList = " ".join(item.pinNetMap.keys())
+                        cirFile.write(
+                            f".SUBCKT {schematicObj.cellName} {pinList}\n")
+                        self.recursiveNetlisting(schematicObj, cirFile)
+                        cirFile.write(".ENDS\n")
+                elif viewDict[viewName].viewType == "veriloga":
+                    with viewDict[viewName].data(Qt.UserRole + 2).open(
+                            mode="r") as vaview:
+                        items = json.load(vaview)
+                    netlistLine = items[3]['netlistLine']
+                    netlistLine = netlistLine.replace("[@instName]",
+                                                      f"{item.instanceName}")
+                    # TODO: fix veriloga netlisting
+                    # for pinName, netName in item.pinNetMap.items():
+                    #     netlistLine = netlistLine.replace(f"[|{pinName}:%]", f"{netName}")
+                    pinList = " ".join(item.pinNetMap.values())
+                    netlistLine = netlistLine.replace("[@pinList]", pinList)
+                    for labelItem in item.labels.values():
+                        if labelItem.labelDefinition in netlistLine:
+                            netlistLine = netlistLine.replace(
+                                labelItem.labelDefinition,
+                                labelItem.labelText)
+                    cirFile.write(f"{netlistLine}\n")
+                    self.netlistedViewsSet.add(viewTuple)
+                elif viewDict[viewName].viewType == "symbol":
+                    cirFile.write(f"{self.createXyceSymbolLine(item)}")
+                    self.netlistedViewsSet.add(ddef.viewTuple(
+                        item.libraryName, item.cellName, item.viewName))
+                break
+
+    def createXyceSymbolLine(self, item):
+        """
+        Create a netlist line from a nlp device format line.
+        """
+        try:
+            xyceNetlistFormatLine = item.attr["XyceNetlistLine"].strip()
+            for labelItem in item.labels.values():
+                if labelItem.labelDefinition in xyceNetlistFormatLine:
+                    xyceNetlistFormatLine = xyceNetlistFormatLine.replace(
+                        labelItem.labelDefinition, labelItem.labelText)
+
+            for attrb, value in item.attr.items():
+                if f'[%{attrb}]' in xyceNetlistFormatLine:
+                    xyceNetlistFormatLine = xyceNetlistFormatLine.replace(
+                        f'[%{attrb}]', value)
+            pinList = " ".join(item.pinNetMap.values())
+            xyceNetlistFormatLine = xyceNetlistFormatLine.replace('[@pinList]', pinList)+'\n'
+            return xyceNetlistFormatLine
+        except Exception as e:
+            self._scene.logger.error(e)
+            self._scene.logger.error(f"Netlist line is not defined for"
+                                     f" {item.instanceName}")
+            # if there is no NLPDeviceFormat line, create a warning line
+            return f"*Netlist line is not defined for symbol of {item.instanceName}\n"
+
+
+class configViewEdit(QMainWindow):
+    def __init__(self, appmainW, schViewItem, configDict, viewItem):
+        super().__init__(parent=appmainW)
+        self.appmainW = appmainW  # app mainwindow
+        self.schViewItem = schViewItem
+        self.configDict = configDict
+        self.viewItem = viewItem
+        self.setWindowTitle('Edit Config View')
+        self.setMinimumSize(500, 600)
+        self._createMenuBar()
+        self._createActions()
+        self._addActions()
+        self._createTriggers()
+        self.centralWidget = configViewEditContainer(self)
+        self.setCentralWidget(self.centralWidget)
+
+    def _createMenuBar(self):
+        self.mainMenu = self.menuBar()
+        self.fileMenu = self.mainMenu.addMenu("&File")
+        self.editMenu = self.mainMenu.addMenu("&Edit")
+        self.status_bar = self.statusBar()
+        self.status_bar.showMessage('Ready')
+
+    def _createActions(self):
+        updateIcon = QIcon(":/icons/arrow-circle.png")
+        self.updateAction = QAction(updateIcon, "Update", self)
+        saveIcon = QIcon(":/icons/database--plus.png")
+        self.saveAction = QAction(saveIcon, "Save", self)
+
+    def _addActions(self):
+        self.fileMenu.addAction(self.updateAction)
+        self.fileMenu.addAction(self.saveAction)
+
+    def _createTriggers(self):
+        self.updateAction.triggered.connect(self.updateClick)
+        self.saveAction.triggered.connect(self.saveClick)
+
+    def updateClick(self):
+        self.centralWidget.configViewTable.updateModel()
+        self.configDict = dict()
+        newConfigDict = dict()
+        model = self.centralWidget.confModel
+        for i in range(model.rowCount()):
+            viewList = [item.strip() for item in
+                        model.itemFromIndex(model.index(i, 3)).text().split(',')]
+            self.configDict[model.item(i, 1).text()] = [model.item(i, 0).text(),
+                                                        model.item(i, 2).text(),
+                                                        viewList]
+        if self.appmainW.libraryBrowser is None:
+            self.appmainW.createLibraryBrowser()
+        topSchematicWindow = schematicEditor(self.schViewItem,
+                                             self.appmainW.libraryDict,
+                                             self.appmainW.libraryBrowser.libBrowserCont.designView)
+        topSchematicWindow.loadSchematic()
+        topSchematicWindow.createConfigView(self.viewItem, self.configDict,
+                                            newConfigDict,
+                                            topSchematicWindow.processedCells)
+        self.configDict = newConfigDict
+
+        self.centralWidget.confModel = configModel(self.configDict)
+        # self.centralWidget.configDictGroup.setVisible(False)
+        self.centralWidget.configDictLayout.removeWidget(
+            self.centralWidget.configViewTable)
+        self.centralWidget.configViewTable = configTable(
+            self.centralWidget.confModel)
+        self.centralWidget.configDictLayout.addWidget(
+            self.centralWidget.configViewTable)  # self.centralWidget.configDictGroup.setVisible(True)
+
+    def saveClick(self):
+        configFilePathObj = self.viewItem.data(Qt.UserRole + 2)
+        items = list()
+        items.insert(0, {"viewName": "config"})
+        items.insert(1, {"reference": self.schViewItem.viewName})
+        items.insert(2, self.configDict)
+        with configFilePathObj.open(mode="w+") as configFile:
+            json.dump(items, configFile, indent=4)
+
+
+class configViewEditContainer(QWidget):
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.parent = parent
+        self.mainLayout = QVBoxLayout()
+        topCellGroup = QGroupBox('Top Cell')
+        topCellLayout = QFormLayout()
+        self.libraryNameEdit = edf.longLineEdit()
+        topCellLayout.addRow(edf.boldLabel('Library:'), self.libraryNameEdit)
+        self.cellNameEdit = edf.longLineEdit()
+        topCellLayout.addRow(edf.boldLabel('Cell:'), self.cellNameEdit)
+        self.viewNameCB = QComboBox()
+        topCellLayout.addRow(edf.boldLabel('View:'), self.viewNameCB)
+        topCellGroup.setLayout(topCellLayout)
+        self.mainLayout.addWidget(topCellGroup)
+        viewGroup = QGroupBox('Switch/Stop Views')
+        viewGroupLayout = QFormLayout()
+        viewGroup.setLayout(viewGroupLayout)
+        self.switchViewsEdit = edf.longLineEdit()
+        viewGroupLayout.addRow(edf.boldLabel('View List:'), self.switchViewsEdit)
+        self.stopViewsEdit = edf.longLineEdit()
+        viewGroupLayout.addRow(edf.boldLabel('Stop List:'), self.stopViewsEdit)
+        self.mainLayout.addWidget(viewGroup)
+        self.configDictGroup = QGroupBox('Cell View Configuration')
+        self.confModel = configModel(self.parent.configDict)
+        self.configDictLayout = QVBoxLayout()
+        self.configViewTable = configTable(self.confModel)
+        self.configDictLayout.addWidget(self.configViewTable)
+        self.configDictGroup.setLayout(self.configDictLayout)
+        self.mainLayout.addWidget(self.configDictGroup)
+        self.setLayout(self.mainLayout)
+
+
+class configModel(QStandardItemModel):
+    def __init__(self, configDict: dict):
+        row = len(configDict.keys())
+        column = 4
+        super().__init__(row, column)
+        self.setHorizontalHeaderLabels(
+            ['Library', 'Cell Name', 'View Found', 'View To '
+                                                   'Use'])
+        for i, (k, v) in enumerate(configDict.items()):
+            item = QStandardItem(v[0])
+            self.setItem(i, 0, item)
+            item = QStandardItem(k)
+            self.setItem(i, 1, item)
+            item = QStandardItem(v[1])
+            self.setItem(i, 2, item)
+            item = QStandardItem(', '.join(v[2]))
+            self.setItem(i, 3, item)
+
+
+class configTable(QTableView):
+    def __init__(self, model: configModel):
+        super().__init__()
+        self.model = model
+        self.setModel(self.model)
+        self.combos = list()
+        self.horizontalHeader().setStretchLastSection(True)
+        self.setSelectionMode(QTableView.SingleSelection)
+        self.setEditTriggers(QTableView.NoEditTriggers)
+        for row in range(self.model.rowCount()):
+            self.combos.append(QComboBox())
+            items = [item.strip() for item in
+                     self.model.itemFromIndex(
+                         self.model.index(row, 3)).text().split(',')]
+            self.combos[-1].addItems(items)
+            self.combos[-1].setCurrentText(
+                self.model.itemFromIndex(self.model.index(row, 2)).text())
+            self.setIndexWidget(self.model.index(row, 3), self.combos[-1])
+
+    def updateModel(self):
+        for row in range(self.model.rowCount()):
+            item = QStandardItem(self.combos[row].currentText())
+            self.model.setItem(row, 2, item)
+
+
+class startThread(QRunnable):
+    __slots__ = ('fn',)
+
+    def __init__(self, fn):
+        super().__init__()
+        self.fn = fn
+
+    @Slot()
+    def run(self) -> None:
+        try:
+            self.fn
+        except Exception as e:
+            print(e)
+
```

### Comparing `revolution-eda-0.4.1/gui/fileDialogues.py` & `revolution-eda-0.5.0/revedaEditor/gui/fileDialogues.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 #  #
 #   Software: Revolution EDA
 #   License: Mozilla Public License 2.0
 #   Licensor: Revolution Semiconductor (Registered in the Netherlands)
 
 import pathlib
 
+import revedaEditor.backend.libraryMethods as libm
+import revedaEditor.common.shape as shp
+import revedaEditor.gui.editFunctions as edf
 from PySide6.QtCore import (Qt, QDir)
-from PySide6.QtGui import (QStandardItemModel, QStandardItem, QCursor, QAction)
+from PySide6.QtGui import (QStandardItemModel, QStandardItem)
 from PySide6.QtWidgets import (QComboBox, QDialog, QDialogButtonBox, QFileDialog,
-                               QFormLayout, QHBoxLayout, QLabel, QLineEdit, QVBoxLayout,
-                               QPushButton, QGroupBox, QTableView, QMenu, )
-
-import backend.schBackEnd as scb
-import common.shape as shp
-import gui.editFunctions as edf
-import backend.libraryMethods as libm
+                               QFormLayout, QHBoxLayout, QLabel, QLineEdit,
+                               QVBoxLayout, QRadioButton, QButtonGroup,
+                               QPushButton, QGroupBox, QTableView, QMenu,
+                               QCheckBox)
 
 
 class createCellDialog(QDialog):
     def __init__(self, parent, model):
         super().__init__(parent=parent)
         self.parent = parent
         self.model = model
@@ -65,25 +65,14 @@
 
     def selectLibrary(self):
         libItem = libm.getLibItem(self.model, self.libNamesCB.currentText())
         cellList = [libItem.child(i).cellName for i in range(libItem.rowCount())]
         self.cellCB.clear()
         self.cellCB.addItems(cellList)
 
-    # @staticmethod
-    # def getLibItem(libraryModel: QStandardItemModel, libName: str) -> scb.libraryItem:
-    #     return libm.getLibItem(libraryModel, libName)
-    #
-    # @staticmethod
-    # def getCellItem(libItem: scb.libraryItem, cellNameInp: str) -> scb.cellItem:
-    #     return libm.getCellItem(libItem,cellNameInp)
-    #
-    # @staticmethod
-    # def getViewItem(cellItem: scb.cellItem, viewNameInp: str) -> scb.viewItem:
-    #     return libm.getViewItem(cellItem, viewNameInp)
 
 
 class deleteCellDialog(createCellDialog):
     def __init__(self, parent, model):
         super().__init__(parent, model)
         self.cellCB.setEditable(False)
         self.setWindowTitle('Delete Cell')
@@ -369,48 +358,51 @@
     def onDirButtonClicked(self):
         self.dirName = QFileDialog.getExistingDirectory()
         if self.dirName:
             self.netlistDirEdit.setText(self.dirName)
 
 
 class goDownHierDialogue(QDialog):
-    def __init__(self, symbolShape: shp.symbolShape, libraryDict: dict[str, pathlib.Path],
-                 *args):
-        self.symbolShape = symbolShape
-        self.libraryDict = libraryDict
-        super().__init__(*args)
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-
-        mainLayout = QVBoxLayout()
-        cellPropLayout = QFormLayout()
-        libraryNameEdit = edf.shortLineEdit()
-        libraryNameEdit.setText(self.symbolShape.libraryName)
-        libraryNameEdit.setReadOnly(True)
-        cellPropLayout.addRow(edf.boldLabel("Library Name:", self), libraryNameEdit)
-        cellNameEdit = edf.shortLineEdit()
-        cellNameEdit.setText(self.symbolShape.cellName)
-        cellNameEdit.setReadOnly(True)
-        cellPropLayout.addRow(edf.boldLabel("Cell Name:", self), cellNameEdit)
-        cellPath = pathlib.Path(
-            self.libraryDict.get(self.symbolShape.libraryName).joinpath(
-                self.symbolShape.cellName))
-        viewList = [str(view.stem) for view in cellPath.iterdir() if
-                    view.suffix == ".json"]
-        self.viewNameCB = QComboBox()
-        self.viewNameCB.addItems(viewList)
-        cellPropLayout.addRow(edf.boldLabel("Select View:", self), self.viewNameCB)
-        mainLayout.addLayout(cellPropLayout)
-        mainLayout.addStretch(2)
-        mainLayout.addWidget(self.buttonBox)
-        self.setLayout(mainLayout)
+    def __init__(self, parent,):
+        super().__init__(parent=parent)
+        self._parent = parent
+        self.setWindowTitle('Go Down Hierarchy')
+        self.setMinimumWidth(250)
+        self.buttonId = 1
+        _mainLayout = QVBoxLayout()
+        viewGroup = QGroupBox('Select a cellview')
+        viewGroupLayout = QVBoxLayout()
+        viewGroup.setLayout(viewGroupLayout)
+        self.viewListCB = QComboBox()
+        viewGroupLayout.addWidget(self.viewListCB)
+        _mainLayout.addWidget(viewGroup)
+        buttonGroupBox = QGroupBox('Open')
+        buttonGroupLayout = QHBoxLayout()
+        buttonGroupBox.setLayout(buttonGroupLayout)
+        self.openButton = QRadioButton('Edit')
+        self.openButton.setChecked(True)
+        self.readOnlyButton = QRadioButton('Read Only')
+        buttonGroupLayout.addWidget(self.openButton)
+        buttonGroupLayout.addWidget(self.readOnlyButton)
+        _mainLayout.addWidget(buttonGroupBox)
+        self.buttonGroup = QButtonGroup()
+        self.buttonGroup.addButton(self.openButton, id = 1)
+        self.buttonGroup.addButton(self.readOnlyButton, id = 2)
+        self.buttonGroup.buttonClicked.connect(self.onButtonClicked)
+        _mainLayout.addWidget(buttonGroupBox)
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        buttonBox = QDialogButtonBox(QBtn)
+        buttonBox.accepted.connect(self.accept)
+        buttonBox.rejected.connect(self.reject)
+        _mainLayout.addWidget(buttonBox)
+        self.setLayout(_mainLayout)
         self.show()
 
+    def onButtonClicked(self):
+        self.buttonId = self.buttonGroup.checkedId()
 
 class importVerilogaCellDialogue(QDialog):
     def __init__(self, model, parent):
         super().__init__(parent)
         self._parent = parent
         self.setWindowTitle('Import a Verilog-a File')
         self._model = model
@@ -436,14 +428,20 @@
         initialCellNames = [self._model.item(0).child(i).cellName for i in
                             range(self._model.item(0).rowCount())]
         self.cellNamesCB.addItems(initialCellNames)
         layout.addRow(edf.boldLabel('Cell:'), self.cellNamesCB)
         self.vaViewName = edf.longLineEdit()
         layout.addRow(edf.boldLabel('Verilog-A view:'), self.vaViewName)
         mainLayout.addLayout(layout)
+        symbolGroupBox = QGroupBox('Symbol Creation')
+        symbolGBLayout = QVBoxLayout()
+        self.symbolCheckBox = QCheckBox('Create a new symbol?')
+        symbolGBLayout.addWidget(self.symbolCheckBox)
+        symbolGroupBox.setLayout(symbolGBLayout)
+        mainLayout.addWidget(symbolGroupBox)
         mainLayout.addSpacing(20)
         QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
         self.buttonBox = QDialogButtonBox(QBtn)
         self.buttonBox.accepted.connect(self.accept)
         self.buttonBox.rejected.connect(self.reject)
         mainLayout.addWidget(self.buttonBox)
         self.setLayout(mainLayout)
@@ -496,17 +494,14 @@
         self.setLayout(self.mainLayout)
 
 
 class appProperties(QDialog):
     def __init__(self, parent):
         self.parent = parent
         super().__init__(parent)
-        self.initUI()
-
-    def initUI(self):
         self.setMinimumSize(550, 200)
         self.setWindowTitle('Revolution EDA Options')
         mainLayout = QVBoxLayout()
         filePathsGroup = QGroupBox('Paths')
         filePathsLayout = QVBoxLayout()
         fileDialogLayout = QHBoxLayout()
         fileDialogLayout.addWidget(edf.boldLabel('Text Editor Path:'), 2)
@@ -530,14 +525,20 @@
         switchViewsLayout = QFormLayout()
         self.switchViewsEdit = edf.longLineEdit()
         switchViewsLayout.addRow(edf.boldLabel('Switch Views:'), self.switchViewsEdit)
         self.stopViewsEdit = edf.longLineEdit()
         switchViewsLayout.addRow(edf.boldLabel('Stop Views:'), self.stopViewsEdit)
         switchViewsGroup.setLayout(switchViewsLayout)
         mainLayout.addWidget(switchViewsGroup)
+        saveGroupBox = QGroupBox('Save Options')
+        saveGBLayout = QVBoxLayout()
+        self.optionSaveBox = QCheckBox('Save options to configuration file?')
+        saveGBLayout.addWidget(self.optionSaveBox)
+        saveGroupBox.setLayout(saveGBLayout)
+        mainLayout.addWidget(saveGroupBox)
         mainLayout.addSpacing(20)
         QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
         self.buttonBox = QDialogButtonBox(QBtn)
         self.buttonBox.accepted.connect(self.accept)
         self.buttonBox.rejected.connect(self.reject)
         mainLayout.addWidget(self.buttonBox)
         self.setLayout(mainLayout)
```

### Comparing `revolution-eda-0.4.1/gui/propertyDialogues.py` & `revolution-eda-0.5.0/revedaEditor/gui/propertyDialogues.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,745 +1,784 @@
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-# properties dialogues for various symbol items
-
-import pathlib
-
-from PySide6.QtGui import (QFontDatabase, )
-from PySide6.QtWidgets import (QDialog, QVBoxLayout, QHBoxLayout, QFormLayout,
-                               QDialogButtonBox, QLineEdit, QLabel, QComboBox,
-                               QGroupBox, QRadioButton, QGridLayout, QTextEdit,
-                               QMenu)
-
-import common.net as net
-import common.shape as shp
-import gui.editFunctions as edf
-
-
-class rectPropertyDialog(QDialog):
-    '''
-    Property dialog for symbol rectangles.
-    '''
-    def __init__(self, parent, rectItem: shp.rectangle):
-        super().__init__(parent)
-        self.parent = parent
-        self.rectItem = rectItem
-        self.location = self.rectItem.scenePos().toTuple()
-        self.coords = self.rectItem.rect.getRect()
-
-        self.setWindowTitle("Rectangle Properties")
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.mainLayout = QVBoxLayout()
-        self.fLayout = QFormLayout()
-        self.fLayout.setContentsMargins(10, 10, 10, 10)
-        self.rectWidthLine = QLineEdit()
-        self.rectWidthLine.setText(str(self.coords[2]))
-        self.fLayout.addRow(QLabel("Width:"), self.rectWidthLine)
-        self.rectHeightLine = QLineEdit()
-        self.rectHeightLine.setText(str(self.coords[3]))
-        self.fLayout.addRow(QLabel("Height:"), self.rectHeightLine)
-        self.rectLeftLine = QLineEdit()
-        self.rectLeftLine.setText(
-            str(self.rectItem.start.toTuple()[0] + self.location[0]))
-        self.fLayout.addRow(QLabel("X Origin:"), self.rectLeftLine)
-        self.rectTopLine = QLineEdit()
-        self.rectTopLine.setText(
-            str(self.rectItem.start.toTuple()[1] + self.location[1]))
-        self.fLayout.addRow(QLabel("Y Origin:"), self.rectTopLine)
-        self.mainLayout.addLayout(self.fLayout)
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-        self.show()
-
-
-class circlePropertyDialog(QDialog):
-    def __init__(self, parent, circleItem: shp.circle):
-        super().__init__(parent)
-        self.parent = parent
-        self.circleItem = circleItem
-        self.location = self.circleItem.scenePos().toTuple()
-        self.centre = self.circleItem.mapToScene(
-            self.circleItem.centre).toTuple()
-        self.radius = self.circleItem.radius
-
-        self.setWindowTitle("Circle Properties")
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.mainLayout = QVBoxLayout()
-        self.fLayout = QFormLayout()
-        self.fLayout.setContentsMargins(10, 10, 10, 10)
-        self.centerXEdit = edf.shortLineEdit()
-        self.centerXEdit.setText(str(self.centre[0]))
-        self.fLayout.addRow(QLabel("center x-coord:"), self.centerXEdit)
-        self.centerYEdit = edf.shortLineEdit()
-        self.centerYEdit.setText(str(self.centre[1]))
-        self.fLayout.addRow(QLabel("center y-coord:"), self.centerYEdit)
-        self.radiusEdit = edf.shortLineEdit()
-        self.radiusEdit.setText(str(self.radius))
-        self.fLayout.addRow(QLabel("radius:"), self.radiusEdit)
-        self.mainLayout.addLayout(self.fLayout)
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-        self.show()
-
-class arcPropertyDialog(QDialog):
-    def __init__(self, parent, arcItem: shp.arc):
-        super().__init__(parent)
-        self.parent = parent
-        self.setWindowTitle("Arc Properties")
-        self.arcItem = arcItem
-        self.location = self.arcItem.scenePos().toTuple()
-        # self.arcType = self.arcItem.arcType
-        # self.arcTypeCombo = QComboBox()
-        # self.arcTypeCombo.addItems(shp.arc.arcTypes)
-        # self.arcTypeCombo.setCurrentText(self.arcType)
-
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.mainLayout = QVBoxLayout()
-        self.fLayout = QFormLayout()
-        self.fLayout.setContentsMargins(10, 10, 10, 10)
-        # self.mainLayout.addWidget(self.arcTypeCombo)
-        self.startXEdit = edf.shortLineEdit()
-        self.startXEdit.setText(
-            str(self.arcItem.start.toTuple()[0] + self.location[0]))
-        self.fLayout.addRow(QLabel("X Origin:"), self.startXEdit)
-        self.startYEdit = edf.shortLineEdit()
-        self.startYEdit.setText(
-            str(self.arcItem.start.toTuple()[1] + self.location[1]))
-        self.fLayout.addRow(QLabel("Y Origin:"), self.startYEdit)
-        self.widthEdit = edf.shortLineEdit()
-        self.widthEdit.setText(str(self.arcItem.width))
-        self.fLayout.addRow(QLabel("Width:"), self.widthEdit)
-        self.heightEdit = edf.shortLineEdit()
-        self.heightEdit.setText(str(self.arcItem.height))
-        self.fLayout.addRow(QLabel("Height:"), self.heightEdit)
-        self.mainLayout.addLayout(self.fLayout)
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-        self.show()
-
-class linePropertyDialog(QDialog):
-    def __init__(self, parent, lineItem: shp.line):
-        super().__init__(parent)
-        self.parent = parent
-        self.lineItem = lineItem
-        self.location = self.lineItem.scenePos().toTuple()
-
-        self.setWindowTitle("Line Properties")
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.mainLayout = QVBoxLayout()
-        self.fLayout = QFormLayout()
-        self.fLayout.setContentsMargins(10, 10, 10, 10)
-        self.startXLine = QLineEdit()
-        self.startXLine.setText(
-            str(self.lineItem.start.toTuple()[0] + self.location[0]))
-        self.fLayout.addRow(QLabel("Start (X):"), self.startXLine)
-        self.startYLine = QLineEdit()
-        self.startYLine.setText(
-            str(self.lineItem.start.toTuple()[1] + self.location[1]))
-        self.fLayout.addRow(QLabel("Start (Y):"), self.startYLine)
-        self.endXLine = QLineEdit()
-        self.endXLine.setText(
-            str(self.lineItem.end.toTuple()[0] + self.location[0]))
-        self.fLayout.addRow(QLabel("End (X):"), self.endXLine)
-        self.endYLine = QLineEdit()
-        self.endYLine.setText(
-            str(self.lineItem.end.toTuple()[1] + self.location[1]))
-        self.fLayout.addRow(QLabel("End (Y):"), self.endYLine)
-        self.mainLayout.addLayout(self.fLayout)
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-        self.show()
-
-
-class createPinDialog(QDialog):
-    def __init__(self, parent) -> None:
-        super().__init__(parent)
-        self.setWindowTitle("Create Pin")
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.mainLayout = QVBoxLayout()
-        self.fLayout = QFormLayout()
-        self.pinName = QLineEdit()
-        self.pinName.setPlaceholderText("Pin Name")
-        self.pinName.setToolTip("Enter pin name")
-        self.fLayout.addRow(QLabel("Pin Name"), self.pinName)
-        self.pinDir = QComboBox()
-        self.pinDir.addItems(shp.pin.pinDirs)
-        self.pinDir.setToolTip("Select pin direction")
-        self.fLayout.addRow(QLabel("Pin Direction"), self.pinDir)
-        self.pinType = QComboBox()
-        self.pinType.addItems(shp.pin.pinTypes)
-        self.pinType.setToolTip("Select pin type")
-        self.fLayout.addRow(QLabel("Pin Type"), self.pinType)
-        self.mainLayout.addLayout(self.fLayout)
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-        self.show()
-
-
-class pinPropertyDialog(createPinDialog):
-    def __init__(self, parent, pinItem: shp.pin):
-        super().__init__(parent)
-        self.parent = parent
-        self.pinItem = pinItem
-        self.location = self.pinItem.scenePos().toTuple()
-
-        self.setWindowTitle("Pin Properties")
-        self.pinName.setText(str(pinItem.pinName))
-        self.pinType.setCurrentText(pinItem.pinType)
-        self.pinDir.setCurrentText(pinItem.pinDir)
-        self.pinXLine = QLineEdit()
-        self.pinXLine.setText(str(self.pinItem.start.x() + self.location[0]))
-        self.pinXLine.setToolTip("X Coordinate")
-        self.fLayout.addRow(QLabel("X:"), self.pinXLine)
-        self.pinYLine = QLineEdit()
-        self.pinYLine.setText(str(self.pinItem.start.y() + self.location[1]))
-        self.pinYLine.setToolTip("Y Coordinate")
-        self.fLayout.addRow(QLabel("Y:"), self.pinYLine)
-
-
-class createSymbolLabelDialog(QDialog):
-    def __init__(self, parent) -> None:
-        super().__init__(parent)
-        self.setWindowTitle("Create Label")
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.mainLayout = QVBoxLayout()
-        self.fLayout = QFormLayout()
-        self.labelDefinition = QLineEdit()
-        self.labelDefinition.setPlaceholderText("Label Definition")
-        self.labelDefinition.setToolTip("Enter label Definition")
-        self.fLayout.addRow(QLabel("Label Definition"), self.labelDefinition)
-        self.labelHeightEdit = QLineEdit()
-        self.labelHeightEdit.setPlaceholderText("Label Height")
-        self.labelHeightEdit.setToolTip("Enter label Height")
-        self.fLayout.addRow(QLabel("Label Height"), self.labelHeightEdit)
-        self.labelAlignCombo = QComboBox()
-        self.labelAlignCombo.addItems(shp.label.labelAlignments)
-        self.fLayout.addRow(QLabel("Label Alignment"), self.labelAlignCombo)
-        self.labelOrientCombo = QComboBox()
-        self.labelOrientCombo.addItems(shp.label.labelOrients)
-        self.fLayout.addRow(QLabel("Label Orientation"), self.labelOrientCombo)
-        self.labelUseCombo = QComboBox()
-        self.labelUseCombo.addItems(shp.label.labelUses)
-        self.fLayout.addRow(QLabel("Label Use"), self.labelUseCombo)
-        self.labelVisiCombo = QComboBox()
-        self.labelVisiCombo.addItems(["Yes", "No"])
-        self.fLayout.addRow(QLabel("Label Visible"),self.labelVisiCombo)
-        self.mainLayout.addLayout(self.fLayout)
-        self.labelTypeGroup = QGroupBox("Label Type")
-        self.labelTypeLayout = QHBoxLayout()
-        self.normalType = QRadioButton(shp.label.labelTypes[0])
-        self.normalType.setChecked(True)
-        self.NLPType = QRadioButton(shp.label.labelTypes[1])
-        self.pyLType = QRadioButton(shp.label.labelTypes[2])
-        self.labelTypeLayout.addWidget(self.normalType)
-        self.labelTypeLayout.addWidget(self.NLPType)
-        self.labelTypeLayout.addWidget(self.pyLType)
-        self.labelTypeGroup.setLayout(self.labelTypeLayout)
-        self.mainLayout.addWidget(self.labelTypeGroup)
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-        self.show()
-
-
-class labelPropertyDialog(createSymbolLabelDialog):
-    def __init__(self, parent, labelItem: shp.label):
-        assert isinstance(labelItem, shp.label)
-        super().__init__(parent)
-        self.parent = parent
-        self.labelItem = labelItem
-        self.location = self.labelItem.scenePos().toTuple()
-
-        self.setWindowTitle("Label Properties")
-        self.labelDefinition.setText(str(labelItem.labelDefinition))
-        self.labelHeightEdit.setText(str(labelItem.labelHeight))
-        self.labelAlignCombo.setCurrentText(labelItem.labelAlign)
-        self.labelOrientCombo.setCurrentText(labelItem.labelOrient)
-        self.labelUseCombo.setCurrentText(labelItem.labelUse)
-        if labelItem.labelVisible:
-            self.labelVisiCombo.setCurrentText("Yes")
-        else:
-            self.labelVisiCombo.setCurrentText("No")
-        if self.labelItem.labelType == "Normal":
-            self.normalType.setChecked(True)
-        elif self.labelItem.labelType == "NLPLabel":
-            self.NLPType.setChecked(True)
-        elif self.labelItem.labelType == "PyLabel":
-            self.pyLType.setChecked(True)
-        self.labelXLine = QLineEdit()
-        self.labelXLine.setText(
-            str(self.labelItem.start.x() + self.location[0]))
-        self.labelXLine.setToolTip("X Coordinate")
-        self.fLayout.addRow(QLabel("X:"), self.labelXLine)
-        self.labelYLine = QLineEdit()
-        self.labelYLine.setText(
-            str(self.labelItem.start.y() + self.location[1]))
-        self.labelYLine.setToolTip("Y Coordinate")
-        self.fLayout.addRow(QLabel("Y:"), self.labelYLine)
-
-
-class symbolLabelsDialogue(QDialog):
-    """
-    Dialog for changing symbol labels and attributes. Symbol properties... menu item.
-    """
-
-    def __init__(self, parent, items: list, attributes: list):
-        super().__init__(parent)
-        self.parent = parent
-        self.items = items
-        self.attributes = attributes
-        self.setWindowTitle("Symbol Labels")
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.mainLayout = QVBoxLayout()
-        self.symbolPropsLayout = QGridLayout()
-        self.symbolLabelsLayout = QGridLayout()
-        self.symbolAttrsMethod()
-        # Symbol Labels Layout
-        self.symbolLabelsMethod()
-        labelsGroup = QGroupBox("Symbol Labels")
-        labelsGroup.setLayout(self.symbolLabelsLayout)
-        self.mainLayout.addWidget(labelsGroup)
-        self.mainLayout.addStretch(1)
-        # self.mainLayout.addLayout(self.symbolLabelsLayout)
-        propsGroup = QGroupBox("Symbol Attributes")
-        propsGroup.setLayout(self.symbolPropsLayout)
-        self.mainLayout.addWidget(propsGroup)
-        self.mainLayout.addStretch(1)
-        # self.mainLayout.addLayout(self.symbolPropsLayout)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-
-    def symbolAttrsMethod(self):
-        self.attributeNameList = []
-        # self.attributeTypeList = []
-        self.attributeDefList = []
-        # Symbol Properties
-        self.symbolPropsLayout.addWidget(QLabel("Attribute Name"), 0, 0)
-        # self.symbolPropsLayout.addWidget(QLabel("Type"), 0, 1)
-        self.symbolPropsLayout.addWidget(QLabel("Definition"), 0, 1)
-        i = 0
-        for item in self.attributes:
-            # print(f'item is :{item}')
-            self.attributeNameList.append(edf.longLineEdit())
-            self.attributeNameList[i].setText(item.name)
-            self.symbolPropsLayout.addWidget(self.attributeNameList[i], i + 1,
-                0)
-            # attrTypeCombo = QComboBox()
-            # attrTypeCombo.addItems(shp.label.labelTypes)
-            # self.attributeTypeList.append(attrTypeCombo)
-            # self.attributeTypeList[i].setCurrentText(item.type)
-            # self.symbolPropsLayout.addWidget(self.attributeTypeList[i], i + 1, 1)
-            self.attributeDefList.append(edf.longLineEdit())
-            self.attributeDefList[i].setText(item.definition)
-            self.symbolPropsLayout.addWidget(self.attributeDefList[i], i + 1, 1)
-            i += 1
-
-        self.attributeNameList.append(edf.longLineEdit())
-        # attrTypeCombo = QComboBox()
-        # attrTypeCombo.addItems(shp.label.labelTypes)
-        # self.attributeTypeList.append(attrTypeCombo)
-        self.attributeDefList.append(edf.longLineEdit())
-        self.symbolPropsLayout.addWidget(self.attributeNameList[-1], i + 2, 0)
-        # self.symbolPropsLayout.addWidget(self.attributeTypeList[-1], i + 2, 1)
-        self.symbolPropsLayout.addWidget(self.attributeDefList[-1], i + 2, 1)
-        self.attributeNameList[-1].setPlaceholderText("Enter Attribute Name")
-        # self.attributeTypeList[-1].setToolTip("Enter Attribute Type")
-        self.attributeDefList[-1].setToolTip("Enter Attribute Definition")
-        self.attributeDefList[-1].editingFinished.connect(
-            lambda: self.updateAttributeDef(i + 1))
-
-    def updateAttributeDef(self, i):
-        i += 1
-        self.attributeNameList.append(edf.longLineEdit())
-        # attrTypeCombo = QComboBox()
-        # attrTypeCombo.addItems(shp.label.labelTypes)
-        # self.attributeTypeList.append(attrTypeCombo)
-        self.attributeDefList.append(edf.longLineEdit())
-        self.symbolPropsLayout.addWidget(self.attributeNameList[-1], i + 1, 0)
-        # self.symbolPropsLayout.addWidget(self.attributeTypeList[-1], i + 1, 1)
-        self.symbolPropsLayout.addWidget(self.attributeDefList[-1], i + 1, 1)
-        self.attributeNameList[-1].setPlaceholderText("Enter Attribute Name")
-        # self.attributeTypeList[-1].setToolTip("Enter Attribute Type")
-        self.attributeDefList[-1].setToolTip("Enter Attribute Definition")
-        self.attributeDefList[-1].editingFinished.connect(
-            lambda: self.updateAttributeDef(i))
-
-    def symbolLabelsMethod(self):
-        self.labelDefinitionList = []
-        self.labelHeightList = []
-        self.labelAlignmentList = []
-        self.labelOrientationList = []
-        self.labelUseList = []
-        self.labelTypeList = []
-        self.labelItemList = []
-        i = 0
-        self.symbolLabelsLayout.addWidget(edf.boldLabel("Definition"), 0, 0)
-        self.symbolLabelsLayout.addWidget(edf.boldLabel("Height"), 0, 1)
-        self.symbolLabelsLayout.addWidget(edf.boldLabel("Alignment"), 0, 2)
-        self.symbolLabelsLayout.addWidget(edf.boldLabel("Orientation"), 0, 3)
-        self.symbolLabelsLayout.addWidget(edf.boldLabel("Use"), 0, 4)
-        self.symbolLabelsLayout.addWidget(edf.boldLabel("Type"), 0, 5)
-        for item in self.items:
-            if type(item) == shp.label:
-                i += 1
-                self.labelItemList.append(item)
-                self.labelDefinitionList.append(edf.longLineEdit())
-                self.labelDefinitionList[-1].setText(item.labelDefinition)
-                self.labelDefinitionList[-1].setReadOnly(True)
-                self.symbolLabelsLayout.addWidget(
-                    self.labelDefinitionList[i - 1], i, 0)
-                self.labelHeightList.append(edf.shortLineEdit())
-                self.labelHeightList[-1].setText(str(item.labelHeight))
-                self.symbolLabelsLayout.addWidget(self.labelHeightList[i - 1],
-                    i, 1)
-                self.labelAlignmentList.append(QComboBox())
-                self.labelAlignmentList[-1].addItems(shp.label.labelAlignments)
-                self.labelAlignmentList[-1].setCurrentText(item.labelAlign)
-                self.symbolLabelsLayout.addWidget(self.labelAlignmentList[-1],
-                    i, 2)
-                self.labelOrientationList.append(QComboBox())
-                self.labelOrientationList[-1].addItems(shp.label.labelOrients)
-                self.labelOrientationList[-1].setCurrentText(item.labelOrient)
-                self.symbolLabelsLayout.addWidget(self.labelOrientationList[-1],
-                    i, 3)
-                self.labelUseList.append(QComboBox())
-                self.labelUseList[-1].addItems(shp.label.labelUses)
-                self.labelUseList[-1].setCurrentText(item.labelUse)
-                self.symbolLabelsLayout.addWidget(self.labelUseList[-1], i, 4)
-                self.labelTypeList.append(QComboBox())
-                self.labelTypeList[-1].addItems(shp.label.labelTypes)
-                self.labelTypeList[-1].setCurrentText(item.labelType)
-                self.symbolLabelsLayout.addWidget(self.labelTypeList[-1], i, 5)
-        if i == 0:  # no labels to edit
-            self.symbolLabelsLayout.addWidget(QLabel("No symbol labels found."),
-                1, 0)
-
-
-class instanceProperties(QDialog):
-    def __init__(self, parent, instance: shp.symbolShape = None):
-        # assert isinstance(instance, shp.symbolShape)
-        super().__init__(parent)
-        self.parent = parent
-        self.instance = instance
-        self.initUI()
-
-    def initUI(self):
-        self.setWindowTitle("Instance Properties")
-        self.mainLayout = QVBoxLayout()
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        formLayout = QFormLayout()
-        self.libNameEdit = edf.longLineEdit()
-        self.libNameEdit.setText(self.instance.libraryName)
-        formLayout.addRow(edf.boldLabel("Library Name", self), self.libNameEdit)
-        self.cellNameEdit = edf.longLineEdit()
-        self.cellNameEdit.setText(self.instance.cellName)
-        formLayout.addRow(edf.boldLabel("Cell Name", self), self.cellNameEdit)
-        self.viewNameEdit = edf.longLineEdit()
-        self.viewNameEdit.setText(self.instance.viewName)
-        formLayout.addRow(edf.boldLabel("View Name", self), self.viewNameEdit)
-        self.instNameEdit = edf.longLineEdit()
-        self.instNameEdit.setText(self.instance.instanceName)
-        formLayout.addRow(edf.boldLabel("Instance Name", self), self.instNameEdit)
-        location = (
-                self.instance.scenePos() - self.instance.scene().origin).toTuple()
-        self.xLocationEdit = edf.shortLineEdit()
-        self.xLocationEdit.setText(str(location[0]))
-        formLayout.addRow(edf.boldLabel("x location", self), self.xLocationEdit)
-        self.yLocationEdit = edf.shortLineEdit()
-        self.yLocationEdit.setText(str(location[1]))
-        formLayout.addRow(edf.boldLabel("y location", self), self.yLocationEdit)
-        self.angleEdit = edf.longLineEdit()
-        self.angleEdit.setText(str(self.instance.angle))
-        formLayout.addRow(edf.boldLabel("Angle", self), self.angleEdit)
-        formLayout.setVerticalSpacing(10)
-        self.instanceLabelsLayout = QGridLayout()
-        row_index = 0
-        for label in self.instance.labels.values():
-            if label.labelDefinition not in shp.label.predefinedLabels:
-                self.instanceLabelsLayout.addWidget(
-                    edf.boldLabel(label.labelName, self), row_index, 0)
-                labelValueEdit = edf.longLineEdit()
-                labelValueEdit.setText(str(label.labelValue))
-                self.instanceLabelsLayout.addWidget(labelValueEdit, row_index,
-                    1)
-                visibleCombo = QComboBox(self)
-                visibleCombo.setInsertPolicy(QComboBox.NoInsert)
-                visibleCombo.addItems(["True", "False"])
-                if label.labelVisible:
-                    visibleCombo.setCurrentIndex(0)
-                else:
-                    visibleCombo.setCurrentIndex(1)
-                self.instanceLabelsLayout.addWidget(visibleCombo,row_index,2)
-                row_index += 1
-
-        instanceAttributesLayout = QGridLayout()
-        instanceAttributesLayout.setColumnMinimumWidth(0, 100)
-        for counter, name in enumerate(self.instance.attr.keys()):
-            instanceAttributesLayout.addWidget(edf.boldLabel(name, self), counter,
-                0)
-            labelType = edf.longLineEdit()
-            labelType.setReadOnly(True)
-            labelName = edf.longLineEdit()
-            labelName.setText(self.instance.attr[name])
-            instanceAttributesLayout.addWidget(labelName, counter, 1)
-
-        self.mainLayout.addLayout(formLayout)
-        self.mainLayout.addWidget(edf.boldLabel("Instance Labels", self))
-        self.mainLayout.addLayout(self.instanceLabelsLayout)
-        self.mainLayout.addSpacing(40)
-        self.mainLayout.addWidget(edf.boldLabel("Instance Attributes", self))
-        self.mainLayout.addLayout(instanceAttributesLayout)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-
-
-class netProperties(QDialog):
-    def __init__(self, parent, net: net.schematicNet = None):
-        # assert isinstance(instance, shp.symbolShape)
-        super().__init__(parent)
-        self.parent = parent
-        self.net = net
-        self.initUI()
-
-    def initUI(self):
-        self.setWindowTitle("Net Properties")
-        self.mainLayout = QVBoxLayout()
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        formBox = QGroupBox('Net Properties')
-        formLayout = QFormLayout()
-        self.netNameEdit = edf.longLineEdit()
-        self.netNameEdit.setText(self.net.name)
-        formLayout.addRow(edf.boldLabel("Net Name", self), self.netNameEdit)
-        formBox.setLayout(formLayout)
-        self.mainLayout.addWidget(formBox)
-        self.mainLayout.addSpacing(40)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-
-
-class createSchematicPinDialog(createPinDialog):
-    def __init__(self, parent):
-        super().__init__(parent)
-        self.setWindowTitle("Create Schematic Pin")
-
-
-class schematicPinPropertiesDialog(createPinDialog):
-    def __init__(self, parent, item):
-        super().__init__(parent)
-        self.setWindowTitle(f"{item.pinName} - Pin Properties")
-        self.pinName.setText(item.pinName)
-        self.pinDir.setCurrentText(item.pinDir)
-        self.pinType.setCurrentText(item.pinType)
-
-class symbolNameDialog(QDialog):
-    def __init__(self, cellPath:pathlib.Path, cellName: str, parent):
-        super().__init__(parent)
-        self.cellPath = cellPath
-        self.cellName = cellName
-        self.symbolViewNames = [view.stem for view in cellPath.iterdir() if 'symbol' in
-                                view.stem]
-        self.initUI()
-    def initUI(self):
-        self.setWindowTitle('Create a symbol?')
-        self.mainLayout = QVBoxLayout()
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        formLayout = QFormLayout()
-        formLayout.addRow(edf.boldLabel('Library Name'), QLabel(
-            self.cellPath.parent.stem) )
-        formLayout.addRow(edf.boldLabel('Cell Name'), QLabel(self.cellPath.stem))
-        self.symbolViewsCB = QComboBox()
-        self.symbolViewsCB.addItems(self.symbolViewNames)
-        self.symbolViewsCB.setEditable(True)
-        formLayout.addRow(edf.boldLabel('Symbol View Name:'), self.symbolViewsCB)
-        self.mainLayout.addLayout(formLayout)
-        self.mainLayout.addSpacing(40)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-
-class symbolCreateDialog(QDialog):
-    def __init__(self, parent, inputPinNames: list, outputPinNames: list,
-                 inoutPinNames: list):
-        super().__init__(parent)
-        self.parent = parent
-        self.inputPinNames = inputPinNames
-        self.outputPinNames = outputPinNames
-        self.inoutPinNames = inoutPinNames
-        self.setWindowTitle("Create Symbol")
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.mainLayout = QVBoxLayout()
-
-        self.fLayout = QFormLayout()
-        self.topPinsEdit = edf.longLineEdit()
-        self.topPinsEdit.setText(', '.join(self.inoutPinNames))
-        self.topPinsEdit.setToolTip("Enter top pins")
-        self.fLayout.addRow(edf.boldLabel("Top Pins:"), self.topPinsEdit)
-        self.leftPinsEdit = edf.longLineEdit()
-        self.leftPinsEdit.setText(', '.join(self.inputPinNames))
-        self.leftPinsEdit.setToolTip("Enter left pins")
-        self.fLayout.addRow(edf.boldLabel("Left Pins:"), self.leftPinsEdit)
-        self.bottomPinsEdit = edf.longLineEdit()
-        self.bottomPinsEdit.setToolTip("Enter bottom pins")
-        self.fLayout.addRow(edf.boldLabel("Bottom Pins:"), self.bottomPinsEdit)
-        self.rightPinsEdit = edf.longLineEdit()
-        self.rightPinsEdit.setText(', '.join(self.outputPinNames))
-        self.rightPinsEdit.setToolTip("Enter right pins")
-        self.fLayout.addRow(edf.boldLabel("Right Pins:"), self.rightPinsEdit)
-        self.mainLayout.addLayout(self.fLayout)
-        self.mainLayout.addSpacing(20)
-        self.geomLayout = QFormLayout()
-        self.stubLengthEdit = QLineEdit()
-        self.stubLengthEdit.setText('60')
-        self.stubLengthEdit.setToolTip('Enter stub lengths')
-        self.geomLayout.addRow(edf.boldLabel("Stub Length:"), self.stubLengthEdit)
-        self.pinDistanceEdit = QLineEdit()
-        self.pinDistanceEdit.setText('80')
-        self.pinDistanceEdit.setToolTip('Enter pin spacing')
-        self.geomLayout.addRow(edf.boldLabel("Pin spacing:"), self.pinDistanceEdit)
-        self.mainLayout.addLayout(self.geomLayout)
-        self.mainLayout.addSpacing(40)
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-        self.show()
-
-
-class noteTextEdit(QDialog):
-    '''
-    Set text properties.
-    '''
-    def __init__(self,parent):
-        super().__init__(parent)
-        self.parent = parent
-        self.setWindowTitle("Edit Text")
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        mainLayout = QVBoxLayout()
-        self.plainTextEdit = QTextEdit()
-        mainLayout.addWidget(self.plainTextEdit)
-        fontFamilies = QFontDatabase.families(QFontDatabase.Latin)
-        fixedFamilies = [family for family in fontFamilies if
-                         QFontDatabase.isFixedPitch(family)]
-        formLayout = QFormLayout()
-        self.familyCB = QComboBox()
-        self.familyCB.addItems(fixedFamilies)
-        self.familyCB.currentTextChanged.connect(self.familyFontStyles)
-        formLayout.addRow(edf.boldLabel('Font Name'),self.familyCB)
-        self.fontStyleCB = QComboBox()
-        self.fontStyles = QFontDatabase.styles(fixedFamilies[0])
-        self.fontStyleCB.addItems(self.fontStyles)
-        self.fontStyleCB.currentTextChanged.connect(self.styleFontSizes)
-        formLayout.addRow(edf.boldLabel('Font Style'), self.fontStyleCB)
-        self.fontsizeCB = QComboBox()
-        self.fontSizes = [str(size) for size in QFontDatabase.pointSizes(fixedFamilies[0],
-                                                          self.fontStyles[0])]
-        self.fontsizeCB.addItems(self.fontSizes)
-        formLayout.addRow(edf.boldLabel('Font Size'),self.fontsizeCB)
-        self.textAlignmCB = QComboBox()
-        self.textAlignmCB.addItems(shp.text.textAlignments)
-        formLayout.addRow(edf.boldLabel('Text Alignment'),self.textAlignmCB)
-        self.textOrientCB = QComboBox()
-        self.textOrientCB.addItems(shp.text.textOrients)
-        formLayout.addRow(edf.boldLabel('Text Orientation'), self.textOrientCB)
-        mainLayout.addLayout(formLayout)
-        mainLayout.addSpacing(40)
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        mainLayout.addWidget(self.buttonBox)
-        self.setLayout(mainLayout)
-        self.show()
-
-    def familyFontStyles(self,s):
-        self.fontStyleCB.clear()
-        self.fontStyles = QFontDatabase.styles(self.familyCB.currentText())
-        self.fontStyleCB.addItems(self.fontStyles)
-
-    def styleFontSizes(self,s):
-        self.fontsizeCB.clear()
-        selectedFamily = self.familyCB.currentText()
-        selectedStyle = self.fontStyleCB.currentText()
-        self.fontSizes = [str(size) for size in QFontDatabase.pointSizes(
-            selectedFamily, selectedStyle)]
-        self.fontsizeCB.addItems(self.fontSizes)
-
-class noteTextEditProperties(noteTextEdit):
-    def __init__(self,parent, note:shp.text):
-        super().__init__(parent)
-        self.note = note
-        self.plainTextEdit.setText(self.note.textContent)
-        self.familyCB.setCurrentText(self.note.fontFamily)
-        self.fontStyleCB.setCurrentText(self.note.fontStyle)
-        self.fontsizeCB.setCurrentText(self.note.textHeight)
-        self.textAlignmCB.setCurrentText(self.note.textAlignment)
-        self.textOrientCB.setCurrentText(self.note.textOrient)
-
-
-class displayConfigDialog(QDialog):
-    def __init__(self, parent):
-        super().__init__(parent)
-        self.parent = parent
-        self.setWindowTitle("Display Options")
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        self.vLayout = QVBoxLayout()
-        fLayout = QFormLayout()
-        self.majorGridEntry = QLineEdit()
-        fLayout.addRow("Major Grid:", self.majorGridEntry)
-
-        self.vLayout.addLayout(fLayout)
-        self.vLayout.addStretch(1)
-        self.vLayout.addWidget(self.buttonBox)
-        self.setLayout(self.vLayout)
-        self.show()
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+# properties dialogues for various symbol items
+
+import pathlib
+
+from PySide6.QtGui import (QFontDatabase, )
+from PySide6.QtWidgets import (QDialog, QVBoxLayout, QHBoxLayout, QFormLayout,
+                               QDialogButtonBox, QLineEdit, QLabel, QComboBox,
+                               QGroupBox, QRadioButton, QGridLayout, QTextEdit,
+                               QMenu)
+
+import revedaEditor.common.net as net
+import revedaEditor.common.shape as shp
+import revedaEditor.gui.editFunctions as edf
+
+
+class rectPropertyDialog(QDialog):
+    '''
+    Property dialog for symbol rectangles.
+    '''
+    def __init__(self, parent, rectItem: shp.rectangle):
+        super().__init__(parent)
+        self.parent = parent
+        self.rectItem = rectItem
+        self.location = self.rectItem.scenePos().toTuple()
+        self.coords = self.rectItem.rect.getRect()
+
+        self.setWindowTitle("Rectangle Properties")
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.mainLayout = QVBoxLayout()
+        self.fLayout = QFormLayout()
+        self.fLayout.setContentsMargins(10, 10, 10, 10)
+        self.rectWidthLine = QLineEdit()
+        self.rectWidthLine.setText(str(self.coords[2]))
+        self.fLayout.addRow(QLabel("Width:"), self.rectWidthLine)
+        self.rectHeightLine = QLineEdit()
+        self.rectHeightLine.setText(str(self.coords[3]))
+        self.fLayout.addRow(QLabel("Height:"), self.rectHeightLine)
+        self.rectLeftLine = QLineEdit()
+        self.rectLeftLine.setText(
+            str(self.rectItem.start.toTuple()[0] + self.location[0]))
+        self.fLayout.addRow(QLabel("X Origin:"), self.rectLeftLine)
+        self.rectTopLine = QLineEdit()
+        self.rectTopLine.setText(
+            str(self.rectItem.start.toTuple()[1] + self.location[1]))
+        self.fLayout.addRow(QLabel("Y Origin:"), self.rectTopLine)
+        self.mainLayout.addLayout(self.fLayout)
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+        self.show()
+
+
+class circlePropertyDialog(QDialog):
+    def __init__(self, parent, circleItem: shp.circle):
+        super().__init__(parent)
+        self.parent = parent
+        self.circleItem = circleItem
+        self.location = self.circleItem.scenePos().toTuple()
+        self.centre = self.circleItem.mapToScene(
+            self.circleItem.centre).toTuple()
+        self.radius = self.circleItem.radius
+
+        self.setWindowTitle("Circle Properties")
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.mainLayout = QVBoxLayout()
+        self.fLayout = QFormLayout()
+        self.fLayout.setContentsMargins(10, 10, 10, 10)
+        self.centerXEdit = edf.shortLineEdit()
+        self.centerXEdit.setText(str(self.centre[0]))
+        self.fLayout.addRow(QLabel("center x-coord:"), self.centerXEdit)
+        self.centerYEdit = edf.shortLineEdit()
+        self.centerYEdit.setText(str(self.centre[1]))
+        self.fLayout.addRow(QLabel("center y-coord:"), self.centerYEdit)
+        self.radiusEdit = edf.shortLineEdit()
+        self.radiusEdit.setText(str(self.radius))
+        self.fLayout.addRow(QLabel("radius:"), self.radiusEdit)
+        self.mainLayout.addLayout(self.fLayout)
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+        self.show()
+
+class arcPropertyDialog(QDialog):
+    def __init__(self, parent, arcItem: shp.arc):
+        super().__init__(parent)
+        self.parent = parent
+        self.setWindowTitle("Arc Properties")
+        self.arcItem = arcItem
+        self.location = self.arcItem.scenePos().toTuple()
+        # self.arcType = self.arcItem.arcType
+        # self.arcTypeCombo = QComboBox()
+        # self.arcTypeCombo.addItems(shp.arc.arcTypes)
+        # self.arcTypeCombo.setCurrentText(self.arcType)
+
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.mainLayout = QVBoxLayout()
+        self.fLayout = QFormLayout()
+        self.fLayout.setContentsMargins(10, 10, 10, 10)
+        # self.mainLayout.addWidget(self.arcTypeCombo)
+        self.startXEdit = edf.shortLineEdit()
+        self.startXEdit.setText(
+            str(self.arcItem.start.toTuple()[0] + self.location[0]))
+        self.fLayout.addRow(QLabel("X Origin:"), self.startXEdit)
+        self.startYEdit = edf.shortLineEdit()
+        self.startYEdit.setText(
+            str(self.arcItem.start.toTuple()[1] + self.location[1]))
+        self.fLayout.addRow(QLabel("Y Origin:"), self.startYEdit)
+        self.widthEdit = edf.shortLineEdit()
+        self.widthEdit.setText(str(self.arcItem.width))
+        self.fLayout.addRow(QLabel("Width:"), self.widthEdit)
+        self.heightEdit = edf.shortLineEdit()
+        self.heightEdit.setText(str(self.arcItem.height))
+        self.fLayout.addRow(QLabel("Height:"), self.heightEdit)
+        self.mainLayout.addLayout(self.fLayout)
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+        self.show()
+
+class linePropertyDialog(QDialog):
+    def __init__(self, parent, lineItem: shp.line):
+        super().__init__(parent)
+        self.parent = parent
+        self.lineItem = lineItem
+        self.location = self.lineItem.scenePos().toTuple()
+
+        self.setWindowTitle("Line Properties")
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.mainLayout = QVBoxLayout()
+        self.fLayout = QFormLayout()
+        self.fLayout.setContentsMargins(10, 10, 10, 10)
+        self.startXLine = QLineEdit()
+        self.startXLine.setText(
+            str(self.lineItem.start.toTuple()[0] + self.location[0]))
+        self.fLayout.addRow(QLabel("Start (X):"), self.startXLine)
+        self.startYLine = QLineEdit()
+        self.startYLine.setText(
+            str(self.lineItem.start.toTuple()[1] + self.location[1]))
+        self.fLayout.addRow(QLabel("Start (Y):"), self.startYLine)
+        self.endXLine = QLineEdit()
+        self.endXLine.setText(
+            str(self.lineItem.end.toTuple()[0] + self.location[0]))
+        self.fLayout.addRow(QLabel("End (X):"), self.endXLine)
+        self.endYLine = QLineEdit()
+        self.endYLine.setText(
+            str(self.lineItem.end.toTuple()[1] + self.location[1]))
+        self.fLayout.addRow(QLabel("End (Y):"), self.endYLine)
+        self.mainLayout.addLayout(self.fLayout)
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+        self.show()
+
+
+class createPinDialog(QDialog):
+    def __init__(self, parent) -> None:
+        super().__init__(parent)
+        self.setWindowTitle("Create Pin")
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.mainLayout = QVBoxLayout()
+        self.fLayout = QFormLayout()
+        self.pinName = QLineEdit()
+        self.pinName.setPlaceholderText("Pin Name")
+        self.pinName.setToolTip("Enter pin name")
+        self.fLayout.addRow(QLabel("Pin Name"), self.pinName)
+        self.pinDir = QComboBox()
+        self.pinDir.addItems(shp.pin.pinDirs)
+        self.pinDir.setToolTip("Select pin direction")
+        self.fLayout.addRow(QLabel("Pin Direction"), self.pinDir)
+        self.pinType = QComboBox()
+        self.pinType.addItems(shp.pin.pinTypes)
+        self.pinType.setToolTip("Select pin type")
+        self.fLayout.addRow(QLabel("Pin Type"), self.pinType)
+        self.mainLayout.addLayout(self.fLayout)
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+        self.show()
+
+
+class pinPropertyDialog(createPinDialog):
+    def __init__(self, parent, pinItem: shp.pin):
+        super().__init__(parent)
+        self.parent = parent
+        self.pinItem = pinItem
+        self.location = self.pinItem.scenePos().toTuple()
+
+        self.setWindowTitle("Pin Properties")
+        self.pinName.setText(str(pinItem.pinName))
+        self.pinType.setCurrentText(pinItem.pinType)
+        self.pinDir.setCurrentText(pinItem.pinDir)
+        self.pinXLine = QLineEdit()
+        self.pinXLine.setText(str(self.pinItem.start.x() + self.location[0]))
+        self.pinXLine.setToolTip("X Coordinate")
+        self.fLayout.addRow(QLabel("X:"), self.pinXLine)
+        self.pinYLine = QLineEdit()
+        self.pinYLine.setText(str(self.pinItem.start.y() + self.location[1]))
+        self.pinYLine.setToolTip("Y Coordinate")
+        self.fLayout.addRow(QLabel("Y:"), self.pinYLine)
+
+
+class createSymbolLabelDialog(QDialog):
+    def __init__(self, parent) -> None:
+        super().__init__(parent)
+        self.setWindowTitle("Create Label")
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.mainLayout = QVBoxLayout()
+        self.fLayout = QFormLayout()
+        self.labelDefinition = QLineEdit()
+        self.labelDefinition.setPlaceholderText("Label Definition")
+        self.labelDefinition.setToolTip("Enter label Definition")
+        self.fLayout.addRow(QLabel("Label Definition"), self.labelDefinition)
+        self.labelHeightEdit = QLineEdit()
+        self.labelHeightEdit.setPlaceholderText("Label Height")
+        self.labelHeightEdit.setToolTip("Enter label Height")
+        self.fLayout.addRow(QLabel("Label Height"), self.labelHeightEdit)
+        self.labelAlignCombo = QComboBox()
+        self.labelAlignCombo.addItems(shp.label.labelAlignments)
+        self.fLayout.addRow(QLabel("Label Alignment"), self.labelAlignCombo)
+        self.labelOrientCombo = QComboBox()
+        self.labelOrientCombo.addItems(shp.label.labelOrients)
+        self.fLayout.addRow(QLabel("Label Orientation"), self.labelOrientCombo)
+        self.labelUseCombo = QComboBox()
+        self.labelUseCombo.addItems(shp.label.labelUses)
+        self.fLayout.addRow(QLabel("Label Use"), self.labelUseCombo)
+        self.labelVisiCombo = QComboBox()
+        self.labelVisiCombo.addItems(["Yes", "No"])
+        self.fLayout.addRow(QLabel("Label Visible"),self.labelVisiCombo)
+        self.mainLayout.addLayout(self.fLayout)
+        self.labelTypeGroup = QGroupBox("Label Type")
+        self.labelTypeLayout = QHBoxLayout()
+        self.normalType = QRadioButton(shp.label.labelTypes[0])
+        self.normalType.setChecked(True)
+        self.NLPType = QRadioButton(shp.label.labelTypes[1])
+        self.pyLType = QRadioButton(shp.label.labelTypes[2])
+        self.labelTypeLayout.addWidget(self.normalType)
+        self.labelTypeLayout.addWidget(self.NLPType)
+        self.labelTypeLayout.addWidget(self.pyLType)
+        self.labelTypeGroup.setLayout(self.labelTypeLayout)
+        self.mainLayout.addWidget(self.labelTypeGroup)
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+        self.show()
+
+
+class labelPropertyDialog(createSymbolLabelDialog):
+    def __init__(self, parent, labelItem: shp.label):
+        assert isinstance(labelItem, shp.label)
+        super().__init__(parent)
+        self.parent = parent
+        self.labelItem = labelItem
+        self.location = self.labelItem.scenePos().toTuple()
+
+        self.setWindowTitle("Label Properties")
+        self.labelDefinition.setText(str(labelItem.labelDefinition))
+        self.labelHeightEdit.setText(str(labelItem.labelHeight))
+        self.labelAlignCombo.setCurrentText(labelItem.labelAlign)
+        self.labelOrientCombo.setCurrentText(labelItem.labelOrient)
+        self.labelUseCombo.setCurrentText(labelItem.labelUse)
+        if labelItem.labelVisible:
+            self.labelVisiCombo.setCurrentText("Yes")
+        else:
+            self.labelVisiCombo.setCurrentText("No")
+        if self.labelItem.labelType == "Normal":
+            self.normalType.setChecked(True)
+        elif self.labelItem.labelType == "NLPLabel":
+            self.NLPType.setChecked(True)
+        elif self.labelItem.labelType == "PyLabel":
+            self.pyLType.setChecked(True)
+        self.labelXLine = QLineEdit()
+        self.labelXLine.setText(
+            str(self.labelItem.start.x() + self.location[0]))
+        self.labelXLine.setToolTip("X Coordinate")
+        self.fLayout.addRow(QLabel("X:"), self.labelXLine)
+        self.labelYLine = QLineEdit()
+        self.labelYLine.setText(
+            str(self.labelItem.start.y() + self.location[1]))
+        self.labelYLine.setToolTip("Y Coordinate")
+        self.fLayout.addRow(QLabel("Y:"), self.labelYLine)
+
+
+class symbolLabelsDialogue(QDialog):
+    """
+    Dialog for changing symbol labels and attributes. Symbol properties... menu item.
+    """
+
+    def __init__(self, parent, items: list, attributes: list):
+        super().__init__(parent)
+        self.parent = parent
+        self.items = items
+        self.attributes = attributes
+        self.setWindowTitle("Symbol Labels")
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.mainLayout = QVBoxLayout()
+        self.symbolPropsLayout = QGridLayout()
+        self.symbolLabelsLayout = QGridLayout()
+        self.symbolAttrsMethod()
+        # Symbol Labels Layout
+        self.symbolLabelsMethod()
+        labelsGroup = QGroupBox("Symbol Labels")
+        labelsGroup.setLayout(self.symbolLabelsLayout)
+        self.mainLayout.addWidget(labelsGroup)
+        self.mainLayout.addStretch(1)
+        # self.mainLayout.addLayout(self.symbolLabelsLayout)
+        propsGroup = QGroupBox("Symbol Attributes")
+        propsGroup.setLayout(self.symbolPropsLayout)
+        self.mainLayout.addWidget(propsGroup)
+        self.mainLayout.addStretch(1)
+        # self.mainLayout.addLayout(self.symbolPropsLayout)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+
+    def symbolAttrsMethod(self):
+        self.attributeNameList = []
+        # self.attributeTypeList = []
+        self.attributeDefList = []
+        # Symbol Properties
+        self.symbolPropsLayout.addWidget(QLabel("Attribute Name"), 0, 0)
+        # self.symbolPropsLayout.addWidget(QLabel("Type"), 0, 1)
+        self.symbolPropsLayout.addWidget(QLabel("Definition"), 0, 1)
+        i = 0
+        for item in self.attributes:
+            self.attributeNameList.append(edf.longLineEdit())
+            self.attributeNameList[i].setText(item.name)
+            self.symbolPropsLayout.addWidget(self.attributeNameList[i], i + 1,
+                0)
+            self.attributeDefList.append(edf.longLineEdit())
+            self.attributeDefList[i].setText(item.definition)
+            self.symbolPropsLayout.addWidget(self.attributeDefList[i], i + 1, 1)
+            i += 1
+
+        self.attributeNameList.append(edf.longLineEdit())
+        self.attributeDefList.append(edf.longLineEdit())
+        self.symbolPropsLayout.addWidget(self.attributeNameList[-1], i + 2, 0)
+        self.symbolPropsLayout.addWidget(self.attributeDefList[-1], i + 2, 1)
+        self.attributeNameList[-1].setPlaceholderText("Enter Attribute Name")
+        self.attributeDefList[-1].setToolTip("Enter Attribute Definition")
+        self.attributeDefList[-1].editingFinished.connect(
+            lambda: self.updateAttributeDef(i + 1))
+
+    def updateAttributeDef(self, i):
+        i += 1
+        self.attributeNameList.append(edf.longLineEdit())
+        self.attributeDefList.append(edf.longLineEdit())
+        self.symbolPropsLayout.addWidget(self.attributeNameList[-1], i + 1, 0)
+        self.symbolPropsLayout.addWidget(self.attributeDefList[-1], i + 1, 1)
+        self.attributeNameList[-1].setPlaceholderText("Enter Attribute Name")
+        self.attributeDefList[-1].setToolTip("Enter Attribute Definition")
+        self.attributeDefList[-1].editingFinished.connect(
+            lambda: self.updateAttributeDef(i))
+
+    def symbolLabelsMethod(self):
+        self.labelDefinitionList = []
+        self.labelHeightList = []
+        self.labelAlignmentList = []
+        self.labelOrientationList = []
+        self.labelUseList = []
+        self.labelTypeList = []
+        self.labelItemList = []
+        i = 0
+        self.symbolLabelsLayout.addWidget(edf.boldLabel("Definition"), 0, 0)
+        self.symbolLabelsLayout.addWidget(edf.boldLabel("Height"), 0, 1)
+        self.symbolLabelsLayout.addWidget(edf.boldLabel("Alignment"), 0, 2)
+        self.symbolLabelsLayout.addWidget(edf.boldLabel("Orientation"), 0, 3)
+        self.symbolLabelsLayout.addWidget(edf.boldLabel("Use"), 0, 4)
+        self.symbolLabelsLayout.addWidget(edf.boldLabel("Type"), 0, 5)
+        for item in self.items:
+            if type(item) == shp.label:
+                i += 1
+                self.labelItemList.append(item)
+                self.labelDefinitionList.append(edf.longLineEdit())
+                self.labelDefinitionList[-1].setText(item.labelDefinition)
+                self.labelDefinitionList[-1].setReadOnly(True)
+                self.symbolLabelsLayout.addWidget(
+                    self.labelDefinitionList[i - 1], i, 0)
+                self.labelHeightList.append(edf.shortLineEdit())
+                self.labelHeightList[-1].setText(str(item.labelHeight))
+                self.symbolLabelsLayout.addWidget(self.labelHeightList[i - 1],
+                    i, 1)
+                self.labelAlignmentList.append(QComboBox())
+                self.labelAlignmentList[-1].addItems(shp.label.labelAlignments)
+                self.labelAlignmentList[-1].setCurrentText(item.labelAlign)
+                self.symbolLabelsLayout.addWidget(self.labelAlignmentList[-1],
+                    i, 2)
+                self.labelOrientationList.append(QComboBox())
+                self.labelOrientationList[-1].addItems(shp.label.labelOrients)
+                self.labelOrientationList[-1].setCurrentText(item.labelOrient)
+                self.symbolLabelsLayout.addWidget(self.labelOrientationList[-1],
+                    i, 3)
+                self.labelUseList.append(QComboBox())
+                self.labelUseList[-1].addItems(shp.label.labelUses)
+                self.labelUseList[-1].setCurrentText(item.labelUse)
+                self.symbolLabelsLayout.addWidget(self.labelUseList[-1], i, 4)
+                self.labelTypeList.append(QComboBox())
+                self.labelTypeList[-1].addItems(shp.label.labelTypes)
+                self.labelTypeList[-1].setCurrentText(item.labelType)
+                self.symbolLabelsLayout.addWidget(self.labelTypeList[-1], i, 5)
+        if i == 0:  # no labels to edit
+            self.symbolLabelsLayout.addWidget(QLabel("No symbol labels found."),
+                1, 0)
+
+
+class instanceProperties(QDialog):
+    def __init__(self, parent, instance: shp.symbolShape = None):
+        # assert isinstance(instance, shp.symbolShape)
+        super().__init__(parent)
+        self.parent = parent
+        self.instance = instance
+        self.initUI()
+
+    def initUI(self):
+        self.setWindowTitle("Instance Properties")
+        self.mainLayout = QVBoxLayout()
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        formLayout = QFormLayout()
+        self.libNameEdit = edf.longLineEdit()
+        self.libNameEdit.setReadOnly(True)
+        self.libNameEdit.setText(self.instance.libraryName)
+        self.libNameEdit.setToolTip("Library Name (Read Only)")
+        formLayout.addRow(edf.boldLabel("Library Name", self), self.libNameEdit)
+        self.cellNameEdit = edf.longLineEdit()
+        self.cellNameEdit.setText(self.instance.cellName)
+        self.cellNameEdit.setReadOnly(True)
+        self.cellNameEdit.setToolTip("Cell Name (Read Only)")
+        formLayout.addRow(edf.boldLabel("Cell Name", self), self.cellNameEdit)
+        self.viewNameEdit = edf.longLineEdit()
+        self.viewNameEdit.setText(self.instance.viewName)
+        self.viewNameEdit.setReadOnly(True)
+        self.viewNameEdit.setToolTip("View Name (Read Only)")
+        formLayout.addRow(edf.boldLabel("View Name", self), self.viewNameEdit)
+        self.instNameEdit = edf.longLineEdit()
+        self.instNameEdit.setText(self.instance.instanceName)
+        self.instNameEdit.setToolTip("Instance Name")
+        formLayout.addRow(edf.boldLabel("Instance Name", self), self.instNameEdit)
+        location = (self.instance.scenePos() - self.instance.scene().origin).toTuple()
+        self.xLocationEdit = edf.shortLineEdit()
+        self.xLocationEdit.setText(str(location[0]))
+        formLayout.addRow(edf.boldLabel("x location", self), self.xLocationEdit)
+        self.yLocationEdit = edf.shortLineEdit()
+        self.yLocationEdit.setText(str(location[1]))
+        formLayout.addRow(edf.boldLabel("y location", self), self.yLocationEdit)
+        self.angleEdit = edf.longLineEdit()
+        self.angleEdit.setText(str(self.instance.angle))
+        formLayout.addRow(edf.boldLabel("Angle", self), self.angleEdit)
+        formLayout.setVerticalSpacing(10)
+        self.instanceLabelsLayout = QGridLayout()
+        self.instanceLabelsLayout.setColumnMinimumWidth(0, 100)
+        self.instanceLabelsLayout.setColumnMinimumWidth(1, 200)
+        self.instanceLabelsLayout.setColumnMinimumWidth(2, 100)
+        self.instanceLabelsLayout.setColumnStretch(0, 0)
+        self.instanceLabelsLayout.setColumnStretch(1, 1)
+        self.instanceLabelsLayout.setColumnStretch(2, 0)
+        row_index = 0
+        for label in self.instance.labels.values():
+            if label.labelDefinition not in shp.label.predefinedLabels:
+                self.instanceLabelsLayout.addWidget(
+                    edf.boldLabel(label.labelName, self), row_index, 0)
+                labelValueEdit = edf.longLineEdit()
+                labelValueEdit.setText(str(label.labelValue))
+                self.instanceLabelsLayout.addWidget(labelValueEdit, row_index,
+                    1)
+                visibleCombo = QComboBox(self)
+                visibleCombo.setInsertPolicy(QComboBox.NoInsert)
+                visibleCombo.addItems(["True", "False"])
+                if label.labelVisible:
+                    visibleCombo.setCurrentIndex(0)
+                else:
+                    visibleCombo.setCurrentIndex(1)
+                self.instanceLabelsLayout.addWidget(visibleCombo,row_index,2)
+                row_index += 1
+
+        instanceAttributesLayout = QGridLayout()
+        instanceAttributesLayout.setColumnMinimumWidth(0, 100)
+        instanceAttributesLayout.setColumnMinimumWidth(1, 200)
+        instanceAttributesLayout.setColumnStretch(0, 0)
+        instanceAttributesLayout.setColumnStretch(1, 1)
+        # now list instance attributes
+        for counter, name in enumerate(self.instance.attr.keys()):
+            instanceAttributesLayout.addWidget(edf.boldLabel(name, self), counter,
+                0)
+            labelType = edf.longLineEdit()
+            labelType.setReadOnly(True)
+            labelNameEdit = edf.longLineEdit()
+            labelNameEdit.setText(self.instance.attr.get(name))
+            labelNameEdit.setToolTip(f"{name} attribute (Read Only)")
+            instanceAttributesLayout.addWidget(labelNameEdit, counter, 1)
+
+        self.mainLayout.addLayout(formLayout)
+        self.mainLayout.addWidget(edf.boldLabel("Instance Labels", self))
+        self.mainLayout.addLayout(self.instanceLabelsLayout)
+        self.mainLayout.addSpacing(40)
+        self.mainLayout.addWidget(edf.boldLabel("Instance Attributes", self))
+        self.mainLayout.addLayout(instanceAttributesLayout)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+
+
+class netProperties(QDialog):
+    def __init__(self, parent, net: net.schematicNet = None):
+        # assert isinstance(instance, shp.symbolShape)
+        super().__init__(parent)
+        self.parent = parent
+        self.net = net
+        self.initUI()
+
+    def initUI(self):
+        self.setWindowTitle("Net Properties")
+        self.mainLayout = QVBoxLayout()
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        formBox = QGroupBox('Net Properties')
+        formLayout = QFormLayout()
+        self.netNameEdit = edf.longLineEdit()
+        self.netNameEdit.setText(self.net.name)
+        formLayout.addRow(edf.boldLabel("Net Name", self), self.netNameEdit)
+        formBox.setLayout(formLayout)
+        self.mainLayout.addWidget(formBox)
+        self.mainLayout.addSpacing(40)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+
+
+class createSchematicPinDialog(createPinDialog):
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.setWindowTitle("Create Schematic Pin")
+
+
+class schematicPinPropertiesDialog(createPinDialog):
+    def __init__(self, parent, item):
+        super().__init__(parent)
+        self.setWindowTitle(f"{item.pinName} - Pin Properties")
+        self.pinName.setText(item.pinName)
+        self.pinDir.setCurrentText(item.pinDir)
+        self.pinType.setCurrentText(item.pinType)
+
+class symbolNameDialog(QDialog):
+    def __init__(self, cellPath:pathlib.Path, cellName: str, parent):
+        super().__init__(parent)
+        self.cellPath = cellPath
+        self.cellName = cellName
+        self.symbolViewNames = [view.stem for view in cellPath.iterdir() if 'symbol' in
+                                view.stem]
+        self.initUI()
+    def initUI(self):
+        self.setWindowTitle('Create a symbol?')
+        self.mainLayout = QVBoxLayout()
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        formLayout = QFormLayout()
+        formLayout.addRow(edf.boldLabel('Library Name'), QLabel(
+            self.cellPath.parent.stem) )
+        formLayout.addRow(edf.boldLabel('Cell Name'), QLabel(self.cellPath.stem))
+        self.symbolViewsCB = QComboBox()
+        self.symbolViewsCB.addItems(self.symbolViewNames)
+        self.symbolViewsCB.setEditable(True)
+        formLayout.addRow(edf.boldLabel('Symbol View Name:'), self.symbolViewsCB)
+        self.mainLayout.addLayout(formLayout)
+        self.mainLayout.addSpacing(40)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+
+class symbolCreateDialog(QDialog):
+    def __init__(self, parent, inputPinNames: list, outputPinNames: list,
+                 inoutPinNames: list):
+        super().__init__(parent)
+        self.parent = parent
+        self.inputPinNames = inputPinNames
+        self.outputPinNames = outputPinNames
+        self.inoutPinNames = inoutPinNames
+        self.setWindowTitle("Create Symbol")
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.mainLayout = QVBoxLayout()
+
+        self.fLayout = QFormLayout()
+        self.topPinsEdit = edf.longLineEdit()
+        self.topPinsEdit.setText(', '.join(self.inoutPinNames))
+        self.topPinsEdit.setToolTip("Enter top pins")
+        self.fLayout.addRow(edf.boldLabel("Top Pins:"), self.topPinsEdit)
+        self.leftPinsEdit = edf.longLineEdit()
+        self.leftPinsEdit.setText(', '.join(self.inputPinNames))
+        self.leftPinsEdit.setToolTip("Enter left pins")
+        self.fLayout.addRow(edf.boldLabel("Left Pins:"), self.leftPinsEdit)
+        self.bottomPinsEdit = edf.longLineEdit()
+        self.bottomPinsEdit.setToolTip("Enter bottom pins")
+        self.fLayout.addRow(edf.boldLabel("Bottom Pins:"), self.bottomPinsEdit)
+        self.rightPinsEdit = edf.longLineEdit()
+        self.rightPinsEdit.setText(', '.join(self.outputPinNames))
+        self.rightPinsEdit.setToolTip("Enter right pins")
+        self.fLayout.addRow(edf.boldLabel("Right Pins:"), self.rightPinsEdit)
+        self.mainLayout.addLayout(self.fLayout)
+        self.mainLayout.addSpacing(20)
+        self.geomLayout = QFormLayout()
+        self.stubLengthEdit = QLineEdit()
+        self.stubLengthEdit.setText('60')
+        self.stubLengthEdit.setToolTip('Enter stub lengths')
+        self.geomLayout.addRow(edf.boldLabel("Stub Length:"), self.stubLengthEdit)
+        self.pinDistanceEdit = QLineEdit()
+        self.pinDistanceEdit.setText('80')
+        self.pinDistanceEdit.setToolTip('Enter pin spacing')
+        self.geomLayout.addRow(edf.boldLabel("Pin spacing:"), self.pinDistanceEdit)
+        self.mainLayout.addLayout(self.geomLayout)
+        self.mainLayout.addSpacing(40)
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+        self.show()
+
+
+class noteTextEdit(QDialog):
+    '''
+    Set text properties.
+    '''
+    def __init__(self,parent):
+        super().__init__(parent)
+        self.parent = parent
+        self.setWindowTitle("Edit Text")
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        mainLayout = QVBoxLayout()
+        self.plainTextEdit = QTextEdit()
+        mainLayout.addWidget(self.plainTextEdit)
+        fontFamilies = QFontDatabase.families(QFontDatabase.Latin)
+        fixedFamilies = [family for family in fontFamilies if
+                         QFontDatabase.isFixedPitch(family)]
+        formLayout = QFormLayout()
+        self.familyCB = QComboBox()
+        self.familyCB.addItems(fixedFamilies)
+        self.familyCB.currentTextChanged.connect(self.familyFontStyles)
+        formLayout.addRow(edf.boldLabel('Font Name'),self.familyCB)
+        self.fontStyleCB = QComboBox()
+        self.fontStyles = QFontDatabase.styles(fixedFamilies[0])
+        self.fontStyleCB.addItems(self.fontStyles)
+        self.fontStyleCB.currentTextChanged.connect(self.styleFontSizes)
+        formLayout.addRow(edf.boldLabel('Font Style'), self.fontStyleCB)
+        self.fontsizeCB = QComboBox()
+        self.fontSizes = [str(size) for size in QFontDatabase.pointSizes(fixedFamilies[0],
+                                                          self.fontStyles[0])]
+        self.fontsizeCB.addItems(self.fontSizes)
+        formLayout.addRow(edf.boldLabel('Font Size'),self.fontsizeCB)
+        self.textAlignmCB = QComboBox()
+        self.textAlignmCB.addItems(shp.text.textAlignments)
+        formLayout.addRow(edf.boldLabel('Text Alignment'),self.textAlignmCB)
+        self.textOrientCB = QComboBox()
+        self.textOrientCB.addItems(shp.text.textOrients)
+        formLayout.addRow(edf.boldLabel('Text Orientation'), self.textOrientCB)
+        mainLayout.addLayout(formLayout)
+        mainLayout.addSpacing(40)
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        mainLayout.addWidget(self.buttonBox)
+        self.setLayout(mainLayout)
+        self.show()
+
+    def familyFontStyles(self,s):
+        self.fontStyleCB.clear()
+        self.fontStyles = QFontDatabase.styles(self.familyCB.currentText())
+        self.fontStyleCB.addItems(self.fontStyles)
+
+    def styleFontSizes(self,s):
+        self.fontsizeCB.clear()
+        selectedFamily = self.familyCB.currentText()
+        selectedStyle = self.fontStyleCB.currentText()
+        self.fontSizes = [str(size) for size in QFontDatabase.pointSizes(
+            selectedFamily, selectedStyle)]
+        self.fontsizeCB.addItems(self.fontSizes)
+
+class noteTextEditProperties(noteTextEdit):
+    def __init__(self,parent, note:shp.text):
+        super().__init__(parent)
+        self.note = note
+        self.plainTextEdit.setText(self.note.textContent)
+        self.familyCB.setCurrentText(self.note.fontFamily)
+        self.fontStyleCB.setCurrentText(self.note.fontStyle)
+        self.fontsizeCB.setCurrentText(self.note.textHeight)
+        self.textAlignmCB.setCurrentText(self.note.textAlignment)
+        self.textOrientCB.setCurrentText(self.note.textOrient)
+
+
+class displayConfigDialog(QDialog):
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.parent = parent
+        self.setWindowTitle("Display Options")
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        self.vLayout = QVBoxLayout()
+        fLayout = QFormLayout()
+        self.majorGridEntry = QLineEdit()
+        fLayout.addRow("Major Grid:", self.majorGridEntry)
+        self.snapDistanceEntry = QLineEdit()
+        fLayout.addRow("Snap Distance", self.snapDistanceEntry)
+
+        gridTypeGroup = QGroupBox("Grid Type")
+        gridTypeLayout = QHBoxLayout()
+        self.dotType = QRadioButton('Dot Grid')
+        self.dotType.setChecked(True)
+        self.lineType = QRadioButton('Line Grid')
+        self.noType = QRadioButton('No Grid')
+        gridTypeLayout.addWidget(self.dotType)
+        gridTypeLayout.addWidget(self.lineType)
+        gridTypeLayout.addWidget(self.noType)
+        gridTypeGroup.setLayout(gridTypeLayout)
+
+        self.vLayout.addLayout(fLayout)
+        self.vLayout.addWidget(gridTypeGroup)
+        self.vLayout.addStretch(1)
+
+        self.vLayout.addWidget(self.buttonBox)
+        self.setLayout(self.vLayout)
+        self.show()
+
+class selectConfigDialogue(QDialog):
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.parent = parent
+        self.setWindowTitle("Selection Options")
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        vLayout = QVBoxLayout()
+        selectionTypeGroup = QGroupBox("Selection Type")
+        selectionTypeLayout = QHBoxLayout()
+        self.fullSelection = QRadioButton('Full')
+        self.partialSelection = QRadioButton('Partial')
+        selectionTypeLayout.addWidget(self.fullSelection)
+        selectionTypeLayout.addWidget(self.partialSelection)
+        selectionTypeGroup.setLayout(selectionTypeLayout)
+        vLayout.addWidget(selectionTypeGroup)
+        vLayout.addStretch(1)
+        vLayout.addWidget(self.buttonBox)
+        self.setLayout(vLayout)
+        self.show()
```

### Comparing `revolution-eda-0.4.1/gui/pythonConsole.py` & `revolution-eda-0.5.0/revedaEditor/gui/pythonConsole.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """ Console
 Interactive console widget.  Use to add an interactive python interpreter
 in a GUI application.
 """
 
-import sys
 import code
 import re
-from typing import Dict, Callable
-from PySide6.QtWidgets import (QLineEdit, QWidget, QGridLayout, QPlainTextEdit,
-                               QApplication)
+from typing import Callable
+
 from PySide6.QtCore import (Qt, Signal, QEvent, QSize, )
 from PySide6.QtGui import (QTextCharFormat, QBrush, QColor, QFont)
+from PySide6.QtWidgets import (QLineEdit, QWidget, QGridLayout, QPlainTextEdit)
 
 
 class LineEdit(QLineEdit):
     """QLIneEdit with a history buffer for recalling previous lines.
     I also accept tab as input (4 spaces).
     """
     newline = Signal(str)  # Signal when return key pressed
```

### Comparing `revolution-eda-0.4.1/pdk/__init__.py` & `revolution-eda-0.5.0/revedaEditor/gui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 #   derives, entirely or substantially, from the functionality of the Software. Any
 #   license notice or attribution required by the License must also include this
 #   Commons Clause License Condition notice.
 #  #
 #   Software: Revolution EDA
 #   License: Mozilla Public License 2.0
 #   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
```

### Comparing `revolution-eda-0.4.1/pyproject.toml` & `revolution-eda-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [tool.setuptools]
-packages = ['api', 'gui', 'pdk', 'common', 'fileio', 'backend', 'resources']
-py-modules = ['revinit']
+packages = ['revedaEditor.gui','revedaEditor.common','revedaEditor.fileio','revedaEditor.backend','revedaEditor.resources','pdk']
+py-modules = ['revinit', 'reveda']
 [project]
 name = "revolution-eda"
-version = "0.4.1"
+version = "0.5.0"
 description = 'Revolution EDA is a new generation integrated circuit design environment.'
-readme = "README_pypi.md"
+readme = "README.md"
 classifiers = ["Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["electronic", "design", "schematic"]
 dependencies = ["PySide6>=6.4.2",
     "quantiphy>=2.19",
 ]
 requires-python = ">=3.10"
 [project.urls]
 Homepage = "https://github.com/eskiyerli/revedaRelease"
 [project.scripts]
-reveda = "gui.appWindow:main"
+reveda = "reveda:main"
```

### Comparing `revolution-eda-0.4.1/resources/resources.py` & `revolution-eda-0.5.0/revedaEditor/resources/resources.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,2946 +1,3693 @@
-
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-# Resource object code (Python 3)
-# Created by: object code
-# Created by: The Resource Compiler for Qt version 6.3.1
-# WARNING! All changes made in this file will be lost!
-
-from PySide6 import QtCore
-
-qt_resource_data = b"\
-\x00\x00\x02\x1a\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xbcIDATx\xda\xa4\
-S=K#Q\x14=o\xe6e\xf1cc\xb3\x90\xa0\
-\x85\xca\x22\xeb.Q\x88\x8a\x04\x05A!\xa5\x95l\xca\
-\xb5\xddZHc\xe1\xb6[\xa9\xb5\xb6\xfe\x82\x80M\x1a\
-\xc1\x8f\xc2\x0fD%Xh1$\xa3\x12\xa3\x19a\xd5\
-,\x92\x99I\xbc\xf7\x8d\x19\x12e\x17\xd4\x0b\x87\xb93\
-\xf7\xde3\xe7\x1e\xde\x13\xd5j\x15\xef\x09\x91H$>\
-\xd33F\x08\xber\xf6\x8e\xb0#]\xd7\x1dI&\x93\
-\xb3\xa1P(\xe2\xba\x0e\x1c\xc7%\xd8\xb0m\xce\x1dT\
-*\x15x\x22u\x08!\x15\xa4\xfc\x00\xcb\xb2\x8e\x97\x97\
-\x17~Kjh+\x95J\x11\xc30T3\x83H\x15\
-\xfe\x97\x13\x22\xa9T\xaaU\x06\x02\x81J<\x1e\x7f\xd3\
-\xfe\xe9tZH\x92)<\x99\x8df\xfeX=\xc5N\
-\xfe^\xe5\xb1\xf6\x8fX\x99\xfc\xd2h\x9e\x10\xbc\xa2\x22\
-\xd0j\xb2\xea\xe3\xe8\xe2\x16\x03\xc3\xc3^\xbe\xb7\xa7\xfc\
-\xa8\x0fM\xd3\xf8\x9b\xe6\x130\xea\xc3)^\xe3\xcc4\
-\xfd\xfc9\x81\xae\xeb\x1e\x81m\xdb\x1a\x17k\x0d\xe6\xcc\
-\x0c\xfe\x1e\x1eb\xaa{\x14\xa7\xe7'\xc8\xf7\x02=a\
-\x03\xbf6\xe6\xd0\xd5\x16\xc5tdQ\xf5\xf1\xca<+\
-\xcb\xe5\xb2\xce\x7f\xaf\x11\xdc\x1c\x1c`l|\x02,\xde\
-\xccna\xe9\xfb\x15\xa2\x83\xdf\xe8m\x08\xbb\xdb\x19\xbf\
-\x8f=\xe0Y&P+\x10\x9b*\x94\x88\xb9\xb0\xb6\x0f\
-\xc7\xfa\x03\xab\x85\x08\x8b:r\xd9\x9c\xaa\x15/\x1f\xfc\
->\xf6\x80g_(\xd0\xfb\xfa\xb0\x99\xc9\x00\x9f\x80\xa6\
-p\x18\x0f\xd7\xc0\xbaQP\xb5\xaf\x1d\xfd~\x9f\x94\xd2\
-S@\x87(\xc0r\xe8<\xa8Bt~\xbe\xc1\xac\xd8\
-\xbf\xee\x00\xcd\xa8\xd9`0\xf8\x93\x1c\xed|\xcbA\x22\
-\xe5\xa6\xa0g\xf3\xd3E\x92\xaf\x9c\xe7]\xee\xc4{\xaf\
-\xf3\xa3\x00\x03\x00%0\x12$Q\x12\x04\x0b\x00\x00\x00\
-\x00IEND\xaeB`\x82\
-\x00\x00\x02$\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xc6IDATx\xda\xa4\
-S\xbbN\x02A\x14\xbd\xfb\x80\x04\x88,\xcaK\x13\x02\
-H\x01\xb4\x84\x92\xd2B\x1bbO\xecL\xa8-\xec\xf8\
-\x05\xfd\x01\x0a\xfd\x03\x1aH4D\x8d\x09\x856\x1b\xb4\
-\xa0\xb1 \x94\x84\x87nx\x84\x00\x01<\x97\xc0\x06\xd8\
-\xed\x98\xe4\xe4\xce\x9d=s\xee\xb9;3\xc2b\xb1\xa0\
-}\x86H{\x0e9\x97\xcb\x1d\x8a\xa2x\x86\xb9\x1b\xe8\
-\xce\xe7\xf3\xd7\xd9l\xf6W\xaf\xd7uR$\x12!I\
-\x92LyR<\x1e\xbf\xccd2\xd7\xc0\x8d\xd3\xe9T\
-*\x95J\xbf\xdb\xed\xd6\xf0Q\x17\x18\x0e\x874\x9dN\
-\x0d\xbc\xd1hT\x93\x1b\x8d\xc61D\xce\x99\xc4\x11\xf9\
-\x93\xa2(\xd9M\x9b\xe3\xf1\x98Z\xad\x96m\x97\xc7\xdf\
-\xe0L\x8ay<\x1e%\x10\x08\x9c\x96J\xa5\xb7b\xb1\
-\xf8i\xb3\xd9\x1edYV'\x93I\x12\x9c|\xbf\xdf\
-W\xb1\xc1\xc0\xd34\xed[\x80\x1d\x0f\xec\xa6A\xf4\x01\
--\x08\x16\xd1k'\x91Hp\x01v\x92\xafV\xab\x84\
-\x9eMy2\x16;\xe8\xefq\xd3\xb2\xd7\xeb\xa5\xc1`\
-\xa0\xe7n\xb7\x9b\x9a\xcd\xa6\x81\x07\x01\x92\xcd\x8e\xc6b\
-\xb1\x10l\xeb9\xacS4\x1a]nX\x0f8\x22\xfe\
-\xd1\x06\x01\xab\xd5J\xbd^ok-\x18\x0c\x12.\xdc\
-\x116]\xb0\x1e\xd0A\xfe\x8c\xf8K\x0e\x87\x83\xff\xe4\
-Vu\x9c\xc2\x1aY\xbb\xddN>\x9f\x8fR\xa9\xd4U\
-\xb9\x5c~A\xd5\x05G\xce\x01\x12L\xaf'\xf7&/\
-\xcd\xa5Q\xe9\x84'\xe1p\xf8@U\xd5\xbb5'\x99\
-L\xde\x22\xdcKf\x02\xfc>\xb8?X\xfe\xc1\x5c]\
-!\xe6\xf7\xfb]\xa1P(\x5c(\x14\xdeq\x8c\x1f\xed\
-v\xfbk\xd3\x01\xcfY\x90K[\xb9\x9bU\x5c\x02\xae\
-\x5c\x00\xdf\x0b\x17\xa0A\x5c\x05\xea\xbb\x02\xc2\xea\x81I\
-&\x107\xc0\xbc)\xdfra\xdf\xe7\xfc/\xc0\x00g\
-y\xed\x91\x1b\x1bx)\x00\x00\x00\x00IEND\xae\
-B`\x82\
-\x00\x00\x01\xc8\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01jIDATx\xda\xa4\
-S?K\xc3@\x14\x7f\x97\xbb\x14\xaaD\x041\x89\x14\
-\x1c\x04!\x90\x0fP\xb4\x22\x08\x19\xfc\x04\x99\xdd\x5ct\
-\xeb\xe2'psq\xeb\xb7\xc8\x22\x96t(8\xf9\x01\
-\x9cj;X\x10\x1d2\x84\xb6\x08\xb9K\xe2\xbd\xab-\
-\x1c\xa2\x90\xf6\xc1\x8f;\x1e\xef\xfd\xee\xf7\xfe\x1c)\xcb\
-\x12\xd61\x16\x86\xe1\x81<\x9b\x12V\xc5\xdc\x89\xc43\
-\xcb\xf3\xfc\xa8\xddn\xdf\xd8\xb6\xed\xe7\xb9\x00!r\x09\
-\x0e\x9c\xe3]@Q\x140\x17I\x81\x10\xa6\xc0X\x0d\
-\x92$y\xe9t\xeen\x99\x0c\xd8\x9a\xcdf\xfeh4\
-R\xc1\x08I\xaa\xf0\xdf]\xc2\x8f\xa2h\x93\x99\xa6Y\
-\x04A\xb0R\xfd\xddn\x970)\x93\xcceVk&\
-!\x04KT\x04\xc6BV\x153\x0c\x03\x09\x8c%\x01\
-\xa2\x8aQJ\xe7\x04\x9cs\x03\xbb\xdd\x7f/\xe1\xe9\x93\
-jA{5\x01\xa7\xe6+L\xa7S\xcd\xef8\x0e4\
-\x1a\x0d\xc0\x5c\x96e\x19\xc5\xd7\x1f\x06\x02\xee\xcf\xb7\xb5\
-\xc0\xeb\xc7/8\xde\x15\xd0j\xb54\x7f\x1c\xc7\xe0\xba\
-.`.\x12\xa8\x12\x86\xe3\x0f\xe8\x0f\xb8\x168\x1c'\
-\x90\xd6R\xc0\x11k\x1b4\x99\xa8\x921w\xa9\xe0\xec\
-\xb0\x0eWq\xa2\x056w\x08\xa4i\x0a\xbd^O\xf3\
-{\x9e\xb7 \xa0L.\x91\x89#\xb9\xf07\x14~\xdb\
-\xc9\x9fcT\xb9\x96e]\xca\x8e\xee\xaf\xb2HR\xc5\
-\x1b\x91g\xfd\xe7#\xb1\x8a\xf9\x02\xdbA\xd6\xfd\xce\xdf\
-\x02\x0c\x00\x93\xb2\xe1\x85\xadb\x1d\x00\x00\x00\x00\x00I\
-END\xaeB`\x82\
-\x00\x00\x01\xbe\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01`IDATx\xdab\
-\xfc\xff\xff?\x03%\x80\x89\x81B0\x0c\x0c`Y\xc1\
-\xc8\xa8\xc8\xc8\xc0\xd0\x0ad\xab\x01\xf1-`\x90V\x03\
-\xf1\xfd\xcf@\x0e'T\xd1\xe6\xd0P\x06%%%\x06\
-fffA&&&g\xa0\x900\x10\xbf\xfd\xf7\xef\
-\xdf^f\x1f\x06\x86\xe9F\xf6\xf6N\x0e\xc1\xc1\xaaL\
-llb\x0f\x1f>T\xfe\xc3\xc0\xb0\xf6\x1f\x03\x831\
-\xd0y\x9b\xdf\x89\x89\xcdz\xa2\xa0\xc0\xf0\xf5\xebW\x86\
-\xdf\xbf\x7f\xfbGEE%\x03q\x01\x1f\x1f\x1f\xff\xe1\
-\xc3\x87?\xb3\x00mRU\x10\x17\x17\xff\xfe\xe4\x09\x03\
-\x88\xde\x0b\xe4C-\x9e\xf9\x93\x81\xe1\xf93QQ\x10\
-;\xed\xd7\xaf_\x0c\xaf^\xbd\xe2\xd4\xd0\xd0p\x07\x19\
-\x06\xa2\x1f<x\xb0\x9d\xd9\x9a\x81\xc1\x91\xe9\xcb\x17Q\
-\xa1_\xbfx\xce\xdd\xba\xf5\xf2\xce\xc7\x8fg\xa7\x03]\
-\xf0\x86\x81\xe1\xac\x04\x03C\xe4\xb2\xd7\xafg}`d\
-<\xfb\xfa\xf5\xeb\xb3o\xdf\xbeU\x17\x11\x11\xe1\x97\x91\
-\x91Q\xdc\xb2e\xcb\xbe\xcd\x9b7\x9f`T``\xd0\
-\x07z\xaa\x86\x85\x81A\x11\xe8\xf4\xfb\xbb\x18\x18&=\
-f`\xb8\x0b\xb4\xf5\x07\x10\x03\x85\x18\x80A\xc4\xc0\x0a\
-\xc4\xec,,,b\xec\xec\xecf@\xb6\x00\x10\x7f\xf8\
-\xf9\xf3\xe7\x11\x90$\x17\x10\xf3Bc\xe4/T\xd3o\
-(\xfd\x0fj\x00H\x8e\x05\x093\x031(\x09\x7fg\
-\x1cM\xca\x94\x1b\x00\x10`\x00\xc7\xc2x1&l\xf2\
-\xc7\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02\xb9\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02[IDATx\xda\x8c\
-\x92\xcdk\x13Q\x14\xc5\xcf|\x90\xc9d2I*m\
-\xa5\xd1\x85\xa1\x12\xb4 !h7\xae*(\xb6$\x15\
-\x85\xb6*\x82`W\x01\xa1\xff\x81)n\xb2Sqi\
-\xc9BqSQ(\xd8\x82\xad]\xd4EW\xb1\x22\x14\
-\xc1\xb4\xa5P,\xc6tfb\x93\xd6I2\xd3\xf9\xf0\
-\xcd\xa4jB\xc1\xf6\xc2\xe1=f\xee\xbb\xef\x9e\xdf}\
-\xd4\xf0\xf00\xf6c\x90\xa8\x0bG\x8b\x1fD\xd3\xce\x86\
-\xfd\xf3E\xd3\xb4\xael6\xfbLUU\xd4j5\x18\
-\x86\x09Y\xfeE\xf6\x16\xbc^\x1e\xa2(\x22\x10\x08 \
-\x18\x0c \x95\xbay\x9fa\x18\xb4\x14p\xc20\x0cT\
-*\x15\x94J%\xb7\x80$\xed\xa2\xaeY\x10\x04\x11\x86\
-i\x80fh\xf8\x04\xbe\xa5\x15\xfa\xbf\x8dR\x80M\x16\
-\x9b\xb2\x1aBCG/@\xd2\x1b\x07\xed\xfd\xc3\xa6\xab\
-\xe6h\xb6\xf0)\x93\xc9\xcc\xc4b\xb1\xa4eY\xa8V\
-\xab\xfbV\x0c\xc2\xc0\x0b\xbf\xdfO\xfc\x07\xb1\xba\xba:\
-Kr\x97N+\x0a\x86\x16\x17[\x0a\x9cO\xa7\xd3\xc9\
-f\x88\x92\xb2\x03\xb5\xae\xc3\xc3y\xe0\x17\x05\x04\x09\xc4\
-+\x89\x1b\xfdc\xa9\xd1\xe9\xfe|>w(\xc4-\xa5\
-\x02U\xd7\xc1\x13p{V\x88@\x04x\x1f\x87\x1eY\
-\x8eD\x14e\xaa\x08<=\x04\xe2?\xef\x16\xd5\xf0/\
-\xc9E\xec0\xcc\x99\xc8\xf8\xf8u\x19x\xc8\x1e:\x85\
-\xbf\x130\xb1\xa7.a}\x83\xc3\xa3\xf9\xf9\xe4\xd5\xee\
-\xee'\xb7m{\xf6\xc8\x10\xebm\x12\xf6\xb8E\xdc\xb9\
-\x96@<\x1e\x9f\x90\xea\xf5\xe7#\xc02\xeb$;A\
-\xd6\x83\x10\x7f\x96Q\xa9\xa9\xe0\xe9\x15\x98\xa5\xf7\xb8\xdc\
-\x97\xc0\xd4\xdb\x0f\xb8pN\xa8.\xaf\x9c\x5c\xce\xb7\xb7\
-\x83\xdd\xdc\xdcD(\x14\x82\xae\xebv+D\x03[\xdb\
-\xdb\xd0\xb5\xcf0\x8d9\x0c\x0e\x0c`\xf2\xcd\x1c\xba{\
-\xc7\xf0\xfd\xd5\x8b|G\x07\x8d\x85r\x19l.\x97C\
-4\x1a\x05\xc7q\x07xPz\x11\x82\xf6\x0e\x83\xc9\x04\
-^N\xce\xa0\xb3\xe7\x1e\xdaN\xf4\x92\x0b\x1e3N\x97\
-kkk\xee\x18y\xf28\xc4p8\xeccY\xd6}\
-,\x1e\x8f\xc7\xb5PZ\x9f\xc4\xad\xbb\xaf\x91\x9d\x18\xc1\
-\xf1\xb3\xa3\xe8<u\x11\x0cKCQ\x14\xbeP(t\
-\x92\xb3\xbb\x843\x8e\x11\x85y\x9e\xbfd\xdbv\xbbi\
-\x92q\xd9\xb6\xdb\x00\xb1\xf1`\xa8\x8f\xfe\xfae\x83\xf9\
-\xb8Qd\xbeQ\x14e\x139\xffe\xd2\xc1\x02\xc9)\
-\xfc\x16`\x00-\xb7L\xed\xde\x12.\xb7\x00\x00\x00\x00\
-IEND\xaeB`\x82\
-\x00\x00\x02Z\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xfcIDATx\xda\xc4\
-S\xbfk\x14A\x18}\xb3;\xfb\xf3\xee\xbc=0\xe6\
-\xce\xe38\x0e\x22),L\xa1\x12\x0e\xed\xd2&'\x04\
-\xb4\xc8\x1f \xfe\x0b\x1a0`0 \xb1\xb11\x85(\
-)RX\x04\x0c\xe9\x0cZ\x88\x82\x98B\x10\xb4\x08\x16\
-\x12\xc2\x81\x09\xf1\xcc\x8f\xbd\xbb\x9d\x99\xdd\xf1\xdb-\xd2\
-\xca\x91\x22\x1f<f\x8ay\x8f\xf7\x1e\xdf0\xad5N\
-3\x06N9\xfc\xf6\xdc\xdc$\x9d\x17\x07\xe4\xb5\xc9\xf9\
-z&\x10+U]\x9d\x9f\x7f>\x08{zv\xf6\xde\
-\x89\x03\xa5\x94\x91P\x0f7\x16\xfa0)\x90\xcd\x81\x84\
-j\x89c\xa0\xe8\x01yG\xc3\xb7\x81\xabu\xc0\x97\xdf\
-\xe0\x1a\x87\xe8\xf7z\x9c\x00)D&\xc0\x14\x09\x5co\
-0\xe4\xe8qJR\x09`\x92z*(\x14\x15\xc5\x80\
-\xd12\xb0\xfd\xf37\xee\xb4Zx\xba\xbc\xecQ\x84k\
-\xdd0\xdc\xe4RJC%\x09\xfe\xfeYB\xb9v\x05\
-\x97.\x8cS\xb3\x0c\x81\xaf\xd19\xea\xa2\x1bv\xa0\xc5\
-\x1e~m\xedC\x88>\xda\xbb\xbb\xf8\xb2\xb2\xf2\xe4r\
-\xabu\x9fD\x0c\xae\x840S\x07\x9b?\xdeck\xe7\
-+\xa6\x9b\x0a\xcd\xd1q\xc8\xd8@\xed\xbc\x8fB\xad\x80\
-R\xae\x81\xa2oP<v\xd2\xc3\xf7\xb5\xb5\xc7\x8d\x89\
-\x89\x87\x5c\x08\x919h\xef\x1c\xa2\xe3J\xbc\xd8\x7f\x89\
-\xd5\x0foP\x1b\xaa\xa3Z\x1aF\xe0\xb9p\xa0a\xca\
-\x08\x8a\x1c\xccLM\xa1V\xa9\xa0\xdcl>b\x8c\xbd\
-\xe32\x8a2\x81J\xfe\x16l\xdb\x85o\xe5P0\xf3\
-\x80\x0e\xd0C\x00\xd7\x0b\xe0\x14\xf3\xf0\xcf\xb9\xd8\xfb\xfc\
-*#\x07cc\x0bD~\xebx\xde\xa7\xd4\x81\x19S\
-\x04\xc7\xf1\x08\x0el\x82\xc9-h\xcd\xd0\x8f4\x8e\x8f\
-%\xdd%\x84\xb4\x10\xdbCx\xb0\xb8\x88\xe1j5\x8c\
-z\xbd\x8f\xdc\xb2\xc0\x8f\x0e\x0el\x93s\xac?\x9b\xf9\
-\xff\x02\xdc\x9c$\x976^ol\x18)9\x1d\x96\x1f\
-\x19\xb9k\xe6r\xf5A\x16)\x0e\xc3\xed\xa4\xdb]\xca\
-\x04\x08\x0e\xa14\xc0\xbf\xa0-A\x87\x10e\x02g\xfe\
-\x1b\xff\x090\x00a\xe3\xce6\x02\xb7\x87\x0e\x00\x00\x00\
-\x00IEND\xaeB`\x82\
-\x00\x00\x02i\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\x0bIDATx\xda\xa4\
-S\xbfk\x14A\x14\xfevow\xcf\x0d\x9c\xa49\xa3\
-\x16\x12\x02\x11\x0b!\xc2\xb4\xdaH\x08\x18\xc1B\x0b\x05\
-ccsb\x95\xc6\xff\xc12\x95\x90\x22V\x0b*\x12\
-\x90\x04,$]\xda\xbb &\xc4\xa8\x84\xa0M\xce\xc4\
-\xc8\xe6.\xb7?gg}on\xef<\x85\xa0\x90\x07\
-\x1fo\xde\xcc\x9bo\xde\xaf1\xf2<\xc7I\xc4\x9ax\
-\xba\x0e\xc30\xc0D\xcd\x95g8;\xf9X\xdb\xc3\xd5\
-j\xdf\x89\xecyR\xabRJO\xa6)\xd28\xd6H\
-\xa2\x08\xd6 \xdb\x99\xeb\x8f\xfa\xeb#\xdf\x87[\xa9\xf4\
-LQ\x80\xc5\x1b\xbcc\x1e\x17\x1a\xbf\x14\xb4ZZ3\
-f\xa6\xcf\x0b\xd2\xb3\x14\xea\xcc\x7f\x11\xb0dR\x22\xee\
-tt\xb8\x87\x87\x19\xeeO_\x10i\x92\xfcAbR\
-\xee\xf3\x84:k\xde\x18\xb05\xb2,\xab3A\x18J\
-\xec\xec\x04\xb8wcL\x93\xe4\x05\x89E\x87\xe2\xe1\xdd\
-+\xe2\xf9\xab\xf7\xfd|\x1f\xdc\x9e\x10A \xc1\x0d\xea\
-\x22\x87\xef'\x88\xa2\x0c\xdb\xdb)\xeeL\x8d\x8b\x17K\
-\xebL\x02\x8b+\xd9j\xa5\xba\xa2=i\xb7S4\xf7\
-\x02\xb4\x83\x10A\x18\x22\xa5\x1aP$\xfa\xacT*\xe1\
-\xeb\xae\x8d\xc9\xabc\xe2\xed\xca\xe6\xac\x95\x90\x83\xe3\x94\
-\xc0\xba'\x072\xc3wSA\x0e9P\xae\x0d\xa5\x88\
-4\xce\xd0I\x94>\x1f\xad\xbax\xb3\xdchP{\xe7\
-\x8c\x91\xda\x12\xe7,\xc8hP\xc3k\xe8\xd6@\xfc]\
-\xd0\xca\xad)\xb1\x1f*\x8c\x9e6\xd1\x5c|\xa7/\xdb\
-\xe5\xb2g\x91sM\xd1\x13\xa6i\xf6\x06J\xdb=\xe1\
-<\xa9\x1b\xf5\x03\xeb\x14*\xc3\xc07\xefu\xf7\xb2\xe3\
-\xe8y\xb0:\x8d\x97\xda)\xdd\xdd\xd0\xb0\xcf]\xd6\xe8\
-O\xe1\xc5\x9bZ\xbb\x06\xe0/x\xfa2~~\xf1\x8e\
->,j\x7f\xe3_\xb3nV/\xc1\xba\xf6\xa4\xae\xa3\
-\xf9\xf1iNm-{\xd9\xde\xc7\xdf\x7f\xa1\x18&\x97\
-\xd3,0T\xeckQ\xfb[\x90\xcd\xcd\xcf\x88\xfc5\
-\xb5\xb6\xb0A[\xe3\xdc\xa8\x02!G\xc0\xb0\x09\x0e\xa1\
-\x5c\xac\x8f\x9bP.NJ\x88\x09\x09\xaf\x8d\x93~\xe7\
-_\x02\x0c\x00\xa0\xa21\xf7\x9c5\x01j\x00\x00\x00\x00\
-IEND\xaeB`\x82\
-\x00\x00\x01\xe3\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\x85IDATx\xdab\
-4.\xdfm\xc6\xc0\xc0\x00\xc2\xa7\xa0\x18\x0e>|\xf8\
-\x00\xc6\xff\x7f~bx\xb7\xa1\x98\x01\x1d\xfc\xff\xff\x9f\
-\x81\x09H\x98\x9f\xe9pI\x00\xd1 \x01d\xcc\xcf\xcf\
-\xcf\xc0\xc1\xc1\xc1\x80\x0f\xb0\x00\x15\x9e6*\xdb\xc5\x08\
-d\xff\x05bq \xff\xe5\xbf\x7f\xff\xc0\x06\x80h\x90\
-!\xbc\xbc\xbc\x0c\x8c\xa6\xe1\x0coO\xaf\xc40\x80\xd1\
-\xb0t'\x8c-\x01\xd4\xe4\x06\xa4w\x015\xbe\x80\x19\
-\x00\xa3al\x90!0\x17\xbe?\xbb\x9a\x81\x05\xc9\xb0\
-\x17 \xcd@\x09w \xbd\x13\xca\xc7\x00\x82\xc6\xa1p\
-CA\x80\x09M\x1ed3H\xb3'\x10K2\x10\x01\
-\x98\xb0\x88\x81\x0c\xd9\x01\xc4D\x19\xc2\x84C\xfc9\xd0\
-\x80\xed@\xda\x9b\x90!\x8c0\x06\x8f\xac\x1e\x83\x84U\
-\x0c\x03\x97\xb4\x0e\x03R\x00J\x01\xb1\x0f\x10o\x01\xf2\
-\x9f\xa1\x07\xec\xfd\xd9\xe1\x08\x03\x90\x0d\x12\xb3\x88b\xe0\
-\x94\xd2\x86)\x04\x19\xe2\x07\xc4\x9b\x80\xf8\x19A\x03`\
-\x80[F\x97A\xd4<\x92\x81CR\x0b\xa4X\x1a(\
-\xe4\x0f\xd4\xb8\x11\xc8~J\x94\x010\x00\xf2\x9200\
-\x11\x01\x0d\x92\x06j\x0c\x04\xe2\xf5@\xfc\x94h\x03`\
-\x00\xe4%`\x1a\x90a\x13\xd7H\x01rY\x81\x86\xec\
-\x7f0'b\x0f\x134 \x99A\x82@\x0cJ\xf8\xdc\
-@\xcc\x07\xc4\x02@,\x04\xc4\x22@,\xf6\xfd\xd9U\
-\x89g\x9b\x1b\xfe\xfe\xfa\xf5\x8b\x0fh\xb3\xfb\xef\xdf\xbf\
-\xbd\xc0y\x81\x81D\xf0\xf3\xf3\x9b\x83\xa2\x91s9\x18\
-\x19\x19\xf7\x82\xa3\x11\x14 \x94\x00\x80\x00\x03\x00\xbd\x03\
-\x05*\xd1F{M\x00\x00\x00\x00IEND\xaeB\
-`\x82\
-\x00\x00\x02\xf9\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\x9bIDATx\xda\x9c\
-S\xdfKSq\x14\xbf\xdf{\xef6\x96n\xfej\xcc\
-9]\xcb\xe6\x8f\x95A\xa8%\x85$\xca$a\x06\x15\
-\xf4\x83 \xb2\x1ez\xecA\xa2\xbf\xa1'{\x0e\xea\xa1\
-\x22\x08\x1f\x1c\x14\x81\xb5\xa0Lt`\xebi\xc5\xe6&\
-\xbai\xba\xe6\xa6\xd9v7w\xb7\xfb\xbd\xb7slW\
-t\xd1K\x07>\x9c\xf3\xfd~\xcf\xe7\x9c\xef9\xdf\xf3\
-%'\xeeM2(\x84\x90r}\x0a\x14bNQ\x94\
-9\xa6$`\xef\xd3,\xf3\xb7\xd8\x01np\xe8\xf1?\
-p\x8d\xa0\x86\xf5-\xdc+\x9d\xed\x13\xbe\xcc\xeek\xac\
-\xd3\xb7^;csfE\xa9\xb6\xf3\xfe\xbbgw\x5c\
-G\xba\x87\xbb\x1a\xaa\xa7\x83\xc9\xd8\xcb\xd9e\xdbJ*\
-\x17\x06\xbf)\x80\xb4sS\xb5\x04\x90\xa1\xfe\x0e\xf3\xf1\
-\xd1\xf3m\x83`k\xa9\xac\x14\xf7f\xe2X\xa2\x01U\
-\x18{=\xef\xfd\xf05\x11\x00{\x87\xc8\x97jio\
-\xb1\x18ZG\x87\xdb\x06\x8b\x92\x8c\x1b\xf9\xf2\xab\xca\xb2\
-B1!\xfa\xac\xa4\xb2b$\x9e\x89\xc2:\xc4\xca\xb2\
-\x8c\x0d\xe9\xbc=\xd0|L\x94dY\xa2\x8a\x04\xa0\xff\
-\x80\x84>\xe8\x8b\x1c\xe4\xe2\x0dz\x01\xd6\xf9\xb5t\xe5\
-!SEao\xd6\x22\x95\x0bB\x9e\x0aB^\x82\x96\
-P\xb1\x08\x01p\xff[t\xb3\x1a\xc8V0{Y\x0c\
-\x10x\xe8\xbe\xfa\xd8\x1b\x09\x80\x03E\xe4D\x9a_\xd9\
-\xd8^\x0b\xc7\x85\xe8\xeaF.\xf5+[\xd8\xce\x8b\x94\
-RI&\x88\xf1\xd9\xd8\x22r\x90\xcbC\xa4\x99\xa3w\
-_\xb1#\x03\x8e\x0e\xa8_\x86lB2#n\xed\xd4\
-LJ\xcf\x8c\xa3\xa10D\x1d\x85\x0b=M\x0e\xe0L\
-\x80=\x83%L\x03\x1c\xcd\xe6\xca\xa6\xf4v\x91\x01r\
-\x1a\x9d\x15|VE\xa50\xbbq\xb4<\xabi\xb5\x18\
-\xd3\x908\x0e\xc36\xad6\xd1\xff\xc4\x1b^\xd2\xf2\x84\
-\xb0\x84\xe1\x09\xcb\xf0\xec^\x90?\xe08\xa21\x19\xb5\
-\x86\x17S\x0bq\xe4 \x97\xab\xe9\xba\x8c\x01\xd67\x05\
-\xb1>\xb1\x95c\xfa;\x1a\x1a)4\x97RE!\x0c\
-\xc6#\x1cdb\xf5:^o2\xe8\xf4\x8f&\x83\xa1\
-@\xecg\x048\x1fq\x04\xd4\xba\x98\xda\xee+\x1a]\
-\xbd\xd3mwv9/\x9d\xb6[z\xda\xcdU\x1e_\
-\x8c\xf3\xf8\x16c\xd7\xfbZ\x1c5\x15\x9a\xc4\x84/\x1a\
-\x8f\x06\xbf\x04\xc5\x1f\xc17\x9b\xfe\xf1\xa2Z\x96:\xc6\
-u\x80\x83\x95\xed.[\x85s\xe80g0\x99\xe0\xb8\
-j\xf5\xe9\x8d\xb3\xd6\x9b\xcf?\xd1\xcc\xfaB68\xb9\
-$\x84\xde\x7f\x07\xbf$ \x85\xe3\xac\x06\xc0n\x1f(\
-a\xf7\x7f\xd4]\x1c;It\xc6s\x8a\x98~\xbb\xe1\
-\x19\xfd\x5c\xda\xc6\x89\xcc\x02r8\xa0D\xfd\x96\xff+\
-\xbf\x05\x18\x00wA~.Fc\xa1t\x00\x00\x00\x00\
-IEND\xaeB`\x82\
-\x00\x00\x02\xad\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02OIDATx\xda\x8c\
-SKk\x13Q\x18=\xf3\xc8d\x82-\xb1B\x22E\
-\x90fa\xa0\x08YX\x17n\xb4\xabV\x10\xb1 X\
-\xd4e7u\xe5Op\xe1\x1f\xf0U\xa9\xba(\xddT\
-\x5c\xc4\x85\xe2Fp\xdd\x08\xc6.\x1a\xa4\xa1\x15j \
-j\x1f\x12mf\x92y\xdd\xcc\xf8}\x93L2\xd9\xf5\
-\x833\xf7y\xcew\xe6~\xf7JK\xd3\x08C\x92\xd0\
-\x8f\xdd\xd4\xa4\xf6\xe3\xc4\xf9\xeb\xd4\xcd\xf4\xa6\x0e'Z\
-\xdf>\xe4\xac-7\xda\x13\x04\xddV\x1d\xd0\xf0\x920\
-\xc5\x9dS{[j\xe1\xeaL\xf6\xd2\xc2\xfdq\x1e\x7f\
-^y\xfa\xbb\xfe\xb1\xf8\x00i\x88\xde\xde\xaf\x84\xc50\
-\xf1\xb3\xe9\xbe@yv~a\xaaZ\xad\x22{\xf7\x05\
-t]C:=\x12.\x1c\x1d\x99\xb0m\x17\x07\xaf\xef\
-!\x9f\xcf\xe3Sq\x95\x05.\x86\x0e:\xfe\xc0\x82\xeb\
-\xbah6\x9b8x|\x13\x9a\xa6\x85\x90e\x19\x9e\xe7\
-\x85k\xc9d2l\xe3\x1c\xb5\xd3\x19\x0c:4\xc8\xe5\
-r0\x0c#\x1c\xd7\xe41X\xb2\xde_\xd7u\x1de\
-[\x83\x99\xca\xe8\x7f2\x93\xf0\xfd\xce\xb0\x03\x16\xe0l\
-\xbc\x91\xc3\xc3\x08\x16\x1f\xaeB\xd0\xbc\xeb\xfbp\x84@\
-yc\x03\x95\xcd\xcd\xd1\xda\xc4\xe5s\xc2\xf3vdv\
-\x10\x81\xc9q\xb8\x84\x80\x88\x82[\x82O\xf6M\xd3\xc4\
-\xa37\xebgin\x86r\xe4eA\x0e\xfa\xa0\x0c\x11\
-\xd9\xb2,\xda\xdc\x82L\xf5U\xe8\x1c\x18z\x22\x81F\
-\xa3\x81\xa5\xb55\xcc\x16\x0a\xcf\xab\x95\xca\xbc*bg\
-\xc0D\xdb\xb6\xd1n\xb7\xe18\x0e\xcc\xa4\xde\x17\x88\xe2\
-\xf6\xdc\x1cl\xda'\xd3\x81\xbe+\x95\x9a\xaa\x10\x03\x01\
-\xce\xcaU\xf0\xc9\xb6DD\x9f.\x0bS\x15\xbee1\
-\x11v\x22)\x0aWD\x19r\xc0Y\x99\xa8\xd0\x22\x87\
-O\xd7\x8d\x1dp)IuHD\xa5\xbe\xeb8\xb2\xea\
-\xc5\x04\xf8v\xca=rX\x15\x11t\x05#\x071\x11\
-\xfe\x92\x80\xa2\xd6L\xe0Ljp\xc1\xe3\xff\xcbU\xe0\
-'\xc2\x0e$Z\xf3\xd9\x0d\xffR\xd0\x15n\x19FB\
-}\xfb\x0b\xb8q\x1a\x18\xd7\xba$%\xe6 \xe1Y\xb8\
-s\xed\x02\xe2\xc1f\xbe\xef\x1e\xee\xed\xe8\x99\x15r\xbb\
-\xcf\x8f)\xf5~\x1f\xa3\xb7Nv3%\xe8\x80\x02\xca\
-\xc0\xb8\x92\x8d\x8c\x05Cmq\xbd\xfe\xf3\xcb\xbf\xfa\x13\
-\xea\x1a\xa1\x00![ka{\xf9U\x09\xc7\x89\xbf\x01\
-\xb6\x99C\x10\xff\x05\x18\x00\xbcv)\xa3\x8f\x8b\x0c\xb4\
-\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02_\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\x01IDATx\xda|\
-\x93\xcfK\x14a\x18\xc7\xbf\xf3#Dl\x88!T\xd4\
-:\x06\xe1R\x07\xf1\xb0\xc5\x0a\xb2\x9d<t\x08\xa2\xbf\
-\xc1S'!\x08TX:t\x0b\x22H\xe8fl\xa7\
-\xe8\x1e\x0b\x8a \xe2Am\xda\xca\x84\x04/\xe2h\xe9\
-\xe6\xba+\xad;\xf3\xbeo\xcf\xf3\xee\xac;\x8d\xdb>\
-\xf0\xec\xfb\xee<\xf3\xfd\xbc\xdf\xe7}\xe75\x1e\xce\xcc\
-\x80\xc30\x8c\xfb4\x0c\xa0s,H)\xb7\xa5\x10P\
-Jaky\x196O8h\x1c\x9c\x9f\x9d\x9d\xabS\
-1\xe0\x94\x12\x82j\xcd\xba\xe7y\x98/\x14&y-\
-\xca\x1f\xfc\xecf&\x03\x93iQ\x1a\x92EA\xa0\xb3\
-^\xab\xe1\xcf\xe9)\xaa\xd5**\x95\x8a\x1e\xdf\xe7r\
-s\xf4\xde=\xd2\xdehZ\xb2\x05\x89\xa30\x18m\xd2\
-\xef%\xcbj\x99\x0eC\x84\x04.\x95Jx\x95\xcf#\
-;<\xfc\xfae>?M\x95g\x1a [\x00\x93\xc5\
-\xa6\xc6\xe0\x02$\x9b\xcd\xeav\x1c\xc7\xc1G\xcf\xfb}\
-\xee \x8c;\x88\x01\xdaA\xd8\x89\x9eR\xbb\xad\x16\xa8\
-\x90l!\x1eI\x08/B\x9a\xb6\x80F\x0b\xa6\x09D\
-+\xb5\x83X\x0d\x80\xd9j!\x068w\xd0\x01b\xd1\
-\x18\xfe\x07\xa0\xf7@\xefC\xc3\xcf\x05\xc8\x93\xcdi\x14\
-O\xbea\xf7\xd6\xafG\xce\xb1\xfbB\xc8\x80Z\xa03\
-O:`Y;H\xf1\xe8\x0bF\xef\x8ebs\xf7\xdd\
-\xb5\x92\xe3SI$Z`\x07tTI\xc8\xe3\xd5)\
-l\x1c\x15\xf9{EY\x94\xa1\xce\xa4!\xbb\xc4\x1a\xfd\
-]\xb7\xcb\xbe\x8f\x9e\xde\xde\x7fNA& \x9f\xf6?\
-\xc3\x1d\xbb\xaaW9\x0c\x0f\x91ypg\x88\xa6C\x8b\
-\x1f\x16`o/-\xe1z:\x8dn\xd7\xb5\xa3\x8d\xd0\
-\xa28d\xe4\xcaml\x14<\x0d\x08\xc6\x81\xad\xb7\xdf\
-\xf7\xc2\xae\xbaO\xb7b\x9d\x9fuS\xf6\xf5\xa7\xd39\
-\x15\x0b\x02(!\xa5\xa2\x8fG\xd1\xe5Rt\xc9\xd4\xc8\
-\x9b\x8c\x1a\xdcI)\xeb\xa9\xbb\xc7\x1a\xd6\xdaM\xc0\xc9\
-\xc1\xc1\xf1\xe5T\xeay\xa7\xbb|\x96\xf2'\xe4J\xad\
-\x1f?\xd5\xd7\x08\x10\xfe\x15`\x00\xefX\x1e\xcd\xe7\xe1\
-\x8b\x7f\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02\xb0\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02RIDATx\xda\x8c\
-R=OSQ\x18~\xee\xe9-\xfdH[\xc2@\xbf\
-\x88\xc4P4\xd2&.n\xc0TY\x1cd\x22,\x0c\
-\x0c&\xc4\xd1\xc9\xcd\xa2\xe8\xe0H\x8c\x89L\x1aI\xba\
-\x95\x1f` &$\x0c\xd5\x85\x06\x16\x13\x89\x0e\xad\x86\
-\x8f\xa6-\xb4\xb7\xb7\xa5\xf7\xde\xfa\xbe\xa7\xbd\xb7*\x89\
-\xf1M\x9e\xbe\xe7\xf6\x9c\xe7y?\x95\x85L\x06l\x8a\
-\xa2\xdc'\x17\xc3\xbf\xed\xa3eYG\x96i\xa2\xdb\xed\
-\xe2\xcb\xde\x1eT>\xb0\x91\x8fo\xae\xaen\x5c\xd2e\
-\x87aY0\xe9\xce\xbe/\x14\x0a\xd8\xdc\xde~\xc8\xb1\
-\x08_\xf9\xbf[\xb3\xb3\x10\xac\xd6\x87b1\xa9\xd3\x91\
-\xb8l\xb5\xa0k\x1a\x1a\x8d\x06\xea\xf5\xba\xf4\xb9\xb5\xb5\
-\x0dzw\x97\xb87\xec\x94T\x93\xc8}SXZ\xd0\
-\xaf\xdb\xe5\x1a$m\x180H\xb8R\xa9\xe0u6\x8b\
-t2\xf9\xe6U6\xfb\x84n^H\x01k  \x98\
-,\xa4\x0c\xae\x88\xa4\xd3iYN0\x18\xc4\x87B\xa1\
-\xeadP)\x97\x11\x1a\x19\xe9\xf7Q\xc1\xe7\x83\x03\x9c\
-S\xca\xc9\xc9IDFG\xafd\x22\x8fT\xae\x13\xb5\
-F\xa9\x95\x8f\x8fa\x1a\x86\x8c\xfd\x83\xce\x0bss\xf8\
-V,\xa2Z\xab\xc9L\xbcn7\x86T\x15\xaa\x10\x1c\
-E\xbe%\xb0\x97SXjj\xda8\x01\xefr9\xa9\
-\xfa\xf3\xf4\x14\xf7ff\xf0\xe9\xf0\x10^\xaf\x17>\x82\
-m\xae\x9e\x80pJ\xd0\x9b\xcd\xc4\xf7\x9d\x9dg\x7f\x0f\
-\x9cGx'\x95\xea\x8d\x94`\xf7\xc4E\xde\xf8]\xa0\
-\xa5\xeb\xa5\xe8\xf4\xf4s\xfex\xb4\xbc\xcc\xdd\xc5\xd2\xfc\
-<\xc6\xa2Q\xe4\xf7\xf7qsb\x02~\xbf\xdfi\xac\
-\x8b\xca \x81A\x0f\xa8\x84\xb7C\x1eO\xe6z\x22q\
-\xf1xe\x05\xedv\x1b\xd7b1\xbc\xdf\xdaB<\x12\
-A(\x10\x80=\x1d\x86,\xa1\xd3\x11\xf6\xbe\x88\xd0\xf0\
-0\xc2\x14\x8d\xd3\xe2\x06\x8d\x11\xe9\xe9\xfa:nOM\
-a<\x1e\xa7\xd9\x8a?\x04\x149\x10C\x18<\x15\xd9\
-D]\x87AQ\xecEz\xb0\xb8\x08\x8bW\x98\xce\xec\
-EoC\xe8\xa37B\x16\xb1K\xd0\xce\xce \x8ev\
-wQ)\x95xm\xd5\xfe28\x91\xa4\xb7\xa3\xf73\
-\xe1\xff\xf9-s\x98\xcb\x01|\xc5|>|^\xadz\
-\x06;= p\xd3\x18*5P\xa5]\xe0)\xf0[\
-\xe60\x97\xa3\xfa\x08\xe1\x8b\x93\x93Z \x95z\x89\xff\
-0K\xd7k\xcc\xe1v\xfc\x12`\x00\x05\xfc+\xe7\xc0\
-x[\xc6\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02+\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xcdIDATx\xdab\
-\xfc\xff\xff?\x03%\x80\x89\x81B\xc0\xd2\x10\xa6\xe3\x0b\
-\xa4\xa5\xc8\xd0\xfb\x0c\xe8\xfa\xcd,\xff\xfe\xfd\x97nX\
-x`\xfa\xdf\x7f\xbf\x89\xd6\xc9\xcc\xc4\xca\xd0\x10\xef\x90\
-\x09v\xc1\xdf\x7f\xff\x98\xfe\xfc\xf9\xc9p\xff\xe6u\x86\
-/\x9f>0\xe8\x98X2\x5c9s\x1c\xac\x10\x1b\x9b\
-\x87O\x80AQ]\x93\x01\xa4\x0fb\xc0\xdf\x7f\xcc\xff\
-\xfe\xfee\xf8\xfc\xf1=\x83\xaa\x9e\x1e\xc3\x8f\x9f_\x18\
-Ttu\xc1\x9a\xb0\xb1o_\xba\xc4\x00R\x0f\xd2\x07\
-6\xe0\xcf\xdf\x7fL\x7f\xff\xfea\xd040f\xf8\xf1\
-\xeb;A\xe7\x83\xd4\x81\xd4\x83\xf4\x81c\x01\xc8`\xfe\
-\xfb\xe7\x0f\xc3\xa5\xd3'\x18\xfe\x00iB\x18\xa4\x0e\xa4\
-\x1e\xa4\x0f\x88A.\xf8\x0bd\xfc\x01\x9a\xfa\x17\xac\x80\
-\x10\x00\xab\x03\xbb\xe0/\xd4\x0b\x7f\xfe\x82]\xa0\xae\xab\
-\xcf\xf0\xed'a/\xecc\xb1ax\xfd\x14d\x19\xd4\
-\x80\xdf /\x00M\xbc~\xf1\x02\x83\x9c\xba:A\x03\
-.>\xfe\xcap\xeb-\x17\xc3g\xd5(\xe3\xdf\x7f!\
-.`\x01\x85*7\x0f\x0f\xc3\x83\xeb\xd7\x194\x811\
-q\x1d\x18\xd2\xe0\x00\x03\xb2\x9b\xf6|fx\xf2\x93\x87\
-\x81\x83\x93\x93\xe1\xc7\xf7\xef\x0cL\xcc\xdf\x19\x5c}t\
-\x19\xe6\xdcv\xb7\xfa\xc5.\x1c\xc3\xf2\xf9\xdb\x0fN\x16\
-&F\x06IYY\x06I\xa8\x1f\xd5\xb4\xb5\xe1\xfe}\
-\xf4\x8d\x93\xc13\xc2\x82\xe1\xc6'\x06\x86\xcf\xd0 :\
-\xf6\x86\x81\xc1!\xcaIj\xc3\xc2#\x05\x8cF\xd2\xac\
-E\xfc\x1c\x0cJ\xb8\x9c\xfcT\xbf\xc4\xf1;\xbf\xaa(\
-\xb2\x98tJ\xa2\xe8\x93yK\x9e\xfc\xe5\x14\xa9d\x04\
-\xf2\xd9\x80X\x10\x94B\x89I\xc6\xbcQ\x8b\xb7\x83h\
-Ff\xd6^.^\xdeE,@\xf6/ ~IT\
-\x1e\xd0\xf4g\xf8\xf9\xfd\xe7\x09 \xf30;7\xcb\x12\
-\x90\x18@\x80\x01\x00\x0f\xe4\xfd\x07\xfe\xffJ\xc1\x00\x00\
-\x00\x00IEND\xaeB`\x82\
-\x00\x00\x05\xc6\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x03iiTXtXML\
-:com.adobe.xmp\x00\x00\
-\x00\x00\x00<?xpacket beg\
-in=\x22\xef\xbb\xbf\x22 id=\x22W5M\
-0MpCehiHzreSzNTc\
-zkc9d\x22?> <x:xmpm\
-eta xmlns:x=\x22ado\
-be:ns:meta/\x22 x:x\
-mptk=\x22Adobe XMP \
-Core 5.0-c060 61\
-.134777, 2010/02\
-/12-17:32:00    \
-    \x22> <rdf:RDF \
-xmlns:rdf=\x22http:\
-//www.w3.org/199\
-9/02/22-rdf-synt\
-ax-ns#\x22> <rdf:De\
-scription rdf:ab\
-out=\x22\x22 xmlns:xmp\
-Rights=\x22http://n\
-s.adobe.com/xap/\
-1.0/rights/\x22 xml\
-ns:xmpMM=\x22http:/\
-/ns.adobe.com/xa\
-p/1.0/mm/\x22 xmlns\
-:stRef=\x22http://n\
-s.adobe.com/xap/\
-1.0/sType/Resour\
-ceRef#\x22 xmlns:xm\
-p=\x22http://ns.ado\
-be.com/xap/1.0/\x22\
- xmpRights:Marke\
-d=\x22False\x22 xmpMM:\
-DocumentID=\x22xmp.\
-did:A383DFD8A324\
-11E0BDD0C34FC039\
-BF22\x22 xmpMM:Inst\
-anceID=\x22xmp.iid:\
-A383DFD7A32411E0\
-BDD0C34FC039BF22\
-\x22 xmp:CreatorToo\
-l=\x22Adobe Photosh\
-op CS3 Windows\x22>\
- <xmpMM:DerivedF\
-rom stRef:instan\
-ceID=\x22uuid:AC1F2\
-E83324ADF11AAB8C\
-5390D85B5B3\x22 stR\
-ef:documentID=\x22u\
-uid:C9D349664A3C\
-DD11B08ABBBCFF17\
-2156\x22/> </rdf:De\
-scription> </rdf\
-:RDF> </x:xmpmet\
-a> <?xpacket end\
-=\x22r\x22?>S\xf3\x1b\x9f\x00\x00\x01\xf3ID\
-ATx\xda\x9cS=O\xdb@\x18~\xee\xce\xb1\xe3\
-\xa0|\xa8\x0dj\xf8(3C\x97N\x1d`\xe8\xc2\xc8\
-\x98\xff\xd0l\x8d2\xf0O\x083\x13?\xa0\xea\xc0\xdc\
-\xa5\x95\xbaU\xeaR\x81DC\xd3\x86\x90\xc4$\xfe\x8c\
-\xcf\xe6\xbd3q\x8a\x98\x82\xa5\xf7\x1e\x9f\xce\xcf\xc7{\
-\xbec\xcdf\xf3\x10\xc0\x06\x9e\xf7\xf4\x8d$I6\xbb\
-\xdd\xee\xc9|>_\x89Y(\x14\xd0j\xb5>(\x01\
-\x16E\x11\xda\xed6lZ(\xf9>\xd6<Oc1\
-\x8e\x01\xc60\x95\x12W\xae\x0b\xa7`\xc2\xb5\x8a(7\
-\x1a\xe8\x9e\x1cCq\x0d)%\xa7\x17l\xce&8*\
-F$M*UU&\x0d&&\xa3[\xf4\xaf\xff@\
-\xca\x18,$\xbd\x19p\xca\xa5\x22Cq\x95\x00\xa3\xc2\
-l\xad\x88\x1f\xbb\xdbH\xd3\x14)-&I\x8a\xdeu\
-\x0f\xbdQ\x04\xb6\xbd\x0e\xc198\x17\x1a=YVd\
-U\xcc\x88\xe3\x98\xabI\xd9t\xf1n\xeb_\xde\xa3\xe3\
-8\xa8\x87\x7f\xf1\xb6\x0ep\xa6;\xc9\xf1\xf7EE\x0b\
-(n\x9e\xc0\x81\x85/F]G\xf3\x83\x00\x97}\x9f\
-\xd2\xbc~\xe4\xacQp\xcc\xcc\xca\xd3\x04\x95Z\x80\xbd\
-\xf7#\xed>\x1c\x8e\xb0\xfb\xc6\xd3\x8e\x9c\x06\xed\xce\x1f\
-R\xd0\xfc\xe2\xac\xbaL\xb0\x10\x18:\x16>}]G\
-\x18\xceq3\xb0\xc1\xe8C!\xfew\x16\x84\x5c\xd7\x9d\
-o=\x12\xd0-X\x15\x81\x9d\xbd*|?\xc0\x0bW\
-\xe4\xcel\x8140\x9e\xe1\xcfK\xb1\x10X\xb6p;\
-\xe6\xf8|nS\x02\x0bHk\x99c\xee\x9a!\xcb\x94\
-0u\x07O[@\xad\x0a~\xb0\x0f\xee\xd3\xcfF\xaa\
-?L\xa8R*\xc9\xb2\x14\xd0H/\xbf\xbe-\x05\xc2\
-0\x14j\xe7\xc5\xc0\xc3\xf7\x8f\xa7(\xbdj\xc0xY\
-\x86\xa8\x95\xc0JV\x16=\x92\xe0S:dw\x01\x1d\
-\xa4\x106i(\x8e\xe2\x1a\xe3\xf1\xd8R\xf1:\x9d\xce\
-JwAq\x14\x97\xd9\xb6\xdd\xa2\xc9\xces\xae\x22\xa5\
-\xb8b\xfa\xc0\xd3\x0eP\x19+\xf2\xe9\xa6ar/\xc0\
-\x00V\x9c\x1c\x9a.}\xcf\x86\x00\x00\x00\x00IEN\
-D\xaeB`\x82\
-\x00\x00\x023\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xd5IDATx\xdab\
-\xfc\xff\xff?\x03%\x80\x89\x81B\xc0\x92\xd2\xf6F\x93\
-\x91\x91q9\x90\xad\x0f\xc4\x17\x81.\x8a\x04\xe2\xeb\x9f\
-/f\xc3\x15\xf1\xeaOe\x00\xaa\xc1\xaa\x8e\xe9\xfb\xf7\
-\xef\xcbu\x95\x98\xf4c=\xb8\x19@4\x88\xff\xf5N\
-?\x8a- >6u?~\xfc``\xf9\xfc\xf9\x93\
-\xbe\xa6<\x1f\xc3\xcf\x9f?\x194\xe5\x99\x18\xf6\x1c\xff\
-\xa4\xcf\xfe\xe5v\x1a\xb2\x01\x7f\xbf\xdcf\xf8\x86E\x1d\
-8\x0c>}\xfap\xf1\xe0\xe9\xe7\x0c \xd3@4\x88\
-\xff\x93Qj\xd6\x9f?\x7ff\x81\xc4@4\x88\x8fM\
-\x1d\x1030\x1a\x87\xee\xd0\xfc\xf7\xef\x1f\xdcoLL\
-L\x91@\xbf^\xe7}\xdd\x01\xb2\x00\xe4\x92Y\x9fE\
-+\x18\x80\xfe\xc5\xaa\x8e\x05(x\xfd\xef\xdf\xbf\x06(\
-!\xfb\xf9 \xc3\x97/_\xe0|F\xd6}\x0c\x7fy\
-\xed1\xd41333\xb0`\x8b\x9a\xcf\x8f6\xa2\xf0\
-\xff1}g\xf8\xfb\xff7\xd0\x15\x7f\x11\x862\xfe\x03\
-\xe2\xbf\x98\xe9\xe0\xcb\xe3\x8d@\xff}B\xc1\xff\xf8]\
-\xa1\xd1\xc8|\x01\x88\xffChFM\xb0kA\xc4\xcb\
-\x1b\xcb\x81x\x19\xd8\x00VVV\x06...\xb8\x81\
-\xbf\x7f\xfff\xf8z\xa9\x91A\xca\xb8s\xb9\xbf\xab\x9c\
-\xbe\xa7\x9d\x0c\xc3\xf6CO\xf47\xee~\x04\x0a\x0f\x03\
-F\xac\xc9\x93\x89\x89\x81\x85\x05l\xb6/0\xf0$A\
-\x0c\x1d\xbf\xe33;KT\xe0j\xca{\xee\x80}\x82\
-5\x0c\x80\x01\xcb\xf0\xeb\xd7/\x90\xb37\x031X\x8c\
-\x83\x83?\xeb\xc0\xa9/\xfa\x16z,\x0c'.\xfd\x01\
-\xf1/^\xdd\x13\xcd\xc0\x8c\xa4\x8f\x11\xea%6 \x06\
-\xf9\x81\x07\x88\x05\x80.\x10\x06b\xb1\xafo/\x5c\xf8\
-\xc5\x1dhp\xf2\x0a\x8b\xd8\xa3g\xbf\xaf^\xdd\x1b_\
-\xfe\xf1\xc5\xf1\xf7\x8ch\x060B3\x183\x16\xcc\x84\
-\x84A\xea~\x83R9#\xa5\xd9\x19 \xc0\x00\x10&\
-\x047G\xd8\x02\xf3\x00\x00\x00\x00IEND\xaeB\
-`\x82\
-\x00\x00\x02\x95\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x027IDATx\xda\x8c\
-S\xcfk\x13Q\x10\xfe\xf6\xedF-&\xa4\x876\xda\
-B\x11\x11Q\xda^\x84B<\xc7\xab\xbdh\xbdx\x90\
-V<\x08\x1e\xfc\x0bl\xa1x\xf0\xe2E\x94\xf6T\xa4\
-\x90\x83\xe8?\x10\x8bB\xa1b\xfcQY\x0d\x0dj\xea\
-\xc5\x16k\x0c\xd9\xa4&aC\xb3\xfb\xe2\xcc\xcb\xbe\xee\
-\x16A\x1c\x98\xcc\xee\xce|\xdf{\xf3\xcd\xc4\x98\x9a\x9d\
-\x05\x9ba\x18\x93\x14\x86\xf0o{)\xa5\xdc\x94\xbe\x8f\
-n\xb7\xab>X\xfa\x81\xe2\xf0\xf2\xdc\xdc\xe2\x1e%;\
-\xecR\xc2\xa7\x9c\xce\xdb\xb6\x8d\xe5\x95\x95\x9b|\x16y\
-I3\x0af\x0b\xdc\x90\x0c\xeat\x94\xef\xb5\xdbp[\
--4\x9bM4\x1a\x0d\x15\x9f\xcd\xcf/R\xdd\x05\xc2\
-\x9d\xd6\x04\x96O\xe0\xc0\x0c\xa6\x16\xf4\x1b3\xcd\xf0\xd2\
-\x9e\x07\x8f\x88\x1d\xc7\xc1\xc3l\x16\x99\xd1\xd1\x85\x07\xd9\
-\xec\x1d\xca\xdcU\x042$\x10\x0c\x16\x8a\x06\x7f\x91d\
-2\x19\xd5N\x22\x91@\xce\xb6k\xfb \x8f\x08\x02'\
-\x1d\x0d|r\xde+\x92\x02\xc5\x8b\xb9s8\x12\x8b\xe1\
-\x90e\xc1\x12\x82\x85\xee\xf1Q\xad\xc6Y>\xb1G[\
-\xb8\xbdv\x0d\xd3gn\xe1\xf1\x97Gx1\xb9\x81\x1f\
-\xf5:J\xa5\x12\x92\xc9$\xaa\xd5*\xd2\xe94\x08c\
-\x84\x1a\x84\x04\xaa\x85W\x97\xbe\xe2\xfc\xd3SX\xa3(\
-\xe9\xca\xc3\xfd\xfd8>1\xa1&\xd3\x1e\x19\x81I5\
-\x84\x11\xfb\x04^\x84@\x8b\x98\xbf\xf2\x0d<\x91\xa8i\
-ML\x8a^\x84@0A\xe0J\x83\xf5\xf2kE\xf2\
-\xa1\xf2\x06\xe9''\xa1\x85\xd5\xd3\x89\x91\x16\x5c\xabq\
-B\xcf\x9d\x5c\xdd`&w\x19\x0b\x1f\xef\xe3\xc6\xf3)\
-\xac_\xfd\x8e\x8a\xeb\xe2]\xb1\x88-\xea\xffm\xa1\xd0\
-k\x81j5\xee`\x0b\x94,N\xff\xc4\xd9\xa5\x146\
-f\xcajlC\xf18\x8e\x8d\x8f+=N\x0c\x0c\xa8\
-5\x8c\xb6`\xed\xee\xec\xe0\xe8\xe0\xe0\x81E\xfa|\xfd\
-\x17x\x81Y\x05\xd1\x93\x97^\xa4>E\xb5\xc0\xcf\xad\
-J\x05bsu\x15\xce\xf66\xaf\xad\x15\xfc\xa9T\x91\
-&\xd3\xef\x82H\xf4w\xaee\x0cc\xf9\x80\xbe\xad|\
->\xb5[\xab\x1d\x0e\x17\x22\x04\x98\x14\xd9-\x12\xd0\xa2\
-\x85\xe2)p-c\x18\xcb\xa7\xf6\x91\xa7~\x97\xcb\xf5\
-\xf8\xd8\xd8=\xfc\x87I\xd7\xad3\x86\xe5\xf8#\xc0\x00\
-C\x847\xef\xe8\xa9\xbf\xc7\x00\x00\x00\x00IEND\
-\xaeB`\x82\
-\x00\x00\x02\xfe\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\xa0IDATx\xda\xa4\
-S\xcfO\x13A\x14~\xb3\xbb\xdd.\xdbm+\x05\x81\
-\x12\xa2h\xb1\xd4`\x83\x881\x1e\x94h4Jb#\
-\x89G\xff\x02\x13\xb9\x98\xe8\xc5\x9b\x89w\x12\x8c'\x0f\
-\x9a\xf8\x07\x18\x88\x88Gc%1$\x9a \xd2\x00E\
-Q\xf9Q\xa1\x14\xbamw\xb7tgg\x9d\x19Z*\
-'\x0fN\xf2\xed\xbc}\xef}\xdf\xbe}\xf3\x06\xb9\xae\
-\x0b\xff\xb3$\xfe\x88\xbf\x06@\x02\x80 \xd27\xd4\x06\
-\x08%\xa8q\x8e\xa2\xa3\x9a\xb7J1\x0d\xaeK\x13\xdd\
-\xdf@\x1c\xba\x11\xc0\xb3\x89=\x81\xbf\xd6\xa0\xda \xdd\
-={\xba\xa3;\x1ain\xd5|^\x1f+\xb0T\xda\
-5\x16\xbee/}\xfe\xb26dZ\xf6S\x9a\xf7\xf6\
-@\x055r(\xa8<\xbc\x95\x88\xf7\x11\x87h\x1b\x99\
-,l\xd4c\x81\xe8\xb1P \xd2\x19\x0a\x8fO\xce\x05\
-w\xf2&\xd4D\xaa\x02nXU\xc4\xe1\xa1\xc1\x93}\
-\x05\xbd\xa8\xe9z\x01&\x9e\xc4\x0f\x94\xf6`$\x0dk\
-9Y\xbbv\xb9\xabo\xfc\xcd\xd7a\xab\xec\xccPw\
-F\xe0Q\xe2$zO\x85\xbb\x0b\x85\xa2f\x18&\xb0\
-\xc6\x8e\xbeLqL&3<%vT\x06\x16\xdb\xb5\
-,-\x1a\x09u3\xce~\x05\xae\x83\xcf\xb7\xb7i\xad\
-z\xbe\xb0\xff\xc5\xb1\xf7\x06'\x0c\xf4\xe6\xa0E]\x87\
-\xf4R\x1eR)\x1dDI\x84`\xb0\xb1\x95qh\xda\
-\xb3\xbd_ \xb8C\x14@u\x1c\x070v@/\x94\
-\xc0\xb4\xca\xd0\x1fS\xe0\xf6\xf5FH-\x9b\xf0\xea\x9d\
-\x09\x82\xe4\x05v\xe8\xb6\x8dU\xc6\xa9\xf7\x80`\x841\
-F\xd6.\x06\xbdX\x06B\x10 Q\x82Gw\x8e\xf0\
-\xf0\xe3\x17\x1b y\xb5\xfd\xea\x08\x92\x10\xe3\xd4\x05\x1c\
-\xbc\x9a\xdb\xb6L\xa3\x22j\xa2\xec\x03\xb1\x9ax\xf3\xfe\
-O\xbe\xcbj\xe3\x81\x86\xda\xe5\x8a\xc98\xcc\xae6\x11\
-O\xaf\xfc\xcam*j\x00d\xc5\xcf\x81\xe8`M=\
-?\xc3\xc1\xec\x9a\x9f!\x9f+f\x19\xa7.\xe0\xe0\xb1\
-\x95\xc5\xe54\xad\xcd\xf0(\x01\xf0x\xfd \xc9j}\
-\x5c\xa9\xcd|\x0c\xd8\x06ckeu\x91q\xea\xbf\xe0\
-\x92L\xc52Gg\x93\xc9`\xcf\xc0\xd5x\x83\xff\x90\
-OR4\xb82\xfc\x9d\x87\xfd\x87\x8f\xf3\xdd\xd4w\x8c\
-\x85\x8fS\xb3\xb8l\x8e\xd2\xb1\xe7\xe7\x8b\xd8\x99#D\
-\x9b&w\x01x.\xde\xf0\xa8\xb1{\xed\xb1\xde\x13-\
-]=Mj0\xd4\xb0G\xdc\xb66\x97\xe6r\xeb\xf3\
-3i\xdb\x9c\x1f\x01;9\xe1V\x96\xf8\xbc\xd4\x04X\
-%M\x14\xcd t\xb6\x81\xd0\x7f\x01P{\x0fU\x0c\
-W\xdb\x96\x01w}\x0e\xc8\xa7\x0f@~lRG\x96\
-b\x8brqM\x80\xf5B\xadB\xfa\xc7\x0d\xa6W\x11\
-\x0cV\x18\xe5\x92?\x02\x0c\x00\xa3\x80,&\x09\xee\xf9\
-\x88\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x01\x8d\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01/IDATx\xda\xa4\
-\x93\xb1N\xc3@\x0c\x86\x9d\xcb\xa5\x055\x0c\x0c \xa0\
-\x8f\xc0#\xb00\xb2\xc0\x86\xc4\xc6\x88\x80\x9d\x95\xbcB\
-\x87\x82\x18\x91\x98:\xc2\x0b\xf0\x10\xbc@\x07\x90h\x14\
-\x05\x84T]\x14\xdb\xc1\xbe\xaa\xac\x97\x12K\xa7\x9c\x94\
-\xff\xffd\x9f\xed\xa8i\x1a\xe8\x12\x06:Ft{\xba\
-\x7f,\xdf\xbd\x7fx?\xb2\xc9\xdb\x8ben\x86\xd9\xe3\
-\xeb=q\xdd\xda\x19\x9b\x04\xb2\xf3\xc3K\xbd[b6\
-\x88\x15\x5c\x8d\xd7Z\x03\xee\xae\x1d\xa8o\x01 \x8e\x99\
-\x08\xca\xb2\x84\x8b\x93~\xd0\xfc\xf0\x5c\x01S\x0f\xd4\xe7\
-\x01Hl\x88\x10\xf2\xfc\x13\x98\x87A\x80\xea\x88vA\
-}K@L\x88P\x14\x85\xff\x11\x0a\xaf\xc3-\x05,\
-3\xa0\x18%\x03\xe7j\xc9\x80\x82\x00\xd5\xa9^}\x0b\
-\x00\x92\xcf I6\xa46\x0e\x02T\xa7z\xf5y@\
-\xad%\x08q0\xd8\xd6\x97\x0d\x02\xbcN\xf4\xf5_\x09\
-HV\xbb\x90\xa6;0\x9a\x84[\x98\xa6 \x99\xbek\
-\x06\xd6\x03~\xe6n\xdd\x9a\x08\x9en\xa6\xad\xe7\xc0\xca\
- \xa9\xcf\xdf\xa7\xf9|vvt0^u\x8e\xbf\x1d\
-\xcc\xfc.\xc8\xe9\xc9\xd9\xd4\x09]\xc1\xaf\xed\xfa\x92M\
-\xae\xa2\xae\xeb\xfc+\xc0\x00\xa2\xb6\xad\x00\x7f!\xda8\
-\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x01\xc2\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01dIDATx\xdab\
-4.\xdfm\xc6\xc0\xc0\x00\xc2\xa7\xfe\xff\xff\x7f\x8a\x01\
-\x09\x00\xf9\x0c\xf8\xc0\xb9.7\x06&\xa0\x22\xf33\x1d\
-.\x09 \x1a(f\x09\xc4\x1a@,\x0e\xc4\xcc\x0cD\
-\x00\x16\xa0\xc6\xd3Fe\xbb\x18\x81\xecK@\xfc\x11\x88\
-\xc5\x80X\x0b\x889\x80\xf8\x0b\x10\xbf\x01\xe2wPq\
-\x03\x90K\x81\xf8\x04\xdc\x00(\xe7\x04\x16\xc3Y\x81\x86\
-\x834\x09@]dx\xbe\xdb=\xc6\xb0t'\x13\xba\
-\x01\xb8\xc0o ~\x0a\xc5\xa0\xf0\xf8eP\xb2\x03\xa4\
-\xf9\x22\x8a\x17\x18\x88\x04@\x03\x8e\x83\x5c\x05\xc4\xef\x91\
-\x03\x97\x85\x08\x8d\x0c\xff\xfe\xfd\x83\xc5\xc8[\xa8w\x88\
-3\x00\xa4\xe9\xcf\x9f?\xc8B\xef\x81X\x17\xc5\x05\xc0\
-\x80\xc1\xaa\x99GV\x8fA\xd84\x9c\x81KZ\x07Y\
-\xf8\x15H\x0a\x88\xd9\x80\xf8\x17H\x80\x09\x97\xed_\x1e\
-_bx\xb8\xae\x1aL\x83\xbc\x00\xc5\x7f\x80\xf8\x0b\x10\
-K\x80\xf8x\x0d\x80\x81\xc7\x1bj\x19\xbe=\xbd\x02\xf6\
-\x0e\x14\xbf\x06ba\xa2\x0d\x80\x19\xf2dc\x1d\xcc\x15\
-o@.\xf8\xfb\xf7/\xf1\x06\x80\x00\xc8\x15\xafO.\
-g\xf8\xfd\xfb\xb7,0`m\x80\x06\xb8\xc0\x0c`\x84\
-\xa6{Vh\xf2\xe5\x06b>h\x0a\x14\x02b\x11h\
-2\x96\xf8x~\xad$\xd0\x00\xa7\xfb\xb3\xc3\xdd\x81\xb4\
-\x17I\x09\x09\x06~~~sP4r.\x07##\
-\xe3^\x10\x9f\x91P\x96%\x04\x00\x02\x0c\x00\xb4\x09\xb6\
-\x061\xc1F\x81\x00\x00\x00\x00IEND\xaeB`\
-\x82\
-\x00\x00\x03=\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\xdfIDATx\xda\xa4\
-SKO\x13Q\x14>3\x9di\xa7C\xa9\xb4\xb4\x05\
-\x0a\xb1\x91\x97\x90\x80\x0bk\x80\xe0k\xe3#\x91\xa8\x09\
-\x1a\x17\xba4q\xeb\x1f0\xc4\x90\xb02\xbap\xe7\xca\
-\x85\xd8\x05&\xc4\x84hLt\xa1i`c\xc0\xc4D\
-j\xa4<Bii\xc5\xd2a\xa63\x9d\xf7xn\xcb\
-\xcb\xb8p\xe1I\xce\xcc\x9d\xf3\x9d\xf3\xdd{\xbe3\x97\
-r\x1c\x07\xfe\xc7\x18\xf2\x18x\xba\x0c\x0c\xcb\x02\xc30\
-@\xbb\x5cQ\x8a\xa2F1<\x8c\xde\xbd\x9b\xf7\x03}\
-\x0e7\x9b\xb6-+g\x9a&\x98\x86q@p\xc8\xae\
-2.g\xbc\xb3\x8d\x0f\xb5F\xb8\xa0\x9fgx\x0a\x83\
-\xa2b\xf6nl\xa9g\xd3\x19\xf9\xaen\xc1\x18\x86f\
-\xfe8A\xd5\x1c\xe7\xaa\xd7\x0d\x13#g\x22\xfde\xc9\
-\x02Kw@\xd4\x8d=\x94?\x1a\xe4\xf8\xbecum\
-3\xc9\xfc\x84dT\xdb\x9e\xd9'pl;J\x835\
-~y0\xda\xbf\xb5\xa9@Y5\xd5t\xae\x9c\xcd\x97\
-T\x81\xe0\xcd\x01\xae\xa13\xeak\xad\xc8\x0c72\xdc\
-\xd4\xff\xea\xfd\xfa\xb8a\xdb\xf3\xd8R\x8e&\x09\xa6\xae\
-\x8f\xc6\x9a\xb8P!'A\xb1$\xab\x1f\x17\xb2\xdf\xb2\
-\x05q\x0c\x89O\x11'k\x12\xdbFl3#BG\
-\xab7Dj,\xd4\xa1J\xa0k\xda\xe9 \xef\x0a\x96\
-wTH\xad\x15\xb3\x86\xae?A\xf6\x04\xc1\x14I\x02\
-\xfcN\x90Xjm;+\xedT \xe4g\x83\xa4\x06\
-\xbdF`\xa8j\x17\xd8\x0e_\xc1\x9e\xb3yA@\xf6\
-\x84\xae\xaa\xf03\x93\x01E\x14A*\x95\xc8)\x13\x1b\
-\x9b%A3-pQ\x14Oj\xd0k\x1a \x93,\
-j\xa6\xa8\xd9Nu\x8d\xa3\x02\x22\x13\x8e\x13\xb5u\x9e\
-\xe12)\x8b\xe2\xa4\x0b\xc7\x5cA@\xd6L\x92w0\
-\x05\xdc\xeds~G\xf3\xd3n\xb7\xa7\xde\xcf\xe9\xc5B\
-\xe9\x0a\x1e\xf9-\xeb\xf1\x108\xbe\xebC\xe1\x88\xbfA\
-\xb0(\xd0\x04U\xc1\x9a%\x02\xd6Z\xd0\xb4O\xeb\xd9\
-b\xaaD\xb1+\xf5\xb1h\x05\x8b\xcf\xe1\xce'UE\
-!\x18\x5c\xb81\x1c\xc7\xf7PS_g\x07\xe6\xc0j\
-\xe6\xd76~\xcf\x1a\xfb\x1a\xe8z\xb2\xb0\xba\xf1Ut\
-s\xe9\xa2\xf7\xc8J\xf3\xf9\x01/\x17\x0e\x5c\xb2L3\
-N\x8e\xba\xaa\xd0\x10\xbfu1\x9e\xae\xd0@\xfbxX\
-^\x5cKc\xcd\xb4\xb97\x05\xecY\xd0\x15e*\xf3\
-\xe6\xc3\x17\x81\xf1,\x17\xbc\x81\xb438(\x05o^\
-\xafG\xf1@b\xdc0/\xd2\xd0\x12\xe6a\xe1\xc5\xeb\
-y]\x96g\xb1\x85\x5c\xf9\xdd\xc3\x9a\x06\xd2\xcb\xdb@\
-GzV\xe8\xe3\xd7*\xfaT\xa5\x97jo\xf7Q\xb1\
-\x98\xdbinql$`9\x16\x02.\x07\xf26\x0a\
-q\xffN<\xf9\xe89)\xfbn\x16\x16')r\x1b\
-\x89\xdahu\xe8a\xca\x1bh\x84pO\x1d\xf8\xa2,\
-\xa5\x8b\x16DN\xdc\x83\xc6\xae\xee\xbf\xaeaq)e\
-\xcf=~p\x98\xc0M\xfeyt/\x99\xe0?n1\
-\x99\xb2I\xe4\xfb-\xc0\x00\x96\x11\xa6p\xd38\xf1\xe0\
-\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02\x90\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x022IDATx\xda\xa4\
-S\xcfk\x13A\x14~3\xd9\xddd\x93mcC\xda\
-b\x8c\xc5\xe6\xa2m@\x94Y/\xfe\x04\x11)\xd1K\
-\x0f\xb5\xa8\xb9\x07/\xd2\x8bw\xff\x03s\xed\xa1\xb7=\
-\x08\xd2S\xbc\x88G\x0f\x22f[0\xa25\x05\xa1j\
-0X\xab\xb1n\x9a\xec\xef\xbeY\xb6e\xa3X\x0f]\
-\xf8\xf8f\xde\xcc\xfb\xde7;o\x88\xef\xfbp\x98O\
-P\x1f5\x81\x10\x02\x5c\xc8\xf7< \x94\xee\xcf\x95t\
-:\xd8\x84\xf3E\xa4\x17\x8e\xe3h\x8em\x83m\x9a\x01\
-\xac~\x1f\x84\x83\xd4\xfb\xdd.\x88\x89\x04\x1f\xb2\x10\xfc\
-\xd3\xa2{\xe8A\x02\xae\xeb\x82\xd5\xeb\x01\xafZ.\xe5\
-\x18\xf2\x02Z+\x0f\x0a\xf8\xfe\x22\xda\xads\x0e\x22\x91\
-9g\x14\xa9s\xbb\x9d\x8e\x03wK\x13\xcc\xb6\xac\x01\
-\x11\x8a\x01v\xe7F\x81/0\x8b\x9f\x0dy~\xa6\xc0\
-\x92\x12\xbd<w}\x92]=\x97+\x96.\x1cg[\
-[&4\x9b\x06\xcc\xcfL\x06\x22~(B\xa6\x1e\xbe\
-\xe6\x95X\xd4V\x8cR\xaa\xa4\xe2\xf2\x91!YI+\
-\xb2\x92\x92\xa5\x94(\xc4\xc4\xbd\xf5\x5cN\x86\xc7\xb5\x86\
-\x8eyU\xda3\x8c\x0aZT\xf9\x1f-\xcf\x9ef\x9c\
-o\xdd,\x9e\xfd\xbdm\xd8\xd3'G\xf2\xad\xf6\xa6\xf9\
-\xb9\xdd\x16\xd77>\x01\xc7\xc7/-x\xb5\xba\x01\xd7\
-.\xa2k\xd3\x5c \xf9\xfb\xcf\xeaxM*\x0a\xff\xe5\
-\x84\x08X63\x9c\x113\xe9,M\xc4\x93{\xf1\x13\
-\xa324\x9e\xaf\xea\x98W\xa5\x9e\xe7\xa9=\xbc.D\
-\x05\xcf\x168)\xcc^\x09\x9c\x1c-\x9d?\xf3\x8b\x8a\
-\xe0N\xe4\x93?G\xb2\xd0\x1a\xca\x82xl\x0c\xf4\xda\
-K\x1d\xabW\xb1\xa0F\xc6\xef=\x05sg\x87\x0b\x0f\
-8\xc1\xb1\x1ee\xb8=\xc7R1\x80\xae\xf6$\xa8,\
-J\x92&a\x8f\x08\xae\xe3\x00\xba\xe0\x02\xaa\xd5X\x06\
-a|\xbaB\xc7\xa6\xc0\xfb\xf6\x1e8\xf3\xee\xf4\xf0*\
-e\x02\xd0Y\xd2\x82d\xf8\xb1\xae\x19o\x96\xc1\xfe\xfa\
-\x16\xc8\xffz\x9d\x8e\x9e\x02\xe1\xd2\x83z\xd0\x22\xdf?\
-T\xbd\xb5\x9a\xe6\xa2\xf8\xfe[\xf8\xa3+\x15\xc4p\x08\
-\x99\x07\xbd\xcd5p\xda\xef\x9a\xd0\xef\xacx+K<\
-\xb3\x88\xd8\x0eaD\x1d\xf0\xb1\x84\x88\x87\x10\xffa\xca\
-A\x98!,r\xd8\xe7\xbc+\xc0\x00\x0d+.?\xd1\
-\xfb\xb1O\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02\xad\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02OIDATx\xda\xa4\
-\x93Kh\x13Q\x18\x85\xcftf\xd2$\x8ey\xb4\xa4\
-E\x85\xc6\x17)\x8a\x0aUD\x17b\xbaq\xe1\xca\x85\
-\x0b\xadAh\x11\xc4\x9dT,R+\xb8\x11AEp\
-\xe5B\x05W\x0d\xb8p\xd7U\xdd$j\xa0h\x1f\xa1\
-\xc1W\xd3'\xc6&i&\xd1\xc4$\xed$\x99\xb9\xde\
-;iF\x13\xb3\xeb\x85\x8f\xf9\xef\xfc\xe7?\xc3\x1d\xce\
-\xe5\x08!\xd8\xca\xe2\xbc\x03\xef\xc1\xf3\x02\x85\xd7_t\
-u\xed\xae68.@\xf16\x1b\xa2\x1f\x0d>\x1fn\
-\xefe\xb5\xd0\xd8L&\xe3\x90$\x1bDQ|\xd6\xed\
-\x16\xbd#\x03\xae\xff\x0c.\xdf\x8d\x19\xc6-\x8dME\
-Q\x90N\xa7(\xb2\xff\xc3l\xcaw\xf5\xde\x02\xd62\
-\xe5:M>\x9fG\x9d\x01!\xdayUU\x17)\xa4\
-\x86C\xd2\x88d.\x8d.\xac\xc8H\xc8\x1bu\x06\xb9\
-\x5c\xf6\xef\xe6\xf8\x85q\xc6bhF&\x9a\xa6\x19\xcc\
-|\xc9\x90\x13}o\xc8\xf4\xe7\x9f\x84\xad\xc9Oi\xb2\
-\xbaV\xd4k\xaag\x0f\xf6/ \x14\x0aE\xe6\xb3\xe7\
-\xe4\x11'*\x95\x8an\xfam9\x87\x91'a<\xbd\
-s\x14=\x07\x1c\xf8\x18\x91\xd1\x7f;\x84]\x9dV\x8c\
-\xbf8\x83\xcd\x99\xea\x11\x14\xa5\x0c\x06\x1b.\x95JX\
-\x8ee\xf1\xf2u\x14\xf7\xaf\x1f\xc6\xc1\xbdVL\x84\x13\
-\xf0\xdd\x0c\xc0\xe54a\xe9{\xd6\xe7\x1b\x0a\xeaz\xc3\
-\x80\x90\x160\x98A\xe6\xd7:B\xd3I\x5c:\xdb\x09\
-\x97]\xc5T$\x81[\x8f&\xf1p\xd0C5\x1c4\
-\x8d\xf3O\x84e\x1f\xad\x83\x86\x01\xcf\x9b\xc1(\x97U\
-\xac&\x8b\xe8\xf1X\xd1f\x13\x11K*\x18\x1d\xfb\x81\
-\xe1+\xfbph\xbf\x1d\xf1\x94Fu\x16\x96\x10?\xa5\
-\xb7f \x98L\x92^\x94J*\x5c\x8eV*\xe2P\
-\xd8 \x88D\xd7\xd1\x7f\xce\x8d\x8e6\x91\x85\x0a5]\
-\xa5\xc2\xd3\x8f\x15\x8c#\x08f\xb3m3]\x22,\x16\
-\x01\xaaF\xa8A\x19\xa7\x8fu@\xb2\xf2\x86\xb0\xa6\x9b\
-\x0b\xdc\xc0\xef\xd4\x14\x9b\xa8\x1ea\xfe\xed5\xd6\x5c\x0a\
-\xcfi4}f\xb4\x9a,p\xef\xd8\x0e\xa7}\x9b\xbe\
-g\xcc\xce\x13]\xc3\xb4\xd5\xe1\x7f\xee\x02\xa5\xbd\xfb\xd4\
-\xe3\x8b;=}C\xe0xw\xd3\x1bC\xd4\x95x\xf4\
-\xd5\x83\xaf\xef\x06\xc7\xe8\x8e\xa5\xa8@3\xa0\xd6\x0c\xac\
-\x14[\xb3X7,\x16\x12\x85\xc2bY\xa6\x06\x9an\
-\xb0\xd5\xeb\xfcG\x80\x01\x00\xa4`\x22K\x8d\x9am\xcc\
-\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x03\x01\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\xa3IDATx\xda\x94\
-SKHTQ\x18\xfe\xeec\xc6\x99\x9a\x11\x0c\x07\x02\
-\x1f\xa05\x9a\x0d\xbeH\xd3QF\x0dF\xd2\xf0\xb5q\
-\x11D\xeb\xa8\x96.JKj\x13\xb6\xad6\x85\x04E\
-\xa5m\x9c\x9c \xccAG\xbbI\x0b\x93\xc8b\x86\x94\
-\xc4\xc8\x071\xe0\x88\xe3xu\xee\xdc{;\xff\x851\
-]\xf4\xfa\xe0\xe7\x9cs\xcf\xff}\xe7?\xdf\xfd\x0f\xd7\
-\xd9\xd9\x09\xc2\x05\x9b\xcf\x189\x0e\xa79\xa0\x11\x7f\x81\
-\x0e\x04\x12I\xbc\x16S\x1f\xfc\xb2\x07\xcdf\x89\xa6-\
-\xde\xeeG\x97\xbf\x85\xc3\x88\xae\xad\xe1D}=\xd4d\
-\x12\x91\xe5e\x08\xa2\x08\x93\xc9\x04\x93\xd9\x8c\xb7w.\
-\xa5\xe9:D\xc1\xe5r\x19\x021\xfd\x00V4\x07\xd2\
-\xb4-\xd3\xd2\xe4S\xd9|\xf8xyym-\xc6}\
->\xe4\x15\x16\x22\x11\x8f#\xb2\xb4\x04e{\x1b\xaa\xa2\
- \xb7\xb2\xe9\xe4\xd7\xe9\xc06U\x90\xcf\xa2\x8a\x85\xfd\
-\x87\x96\x09\x8b\x9e]\xe4\xc8\xcd\xae-\xae\xa8@px\
-\x18\x95\x1e\x8f1z\x9a\x9a\x90d\xc4X4\x0aeg\
-\x07\xeb\xab\x8b\x91xB?(\xaa\xaa\xea\xee\xea\xea\xba\
-\xeap8\x5c\x91\xd0\x04\xe4/\x01T\xd7\xd5c\xa0\xbf\
-\x1f-\x1d\x1d\x18\xf5\xfbq\xaa\xb1\x11\xd2\xc8\x08\xca\x98\
-\xa8\xa6\xaa\xfa\xa7\xf7\xef\xa2\xf3\xd3c\x9f\x05\x1e\xafx\
-M\xd3\xd2\xe3\xf1\xb8kaa\x01\xb3\xfe{\xa8\xa8v\
-\xc3\xf7|\x10\xb25\x0b\x0f\x1f\xdcG]C\x03\x82\x81\
-\x00\x8aKK!\x05\x83\x18\x0dNqw\x07\xc7\xc7\xb6\
-\x14\xfd\x9c\xaa\xe1\xb1\xc8L\xd1\xbc^\xaf\xe1\xc3\xbcM\
-\x86o\xa0\x0f5g\xaf\xc0Y\xd3\x8e\xb04\x84\xe1'\
-\xb7\xd0\xda\xd6\x867\x13\x138T\xd6\x8e\x1a\xa7\x1b\xd2\
-\xfa\xed\xb1\x8f\xc0J\xf6N\x08b2\x99\xe4X\x15\xd0\
-\x99\xa5\xf9U-F\x10\xd8\xd5P\xc0Dh\xef\xe5\xb3\
->\xe45\x9cG\xfa\x91*#\x8f8\x94\xb3(\x14\x18\
-\x02<%\xbb_\x1c\xc3T[\x08\x92$!##\x03\
-\x16\x8b\x05f\xf6\xbb\x8eV\xb7\x1a\x91\x02\xcf\xf3$\xc0\
-\xa7\xd6\xbb\x02\x93gfi\x03n\xb7{_\xc3\xd0\xb7\
-\xbd\x10\x04a\xbf\x80\xa2(<%}\xe8\xedAq\xef\
-M\xcc\xcc\xcc\xc0j\xb5\xee\x12dY6\xd6\xa9\xb1\xa4\
-\xa4\x04\xc4\xd9\x15H$\x12\x02UP\xd4}\xdd8\xad\
-\x94\xb9\xfd'P.q\xf6\x0a\x18W\xe8\x19\xca\xc4\x8d\
-\xd6U\x84\xa9\x85Y\xb3\x90\x0f\x84\xd4\xdcf\xb3!'\
-'\xc7\xf0\x808\xb4\xb7\xb1\xb1\xf1\xab\x82k\xcd\xdfA\
-\xd7u:\x9d\xbf=\x9d*\x14\xd9{ \xce\xe6\xe6&\
-\xe6\xe6\xe6 \xb2&2q\xec\x09\xd2#\xf9\x17P.\
-q\x18\xd9A\x16qv\xbb\xfd\x22s6\x0b\xff\x01V\
-q$\x16\x8b\x8d\xb2\xe9\xdaO\x01\x06\x00\x9b\xccJ\x11\
-{\xc3B\xfe\x00\x00\x00\x00IEND\xaeB`\x82\
-\
-\x00\x00\x02^\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\x00IDATx\xda\x8c\
-\x93\xbfk\x14A\x1c\xc5\xdf\xcc\xed]\x90\x035E\x10\
-\xe3\x05\x1b\x03b `\xa3\x11\xd2\x04\x85\x83\x83\x98F\
-\xb0\xb0W\xfc\x1b\x84\x10H#\xd8\xca\xa5\x16\x09\xd8X\
-\xda\xa4\x90\x10$\xa9\x22{\xc5%\x84\xfc*.\x9dd\
-\xef\x12oc\xf6\xf6\x97\xef\xbb\xee,\x9b\xe5\x0a\xbf\xf0\
-\x18fv\xbfo\xdegvV\xbdX\x5c\x84Rj\x1e\
-\xc0m\x0c\xaf\xefa\x18\x1eDa\x88r\xa5\x92,x\
-\xed\x1f\x08v\xb7\xb0\xff\xcb\x87\x15E\x91\xac\xdd\xf9\xbc\
-\xb4\xb4\xe2\x05\x01\x06\x9c\xfb|9\x8ac\xd8\xb6\x8dO\
-kko\xf9\x5cQ\xfb\xc6\xd1\xba\xff\x04z\xf2\x11\xc6\
-~nB\x8b3\xa5b6F4\x88\x06\x03\x0c./\
-\xe1\xba.\xfa\xfd>\xbe./\xaf\xf0\xf93\xf6M\x16\
-\xa3\x8d=\xa4Q\xc0&\x8a\x14\x0a%\xaabY8\xea\
-t\xd0\xda\xdbC\xfb\xf8\x18\xef\x9aM<\xa8\xd5\x9ag\
-\xdd\xee\x07\xf6\xbc\xa6\xee\xe5M,1`i\xcdf\xad\
-5\xc0$\xbf\xb9\xfb\xf3\xd9Y\xd4gf2\xa47q\
-\xbc@\xa4\x85\x22\x92\x0e|\x1f\x94\xb4&\x09\x12\x13\xf2\
-\xff/Rf\xa0\xd2f1\x91\x03\xcc#]+\x971\
-\xc2\xd1q\x1c|\x5c]\xc5\xd3\xa9\xa9f\xdb\xb6_\xee\
-\xb4ZD\xa0A\x86@!\xc5\xc8#\x89\x89T\xa3^\
-\x87|\xa9j\xb5\x8ao\xdb\xdb\xbd\xe4\x0c\xfc\xd4@\xa5\
-\x08R\xf2i\x0d\x12\x0a&\xffv\xd3I\xea\xab\x06|\
-9\x89\x9d\x1a\xa8\x5c\x82\xa2\xc9U\x03\xcf\xcb\x12Hl\
-\xb9Vr7\x8aHy\x93R\xa9\x94\x19\xe8\x83\xf5u\
-\xf4\x1cgD&fW^]\x18$\x9d;\x5c3\x8a\
-\x98\x5cKz\xebO\xb7{\xd7999\xbf>=\xfd\
-\xde0\xde\x1a\x1f\x7f\xfc\xaa\xd1\x983Hi\xee,\x89\
-l\xed\x1b\x04\xea\xcc=<\xfc\x92^\x8e\xa4j\x13\x13\
-1's\x06\xa9h\x22\xebD\xd7\xee\xe9ib\xd0K\
-e\xeaf\xdfu\xbd\x0c\x89\x8a\xe5^\xc8\xd9\xc8\x05\x13\
-\x13J\xb0;\x1b\x1b\xa3\xd6\x90\xdf\xf7F\x11iXE\
-\x17\x17\xe7\x1cF\xff\x0a0\x00/\x1c\x22<\xdf\xc8\x0e\
-%\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02\x03\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xa5IDATx\xda\x94\
-\x92\xcfK\x02A\x14\xc7\xbf\xbb\xab\xd4JA\x04u0\
-(\xf3P'\xeb\xd0\xa1SQ\x9e\xbaU\x84%\x88b\
-\x98\x85Pl?!/y\xf4\xd6\xbdc\x9e\xfc+R\
-\xb1\xab-A\x91E\x1a\x86&t\xe8\xd0\xb6\xe4\x8f\xdd\
-\xb6\x99\x0aA\x1c\xc4\xde\xf2\x19\xde\xf0\x1eo>\xcc\x0e\
-'\x1c\x09\xf8\x09\x0e\xa7d\x9dDgq\x0d\x03\xfb\x8d\
-\xdd\xa0\xcd\x06W$\xb2it\x18\xc2\xa1pA\x00\x85\
-\xfb\x9b\xb1\x99\xcb\xe5\xce\xf2\xf9<(\xc1`\x10O\xe5\
-\x0a\xf3\xe8Q\xab\x08\xf3\x81)ARgSa)\x1c\
-\x0e\xe9__\x86\xa6\xebm\xa1=\x82$$\x08\xa00\
-\x0d\xd6\x03\x01\x14\xcaU\xb6\xc1\x90\x88.\xc9\x9c$\xe9\
-|Saaoo\xbbFN\xa8\xd4\xebm\xa1=B\
-HH\x12@a\x1ax\xfd~\x14^jL\x03\xfb\xb0\
-\x05b\xc8\x9c\x22\xe9\x5cSankk\xf7S\xd3\x0c\
-\xa5Ri\x0b\xed\xe1\x03|\x8a\x00\x0a\xd3`\xcd\xe7C\
-\xb1Tg\xdf\xc1\x88\x88\xde\x8d\xae4Ig\x9b\x0a\xd3\
-^\xef\xa1R\xab\x19o\xaa\xda\x16\xda\xc3{\xf84\x01\
-\xae\x09\x8em\xb0\xe2\xf1\xa0X\xd4\xd8w`\xb7\xa0\xcf\
-\xdb}y\x920f\xc6_\x8d\xc6\x008\x96\x97\x8f/\
-\xe3\xf1h\xb5\xda\xfa\xfb\xb2\x92\x04E\x96\x7f_<\xcf\
-\xe3\xee\xf1\xea\xc3\xfa\x8e{\x03\xc80\x0d\x16\xddn\x94\
-\x8azc\xc0\xed\xaa\x13\xae\xa9\x89\x96\xc1\xe7\xb1Xc\
-\x00z\x1d\x8ehI\x96\x8f5\xadU=\xb5\xb3\x83r\
-&\xf3k\xc0q\xb8\xc9f\xd4\x01\x15\xd9\xe7?\x83~\
-\x82\x15c\x08\xa3\x87\xac\x9d\xc4\x07\x1e\xc8\x17%\xd9\x0b\
-\x1d R\x01\x82\x09\xff\x0b\xaa\xaa|\x0b0\x00@\x99\
-caMt\x03\xde\x00\x00\x00\x00IEND\xaeB\
-`\x82\
-\x00\x00\x03\x0a\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\xacIDATx\xda|\
-SKL\x13Q\x14=of\x0a\xa5tZ\xa4i\xa6\
-\xa5\x09\xa5h\xb0\x01q\x0d.\x5c\xd4\x18\x17\xa8\xedB\
-\x13b\x8cqaR\x97\xee\xdc5)\x0b\xe2B\x13\x12\
-M$\xc4\x15H\xdc\xb0T\x83\x92\x18\xdd\xb8\xaeF\x92\
-Vj\x80bPLKK?\xd3\xcf0S\xef\x1b>\
-\xd6\x1f79yo\xee\xbb\xf7\xbcs\xdf\xbd\xc3\xae\xc4\
-b80\xc6\xd8%Z\xbc\xf8\xb7\xbd1\x0c#M\xf8\
-\xcd)5\x9b\xcd\xc3\x0f\xda\xf7<\x89\xc5\xa6\xd5z\x1d\
-:\xf9\x0f\xce\x12\x89\x04f\x97\x96n\xf3;\x08+\xad\
-\x04\x82\xa1\xebh\x01ct\x83\xdeh\xa0Z\xa9\xa0\x5c\
-.\xa3T*\x99\xeb\xc2\xc4\xc44\x9d\x9f\xab\xa9j_\
-!\x97\x03\x07\xcbf!\x08\xa9\x94\xb9\xd1\x89\x80\xc0D\
-\xc6`\x95$t\xb4\xb5A\x12\x04^\x16\xb6\xb7\xb7\xf1\
-h~\x1e\xa1\xc1\xc1\xc7\xe9d\xf2\xfa\xd7\xf5u\xb0}\
-\x02\xc9\x94A\x01\x96j\x15uE\x11\xb8FQ\x14a\
-\xdd\x97X%5\xa1P\xc8,G\x96e\xbcJ$\xf2\
-\xed[[`\x14\xcf\x0b\xe4\x04\x02a\x8c\x1c=\x8bS\
-S\xfdq\xc6p\x94\xf1\x98H$\x12\xa5\xed&\xe1\x85\
-\x18\x0c\x06]\x84p<\x1e\xbf_,\x16G\xddn\xb7\
-)[\xa22Za\xaa\xb2Z1000:99\
-y1\x9dN\xa7\xb2\xd9\xec'I\xd34\xb7\xc7\xe3\x09\
-P2\x0a\x85\x02\x1c\x0e\x87\xb9\xd6\xa9\x13\xc5b\x09\xdc\
-_\xab\xd5@qp\xb9\x5cp:\x1dX^^\x81\xdd\
-.\x07x.'P|>\x9f?\x9f\xcf\x83\x18\x89\xc0\
-\x89\xb5\xb5\x0d\xa8j\x15\xbfZ,\xc2b\x11\x89\xc40\
-cj\xb5]tv\x1e\xf3\xf3\x5c\xa9\xd1hx\x88\xa0\
-\xb7Bm\xcb\xd1\xcbvw{`\x18\x12\xc9\x95\xff\xaa\
-_\xa0'.\x0f\x8f\xe3\xd9\xd0gD\xaa}\xbd<W\
-\x22\xa9n\x92\xdc\xcf\x93\xb9\x0a\x9e\xdc\xd1!\xff\xf7\x11\
-s6/\xca\xaf\xbd\xf8\xd2\x95\xef\xe7\xb9\x9c\xc0j\xb3\
-\xd9I\x16\xb5b,\x0c\xbf\xff$\x91\xf0)\xdc\xeb\xc6\
-\xdb\x8a\x17\xf5N\xe5\x90\xa0\xbdQ\xc7Xx\x18\xcf\x17\
->\xa2\x1a8\x7fFRU\xd5\xa2i\x0c6\x9bL\x03\
-\xf3\xc3D\xab}\xf3^\xc5\xad\xe8(\x92E\xa0\xb4\xbb\
-\xe7{\x9f\x05\x82\x17N#\xb5\x9a9\xcb\x9cN\xe7\x1d\
-j\x91\x9b\x1f\xec\xec\xec\x88\x99L\xe6\xee\x8dYRs\
-\x8anc+\x98y\x97B\xae\xd8EmlC\xc0\xe3\
-\xc4rz}\xebx\xf4\xa6\xb2:3\xf7\xbd\x91\x5c|\
-\xc9\xf3x\xc1=\x1c\xca\xc8\xc8D\xf3\x0f\xd3\xa9\x1e\x0e\
-M\xd7\x9b\x1a\xad\x8e\xf1\x99M\xf9\xda\xdc\x07{\xf8\x01\
-\xff\xb9d>\x89%\x8evEA\xa5\x5c\xde\xb0\x0f\x0d\
-\xdd;j\x12w}\x97CM\xfb\x89\x87\x96&\x9e\xf2\
-\xef\x9f\x02\x0c\x00`\xb3o\x8c\xe2\xe0=\xdc\x00\x00\x00\
-\x00IEND\xaeB`\x82\
-\x00\x00\x02h\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\x0aIDATx\xda\xa4\
-S;o\x13A\x10\x9e\xbd\xdb\x9c\xef\xec\x84G\x91&\
-(\x91\xf9\x01\xa6#\x15\xb2@\x0a\x14\x01\x81\xe8\x82\x10\
-\xc9O\x88\x04U\x1a$h\x10\x05\x91\xf2\x03(\x12S\
-\xa4\x22\xa2H\x0a\x08\x02\xae\xb2\xa0\xc3%M$dL\
-\x04\x81\xc8\xce=v\xd7\xbb\xcb\xcc\xd9\x17\xc5\x81\x02+\
-+\x8d\xe6\xb1\xdf|\xbb3\xb3\xcb\xac\xb5p\x92\xc5/\
-.m\x93\xbe\x8a<\xe3\xc3$2\x06?P\xbd\xe1\xae\
-\x93\xf9\x93[K\xd5\xc5\xae\xb1\xe2\xbfNuXa\xf6\
-I\xb8\x92\xd9^\x8f P\xda\xa6\x9fw~\x7f}\xf6\
-\xaa\xd1\xc8\x81\xab\x8b\xd5Y\xd2\x0b+\xe1V\x1e{p\
-\xabR\xb9P>;\x89y\x01\xf9\xce\x88c\x01%\xc0\
-\x9b\x8c<\xddh|4\x16\x1e\x91t\x0d$\xd8\x1fC\
-Bv\x1e'\x0ca)\x87r\xb9\xcb\xb2zv\xef.\
-\x87/\xd1\x0e\xa9\xa7\xa9fD\x1e\x19c\x0d\x19R\xb3\
-\x88\xb4\xefZ \x0cb=\xee\xc0.ay\xfff5\
-J\xa1yH\xc30!\x8bE\x892B*\x93\xa2\x9f\
-\x118xR\xc1\xb5u\xc4\xd6\xf3\xd9\xf1\xe3\x0d\x8a\xe4\
-\xa1\xa9Z\xfbI\x0bY\xad6\xa0\xf2\xbdB0\x88w\
-\x8e:i\x97\x0d\xeeYF\x05:Gq\xc70\xc0\xbf\
-4\x7f\xc1h\xe0\xc1\xe9\x92\x0f\x9aq\x1c\xd1\xe1\x9e\x8f\
-\xe2\xf6\xc6f\xfd<H\xe5y\x18M\x85\x82V}\xbd\
-WB,\xbap\x90\xb4\xe1\xccX\x91\x9e\x08\x8c\x15=\
-\x0a\x97\x80\xd9\x8c\x00\xbb]\x22\xdd\x89e\xd6\xa9\x9f{\
-\x09$BB\xf3}m\xb0\x07\x9dX\xe0D\x18\x9dX\
->U\xf4J\x0c\x18g}\x82v,\xcb\x07\x89\xdc\xa1\
-\xa7\x9f\x0a\xf9\xef\x1e\xf4\xd7\xed\xfdH\xde\xb8\x5c\x99\x18\
-M\xa4\x16\xb1\xd2\x82l\x8a\xd1\xde_\xaf\x12\x19g\x8c\
-1WP\xbf\x93Rn\xbb\xae;\xf5\xfa\xf1\xf5\xb9X\
-\xea\x04K\x8b\x09tszjz\xee\xd2\xf9\xe2\xb5\x87\
-\x9b\xebZ\xeb\xc1?11\xbf\xb6\xdc\x5c\xbdW=\xb7\
-P\x0b\xd1\xff>\xcc\x87\xfa\xb66\xff\x82+\xa5\xde\x8e\
-\xdfy\xee[\xd1\xfe\xb0\xb7q\xff\xd3\x90\xbf\xb9\xf3G\
-\x80\x01\x00\xd0*\xf6-\x03e\x5c\xa6\x00\x00\x00\x00I\
-END\xaeB`\x82\
-\x00\x00\x02\xbb\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02]IDATx\xda|\
-SMh\x13A\x18}\x9b\x84\x0d\xd4\xd4\xc4\xa4\xda6\
-`h@\x8bM5\x0a\xa9^,=\x88H1\xe2\xa1\
-'\x05A\x8b\xd2^\xa4\xea\xcd\x83\xa0\x07\x0f\xeaE\xaf\
-\x82X<)\x22zR\x14\xc4\x82\x97Z\x9b\x05c\xad\
-\x16\xb5M,6\xc56\x0d.i\xba\xb3\xff~\xb3\xf9\
-\xb1m\xaa\x0f\xde~\xdf\xbc\x99y3\xf3\xed\x8c \xdc\
-x\x8b5\x10\x84\xe3\xf4\xbd\x83z\x5c\xb4\xdb\xfa\x92\x14\
-\x13D\x09\xb6=\x88\x92\x05\x0f\x0cs\xfd\xc0\xa1\xfd\xf1\
-][#\xad\xcd\xbe\xaa0;\xffky\xfc\xe3\xd4\x10\
-t;p\xeeh\x7f\xe2\xde\x8ba\xc0\xb4\x9d>\xcf\xe9\
-\xd7\xf7\xf1\xa0\xe7\xd4j\x83\xb6M\xa2\xc7\x97\xc9dj\
-\xc2\x9c~\xd3g7\x8duC\xb5>\xc9\xa6\x0c\x8a\x5c\
-N\xc1\x86$\x8cP\x96\x8e\xec\xc1\xa5\x13\xd7\xab\xe3\xbf\
-u\xf7\x1c\xd8Q,\x16k\x06\xd3\xa5~t%\x9b\xeb\
-\xce4\xf2\xf4\x8d\xe4>CI\x8b\xbc\x80}?&\xf0\
-j\xe7A\xc00\xce\xb7no\x0d1U\x85eY\x0e\
-\x99:\x85\xcf\xef>\xb0\xecd:\xed\xebh\x0c\xbf\x7f\
-4*e'f\xe6\xe9\x18\x92\xab\xea\xb6\xf7\xe7$n\
-?\xb9\x06(\xcc\xd2t\x1d\xfa*F\xb6\x5c\x810s\
-9\x0b\xc5B\xc1,\x80G\x18v\x17\x1da\xd0E\xa5\
-\xe8%\xa68\xe3\xb9/\xa9\x93\xe3\xcf\xfc\xdcP\x14\xc5\
-\x1a\x1d\x94V\xacmL\x95r\xb7\xbeJ<v\x8a\x0a\
-:\xfd*<\x060\xb0;y,\xda\x12\x8b\x05\x9d\x82\
--\xb9\xa1?\x1cv\xe6L\x94f~\xcb-\xe5\xf9\xb1\
-p.\xd0\x11\xd7\x13\x95\x0d\xf3\xd8k\xdb\xc6K\x8f\x06\
-D|\x0bZp\xf1\xf9c\xa7\xe7H\x85\x1cw\xfb\xb2\
-\xd3\xe2\x85\xc3\x89h4J\xad\xf6\x001\xcc\xf5l\xee\
-{a4=2@\xa9c\x00\x8d1h0\xea\xaa\xac\
-\x91\xe4\xa1\x22\xe6\xf3y\xc8\xb2\x5c\xd3\xfd\xfe@Pc\
-\x888\xf7\x80\xd1\x87\x91\x01C\xdd\x85\x82J\x06\xa2a\
-\xd0\x8f)\xb3\x0a\x9ek\xac\x9c;\x06\x9a\xa2l\xb8\x03\
-FR\x83iB\xd7t\x98\xe6\xdf\x05x\x9b)\x15\x03\
-\x1e-\x97\x0b\xeeP\xa0\xde@_,\xaf\xa6kkv\
-\xc0\xdbl\xa5b0F\x17qn6\x8d\x8dP\xa0\x02\
-5Q\x0d\x04A\x80\xd7\xeb]\xf5\xde\x04(\xcb\x95\x9c\
-\xd8@l$\xba\xd7\xcdo\xdc|\x08W]!\xb4o\
-dn-!M<+\xe0\xff\x08\xffC\xe7\x05\xe1\x8f\
-e\xe5\x8f\x00\x03\x00F\xb8\x1d7\x90|\x0e\x07\x00\x00\
-\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02o\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\x11IDATx\xda\x8c\
-SKk\x13Q\x18=w\xe6fJ\x9b\xb6N\x1e\xcd\
-\xc4\x075\x1a#\x8aP\x84\xec\xa5\xa0\xfe\x06\xd7A\x85\
-\x8a\x0b\x17\x05\xd1\x85\xcb\xaa\x0bK\x17E\x10\x04\x05q\
-\xdb\x8d\xaeDA\x10\x05-\x88 jK\xa4$i\xa7\
-\x09IM(\x1d\x9a\xc7Lf>\xef$\x99\x10\xb5I\
-\xbd\xcc\xe1\xbb\xdf\xeb\xcc\xb9\xf3\xddaoS\x1c`\xad\
-g\x06@\x1c\xed\xb5F\xc0\xa3J\x95\x10\x1aa(\xf7\
-\xb1$\x8a\xb8[-\x9a]\xe7\xc4\xb9[\xcffm\xcb\
-\xc2\x87\xf9\xcb\xf3\x8c\xe1\xbf\x16\x17$\xd7@\x88\x17\x0c\
-\xba\xb8\x91NcB\xd3\xe0\x00\xd3\x12\xe1\x81\xc8\xa9\x82\
-x{\x80]\xe3\x8d&\xce\x5c\xb8\xfd\xf4z\xfa\xf5s\
-D''a\xd5j\x88\x9e=\x9f\x8cO_J\x16\xb2\
-Y\x1c\x8c\xc5\xb0\x97=\x92H\xe0\xcd\xbd\xd4Ci\xd7\
-\x22\xffN\xb1\x88\x9c^F>\x93\x81c\xdb\xa8\x1a\x06\
-*\x9b\x9b\x18\xf2\xf9\xfaZ\xb7\xc7\xed\xe5;u\xd2\x97\
-\x16n\xbe\x08\x8e\xb0)\xed\xf0\x95\x98)\x14\xe4\xbe}\
-\xca~Y\xfe\xf8u\xdf\xf3K\xd0y\xd3\xc1\x1d\xd7\xc9\
-W\xe8Ia}=\x15\x08\x061$\xe3\x95\x08\xcd\xd4\
-,\x1aH0\xecc\xe0~\x85\xc1\xaf\x08o\x14\xf6D\
-4\x8a\x86P`\x13\xe4\xc8(C\xd1\x00\xea\xcd\xc1$\
-\x5c\xdf\xea\x16(\xa7u\x1d\x07T\x15BUk\xbc!\
-?\xc3\xaf]\xa01\x80\x84\xc7\xb4\xee\xc0Y8\x12i\
-+p {\xc1\xc00C\xa5\x0a\x98\xf6\xde$|u\
-\xc3\xf1\xf6\xf2T>\x8f\xb1\xf1qq\x04\x92{\x8b\x16\
-\x97\x09?J\x7f\x12$B\x0c\xa7\xc2\x04~\xfcPW\
-\x01\x0f\x85\xc3\xa8\xb7\x15p/x\xf7\x1dae\xeb\xdf\
-\xb7\xff,\x93\x00 \xcd\xbet\xf0=C.\xa4\x92\x98\
-\xad\xe380\x9bP\x040\xd7\xa7\xb9wI%\x13X\
-\xca\x01Q\x0d\x01M\x5ccEQ`\x984v\xff=\
-au\x9ff\xef?:\xea~\xf0\xabI\xdc8\xa6\xe2\
-\xa4\x1b\xcclc\xe5\xf1g\xcc\x89\xad%`v\xac\x07\
-\xa1\x0d\xb6\x80\xe3\x11\xa8\xee\x9d\xe8\x10R'\xe1\xc1\xee\
-)\xb6\xff\xca\xb5\xe4\xfd\x16`\x00\x1d\xfa\x0d\xd8wp\
-b\xe0\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02U\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xf7IDATx\xdab\
-\xfc\xff\xff?\x03%\x80\x89\x81B\xc0R]]-\xc8\
-\xc4\xc4\xe4\x0cd\x0b\x03\xf1\xdb\x7f\xff\xfe\xed\xfd\xfb\xf7\
-\xef\xfb{\xf7\xee1\x80\x5c\x07\xc2&\x1a\xd7\xc1\x18\x04\
-fm\x0aa\xf0\xb8v\xcd\xd2\xf1\xda\xb5\xb2\x17\x0c\x0c\
-\x13\x99^\xbf~\xed\xe6\xe7\xe7\x97\xd2\xd8\xd88\x03D\
-\x83\xf8O\x9e<\xc1i#\xd0@\x95K\xbc\xbc\xce\x8a\
-\xf5\xf5\x01\xaf\x19\x18\x1aY\x1e<x \xa1\xa1\xa1\xe1\
-\xfe\xf5\xebW\x06\x10\x0d\xe4o\xe7\xe7\xe7O\x83\xaa\x7f\
-\x0e\xc4\x9b\x11\x9a\x19\xec\xbf}\xfb\xa6\xdb\xb1\x7f\x7f\xb3\
-\xbb\xb2r\x7f\xe4\xff\xff;\x98\x80\x1a\xde\xaf]\xbbv\
-\xdf\xa7O\x9f\x18@4\x88\x0fd\xcf\x02ze\xd6\xef\
-\xdf\xbf%\xff\xfc\xf9\x03v>X\xf3W\x86\xb2\xb5s\
-\xf4'kkk\xd7\x9d\xf9\xf1c\xc1_\x06\x86],\
-/_\xbe\xdc\x96\x93\x93\xc3\x0c\xb4`\x17\x10\xbfbf\
-f\xde\x06\xf4\x06\x83\x85\x85\x05\xd8V+\xbd\xbbp\xcd\
-\xee\xfe\x15^\xf3ft\xec\xd7V`?r\xe8,\xfb\
-%p \x02\x03\xec\x0d\xd0\xa6\xf9\xc8\xfe\x94\x92\x92b\
-\xf8\xf1\xe3\x07\x83\xb4\xc0\xc7}\x16:wP4\x7f\xf9\
-\xf2\xbf\xed\xdf?\x86\xfd\xf0X\xc0\x16P\x8d\xe17\x80\
-\xe4\x0d\x86\x7f\xff\x19\x98\xbe}eD\xd7\xbc\x07%\x1a\
-\xd15\xbb\x18\xfe`x\xff\x19\xc2\xfe\xf9\x9b12\xaf\
-\xec\x86\xd7\xb4.\x0d\xac\x9a\xe1\x06\x80\xe2\x1a\x18h`\
-\x81\x8dG\xfe\x021<\xdc\x1b\xae?\xd2X\xc3/\xc0\
-0I@\x90\xe106\xd72\xa2\x0b\xf0\xf0\xf0\x801\
-\xd8\x05?\x7fJ9\xea\x7f}\xa6*\xff\x9bA@\xf0\
-?\xc3\xde\x13\x0c\x0c{N\x10\x91<\xf9\xf8\xf8\x18\x04\
-\x05\x05A8\x0dD;\x98\xb0\x92\x9e\xc6\xd9\xd9\xd9\x19\
-899\xa5\xd8\xd8\xd8\xf0\xaacF\xf2\x0a;\x10s\
-\x031/\x10\xf3\x03\xc3\x85\x11\x88\x83\x81\xd1|\x0dH\
-s#\xa9\xfd\x8f-\x0c@4\x1b\xd4\x10\x10\xcd\x0a\x15\
-\x03&6\x86?P\xfc\x1b\x8a\xff \x1b\x02\x10`\x00\
-\xc8\x1f\xfcq|\xf3>4\x00\x00\x00\x00IEND\
-\xaeB`\x82\
-\x00\x00\x01\xb2\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01TIDATx\xda\xa4\
-\x93\xbfJ\xc3P\x14\xc6On\x12\xa1\x18D\xc7*\x1d\
-\x04\xb5\x94\x98*\xe8\x22.\x8e.\x8e\x82\x9b\xb3Oa\
-^B\x9c]]}\x017\x05\x8bC\x08\x04qP\x17\
-\x87:\xd8\xda\x12\x13s\xcf\x8d\xf7\x9c\x06]\x22i\xed\
-\x85\xc3\xfd\x86\xdfw8\xdf\xfdc\xe4y\x0e\xd3,\x01\
-S.\xe3\xf4\xd0=\xd0\xfb\xe2?\xbc\xaf\xfeexe\
-)\x95/\xf9\x17\xd7\xe7\xa8\xb2\xb1\x9d\xa6\xb0\xc1?\xde\
-;!m\xa1RB\xca\x14\x9e\x1e\x22\x18~\xf4`}\
-{\x07\xc2\xce\x0d\x83e\xda\x99\x9b\x87\xe5f\x0b\xc87\
-j\x80\xcaT\x880\xe8\xbf\xc3j\xbb\x0dI:\x84\x15\
-\xcfcS\x99~\x0c\x02 \x9e|\xdc@\xa2\x12\x88\x12\
-Z\x9b[\x90|}V\x8eO\x1c\xf1\xe4\xe3[\xd0\xc2\
-D)!\xb8\xbb\x05\xa9\xf7\xaa\x22\x8ex\xf9;\x01\x9a\
-RwD=\x16\x01U\x8b9\x9e\x00\x8b\x06\x12y\x82\
-\xa6\xb7\x01qZ\x1d\x818\x9e@\x8e\x1a\x88\x8c\x22\xe8\
-\x8e\xe1}g\xac\x08\xc4\x11\x9f\x15\x11\xf4\x15\xa2E\xa7\
-:\xeb8\xf0\x1cEP\xb3m\xde\xff\xd2\xc4)\x8e\x8b\
-\x16G\x18\xc4I\xcd\x12\x06\xd4\x1b\x0d\xa8\x17\x19\xd7\x5c\
-\xf7'o\x99&\x9e|\xac_\xde\xe2\xee\xd1\xfe\xee\xd9\
-\xa4\xef\xb8\x9f@\x97\xff\x82\xae\x19]\x0b\xf4B'\xf0\
-\xa3\xae\x9e\xfe\xc9\xa91\xedw\xfe\x16`\x00s\x8d\x0e\
-G\x22\xb7Z`\x00\x00\x00\x00IEND\xaeB`\
-\x82\
-\x00\x00\x02\x82\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02$IDATx\xda\x84\
-S\xcfk\x13Q\x10\xfe6\xbb\x89Y\xd2\x92\xdaT\x22\
-\x0dUk{\x11\xc9A\x16\xf4*\x1e<\xe9\xc9\x83G\
-E\x90\x82\xf8'\xe4f\xff\x06A*\x82`z\x10\xb5\
-\x18\x85\x06\xaah\x8f1\xd9\x80H+Z\x11\x0bZ\x12\
-06\xddd\xb3\xbfw\x9d\x09\xd944\xa9~0\xbc\
-7\xf3\xcd|;\xef\xbdY!\x08\x020.>\xaa#\
-\x84 \x08\x0fhQ\xb0\x0f\x95\xf2\x16B\xe7\xfd\xadt\
-\x9f\x90\xc2\x8d\xa9\xeb\x88\xc5\xe3\xa1\xab\x5c\xbf<\xad8\
-N\x00I\x12\xf0tm\xa7_`\x9b&\x06\xd1\x17\xb0\
-\x0c\x03\x9e\xeb\x22\xda\x13\xe9t<h\x9a\x87\xf1q\x11\
-.\xc5\x19\x0e\x15\xbb\x8e3Z\x80\xc1\x02~\xa7\x83\x88\
-$\xc10\x5c\xb4Z\x0eD1\x0a\xc7\xb6\xe1\x13\x17\xf8\
->\x0e\xa2/@g\xec\x9e;\xf0<\xf8d\x96\xe5\xc1\
-4]Z\x05\xb8\x96\xc5)\x95^\x9eJ\xcb\xc2\x90\x00\
-\xb5\xb6B\xa4r\xe3ZV\xd9\xdd\xb5\xd1l\x1ad-\
-2\x07\xd9SqebB\xc6\xdbRM\xa5\x0b^\x19\
-\xec 2\xd0A\x91\xbe\x94{\x98/\xd3\x8d[\xd8\xda\
-\xdaF\xa3\xd1 \xd3 \xcbQ\x14\xd7\x7f\xa8\xccs\xde\
-H\x81P\xc4\xb6\xcc\xdc\xf2\x8b\xaazrv\x0a\x81 \
- 33\x89\xd5w_U\x8e\x1f,\x1e\x12`\xf8\xbe\
-_\xd4\x9b{\xb9g\xcfK\xea\xd1L\x0a/\x0b\x15\x95\
-}\x8ec\x04\xa4QAN6\xdam\x14\xf2o\x16\x85\
-H$'\x8f\x8d\x8d,\xee\x0e]8\x89\xd3wW\xf7\
-\xdb\x12\xc5\xee\xd3\xd94\x1b1YF4\x16\xeb\xbe\x0c\
-\xa3]\xceC+=9\xfc\x08\xbd\xbb\xc8P\xd1R\x22\
-\x99\xac\xf0\xca\xfe\x7f;\xa0\xe7A\xf2\xca\x22\xa2\xc7\xcf\
-\xb2\xbbt\xe1R\xf6\xaa8\x7f:\xad\x7f\xf9^\xff\xb8\
-\xfe\xe9\x15\xc5n;\xb5\x0d\xec\xbd\xce!\xac\x19\xea\x80\
-Ic\xbb\xcac}N\x9b\x9dK\x17j\x02vf\xe6\
-\xd2\xecs\x9c\xf9\x7f\xbd\x02\xefe}\xed^\xcai7\
-7~\x957\xeb\xc7\x8e\x00\xbf\xab\x9bu\xf6)>E\
-|\x82L<\xec\x08L$\xc9R\xc2\xe4\xfc\x89\xc8\xf9\
-;7\x11K\x9c\x81\xad\x7f\xf6?\xdc\x7f\x1c\xfc\xf9\xf6\
-\x93\xb8\x06Y\x93j\xfa\x7f\xd4_\x01\x06\x00zl0\
-\x8b\x82\xa5\xcd\x98\x00\x00\x00\x00IEND\xaeB`\
-\x82\
-\x00\x00\x01\xb3\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01UIDATx\xda\xc4\
-S\xb1n\x830\x10=G\x05\x85\x94f\x02\x86\x8c]\
-\xbaD]\xdb\xff`\xce\xce\xc6\xdc\x091u\xc9\xc2\x10\
-e\xc8\xc4?\xe4#\xe8\xdcJ\x1d*!\xb1\xa1\x0c!\
-\xb4@\x22B\x94\xfaYe !j%\x86\x9etz\
-w\xf6\xbbw6\x9c\xd9\xf1x\xa4.\xd6\xa3\x8e\xd6Y\
-\xe0\xaa\x0e\x1c\xc7!\xc6\xd8-\x0f\x1f\xb8\xdf\x5c\xe0\x7f\
-q\x7f\xe1\xd7\x0e]\xd7m\x0aTU\x05x\xb4m\xfb\
-\xc90\x8cq[\xf5j\xb5z\xf3<\xef\x99\x87\xe1\xd9\
-\x09\xca\xb2\x04\x0c5M\x1b\xff\x885,\x8ec\x1a\x8d\
-Fc\xce\x1b\xb6~\x83\xddn\x07g(>\xf5\xcdf\
-C\xcb\xe5R\xc4\xe0\x80{Q\xe0p8\xd0l6\xa3\
-\xf5zM\xfb\xfd^\xa0\xef\xfb\x94\xe79a\xef7\x81\
-\x1e\x8a\xd0q>\x9fS\x18\x86\x02\x91\x9b\xa6)\x04\xc1\
-i\x15(\x8a\x02.N0\x99L(I\x12Z,\x16\
-\x02\x91+\x8a\x22N\x00\x0e\xb8g\x02\xdb\xed\x16.\x04\
-\x06\x83\x01Y\x96Ei\x9a\x0aD\x8e\xee\xd8\x03\x07\xdc\
-3\x81 \x08\xd0-\x8b\xa2\xe8]\x96e\xd2u\x9d\xa6\
-\xd3\xa9@I\x92\x08k\xd8\x03\x07\xdc\xdaX\xfd\x16\xf8\
-\x10\xe9\xaa\xaa\xde\xf7\xfb\xfd;\x1e_\xb7\xcd\x01\xe7\xe6\
-\xfc\xfe\x1fY\x96\xbd\xf28>\x15@\x11\xfe1\xfb\xc3\
-\x04\x7f\xf2\xba\xac!\xf0o\x8f\xe9[\x80\x01\x00i/\
-\xeea\x09o\xb4\xd2\x00\x00\x00\x00IEND\xaeB\
-`\x82\
-\x00\x00\x02\x18\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xbaIDATx\xda\x8c\
-S?k\xc2P\x10\x7fI^b\x84RP\x84\x12'\
-\x05]\x9aZ\x10\x87b\xd7.\x19\x94\x0e\x9d\xfa\x05\xfa\
-\x15\x84\xd2\xcfP\xbatr*8\x95\x8e\x0e\x82S\x97\
-.\xddD(\x14\x073\x08\xa1`\x03\xc5$\xc6\x9a\xa4\
-w!\x89\x89\xb4\xa9\x07\x8f\xdc\xbd\xbb\xdf\xef]\xee\x0f\
-\xd3\xeat\x08\x0a\xcb\xb2D\xe0\xf9&\xa85\xb2\xa3x\
-\x9e\xd7\xa71\xa3y\xd5n_\x9f5\x1a-\xd0S\x81\
-\xa6m\xcfo\xba\xdd\xdb\xa9\xa6\xf1\xf4{\xb5\x0a\xefk\
-\xcdz\xbd\xf5i\x18\xa9`!\x93!\x0f\x83A\xff]\
-U\x1f)\xcf\xab\xd4Z.#\xe7\x17\xe8\x8b\x7f\x08\xf6\
-\x18\x86<\x0d\x87/\x1c\xc7M\xd6\x8eC\xa8i\x9a\x91\
-s\xed\xbad4\x1e\xfbz.\x97#\x96e\x91r\xb9\
-\x9c \xc0\x988&A\xc0\x02{\xa5RI\x00\xf0n\
-\xdb\xfe\x93\x80\x01\xe7t:\xf5_\xd7u=\x01\xc4\xbb\
-%\xfc\xe2\x91,o\x11@\x9a\xa1p@P\xadV}\
-\xbdP(\xfcZ\x03\x8c\x89c\xa8\x157\xc0\xa9\xaaj\
-\xe2U\xcc\x04\xbf(\x18{\x10\xd4&\xc2\xd8\xb6\xbda\
-\x87a\x0a3\x08\xa5$I\xc9\x0c &\x8e\x89\xcf\x01\
-C\xc1\x895\x88w\xe1\xb0TJ\x10`\x0c`\xa2\xca\
-RoC@\xf1\xffN\xa0Hi\x821\x80\x89&\x98\
-\x12\x1c\x1cQ\xf4\x87\xcc\x80\xea\xba\xd0gl\x15v\x04\
-\xf7\x03u\xdf\x0et$ \x8e#\xf8h\xe8\x0a%X\
-\x10Q\x94\xcf\x15\xe5t4\x99\x10\x9e\xe3p\xa9H\x06\
-\x8f \x1018h\xe3}\x90\xbb\x88`2\x9b\xc1\x8f\
-\xe7\xf3\xb2\xac(w\x1f\xf3\xb9\x0e\xaf{\xa9\x07\xb6\xec\
-\xbe\xd7{f$\xe9\x02H\xf6\x91\x88a\xb2\xd9c\xb6\
-X\xbc\xdcy\x85\x0d\xe3\xcd\xd5\xb4W\x5c\x1d8\x8b\x1f\
-\x01\x06\x00\x7f\x92\xd60_\xf0?_\x00\x00\x00\x00I\
-END\xaeB`\x82\
-\x00\x00\x02\x17\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xb9IDATx\xda\xa4\
-S;K\xc4@\x10\x9el\x12s\x069_\x95(\xca\
-)X\xa8\x8d\x87\x8d\x22d\x9b+\xe4\x0a\x7f\x80\xb5\xd6\
-\x96\xe2/\xb0\xb4\xb6\xb7\xd7B\x10l\x12\xf0\x10\x1b\xc1\
-\x07\xa2\xe2\xa3\x94\x03\xd1\xcb\x9d\x17M\xf6\x928\xb3g\
-\x0e_w\x16\xb70\xcc\xee\xcc7\xdf|\x9b\xcc*q\
-\x1cC;K[\xd9x\x96\x0c\x8a\xa28\xb5\x9a\xe0\x9e\
-\xe7\x81\x10\xe2\x17P\xd7u0M\x134M\xb7\xb1\xa9\
-E\xb1\xad\xb5>E{{\xf3\xb0\x989\xbe\xff\xce\xc3\
-0l\xda\x89H]\xd7\x05UU\xb9a\xa4\x90$B\
-\x92>\xd0\xb0\xa3\x83\xdd9\x02l\xc6\x98\xf5\x9fd\xc4\
-9\xd8\x88\xa3\x0a[^!\x8a\x22^.\xbb\xb4\xb7\x0e\
-6G!\x8cD\xd3b\x95\xe9\x90[\xbd\x97M\xd2\xe9\
-nN\x9e\xb9n\x09*\x95\xb2\xb4@\xbc\xc3\xd9q\x01\
-\xdc\xe7\xa7?=\xe5\x13,\xd5I\x05\xc5b\xb1\xd1!\
-\xc4{\x0ee\xc6\x80\xe9*d&&d,\xf1\x83\x18\
-\xa7|\xb5\xea\xc9s\xe2\x99\xef\x0bHL\x88\x00\xee\xae\
-.!\x08\x82_v\x8fq\xca\x7f\xc5K\x05q\xcc\x1a\
-\x0aj\x08\x18\x18\x1e\x91\x05?\x17\xc5)\xff\x15/\x15\
-\x98f?\xfe\x9a\x944\x02<\xdc\x5c\x83\xffZ\x85\xdb\
-\xf3\xf3o\x9e\xe2\x94O\xb0T'\x15\x18F7\xb2*\
-\xf5\xaf\x0c1\x8cON\xca\xfd_\x9e\xf2\x1d\x1d]\xf2\
-l\x18\xe9:\x01\x0e\x91\x1dy\x0f8D\xe2pa}\
-f\x1eg\xae\xf5\x1cTN\x0b\xaa\xaa\x83\xd29Ms\
-\xc0QA\x97\x95\x1a\xb4\xec\x8b\x83\xa5\xdc\x8d\xbd\xdcK\
-S\xdd\x8a\xa0g`\xeee*\xb7\xfd9\x89\xa8\xe0S\
-\x92\x95\xcd\xef\xec\x97\x1e\x8f\xf8\xc9\xdeb\xd3\xe2l~\
-\x17\x09f\x1boA\xbe\xa1v_#\x836\xd7\x87\x00\
-\x03\x00\x9b/\x02\xcc\xf69c\xa8\x00\x00\x00\x00IE\
-ND\xaeB`\x82\
-\x00\x00\x02\xe4\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\x86IDATx\xdal\
-S\xcdk\x13A\x14\x7f\xbb\xb3\xbbiMT\x92\xfa\x11\
-\xbd\x08\x05k\xacz\x9a\x9c*m\xf0\x10Y/\xc6\xa0\
-\xe0A\xbc\x14\xb5\x87\x9e\x83\x97\x1cs\x08\xf8\x17\xb4\x0a\
-\x0a\x11\x0f\x8a\x94\x5ct\xc1\x83\x89\xa0($\x07\xb1-\
-\x85b\xc1\x8b\x1fmMIbLwg?|o\xcd\
-\xb6\xd1f\xe0\xed\xec\xfb\xbdy\xbf\x99\xf7\xe67\xd2\xa1\
-\xd4m\x90\x19\x03\xa608\x91\xc9\x81$I\xa0\xa8*\
-0\xc6t\x00(\xa0\xe5\x1d\xc71l!\xc0\xf3<\xf8\
-R\xbe\x07\x8e\xed\x80\xeb8\xb0Q\x99\x07e$u\x0b\
-TM\x035\x14\x82\xbe\xa1cR\xe1\xea\x85c\xfc\xf9\
-\xebo\x85\x1ef\xd0'\x9e\x9e\x05a\x9a ,\xcb\x07\
-e\xd8;t\xdc\xadpe*\xce\xdbm\x17h&\x9f\
-\xf0\x01kA\xe9w\xda\xcd&\xac7\x1aY\xfa/\xae\
-\xad\xd5s\xd3\x93\xbcx\xffM\xbd\x17\xce\x1e\x89\xc5\x0c\
-\x0d\xcb\x1bH\x80\xf5\xe9\xaa\xa2d\xf7\x87\xc33\xedN\
-\x87\xa0\x9a\x10^\x10N\x22\x0e\x18\x9f\xc3u\x0bA9\
-\xbb\x04\x98l[\x96_\xeb\x90,\x83<<\x0c\xcdn\
-\x17\x84p\xfc\xf0A\xf45\xc4q\x0dG\x97\xe3\xfa\x9d\
-\x9e\xc8\xb4\xb3\xc0\x1a\xb3\xe9\x04\xa7\xc6`\xf3jL\x92\
-jC\x8a\x02\x9b\x8d&\xd0L>\xe1\x14\xbfx\xfe8\
-\xa7\xf5\x94G\x04\xd2\xe8\xddj\xed\xfa\xe5$o4,\
-\x88FU0\xf1\x8a~\xfe\xfa\x0d\xa6\xb0\xa1\xd9\xda\x86\
-HX\xf3\xaf\x8f6u\xf1\xb3\xbe\xd9\x81S\xa31\xa8\
-VV\xeb\x9f\x8bSIE\x98V\xbe\xf4\xf4m\xe1\xc6\
-\xb5\x09\xfe\xf8\xd9\xbbz\x7f\x83\xce\xa5\xce\xf2\xf7\xd5\xc5\
-\x7f\xb0\xb1\x89\xd3\xfc\x95\xb1XG\xbd\xe4\xfd\x1e \xbb\
-/\x92GO*~\x0fP@I\x9a\xe9\xc8-\xa6\xf9\
-\xf7\xdd\x8f-U>\xfa\xc9(6c\xa7\x89>\xc9_\
-ad\xb7\x91\x8c\xd4H\xeal\xca!_4&\xaa\x8e\
-\xca\xc0$:\xcd\x82\xa2i\xbb\xb7\xd0\xfaP\x02vt\
-\x1c\xa4\x911\xc3\x11\xc2p]w\x0e\x198\xee\x06-\
-\x16\x0a\x14WC\x86\xba\xedy3\x0cu`}\xfd\x04\
-\xdd\x1f\xcb\x08\xa7A\x0a\x98\xd4\xf8\x19`\xe3\x19\x90\x0f\
-'t\xdc\xad\xb0o\xfa&\xdf\xc2\xdc\x03\xa8\x1b\xf3a\
-\xc9?\xb6\xbb\xb1b8\xcbe\x10\xdf\x97\x02\xed\xec\x95\
-&\x12\x802\x99\xd3\xd5\xec\x83Z\xe4\x85\xe7\xd1L>\
-\xe1\xff\x0f\x22\xa0\x130\xb4\x08Z\x944\x13\xf4EN\
-d8\x9c\xbct\x07V_\xce\xbb+\xe5\xe0&l\xb4\
-\x16\xda\x16)\x1f\x09\x1c\xa9\xf7\xa04\x12a\xcf\x06=\
-\xb0`\xb8h&Z\x17\xcdB\x02\xf7\x8f\x00\x03\x00s\
-\x0b@\xa4\x95\xffZ\x8d\x00\x00\x00\x00IEND\xae\
-B`\x82\
-\x00\x00\x02\x1e\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xc0IDATx\xda\xa4\
-\x93=/\x04Q\x14\x86\xdf{wv\xcc\xb0>\x96\x84\
-\x15\x85\x84\x8aP \x94\x12\x05=\xbf\xc3\x1f\x90P\x88\
-R%\xd1\xf9\x19\x14\xa8\x04\x0d\x11\x85\xd0\x90X\x95\xad\
-ve\xc7Z\xcb\xdc\x0f\xe7\xdc\x1d\x8bh\xc8\xde\xe4\xcc\
-\xdc\x99\xb9\xe7\x9d\xe7\xbc\xe7^a\xadE3C\xa2\xc9\
-\xe1]\xecJ\x08\x81u\x9a\x8f\xfe1g\xcb\x18\x9cR\
-\x80\xe1=\xbeP\x8cM\xcc\xee,\x19\xf5Ls\xfe\xa2\
-aL\x0c\xad^\xa1u\x0dF\xc7.\xb3P\xb8\xc7K\
-q\x8f\xa9\x05\xc5\x89#`%\xf7\xc2\xbc\xc1\xc4ON\
-\x80}\xe1\xbb\xd1\x0a*\xa6P1\x09j\xd4j5L\
-\xcf\x1f.\x9d\x1d,\x88D\xe4\xf8K\x00\x5c\x8aHl\
-1\xee\x9eJy\x0dn\xa5\xde\x11E\x11\x8e\xf6W\xe9\
-if\xb1\xf8x\x9e\xa5\xc9\x9c\xa7u\xddL!$\xae\
-\xae*\xf4g\x8dL\xa7F\xb9\xa4\xd0\xd3G\xe8\xcaG\
-.\xd7\xe6\x16\x8d\x8cL9\x92 \x08p\xa3\xce#W\
-\xc2w\x81\x81a\xe9\x8c\x01EG\xb6nR\x98\xf6\x7f\
-\x91\xf0\xa0<\xd7AO%\x02 \x81B\xbe.\xc0\x91\
-\xe9\x02\xcaE\x9e\xbf\xd1\xe2\x0a\xda2Ug&\xd9\x80\
-\xb1\xf1A\xa8O\x81/\x02\x81\xfe\xa1dk$\x22L\
-\x11\xa6\x03\x84~K\xc3XM\xc6\xcaT\xcbo\x02A\
-\xcf\xd4%7\xda\xb3\x12Q\x09\xe8\xc9\x11j5\x85\xd6\
-\xde\x9f\xc6J/\xfcF\xa0>K\x10\x98\x9c\xec\x82M\
-L\xb0\x83\xb6\xd1Rc\xcc\x8f\xeeH\x99\x06\x838\x81\
-\x95M\x8b\xb5e\xf8\x90\x1d\x10i\xea'\xa3\xf2BJ\
-\x16\x09\xb6\xe0\xcd\x05\xe3:dILH\x1f\xd5W\xeb\
-ol\x93\xc0\xcd\x1d\xba/\xaf\x91\xafl-\x06\xff9\
-\x03\xb7\x0f\xc8s.\xef\x9c\x90\xcbf\x9a\x7f\x9e#.\
-\xfeY4{\x9c?\x04\x18\x00\xfb\x1f\xf0\xdf\x8a\xf9\x97\
-K\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x024\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xd6IDATx\xda\x8c\
-\x93\xbdN\x02A\x10\xc7\xe7\x96#\xc6\x0f\x0a\x0b4~\
-\x956\x0a\x15\x0d\x85\x15\xb6\xda\x99\xe8\x03X\x18+_\
-@H\x88\x85\xb51\xd1RI\xe8|\x01\x831!\xb1\
-\x14r6PH\xac\x0c`\x83\x22\x90;\xbd\xbb]g\
-\x96[\xef<\x89q\x92\xb9\xbd\xdb\xd9\xf9\xcd\x7fv\xf7\
-\xb4\xadl\x16\xc84M\xdb\xc4a\x0e\xfe\xb6[\xcey\
-\x83\xbb.\x08!\x80?\xdf\x81N/d8\xce\x17r\
-\xb9\xf3O\x0c\xda\xe4\x9c\x83\x8b1\x157\x0c\x03\x0a\xa5\
-\xd2\x1e\xd5B\x7f\xa49\xb6\xb8\x06\x8ch\x9ek\x9c\x92\
-l[\xfa\xa7e\x819\x18@\xbf\xdf\x87^\xaf'\xc7\
-\xab|\xfe\x1c\xd7\xadc\xee\xb2\x92\xa4\xbb\x98\xec\x99F\
-h\x86\xcfh$\xe2\x8bv\x1cp\x10\xdc\xe9t\xe0\xb4\
-X\x84\xcc\xca\xca\xd9I\xb1x\x88\x91#\x09\xe0>\x80\
-Q2\x93\x18\xf8\x05\xc9d2\xb2\x9dX,\x06\xd7\x86\
-\xf1\xfa\xad\xc0\x09*\x08\x00FAH\x89|\xc5v\xfd\
-\x160\x10n!ha\x08\x15\xc1\x9c\x91\x80a\x0b\x8c\
-\x01x\x95FA\x22C\x00\xf3[\x08\x00\xbe\x15\xfc\x01\
-\x89\xe0\xe8\x04\x00\x8c\x00\x9e\xcb=P\xfb@J\xd4\xa6\
-*'H\x14\xe7i-\xe5\xa4\xee\xef\xb1\x05<\xf3\xb0\
-\x02\xaa\xcd\x86M\xfdR\x22[\xb0m\xb6}s\x03s\
-\xedv\xa8\x05R\x80G\x15\x86<\xec\xefC\xb7RQ\
-G\x05\xbb\xf5\xfa\xc1\x94i\xee\xe0\x1d\xad\xe8\xddV\x0b\
-&\xe3\xf1\x1f\xa7\xc0C\x90f\xb5\x0a\x1b\xc9\xa4/#\
-\x91X\xc0\xe7\xc2e\xa1\x00z\xa3\x5c\x86\xa5t\x1a\xc6\
-\xa7\xa7uU\x81\x92\x82\x90\xb1T\x0a.\x94\x02\xf4\xa7\
-Z\xad9aY-L\x90\x93\xe3\xe83\xb3\xe9t^\
-\x04\x0c\x01\xc2\xe5\x5c\xe0\xe5\x11\xf8s\x09\xfc\xc9\x84\xe5\
-8\xe2\x03\xbfi-\xe5P\xae\xae\x00\xef//oS\
-\xab\xab\xc7\xf0\x0f\xe3\xa6\xf9\xe6\x01\x9c/\x01\x06\x00\xc2\
-5\x11x\xfc\xd3\x22\xfc\x00\x00\x00\x00IEND\xae\
-B`\x82\
-\x00\x00\x02\xd2\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02tIDATx\xda\x8c\
-S\xbd\x8f\x12Q\x10\xff\xedGXva\x81\x83\xe3\x92\
-#\x16\xc6\x82\xe4h(L\xce\x0a\x09\xd0\x98p\x96\xc4\
-\xca\x86\xc2\x90\x98\x5ccO\x82&\xc4\xbf\xc0\xc4\xe4\x8a\
-K\xfc\x0f\x5c\x0b;C\xe1\x07\xa8\xed\x15\x5cI@\x91\
-\xcf=\x04\x0e\xdc\xdd\xe7\xbc=\x8ep\xe7\x15N2;\
-\xef\xcd{3o\xe67\xbf\x15\x0a\x85\x02V\xf2\x90t\
-\x17\xff'?H\x0d\xbe\x90/=\x8b\xc5b\xf7\xe8\xe8\
-\xe8\xf5t:\xc5|>\x87e\xd9\xe8\xf5~\xd3\xda\x81\
-\xd7\xabB\xd7u\x04\x02\x01\x04\x83\x01\x94J\x8f\x9eJ\
-\x92\xe4\xc6\xc9'''H$\x12\xee\xc6\xb2,\xd4\xeb\
-uL&\x13\x84\xc3\x11\xccf\x0c\xe7\x0b\x07>\x9f\x0e\
-\xcb\xb6 J\x224\x9fz\xa5\x14\x91'\xa8\xd5jk\
-\xc7`0@&\x93\x81i\x8e)\xe1\x12\x8c|Lp\
-.\x14\x17\xba)\xbc\x85B\xaf\xd7\xbbe\x18\x06\xb2\xd9\
-\xac\xeb\xec\xf7\xfb\xd8\xdf\xbf\x87\x8f\x9f\xea\x14\xe8\xa5 \
-\xb6\x0a\xb6]\xbd\x92@\x10\x84;\xa7\xa7\xa7/7\x9d\
-\x8e\xe3`4\x1a!\xbc\xa5\xa3\xddn\xe3g\xbb\x09\xbf\
-\xdfO\xfd\x07\xd1l6\xdf\xd3\x95o\x97w\x05\x02\xe3\
-1\xd9\xdb|S\xa9T\x9es\x9b\xcb\xe5\x10\x89l\xe3\
-\xf3\x97\xafP\xfd[\xd0\x098\xbf\xeeC\x90@\xe4@\
-\x1e\x96\x8a\x1c\xc4W.\x06\xa4o\xa2\xd1\xe8\x8b|>\
-\xdf-\x16\x8bX.\x97\xa0=\x0c\xe3-\xcei=0\
-\x87\xe8\x0e\xba\x18\x91\x9dL\xcf\xf0\xc7Z\x5c\x05qo\
-o\x0f\xa9Tj\xed\x88D\x228>>\xa6$;P\
-5m\xdd\xbb#\xd87c\xc0\x13lJ:\x9dv'\
-\xc1y\xd0\x1d\x8e7&@IVz}\x0a\x97\xf2\xbd\
-Z\xad\xbeK&\x93\x07\x1c\xc4\xd9l\xb6Jd\x11\x91\
-\xbc\x18\x12\x88}\x02\xd1\xb8\x06\xa2\xcc/\xaf\x90\xbf[\
-.\x97\x0f6\x99\xf8\x8b*0\xe7S\xc8\x8a\x08\x9f_\
-%\x00u\xdc\xcf\xe7\x1e<{rh\xd0\xf4\x1an\x82\
-V\xab\x85P(\xc4\xc1c\xfc5\xd34\xd7/wi\
-\x94\xe6r\x0aE\xf3 \xc4\x02\x10e\x06MS@\x8f\
-\xd8\xa2(b<\x1eCn4\x1a\x88\xc7\xe3P\x14E\
-\xbe\xf9\xbfa\xff0\x91\x1e\x90x\x95\xc4\x1f\x17\x03\x95\
-\xc8\xa1\xc7b1M\x96e\x97,\x1e\x8f\xc7mAR\
-Th\xe7g\x10\x15\xc1mA\xd3TH\xb2\xc8\x99\xaa\
-v:\x9d\x1d\x8a\x9d\x08\xf4\x09\x93\xc6TU\xcd0\xc6\
-\xb6m\x9bF\xc5\x98K2\xae$\xfc\x03^2Y\xc6\
-\xd7t\xde\xa3\x0a>\xd0y\xe7\xaf\x00\x03\x00-\x9f8\
-\xb0\xf8(\xc4\xeb\x00\x00\x00\x00IEND\xaeB`\
-\x82\
-\x00\x00\x02<\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xdeIDATx\xda\xa4\
-S\xcdJ\x1cA\x10\xfezz\xf67\x19\x89\x07\xc5\xdd\
-\x0d\x91M \x8a{Q\xd0\x8b\x0a\xeb\x1er\xf2\xe2Y\
-\x08$o\x10\xf2$y\x82\xe4\x15r\xf1\x94\xc3.\xc8\
-B\x82BBDQ\xf1\xe7\xe4\x88\xffn\xc6\x19\x9d\xe9\
-\x99\xe9t\xb5\x19\xd9]7\xa7m(\xaa\xba\xea\xab\xaf\
-\xab\xba\xbb\x98\x94\x12\xfd,V}\xdf\x84e\x0d\xc04\
-Mp\xce\x91\xcf\xe7\x91\xcb\xe5\x8b\x8a\xf8\xe8\x01\xc4X\
-\xe9\xf6\xd6\xb3=\xcfC\x14E\x08\xc3\x10\x8e\xf3\x07\x8d\
-\xcf\xb30\xbb\x19\x09\xa4\xc4\xced\xb25\xc3`\xf58\
-\x965\xdf\xbf\xb3\xffW\x81\x91\x18q\x1c7\x14\xbbL\
-\xc4\xf3\xdczyD\x82t\xbb\x9fp\xed\x04\xa6*M\
-\x97\xaeV\xf5\xdb\xa7\x97\x88b\xd1u\xc6\xc0\x83\xc5\x8d\
-\x14\xde|8\xa8\x92My\xba\x02\xdf\x0f\x8a\xad\xd6\xb5\
-\xee)\x10w\xf8\xfd\xa3\x89\xd6\xe5yOMq\xc2\x11\
-\x9e\xf2t\x05B\x88#\xb5\xa1~\x11\x09\x81\xe7\xe5W\
-0R\x1c\xe5\x89\x09}B\xa2K\xcaOq\xd7\xf5T\
-\xbbr\x81\xee\x87\xeeWU  DX\x9f\x1c\x7f\xa6\
-t\x80\xfd\xed-\x04A\xf0H\x0e\x94\x9f\xe2\xf7\xb8\xb0\
-Ny\xba\x05)\x0dH\xc9j\xdf\x7f] T\x80\xc2\
-\x8b\xd1\x9e\x04\xe4\xa78\xe1\x08Oy\x9a\x801^\xe2\
-<\xd3\xe0<\xab\x01\x87\xbb;\xf0o\x5c\xecmlt\
-h\xf2S\x9cp\x84\xa7<}\x07\x9c\xa7\xedT\xea\xc9\
-\xfd-C\xe2u\xa5\xa2\xed^\x9a\xe2\xe9\xf4S\xbd\x17\
-\xc2\xd5\x7f\x83\x0d\x8f\xbdS\x8ciX\xc33\xab\xd6\xd0\
-\xf4|\xfb\x03NW,\xaco:\x1d\x8f\xea\x9c\xad7\
-\x9d\xd3\xb5\xf9(\x0ap\xb2\xfd\xa5#\x96URPB\
-\xcfS\x1c\x9d\xfc\xb8<\xf7v_\x92N|\xff$\x97\
-$\xd0\x1c\xb1\xee\xaf9X\x98\xc3\xd4\xe2W5\x0bq\
-\xdb,\x18\xa5\x9f+K\xf6\xd5q\xb3\x03\xab\x09\xfa\x9e\
-\xc6~\x09\xfe\x0a0\x00@\xdf6\xdc\x81!w\x05\x00\
-\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02\x01\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xa3IDATx\xda\xa4\
-\x93\xbfK\xc3@\x14\xc7\xf3.\x01u\x11Q\xfcQ*\
-\xb8\xa8\xe8\xaa\xad\x1d\x1d\x8aE\xc5\x1f8\xb9\x08\xba\xba\
-:\xa8\xff\x82\x8b\xa3\xe0&\xd4]\xc4A\xacvp\xab\
-\x0d\x0e.:8\x09:\xd6\x9a\xa61Mr?|\xd7\
-4!V\x87@C.\xef\x91{\x9f\xef{w\xef\x0e\
-\x84\x10J'\x8f\x96:\xbc\x9bC+G\x19\xc5\xcaq\
- \x00\x08\x19\x0d\xa1\xcc\xe3\xd1\xc2\xf6\xec\xc1-\xe0\x8f\
-\x898\x02\xc8\xf4\x07\x8c\x14\xd0g\xf6\x0bd77\x9e\
-ZO'\xa7\xe3\x08\x5c\xea\x1f/\xc8\xe4\xd1\xd5\xa5@\
-\x09\x9d\xc9\xb5tr\xca\xf6\x98\x11G@\xc6\x9e\xdc\xbc\
-\x16\xd1-i\xadM$\x5c\x08\xce\xb8`q\x04d,\
-r\xa4\xb9\x89\x9c\xf3\xe6\xbeP&\xb8\x1c\xd1@\x8fq\
-\xb7\xde\xa0\xa6\xed0\xcb\xa1\x0c_?\xc1p_w\x02\
-9\x88\x0a\x10\x99\x1d\x81f\x80G\x85W\xb5\x9cO\xd3\
-\xa6u,\xb0%*\x94\xa0\xe1.\xe5\xf2\xf1+\x08\x96\
-@\xb9\xe0\x1ef\xb0\x1a\xd4\xaa\x98N\x15\x059\x80B\
-p\x9a\xa0U\xa2\xc7\x05}\xb5}\x09\x842\xce\xbf\xea\
-\xaei\xd8\x9e\x89\xa9\x08R\xe0\xf7<\xe8\xbdoZ\x1f\
-\x12V\x10\x08`f\xc7\xf8vmL\xa4B{\xdf\x83\
-\x03\x14\xfaB\x0b\x05\x18c\xf2d\x11\x87r\x0fC4\
-\xf8\x87\x83?>\xa8R@._*eq\x22q\xf5\
-\xf0V[\xcd\x8c\x0dE`\x88\xd8_\x05a\xac\x81\x89\
-\x13\xe8g5\xd7u\x97\xdf\xcf\xb6\xe6Gw\xce\xef\xf3\
-\xc5\xe7\xa7\x98wh\x04\x99Edz`p\xf3tE\
-\x80\xba$\x9cZ\xa1r\xb1\xa7\xc7\xa1\x076\x8e\xd3\xd0\
-\xd5\x9b\x03\xc1\xae\xa1\xd3\xeb\xfc#\xc0\x00/\xd7\x0a\xde\
-\xec\x13\x8fq\x00\x00\x00\x00IEND\xaeB`\x82\
-\
-\x00\x00\x02\x83\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02%IDATx\xdab\
-\xfc\xff\xff?\x03%\x80E\xbfx;\x03+++\xb2\
-\x98\x19\x14\x9f\x02\x1a~\x0a\x9b&FFF\xb8\x1a\x16\
-\x90\xc0\x9f?\x7f\x18\x98\x98\x98@\x12 \xae\xf9\xd9N\
-\xd7x\xe3\xf2\xdd \x8e*6\x03\x80\x06\x0b\xc1\xd40\
-\xea\x15m\x03\x0bB\x0d\xd0\x022\x1d\x80\x985\xcbC\
-\xd5\xd4\xcfXJ\x0d]3;+\x13\xafc\xc3\xfe\xc9\
- 5@|\x92\x05IN\x1bh\xb2\xf1\xfeF\xa7\x9c\
-\x1f\xbf\xfe~\xfa\xfd\xf7\xff\xb7\xef\xbf\xfe~@\xd6\xcc\
-\xcf\xcd*\xe3P\xbf\xaf\x1d\xc8<\x0b\xc4WA.\x06\
-\x19`\x05\xc4\x96\xff\xfe\xfd\xfb\xbd\xbf\xd19\xed\xed\xe7\
-_\x0f\x915132\xb2\xb0\xb12qs\xb02\xf1\
-\xd9\xd7\xee\xe9\x02i\x06\xba\xf6*<\x10\x81\x1a\xad/\
-\xf7{\x87\xeb\x16n]\xf9\xf9\xc7\x9f\xf7\xbf\xfe\xfc\xfb\
-\x8b\xe4\xd7\x7f\xbb.>\x7f;w\xcf\x9d\x8b\xa0\xa0\x02\
-\xe23\xc8\x9a\xc1^\x07*:\xaeS\xb0eM\x8a\x8b\
-\x8a\xc1\xe7\xef\x7f>\x00\x0d\xf8\xfd\xf5\xe7\x9fo\x8f\xde\
-|{\xfa\xee\xcb\xafOsv\xdf\xbe\x02\xb2\x00\xa8\x8e\
-\x1d\x88\xaf\xfc\xfd\xfb\x97\xe1\xf7\xef\xdf\x0c\xbf~\xfdb\
-\xf8\xf9\xf3'\x03\x0bP\xf0\x08\x10k\xb9\x1bJI|\
-\xfa\xfe\xfb\xfd\xd7\x1f\x7f\xbe\xbe\xf9\xf4\xeb\xc3\xdf\x7f\xff\
-\xff~\xfb\xc9\xf4;\xc4R^U+o\xd3:\xa0e\
- \x97\xe9\x01]|\x09\x88\x19@\x18\x94\x86X@&\
-\x82\x5c\xf2\x1b\xe8\xf4\xb7\x9f~}\xfa\xf0\xed\xf7\x17h\
-\xe2b\x06\x06\xe2_]y\xa1_v\xda\xe2\xba\x92\x02\
-\x1cb\x81\x1d\xfb>\x83\x92\x01\x10_\x84{\x01d\x00\
-\xd04\xe6/?\xfe\xfcx\xff\xf5\xd7\xf7\x7f\xff\xff3\
-\x83\xc2\x06\x86\x7f\xfe\xf9\xfb\xef\xf9\x87\x1f\xef\xce=\xf8\
-pc]\x85S\x04P\xad\x0dP\xdc\x00\x9e\xa8\x94\xd2\
-V9\x81\xe2>\xd2^E\xd9Y_\x86\x83P\xd2\x15\
-\xe7g\x17\xf5m\xde\xb9\x1b\x9a\x0e\x0e\xb0\x00\x03\xc2\xeb\
-\xc9\x82\x18\x07\x99\x84%\x07\x16\xec\xba\xfa\x82\xc8, \
-\x01\xd5\xc3\xc5(\x165\xcf\x0b\xe8g\xaf\xff?>\xee\
-~\xb3\xbe\xe841\xbaE\x02\xfbL\x199\xf8]\x81\
-\x09i\x1b#\xa5\xb9\x91\x89\x81B\x00\x10`\x00\xcc\xb0\
-\x1a\x0a\x9c\xeb7\x9d\x00\x00\x00\x00IEND\xaeB\
-`\x82\
-\x00\x00\x05\xff\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x03iiTXtXML\
-:com.adobe.xmp\x00\x00\
-\x00\x00\x00<?xpacket beg\
-in=\x22\xef\xbb\xbf\x22 id=\x22W5M\
-0MpCehiHzreSzNTc\
-zkc9d\x22?> <x:xmpm\
-eta xmlns:x=\x22ado\
-be:ns:meta/\x22 x:x\
-mptk=\x22Adobe XMP \
-Core 5.0-c060 61\
-.134777, 2010/02\
-/12-17:32:00    \
-    \x22> <rdf:RDF \
-xmlns:rdf=\x22http:\
-//www.w3.org/199\
-9/02/22-rdf-synt\
-ax-ns#\x22> <rdf:De\
-scription rdf:ab\
-out=\x22\x22 xmlns:xmp\
-Rights=\x22http://n\
-s.adobe.com/xap/\
-1.0/rights/\x22 xml\
-ns:xmpMM=\x22http:/\
-/ns.adobe.com/xa\
-p/1.0/mm/\x22 xmlns\
-:stRef=\x22http://n\
-s.adobe.com/xap/\
-1.0/sType/Resour\
-ceRef#\x22 xmlns:xm\
-p=\x22http://ns.ado\
-be.com/xap/1.0/\x22\
- xmpRights:Marke\
-d=\x22False\x22 xmpMM:\
-DocumentID=\x22xmp.\
-did:C43B52F403BD\
-11E18A2098D75C57\
-074B\x22 xmpMM:Inst\
-anceID=\x22xmp.iid:\
-C43B52F303BD11E1\
-8A2098D75C57074B\
-\x22 xmp:CreatorToo\
-l=\x22Adobe Photosh\
-op CS3 Windows\x22>\
- <xmpMM:DerivedF\
-rom stRef:instan\
-ceID=\x22uuid:AC1F2\
-E83324ADF11AAB8C\
-5390D85B5B3\x22 stR\
-ef:documentID=\x22u\
-uid:C9D349664A3C\
-DD11B08ABBBCFF17\
-2156\x22/> </rdf:De\
-scription> </rdf\
-:RDF> </x:xmpmet\
-a> <?xpacket end\
-=\x22r\x22?>\xb8B\xe1S\x00\x00\x02,ID\
-ATx\xda\xa4\x93\xcfk\x13A\x14\xc7\xbf3\x99\xdd\
-nL\xb6\xdaT\xa8D,x\x11\x95\x8a\xa0D/j\
-\xd4ZA\xfa\x07x\xc8\xa1x\x11\x05A\x0f=x\xd5\
-\x83\x17O\xe2MAQ\x10\xd4\x8b\x82\x82PP\x1b*\
-\x8a\x04\x05\xad?\x0aE\x03\xb1\x86\xa61\xc44M7\
-\xd9\x1f\x19\xdf4\x9b\x98\xc4K\xc0\x81/\xbcy3\xef\
-\xbd\xcf{;\xcb\xa4\x94\xf8\x9f%\x12\x079v\x0d3\
-\x8c\x0c7\x1c\x01\xce`\xe8\xd8\xcb\x808m\x87\xfc{\
-9*\x93\xac\xdax\xe7\xd5\x1b\x05?e\x80\xd9\x8c\x04\
-{r\x91wd\xe4\x8c\xc5\xcc\xc1\xe8\xe9\x1dGN\x1d\
-\xcf.\xfe\x0a*_t\xd3F\xeb\xeb\xcb\xdbS\xe5B\
-\xf6F]\xcaT\x07\x81ewC\xc9\xb1=\x07&\xc6\
-\xdf<\x9f*~\xf9\xf0\xf6\xb1\xf2\xec\xdc\xbd\xffX\xec\
-\xd0\xc4\xf8\xcc\xc3+i\xdav$\xe0\xba`h\xaal\
-Ai\x8bd\xc6Pf\xfe\xfd\x82.p^I\xd9\xca\
-\xa7\xce\xd4\x1d\x11`\xd0|\x89\x0d!\xbf.\x891\x86\
-t\xae\x1e\xae\x94\x969\xa4S\x0bS\x03\x85e@\xd7\
-\x9c\x9aU^\xe1eK\x86\xa3\x11\x063\xa8Z\xf5[\
-h\xa39\x1b\xd4\xb1m\xb5&\xb5\xd2\xef\x22\x04\x87C\
-\x97\x1e\xb8\x9e\xdc*8\xfb1\xf7y\x16\xea\x8cHo\
-\xd2\xdd\x8f\xa4\xeb*\x88M_\x0a4\x09\xae\x1e>s\
-w\xd2Y\xb5`W\xab\xb0-R\xcdB\xb10\x8f>\
-\x1dXg4\x14\x0c\x0bL\xdf\xbfs\x8d\x92_\xe8&\
-@*\x99\xa4\xca\x1cB\x08j\x87\xc3\xf3\x5c\x14\x8b\x16\
-\x02T\xc3\xd0(\x98\x12\x85L\xad\xf3\x1d\xb4ob\xf1\
-8\xba\x09\xfa\xf4\x95\x7f\x08\xbe\xbdnK\xe0\xb8\xad!\
-\xca^\x09(F\xb6\x86\xb8\x90k=eo\xec\x5co\
-\x04/\xf2\xd2aM\x82\xcb\x8f$\x12\xfb\xd6l\xbdW\
-\x82\xf4O\xa9\xa9\x04\xf7\xe8I\x89t^\xe2\xd6+\x86\
-\x13\xdb1\x18\x1b\x1d\x85g;p\x89\xc0%\x02\x97\x08\
-\xfa\xfb]\xe8\x14h\x18\x7f\xb5X\xc0\xc0\xb39 [\
-\x92kC\x8c\x90\x11\xfd\xbe\x04\x9e8z\xf2)a\xe6\
-#\xebY%2\x00\x1e\x0e\xc1\x9cI\xc9\xcd\xfe;C\
-\x13{\xa9\x02+[\xc2\x08\x99Y\xe5S?\x8c\xd9\xfd\
-EzXj\xfc\xe5?\x02\x0c\x00R\x16\xfb\xb0J\x9c\
-+Z\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x03:\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\xdcIDATx\xda\xa4\
-SKh\x13Q\x14\xbd\xf3K\x93\xb1\xbf\xa4\x89\xa9i\
-\xb5B[\xa1\xc5n\x8c\xb4%\x12\xdd\xf8C)B\x15\
-Ap#.\xdc\xb9\x11\xb7E\x0au\xe9B\x5c\xb9U\
-\xbapQD)\xb8\x10Q\xb4.\x94V(\xdah\x9b\
-\xa6\xad\xe9L2\xa9\xf9M\x92\x99\xc9\xfc\x9e\xf7\xa5\x9f\
-\x85n\x04\x1f\x1cx\xef~\xce\xbb\xf7\xbcw\x19B\x08\
-\xfc\xcf\xe2\x87\x1f\xaeno\x04\x01x\x9e\x07\x96\xe3\x22\
-\x0c\xc3\x8c\xa3)\x868\xb2\x13\xb7\x8c\xf8\x88\x97\xcd\xb8\
-\x8e#\xdb\xb6\x0d\xb6e\xc1\xa7\xdb\xbd\xc0\xffA8\xc6\
-sd\xb2\xef\xa0\x18\xec\x0ey\x03\xad\x22/\xd2\xfaT\
-\xcd\x1e\x90rF<\xb9Y\xbbi:0\x81\xa6\x97{\
-\x15\xec\xa5\x122\xe6k\x82\xa9\xb1\xf8\xfe!\xb5\xec\x80\
-c\x12(\x9b\xd6\xaeW<\xd4\xe1\x15\x07\x0f\xef\xeb\x9e\
-\xfd\x90\x9d\xaaX\x8d\xb6\x1b$<\x96\x04Xr\x84c\
-\xdc\xc9\x8b\xb1\xf0\x90\x22kP\xd5m#)W\xa5l\
-\xd1(\xd1\xa0N\xbf\xb7\xbd/\xd2\xdc\xa5Wy\xef\xb9\
-\x91\xd0\xd0\xcc\x9b\xf4$q\xddyt\xc9\xac\x83\xbd\xd8\
-\xa69\xde\xdb\xe5\x0bf\xd2*\x14\x8a5\xe3\xed\x82\xf4\
-MR\xd4\x09\x0c:NA\xf7\xd4\x96G\x9f\x22W\xa0\
-'\xec\x0d\xd2\x1cJ\xce\x9a\xf5: N\x04[\x85@\
-\xa5\xacCb\xbd Y\xa6\xf9\x001\xadU*;\xdd\
-\x91ijK\xac\xe7\xa5j\xd9\x80\x80\xc8\x05hN\x83\
-\xc02\x0c@\xf4s\x0c#\xd6m\x0763\xc5\x12\xb2\
-OW\x8aE\xd0T\x15r\xe94\x98\x18CmR\xb6\
-T\xd2\xa9..\x11iNC\x03Z\x01]\xb5\xba\x0d\
-:jC\xcf\x0e>\x13>\xe7u4\xc7\x11\xb7T$\
-c\xe8m\x1cW\xd3\x5c\xa2:\x18\x8bq\xb5m\x02d\
-\xc7\xb5\xa2\x94\x8c\x01\xdde\xc5@@l\xcf\xca\x85G\
-H2\xba\xfb\x04\x16\x92\x0a\x1e\xcf\x85\x8e\xb0\xdf,\xbb\
-\x9c\xe4\x96\xebu\xcc\xfb\xbc\xdd\x02:\x11sk\xe9_\
-\x85\x22#@\xf8h_/\x9eGO_\x8eE\xa9\xcf\
-\xd04\xaa\xc11\xd4\xe0dKOD\xc7\x98\xd4O)\
-\x9f@\xdf\xbb\x06\x01\xfdQ\xe8\x9cY]ZO\xb2\xcd\
-\x22$u\x16\xa2W\xcfD\xd74v\xb7\x9d\xa87\xe4\
-?\xdbyj\xd8\x97\xf7\xb5\xa5T\x8f7\xa9\xacm.\
-b\xce\xfb\x06A\xf5\xd5=*\x92l\xd6js\x0bO\
-\x9e\xcf\x1f\x08\x890\xaf\xb2P\xe1=T8\x08\x5c\xb9\
-\xd4BFF*\x8a\xcf\x9f,\xf1M\xab\xe9\xd9\xd7_\
-LM{\x86\xff\xa7\xf1Gx[Y\x02\xc6\xb2\xa8`\
-\xe7\xe3woD\xd35\x02\xfe6\x00A`he\x90\
-!\x02a\x94\x8cB66L\x92JU]\xf9k\xc2\
-\xfd\xf1\x22\xe3\xe6\xbe\x03<\xbd\xd6\x10\xb7\x9b\x8d\xdd\xb9\
-\x0f\x1d\xfd\x83\x7f\x8dZ~e\x19r\x8b\x8f\x89\xa7\x95\
-\x83\xaal\xc1VB'z\x89\xaa\xbf\x85(\xa06\x0e\
-%h\xdd\x99\x09\x01\xc1\xfd\xc3\x04\xd3\x01\xd1\x10:\x12\
-\xb8\xbf\x05\x18\x00\xc3\xa8\xbe\x001\x85a\xc2\x00\x00\x00\
-\x00IEND\xaeB`\x82\
-\x00\x00\x02,\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xceIDATx\xda\xa4\
-S\xbdN\xc30\x10>\xc7&IK\x08\x08\x10P~\
-\xfa\x08\x0cL\x80\x84\x08\x1b\x12\x03\x8f\xc0\xc4;\xf0\x06\
-\xbc\x02\xe2\x01\x10\x8c\x0c\xec\xed\x02\x0bbCH\x88\xa1\
-\xeaP\x84D)\xfdI\x9bF6\xe6\xce\x90\xd2\x92V\
-\x0c\x9ct\xb2}\xf7}\xdf\xf9\xce2;<\xaej@\
-c\x8c\x15\xa5\x94\x01:DQ\x07~\x9b\xebf@\x08\
-A^\xd0ZoS\xec\xf4h\x9a\x89n72\xe48\
-\xee\x06J}\xc0(KD9\xb7\x02\xdbvz\x22\xa2\
-\xd3\xe9\x14Q\x00\xc9\xb2\x80+\x05\x19\xba\xfe\xe6\xa5\xf6\
-\x88+b\xa1\x00\x05\x0aF@\xeb\x8f\xa0\xd9l\xd1~\
-\xdb\xb6m\xc69O\xc0\xd0G4\xa6\x94bq\x1c\x1b\
-A\xcf\xf3\x02#@W\x0bC#\xc0\xa2\x88\x03\x09\xf8\
-\xfed\xaa\x85F\xa3N\x02F\xc4\x10\x85)\x04\xa2R\
-\xa9$\x18\x9dT\xc3\x1eqhn_\xff\x11\xd4j\xb5\
-\x01\x5c\x18\x86\xb8\xac\xd2\x0c\xa2T\xb5R\xa9\x04\xf9|\
-\x1e\xb2\xd9,\xb4\xdbm(\x97\xcb#\x87+\xa4T\xa9\
-^\xc9\xaa\xd5&H\xe9@\xbdN\xab\x82a31\x02\
-\xea'\xa7\xfb\x93R\xbaHVfU\x03\xfcA\x9c\xb0\
-,;u-\xcf\x9b\xc7!}\xcd@\x88\x0c\x0eu\x05\
-Z\xad\x97\xa1-X\xbe\xbf\x08q\xe3\x11\xc6\xc6\xc6\x99\
-\xe3\xf801\xb1\xd0#\xf7\xaa\xe0\x99\xe2\x94'\x1c\xe1\
-\x89g\x04(\xf9\xf6t\x86\x93\x1f\xd7\xae\xeb\xe33:\
-C+Q\x9c\xf2\x84#|R\xc4b\xcc*\xb4^\xef\
-f\xbb\xf5\x87[\xcem]\xb9?\x01\xcb\xe2\x9a\xfc\xf7\
-\x9e\xf2\x84C\xfc\x1c\xf1\x8c\xc2\xd6AI\xaf\xee^\x5c\
-O\xe56\x17\xf0\xb8\xf8\x97#.\x87\xf8\x1b\xe2\xa1\xd1\
-\xe7\xca\xc0\xccR\xb01\xbb\xbcs\xfe\xfe|\x13\xdc]\
-\xed\x8f|\xf3\xb5\xbdK\x98\xcam\xd0GZ\xef\xbd)\
-\xa9\xfc\xc7>\x05\x18\x00i\x93\xd4\x80\xf4\xde:\xf1\x00\
-\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x01\xc2\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01dIDATx\xda\xec\
-\x921H\x02a\x14\xc7\xff\xdf\xdd\x99\xa9tZY\x12\
-\xb9h\x18\xba\xa65\x97en5\xb584T\xd4\xda\
-\xde\xe2\xd2\xdc\x185\xd6|4\x06J.\x82-\x15\xb5\
-\x18$\x98\x88&I\x91(\x97\xdd\xe9\xdd\xf5\x8e\x14\xda\
-\xdd\xa2\x07?\xde\xe3{\xef\xfb\xf3\xbd\xf7>f\x18\x06\
-\x061\x0e\x03\xda\x1f\x10\x10\xd8\xb9\x1bh\xeb\xc0\x08\x0f\
-0\xe6\x03\xc3!\x9d\xcf\x12O0p\x00\xc3x\xde\xb8\
-X\x82\xdf\xef\x07\xcf\xf3\xa3\x1c\xc7-Sn\x9cx\xd7\
-u\xfd\x8a\xc7\x9a\xfd\x06\x9aqK\xc55h8^\x08\
-E\xa2\xab\xe1\x95\xc0\x10g\x99\xac\xbeTg\x16\xaf\xe7\
-$\xc7\xe70dYF\xa7\xd3YO$\x12\xdb\xc4\xbe\
-(\x8a\xcel6\xdb\x12\xd0\xea\xd6H\xed\x04\x0a\x22\xe4\
-\x03\xcei\xd1SQ+0=r\xdd\xc0\xc4\x9bk\xd7\
-|\xaa\xaa\xaa\xa8\xd7\xeb\xb6`0\x187\xc5L_*\
-\x95.\x054\xb5)T\xf4=\xa4\x14`\xcbV\xb8\x7f\
-\xb8\xf3\x8a!\x97\xa7\xf9\xd8x\xa5\x5c!\x9f\xcf\x9f\xf6\
-\xfb%\x91MI\x922\xb1X,\x9aN\xa73$\xf0\
-\xc1\x90t\x00g_@Qs\xc3\xcb\x85\x11\xe7w \
-\xc0G\xed\x14\x91\xd2\x8eP\xd6\xcb\xbd\xfb\x16A\x10\xc6\
-\xacV\xeb<\xc5.\xa2\xa1(J\xeeG )\x9b\x05\
-vB$\x18ASE\x97\xd0zq\x7fc\xbc9\xf8\
-_\xdbk\xb3\xff\xaf<\xb8\xc0\xb7\x00\x03\x00\x88\xe2\x83\
-\xb2\xf3\x16\xdd/\x00\x00\x00\x00IEND\xaeB`\
-\x82\
-\x00\x00\x02\xbf\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02aIDATx\xda\xa4\
-S_HSa\x14?\xdf\xbdw\x11\xdb\x8a\x1e\xf2A\
-\x1f\x12E\x0bt\x19q{\xc9\x06\x15\x85\xba\x06Np\
-\xeem\x0f\x85\x12\xe6\x83\xb1\x9e\x0a!f\xf5`O\xb6\
-7\xb9A L\xa5E\xbd4\xbb\x82+$G/[\
-\x7f@\xf6\xb0\xb0\x1eb#\xc9tk\xb3\xb6\xb9\xfb}\
-\x9d\xefn\xd6&\xad\x1e:\xf0\xe3|\xf7|\xe7w\xfe\
-}\xe7\x12\xc6\x18\xfc\x8f\x90\x9dC'!\xe0A}\xf2\
-\xcf~V\xc4\xa8\x06\xe0\xdb\x04x\xf9\x19?>a\xe2\
-\x02j\x81\x13\x1f!\x02\xb5\xc9\x5cF\x1bfg\x9dy\
-\x80kX\xef\xe9\xca\x0b\xe1\x1fD](\xfaA\x22\x01\
-M>\x9f\xe3\x07\xc0u\x0cr\xeeW\x80Z\xa4\x8a\xc9\
-X\xb7\xd1\xaf\x90\xc9@bq\x11\xea\xfa\xfb\xbb\xd3\x8c\
-y\xf1\xbe\xfb\xaf\x01*{oR\x94\xbe\xcc\xea*d\
-\xb3Y\xd8\x9b\xcbA\x97\xcbu\x0a\x83\xde\xe1I\xa4]\
-\x04/\xa2\xad\x5c\x81\x80\xe5\x8a-\x8a\xe2\xf8\xba\xb4\x04\
-9M\x83\xb7\xa1\xd0+n\xc3\xe1\x89x?\xc6\xfd\xa4\
-x\xf53\xda\xcf\xcc\xcd\xc9\x90L\x82\x86\x99\xbe\xa7R\
-\xb0C\x0e\xce\xccD\x8a\x00\xe3\x98Q\xadd\x90Pu\
-\xdf=\xe8t\xbbKQ\xe4T8\x0c\x1bkk\x90\xa7\
-\x14V\x16\x16\xc2\xebh\xbfw\xf3\x80\x1ao7\xe8\x8e\
-\xf6\xc0\x16\xc06\x03i\xba:\x80\x8ao]\x9f\x1f\x1a\
-\x1a\xe9\xf4x\xe4o\xb1\x18\x18M&\xc8\x00\x18\xe6\x9d\
-F5\xdef\x98B'\x19]\xa3A\xa7\xf12lQ\
-\x0c@\xc8\xef\x00\x8c\xedC\xb5gxyY\x0eY\xad\
-\xd1\x13v\xbbl\x96$\xbe0\xe2\xfbV\x89g\x94\x07\
-/\x5c\x94\xef\xcf?\x00\xd0J\x8dT\x0eQ$\x84\xf4\
-\xc4b\xb1I\x8b\xc52\xd6'\x08\x1b\xb9`\x10z\x07\
-\x06\xe4\xe9K\xa6\xc6x\x8b\x14\xc1~ \xad\xa5\x81k\
-\x94\x08V\x13E\x0e\x01R\xaa\xe2\xac\xdf\xef\xbf\xebv\
-\xbb\x15<\x07z)\xdd\xb4S\xaa\xcf\xe4\xc6\xad\xfd\x8d\
-\x1d\x83\xe7\x0f\xee~\xe3\x17\x8f\x9fGu\xa6(\x8aG\
-m6\xdbUUU\x9fPJ\x9f!4n?\x82h\
-E<\xbdb\x9a\x82f\x91\xf7\x0e\x16\xd71y\xe5\xe1\
-\xbb\xa8\x1e\xe1\x83\xa6\xebC\x92$M\x08\x82\xe0\xc0\xf3\
-qDGy\x17\x0e#\x9a\xf9=\xa2\x1eQ\x07^\xf3\
-\x9b\x86\x8f\xed\x0c\xc6\xcd\xaf\xf1\xdb\xc0\x17\x91\xcf ]\
-,\x16'\xcb\x7f&+\xad~\x0d|)D\x92\x13q\
-\x06\x06\x12)\xdb\xd8O\x01\x06\x00\x8b \xf5\xb9Xl\
-\x045\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02\xb9\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02[IDATx\xda\x8c\
-\x93_HSQ\x1c\xc7\xbfw\xf7\xae\xfd\x81m\xe1P\
-\xd8rkZA\x91\x22\x14H/\x9a\x15D \x91=\
-H\xee!\x99\x88\x83A(\xb6)\xad\x17\xf7\x12\x85A\
->\x19d\xf8\x94\xf4\xd0\x1e\x82^F\x0f5\x17Q\x0b\
-3\x89\x88(\xdabn\xd3X\xca\x98\xdb\xdc\xddv\xef\
-n\xe7\xceusp\x11\x7f\xf0\xb9\xf7w\xee\xef\x9c\xdf\
-\xef{\xcf\xef\x1c\x8a\x9e\xa0Q5\x0a\x0f\xc8\xb3\x03\xfb\
-\xb3\xcf\x10pS\x1a5\xd9l\xe8\x9f\x9ar\x0a\xfb4\
-\xdaC\xbf&@\x84\xaa\xe5pF\x22\x91G\xd1h\x14\
-\x22###\xf8\xb5\xce\xca\x96n1k\xa0t3A\
-\xe2\x9e\xaf\x0b\xf4y\xbd.\xbeR\x118\x9e\xdf\x13q\
-\x0e=F\x07\x09\x10\x91U04<\x8c\xd8zQ^\
-\xc1!\x0dTc\xcaE\xe2\x9e\xab\x0b\x5c\x1a\x1f\xbfQ\
-\x22\x15\xd8ryO\xc49\xb4\x8b^$@DV\xc1\
-u\x87\x03\xb1\xb5\x92\xac\x82V\xab\x16\x1a\x972D\xdc\
-\x1eq\xcc\xd4\xbe\xcf\x0dOOk\x03\xb3\xb33g\xba\
-\xba\xc0\x0b\x02\x9aM\xca\xba\x85[kO\x90\xdb\x08 \
-M_\x06x\xa9\xb0\x94\xc09?99\xf36\x18\xac\
-*\xb868\x88D\xb2\xfc\x7f\xb5\xc0\x82\xfb\xfd\x06\xad\
-'\xfa\x91\x8a\xbf\x84\x1a\xa0Yn'T;EX\xfe\
-\x90N\xe7o\x8f\x8e^<\xde\xd6\x06\xd2j\xe8t\x0a\
-\x09\x05\xfb\x0aZU\x06\x0dF\x0b\xd8B\x1a\x9f~\xbc\
-\xcf\xa5\xf2xx\x80\xe8P\xfcS\xf0\xd4\xe7\xbb\x1f\x0e\
-\x85\xe0_X@\x85$X\x8d\x97wXe\xb1\x1e}\
-\x01\x9d\xc1\x02\xbb\xe3\x19t\xfa&\xf4\x98`\x0c\xf4\x0a\
-\x0cAJ0\xd7\xe7\xf1x;\xbb\xbbq\xd5nG\xa5\
-R\x81\xd9\xac\xa8bP\xbf\x83A\xaf\x00\xc5\xa7\xe0\xf7\
-\xfb\xb1\x9d\x89\xe2h\xa3U\xcb\xf18[\xe6 \xdf\x85\
-+\x03\x03H&x\xf1\xe7\xb1\x1d\x9f\x80\xe5\xb0\x1a\x05\
-\xee'\xa2\xb1\x0eX\x9a\x97\x90\xcd\x16\xb9B,<O\
-\xea\xb8\xa4\xdd\xd4\xb5\xb7\xdfM\xae\xac\xdc\xe28N\xda\
-\xbb\xec\x9f06\x22\xf7`4\x95\xc0s\x19\x1c9\xb9\
-\x8c\xc8\xd7\xd3\xd5\x9b\x97\xf8\xf6=\x9c\xdf\xca\xb9\xc5.\
-4\x10\xcc\xd9\xe2\x17\xab\xbe\x93\xf9\xb8\xbbu\xee\x0b\x94\
-\xcd\xde\xdbrP\xa3P1P\x0a\xc8oz\x91\xdb|\
-^\x8d5\x9a\x0c\xc7\xd6\x92\xb9\xaa\x02\x8d(`WK\
-%{|\x07>\xf2:%w\xa0(\x0a\x02\xc3`\xe9\
-\xaf\x00\x03\x00fMf\x08\xea\x03\x80=\x00\x00\x00\x00\
-IEND\xaeB`\x82\
-\x00\x00\x02\xf5\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\x97IDATx\xda\x84\
-\x93_HSq\x14\xc7\xbf\xf7\xeen\xc3\xd4\x9c\xe6\x98\
-\x95\x93r\xd7?\x9b=(HZ\xe8\x10\xb5l\x89o\
-\xedA\xd0\x17\x1f$\x84$\x14+\xb0|\x10\xac\x95\xb4\
-\x82\xc2\xc2\x07_|\xf0a\xf4\x07\xa4\x7fJ\x90X\x0f\
-\x8a\x1a\x08Z\xd9\x1fr\x19\xb2\xcdh\x96%s\xf7\xee\
-v~\x97\xb5&\x0e:p8\xdc\xef9\x9fs\xce\xef\
-\xf7\xe3r\x883>)\x09\xba\x9c\x1cly\xbd\x88l\
-n\xa2\xa0\xa2\x026\xbb\x1d\xbcF\x03\x9e\xe7E*\xa9\
-\xc6v[\x15\x90\xc0,\xa5\xa5((+S\xc1\xa8\xe5\
-E\x22\x91jOo\xef\xdd\xbf\x02G~\xaa\xa7\xe7\xf4\
-\xb6\x06\x07\x8a\x8bUX#l\x93\xf3\x22\xb2\x5c\xe3\xe9\
-\xeb\xbb393\x83\xd7\x0b\x0b()*B%\xd5\x91\
-\xce\xa9\x95\xe6\x92\x12\x1c$A\x10v,\x94'\xcbr\
-\xed=\x97k\x80\x22\x02\xeb\xebH\xcf\xc8\xe0(*,\
-)\xb3\x06eMM\xd0h\xb5\x89N\x92O\x13\x8e\xdd\
-\xef\xef\xbf\x1d\x0a\x85\xa0\xa1\xe3X-\x16\xac\xf8\xfd\x8a\
-\xd9dR\x0b(\xcf'\xbc\x03\x06K\xb2|\xfc\xa1\xdb\
-}\xebWp\x0e\xca\xb7+\xd0\x1a\xbb\x91\x9b}\x08\xa2\
-\xd9\xac6;\xd9\xd1q\x86\xeea\x9cO\x00\x17\xc8\x92\
-T\xf7\x80\xe0\x8d\xb5i(+=\x00\xbdH\xd8{\x91\
-\xad\xac^\xac\xa3\xbd\xbd\x9d\xa6\x8f\xd39\x96\x84\x04\xf0\
-\x89\xd1\x81\x81\x9b?W_AX\xee\x8e%8\xf1\x1a\
-tz=\xea\xda\xda\xcer\x1c7F\x8d\xde1=\xbe\
-A\xa1$I\x8e\xc7\x83\x83\xee\x1f_&\xa0\xffp.\
-\x96\x88Xo %\xf30j[[;\x08~\xa6\x89\
-\xc2\xf1\x0d\xac\x0c~:4t=\xe8}\x81]\xef\xbb\
-b\xb0T\xe8Fj\xd6QT\xb7\xb4t\x12\xfc\x84\xe0\
-\xb7\xf1+\xb3\x06V9\x1c\xae\x1f\x1b\x1e\xeegp\x0a\
-[[\xa7S\x93\xa1\x5c\x17v\xef\xafDUss\x17\
-\x18,\x081\xf8\xd3\xf44>NMA\xa0\xc9\x0d\xcf\
-GF\xae\xfa\xfc~d\xae]\x06\x92\x93\xd5\x82\xdf\xa6\
-K0\x10lol<O\x93\x1f\xd1\xe47L_\x9e\
-\x9b\xc3\xf2\xec\xec\xbf\xbb)v:m\x8a\xa24Lx\
-<\xae\xef_'\x91\xb6\xe1\xc6Fj'\x0c\xfb*P\
-\xe9t^ x\x94\xe0E\xdf\xe2\x22V\xe6\xe7w\xbe\
-Y\x96\xcd\x86\xc2\xfa\xfa\xa2|\x87\xa3;H\x9d\x96|\
->e\x9d\x22\xfbf:\xcb\xff\xcf\xd8\x1f\x93\x96&\x8a\
-5\xa6\xf2\xf2^\xd6\x84E\x83(V\x91\xbe\x87<\x9d\
-\xe5\xc9S\xc8\x93\xc8\xf5\xe4\xda(\xc7q\xd1\x8f\xbd\xe4\
-\x99:\xa31[k4\x1e\x09\x07\x02/\xb7\x02\x81\xcf\
-\xa4\x85\xd9CD#\xf3\xad8\x8d\xb9\xfcG\x80\x01\x00\
-\x06\xd4\xffg\xbc\x0c\x93)\x00\x00\x00\x00IEND\
-\xaeB`\x82\
-\x00\x00\x020\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xd2IDATx\xda\xa4\
-\x931H\x1cA\x14\x86\xff\xd9\x9d[\xf7D\xc5\x22!\
- \x9c\xc7\x1aA\x02*X\x041]\x88\x88il\xb4\
-\x09I\x1bH\x91&\x85\x956\x81\x04\x03\x0b\xf66\xda\
-\x04\x02\x81\x80e:\x0b\x9b\x14\xa9.e\xbc;\x0c\x06\
-Br'\xde\xee\x9d7\xb7\xb73\xe3\x9b\x91\x84\xc8&\
-\x07\x87\x03o\x99\x99\x9d\xef\x7f\xff\x9b\xdd\xc7\xb4\xd6\xb8\
-\xce\xe0O\xb7\xea\xab\x8c\xb1\x90\xe6A\x9fl\x95\x92\xaf\
-s!\xda\xe1\xc3{\xa3A\xe1V\x0e_\xcam\xdc\xbd\
-\xe3cnj\x00\xdce=\xe9\xd2\xd7N\x10\xbe\xfd\x15\
-\xf2f\xb3I\xf0M(*%\x8e\xdb\x98\x9d\x1c\x06\x83\
-\x82\x94\xbd\xd3O\xdf\xce\xc1\xb0N\x145,\xac\x94\x84\
-\xe8\x08@\xa7H\xd3l,=\xfb\x8c\xef?\xcf\xff\xac\
-%e0\xac\x13\xc7\x11\xb4RPRA\x08\xf1O\xd8\
-\x849\xb7\xf6\xe2\x13N~\xb4\xae\xec\xf1V\xeb\x9c\x1c\
-\x90\x00\x89$Ib\x95\x17\x1e\x1f\xfc\xd7\xfa\xca\xf3C\
-\xeclL\x22(\x8c\xc2\xb0N\xa7\xd3%\x07\xda\x96\x91\
-v\xa5\x151{\xbd\xe2\xe5\xde\x18\xce\xce\x22;\xe7Z\
-;\xb0\xff\x02\x85\xa42\xea\xf5\x08A\xf0 \x93\xb9R\
-\xb9t51q\x1f\xef^\x03\xb5\x9a\x07\xc3r\xd7\xf5\
-\xad@7\xa52\xb4\x0b\xce=\xbc\x7f\xc33\x02\xf3\x8f\
-|\x14\x8b\x0b\xf6\xdd\xe9i\x03\xb9\xdc\x00\x0c\xcb=o\
-\x882S\x09\x92\xd1f\x1e\x9e\x97\xa7\xcf\x93d\x04\x0c\
-\xfc!\xcc\xa3\xd1h\xd93f\x18\x96\xfb\xfe\x089\xe0\
-\xa4\xa6I`\x10\xcc\xc9\x93\xad\xec\xe5\xedo{t\xeb\
-\x89M\xf2{\x18\xd6\xa1G\xb5|\x22I\x80cdh\
-\x10\xa5\xb2&\x11\xcfZ\xfc;\x84`W\xd6\xa5#e\
-\x04\xaalfq\xf7\xc9\x8d\xf1\xe5W`n\xb1\xafN\
-\xd0\xf2\xb8\xf6\xed\xe3\xa6\xf9\xe1\x8d\xa7a\xd3X}6\
-SJ\x11\xb3\xeb\xb6\xf3\x85\x00\x03\x00Kb\x16\x94\x80\
-n\x06\x02\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x03\x22\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\xc4IDATx\xda\xa4\
-SKk\x13Q\x14>w\x1eI\x93\xd04MkL\
-\x1bju\xfaP[*HpUkQ\xc4\x85\xd2\xaa\
-E\x04K\x7f\x82\xb8p+\xb8(\x88[]\xba\xf0\xb1\
-(\xe8B\x84\xb6P\xa4\xb8\x91*\x8a\x98\x0a\x16m5\
-\xb4\x0d\xad\xa6v:I\xf3\x9a\xc9\xbc\xee\x8c\xe7&}\
-\x09\x82\x0b\x07\xbe\x99;\xe7|\xdfw\xce}\x11\xd7u\
-\xe1\x7f\x1e\x81\xbdN?\x96\x1f\xe0'\xfe\x97|\x02q\
-\x17!\x22JX,\xe3Pj\xda\xb6\x0d\xb6e\xc1\x87\
-\x1bmU\x03J\xe9\x0c\xb8n|\xe4Bs\xbc\xacU\
-;\x12E\x02\xcf\xa6\xd3p\xe5LS\xab\x927\xf7\xa5\
-\x15\xc3L\xa5\xb5\x92Ia\x1e\xd3k\xdb\x158\xf6B\
-\xb71t}\xf9d|%\xc1\xf3.\x14\xf2\x16\x18\x06\
-\x05V)\x9f\xb3\x88\xe8\x92\xfdR\xc4\xd7z\xa9?\xd2\
-\xed\x15\xddsXL\xfa\xc3\xc02\x8cf\xa0V\xef\xe5\
-S\xd1\xf8\xda\x0f\x15B\xf5\x02\x9aR\xb0L\x13&\xde\
-\xac\x14\xdf\xcd\xad\xd7\xca\x1b\xa5\xf6\xf5\xb4\xd66p2\
-z\x9c#\xf4\xaa\xeb8\xa1\xdd\x0eLs\xa8\xf3@\xa0\
-=+\xabP\x1b\x14\xe0\xd1\xf3\xf9D]\xbd\x07l\xc3\
-\x00\x9cs\xe2\xd7Fq\xfa\xf5\xa7tYQJ\xd2\xda\
-j\xa1]j\xf2\x1dCM\xdf\xce\x22\x9a\x86\xd1\xdb\x18\
-\x14\xc3\xbaf\xc2\xe7Df\x11\xff\xdf\xdf\x7f8[\xed\
-\x11M<^\xef,v\x13\x9dOe\xe2]-\xa1X\
-$\x5cc \xa7\x1f\xb3\x93\xd5)\xe8z\x07O\x88\xbf\
-\x88\x06\xc9E9Gm\xfb:V\xbf\x87H`%\xd0\
-U\x95u9\x95\x96\xf3\x1eU\xb7b\xc8\x95Psb\
-o\x07\xa0\x1a6\xe4\xcave\xech\x1a\x08\xa28\xc6\
-\xc0\x0c\x0c\xbd\x0c</\x00\xc7\xf3\x01\x95\xbaA\xc6E\
-^`g\x0dL]O\xae\xe7tM\xe5\x04\xa8\x0b\xf9\
-B(\x1a.nn\xc2\xa6\xa2@V\x96\xc1,\xeb\xac\
-\x83a\x96c\x1c\xc6e\x9a\xbd\xbb\xf0vyU\xc9\x16\
-\x05\x0f\xb4\x1cm\x8d\xe1|o\xe2\xa1\x19\xc6xe\x19\
-*c\x8c\xb1\x1c\xe30.\xd3\xec\x1a\x98\xe6\x8b\xe5\x85\
-\x94B\x03>H\x81\xbf&>\xd8\xdb\xdd|02\x8a\
-[\xf5\x91\x81\x8dY\x8c\xe5\x18\x87q\x99\x86i\x09\xbb\
-\x0b\xc1\x91\xa7l\xbb\x06\xf8\x80\xffN\xc3\xc5\xf3=e\
-\x1bc^\x02!o\xc5\x1fr\x86\x03\x05\xc3\x05\x9f@\
- 3>5GU\xed\x16\xae\xc7da\xecZ\xd5\x80\
-\x10\x02\x5c\xe4\x08p\x87\x07\x07\xb8X\xcf\xa8\xd8\xd9\xd1\
-H\xa4Ca'\xdc\xe0\xaf\xb4\x99\xcdh\xee\xd2r\xd6\
-\xfa\x9eT\x9c\x9fs\xb7\x9do\x13\x93\x8e\xbc\x00\x15\xed\
-\x96\x01\xdb\x8d\x06D#\x89tE\x89t\xb6\x0f\xc2\x1d\
-\xdd\xc0\x8b\xd5#K\xad%\xc8&\xbf\xb8K\xaff\x5c\
-\xf9\xab\x8c\x91\x0d\x84\x82Z{\xdb\x80\xf5\xea\xdf\x82\xf0\
-\x8f\x1bL\x11*BC\xad\xf3[\x80\x01\x00\xc4F\xad\
-\xe2\xe9g\xd4[\x00\x00\x00\x00IEND\xaeB`\
-\x82\
-\x00\x00\x02\x98\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02:IDATx\xda\x94\
-\x92\xbf\x8b\x13Q\x10\xc7\xbf\xfb\x83\xdd\xec&\x9bDD\
-\xf1Rl!\x92&E\x0a+m\x02\x8apxw\xc5\
-\x15Al\xad\x02\xa2\x22XJ\x0a\x8b\x80\x95\x95\x82p\
-X\xdc\x1f\xa0\xc5Y\x08\x82V\x16\x17.M\x08\x829\
-\x11C$\xdem6\xd9\xec\xe56?6ow}o\
-\x135\xc1\xd3;\x07fgXf\xe6\xcd|f\xb8|\
->\x8f\x99\xacQ]\xc2\xc9\xe4;\xd5-\xe6\x88?\xff\
-\x8c\xc7\xe3\xa5\x8d\x8d\x8d\xe7\x8e\xe3`8\x1c\x82\x10\x0f\
-\xed\xf6!\xf5}D\x22\x0a4MC<\x1eG\x22\x11\
-G\xa1p\xe3\xb6 \x08X(\xc0\x84\x10\x02\xdb\xb6\xd1\
-\xe9t\xc2\x02\x86\xd1\xc7h\xec#\x1a\xd5@<\x02^\
-\xe0\xa1F\x95\x85V\xf8\x7f6\xca\x01\x015\x01\xe7O\
-\x15S=y\x01\x1a>M\x0cf\xc9^\xa8\xf32?\
-B\xa5T*\xbd\xcef\xb3\xab\xbe\xefc0\x18\xccF\
-!\x94A\x04\xb1X\x8c\xce\x9f@\xbd^\x7fCcw\
-\x8e*p\xb1X,\xae\xceC4\xcc\x038#\x17\x92\
-,!\xa6E\x91\xa0\x10\xaf\xad\xac/\xdf-\xdcb\x1b\
-(\x1f\x0bq\xdf\xb4\xe1\xb8.\x14\x0an\xe2')D\
-@Q\xe5\xff\x81\xf8{v\x9f\xf3\x8eep\xf4\x16~\
-m\xc0\xc3c\xe3\x09\xbe\xec5`\xe5\xda7O\x9b\xf1\
-g\xc4'\x102\x99L\x18\xeby\x1e\xaa\xd5j\x8a\xda\
-4\x1b\xa1\xd5j\xe1[\xe3+z\x86\x01\xc7\xea\xc1\xe9\
-\xf6\xb0\xc5\xbdE\xeej\x0e\x1f\x9a\xdb\x83\xbd3\x9d\xa7\
-\xe6\xa9\x1eDF\x9c\x09\xb5\x7fB\xa4I\xf6\xd0\xc1\x8b\
-\xe1&v\xc7\xbbPy\x05\xb6gC\x1cp*\x91\x83\
-\x1d\xdaVEl6\x9bH&\x93p]7X\x84H\
-\xb0oY\xb0]\x07\xb5Q\x0d\xe7\xd7.\x84\x0f\x99\xc4\
-\xc4\xa5\xf5\xcb:u\xf5\xf7/\xdfA,\x97\xcbH\xa7\
-\xd3\x90eY\xfc\xdb1\xe9A\x0a\x8dW\x9f!\x8a\x22\
-\xa4\xe5(>m\xd6\x9a\x93\x88gPF\x15\x96\xa4\xd0\
-\xe3\xd0R\xa9\x94\xca\x02\xd8\xb1H\x92\x14\x8e \xc8\x0a\
-\xd4\xd1\x01\xee\xcbw\x10\x8d)\xb8\xb7\xfd\x00]\xaf\x0b\
-\xff\x90px\xd8\xbfNs\xfba\x01\xaag-\xcbr\
-u]\x7f\xc4`\x06A0\xdb\x018*\xec\x03\x9e\xe7\
-1\xb9\xe2\xaf\xf8e\x9c\xe3\xda\xc1G\x96\xc3N\xe7\x87\
-\x00\x03\x00\xee\x8d87\x1a\x1e4\xb5\x00\x00\x00\x00I\
-END\xaeB`\x82\
-\x00\x00\x02F\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xe8IDATx\xda\xa4\
-\x93\xbfO\x14A\x14\xc7\xbf\xb3\x8cw\xb9C.\xa2\x85\
-\xc9\xa1$\xc6\xd0\x98\xf8#jb\xa8\x88Z\x5ce\xed\
-_@,L\xe4/0\x16\xd6\x14\x16$K\xa56j\
-\xa7\xa5vXY\x08\x06N\x0a.\x86\x10sp\x07\x01\
-\xf6v\xf5\x8e\xbdefv\x9d\xf7vo\xa3v\xc0$\
-\xdf}3o\xe6\xf3\x9d\x99\x97Y\x91$\x09N\xd2\xe4\
-\xddW\xbb\xf7m\x9c\xb1\xaa\x1e\x91mY\xbd\x90\xb11\
-3w\xae\x9c\x9b:{ZVb\x9d \xd6\x06Z\xc5\
-\xd0:Fd\xd57\x09\xba\x02\xf0\x87\x04<9\x04\xaf\
-\xe0`\xff\x94\x03\x84fbb\xad\x032\xa8\x06{\xdd\
-\x8a\xbfk\xe18f\x19c\xf28\x90\xfd\xe0\x8c\xcd\x8d\
-\xd8x1]WYn\xfe\xaaJY(`\xfe\xc1\xe8\
-\xb1\xeeo\xaf\x0f\xc7h\x9d\xef\xfce\xcd\xc0\xfd\xa8\xb1\
-\xf8C\x83\x8a\xab\x9as\xe8}\xbd\x8d\xfe\xd6\x1c\x03\xee\
-\xba\xcb\xf9\xfc\x84\x96e\x03J\xd0\xc4\x87\x85\x1d\x5c\x1f\
-\x8b\xd0\xa87!\x84@\xd8x\x0dq~\x1a\xed\xcdw\
-l\xd0\xeb\xf7\x18\xd4\x19\xc3\x06Z\xa9\xdc\xb1\xfe}\x13\
-\x93W\x87!w\x1a\x0cD-\x1f\xe5\xf1G\xf8y\x10\
-\xf2\xd8?\xf0\xff1 \x96\x0d(\x11E\x11\xde\xcf^\
-\xe3~i{53H\xc1\x8d4\xa0\xd3\xed\xb0\x81\xca\
-\x18b\xa5><d7JR+\x97\xcb\xd6\xa0\x9e\x1a\
-l\xa5\xe4zf\xe0u\xbdtg\x0b\xd3\x15\x89\x95\xca\
-\xee\xfc\xb7\x01\xf5\x87\x83\x0d\xb4\xdf\xccBy\x0e\xd7\xa6\
-\xadJx[\x7f\x890\x0a\xf3\xb5\x8e\xe3\x80XGe\
-'\xe0#Y\x85a\x88\x0b\xf7jh\xb9\xcfP\x99\x9a\
-F\x10\x04\x98\xbc\xfc\x10\xee\xd2<j\x97j<?\xa8\
-\x01\xb1b\xec\xc9\xa7\xc5\xe5\xa77oQr\xd0\x8a\xc5\
-\x22\x8b\xeaB\xfa\x7f\xcc\xff\x80\x94\xb8\xf1\xfc\xdb\x92\xdc\
-_\xfd\xbc2\xfex\xfbX\x0f)\xd9k\xac\xd8W\x8e\
-\x92\xd5\x08\x99\x1e\x91\xa7#\xff\x16'\xfd\x9d\xff\x080\
-\x00\xdb\xf2j\x84\x0b\xe2\xe5X\x00\x00\x00\x00IEN\
-D\xaeB`\x82\
-\x00\x00\x03\x00\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\xa2IDATx\xda\x94\
-S]H\x93a\x14~\xb6\xef\xdb\x9a)\xa3e\x81\x08\
-\xb3\xacL3\x9c\x89\x9aN1\x179[\xa2\xfd\xd0\x95\
-\x10]V\xe0@\x22$\xd0\x94\xbc\xaa\x9bn\xec&\xeb\
-\xc2\x92\x91\x10\x99?E\xfe,\x94\x9c^53\xca4\
-\xa5\x1f\xcd_\x9a\xb9$\xe7\xe6\xb6oo\xef\xf9r\x82\
-A\x7f\x0f\x1c\xce\xfb\xbe\xdfs\x9e\xf7|\xe7\x9cWa\
-j\xf8\x02Bu_\xac\xec\x15\x0a\x1cU\x00f\xfc\x05\
-\x0c\xb0\xfb\x83\xe8\x12\xc3\x07\x8d\x86f\x94\x0e\x9d\xa6e\
-qA\xe5=\xeb\xe4\xe8(\xdc\x8b\x8bH\xcf\xcf\x87\x14\
-\x0c\xc253\x03A\x14\xa1R\xa9\xa0R\xab\xd1_W\
-\xb6\x891\x88\xc2\xce\x93\x15\xb2\xc0\x92F\x8f\xc9-9\
-\xd8\xec\x99R\xcdv\xd6y\xd51\xc9ii\xb9\xb9\xe8\
-iiA|b\x22\xfc\x1e\x0f\x5c\xd3\xd3\x08\xf8|\x90\
-\x02\x01\xc4eZ\x0e~xa\xf7Q\x06G\xb8\x95s\
-\x8b\x9d\xd2\x19\x01\xfd\x05ma\xcc\x8e\x98\x94\x8c\x0c\xf4\
-\xb6\xb5!3/O\xf6y\x16\x0b\x82<\xf0\xbb\xdb\x8d\
-\xc0\xea*\xbe\xcdM\xb8<~\x16)\x86$\xa9<+\
-9:\x7fk\xa4\xa8\x15\xc6:\x10\x8f.\x14\x99\x8d\xb8\
-}\xc7\x86\xd2S\x16t\xb7\xb7\xe3\xb0\xd9\x0cGg'\
-\x0epQ\x7f\x88\xe1\xed\x9bw\xab\x9f\xfa\x1f\x0e\x0bJ\
-<Ur\x81\xd8\xa5\x85e\xed\xc7\x097|\x1d\xd7P\
-\x98\x93\x86\x86\xa6v\xbcW\xef\xc7\x8d[6\x1c2\x99\
-\xd0k\xb7#%5\x15\xdd=\xfdh\xb2\xbfB\xfdx\
-\xb4k%\xc0\xceH!4\x82w\xc1\xc9\xd60>\xd0\
-\xca\xeeZ\xb3eO\x18\xe9kf\xf5\xe7\xd2\xd9\xec\x93\
-Z\xf6\xe0r\x01{\xd6t\x939\x9dNF1\xd4\xbd\
-\xf3\x97* R\x85C\xa1\x108\x1f\xbb\xb2\x8ae#\
-H\x92\x84\xbd9'\xe4o\x8f\xef_G\xbc\xe9,\xb4\
-\xbb\xb3d\x1e\xc5\x10F\x92.\xfe\x14 \xb2\xb15\x09\
-\x03\xc7G\xe0p8\xa0\xd3\xe9\xa0\xd1h\xa0\xe6\xed\xda\
-\x93]\x22[\x18J\xa5\x12\x92s~}/ReI\
-\xe0y\xd1k\x04\xb9\x98\xd1h\xdc00\xc1\xb5\xdb\xc2\
-\x10\x04A\xee\xc6\x06\x01\x22\x0d\xd5T!\xa5\xa6\x16\x83\
-\x83\x83\x88\x88\x88X'x\xbd^y\x1f\xf6\x06\x83\xe1\
-\x17\x01\xbf_\xce`_e\xb5,\x94\xca\xab\xfd'\x10\
-\x97b\xd6\x05h(\xe8\xb0\xea\xd16\x5c-\x99\xc3(\
-\x8d0\x1f\x16\xaa\x03!\xbc\x8e\x8a\x8a\x82^\xaf\x97k\
-@1\x84\x95\xc9\x97\x5c`-\x83+\xc7\xa6@\xbf\x9b\
-\x90\x90\xf0\xdb\xdb)C\x91\xbf\x07\x8a\xf1}\x1e\xc2\xb4\
-\xcd\x0a\xd1\xbb\xbc\xcc_\xa0B~$\xff\x02\xe2R\xcc\
-\x8c\xcd\xba\x9dJ$~\x1d~>\x1cW6\x8f\xff\x01\
-[\x18\x1b\xe7\x8e\x04\x16\x7f\x080\x00A\x00Z5\xf6\
-\x03<I\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02\x9e\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02@IDATx\xda\x8c\
-SMo\x12Q\x14=\xcc\x8c\x033\xc3\xc0\xa0\x05\x0b\
-\x89\x8bn\xd8X\xc5\xa4\x91\xbd\x0b\x12\x13jL\xd3\x10\
-\x17\xb2rEb\xe2O`\xc9_06ld\xdfU\
-\x9b\xd8\x05Iw.\x10\xe2\xa6I\x01c\x5c\x10\x87\x00\
-C\x85A>\x9d\x0f\xef\x00\x1a\xb0\xa6\xedI\xee\xdc;\
-\xef\xdd{\xe6\xdd\xf3\xee\xb8R\xa9\x14\x96xF\x16\xc6\
-\xcd\xd0$;r\x02\xee\xcf\xcat:\x0d\xe7\xf3\xf9w\
-\xc3\xe1\x10\xe3\xf1\x18\x86a\xa2\xd3\xf9I\xb1\x05\x8fG\
-\x80,\xcb\xf0\xf9|\xf0\xfb}\xc8d^\xbcfY\x16\
-k\x04\x0e\x0c\xc3@\xbf\xdfG\xb7\xdb\x9d\x13\xb4\xdb\x03\
-L\xa6\x16$I\x86a\x1a`X\x06\xa2$\xac\x1d\x85\
-\xb9\xf2\xa0.\xc0&g\xbb\xac\x85aa7'\xa0\xf4\
-E\xa1\xbd,6\xe7\xb6\x8a\xd5\x16*\xb9\x5c\xee8\x16\
-\x8b\xedZ\x96\x85\xd1h\xb4l\xc5 \x0d<\xf0z\xbd\
-\xd4\xbf\x1f\xf5z\xfd\x84r\xcb\xff#\xd8\xc9f\xb3\xbb\
-\xab\x22\xb65\x1d\xc3\xc9\x0c\xbc\x9b\x87W\x96\xe0'\x11\
-\x13\xc9\xbd\xa7o2\xaf\x9c\x1b(]+bK\xebc\
-8\x9bA \xe1~Y\x0a\x89\x08\x08\xa2\xfbo\xfe\xfd\
-ju\x9d\xe0_\x84\xc3!(\x01\x05]\xbdG7!\
-\xe2\x1e\xbdK\x92\x84\x87\xb5\xda\xa7\xcd\x8b\x0b\xdc\xe9t\
-\xae!\xd8\x0c\xe1{\xfa%\x1e\x1f\x1c\xc0\xdc\xda\xc2\xe7\
-Db\xf1\xe5Z\xed\xedBbT\xae\x14\xd1M\xbd\x9b\
-\x81\x00N\xd3i\xec\x9f\x9fc@k\xc9x\x1c\xd8\xde\
-\xdeq\x0a\xde\x17\x0a\xe0\x9cd\x07\xe4/\x89\xe8W\x02\
-8\xa1\xc2\xe7\x87\x87h\xff\xd0\xa8\x15\x1d\x85b\x11M\
-U\xad,\x05\xacp\x8dF\x03\x8a\xa2`6\x9b\xd9\xeb\
-\x22\x1ahu5<\xfap\x8cr_\x83\xf8\xad\x8aD\
-\xe5#$Q\xc2~r/\xf3\xe0\xec\xac|\xb7\xd7\x03\
-W*\x95\x10\x8dF\xe9\xb8\xeeKz4[-T\x1b\
-_\xc1K\xb7\xa0\x18>\x1a*\x13\xa1\x8d t]\x8f\
-\x17\x83\xc1\xf2\x17\x87\x80\xf2\x04\x1a\x0e9\x12\x89\x88\x1c\
-\xc7\xcd\x87\x85\xe7\xf9y\x0b\xac[\x808\xd1\xc1\xb8]\
-\x90\xbc\x14\x8b\x02X\x8e\x81\xa6i\x82\xaa\xaa!\xaa\x1d\
-\xd0\xb4\xe36YD\x10\x84'\xb6mo\x98&\x8d\xab\
-m/\xff\x04\xb8\x08\xce\x03\x0c\xc38\xdevb\xda\xef\
-\x90N\xa7\xb4\xaf\xfe\x16`\x00D\x1c!\xc5N\x09>\
-\xcb\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02\xb5\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02WIDATx\xda|\
-R\xdfKSa\x18~\xce\xb73i\xc1\x0a\x1a\x15\x8e\
-n\xce,\x12\x8b~h\x91\x91I.H\xba\x10\xba\xa8\
-\x8b\xfe\x83\xfe\x81\xa2.r%]\x86\x82\x04yW\x08\
-\xbb\x0b\x14D\xf3\x07\x05\xc6L)/\xa6\xd5H\xd4\x86\
-82fN\xa6[;\xe9\xd9\xf7\xf5\xbeg;\xf3`\
-\xe0\x0b\xcf\xbe\xb3\xf3\xbd\xcf\xf3=\xef\xf3\x1d\xedv{\
-;\xb84Mk\xa3\xa5\x1a{\xd7{)\xe5\x82,\x16\
-\xa1\x94\xc2\xf7X\x0c:?p\xd1\x1a\xec\x8dDz\xb6\
-hs\x9b!%\x8a\xb4\xe7\xec\xc7\xe3q\xf4\x8e\x8d\xdd\
-\xe3\xb3\x08\xf3\xfc\xae\xb6\xa9\x09\x82\xd5\xca\xd0$\x93\xb6\
-\xb7ml\x99&\x0a\xf9<r\xb9\x1c677\xed\xf5\
-MGG\x0f\xf5]'\xee\x09\xc7\x92^$r\xb94\
-\x96\x16\xf4\xeb\xf5xvL[\x16,\x12\xced2x\
-\x11\x8d\x22\x5cW\xf7\xb2;\x1a}L;\xcfl\x01\xb9\
-# \x98,l\x19\xfc'\x12\x0e\x87\xedq\xfc~?\
-F\xe2\xf1\xf5\x0a\xc9\x22\x812(\xc7\x92\x80\x03\x16\xd9\
-\xe7\xf5\xa2J\xd7\xa1\x0b\xc1A\x97\xf4\xa8\x979W'\
-&h\x04R\xdf=\x82\xbbv;a\x11\xe2h\xf7\xfb\
-\xfbq0\x95\x82`\x812J#\xd0Ib\x0f'\x1e\
-\xfa\x7f*\x99\x0c\x1dO\xa5\xfah\xf8k\xc2\xe2\x90J\
-\x10\x8e\x83\xbdD\xd6\xd3i\xe4M\xf3\xa4\x11\x89\xdcZ\
-\x05\x9e\xea\x96{\x04j\xb4s(E\x0aP\xfa\xee2\
-3SH\xcc\xfcA\xf7\xc0\xc0\xcd\xd6\x9a\x9a\xae\xbbJ\
-\x0d\x0b\xe7\xde\x09\x15\x07\x950]Nr\xbf?b\xf9\
-k\x17\xda.}B}s\xf3\xc8\xb4i\xbe\xa6\x11F\
-\xdd\x0e\x84\xed\x80\xae\x8a\x09|\xb6\xe3$\xfb\xeb\x03\x96\
-\xbet\xe2b\xc3y\x0c\x0eO!T[\xb5dJc\
-\xf6s0\x08\x91]Yq2\xa8\xdc\x82\xdb\xc9F:\
-\x86\xe4l'.\xd4\x9f\xc3\xe0\xdbI\x9c\xb9\xf2\x08\xa9\
-B\xf5\x8f\x03\x86\x81w\x81\x00\xc4\xc2\xf882t\x1d\
-\xf4\xd9\xea\xe5 *\x22\xf9\xb5y,\xce<GC\xfd\
-Y\x0c\x11\xf9\xf4\xe5\x078\x16j\xb1{\x99\xc3\x5c.\
-\x1f\xe1\xc8\xd1\xc6\xc6\x0e\xe5*I\x98\x1cz\xa2Tn\
-N\xf5\xbdjQ\x8bsc\xca\xb4,\xf5WJ\xc5\xbd\
-\xcca.\x1ft\x88\x10\xf4\x19\xc6\x0d\xe1\xf3\x1dv\xa7\
-\x9eO$\x1e\xdei\xdd?\xf7-\x1b\x98^\xda\xf0/\
-;\xefe\xa1\xb0ZH&G\xe9\xf1\xe7?\x01\x06\x00\
-\xa6\xe8M\xd6m\xca\x89\x98\x00\x00\x00\x00IEND\
-\xaeB`\x82\
-\x00\x00\x02\xf0\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02\x92IDATx\xda|\
-S]HSa\x18~\xcf9\xdfY\x07e)d\xad\
-\x0b5\xc3RJ\x89Ff\xd4\x9a\xd1\xfa\x13\xd9\x85\xcc\
-\xb0\x10\x22\xeb\xa2\x940*\x0aR(\x93$\xb3`\x04\
-#\xf4\xca\xdaE\x17\x11\x91P^\x98xQ\x9a\x83A\
-dDM\xbch\x924\xcb\x896\x9bz\xce\xd9\xe0\xf4\
-\xbe\xdf\xe6I!\xfa\xe09{\xce\xf3>\xcf\xfb}\xef\
-\xc7\x8e\xb0\x01\x00\x04\x82 \xa4~\xd3\xc0\xb5\x1fq)\
-E\xe1A\xdez\x18\xce\xcb1*\x90\xe7 f\x10o\
-\xa9\xc0\xe0\xdf\x8b\x8c\x97\xbd]]\xd5\xf4r\xa5\xb1Q\
-\x9a\x8c\x82x\xae\xde]z\xba\xa5\xfb\xa1\xffN\xc3\x85\
-\xff58`\x00\x5c\xbd\xef\xf3\xb9\xcb\xca\x0a\xb9p\xcf\
-\xe7\xab\xbe\xd6\xd4\xc4B\xe1\xd8\xf4Bl\x06\xe2\xf1E\
-y\xd9,e\xae\x1e\xe1 \xd2\xeb\x1d^o\x95\xc3\xb1\
-=\xa5!rs\xd7\xc1\xd6m\xf6\xa2\x0f\xa1I{\x96\
-5\x03\xc2\xa1\xe0\xa0\xaa\xeb#\x88U'8\x84;\xb7\
-\xdc\xee\xect9\x9d\xa5\x10x\xdc\x01Y\xe5'x!\
-\x16|\x0a\xce\xfafH$\x12\xe0\xf7?\x875\x89\xf9\
-]\xd1\xe8\x1c\x18+F8b\x18\xc6\x8d\x9b\xed\xedN\
-\x97\xcb\x0e\xb2,\xc3\xc2\xcf\x09(q\xd6\xf2b\xe4e\
-'\xd7\xa8\xa6\xe3\xae\xaf\xfb\xfbO\x8e\x86\xc6z\xb0\xc1\
-\x0058\x8a\xe4VKk\xeb\xde\xca\xca=\xa0(\x8a\
-y\xa4\xec\x0c\x8b\xc9%I\xe2 \x0f\x9d$04\xd4\
-F\x93\x8b\xf8h_\xcb\xd8\x9bw\xcf\xda\xce\xdbl6\
-\xd3\x98i+\x80\xef\xc1>\x0e\xe2\xcb:y\xc8K\x19\
-\xca2\xdc\xbd\xbc ?\x07<5\xfb\x1aDQ\xe4&\
-Z\xc7.v\x98\xbb\x17\x17\xff\xe5\xe4\xf1\xd4x\xc4\xb9\
-'#\xcd\x1f\xbf\xfe\x00\xb1\x10\xc3\xa7j\xcbAO$\
-E\x11\xc3\x8c1\x8e\xf1\xe00x\xcfTs\x10_\xd6\
-\xc9C^\xcaP\x96\x9d=\xbe\x1b4=\xc1\x9b\x0bb\
-\xcaD\xeb\xfd\x8b\x1e\xf0\xb8\x1d\x9c\x07\x90\xef\xa88\xcc\
-9y\xd0O\xa3\x03e\x99\xaa\xe9\xe6=\xad\x1c\xc1\xd0\
-\x17\xf9\x8d[\xadV\xd8\xb2i\xa3\xa9\x93\x073\x929\
-\xd2\x97\x89iXR5\x026\x90\xcc\xcbR\x14\x0b\xa8\
-\xaa\x0a\xb3\xb3\xf3\xd0\xdb;h\xea\xe4!/e(+\
-v\xf7}\x82\xb1o3(\xaa\x92\xb0\xaa\x81\xcc\x1b(\
-\x0a\x83\xba\xba*S\x17x\x03U\xa2\x0cei\x96\xac\
-G\x03c\xb6\xf8\xc2\x12\x13\x98\x05DK\x06\x87\xc5\x22\
-\x83\xa6i\x10\x89D`jj\xca\xd4\xc9C^\xcaP\
-\x96>\x83|\xfa\xcf\xec\xc4o \x1b\xa0\x88\xe6\xfa\x05\
-\xf0\xea7c%H\xc3\xe9Q7[\x93\xc9\xcfXw\
-\xa7\xeb\xe3\xa3\x00w\x89\xfe\x11`\x00\xce\x92\xf8\xe0\x98\
-`\x1e\x9f\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x02\x86\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x02(IDATx\xda|\
-RMh\x13A\x14~;\x9d6\xcd\x0fX\xb4\x98\xd6\
-\xb4\x87P\x11D<\x94\x15<\x16Tl\xb4\x8a\x14<\
-h\xefR\xd0\x93\xf7\x1e\x0a\xee\xb9\x9e\xf4\xa2'\xbdx\
-\xae\x15\x8bzP\x14\x0fj,UZ)\xa5J!\x7f\
-\x0b\x8d&1\xfb\x93\x9d\xc9\xae\xef-n\xba\xa9[\x1f\
-\x0c\xf3\xbe\xef\xcd\xfb\xde\xbc7\xa3x\x9e\x07d\xc3\xe7\
-o\xc1\xc8\xd4m\xe8\xed\xeb\x03\xce9\xf4p\x9eCZ\
-\xc35\xd7\x96rYJ\x09\xc2q\xa0\xf0\xec.\x94_\
-\xdc\x83\xc0X\xe0\x0c\x9d\xbb\x09!\xcba\x92v}\xf2\
-\xb0J;\xe1}\xce\xed\x0at\xcc\xf3rXM\x9b\xb9\
-pD-\x14\x04\x5c\x9b\x1cV\x09\x13\x0f\x11\xc6\xf6&\
-\x0b!0yT\xdd\xdc4\xc00\x1c\xd8\xda2\xe1\xea\
-\xd9\x8cJ|\x94\x08\xdb\xcd\xc5\xca\x8e\xa3\xcd\x5c\xcc\xaa\
-\xe5\xb2\x85\xd8\x05\xd3\x14\xe0\xba.\xe8\xba\x0dW&F\
-U\x8a{{Dx\xe0H!\xa6i\xa0\x0f\x9f\xac\xe6\
-\x09OM\x1cS]\xd7\x03\xc6\x14Xz\xbd\x91\x0f\xce\
-)\x8a2\x8d\xdb\xf2?\x02\x98<K\xd5<\x5c\xae\x94\
-\x9fl\xdb\x81z\xbd\x81m\xb8 l\x1b\x18\xe7\xa7\x14\
-\xc6P\xb0\xbbk\x1e\x06m!\xc06\x0d\xdf/\x95*\
-(`A\x22\x11\x03\xdb2}\xae?\x91\x04\x16\x8bE\
-\x0b4\xaaUh\xd6j\x9d\x80\x84\x0c\xf0x\x0c\xda\xd8\
-\xc2\xef\x9f\xbf|\x8e\xf6\xd4\xc0@\xb4\xc0N\xb1\x18z\
-\x0c/\xff|\xf1}\x07\xe3\xd5\xf3\xd8\xbb\xef\xdb\x86\x11\
--\x10O\xa5\xc2\xfcl\xf0C\xff\x0e\xae\xe3;\xc5/\
-\xd1\x02\xfd\xc9d\xb8b\x06\x93\xe6\xd1\x1d\xc7\xb5\x82b\
-\xf38\x5c\xff\x8a\xb2\xfe\xbdK@\x09*Q\x95\x03\x97\
-4\xe8\x1d:A\xf0\xc1\xe93'/\xf3\xa3\xd9ts\
-\xe3\x87\xbe\xfa\xe6\xebS\xe4n\x88\xca\x1a\xd4\x97\xe6 \
-|\xbb\xae7\xa1\xa0\xb5\xfd\x19Z\x965\xde\xc8\x8e\xa5\
-\x17+\x0cJ#ci\xc2\xc4S\xfc\x7f_\x99\xfc\xb8\
-\xf1\xf2\xce!\xd1\xac\xad\x15?\xae\xeb\x83\xf8b;+\
-\xeb:a\xe4\x071N}\xf6\xec\xf7\x0fhRq\x5c\
-\x07[o\x17\x1em\xb7l\x06\xaf\xde\x1d\x07\xc7\xf8\xe6\
-~\xb8\xff\x18y\x12\xa8\xd2\x1c\xe9\xcb\x04I\x7f\x04\x18\
-\x00*-\x12\x92\xf2.p\xe1\x00\x00\x00\x00IEN\
-D\xaeB`\x82\
-"
-
-qt_resource_name = b"\
-\x00\x05\
-\x00o\xa6S\
-\x00i\
-\x00c\x00o\x00n\x00s\
-\x00\x15\
-\x01\xe5\x04'\
-\x00a\
-\x00p\x00p\x00l\x00i\x00c\x00a\x00t\x00i\x00o\x00n\x00-\x00b\x00l\x00o\x00c\x00k\
-\x00.\x00p\x00n\x00g\
-\x00\x08\
-\x05\xa8Y\xe7\
-\x00n\
-\x00o\x00d\x00e\x00.\x00p\x00n\x00g\
-\x00\x16\
-\x04\xaf\x19\xc7\
-\x00a\
-\x00p\x00p\x00l\x00i\x00c\x00a\x00t\x00i\x00o\x00n\x00-\x00d\x00i\x00a\x00l\x00o\
-\x00g\x00.\x00p\x00n\x00g\
-\x00\x0f\
-\x09\xa2\xd2g\
-\x00n\
-\x00o\x00d\x00e\x00-\x00d\x00e\x00l\x00e\x00t\x00e\x00.\x00p\x00n\x00g\
-\x00\x14\
-\x04i\x90\xc7\
-\x00d\
-\x00a\x00t\x00a\x00b\x00a\x00s\x00e\x00-\x00-\x00p\x00e\x00n\x00c\x00i\x00l\x00.\
-\x00p\x00n\x00g\
-\x00\x10\
-\x0d\x8c\xc4G\
-\x00i\
-\x00m\x00a\x00g\x00e\x00-\x00e\x00x\x00p\x00o\x00r\x00t\x00.\x00p\x00n\x00g\
-\x00\x0e\
-\x05.\x04'\
-\x00a\
-\x00r\x00r\x00o\x00w\x00-\x00s\x00k\x00i\x00p\x00.\x00p\x00n\x00g\
-\x00\x14\
-\x02\xbd\xa4'\
-\x00l\
-\x00a\x00y\x00e\x00r\x00-\x00s\x00h\x00a\x00p\x00e\x00-\x00l\x00i\x00n\x00e\x00.\
-\x00p\x00n\x00g\
-\x00\x17\
-\x09_\xee\xe7\
-\x00l\
-\x00a\x00y\x00e\x00r\x00-\x00s\x00h\x00a\x00p\x00e\x00-\x00e\x00l\x00l\x00i\x00p\
-\x00s\x00e\x00.\x00p\x00n\x00g\
-\x00\x13\
-\x03k|g\
-\x00c\
-\x00l\x00i\x00p\x00b\x00o\x00a\x00r\x00d\x00-\x00p\x00a\x00s\x00t\x00e\x00.\x00p\
-\x00n\x00g\
-\x00\x12\
-\x01\xc1\xefG\
-\x00d\
-\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00-\x00p\x00l\x00u\x00s\x00.\x00p\x00n\
-\x00g\
-\x00\x13\
-\x01\x1aQ\xe7\
-\x00d\
-\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00i\x00m\x00p\x00o\x00r\x00t\x00.\x00p\
-\x00n\x00g\
-\x00\x0f\
-\x00l#\xe7\
-\x00z\
-\x00o\x00n\x00e\x00-\x00-\x00a\x00r\x00r\x00o\x00w\x00.\x00p\x00n\x00g\
-\x00\x14\
-\x08F\x83\x07\
-\x00r\
-\x00e\x00s\x00o\x00u\x00r\x00c\x00e\x00-\x00m\x00o\x00n\x00i\x00t\x00o\x00r\x00.\
-\x00p\x00n\x00g\
-\x00\x13\
-\x05\x12\x08\xe7\
-\x00n\
-\x00o\x00d\x00e\x00-\x00s\x00e\x00l\x00e\x00c\x00t\x00-\x00a\x00l\x00l\x00.\x00p\
-\x00n\x00g\
-\x00\x11\
-\x0f\xbd\xd5\x07\
-\x00d\
-\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00t\x00a\x00s\x00k\x00.\x00p\x00n\x00g\
-\
-\x00\x0c\
-\x03v\xc2\x07\
-\x00q\
-\x00u\x00e\x00s\x00t\x00i\x00o\x00n\x00.\x00p\x00n\x00g\
-\x00\x0f\
-\x02\xacb\x87\
-\x00z\
-\x00o\x00n\x00e\x00-\x00s\x00e\x00l\x00e\x00c\x00t\x00.\x00p\x00n\x00g\
-\x00\x18\
-\x0f\xa1\xdc\xc7\
-\x00l\
-\x00a\x00y\x00e\x00r\x00-\x00s\x00h\x00a\x00p\x00e\x00-\x00p\x00o\x00l\x00y\x00l\
-\x00i\x00n\x00e\x00.\x00p\x00n\x00g\
-\x00\x14\
-\x02\x1a\xad\x87\
-\x00a\
-\x00r\x00r\x00o\x00w\x00-\x00c\x00i\x00r\x00c\x00l\x00e\x00-\x002\x002\x005\x00.\
-\x00p\x00n\x00g\
-\x00\x14\
-\x0a\xb0\xb0\xa7\
-\x00a\
-\x00r\x00r\x00o\x00w\x00-\x00t\x00r\x00a\x00n\x00s\x00i\x00t\x00i\x00o\x00n\x00.\
-\x00p\x00n\x00g\
-\x00\x0c\
-\x09\xe0\x0eg\
-\x00e\
-\x00x\x00t\x00e\x00r\x00n\x00a\x00l\x00.\x00p\x00n\x00g\
-\x00\x0c\
-\x07J\x9a\xc7\
-\x00p\
-\x00r\x00o\x00p\x00e\x00r\x00t\x00y\x00.\x00p\x00n\x00g\
-\x00\x11\
-\x01_\xdb\x07\
-\x00d\
-\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00c\x00o\x00p\x00y\x00.\x00p\x00n\x00g\
-\
-\x00\x11\
-\x06\x89\xcd\xe7\
-\x00r\
-\x00e\x00p\x00o\x00r\x00t\x00-\x00-\x00m\x00i\x00n\x00u\x00s\x00.\x00p\x00n\x00g\
-\
-\x00\x12\
-\x0c\x160\xe7\
-\x00p\
-\x00r\x00i\x00n\x00t\x00e\x00r\x00-\x00-\x00a\x00r\x00r\x00o\x00w\x00.\x00p\x00n\
-\x00g\
-\x00\x14\
-\x02\x0a\xb5'\
-\x00l\
-\x00a\x00y\x00e\x00r\x00-\x00s\x00h\x00a\x00p\x00e\x00-\x00t\x00e\x00x\x00t\x00.\
-\x00p\x00n\x00g\
-\x00\x0f\
-\x09\x00\xfbg\
-\x00b\
-\x00l\x00o\x00c\x00k\x00-\x00-\x00p\x00l\x00u\x00s\x00.\x00p\x00n\x00g\
-\x00\x09\
-\x02\xc5\xa4\xc7\
-\x00r\
-\x00u\x00l\x00e\x00r\x00.\x00p\x00n\x00g\
-\x00\x0f\
-\x0a\xe7\xdb\x07\
-\x00n\
-\x00o\x00d\x00e\x00-\x00d\x00e\x00s\x00i\x00g\x00n\x00.\x00p\x00n\x00g\
-\x00\x08\
-\x06HGg\
-\x00z\
-\x00o\x00n\x00e\x00.\x00p\x00n\x00g\
-\x00\x0e\
-\x09\xee\x04'\
-\x00a\
-\x00r\x00r\x00o\x00w\x00-\x00s\x00t\x00e\x00p\x00.\x00p\x00n\x00g\
-\x00\x10\
-\x0a\xa2\x9b\xc7\
-\x00u\
-\x00i\x00-\x00c\x00h\x00e\x00c\x00k\x00-\x00b\x00o\x00x\x00.\x00p\x00n\x00g\
-\x00\x0f\
-\x0e\xf8X\xa7\
-\x00s\
-\x00c\x00r\x00i\x00p\x00t\x00-\x00t\x00e\x00x\x00t\x00.\x00p\x00n\x00g\
-\x00\x0f\
-\x08\x0fK\x87\
-\x00z\
-\x00o\x00n\x00e\x00-\x00r\x00e\x00s\x00i\x00z\x00e\x00.\x00p\x00n\x00g\
-\x00\x0e\
-\x05\xed5\xe7\
-\x00a\
-\x00r\x00r\x00o\x00w\x00-\x00m\x00o\x00v\x00e\x00.\x00p\x00n\x00g\
-\x00\x14\
-\x0d\xcb\xc0G\
-\x00s\
-\x00t\x00i\x00c\x00k\x00y\x00-\x00n\x00o\x00t\x00e\x00-\x00t\x00e\x00x\x00t\x00.\
-\x00p\x00n\x00g\
-\x00\x13\
-\x02\x81\xde\x87\
-\x00d\
-\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00-\x00m\x00i\x00n\x00u\x00s\x00.\x00p\
-\x00n\x00g\
-\x00\x13\
-\x0f\xb9>\xc7\
-\x00d\
-\x00a\x00t\x00a\x00b\x00a\x00s\x00e\x00-\x00i\x00m\x00p\x00o\x00r\x00t\x00.\x00p\
-\x00n\x00g\
-\x00\x16\
-\x0a\x9a8'\
-\x00z\
-\x00o\x00n\x00e\x00-\x00r\x00e\x00s\x00i\x00z\x00e\x00-\x00a\x00c\x00t\x00u\x00a\
-\x00l\x00.\x00p\x00n\x00g\
-\x00\x0f\
-\x07\xef\x0e\xa7\
-\x00l\
-\x00a\x00y\x00e\x00r\x00-\x00s\x00h\x00a\x00p\x00e\x00.\x00p\x00n\x00g\
-\x00\x17\
-\x04\x9c\xcf\x07\
-\x00l\
-\x00a\x00y\x00e\x00r\x00-\x00s\x00h\x00a\x00p\x00e\x00-\x00p\x00o\x00l\x00y\x00g\
-\x00o\x00n\x00.\x00p\x00n\x00g\
-\x00\x08\
-\x05\x9eY'\
-\x00l\
-\x00o\x00c\x00k\x00.\x00p\x00n\x00g\
-\x00\x19\
-\x07\xf6\x08G\
-\x00a\
-\x00r\x00r\x00o\x00w\x00-\x00c\x00i\x00r\x00c\x00l\x00e\x00-\x003\x001\x005\x00-\
-\x00l\x00e\x00f\x00t\x00.\x00p\x00n\x00g\
-\x00\x14\
-\x0d\x83\xd8g\
-\x00s\
-\x00e\x00l\x00e\x00c\x00t\x00i\x00o\x00n\x00-\x00r\x00e\x00s\x00i\x00z\x00e\x00.\
-\x00p\x00n\x00g\
-\x00\x0f\
-\x09\x91\x09\x07\
-\x00n\
-\x00o\x00d\x00e\x00-\x00i\x00n\x00s\x00e\x00r\x00t\x00.\x00p\x00n\x00g\
-\x00\x0d\
-\x0d\xc8^g\
-\x00p\
-\x00i\x00n\x00-\x00-\x00p\x00l\x00u\x00s\x00.\x00p\x00n\x00g\
-\x00\x17\
-\x06\xaf\xee\xe7\
-\x00r\
-\x00e\x00p\x00o\x00r\x00t\x00-\x00-\x00e\x00x\x00c\x00l\x00a\x00m\x00a\x00t\x00i\
-\x00o\x00n\x00.\x00p\x00n\x00g\
-\x00\x14\
-\x0a\x13\x0c'\
-\x00t\
-\x00a\x00g\x00-\x00l\x00a\x00b\x00e\x00l\x00-\x00y\x00e\x00l\x00l\x00o\x00w\x00.\
-\x00p\x00n\x00g\
-\x00\x08\
-\x00/Z\xe7\
-\x00f\
-\x00i\x00l\x00l\x00.\x00p\x00n\x00g\
-\x00\x10\
-\x07}0\x07\
-\x00a\
-\x00r\x00r\x00o\x00w\x00-\x00c\x00i\x00r\x00c\x00l\x00e\x00.\x00p\x00n\x00g\
-\x00\x12\
-\x08K\xc1\xa7\
-\x00d\
-\x00a\x00t\x00a\x00b\x00a\x00s\x00e\x00-\x00-\x00p\x00l\x00u\x00s\x00.\x00p\x00n\
-\x00g\
-\x00\x14\
-\x00\x83\xac\xe7\
-\x00a\
-\x00p\x00p\x00l\x00i\x00c\x00a\x00t\x00i\x00o\x00n\x00-\x00w\x00a\x00v\x00e\x00.\
-\x00p\x00n\x00g\
-\x00\x11\
-\x0ba\x09\xc7\
-\x00p\
-\x00r\x00o\x00p\x00e\x00r\x00t\x00y\x00-\x00b\x00l\x00u\x00e\x00.\x00p\x00n\x00g\
-\
-\x00\x13\
-\x05\x8a\xeeg\
-\x00d\
-\x00a\x00t\x00a\x00b\x00a\x00s\x00e\x00-\x00d\x00e\x00l\x00e\x00t\x00e\x00.\x00p\
-\x00n\x00g\
-\x00\x14\
-\x02Gc'\
-\x00d\
-\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00-\x00p\x00e\x00n\x00c\x00i\x00l\x00.\
-\x00p\x00n\x00g\
-\x00\x08\
-\x068Z\xa7\
-\x00h\
-\x00o\x00m\x00e\x00.\x00p\x00n\x00g\
-\x00\x12\
-\x05\xb4\x8ag\
-\x00a\
-\x00r\x00r\x00o\x00w\x00-\x00s\x00t\x00e\x00p\x00-\x00o\x00u\x00t\x00.\x00p\x00n\
-\x00g\
-"
-
-qt_resource_struct = b"\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
-\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00:\x00\x00\x00\x02\
-\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x07\xbe\x00\x00\x00\x00\x00\x01\x00\x00|\xe1\
-\x00\x00\x01&\x0c\xfa\x09P\
-\x00\x00\x02\x06\x00\x00\x00\x00\x00\x01\x00\x00\x1c\x08\
-\x00\x00\x01\x225\xb4K \
-\x00\x00\x08$\x00\x00\x00\x00\x00\x01\x00\x00\x84\xd7\
-\x00\x00\x01&\xe1\x85\xbf\xc0\
-\x00\x00\x01\xda\x00\x00\x00\x00\x00\x01\x00\x00\x19T\
-\x00\x00\x01!\xc5.\xd0\x00\
-\x00\x00\x03\xbc\x00\x00\x00\x00\x00\x01\x00\x00:\xb5\
-\x00\x00\x01!+p; \
-\x00\x00\x01\xb0\x00\x00\x00\x00\x00\x01\x00\x00\x16\xf1\
-\x00\x00\x01!+p3P\
-\x00\x00\x00\x10\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01$\xea\xc5\x09\x80\
-\x00\x00\x046\x00\x00\x00\x00\x00\x01\x00\x00B,\
-\x00\x00\x01!+p\xee\xd0\
-\x00\x00\x03$\x00\x00\x00\x00\x00\x01\x00\x00/*\
-\x00\x00\x01!+o\x1a\x10\
-\x00\x00\x08\xa6\x00\x00\x00\x00\x00\x01\x00\x00\x8c\xc7\
-\x00\x00\x01!+p3P\
-\x00\x00\x05\xba\x00\x00\x00\x00\x00\x01\x00\x00[W\
-\x00\x00\x01!+p3P\
-\x00\x00\x02\xca\x00\x00\x00\x00\x00\x01\x00\x00+\xd3\
-\x00\x00\x01&\xe1\x85\xbf\xc0\
-\x00\x00\x01\x22\x00\x00\x00\x00\x00\x01\x00\x00\x0f\x5c\
-\x00\x00\x01!+p\xee\xd0\
-\x00\x00\x04\x88\x00\x00\x00\x00\x00\x01\x00\x00GW\
-\x00\x00\x01!+q\x92\xe0\
-\x00\x00\x01\x84\x00\x00\x00\x00\x00\x01\x00\x00\x14@\
-\x00\x00\x01!+o\xc5\xf0\
-\x00\x00\x02\xac\x00\x00\x00\x00\x00\x01\x00\x00(\xd1\
-\x00\x00\x01!5\x90=\xd0\
-\x00\x00\x00\xac\x00\x00\x00\x00\x00\x01\x00\x00\x07\xd4\
-\x00\x00\x01$\xf8i\xd5\xc0\
-\x00\x00\x06h\x00\x00\x00\x00\x00\x01\x00\x00d\xaa\
-\x00\x00\x01!+p\xee\xd0\
-\x00\x00\x00V\x00\x00\x00\x00\x00\x01\x00\x00\x04F\
-\x00\x00\x01$\xf2S\x8b\xe0\
-\x00\x00\x02X\x00\x00\x00\x00\x00\x01\x00\x00$\x01\
-\x00\x00\x01!\xd5\x9d\x91\xb0\
-\x00\x00\x01\x00\x00\x00\x00\x00\x00\x01\x00\x00\x0c\xef\
-\x00\x00\x01!+oA \
-\x00\x00\x08z\x00\x00\x00\x00\x00\x01\x00\x00\x8a%\
-\x00\x00\x01$\xf8i\xd5\xc0\
-\x00\x00\x06\x9c\x00\x00\x00\x00\x00\x01\x00\x00g1\
-\x00\x00\x013[\xb7\xe4\x10\
-\x00\x00\x00@\x00\x00\x00\x00\x00\x01\x00\x00\x02\x1e\
-\x00\x00\x01!\xd5\x9d\x91\xb0\
-\x00\x00\x08\xea\x00\x00\x00\x00\x00\x01\x00\x00\x92t\
-\x00\x00\x01\x22T\xc0\x89 \
-\x00\x00\x05j\x00\x00\x00\x00\x00\x01\x00\x00VM\
-\x00\x00\x01!+o9P\
-\x00\x00\x08\xd4\x00\x00\x00\x00\x00\x01\x00\x00\x8f\x80\
-\x00\x00\x01!+p\xc7\xc0\
-\x00\x00\x04\xc4\x00\x00\x00\x00\x00\x01\x00\x00L#\
-\x00\x00\x01\x225\xb4K \
-\x00\x00\x03\xe4\x00\x00\x00\x00\x00\x01\x00\x00=\x17\
-\x00\x00\x01!+q\x92\xe0\
-\x00\x00\x07\x5c\x00\x00\x00\x00\x00\x01\x00\x00w+\
-\x00\x00\x01!+q\x92\xe0\
-\x00\x00\x03\x9e\x00\x00\x00\x00\x00\x01\x00\x007\xb0\
-\x00\x00\x01\x22T\xc0\x89 \
-\x00\x00\x07\xd4\x00\x00\x00\x00\x00\x01\x00\x00\x7f\x15\
-\x00\x00\x01!+o\x1a\x10\
-\x00\x00\x06D\x00\x00\x00\x00\x00\x01\x00\x00b\xa5\
-\x00\x00\x01!+p\xee\xd0\
-\x00\x00\x06\xb2\x00\x00\x00\x00\x00\x01\x00\x00m4\
-\x00\x00\x01!+o\x1a\x10\
-\x00\x00\x05F\x00\x00\x00\x00\x00\x01\x00\x00T2\
-\x00\x00\x017\xbb\xfe\xd8p\
-\x00\x00\x02*\x00\x00\x00\x00\x00\x01\x00\x00\x1e7\
-\x00\x00\x010\xe2p#\xd0\
-\x00\x00\x07\xfa\x00\x00\x00\x00\x00\x01\x00\x00\x82;\
-\x00\x00\x01$\xf8i\xd5\xc0\
-\x00\x00\x04d\x00\x00\x00\x00\x00\x01\x00\x00D\x98\
-\x00\x00\x01!+op\x00\
-\x00\x00\x01P\x00\x00\x00\x00\x00\x01\x00\x00\x11C\
-\x00\x00\x01!+p\xee\xd0\
-\x00\x00\x07\x18\x00\x00\x00\x00\x00\x01\x00\x00r\xa2\
-\x00\x00\x01!\xd5\x9d\x91\xb0\
-\x00\x00\x00\x88\x00\x00\x00\x00\x00\x01\x00\x00\x06\x12\
-\x00\x00\x01!\xd5\x9d\x91\xb0\
-\x00\x00\x03\x80\x00\x00\x00\x00\x00\x01\x00\x004\xff\
-\x00\x00\x01%\xcf\xb4\xa4`\
-\x00\x00\x04\xda\x00\x00\x00\x00\x00\x01\x00\x00M\xd9\
-\x00\x00\x01\x22T\xc0\x89 \
-\x00\x00\x07\x90\x00\x00\x00\x00\x00\x01\x00\x00y\xe8\
-\x00\x00\x01(x@V\x90\
-\x00\x00\x06\x12\x00\x00\x00\x00\x00\x01\x00\x00`e\
-\x00\x00\x017\xbb\xfe\xd8p\
-\x00\x00\x04\xfc\x00\x00\x00\x00\x00\x01\x00\x00P_\
-\x00\x00\x01!+r\x17\xb0\
-\x00\x00\x03R\x00\x00\x00\x00\x00\x01\x00\x002k\
-\x00\x00\x01&W-\x08\x10\
-\x00\x00\x04\xa0\x00\x00\x00\x00\x00\x01\x00\x00I\xca\
-\x00\x00\x01!\xd5\x9d\x91\xb0\
-\x00\x00\x08R\x00\x00\x00\x00\x00\x01\x00\x00\x87!\
-\x00\x00\x01\x22T\xc0\x89 \
-\x00\x00\x04\x0c\x00\x00\x00\x00\x00\x01\x00\x00?\x1e\
-\x00\x00\x01!+q\x8b\x10\
-\x00\x00\x06\xea\x00\x00\x00\x00\x00\x01\x00\x00pr\
-\x00\x00\x017\xbb\xfe\xd8p\
-\x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\x0a\x91\
-\x00\x00\x01\x22A}\x0c0\
-\x00\x00\x07<\x00\x00\x00\x00\x00\x01\x00\x00th\
-\x00\x00\x01$\xea\xc5\x11P\
-\x00\x00\x05\x8c\x00\x00\x00\x00\x00\x01\x00\x00Y5\
-\x00\x00\x01$\xd4\xa8-\xd0\
-\x00\x00\x05\x22\x00\x00\x00\x00\x00\x01\x00\x00R\x16\
-\x00\x00\x01$\xdb\x18v\xc0\
-\x00\x00\x02\xee\x00\x00\x00\x00\x00\x01\x00\x00-d\
-\x00\x00\x01!+p\xee\xd0\
-\x00\x00\x05\xe6\x00\x00\x00\x00\x00\x01\x00\x00]\x8f\
-\x00\x00\x01$\xf8i\xd5\xc0\
-\x00\x00\x02\x84\x00\x00\x00\x00\x00\x01\x00\x00&8\
-\x00\x00\x01$\x8eH\xe3\xc0\
-"
-
-def qInitResources():
-    QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
-
-def qCleanupResources():
-    QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
-
-qInitResources()
+# Resource object code (Python 3)
+# Created by: object code
+# Created by: The Resource Compiler for Qt version 6.4.2
+# WARNING! All changes made in this file will be lost!
+
+from PySide6 import QtCore
+
+qt_resource_data = b"\
+\x00\x00\x01\xd6\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01xIDATx\xdab\
+\xfc\xff\xff?\x03%\x80\x05\x99\xe30\xef%\x03##\
+\xe3L \xf3\xf0\x9f?\x7f\x96\xfc\xf9\xfd\x9b\xe1\xf7\xcf\
+\x9f`\xfc\xeb\xc7\x0f\x86\xeb\x0d\xa6\xf8\x0d\xf8\xfb\xf7/\
+\x882\x86b\x10XB\xc8\x05L\xc8\x1c\x90\x8d \x1c\
+\xeb-e\x0c\xa4\x0b\x18\xfe\xff\x8f!\xc9\x00\x98s\xdf\
+\xbf\xff\xc3\x10\xef'o\xfc\xfb\xd7/\x82\x86`5\xe0\
+\xfb\xf7?\x0c\x97/\x7fb\x88\xf5S\x01\x1b\xf2\x1f\x8f\
+!(\x06\x80\x02\x0a\x84\x7f\xff\xfe\x074\xe4\x07\xc3\xf1\
+\xe3\x8f\x18\x82\x5c\x81.\xf9\xf9\x13\xa7!X\x0dx\xf3\
+\xee\x03\xc3\xe3\xa7O\x81\xf4;\x86\xc3G\xef0\xb8\xdb\
+\xca\x82\x0d!\x18\x8d\xbf\xbe\x7f\x07\xd3\xaf~\xfdg\xf8\
+\xc0\xce\x0df\xeb(\x092\xac\xddt\xfe,0z'\
+\x106\x00h;\x08\xbcd\xe5fx\xc9\xcd\xc6\xa0+\
+\xc9\xc1\xb0m\xe5~\xb0fVv\xf6%\x84\xbd\x00J\
+0@\xfc\x82\x95\x87A\x5cZ\x90\xe1\xd8\xa2\x1dg\x81\
+\x818\x01\xe8\xff%?\x9f\x5c\x22\x9c\x12A1\x00\x16\
+dga\xb8>s\x09\xc4\xd9\xefn/\xf9ri-\
+\xc3\xef\xe7W\x802%\x18\x060\x22\xe7\x05V\xed\x00\
+\x06&\x0d\xbf3 \xf6\xff77'\xfc\xbb\xb1y\xc9\
+\xdfW\xd7\xe1\xf2\xd8\xf2\x0d\x8a\x0b\xfe\x5c\xdb\xc8\xc1$\
+\xa0r\x8d\xe1\xc7\x87K\xff\xce\xcd\x05Y\xa9\x01\xc4?\
+\xa0\xf8=\x10\xff\xc4\xeb\x02\xa0\x93A\x06\x0aA\x0d\xfe\
+\x072\x13\x09\xff\x00\xaa\xfd\x83\xd7\x00r\x00@\x80\x01\
+\x00\x0a\xc9\xd8\x8cdC|\x05\x00\x00\x00\x00IEN\
+D\xaeB`\x82\
+\x00\x00\x01\xc8\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01jIDATx\xda\xa4\
+S?K\xc3@\x14\x7f\x97\xbb\x14\xaaD\x041\x89\x14\
+\x1c\x04!\x90\x0fP\xb4\x22\x08\x19\xfc\x04\x99\xdd\x5ct\
+\xeb\xe2'psq\xeb\xb7\xc8\x22\x96t(8\xf9\x01\
+\x9cj;X\x10\x1d2\x84\xb6\x08\xb9K\xe2\xbd\xab-\
+\x1c\xa2\x90\xf6\xc1\x8f;\x1e\xef\xfd\xee\xf7\xfe\x1c)\xcb\
+\x12\xd61\x16\x86\xe1\x81<\x9b\x12V\xc5\xdc\x89\xc43\
+\xcb\xf3\xfc\xa8\xddn\xdf\xd8\xb6\xed\xe7\xb9\x00!r\x09\
+\x0e\x9c\xe3]@Q\x140\x17I\x81\x10\xa6\xc0X\x0d\
+\x92$y\xe9t\xeen\x99\x0c\xd8\x9a\xcdf\xfeh4\
+R\xc1\x08I\xaa\xf0\xdf]\xc2\x8f\xa2h\x93\x99\xa6Y\
+\x04A\xb0R\xfd\xddn\x970)\x93\xcceVk&\
+!\x04KT\x04\xc6BV\x153\x0c\x03\x09\x8c%\x01\
+\xa2\x8aQJ\xe7\x04\x9cs\x03\xbb\xdd\x7f/\xe1\xe9\x93\
+jA{5\x01\xa7\xe6+L\xa7S\xcd\xef8\x0e4\
+\x1a\x0d\xc0\x5c\x96e\x19\xc5\xd7\x1f\x06\x02\xee\xcf\xb7\xb5\
+\xc0\xeb\xc7/8\xde\x15\xd0j\xb54\x7f\x1c\xc7\xe0\xba\
+.`.\x12\xa8\x12\x86\xe3\x0f\xe8\x0f\xb8\x168\x1c'\
+\x90\xd6R\xc0\x11k\x1b4\x99\xa8\x921w\xa9\xe0\xec\
+\xb0\x0eWq\xa2\x056w\x08\xa4i\x0a\xbd^O\xf3\
+{\x9e\xb7 \xa0L.\x91\x89#\xb9\xf07\x14~\xdb\
+\xc9\x9fcT\xb9\x96e]\xca\x8e\xee\xaf\xb2HR\xc5\
+\x1b\x91g\xfd\xe7#\xb1\x8a\xf9\x02\xdbA\xd6\xfd\xce\xdf\
+\x02\x0c\x00\x93\xb2\xe1\x85\xadb\x1d\x00\x00\x00\x00\x00I\
+END\xaeB`\x82\
+\x00\x00\x02\xb9\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02[IDATx\xda\x8c\
+\x92\xcdk\x13Q\x14\xc5\xcf|\x90\xc9d2I*m\
+\xa5\xd1\x85\xa1\x12\xb4 !h7\xae*(\xb6$\x15\
+\x85\xb6*\x82`W\x01\xa1\xff\x81)n\xb2Sqi\
+\xc9BqSQ(\xd8\x82\xad]\xd4EW\xb1\x22\x14\
+\xc1\xb4\xa5P,\xc6tfb\x93\xd6I2\xd3\xf9\xf0\
+\xcd\xa4jB\xc1\xf6\xc2\xe1=f\xee\xbb\xef\x9e\xdf}\
+\xd4\xf0\xf00\xf6c\x90\xa8\x0bG\x8b\x1fD\xd3\xce\x86\
+\xfd\xf3E\xd3\xb4\xael6\xfbLUU\xd4j5\x18\
+\x86\x09Y\xfeE\xf6\x16\xbc^\x1e\xa2(\x22\x10\x08 \
+\x18\x0c \x95\xbay\x9fa\x18\xb4\x14p\xc20\x0cT\
+*\x15\x94J%\xb7\x80$\xed\xa2\xaeY\x10\x04\x11\x86\
+i\x80fh\xf8\x04\xbe\xa5\x15\xfa\xbf\x8dR\x80M\x16\
+\x9b\xb2\x1aBCG/@\xd2\x1b\x07\xed\xfd\xc3\xa6\xab\
+\xe6h\xb6\xf0)\x93\xc9\xcc\xc4b\xb1\xa4eY\xa8V\
+\xab\xfbV\x0c\xc2\xc0\x0b\xbf\xdfO\xfc\x07\xb1\xba\xba:\
+Kr\x97N+\x0a\x86\x16\x17[\x0a\x9cO\xa7\xd3\xc9\
+f\x88\x92\xb2\x03\xb5\xae\xc3\xc3y\xe0\x17\x05\x04\x09\xc4\
++\x89\x1b\xfdc\xa9\xd1\xe9\xfe|>w(\xc4-\xa5\
+\x02U\xd7\xc1\x13p{V\x88@\x04x\x1f\x87\x1eY\
+\x8eD\x14e\xaa\x08<=\x04\xe2?\xef\x16\xd5\xf0/\
+\xc9E\xec0\xcc\x99\xc8\xf8\xf8u\x19x\xc8\x1e:\x85\
+\xbf\x130\xb1\xa7.a}\x83\xc3\xa3\xf9\xf9\xe4\xd5\xee\
+\xee'\xb7m{\xf6\xc8\x10\xebm\x12\xf6\xb8E\xdc\xb9\
+\x96@<\x1e\x9f\x90\xea\xf5\xe7#\xc02\xeb$;A\
+\xd6\x83\x10\x7f\x96Q\xa9\xa9\xe0\xe9\x15\x98\xa5\xf7\xb8\xdc\
+\x97\xc0\xd4\xdb\x0f\xb8pN\xa8.\xaf\x9c\x5c\xce\xb7\xb7\
+\x83\xdd\xdc\xdcD(\x14\x82\xae\xebv+D\x03[\xdb\
+\xdb\xd0\xb5\xcf0\x8d9\x0c\x0e\x0c`\xf2\xcd\x1c\xba{\
+\xc7\xf0\xfd\xd5\x8b|G\x07\x8d\x85r\x19l.\x97C\
+4\x1a\x05\xc7q\x07xPz\x11\x82\xf6\x0e\x83\xc9\x04\
+^N\xce\xa0\xb3\xe7\x1e\xdaN\xf4\x92\x0b\x1e3N\x97\
+kkk\xee\x18y\xf28\xc4p8\xeccY\xd6}\
+,\x1e\x8f\xc7\xb5PZ\x9f\xc4\xad\xbb\xaf\x91\x9d\x18\xc1\
+\xf1\xb3\xa3\xe8<u\x11\x0cKCQ\x14\xbeP(t\
+\x92\xb3\xbb\x843\x8e\x11\x85y\x9e\xbfd\xdbv\xbbi\
+\x92q\xd9\xb6\xdb\x00\xb1\xf1`\xa8\x8f\xfe\xfae\x83\xf9\
+\xb8Qd\xbeQ\x14e\x139\xffe\xd2\xc1\x02\xc9)\
+\xfc\x16`\x00-\xb7L\xed\xde\x12.\xb7\x00\x00\x00\x00\
+IEND\xaeB`\x82\
+\x00\x00\x02O\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xf1IDATx\xdab\
+\x9cb\xcf\x00\x06\x8c\x8c\x0cpp\x9fS\x93\xed\x01\xb7\
+\xb6\x0f\x90)\x0a\x15z\xad\xf0\xf5\xea\x16\xc5\xef\xd7\x7f\
+\xc1\xd4\xfc\xff\x0f\xa1Y\x10\xda\x18f\x02\xb11\x88!\
+\xf4\xe2:\x8b\x9e\xbb\xab\x98ER\x9e$\x88\x7fb\xde\
+\xa4\xe7Ov\xae\xa9c\xe0g\xf8\x03U{\x16\x88\xd3\
+\xc1\x16O\xb6\x87\x1bp\xc6-,\xc9\xf8\xf2\xe5\xcb\x0c\
+\xd2\xf1s\x1988\xd8\x18\xf8\xf9y\xc0\x12\x1f?~\
+a\xf8\xf1\xe3\x17\xc3\xd3\x85\xc9\x0c\xba\xba\xba\x0c\xbbV\
+\xcd\x03\x19`\x02v\xc1\xdf\x7f\x08'\xa8e\xcde8\
+\xb9x\x09\xc3\xa1C;\x81\x9a\xf9\x19xyy\x19X\
+YY\x19\xbe|\xfd\xca\xf0\xe9\xe3G\x061\xbb\x22\x06\
+\xb5\xc8\x08\x86\xed+\xe6\xc1\xf5\xb0\xfc\xfd\x8b0\x00\xe4\
+\xad\xa8\x98h\x86\xfb\xf7\xee1`\x03\x8aJJ`5\
+\xc8zP\x5c\xf0\x17\x182\xff\xfe\xfdc\x90SP\xc0\
+j\xc0_\xa0\xdc\x7f&&\x06d=(.\xf8\x074\
+\xe0\xd0\x85\x0b`\xb6\xa0\xa0 \xc3\xf7\xef\xdf\x19\x8c\xd4\
+\xd4P\x0ca\x01F\x17\x8a\x0b\xfe\xfcC\xb5A\x01\xc9\
+vP8\xfcAV\x0d\x8enF\x06d=,\x7f\xfe\
+\xa2z\xe1\xf6\xed\xdb`\xdb\xdf\xbf\x7f\x0f\x16\xbb\x0d\x95\
+\x03\x89\xfd\xf8\xf1\x83\xc1DK\x8b\xe1\x0f\x8a\x0b\xfe\xa0\
+\x1a //\x0ff\xf3\xf1\xf1a\x84\x01H\x0c\xa4\x06\
+Y\x0f\xaa\x0b\x80^\xb8s\xe7\x0e\x9c\x0fs\x09\x88\x06\
+\x01P\x98H\x00\xd9(.\xf8\xfd\x17\xbb\x0b`@N\
+R\x125&\x80j\x90\xf5\xb0<\xfc\xc2\xc0 \xcd\x89\
+\x90\x84\xb9\x00\x16\x0b<\xaa\xaa\x18\x06\xc0\x5c\xf0\xf4;\
+\xd0\x80\xb5\xcf\x18\x18\xfc\xc4\x19\x18$\xd9 \xd1\xa8\xab\
+\xad\x8d\x11\xf7\xc8\x00\xa4\xe6'0K=\x07\xe2M/\
+!\x99\x89\x13\xc8\xe0\x0d\x15\x00r\x80\xc9\x96\x93\x9b\x9b\
+\x01\x1f\x00\xa9y\xf7\x19\xa8\xf9\x03\x83\x18\x90\xfb\x19l\
+\x00\x10\x8b=\xfc\xcap+\x8e\x97\x9d\x81\x18\xf0\xfe?\
+\xc3-\x90\x1e \xfe\x03\x10`\x00\x8d\xd8\xd1\xd3\x02\xd0\
+p\x99\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x01\xf8\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\x9aIDATx\xda\x94\
+\x93\xbdK\xc3@\x14\xc0_\xd2\xa4$\xa9UK\x1d\x9c\
+:\xb4P\x84\x0e\xe2\xe6\x1fP\xdc]\x8b\xa3\xd4\xc9Q\
+\xfc\x1f\x84\xee\xa5~\xd0I\xec\xecTq\xd6M\x91.\
+\x12MA\xf1\x0b\xa1\xc6Al \xb9\xc4w\x97K\xcc\
+G\x0b\xfa\xe0\x91\xbb{w\xbf\xdf\xdd%\x11\x00C\x14\
+E\x96\x91X\xc3\xac;\xeb\xc7s0=t\xcc\x96\x84\
+1\xa9X?\xe9\xf7w\x94l\x164U\x85\xbc\xa6\x85\
+9\x83}UQ`\xa5\xd1\xd8\xa2\x13\x85\x04\x80\x99\x97\
+\x9b\x87\x9b\x85\xbcZ\x90f\x17'\xaaK\x0b\x1at\xce\
+\x87\xfb\xd8lJ\xff5\xef\xf5\xfa\x00\xc5%\x00\xf7\x8e\
+\x9dYJ\x9a\xdbg#\xf0\xcd\xdf<\xe3\xe6\xe1[\x0e\
+Vs\x16\x02H\x0c\xf0g\xb3\xf1:\x00\xc7q\x10\xe0\
+d\x18\x80\x10B\x9f\xe5^\xbb\x0d\x85\xfa.\xe7\xa5\xed\
+\x81\xd9s]\xb0m\x1b\x80p\x00\xaf\x8b\xb5Z\x0d\xa4\
+R\xc9/&B\x96\xe5\xd0\xec\xa2\x90\x03\xa4(@\xa2\
+E\xc7\xb2@\xd7\xf5\x14\xa0Z\xad\x86f\x978\x1c`\
+\xc7\x00\x19v.L\xfaAU*\x95p\xb1a\x181\
+3\xb19\xc0\x89\x03d6\x88)\x08\x02\x98\xa6\x19\x02\
+h?j\xf6\x5c\xe2\x17\xecq\x16\x06G\xbfG\x08\x00\
+\xac\x96\xb8\x87\xa8\xf9cdZ\x07\x9d\x8b+\xf8z~\
+\x87O\xa3\x9c\xda\xc14@`\xbe\xbd\x7f\xba\x84\xeb\xd6\
+\x06/\x8dS\x00\xcf\xf3b\x80\xa0\x1f1?\xe2\xb0B\
+\xdf,\xdb:N\x98\xc7s\xaa\xf4\xa2(MQ\x94\xd4\
++\x8c\x98\xb7\xb1I/h\x1c\xd4\xe9\x9a9\x84\x9cv\
+\xbb\xdd\x22\xdc\x14\x1f\xa6\xfe\xbc\xbe\x99.|\x89\x0e\xff\
+\x080\x00\xb9\xfc\xfe\x16J\x11\xd5\x16\x00\x00\x00\x00I\
+END\xaeB`\x82\
+\x00\x00\x01\x9b\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01=IDATx\xda\xc4\
+S;R\xc30\x10}B\x06\x8c\x13h\x98\x0c\x05=\
+\x15\x9dK\x0aJ\xce\x90\x16\x0a\x0e\xc098@\x0a\xe8\
+9\x03\x15\x05%%\x05TP0$d`\xc6\xb1\xf1\
+G\x92%\xd6vp\xd0`\x87\xcc\xa4@3\xfa\xac\xf4\
+\xf6\xe9iw\xc5\x8c1X\xa6\xad`\xc9\xe6\x14\xc3\xe1\
+\xe5\x08\x8c\xb1\x01-\xfd\x05|\xeeH\xf5\xe9\xcd\xf1\xce\
+\x8c W\xaa\x98\xfc\xfe\xd1\xae/\xa5\xfd\xa4\x9f/t\
+\x1c\x86\xab\xeb\x97\xdf\x0ad\x96\x95F\x1c\xe7\x08\x02\xd5\
+zu\xb7\xcbk\xacE \xd2\xb44\xd2Ta2\x11\
+\xf5\xa1\x94\x12Y&\xa0\x94\x84\xd6\x1a\xbd^\xa7\xc6Z\
+\x04Y\x92\x94\x86\x10\x9aH$\xa2(B\x18\x86\xe4\x9c\
+\xc1\xce\x92\xa8\xb16A\x1c\x97F\x94\xa4xz\x1dB\
+\xd0\xcdU\x8e\xb8\x05N\xf4\x0c\xdb\xa8\xe0\xf9S`\xe8\
+\xb8\xb4\xeb6\x07\x81\xaf\xcdW0\xe2\x1e\xc6\x9d\xd5\xd6\
+ \x8au>_\xc1\x9b\xe3\xe1\xc3m\xafLA\xdc\xb2\
+I\xc1wj\x0c\xe7\xd8\xf4\x00m\xa6\x1d\xd5l\xa6\xf5\
+ Y\x85\xd5\xe3\x07\xda\xe9\x97>\xac\x882U!\xe7\
+\x07g\x17\xd8\xde\xdb\xff\xb3\x0e\xdf\x1f\xef\xf3\xdb\xf3\x13\
+\xf2S\x16\x01\xad\xb7\xa8o,P\xca\x85\xdc\xc0\x22\xf8\
+\xd7\xdf\xf8%\xc0\x008\xeb\xad\x82\xf1g\xf9\xc8\x00\x00\
+\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02+\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xcdIDATx\xdab\
+\xfc\xff\xff?\x03%\x80\x89\x81B\xc0\xd2\x10\xa6\xe3\x0b\
+\xa4\xa5\xc8\xd0\xfb\x0c\xe8\xfa\xcd,\xff\xfe\xfd\x97nX\
+x`\xfa\xdf\x7f\xbf\x89\xd6\xc9\xcc\xc4\xca\xd0\x10\xef\x90\
+\x09v\xc1\xdf\x7f\xff\x98\xfe\xfc\xf9\xc9p\xff\xe6u\x86\
+/\x9f>0\xe8\x98X2\x5c9s\x1c\xac\x10\x1b\x9b\
+\x87O\x80AQ]\x93\x01\xa4\x0fb\xc0\xdf\x7f\xcc\xff\
+\xfe\xfee\xf8\xfc\xf1=\x83\xaa\x9e\x1e\xc3\x8f\x9f_\x18\
+Ttu\xc1\x9a\xb0\xb1o_\xba\xc4\x00R\x0f\xd2\x07\
+6\xe0\xcf\xdf\x7fL\x7f\xff\xfea\xd040f\xf8\xf1\
+\xeb;A\xe7\x83\xd4\x81\xd4\x83\xf4\x81c\x01\xc8`\xfe\
+\xfb\xe7\x0f\xc3\xa5\xd3'\x18\xfe\x00iB\x18\xa4\x0e\xa4\
+\x1e\xa4\x0f\x88A.\xf8\x0bd\xfc\x01\x9a\xfa\x17\xac\x80\
+\x10\x00\xab\x03\xbb\xe0/\xd4\x0b\x7f\xfe\x82]\xa0\xae\xab\
+\xcf\xf0\xed'a/\xecc\xb1ax\xfd\x14d\x19\xd4\
+\x80\xdf /\x00M\xbc~\xf1\x02\x83\x9c\xba:A\x03\
+.>\xfe\xcap\xeb-\x17\xc3g\xd5(\xe3\xdf\x7f!\
+.`\x01\x85*7\x0f\x0f\xc3\x83\xeb\xd7\x194\x811\
+q\x1d\x18\xd2\xe0\x00\x03\xb2\x9b\xf6|fx\xf2\x93\x87\
+\x81\x83\x93\x93\xe1\xc7\xf7\xef\x0cL\xcc\xdf\x19\x5c}t\
+\x19\xe6\xdcv\xb7\xfa\xc5.\x1c\xc3\xf2\xf9\xdb\x0fN\x16\
+&F\x06IYY\x06I\xa8\x1f\xd5\xb4\xb5\xe1\xfe}\
+\xf4\x8d\x93\xc13\xc2\x82\xe1\xc6'\x06\x86\xcf\xd0 :\
+\xf6\x86\x81\xc1!\xcaIj\xc3\xc2#\x05\x8cF\xd2\xac\
+E\xfc\x1c\x0cJ\xb8\x9c\xfcT\xbf\xc4\xf1;\xbf\xaa(\
+\xb2\x98tJ\xa2\xe8\x93yK\x9e\xfc\xe5\x14\xa9d\x04\
+\xf2\xd9\x80X\x10\x94B\x89I\xc6\xbcQ\x8b\xb7\x83h\
+Ff\xd6^.^\xdeE,@\xf6/ ~IT\
+\x1e\xd0\xf4g\xf8\xf9\xfd\xe7\x09 \xf30;7\xcb\x12\
+\x90\x18@\x80\x01\x00\x0f\xe4\xfd\x07\xfe\xffJ\xc1\x00\x00\
+\x00\x00IEND\xaeB`\x82\
+\x00\x00\x023\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xd5IDATx\xdab\
+\xfc\xff\xff?\x03%\x80\x89\x81B\xc0\x92\xd2\xf6F\x93\
+\x91\x91q9\x90\xad\x0f\xc4\x17\x81.\x8a\x04\xe2\xeb\x9f\
+/f\xc3\x15\xf1\xeaOe\x00\xaa\xc1\xaa\x8e\xe9\xfb\xf7\
+\xef\xcbu\x95\x98\xf4c=\xb8\x19@4\x88\xff\xf5N\
+?\x8a- >6u?~\xfc``\xf9\xfc\xf9\x93\
+\xbe\xa6<\x1f\xc3\xcf\x9f?\x194\xe5\x99\x18\xf6\x1c\xff\
+\xa4\xcf\xfe\xe5v\x1a\xb2\x01\x7f\xbf\xdcf\xf8\x86E\x1d\
+8\x0c>}\xfap\xf1\xe0\xe9\xe7\x0c \xd3@4\x88\
+\xff\x93Qj\xd6\x9f?\x7ff\x81\xc4@4\x88\x8fM\
+\x1d\x1030\x1a\x87\xee\xd0\xfc\xf7\xef\x1f\xdcoLL\
+L\x91@\xbf^\xe7}\xdd\x01\xb2\x00\xe4\x92Y\x9fE\
++\x18\x80\xfe\xc5\xaa\x8e\x05(x\xfd\xef\xdf\xbf\x06(\
+!\xfb\xf9 \xc3\x97/_\xe0|F\xd6}\x0c\x7fy\
+\xed1\xd41333\xb0`\x8b\x9a\xcf\x8f6\xa2\xf0\
+\xff1}g\xf8\xfb\xff7\xd0\x15\x7f\x11\x862\xfe\x03\
+\xe2\xbf\x98\xe9\xe0\xcb\xe3\x8d@\xff}B\xc1\xff\xf8]\
+\xa1\xd1\xc8|\x01\x88\xffChFM\xb0kA\xc4\xcb\
+\x1b\xcb\x81x\x19\xd8\x00VVV\x06...\xb8\x81\
+\xbf\x7f\xfff\xf8z\xa9\x91A\xca\xb8s\xb9\xbf\xab\x9c\
+\xbe\xa7\x9d\x0c\xc3\xf6CO\xf47\xee~\x04\x0a\x0f\x03\
+F\xac\xc9\x93\x89\x89\x81\x85\x05l\xb6/0\xf0$A\
+\x0c\x1d\xbf\xe33;KT\xe0j\xca{\xee\x80}\x82\
+5\x0c\x80\x01\xcb\xf0\xeb\xd7/\x90\xb37\x031X\x8c\
+\x83\x83?\xeb\xc0\xa9/\xfa\x16z,\x0c'.\xfd\x01\
+\xf1/^\xdd\x13\xcd\xc0\x8c\xa4\x8f\x11\xea%6 \x06\
+\xf9\x81\x07\x88\x05\x80.\x10\x06b\xb1\xafo/\x5c\xf8\
+\xc5\x1dhp\xf2\x0a\x8b\xd8\xa3g\xbf\xaf^\xdd\x1b_\
+\xfe\xf1\xc5\xf1\xf7\x8ch\x060B3\x183\x16\xcc\x84\
+\x84A\xea~\x83R9#\xa5\xd9\x19 \xc0\x00\x10&\
+\x047G\xd8\x02\xf3\x00\x00\x00\x00IEND\xaeB\
+`\x82\
+\x00\x00\x02\x87\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02)IDATx\xda\x8c\
+\x93\xcfk\x13Q\x10\xc7gw\xdf\xfe\xa2\xb1\x9b\x14D\
+i\xa994Q\x88\x0d\xb4\xd0RK(x\x11\xf6\xd0\
+B\xff\x86\x82x\xf0?\xd0\xff\xa1'E{\x15Z\xc1\
+\xb3\x04\xda\x8b^\x14\xfb\xc3[\x15AK\x82\x87&H\
+\xb2\x9a4\x9b\xdd\xed\xbao\x9dy\xed.5\x84\xea\x83\
+\xe1\xbd\x9d\xd9\xf9\xceg\xe7\xcdJ\xf2\xd8\x18\xdc\xacT\
+`zv\x16$I\x02\xd7uA\x96e\xd0u}\x11\
+\x9f\xcbp\xc9\x8a\xe3\xb8\xc1\xec\xb55\x910\x10X\xbc\
+\xbf\xb2\xf2\xe8\xde\xdc\xdc2\x8f\xe3\xa1\xc9}\xdfo?\
+\xde\xd8Xg\x83\x01\xac\x0c\x9dn\xb7|gff\xb9\
+\xd1\xe9\x0cM6\x0d\x03^T\xab\xaf\xbf\xd4\xeb\xaf\xd8\
+\xc5\xaa\xb8\x95\x15E\x01]\xd3\x96\xb6\xf7\xf6\xc0q\x1c\
+`\x8cA\x14E`\x9a&\x5c\x19\x19\x81[\xf9<p\
+\xf4\xbd\xacV\xdf\xab\xaa\xfa\x8d\xfd/\xb2\x17\x04\xb0}\
+p\x00\x12\x9e\xc9z\xbd\x9e\xf03\x1f\x03T\xf9_\xc8\
+\xbb\x87\x87\xa0c\xe5v\xbb\x0d\xd6\xe8(\x9c$\x02\x89\
+R\x17\x85N<o\xa8\x00!\x7fo6\xe1\xee\xfc<\
+\xd1\x02\xc3\xa6\xd3m\xfd%@X\xb5Z\x0d,\xcb\x12\
+\xc1\x1b\x93\x93\xa9\x00\xc5\x02\xdf\x87\xdfa\x08\xe1\xe9)\
+0\xbc\xfa~\xbf\x7f&\x90\xa0\xc88\x03\xc5bQ4\
+,\x97\xcb\x81r\xe1j)FW}\x0d\xfd\xb4T<\
+\x93\xa0\x10HQ\xd0I\x04\xd9l\x16Z\xad\x16p\xce\
+S\xab,,\x88\xa6%B\x0a\xeeq\x10\xa8\x22/E\
+\xc1@\xa1P\x10\x09D@$\x166/\x89I\xe8\xa7\
+\x86\x1b\x9a\x06\x8a\x8a\xb9\x9c\x9b\x80\x14,AQ\xcf\x09\
+\xa8I\xd4\x07\x12\xbe:5\x95\xc6\xb2\x99\x0c\x5cGa\
+\x1a\xf7g[[o\xc1\xf3\xbe\xc2\xf1\xb1I\x1fN\xef\
+<l\xec\xef?\xa1\xea\x09f\xba\xa3iX1S*\
+\xed\xc8\x9c\x7f\x14s\xe3\xba\x9fy\xb3\xf9\x0e\x8f\xbf\x18\
+\xa2\x94Vm{\xe9\xd3\xd1\x91x\x91\x10M2\xc47\
+q\xac\x13\xe48\x0cw\xa3z\xfdy2\xb8h\xbe\xb0\
+\xdb\xb6\xbd\xfe\xc3q~F\x9c\xc7\xc3\x0c'3~\xba\
+\xb9\xf9\x06\xc6\xc7Wi\xa6\x06gD\x92'&\x1eH\
+\x86\x91\xbf\xf4\xb7=C\xfe\x80G\xe7\xdc\xd2\xf5G\x80\
+\x01\x00\x22*\x17\x8f\xde'kv\x00\x00\x00\x00IE\
+ND\xaeB`\x82\
+\x00\x00\x01\x8d\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01/IDATx\xda\xa4\
+\x93\xb1N\xc3@\x0c\x86\x9d\xcb\xa5\x055\x0c\x0c \xa0\
+\x8f\xc0#\xb00\xb2\xc0\x86\xc4\xc6\x88\x80\x9d\x95\xbcB\
+\x87\x82\x18\x91\x98:\xc2\x0b\xf0\x10\xbc@\x07\x90h\x14\
+\x05\x84T]\x14\xdb\xc1\xbe\xaa\xac\x97\x12K\xa7\x9c\x94\
+\xff\xffd\x9f\xed\xa8i\x1a\xe8\x12\x06:Ft{\xba\
+\x7f,\xdf\xbd\x7fx?\xb2\xc9\xdb\x8ben\x86\xd9\xe3\
+\xeb=q\xdd\xda\x19\x9b\x04\xb2\xf3\xc3K\xbd[b6\
+\x88\x15\x5c\x8d\xd7Z\x03\xee\xae\x1d\xa8o\x01 \x8e\x99\
+\x08\xca\xb2\x84\x8b\x93~\xd0\xfc\xf0\x5c\x01S\x0f\xd4\xe7\
+\x01Hl\x88\x10\xf2\xfc\x13\x98\x87A\x80\xea\x88vA\
+}K@L\x88P\x14\x85\xff\x11\x0a\xaf\xc3-\x05,\
+3\xa0\x18%\x03\xe7j\xc9\x80\x82\x00\xd5\xa9^}\x0b\
+\x00\x92\xcf I6\xa46\x0e\x02T\xa7z\xf5y@\
+\xad%\x08q0\xd8\xd6\x97\x0d\x02\xbcN\xf4\xf5_\x09\
+HV\xbb\x90\xa6;0\x9a\x84[\x98\xa6 \x99\xbek\
+\x06\xd6\x03~\xe6n\xdd\x9a\x08\x9en\xa6\xad\xe7\xc0\xca\
+ \xa9\xcf\xdf\xa7\xf9|vvt0^u\x8e\xbf\x1d\
+\xcc\xfc.\xc8\xe9\xc9\xd9\xd4\x09]\xc1\xaf\xed\xfa\x92M\
+\xae\xa2\xae\xeb\xfc+\xc0\x00\xa2\xb6\xad\x00\x7f!\xda8\
+\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x01\xc2\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01dIDATx\xdab\
+4.\xdfm\xc6\xc0\xc0\x00\xc2\xa7\xfe\xff\xff\x7f\x8a\x01\
+\x09\x00\xf9\x0c\xf8\xc0\xb9.7\x06&\xa0\x22\xf33\x1d\
+.\x09 \x1a(f\x09\xc4\x1a@,\x0e\xc4\xcc\x0cD\
+\x00\x16\xa0\xc6\xd3Fe\xbb\x18\x81\xecK@\xfc\x11\x88\
+\xc5\x80X\x0b\x889\x80\xf8\x0b\x10\xbf\x01\xe2wPq\
+\x03\x90K\x81\xf8\x04\xdc\x00(\xe7\x04\x16\xc3Y\x81\x86\
+\x834\x09@]dx\xbe\xdb=\xc6\xb0t'\x13\xba\
+\x01\xb8\xc0o ~\x0a\xc5\xa0\xf0\xf8eP\xb2\x03\xa4\
+\xf9\x22\x8a\x17\x18\x88\x04@\x03\x8e\x83\x5c\x05\xc4\xef\x91\
+\x03\x97\x85\x08\x8d\x0c\xff\xfe\xfd\x83\xc5\xc8[\xa8w\x88\
+3\x00\xa4\xe9\xcf\x9f?\xc8B\xef\x81X\x17\xc5\x05\xc0\
+\x80\xc1\xaa\x99GV\x8fA\xd84\x9c\x81KZ\x07Y\
+\xf8\x15H\x0a\x88\xd9\x80\xf8\x17H\x80\x09\x97\xed_\x1e\
+_bx\xb8\xae\x1aL\x83\xbc\x00\xc5\x7f\x80\xf8\x0b\x10\
+K\x80\xf8x\x0d\x80\x81\xc7\x1bj\x19\xbe=\xbd\x02\xf6\
+\x0e\x14\xbf\x06ba\xa2\x0d\x80\x19\xf2dc\x1d\xcc\x15\
+o@.\xf8\xfb\xf7/\xf1\x06\x80\x00\xc8\x15\xafO.\
+g\xf8\xfd\xfb\xb7,0`m\x80\x06\xb8\xc0\x0c`\x84\
+\xa6{Vh\xf2\xe5\x06b>h\x0a\x14\x02b\x11h\
+2\x96\xf8x~\xad$\xd0\x00\xa7\xfb\xb3\xc3\xdd\x81\xb4\
+\x17I\x09\x09\x06~~~sP4r.\x07##\
+\xe3^\x10\x9f\x91P\x96%\x04\x00\x02\x0c\x00\xb4\x09\xb6\
+\x061\xc1F\x81\x00\x00\x00\x00IEND\xaeB`\
+\x82\
+\x00\x00\x01\xdf\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\x81IDATx\xda\xa4\
+R\xc1j\xc2@\x10\x9d,\x06\x0d\xf4\xdcBK\xc1\x8f\
+\xc8\xdd\xb3\x01o\xd2\xfe\x81\xd0\x0f(^<\x15<H\
+?\xa0?\xe0%\xb1\xd0\x83G\xa1\xe0=\x81\xdc\x93\x88\
+Xl\x82'\x05\x115i\xd2\x995)KjcK\
+\x07^f\x98\xd9\x9d\xcc\xec{R\x92$\xf0\x1f\x93:\
+\x9d\x0eH\x92\xd4@\x5c\x8a\x05l\xfc\x8e\x18R\xdc\xed\
+v\x7flP\xda\xedv\xe4\xafz\xbd\xdeS\x964M\
+\x13\x06\x83\xc1\x1d\xc5\x86a\x14N\xc0\xd6\xeb5 \xd8\
+x<\x86\xedv\x0b\xfd~\x1f\x82 \xe09\xc7q`\
+6\x9b\x157X\xadV\x80`\xf3\xf9\x1ch\x1d\xdb\xb6\
+\xa1V\xab\xf1\xdcd2\xa13\xcf\x88\xdb#\xfe\x81\xaf\
+\xb0\x5c.y\xa3z\xbd\x0e\xd3\xe9\x14Z\xad\x16DQ\
+\x04\x98g\x8a\xa2P\xad\x99\xfeL\xcf\xf9\xc3#\xaa\xaa\
+\x0a\xf8\x0e78\xfe\xb5X\xa8T*o\xe5r\xd9\xb0\
+,\xabp\x85\x12}\xf0\xb2A\xab\xe4\x0d\x1b\xfc\x8eF\
+\xc6\x18\x87hq\x1cs\x9c\xa41\xe5\xbc\x81\x87\xbf\xe9\
+\x00\xdd0\x8d\xff\xa6\x03\xb2v\xbb\xcdu\xa0\xebz\xf1\
+\x1b\x90\x0e\x88\x85\xfd~\xff52\xadC:\xf0}\xff\
+\xb4\x0e\x5c\xd7\xe5\x9c\xd3$\x9b\xcd\x86\x83b\xcay\x9e\
+Gg\x16\x88\xfb#\xfe\x85O0\x1a\x8dJ\x9a\xa61\
+\xe2>\x9b \xd3\x01M\x80v\x9e\xfe\xec1\xe7\x0f,\
+\x10\xe5\xd5j\xb5)\xcb\xf2\x85X\x08\xc3p\x81\xc2z\
+\xa5~\x88\x0f\xc1\x13\xe2\x0cR\xca\xc4\x19B\xc9\x18\x14\
+.\xc49$\x82\xe7\xf8\x14`\x00\xf2\xa5\xe3%\x9b`\
+\x90\x1c\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x03\x01\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\xa3IDATx\xda\x94\
+SKHTQ\x18\xfe\xeec\xc6\x99\x9a\x11\x0c\x07\x02\
+\x1f\xa05\x9a\x0d\xbeH\xd3QF\x0dF\xd2\xf0\xb5q\
+\x11D\xeb\xa8\x96.JKj\x13\xb6\xad6\x85\x04E\
+\xa5m\x9c\x9c \xccAG\xbbI\x0b\x93\xc8b\x86\x94\
+\xc4\xc8\x071\xe0\x88\xe3xu\xee\xdc{;\xff\x851\
+]\xf4\xfa\xe0\xe7\x9cs\xcf\xff}\xe7?\xdf\xfd\x0f\xd7\
+\xd9\xd9\x09\xc2\x05\x9b\xcf\x189\x0e\xa79\xa0\x11\x7f\x81\
+\x0e\x04\x12I\xbc\x16S\x1f\xfc\xb2\x07\xcdf\x89\xa6-\
+\xde\xeeG\x97\xbf\x85\xc3\x88\xae\xad\xe1D}=\xd4d\
+\x12\x91\xe5e\x08\xa2\x08\x93\xc9\x04\x93\xd9\x8c\xb7w.\
+\xa5\xe9:D\xc1\xe5r\x19\x021\xfd\x00V4\x07\xd2\
+\xb4-\xd3\xd2\xe4S\xd9|\xf8xyym-\xc6}\
+>\xe4\x15\x16\x22\x11\x8f#\xb2\xb4\x04e{\x1b\xaa\xa2\
+ \xb7\xb2\xe9\xe4\xd7\xe9\xc06U\x90\xcf\xa2\x8a\x85\xfd\
+\x87\x96\x09\x8b\x9e]\xe4\xc8\xcd\xae-\xae\xa8@px\
+\x18\x95\x1e\x8f1z\x9a\x9a\x90d\xc4X4\x0aeg\
+\x07\xeb\xab\x8b\x91xB?(\xaa\xaa\xea\xee\xea\xea\xba\
+\xeap8\x5c\x91\xd0\x04\xe4/\x01T\xd7\xd5c\xa0\xbf\
+\x1f-\x1d\x1d\x18\xf5\xfbq\xaa\xb1\x11\xd2\xc8\x08\xca\x98\
+\xa8\xa6\xaa\xfa\xa7\xf7\xef\xa2\xf3\xd3c\x9f\x05\x1e\xafx\
+M\xd3\xd2\xe3\xf1\xb8kaa\x01\xb3\xfe{\xa8\xa8v\
+\xc3\xf7|\x10\xb25\x0b\x0f\x1f\xdcG]C\x03\x82\x81\
+\x00\x8aKK!\x05\x83\x18\x0dNqw\x07\xc7\xc7\xb6\
+\x14\xfd\x9c\xaa\xe1\xb1\xc8L\xd1\xbc^\xaf\xe1\xc3\xbcM\
+\x86o\xa0\x0f5g\xaf\xc0Y\xd3\x8e\xb04\x84\xe1'\
+\xb7\xd0\xda\xd6\x867\x13\x138T\xd6\x8e\x1a\xa7\x1b\xd2\
+\xfa\xed\xb1\x8f\xc0J\xf6N\x08b2\x99\xe4X\x15\xd0\
+\x99\xa5\xf9U-F\x10\xd8\xd5P\xc0Dh\xef\xe5\xb3\
+>\xe45\x9cG\xfa\x91*#\x8f8\x94\xb3(\x14\x18\
+\x02<%\xbb_\x1c\xc3T[\x08\x92$!##\x03\
+\x16\x8b\x05f\xf6\xbb\x8eV\xb7\x1a\x91\x02\xcf\xf3$\xc0\
+\xa7\xd6\xbb\x02\x93gfi\x03n\xb7{_\xc3\xd0\xb7\
+\xbd\x10\x04a\xbf\x80\xa2(<%}\xe8\xedAq\xef\
+M\xcc\xcc\xcc\xc0j\xb5\xee\x12dY6\xd6\xa9\xb1\xa4\
+\xa4\x04\xc4\xd9\x15H$\x12\x02UP\xd4}\xdd8\xad\
+\x94\xb9\xfd'P.q\xf6\x0a\x18W\xe8\x19\xca\xc4\x8d\
+\xd6U\x84\xa9\x85Y\xb3\x90\x0f\x84\xd4\xdcf\xb3!'\
+'\xc7\xf0\x808\xb4\xb7\xb1\xb1\xf1\xab\x82k\xcd\xdfA\
+\xd7u:\x9d\xbf=\x9d*\x14\xd9{ \xce\xe6\xe6&\
+\xe6\xe6\xe6 \xb2&2q\xec\x09\xd2#\xf9\x17P.\
+q\x18\xd9A\x16qv\xbb\xfd\x22s6\x0b\xff\x01V\
+q$\x16\x8b\x8d\xb2\xe9\xdaO\x01\x06\x00\x9b\xccJ\x11\
+{\xc3B\xfe\x00\x00\x00\x00IEND\xaeB`\x82\
+\
+\x00\x00\x02\x03\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xa5IDATx\xda\x94\
+\x92\xcfK\x02A\x14\xc7\xbf\xbb\xab\xd4JA\x04u0\
+(\xf3P'\xeb\xd0\xa1SQ\x9e\xbaU\x84%\x88b\
+\x98\x85Pl?!/y\xf4\xd6\xbdc\x9e\xfc+R\
+\xb1\xab-A\x91E\x1a\x86&t\xe8\xd0\xb6\xe4\x8f\xdd\
+\xb6\x99\x0aA\x1c\xc4\xde\xf2\x19\xde\xf0\x1eo>\xcc\x0e\
+'\x1c\x09\xf8\x09\x0e\xa7d\x9dDgq\x0d\x03\xfb\x8d\
+\xdd\xa0\xcd\x06W$\xb2it\x18\xc2\xa1pA\x00\x85\
+\xfb\x9b\xb1\x99\xcb\xe5\xce\xf2\xf9<(\xc1`\x10O\xe5\
+\x0a\xf3\xe8Q\xab\x08\xf3\x81)ARgSa)\x1c\
+\x0e\xe9__\x86\xa6\xebm\xa1=\x82$$\x08\xa00\
+\x0d\xd6\x03\x01\x14\xcaU\xb6\xc1\x90\x88.\xc9\x9c$\xe9\
+|Saaoo\xbbFN\xa8\xd4\xebm\xa1=B\
+HH\x12@a\x1ax\xfd~\x14^jL\x03\xfb\xb0\
+\x05b\xc8\x9c\x22\xe9\x5cSankk\xf7S\xd3\x0c\
+\xa5Ri\x0b\xed\xe1\x03|\x8a\x00\x0a\xd3`\xcd\xe7C\
+\xb1Tg\xdf\xc1\x88\x88\xde\x8d\xae4Ig\x9b\x0a\xd3\
+^\xef\xa1R\xab\x19o\xaa\xda\x16\xda\xc3{\xf84\x01\
+\xae\x09\x8em\xb0\xe2\xf1\xa0X\xd4\xd8w`\xb7\xa0\xcf\
+\xdb}y\x920f\xc6_\x8d\xc6\x008\x96\x97\x8f/\
+\xe3\xf1h\xb5\xda\xfa\xfb\xb2\x92\x04E\x96\x7f_<\xcf\
+\xe3\xee\xf1\xea\xc3\xfa\x8e{\x03\xc80\x0d\x16\xddn\x94\
+\x8azc\xc0\xed\xaa\x13\xae\xa9\x89\x96\xc1\xe7\xb1Xc\
+\x00z\x1d\x8ehI\x96\x8f5\xadU=\xb5\xb3\x83r\
+&\xf3k\xc0q\xb8\xc9f\xd4\x01\x15\xd9\xe7?\x83~\
+\x82\x15c\x08\xa3\x87\xac\x9d\xc4\x07\x1e\xc8\x17%\xd9\x0b\
+\x1d R\x01\x82\x09\xff\x0b\xaa\xaa|\x0b0\x00@\x99\
+caMt\x03\xde\x00\x00\x00\x00IEND\xaeB\
+`\x82\
+\x00\x00\x03\x0a\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\xacIDATx\xda|\
+SKL\x13Q\x14=of\x0a\xa5tZ\xa4i\xa6\
+\xa5\x09\xa5h\xb0\x01q\x0d.\x5c\xd4\x18\x17\xa8\xedB\
+\x13b\x8cqaR\x97\xee\xdc5)\x0b\xe2B\x13\x12\
+M$\xc4\x15H\xdc\xb0T\x83\x92\x18\xdd\xb8\xaeF\x92\
+Vj\x80bPLKK?\xd3\xcf0S\xef\x1b>\
+\xd6\x1f79yo\xee\xbb\xf7\xbcs\xdf\xbd\xc3\xae\xc4\
+b80\xc6\xd8%Z\xbc\xf8\xb7\xbd1\x0c#M\xf8\
+\xcd)5\x9b\xcd\xc3\x0f\xda\xf7<\x89\xc5\xa6\xd5z\x1d\
+:\xf9\x0f\xce\x12\x89\x04f\x97\x96n\xf3;\x08+\xad\
+\x04\x82\xa1\xebh\x01ct\x83\xdeh\xa0Z\xa9\xa0\x5c\
+.\xa3T*\x99\xeb\xc2\xc4\xc44\x9d\x9f\xab\xa9j_\
+!\x97\x03\x07\xcbf!\x08\xa9\x94\xb9\xd1\x89\x80\xc0D\
+\xc6`\x95$t\xb4\xb5A\x12\x04^\x16\xb6\xb7\xb7\xf1\
+h~\x1e\xa1\xc1\xc1\xc7\xe9d\xf2\xfa\xd7\xf5u\xb0}\
+\x02\xc9\x94A\x01\x96j\x15uE\x11\xb8FQ\x14a\
+\xdd\x97X%5\xa1P\xc8,G\x96e\xbcJ$\xf2\
+\xed[[`\x14\xcf\x0b\xe4\x04\x02a\x8c\x1c=\x8bS\
+S\xfdq\xc6p\x94\xf1\x98H$\x12\xa5\xed&\xe1\x85\
+\x18\x0c\x06]\x84p<\x1e\xbf_,\x16G\xddn\xb7\
+)[\xa22Za\xaa\xb2Z1000:99\
+y1\x9dN\xa7\xb2\xd9\xec'I\xd34\xb7\xc7\xe3\x09\
+P2\x0a\x85\x02\x1c\x0e\x87\xb9\xd6\xa9\x13\xc5b\x09\xdc\
+_\xab\xd5@qp\xb9\x5cp:\x1dX^^\x81\xdd\
+.\x07x.'P|>\x9f?\x9f\xcf\x83\x18\x89\xc0\
+\x89\xb5\xb5\x0d\xa8j\x15\xbfZ,\xc2b\x11\x89\xc40\
+cj\xb5]tv\x1e\xf3\xf3\x5c\xa9\xd1hx\x88\xa0\
+\xb7Bm\xcb\xd1\xcbvw{`\x18\x12\xc9\x95\xff\xaa\
+_\xa0'.\x0f\x8f\xe3\xd9\xd0gD\xaa}\xbd<W\
+\x22\xa9n\x92\xdc\xcf\x93\xb9\x0a\x9e\xdc\xd1!\xff\xf7\x11\
+s6/\xca\xaf\xbd\xf8\xd2\x95\xef\xe7\xb9\x9c\xc0j\xb3\
+\xd9I\x16\xb5b,\x0c\xbf\xff$\x91\xf0)\xdc\xeb\xc6\
+\xdb\x8a\x17\xf5N\xe5\x90\xa0\xbdQ\xc7Xx\x18\xcf\x17\
+>\xa2\x1a8\x7fFRU\xd5\xa2i\x0c6\x9bL\x03\
+\xf3\xc3D\xab}\xf3^\xc5\xad\xe8(\x92E\xa0\xb4\xbb\
+\xe7{\x9f\x05\x82\x17N#\xb5\x9a9\xcb\x9cN\xe7\x1d\
+j\x91\x9b\x1f\xec\xec\xec\x88\x99L\xe6\xee\x8dYRs\
+\x8anc+\x98y\x97B\xae\xd8EmlC\xc0\xe3\
+\xc4rz}\xebx\xf4\xa6\xb2:3\xf7\xbd\x91\x5c|\
+\xc9\xf3x\xc1=\x1c\xca\xc8\xc8D\xf3\x0f\xd3\xa9\x1e\x0e\
+M\xd7\x9b\x1a\xad\x8e\xf1\x99M\xf9\xda\xdc\x07{\xf8\x01\
+\xff\xb9d>\x89%\x8evEA\xa5\x5c\xde\xb0\x0f\x0d\
+\xdd;j\x12w}\x97CM\xfb\x89\x87\x96&\x9e\xf2\
+\xef\x9f\x02\x0c\x00`\xb3o\x8c\xe2\xe0=\xdc\x00\x00\x00\
+\x00IEND\xaeB`\x82\
+\x00\x00\x02h\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\x0aIDATx\xda\xa4\
+S;o\x13A\x10\x9e\xbd\xdb\x9c\xef\xec\x84G\x91&\
+(\x91\xf9\x01\xa6#\x15\xb2@\x0a\x14\x01\x81\xe8\x82\x10\
+\xc9O\x88\x04U\x1a$h\x10\x05\x91\xf2\x03(\x12S\
+\xa4\x22\xa2H\x0a\x08\x02\xae\xb2\xa0\xc3%M$dL\
+\x04\x81\xc8\xce=v\xd7\xbb\xcb\xcc\xd9\x17\xc5\x81\x02+\
++\x8d\xe6\xb1\xdf|\xbb3\xb3\xcb\xac\xb5p\x92\xc5/\
+.m\x93\xbe\x8a<\xe3\xc3$2\x06?P\xbd\xe1\xae\
+\x93\xf9\x93[K\xd5\xc5\xae\xb1\xe2\xbfNuXa\xf6\
+I\xb8\x92\xd9^\x8f P\xda\xa6\x9fw~\x7f}\xf6\
+\xaa\xd1\xc8\x81\xab\x8b\xd5Y\xd2\x0b+\xe1V\x1e{p\
+\xabR\xb9P>;\x89y\x01\xf9\xce\x88c\x01%\xc0\
+\x9b\x8c<\xddh|4\x16\x1e\x91t\x0d$\xd8\x1fC\
+Bv\x1e'\x0ca)\x87r\xb9\xcb\xb2zv\xef.\
+\x87/\xd1\x0e\xa9\xa7\xa9fD\x1e\x19c\x0d\x19R\xb3\
+\x88\xb4\xefZ \x0cb=\xee\xc0.ay\xfff5\
+J\xa1yH\xc30!\x8bE\x892B*\x93\xa2\x9f\
+\x118xR\xc1\xb5u\xc4\xd6\xf3\xd9\xf1\xe3\x0d\x8a\xe4\
+\xa1\xa9Z\xfbI\x0bY\xad6\xa0\xf2\xbdB0\x88w\
+\x8e:i\x97\x0d\xeeYF\x05:Gq\xc70\xc0\xbf\
+4\x7f\xc1h\xe0\xc1\xe9\x92\x0f\x9aq\x1c\xd1\xe1\x9e\x8f\
+\xe2\xf6\xc6f\xfd<H\xe5y\x18M\x85\x82V}\xbd\
+WB,\xbap\x90\xb4\xe1\xccX\x91\x9e\x08\x8c\x15=\
+\x0a\x97\x80\xd9\x8c\x00\xbb]\x22\xdd\x89e\xd6\xa9\x9f{\
+\x09$BB\xf3}m\xb0\x07\x9dX\xe0D\x18\x9dX\
+>U\xf4J\x0c\x18g}\x82v,\xcb\x07\x89\xdc\xa1\
+\xa7\x9f\x0a\xf9\xef\x1e\xf4\xd7\xed\xfdH\xde\xb8\x5c\x99\x18\
+M\xa4\x16\xb1\xd2\x82l\x8a\xd1\xde_\xaf\x12\x19g\x8c\
+1WP\xbf\x93Rn\xbb\xae;\xf5\xfa\xf1\xf5\xb9X\
+\xea\x04K\x8b\x09tszjz\xee\xd2\xf9\xe2\xb5\x87\
+\x9b\xebZ\xeb\xc1?11\xbf\xb6\xdc\x5c\xbdW=\xb7\
+P\x0b\xd1\xff>\xcc\x87\xfa\xb66\xff\x82+\xa5\xde\x8e\
+\xdfy\xee[\xd1\xfe\xb0\xb7q\xff\xd3\x90\xbf\xb9\xf3G\
+\x80\x01\x00\xd0*\xf6-\x03e\x5c\xa6\x00\x00\x00\x00I\
+END\xaeB`\x82\
+\x00\x00\x02\xbb\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02]IDATx\xda|\
+SMh\x13A\x18}\x9b\x84\x0d\xd4\xd4\xc4\xa4\xda6\
+`h@\x8bM5\x0a\xa9^,=\x88H1\xe2\xa1\
+'\x05A\x8b\xd2^\xa4\xea\xcd\x83\xa0\x07\x0f\xeaE\xaf\
+\x82X<)\x22zR\x14\xc4\x82\x97Z\x9b\x05c\xad\
+\x16\xb5M,6\xc56\x0d.i\xba\xb3\xff~\xb3\xf9\
+\xb1m\xaa\x0f\xde~\xdf\xbc\x99y3\xf3\xed\x8c \xdc\
+x\x8b5\x10\x84\xe3\xf4\xbd\x83z\x5c\xb4\xdb\xfa\x92\x14\
+\x13D\x09\xb6=\x88\x92\x05\x0f\x0cs\xfd\xc0\xa1\xfd\xf1\
+][#\xad\xcd\xbe\xaa0;\xffky\xfc\xe3\xd4\x10\
+t;p\xeeh\x7f\xe2\xde\x8ba\xc0\xb4\x9d>\xcf\xe9\
+\xd7\xf7\xf1\xa0\xe7\xd4j\x83\xb6M\xa2\xc7\x97\xc9dj\
+\xc2\x9c~\xd3g7\x8duC\xb5>\xc9\xa6\x0c\x8a\x5c\
+N\xc1\x86$\x8cP\x96\x8e\xec\xc1\xa5\x13\xd7\xab\xe3\xbf\
+u\xf7\x1c\xd8Q,\x16k\x06\xd3\xa5~t%\x9b\xeb\
+\xce4\xf2\xf4\x8d\xe4>CI\x8b\xbc\x80}?&\xf0\
+j\xe7A\xc00\xce\xb7no\x0d1U\x85eY\x0e\
+\x99:\x85\xcf\xef>\xb0\xecd:\xed\xebh\x0c\xbf\x7f\
+4*e'f\xe6\xe9\x18\x92\xab\xea\xb6\xf7\xe7$n\
+?\xb9\x06(\xcc\xd2t\x1d\xfa*F\xb6\x5c\x810s\
+9\x0b\xc5B\xc1,\x80G\x18v\x17\x1da\xd0E\xa5\
+\xe8%\xa68\xe3\xb9/\xa9\x93\xe3\xcf\xfc\xdcP\x14\xc5\
+\x1a\x1d\x94V\xacmL\x95r\xb7\xbeJ<v\x8a\x0a\
+:\xfd*<\x060\xb0;y,\xda\x12\x8b\x05\x9d\x82\
+-\xb9\xa1?\x1cv\xe6L\x94f~\xcb-\xe5\xf9\xb1\
+p.\xd0\x11\xd7\x13\x95\x0d\xf3\xd8k\xdb\xc6K\x8f\x06\
+D|\x0bZp\xf1\xf9c\xa7\xe7H\x85\x1cw\xfb\xb2\
+\xd3\xe2\x85\xc3\x89h4J\xad\xf6\x001\xcc\xf5l\xee\
+{a4=2@\xa9c\x00\x8d1h0\xea\xaa\xac\
+\x91\xe4\xa1\x22\xe6\xf3y\xc8\xb2\x5c\xd3\xfd\xfe@Pc\
+\x888\xf7\x80\xd1\x87\x91\x01C\xdd\x85\x82J\x06\xa2a\
+\xd0\x8f)\xb3\x0a\x9ek\xac\x9c;\x06\x9a\xa2l\xb8\x03\
+FR\x83iB\xd7t\x98\xe6\xdf\x05x\x9b)\x15\x03\
+\x1e-\x97\x0b\xeeP\xa0\xde@_,\xaf\xa6kkv\
+\xc0\xdbl\xa5b0F\x17qn6\x8d\x8dP\xa0\x02\
+5Q\x0d\x04A\x80\xd7\xeb]\xf5\xde\x04(\xcb\x95\x9c\
+\xd8@l$\xba\xd7\xcdo\xdc|\x08W]!\xb4o\
+dn-!M<+\xe0\xff\x08\xffC\xe7\x05\xe1\x8f\
+e\xe5\x8f\x00\x03\x00F\xb8\x1d7\x90|\x0e\x07\x00\x00\
+\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02o\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\x11IDATx\xda\x8c\
+SKk\x13Q\x18=w\xe6fJ\x9b\xb6N\x1e\xcd\
+\xc4\x075\x1a#\x8aP\x84\xec\xa5\xa0\xfe\x06\xd7A\x85\
+\x8a\x0b\x17\x05\xd1\x85\xcb\xaa\x0bK\x17E\x10\x04\x05q\
+\xdb\x8d\xaeDA\x10\x05-\x88 jK\xa4$i\xa7\
+\x09IM(\x1d\x9a\xc7Lf>\xef$\x99\x10\xb5I\
+\xbd\xcc\xe1\xbb\xdf\xeb\xcc\xb9\xf3\xddaoS\x1c`\xad\
+g\x06@\x1c\xed\xb5F\xc0\xa3J\x95\x10\x1aa(\xf7\
+\xb1$\x8a\xb8[-\x9a]\xe7\xc4\xb9[\xcffm\xcb\
+\xc2\x87\xf9\xcb\xf3\x8c\xe1\xbf\x16\x17$\xd7@\x88\x17\x0c\
+\xba\xb8\x91NcB\xd3\xe0\x00\xd3\x12\xe1\x81\xc8\xa9\x82\
+x{\x80]\xe3\x8d&\xce\x5c\xb8\xfd\xf4z\xfa\xf5s\
+D''a\xd5j\x88\x9e=\x9f\x8cO_J\x16\xb2\
+Y\x1c\x8c\xc5\xb0\x97=\x92H\xe0\xcd\xbd\xd4Ci\xd7\
+\x22\xffN\xb1\x88\x9c^F>\x93\x81c\xdb\xa8\x1a\x06\
+*\x9b\x9b\x18\xf2\xf9\xfaZ\xb7\xc7\xed\xe5;u\xd2\x97\
+\x16n\xbe\x08\x8e\xb0)\xed\xf0\x95\x98)\x14\xe4\xbe}\
+\xca~Y\xfe\xf8u\xdf\xf3K\xd0y\xd3\xc1\x1d\xd7\xc9\
+W\xe8Ia}=\x15\x08\x061$\xe3\x95\x08\xcd\xd4\
+,\x1aH0\xecc\xe0~\x85\xc1\xaf\x08o\x14\xf6D\
+4\x8a\x86P`\x13\xe4\xc8(C\xd1\x00\xea\xcd\xc1$\
+\x5c\xdf\xea\x16(\xa7u\x1d\x07T\x15BUk\xbc!\
+?\xc3\xaf]\xa01\x80\x84\xc7\xb4\xee\xc0Y8\x12i\
++p {\xc1\xc00C\xa5\x0a\x98\xf6\xde$|u\
+\xc3\xf1\xf6\xf2T>\x8f\xb1\xf1qq\x04\x92{\x8b\x16\
+\x97\x09?J\x7f\x12$B\x0c\xa7\xc2\x04~\xfcPW\
+\x01\x0f\x85\xc3\xa8\xb7\x15p/x\xf7\x1dae\xeb\xdf\
+\xb7\xff,\x93\x00 \xcd\xbet\xf0=C.\xa4\x92\x98\
+\xad\xe380\x9bP\x040\xd7\xa7\xb9wI%\x13X\
+\xca\x01Q\x0d\x01M\x5ccEQ`\x984v\xff=\
+au\x9ff\xef?:\xea~\xf0\xabI\xdc8\xa6\xe2\
+\xa4\x1b\xcclc\xe5\xf1g\xcc\x89\xad%`v\xac\x07\
+\xa1\x0d\xb6\x80\xe3\x11\xa8\xee\x9d\xe8\x10R'\xe1\xc1\xee\
+)\xb6\xff\xca\xb5\xe4\xfd\x16`\x00\x1d\xfa\x0d\xd8wp\
+b\xe0\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02\x18\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xbaIDATx\xda\x8c\
+S?k\xc2P\x10\x7fI^b\x84RP\x84\x12'\
+\x05]\x9aZ\x10\x87b\xd7.\x19\x94\x0e\x9d\xfa\x05\xfa\
+\x15\x84\xd2\xcfP\xbatr*8\x95\x8e\x0e\x82S\x97\
+.\xddD(\x14\x073\x08\xa1`\x03\xc5$\xc6\x9a\xa4\
+w!\x89\x89\xb4\xa9\x07\x8f\xdc\xbd\xbb\xdf\xef]\xee\x0f\
+\xd3\xeat\x08\x0a\xcb\xb2D\xe0\xf9&\xa85\xb2\xa3x\
+\x9e\xd7\xa71\xa3y\xd5n_\x9f5\x1a-\xd0S\x81\
+\xa6m\xcfo\xba\xdd\xdb\xa9\xa6\xf1\xf4{\xb5\x0a\xefk\
+\xcdz\xbd\xf5i\x18\xa9`!\x93!\x0f\x83A\xff]\
+U\x1f)\xcf\xab\xd4Z.#\xe7\x17\xe8\x8b\x7f\x08\xf6\
+\x18\x86<\x0d\x87/\x1c\xc7M\xd6\x8eC\xa8i\x9a\x91\
+s\xed\xbad4\x1e\xfbz.\x97#\x96e\x91r\xb9\
+\x9c \xc0\x988&A\xc0\x02{\xa5RI\x00\xf0n\
+\xdb\xfe\x93\x80\x01\xe7t:\xf5_\xd7u=\x01\xc4\xbb\
+%\xfc\xe2\x91,o\x11@\x9a\xa1p@P\xadV}\
+\xbdP(\xfcZ\x03\x8c\x89c\xa8\x157\xc0\xa9\xaaj\
+\xe2U\xcc\x04\xbf(\x18{\x10\xd4&\xc2\xd8\xb6\xbda\
+\x87a\x0a3\x08\xa5$I\xc9\x0c &\x8e\x89\xcf\x01\
+C\xc1\x895\x88w\xe1\xb0TJ\x10`\x0c`\xa2\xca\
+RoC@\xf1\xffN\xa0Hi\x821\x80\x89&\x98\
+\x12\x1c\x1cQ\xf4\x87\xcc\x80\xea\xba\xd0gl\x15v\x04\
+\xf7\x03u\xdf\x0et$ \x8e#\xf8h\xe8\x0a%X\
+\x10Q\x94\xcf\x15\xe5t4\x99\x10\x9e\xe3p\xa9H\x06\
+\x8f \x1018h\xe3}\x90\xbb\x88`2\x9b\xc1\x8f\
+\xe7\xf3\xb2\xac(w\x1f\xf3\xb9\x0e\xaf{\xa9\x07\xb6\xec\
+\xbe\xd7{f$\xe9\x02H\xf6\x91\x88a\xb2\xd9c\xb6\
+X\xbc\xdcy\x85\x0d\xe3\xcd\xd5\xb4W\x5c\x1d8\x8b\x1f\
+\x01\x06\x00\x7f\x92\xd60_\xf0?_\x00\x00\x00\x00I\
+END\xaeB`\x82\
+\x00\x00\x02r\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\x14IDATx\xda\x8c\
+RMk\x13Q\x14=of\xde\xa4\xd3\x98X\xfb\x09\
+\xa5\xda\x8dTD\xe8O0\x8bF\xbb\xea\x0fp!\xe2\
+\xd6\x9d \xe8F\x14\x5c\xbb*TA\x90\xa2 \xba\xf1\
+\x07\x08Y\xd4\xe2\xda\xa2dQ\x92E\x93R\x95DB\
+\xa6\xf9h\xd2f\xde\xf3\xdey\x99d,\xa9\xf8\xe02\
+o\xe6\x9c{\xee\xb9\xf7\x8e\xc8<\xc9\xa1\x7f\xd6(\xe6\
+\xf1\xefCd]\x84\xd6(m\xbd\xc5\xde\xd6\x1b8\xf4\
+!\x02\x17^\xdf\xcfl\x1cu{\x08\x94B\x10h(\
+E\x986x\xa1T\xc1\xcb\xdc\xde=\xba\x0a~]\xcc\
+\xdc\x06\x87\x15\x12L\xd8\xdd\x93\x1e\xfcv\x07\xf5f\x07\
+\xb5\xc36*\xb5\x16~\xfen\xe2G\xb5\x81F\xb3\x8d\
+w\x0fW6\x88\xb7J\x02KQ\xd5\xbf\x04\x84\x10\xb0\
+,\xc0q,Hi\xc3u-\xd8\xb6\x05\xfe^\xad\xd5\
+\xb1\xf9q\x1b7\x97\x12\xeb\xa2U}L\x01\x8ex\x0b\
+6\x9b3\x22:\x14\x89\xce\xf11\xb0|\xf52\xd5\xd0\
+\x98\x9fI\xe1\xd3\xee\xd1\xd7\x08s\xa0\xd5\xe0N\xb9\x94\
+,\xa8w\x8c\x14\x09\x82>W+'&\xa0\x87\x02d\
+!j\xe3,\x11p\x15\xad\x9dQ\x0e\xa4q\xc0\xc9\x02\
+\xdd\xd6gt\x9b\xdbfP\xf2\x12d\xf2\x96\xb9[,\
+\xa0\xe4\xc8\x16\xe23h\xd4r\x98\x98\xbb\x0b\xc7]\x0c\
+{W}\x9am\x8b\xd3-\xc4\x1c@\x0cf\xe0\xa5\xaf\
+\xe3W\xe9E\x08\xa4'\xb3HM\xae\x84\xed\xf0V\xce\
+r \x8d\x03c\xf3\xc2\xcc\x0dLLg\xd1:,\xa0\
+\x5c\x5cGz*\x1b:c\xfc\x94\x80\x8e90-\xf0\
+j\x8b\xf9\xe7h\xf8\xbb!0\xb7\xb06pf`=\
+\x14\xf0\xcb\xdfq\xfe\xe2\xb5\xbe\x03a\x08d\xe5\xca\xf2\
+\x83P\x9b\x7f\xe7h\x06<`n3r\xe0\xef\xe7a\
+\xed\xbc\x7f\x0a\xbf\xfc\x0dB\x9d$#\x07B\x0c\x9f\x5c\
+9Z\xed\x00#.\xe7p./\xd9\xdb\xf9\xf0l\x16\
+\xbd\xce\x94C,\xcf\x91\xf0\xa4\x8bq)1\xee\xbaH\
+R\x9c\x1bs\x91\x1aK \xed%\x90\x90\xb4\x00\xe2\x86\
+9\x94\xcb\xeb\xf0(f\xeb\xe5|\xe5\xce\xa3W_\xf0\
+\x1f\xa7~P\xa8p\x0eE\xef\x8f\x00\x03\x00\xd3\x8c\xe5\
+O;O\xe1r\x00\x00\x00\x00IEND\xaeB`\
+\x82\
+\x00\x00\x02\x17\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xb9IDATx\xda\xa4\
+S;K\xc4@\x10\x9el\x12s\x069_\x95(\xca\
+)X\xa8\x8d\x87\x8d\x22d\x9b+\xe4\x0a\x7f\x80\xb5\xd6\
+\x96\xe2/\xb0\xb4\xb6\xb7\xd7B\x10l\x12\xf0\x10\x1b\xc1\
+\x07\xa2\xe2\xa3\x94\x03\xd1\xcb\x9d\x17M\xf6\x928\xb3g\
+\x0e_w\x16\xb70\xcc\xee\xcc7\xdf|\x9b\xcc*q\
+\x1cC;K[\xd9x\x96\x0c\x8a\xa28\xb5\x9a\xe0\x9e\
+\xe7\x81\x10\xe2\x17P\xd7u0M\x134M\xb7\xb1\xa9\
+E\xb1\xad\xb5>E{{\xf3\xb0\x989\xbe\xff\xce\xc3\
+0l\xda\x89H]\xd7\x05UU\xb9a\xa4\x90$B\
+\x92>\xd0\xb0\xa3\x83\xdd9\x02l\xc6\x98\xf5\x9fd\xc4\
+9\xd8\x88\xa3\x0a[^!\x8a\x22^.\xbb\xb4\xb7\x0e\
+6G!\x8cD\xd3b\x95\xe9\x90[\xbd\x97M\xd2\xe9\
+nN\x9e\xb9n\x09*\x95\xb2\xb4@\xbc\xc3\xd9q\x01\
+\xdc\xe7\xa7?=\xe5\x13,\xd5I\x05\xc5b\xb1\xd1!\
+\xc4{\x0ee\xc6\x80\xe9*d&&d,\xf1\x83\x18\
+\xa7|\xb5\xea\xc9s\xe2\x99\xef\x0bHL\x88\x00\xee\xae\
+.!\x08\x82_v\x8fq\xca\x7f\xc5K\x05q\xcc\x1a\
+\x0aj\x08\x18\x18\x1e\x91\x05?\x17\xc5)\xff\x15/\x15\
+\x98f?\xfe\x9a\x944\x02<\xdc\x5c\x83\xffZ\x85\xdb\
+\xf3\xf3o\x9e\xe2\x94O\xb0T'\x15\x18F7\xb2*\
+\xf5\xaf\x0c1\x8cON\xca\xfd_\x9e\xf2\x1d\x1d]\xf2\
+l\x18\xe9:\x01\x0e\x91\x1dy\x0f8D\xe2pa}\
+f\x1eg\xae\xf5\x1cTN\x0b\xaa\xaa\x83\xd29Ms\
+\xc0QA\x97\x95\x1a\xb4\xec\x8b\x83\xa5\xdc\x8d\xbd\xdcK\
+S\xdd\x8a\xa0g`\xeee*\xb7\xfd9\x89\xa8\xe0S\
+\x92\x95\xcd\xef\xec\x97\x1e\x8f\xf8\xc9\xdeb\xd3\xe2l~\
+\x17\x09f\x1boA\xbe\xa1v_#\x836\xd7\x87\x00\
+\x03\x00\x9b/\x02\xcc\xf69c\xa8\x00\x00\x00\x00IE\
+ND\xaeB`\x82\
+\x00\x00\x02\x1e\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xc0IDATx\xda\xa4\
+\x93=/\x04Q\x14\x86\xdf{wv\xcc\xb0>\x96\x84\
+\x15\x85\x84\x8aP \x94\x12\x05=\xbf\xc3\x1f\x90P\x88\
+R%\xd1\xf9\x19\x14\xa8\x04\x0d\x11\x85\xd0\x90X\x95\xad\
+ve\xc7Z\xcb\xdc\x0f\xe7\xdc\x1d\x8bh\xc8\xde\xe4\xcc\
+\xdc\x99\xb9\xe7\x9d\xe7\xbc\xe7^a\xadE3C\xa2\xc9\
+\xe1]\xecJ\x08\x81u\x9a\x8f\xfe1g\xcb\x18\x9cR\
+\x80\xe1=\xbeP\x8cM\xcc\xee,\x19\xf5Ls\xfe\xa2\
+aL\x0c\xad^\xa1u\x0dF\xc7.\xb3P\xb8\xc7K\
+q\x8f\xa9\x05\xc5\x89#`%\xf7\xc2\xbc\xc1\xc4ON\
+\x80}\xe1\xbb\xd1\x0a*\xa6P1\x09j\xd4j5L\
+\xcf\x1f.\x9d\x1d,\x88D\xe4\xf8K\x00\x5c\x8aHl\
+1\xee\x9eJy\x0dn\xa5\xde\x11E\x11\x8e\xf6W\xe9\
+if\xb1\xf8x\x9e\xa5\xc9\x9c\xa7u\xddL!$\xae\
+\xae*\xf4g\x8dL\xa7F\xb9\xa4\xd0\xd3G\xe8\xcaG\
+.\xd7\xe6\x16\x8d\x8cL9\x92 \x08p\xa3\xce#W\
+\xc2w\x81\x81a\xe9\x8c\x01EG\xb6nR\x98\xf6\x7f\
+\x91\xf0\xa0<\xd7AO%\x02 \x81B\xbe.\xc0\x91\
+\xe9\x02\xcaE\x9e\xbf\xd1\xe2\x0a\xda2Ug&\xd9\x80\
+\xb1\xf1A\xa8O\x81/\x02\x81\xfe\xa1dk$\x22L\
+\x11\xa6\x03\x84~K\xc3XM\xc6\xcaT\xcbo\x02A\
+\xcf\xd4%7\xda\xb3\x12Q\x09\xe8\xc9\x11j5\x85\xd6\
+\xde\x9f\xc6J/\xfcF\xa0>K\x10\x98\x9c\xec\x82M\
+L\xb0\x83\xb6\xd1Rc\xcc\x8f\xeeH\x99\x06\x838\x81\
+\x95M\x8b\xb5e\xf8\x90\x1d\x10i\xea'\xa3\xf2BJ\
+\x16\x09\xb6\xe0\xcd\x05\xe3:dILH\x1f\xd5W\xeb\
+ol\x93\xc0\xcd\x1d\xba/\xaf\x91\xafl-\x06\xff9\
+\x03\xb7\x0f\xc8s.\xef\x9c\x90\xcbf\x9a\x7f\x9e#.\
+\xfeY4{\x9c?\x04\x18\x00\xfb\x1f\xf0\xdf\x8a\xf9\x97\
+K\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02\xd2\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02tIDATx\xda\x8c\
+S\xbd\x8f\x12Q\x10\xff\xedGXva\x81\x83\xe3\x92\
+#\x16\xc6\x82\xe4h(L\xce\x0a\x09\xd0\x98p\x96\xc4\
+\xca\x86\xc2\x90\x98\x5ccO\x82&\xc4\xbf\xc0\xc4\xe4\x8a\
+K\xfc\x0f\x5c\x0b;C\xe1\x07\xa8\xed\x15\x5cI@\x91\
+\xcf=\x04\x0e\xdc\xdd\xe7\xbc=\x8ep\xe7\x15N2;\
+\xef\xcd{3o\xe67\xbf\x15\x0a\x85\x02V\xf2\x90t\
+\x17\xff'?H\x0d\xbe\x90/=\x8b\xc5b\xf7\xe8\xe8\
+\xe8\xf5t:\xc5|>\x87e\xd9\xe8\xf5~\xd3\xda\x81\
+\xd7\xabB\xd7u\x04\x02\x01\x04\x83\x01\x94J\x8f\x9eJ\
+\x92\xe4\xc6\xc9'''H$\x12\xee\xc6\xb2,\xd4\xeb\
+uL&\x13\x84\xc3\x11\xccf\x0c\xe7\x0b\x07>\x9f\x0e\
+\xcb\xb6 J\x224\x9fz\xa5\x14\x91'\xa8\xd5jk\
+\xc7`0@&\x93\x81i\x8e)\xe1\x12\x8c|Lp\
+.\x14\x17\xba)\xbc\x85B\xaf\xd7\xbbe\x18\x06\xb2\xd9\
+\xac\xeb\xec\xf7\xfb\xd8\xdf\xbf\x87\x8f\x9f\xea\x14\xe8\xa5 \
+\xb6\x0a\xb6]\xbd\x92@\x10\x84;\xa7\xa7\xa7/7\x9d\
+\x8e\xe3`4\x1a!\xbc\xa5\xa3\xddn\xe3g\xbb\x09\xbf\
+\xdfO\xfd\x07\xd1l6\xdf\xd3\x95o\x97w\x05\x02\xe3\
+1\xd9\xdb|S\xa9T\x9es\x9b\xcb\xe5\x10\x89l\xe3\
+\xf3\x97\xafP\xfd[\xd0\x098\xbf\xeeC\x90@\xe4@\
+\x1e\x96\x8a\x1c\xc4W.\x06\xa4o\xa2\xd1\xe8\x8b|>\
+\xdf-\x16\x8bX.\x97\xa0=\x0c\xe3-\xcei=0\
+\x87\xe8\x0e\xba\x18\x91\x9dL\xcf\xf0\xc7Z\x5c\x05qo\
+o\x0f\xa9Tj\xed\x88D\x228>>\xa6$;P\
+5m\xdd\xbb#\xd87c\xc0\x13lJ:\x9dv'\
+\xc1y\xd0\x1d\x8e7&@IVz}\x0a\x97\xf2\xbd\
+Z\xad\xbeK&\x93\x07\x1c\xc4\xd9l\xb6Jd\x11\x91\
+\xbc\x18\x12\x88}\x02\xd1\xb8\x06\xa2\xcc/\xaf\x90\xbf[\
+.\x97\x0f6\x99\xf8\x8b*0\xe7S\xc8\x8a\x08\x9f_\
+%\x00u\xdc\xcf\xe7\x1e<{rh\xd0\xf4\x1an\x82\
+V\xab\x85P(\xc4\xc1c\xfc5\xd34\xd7/wi\
+\x94\xe6r\x0aE\xf3 \xc4\x02\x10e\x06MS@\x8f\
+\xd8\xa2(b<\x1eCn4\x1a\x88\xc7\xe3P\x14E\
+\xbe\xf9\xbfa\xff0\x91\x1e\x90x\x95\xc4\x1f\x17\x03\x95\
+\xc8\xa1\xc7b1M\x96e\x97,\x1e\x8f\xc7mAR\
+Th\xe7g\x10\x15\xc1mA\xd3TH\xb2\xc8\x99\xaa\
+v:\x9d\x1d\x8a\x9d\x08\xf4\x09\x93\xc6TU\xcd0\xc6\
+\xb6m\x9bF\xc5\x98K2\xae$\xfc\x03^2Y\xc6\
+\xd7t\xde\xa3\x0a>\xd0y\xe7\xaf\x00\x03\x00-\x9f8\
+\xb0\xf8(\xc4\xeb\x00\x00\x00\x00IEND\xaeB`\
+\x82\
+\x00\x00\x02<\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xdeIDATx\xda\xa4\
+S\xcdJ\x1cA\x10\xfezz\xf67\x19\x89\x07\xc5\xdd\
+\x0d\x91M \x8a{Q\xd0\x8b\x0a\xeb\x1er\xf2\xe2Y\
+\x08$o\x10\xf2$y\x82\xe4\x15r\xf1\x94\xc3.\xc8\
+B\x82BBDQ\xf1\xe7\xe4\x88\xffn\xc6\x19\x9d\xe9\
+\x99\xe9t\xb5\x19\xd9]7\xa7m(\xaa\xba\xea\xab\xaf\
+\xab\xba\xbb\x98\x94\x12\xfd,V}\xdf\x84e\x0d\xc04\
+Mp\xce\x91\xcf\xe7\x91\xcb\xe5\x8b\x8a\xf8\xe8\x01\xc4X\
+\xe9\xf6\xd6\xb3=\xcfC\x14E\x08\xc3\x10\x8e\xf3\x07\x8d\
+\xcf\xb30\xbb\x19\x09\xa4\xc4\xced\xb25\xc3`\xf58\
+\x965\xdf\xbf\xb3\xffW\x81\x91\x18q\x1c7\x14\xbbL\
+\xc4\xf3\xdczyD\x82t\xbb\x9fp\xed\x04\xa6*M\
+\x97\xaeV\xf5\xdb\xa7\x97\x88b\xd1u\xc6\xc0\x83\xc5\x8d\
+\x14\xde|8\xa8\x92My\xba\x02\xdf\x0f\x8a\xad\xd6\xb5\
+\xee)\x10w\xf8\xfd\xa3\x89\xd6\xe5yOMq\xc2\x11\
+\x9e\xf2t\x05B\x88#\xb5\xa1~\x11\x09\x81\xe7\xe5W\
+0R\x1c\xe5\x89\x09}B\xa2K\xcaOq\xd7\xf5T\
+\xbbr\x81\xee\x87\xeeWU  DX\x9f\x1c\x7f\xa6\
+t\x80\xfd\xed-\x04A\xf0H\x0e\x94\x9f\xe2\xf7\xb8\xb0\
+Ny\xba\x05)\x0dH\xc9j\xdf\x7f] T\x80\xc2\
+\x8b\xd1\x9e\x04\xe4\xa78\xe1\x08Oy\x9a\x801^\xe2\
+<\xd3\xe0<\xab\x01\x87\xbb;\xf0o\x5c\xecmlt\
+h\xf2S\x9cp\x84\xa7<}\x07\x9c\xa7\xedT\xea\xc9\
+\xfd-C\xe2u\xa5\xa2\xed^\x9a\xe2\xe9\xf4S\xbd\x17\
+\xc2\xd5\x7f\x83\x0d\x8f\xbdS\x8ciX\xc33\xab\xd6\xd0\
+\xf4|\xfb\x03NW,\xaco:\x1d\x8f\xea\x9c\xad7\
+\x9d\xd3\xb5\xf9(\x0ap\xb2\xfd\xa5#\x96URPB\
+\xcfS\x1c\x9d\xfc\xb8<\xf7v_\x92N|\xff$\x97\
+$\xd0\x1c\xb1\xee\xaf9X\x98\xc3\xd4\xe2W5\x0bq\
+\xdb,\x18\xa5\x9f+K\xf6\xd5q\xb3\x03\xab\x09\xfa\x9e\
+\xc6~\x09\xfe\x0a0\x00@\xdf6\xdc\x81!w\x05\x00\
+\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x01\x8d\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01/IDATx\xda\x94\
+S=j\x84@\x14~\xa3ca \x85\x9d\xa6\xc81\
+\xd6b\xed\x02v\xb1\xf3\x02V\xb1\xc9\x11\x12\x92K\x98\
+\x5cA\xc4\xc2\x9c@\xec\x16Oa#\x04\xac\x02\xba\xae\
+\x7fyo\xc0\xb0\xdbl\x1c\xe5\xe3\x1b\x1e~\xdf|o\
+\xc6\xc7|\xdf\x7f\x04\x00\x0b\xe4\x9f:\x8e\xe3/>\xcf\
+\xf3]\x14E\x1f\xc30lVj\x9a\x06a\x18>\xd1\
+\x9a\xa7i\xfa\xa0\xaa\xaa\xf4\xf6\xa4C\xfa\xe4\x8c\xb1\xd3\
+\xfey\x0f\xcb\xb2\x08`\xa2\xab\xdc4\x0d\x18\x86\x01I\
+\x92\x9cD\x024\xe8-\xcb\x12\x1f\x10\xa6i\xba\x8a<\
+\xcf\xc1u] \x1d\x19(\x88\xa3L\xf4\xddn\xb7.\
+\x8f\x7f\x09\x0e\xd1A\xaa\xffo|\xd7\x04\xdcq\x9c*\
+\x08\x02\xe8\xban\xb3\x81\xae\xebP\x96e%Z\x18\xc7\
+Q\xa1\xde\xb0\x002L\xba\xd5\x80Q\x81z\x93a\xd2\
+]$(\x8a\x02d\xf8<\x810\xb0m\x1b\xb60\xfd\
+\xb1\x17\x06}\xdf\xabt\xfft\xbf[\x98\xc4\xc4\xa4#\
+\x03f\x9a\xe6[\x96e/\x9csq\x13t\xc2\xff1\
+\xee\x0e\x9e\xe7\xbd\xd7u\xfd\xca\xb0\x10*\x8ar/;\
+\x0b\x98\xa2j\xdb6\xa2\x93\xbcA\xdc\x22d&jB\
+\xfc\xe0l\xb4\xbf\x02\x0c\x00\xeb\xf2PhUz\x22|\
+\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02\x01\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xa3IDATx\xda\xa4\
+\x93\xbfK\xc3@\x14\xc7\xf3.\x01u\x11Q\xfcQ*\
+\xb8\xa8\xe8\xaa\xad\x1d\x1d\x8aE\xc5\x1f8\xb9\x08\xba\xba\
+:\xa8\xff\x82\x8b\xa3\xe0&\xd4]\xc4A\xacvp\xab\
+\x0d\x0e.:8\x09:\xd6\x9a\xa61Mr?|\xd7\
+4!V\x87@C.\xef\x91{\x9f\xef{w\xef\x0e\
+\x84\x10J'\x8f\x96:\xbc\x9bC+G\x19\xc5\xcaq\
+ \x00\x08\x19\x0d\xa1\xcc\xe3\xd1\xc2\xf6\xec\xc1-\xe0\x8f\
+\x898\x02\xc8\xf4\x07\x8c\x14\xd0g\xf6\x0bd77\x9e\
+ZO'\xa7\xe3\x08\x5c\xea\x1f/\xc8\xe4\xd1\xd5\xa5@\
+\x09\x9d\xc9\xb5tr\xca\xf6\x98\x11G@\xc6\x9e\xdc\xbc\
+\x16\xd1-i\xadM$\x5c\x08\xce\xb8`q\x04d,\
+r\xa4\xb9\x89\x9c\xf3\xe6\xbeP&\xb8\x1c\xd1@\x8fq\
+\xb7\xde\xa0\xa6\xed0\xcb\xa1\x0c_?\xc1p_w\x02\
+9\x88\x0a\x10\x99\x1d\x81f\x80G\x85W\xb5\x9cO\xd3\
+\xa6u,\xb0%*\x94\xa0\xe1.\xe5\xf2\xf1+\x08\x96\
+@\xb9\xe0\x1ef\xb0\x1a\xd4\xaa\x98N\x15\x059\x80B\
+p\x9a\xa0U\xa2\xc7\x05}\xb5}\x09\x842\xce\xbf\xea\
+\xaei\xd8\x9e\x89\xa9\x08R\xe0\xf7<\xe8\xbdoZ\x1f\
+\x12V\x10\x08`f\xc7\xf8vmL\xa4B{\xdf\x83\
+\x03\x14\xfaB\x0b\x05\x18c\xf2d\x11\x87r\x0fC4\
+\xf8\x87\x83?>\xa8R@._*eq\x22q\xf5\
+\xf0V[\xcd\x8c\x0dE`\x88\xd8_\x05a\xac\x81\x89\
+\x13\xe8g5\xd7u\x97\xdf\xcf\xb6\xe6Gw\xce\xef\xf3\
+\xc5\xe7\xa7\x98wh\x04\x99Edz`p\xf3tE\
+\x80\xba$\x9cZ\xa1r\xb1\xa7\xc7\xa1\x076\x8e\xd3\xd0\
+\xd5\x9b\x03\xc1\xae\xa1\xd3\xeb\xfc#\xc0\x00/\xd7\x0a\xde\
+\xec\x13\x8fq\x00\x00\x00\x00IEND\xaeB`\x82\
+\
+\x00\x00\x02\x83\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02%IDATx\xdab\
+\xfc\xff\xff?\x03%\x80E\xbfx;\x03+++\xb2\
+\x98\x19\x14\x9f\x02\x1a~\x0a\x9b&FFF\xb8\x1a\x16\
+\x90\xc0\x9f?\x7f\x18\x98\x98\x98@\x12 \xae\xf9\xd9N\
+\xd7x\xe3\xf2\xdd \x8e*6\x03\x80\x06\x0b\xc1\xd40\
+\xea\x15m\x03\x0bB\x0d\xd0\x022\x1d\x80\x985\xcbC\
+\xd5\xd4\xcfXJ\x0d]3;+\x13\xafc\xc3\xfe\xc9\
+ 5@|\x92\x05IN\x1bh\xb2\xf1\xfeF\xa7\x9c\
+\x1f\xbf\xfe~\xfa\xfd\xf7\xff\xb7\xef\xbf\xfe~@\xd6\xcc\
+\xcf\xcd*\xe3P\xbf\xaf\x1d\xc8<\x0b\xc4WA.\x06\
+\x19`\x05\xc4\x96\xff\xfe\xfd\xfb\xbd\xbf\xd19\xed\xed\xe7\
+_\x0f\x915132\xb2\xb0\xb12qs\xb02\xf1\
+\xd9\xd7\xee\xe9\x02i\x06\xba\xf6*<\x10\x81\x1a\xad/\
+\xf7{\x87\xeb\x16n]\xf9\xf9\xc7\x9f\xf7\xbf\xfe\xfc\xfb\
+\x8b\xe4\xd7\x7f\xbb.>\x7f;w\xcf\x9d\x8b\xa0\xa0\x02\
+\xe23\xc8\x9a\xc1^\x07*:\xaeS\xb0eM\x8a\x8b\
+\x8a\xc1\xe7\xef\x7f>\x00\x0d\xf8\xfd\xf5\xe7\x9fo\x8f\xde\
+|{\xfa\xee\xcb\xafOsv\xdf\xbe\x02\xb2\x00\xa8\x8e\
+\x1d\x88\xaf\xfc\xfd\xfb\x97\xe1\xf7\xef\xdf\x0c\xbf~\xfdb\
+\xf8\xf9\xf3'\x03\x0bP\xf0\x08\x10k\xb9\x1bJI|\
+\xfa\xfe\xfb\xfd\xd7\x1f\x7f\xbe\xbe\xf9\xf4\xeb\xc3\xdf\x7f\xff\
+\xff~\xfb\xc9\xf4;\xc4R^U+o\xd3:\xa0e\
+ \x97\xe9\x01]|\x09\x88\x19@\x18\x94\x86X@&\
+\x82\x5c\xf2\x1b\xe8\xf4\xb7\x9f~}\xfa\xf0\xed\xf7\x17h\
+\xe2b\x06\x06\xe2_]y\xa1_v\xda\xe2\xba\x92\x02\
+\x1cb\x81\x1d\xfb>\x83\x92\x01\x10_\x84{\x01d\x00\
+\xd04\xe6/?\xfe\xfcx\xff\xf5\xd7\xf7\x7f\xff\xff3\
+\x83\xc2\x06\x86\x7f\xfe\xf9\xfb\xef\xf9\x87\x1f\xef\xce=\xf8\
+pc]\x85S\x04P\xad\x0dP\xdc\x00\x9e\xa8\x94\xd2\
+V9\x81\xe2>\xd2^E\xd9Y_\x86\x83P\xd2\x15\
+\xe7g\x17\xf5m\xde\xb9\x1b\x9a\x0e\x0e\xb0\x00\x03\xc2\xeb\
+\xc9\x82\x18\x07\x99\x84%\x07\x16\xec\xba\xfa\x82\xc8, \
+\x01\xd5\xc3\xc5(\x165\xcf\x0b\xe8g\xaf\xff?>\xee\
+~\xb3\xbe\xe841\xbaE\x02\xfbL\x199\xf8]\x81\
+\x09i\x1b#\xa5\xb9\x91\x89\x81B\x00\x10`\x00\xcc\xb0\
+\x1a\x0a\x9c\xeb7\x9d\x00\x00\x00\x00IEND\xaeB\
+`\x82\
+\x00\x00\x03:\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\xdcIDATx\xda\xa4\
+SKh\x13Q\x14\xbd\xf3K\x93\xb1\xbf\xa4\x89\xa9i\
+\xb5B[\xa1\xc5n\x8c\xb4%\x12\xdd\xf8C)B\x15\
+Ap#.\xdc\xb9\x11\xb7E\x0au\xe9B\x5c\xb9U\
+\xbapQD)\xb8\x10Q\xb4.\x94V(\xdah\x9b\
+\xa6\xad\xe9L2\xa9\xf9M\x92\x99\xc9\xfc\x9e\xf7\xa5\x9f\
+\x85n\x04\x1f\x1cx\xef~\xce\xbb\xf7\xbcw\x19B\x08\
+\xfc\xcf\xe2\x87\x1f\xaeno\x04\x01x\x9e\x07\x96\xe3\x22\
+\x0c\xc3\x8c\xa3)\x868\xb2\x13\xb7\x8c\xf8\x88\x97\xcd\xb8\
+\x8e#\xdb\xb6\x0d\xb6e\xc1\xa7\xdb\xbd\xc0\xffA8\xc6\
+sd\xb2\xef\xa0\x18\xec\x0ey\x03\xad\x22/\xd2\xfaT\
+\xcd\x1e\x90rF<\xb9Y\xbbi:0\x81\xa6\x97{\
+\x15\xec\xa5\x122\xe6k\x82\xa9\xb1\xf8\xfe!\xb5\xec\x80\
+c\x12(\x9b\xd6\xaeW<\xd4\xe1\x15\x07\x0f\xef\xeb\x9e\
+\xfd\x90\x9d\xaaX\x8d\xb6\x1b$<\x96\x04Xr\x84c\
+\xdc\xc9\x8b\xb1\xf0\x90\x22kP\xd5m#)W\xa5l\
+\xd1(\xd1\xa0N\xbf\xb7\xbd/\xd2\xdc\xa5Wy\xef\xb9\
+\x91\xd0\xd0\xcc\x9b\xf4$q\xddyt\xc9\xac\x83\xbd\xd8\
+\xa69\xde\xdb\xe5\x0bf\xd2*\x14\x8a5\xe3\xed\x82\xf4\
+MR\xd4\x09\x0c:NA\xf7\xd4\x96G\x9f\x22W\xa0\
+'\xec\x0d\xd2\x1cJ\xce\x9a\xf5: N\x04[\x85@\
+\xa5\xacCb\xbd Y\xa6\xf9\x001\xadU*;\xdd\
+\x91ijK\xac\xe7\xa5j\xd9\x80\x80\xc8\x05hN\x83\
+\xc02\x0c@\xf4s\x0c#\xd6m\x0763\xc5\x12\xb2\
+OW\x8aE\xd0T\x15r\xe94\x98\x18CmR\xb6\
+T\xd2\xa9..\x11iNC\x03Z\x01]\xb5\xba\x0d\
+:jC\xcf\x0e>\x13>\xe7u4\xc7\x11\xb7T$\
+c\xe8m\x1cW\xd3\x5c\xa2:\x18\x8bq\xb5m\x02d\
+\xc7\xb5\xa2\x94\x8c\x01\xdde\xc5@@l\xcf\xca\x85G\
+H2\xba\xfb\x04\x16\x92\x0a\x1e\xcf\x85\x8e\xb0\xdf,\xbb\
+\x9c\xe4\x96\xebu\xcc\xfb\xbc\xdd\x02:\x11sk\xe9_\
+\x85\x22#@\xf8h_/\x9eGO_\x8eE\xa9\xcf\
+\xd04\xaa\xc11\xd4\xe0dKOD\xc7\x98\xd4O)\
+\x9f@\xdf\xbb\x06\x01\xfdQ\xe8\x9cY]ZO\xb2\xcd\
+\x22$u\x16\xa2W\xcfD\xd74v\xb7\x9d\xa87\xe4\
+?\xdbyj\xd8\x97\xf7\xb5\xa5T\x8f7\xa9\xacm.\
+b\xce\xfb\x06A\xf5\xd5=*\x92l\xd6js\x0bO\
+\x9e\xcf\x1f\x08\x890\xaf\xb2P\xe1=T8\x08\x5c\xb9\
+\xd4BFF*\x8a\xcf\x9f,\xf1M\xab\xe9\xd9\xd7_\
+LM{\x86\xff\xa7\xf1Gx[Y\x02\xc6\xb2\xa8`\
+\xe7\xe3woD\xd35\x02\xfe6\x00A`he\x90\
+!\x02a\x94\x8cB66L\x92JU]\xf9k\xc2\
+\xfd\xf1\x22\xe3\xe6\xbe\x03<\xbd\xd6\x10\xb7\x9b\x8d\xdd\xb9\
+\x0f\x1d\xfd\x83\x7f\x8dZ~e\x19r\x8b\x8f\x89\xa7\x95\
+\x83\xaal\xc1VB'z\x89\xaa\xbf\x85(\xa06\x0e\
+%h\xdd\x99\x09\x01\xc1\xfd\xc3\x04\xd3\x01\xd1\x10:\x12\
+\xb8\xbf\x05\x18\x00\xc3\xa8\xbe\x001\x85a\xc2\x00\x00\x00\
+\x00IEND\xaeB`\x82\
+\x00\x00\x02\xb9\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02[IDATx\xda\x8c\
+\x93_HSQ\x1c\xc7\xbfw\xf7\xae\xfd\x81m\xe1P\
+\xd8rkZA\x91\x22\x14H/\x9a\x15D \x91=\
+H\xee!\x99\x88\x83A(\xb6)\xad\x17\xf7\x12\x85A\
+>\x19d\xf8\x94\xf4\xd0\x1e\x82^F\x0f5\x17Q\x0b\
+3\x89\x88(\xdabn\xd3X\xca\x98\xdb\xdc\xddv\xef\
+n\xe7\xceusp\x11\x7f\xf0\xb9\xf7w\xee\xef\x9c\xdf\
+\xef{\xcf\xef\x1c\x8a\x9e\xa0Q5\x0a\x0f\xc8\xb3\x03\xfb\
+\xb3\xcf\x10pS\x1a5\xd9l\xe8\x9f\x9ar\x0a\xfb4\
+\xdaC\xbf&@\x84\xaa\xe5pF\x22\x91G\xd1h\x14\
+\x22###\xf8\xb5\xce\xca\x96n1k\xa0t3A\
+\xe2\x9e\xaf\x0b\xf4y\xbd.\xbeR\x118\x9e\xdf\x13q\
+\x0e=F\x07\x09\x10\x91U04<\x8c\xd8zQ^\
+\xc1!\x0dTc\xcaE\xe2\x9e\xab\x0b\x5c\x1a\x1f\xbfQ\
+\x22\x15\xd8ryO\xc49\xb4\x8b^$@DV\xc1\
+u\x87\x03\xb1\xb5\x92\xac\x82V\xab\x16\x1a\x972D\xdc\
+\x1eq\xcc\xd4\xbe\xcf\x0dOOk\x03\xb3\xb33g\xba\
+\xba\xc0\x0b\x02\x9aM\xca\xba\x85[kO\x90\xdb\x08 \
+M_\x06x\xa9\xb0\x94\xc09?99\xf36\x18\xac\
+*\xb868\x88D\xb2\xfc\x7f\xb5\xc0\x82\xfb\xfd\x06\xad\
+'\xfa\x91\x8a\xbf\x84\x1a\xa0Yn'T;EX\xfe\
+\x90N\xe7o\x8f\x8e^<\xde\xd6\x06\xd2j\xe8t\x0a\
+\x09\x05\xfb\x0aZU\x06\x0dF\x0b\xd8B\x1a\x9f~\xbc\
+\xcf\xa5\xf2xx\x80\xe8P\xfcS\xf0\xd4\xe7\xbb\x1f\x0e\
+\x85\xe0_X@\x85$X\x8d\x97wXe\xb1\x1e}\
+\x01\x9d\xc1\x02\xbb\xe3\x19t\xfa&\xf4\x98`\x0c\xf4\x0a\
+\x0cAJ0\xd7\xe7\xf1x;\xbb\xbbq\xd5nG\xa5\
+R\x81\xd9\xac\xa8bP\xbf\x83A\xaf\x00\xc5\xa7\xe0\xf7\
+\xfb\xb1\x9d\x89\xe2h\xa3U\xcb\xf18[\xe6 \xdf\x85\
++\x03\x03H&x\xf1\xe7\xb1\x1d\x9f\x80\xe5\xb0\x1a\x05\
+\xee'\xa2\xb1\x0eX\x9a\x97\x90\xcd\x16\xb9B,<O\
+\xea\xb8\xa4\xdd\xd4\xb5\xb7\xdfM\xae\xac\xdc\xe28N\xda\
+\xbb\xec\x9f06\x22\xf7`4\x95\xc0s\x19\x1c9\xb9\
+\x8c\xc8\xd7\xd3\xd5\x9b\x97\xf8\xf6=\x9c\xdf\xca\xb9\xc5.\
+4\x10\xcc\xd9\xe2\x17\xab\xbe\x93\xf9\xb8\xbbu\xee\x0b\x94\
+\xcd\xde\xdbrP\xa3P1P\x0a\xc8oz\x91\xdb|\
+^\x8d5\x9a\x0c\xc7\xd6\x92\xb9\xaa\x02\x8d(`WK\
+%{|\x07>\xf2:%w\xa0(\x0a\x02\xc3`\xe9\
+\xaf\x00\x03\x00fMf\x08\xea\x03\x80=\x00\x00\x00\x00\
+IEND\xaeB`\x82\
+\x00\x00\x02\xf5\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\x97IDATx\xda\x84\
+\x93_HSq\x14\xc7\xbf\xf7\xeen\xc3\xd4\x9c\xe6\x98\
+\x95\x93r\xd7?\x9b=(HZ\xe8\x10\xb5l\x89o\
+\xedA\xd0\x17\x1f$\x84$\x14+\xb0|\x10\xac\x95\xb4\
+\x82\xc2\xc2\x07_|\xf0a\xf4\x07\xa4\x7fJ\x90X\x0f\
+\x8a\x1a\x08Z\xd9\x1fr\x19\xb2\xcdh\x96%s\xf7\xee\
+v~\x97\xb5&\x0e:p8\xdc\xef9\x9fs\xce\xef\
+\xf7\xe3r\x883>)\x09\xba\x9c\x1cly\xbd\x88l\
+n\xa2\xa0\xa2\x026\xbb\x1d\xbcF\x03\x9e\xe7E*\xa9\
+\xc6v[\x15\x90\xc0,\xa5\xa5((+S\xc1\xa8\xe5\
+E\x22\x91jOo\xef\xdd\xbf\x02G~\xaa\xa7\xe7\xf4\
+\xb6\x06\x07\x8a\x8bUX#l\x93\xf3\x22\xb2\x5c\xe3\xe9\
+\xeb\xbb393\x83\xd7\x0b\x0b()*B%\xd5\x91\
+\xce\xa9\x95\xe6\x92\x12\x1c$A\x10v,\x94'\xcbr\
+\xed=\x97k\x80\x22\x02\xeb\xebH\xcf\xc8\xe0(*,\
+)\xb3\x06eMM\xd0h\xb5\x89N\x92O\x13\x8e\xdd\
+\xef\xef\xbf\x1d\x0a\x85\xa0\xa1\xe3X-\x16\xac\xf8\xfd\x8a\
+\xd9dR\x0b(\xcf'\xbc\x03\x06K\xb2|\xfc\xa1\xdb\
+}\xebWp\x0e\xca\xb7+\xd0\x1a\xbb\x91\x9b}\x08\xa2\
+\xd9\xac6;\xd9\xd1q\x86\xeea\x9cO\x00\x17\xc8\x92\
+T\xf7\x80\xe0\x8d\xb5i(+=\x00\xbdH\xd8{\x91\
+\xad\xac^\xac\xa3\xbd\xbd\x9d\xa6\x8f\xd39\x96\x84\x04\xf0\
+\x89\xd1\x81\x81\x9b?W_AX\xee\x8e%8\xf1\x1a\
+tz=\xea\xda\xda\xcer\x1c7F\x8d\xde1=\xbe\
+A\xa1$I\x8e\xc7\x83\x83\xee\x1f_&\xa0\xffp.\
+\x96\x88Xo %\xf30j[[;\x08~\xa6\x89\
+\xc2\xf1\x0d\xac\x0c~:4t=\xe8}\x81]\xef\xbb\
+b\xb0T\xe8Fj\xd6QT\xb7\xb4t\x12\xfc\x84\xe0\
+\xb7\xf1+\xb3\x06V9\x1c\xae\x1f\x1b\x1e\xeegp\x0a\
+[[\xa7S\x93\xa1\x5c\x17v\xef\xafDUss\x17\
+\x18,\x081\xf8\xd3\xf44>NMA\xa0\xc9\x0d\xcf\
+GF\xae\xfa\xfc~d\xae]\x06\x92\x93\xd5\x82\xdf\xa6\
+K0\x10lol<O\x93\x1f\xd1\xe47L_\x9e\
+\x9b\xc3\xf2\xec\xec\xbf\xbb)v:m\x8a\xa24Lx\
+<\xae\xef_'\x91\xb6\xe1\xc6Fj'\x0c\xfb*P\
+\xe9t^ x\x94\xe0E\xdf\xe2\x22V\xe6\xe7w\xbe\
+Y\x96\xcd\x86\xc2\xfa\xfa\xa2|\x87\xa3;H\x9d\x96|\
+>e\x9d\x22\xfbf:\xcb\xff\xcf\xd8\x1f\x93\x96&\x8a\
+5\xa6\xf2\xf2^\xd6\x84E\x83(V\x91\xbe\x87<\x9d\
+\xe5\xc9S\xc8\x93\xc8\xf5\xe4\xda(\xc7q\xd1\x8f\xbd\xe4\
+\x99:\xa31[k4\x1e\x09\x07\x02/\xb7\x02\x81\xcf\
+\xa4\x85\xd9CD#\xf3\xad8\x8d\xb9\xfcG\x80\x01\x00\
+\x06\xd4\xffg\xbc\x0c\x93)\x00\x00\x00\x00IEND\
+\xaeB`\x82\
+\x00\x00\x03\x22\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\xc4IDATx\xda\xa4\
+SKk\x13Q\x14>w\x1eI\x93\xd04MkL\
+\x1bju\xfaP[*HpUkQ\xc4\x85\xd2\xaa\
+E\x04K\x7f\x82\xb8p+\xb8(\x88[]\xba\xf0\xb1\
+(\xe8B\x84\xb6P\xa4\xb8\x91*\x8a\x98\x0a\x16m5\
+\xb4\x0d\xad\xa6v:I\xf3\x9a\xc9\xbc\xee\x8c\xe7&}\
+\x09\x82\x0b\x07\xbe\x99;\xe7|\xdfw\xce}\x11\xd7u\
+\xe1\x7f\x1e\x81\xbdN?\x96\x1f\xe0'\xfe\x97|\x02q\
+\x17!\x22JX,\xe3Pj\xda\xb6\x0d\xb6e\xc1\x87\
+\x1bmU\x03J\xe9\x0c\xb8n|\xe4Bs\xbc\xacU\
+;\x12E\x02\xcf\xa6\xd3p\xe5LS\xab\x927\xf7\xa5\
+\x15\xc3L\xa5\xb5\x92Ia\x1e\xd3k\xdb\x158\xf6B\
+\xb71t}\xf9d|%\xc1\xf3.\x14\xf2\x16\x18\x06\
+\x05V)\x9f\xb3\x88\xe8\x92\xfdR\xc4\xd7z\xa9?\xd2\
+\xed\x15\xddsXL\xfa\xc3\xc02\x8cf\xa0V\xef\xe5\
+S\xd1\xf8\xda\x0f\x15B\xf5\x02\x9aR\xb0L\x13&\xde\
+\xac\x14\xdf\xcd\xad\xd7\xca\x1b\xa5\xf6\xf5\xb4\xd66p2\
+z\x9c#\xf4\xaa\xeb8\xa1\xdd\x0eLs\xa8\xf3@\xa0\
+=+\xabP\x1b\x14\xe0\xd1\xf3\xf9D]\xbd\x07l\xc3\
+\x00\x9cs\xe2\xd7Fq\xfa\xf5\xa7tYQJ\xd2\xda\
+j\xa1]j\xf2\x1dCM\xdf\xce\x22\x9a\x86\xd1\xdb\x18\
+\x14\xc3\xbaf\xc2\xe7Df\x11\xff\xdf\xdf\x7f8[\xed\
+\x11M<^\xef,v\x13\x9dOe\xe2]-\xa1X\
+$\x5cc \xa7\x1f\xb3\x93\xd5)\xe8z\x07O\x88\xbf\
+\x88\x06\xc9E9Gm\xfb:V\xbf\x87H`%\xd0\
+U\x95u9\x95\x96\xf3\x1eU\xb7b\xc8\x95Psb\
+o\x07\xa0\x1a6\xe4\xcave\xech\x1a\x08\xa28\xc6\
+\xc0\x0c\x0c\xbd\x0c</\x00\xc7\xf3\x01\x95\xbaA\xc6E\
+^`g\x0dL]O\xae\xe7tM\xe5\x04\xa8\x0b\xf9\
+B(\x1a.nn\xc2\xa6\xa2@V\x96\xc1,\xeb\xac\
+\x83a\x96c\x1c\xc6e\x9a\xbd\xbb\xf0vyU\xc9\x16\
+\x05\x0f\xb4\x1cm\x8d\xe1|o\xe2\xa1\x19\xc6xe\x19\
+*c\x8c\xb1\x1c\xe30.\xd3\xec\x1a\x98\xe6\x8b\xe5\x85\
+\x94B\x03>H\x81\xbf&>\xd8\xdb\xdd|02\x8a\
+[\xf5\x91\x81\x8dY\x8c\xe5\x18\x87q\x99\x86i\x09\xbb\
+\x0b\xc1\x91\xa7l\xbb\x06\xf8\x80\xffN\xc3\xc5\xf3=e\
+\x1bc^\x02!o\xc5\x1fr\x86\x03\x05\xc3\x05\x9f@\
+ 3>5GU\xed\x16\xae\xc7da\xecZ\xd5\x80\
+\x10\x02\x5c\xe4\x08p\x87\x07\x07\xb8X\xcf\xa8\xd8\xd9\xd1\
+H\xa4Ca'\xdc\xe0\xaf\xb4\x99\xcdh\xee\xd2r\xd6\
+\xfa\x9eT\x9c\x9fs\xb7\x9do\x13\x93\x8e\xbc\x00\x15\xed\
+\x96\x01\xdb\x8d\x06D#\x89tE\x89t\xb6\x0f\xc2\x1d\
+\xdd\xc0\x8b\xd5#K\xad%\xc8&\xbf\xb8K\xaff\x5c\
+\xf9\xab\x8c\x91\x0d\x84\x82Z{\xdb\x80\xf5\xea\xdf\x82\xf0\
+\x8f\x1bL\x11*BC\xad\xf3[\x80\x01\x00\xc4F\xad\
+\xe2\xe9g\xd4[\x00\x00\x00\x00IEND\xaeB`\
+\x82\
+\x00\x00\x02F\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xe8IDATx\xda\xa4\
+\x93\xbfO\x14A\x14\xc7\xbf\xb3\x8cw\xb9C.\xa2\x85\
+\xc9\xa1$\xc6\xd0\x98\xf8#jb\xa8\x88Z\x5ce\xed\
+_@,L\xe4/0\x16\xd6\x14\x16$K\xa56j\
+\xa7\xa5vXY\x08\x06N\x0a.\x86\x10sp\x07\x01\
+\xf6v\xf5\x8e\xbdefv\x9d\xf7vo\xa3v\xc0$\
+\xdf}3o\xe6\xf3\x9d\x99\x97Y\x91$\x09N\xd2\xe4\
+\xddW\xbb\xf7m\x9c\xb1\xaa\x1e\x91mY\xbd\x90\xb11\
+3w\xae\x9c\x9b:{ZVb\x9d \xd6\x06Z\xc5\
+\xd0:Fd\xd57\x09\xba\x02\xf0\x87\x04<9\x04\xaf\
+\xe0`\xff\x94\x03\x84fbb\xad\x032\xa8\x06{\xdd\
+\x8a\xbfk\xe18f\x19c\xf28\x90\xfd\xe0\x8c\xcd\x8d\
+\xd8x1]WYn\xfe\xaaJY(`\xfe\xc1\xe8\
+\xb1\xeeo\xaf\x0f\xc7h\x9d\xef\xfce\xcd\xc0\xfd\xa8\xb1\
+\xf8C\x83\x8a\xab\x9as\xe8}\xbd\x8d\xfe\xd6\x1c\x03\xee\
+\xba\xcb\xf9\xfc\x84\x96e\x03J\xd0\xc4\x87\x85\x1d\x5c\x1f\
+\x8b\xd0\xa87!\x84@\xd8x\x0dq~\x1a\xed\xcdw\
+l\xd0\xeb\xf7\x18\xd4\x19\xc3\x06Z\xa9\xdc\xb1\xfe}\x13\
+\x93W\x87!w\x1a\x0cD-\x1f\xe5\xf1G\xf8y\x10\
+\xf2\xd8?\xf0\xff1 \x96\x0d(\x11E\x11\xde\xcf^\
+\xe3~i{53H\xc1\x8d4\xa0\xd3\xed\xb0\x81\xca\
+\x18b\xa5><d7JR+\x97\xcb\xd6\xa0\x9e\x1a\
+l\xa5\xe4zf\xe0u\xbdtg\x0b\xd3\x15\x89\x95\xca\
+\xee\xfc\xb7\x01\xf5\x87\x83\x0d\xb4\xdf\xccBy\x0e\xd7\xa6\
+\xadJx[\x7f\x890\x0a\xf3\xb5\x8e\xe3\x80XGe\
+'\xe0#Y\x85a\x88\x0b\xf7jh\xb9\xcfP\x99\x9a\
+F\x10\x04\x98\xbc\xfc\x10\xee\xd2<j\x97j<?\xa8\
+\x01\xb1b\xec\xc9\xa7\xc5\xe5\xa77oQr\xd0\x8a\xc5\
+\x22\x8b\xeaB\xfa\x7f\xcc\xff\x80\x94\xb8\xf1\xfc\xdb\x92\xdc\
+_\xfd\xbc2\xfex\xfbX\x0f)\xd9k\xac\xd8W\x8e\
+\x92\xd5\x08\x99\x1e\x91\xa7#\xff\x16'\xfd\x9d\xff\x080\
+\x00\xdb\xf2j\x84\x0b\xe2\xe5X\x00\x00\x00\x00IEN\
+D\xaeB`\x82\
+\x00\x00\x02\xb5\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02WIDATx\xda|\
+R\xdfKSa\x18~\xce\xb73i\xc1\x0a\x1a\x15\x8e\
+n\xce,\x12\x8b~h\x91\x91I.H\xba\x10\xba\xa8\
+\x8b\xfe\x83\xfe\x81\xa2.r%]\x86\x82\x04yW\x08\
+\xbb\x0b\x14D\xf3\x07\x05\xc6L)/\xa6\xd5H\xd4\x86\
+82fN\xa6[;\xe9\xd9\xf7\xf5\xbeg;\xf3`\
+\xe0\x0b\xcf\xbe\xb3\xf3\xbd\xcf\xf3=\xef\xf3\x1d\xedv{\
+;\xb84Mk\xa3\xa5\x1a{\xd7{)\xe5\x82,\x16\
+\xa1\x94\xc2\xf7X\x0c:?p\xd1\x1a\xec\x8dDz\xb6\
+hs\x9b!%\x8a\xb4\xe7\xec\xc7\xe3q\xf4\x8e\x8d\xdd\
+\xe3\xb3\x08\xf3\xfc\xae\xb6\xa9\x09\x82\xd5\xca\xd0$\x93\xb6\
+\xb7ml\x99&\x0a\xf9<r\xb9\x1c677\xed\xf5\
+MGG\x0f\xf5]'\xee\x09\xc7\x92^$r\xb94\
+\x96\x16\xf4\xeb\xf5xvL[\x16,\x12\xced2x\
+\x11\x8d\x22\x5cW\xf7\xb2;\x1a}L;\xcfl\x01\xb9\
+# \x98,l\x19\xfc'\x12\x0e\x87\xedq\xfc~?\
+F\xe2\xf1\xf5\x0a\xc9\x22\x812(\xc7\x92\x80\x03\x16\xd9\
+\xe7\xf5\xa2J\xd7\xa1\x0b\xc1A\x97\xf4\xa8\x979W'\
+&h\x04R\xdf=\x82\xbbv;a\x11\xe2h\xf7\xfb\
+\xfbq0\x95\x82`\x812J#\xd0Ib\x0f'\x1e\
+\xfa\x7f*\x99\x0c\x1dO\xa5\xfah\xf8k\xc2\xe2\x90J\
+\x10\x8e\x83\xbdD\xd6\xd3i\xe4M\xf3\xa4\x11\x89\xdcZ\
+\x05\x9e\xea\x96{\x04j\xb4s(E\x0aP\xfa\xee2\
+3SH\xcc\xfcA\xf7\xc0\xc0\xcd\xd6\x9a\x9a\xae\xbbJ\
+\x0d\x0b\xe7\xde\x09\x15\x07\x950]Nr\xbf?b\xf9\
+k\x17\xda.}B}s\xf3\xc8\xb4i\xbe\xa6\x11F\
+\xdd\x0e\x84\xed\x80\xae\x8a\x09|\xb6\xe3$\xfb\xeb\x03\x96\
+\xbet\xe2b\xc3y\x0c\x0eO!T[\xb5dJc\
+\xf6s0\x08\x91]Yq2\xa8\xdc\x82\xdb\xc9F:\
+\x86\xe4l'.\xd4\x9f\xc3\xe0\xdbI\x9c\xb9\xf2\x08\xa9\
+B\xf5\x8f\x03\x86\x81w\x81\x00\xc4\xc2\xf882t\x1d\
+\xf4\xd9\xea\xe5 *\x22\xf9\xb5y,\xce<GC\xfd\
+Y\x0c\x11\xf9\xf4\xe5\x078\x16j\xb1{\x99\xc3\x5c.\
+\x1f\xe1\xc8\xd1\xc6\xc6\x0e\xe5*I\x98\x1cz\xa2Tn\
+N\xf5\xbdjQ\x8bsc\xca\xb4,\xf5WJ\xc5\xbd\
+\xcca.\x1ft\x88\x10\xf4\x19\xc6\x0d\xe1\xf3\x1dv\xa7\
+\x9eO$\x1e\xdei\xdd?\xf7-\x1b\x98^\xda\xf0/\
+;\xefe\xa1\xb0ZH&G\xe9\xf1\xe7?\x01\x06\x00\
+\xa6\xe8M\xd6m\xca\x89\x98\x00\x00\x00\x00IEND\
+\xaeB`\x82\
+\x00\x00\x023\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xd5IDATx\xda\x9c\
+\x93\xcbN\xdbP\x10\x86\x7f\x1b\x07\xc7\xa1E\xed\x12P\
+@N\x94\x8b\x12TQ\xaa\xaaR\xb7\xa1\xec\xba+\xef\
+@\xf7\xac\x13)O\xd1\x15O\xc0\x1b\xb0\xab*\x10 \
+\xee\x09\x8a\x88\x92\x88\xa6QV\xa8\x8bV!\x01\x1f\xbb\
+3\x93\xd8\xb9\xacJ\x8e4\xf2?\xb6\xff\x99o\x8e\x8f\
+\xb5\xadB\xe13\x80\x05L\xb7\xda\x86\xeb\xba\x8b{\xc5\
+\xe2\xb7i\xdc_\xf2\xf9m\xc3UJ\xf3(\xd9<\x05\
+<\xcf\x0b\x82\x0aKx|\x1d\xcd\x07\xcf\x8fs\xaf\xc0\
+^])\xa5\xf3\x0b\xbc>\xc55\xb9n\xc4\x86:G\
+:g{\xc1}_\xb3\x87\xbd\x86r\x1cMI\x01\x0d\
+\xfb5\x0f1\xa3K\x93u\xa4\xf3\x86E\x1d\xdb.4\
+z\xce\xda\x0d4\x99\xbdy\xb0\xd7p\x1cg\x8c\xc0\xfd\
+\xf5\x80\x9d\xcck\xc9Ono\xf1>\x99\x14}P.\
+\xe3c6+\xfa\xfb\xe5%\x11,\x83\xbd#\x04\x10\x82\
+\x9c\x09\x9c\xd7\xeb2\xef\x5c8\x8c\xa3JEf~a\
+Y\xf8q}-\x9a\x17{\x02\x02E/\x0f\x09\x80\xd5\
+\x95\x15\xc9/j5\xac'\x12}\x1a*\xf4!\x93\x11\
+}X*\x81=B \x05&\x08JwwB`\x99\
+&\xce\xaaU\xe9\x1aa\x9a\x9b\x9b1\x82~\x81\xa7\xa7\
+`\x04\x9f \x1d\x8dJ^j4\xf0&\x1e\x17}N\
+\xfb\xf1.\x9d\xee\xd3P!)@\xde\xb1M\xf4\x09*\
+\xcd\xa6\x10\x98\xb3\xb3\xb8\xa21\xb8k\x98hN\x07\xfb\
+\xe1\x7fF\xf6\xeaTEW\x13\xe7 \xb1\xb4\x84\x14Q\
+\xf4\x1e\x1f\x91\xb5m\xac\xc6b\xe8\xf6zX\xa3/\xf2\
+6\x95\x1a\x8e@^\xa3\xd7\xed\xceL\x12T[-!\
+\xe0U\xa61\xfc\xae\x174\xc6(\x01{\x8d\xdf\xf7\xf7\
+f(\x14\xc2n\xea\xef\xe0\x84\x9b\xff\xf5o\xb1\x87\xbd\
+\x9ae\xdb_\xf5Hdy\x9a\x9f\xc9\xedt~\xf2\xd0\
+\x16\xc5K\x0a\xe3\x99~\x87\xe2\xcf?\x01\x06\x00@(\
+K\xf8\xa2\x22\x9e\x10\x00\x00\x00\x00IEND\xaeB\
+`\x82\
+\x00\x00\x02\x86\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02(IDATx\xda|\
+RMh\x13A\x14~;\x9d6\xcd\x0fX\xb4\x98\xd6\
+\xb4\x87P\x11D<\x94\x15<\x16Tl\xb4\x8a\x14<\
+h\xefR\xd0\x93\xf7\x1e\x0a\xee\xb9\x9e\xf4\xa2'\xbdx\
+\xae\x15\x8bzP\x14\x0fj,UZ)\xa5J!\x7f\
+\x0b\x8d&1\xfb\x93\x9d\xc9\xae\xef-n\xba\xa9[\x1f\
+\x0c\xf3\xbe\xef\xcd\xfb\xde\xbc7\xa3x\x9e\x07d\xc3\xe7\
+o\xc1\xc8\xd4m\xe8\xed\xeb\x03\xce9\xf4p\x9eCZ\
+\xc35\xd7\x96rYJ\x09\xc2q\xa0\xf0\xec.\x94_\
+\xdc\x83\xc0X\xe0\x0c\x9d\xbb\x09!\xcba\x92v}\xf2\
+\xb0J;\xe1}\xce\xed\x0at\xcc\xf3rXM\x9b\xb9\
+pD-\x14\x04\x5c\x9b\x1cV\x09\x13\x0f\x11\xc6\xf6&\
+\x0b!0yT\xdd\xdc4\xc00\x1c\xd8\xda2\xe1\xea\
+\xd9\x8cJ|\x94\x08\xdb\xcd\xc5\xca\x8e\xa3\xcd\x5c\xcc\xaa\
+\xe5\xb2\x85\xd8\x05\xd3\x14\xe0\xba.\xe8\xba\x0dW&F\
+U\x8a{{Dx\xe0H!\xa6i\xa0\x0f\x9f\xac\xe6\
+\x09OM\x1cS]\xd7\x03\xc6\x14Xz\xbd\x91\x0f\xce\
+)\x8a2\x8d\xdb\xf2?\x02\x98<K\xd5<\x5c\xae\x94\
+\x9fl\xdb\x81z\xbd\x81m\xb8 l\x1b\x18\xe7\xa7\x14\
+\xc6P\xb0\xbbk\x1e\x06m!\xc06\x0d\xdf/\x95*\
+(`A\x22\x11\x03\xdb2}\xae?\x91\x04\x16\x8bE\
+\x0b4\xaaUh\xd6j\x9d\x80\x84\x0c\xf0x\x0c\xda\xd8\
+\xc2\xef\x9f\xbf|\x8e\xf6\xd4\xc0@\xb4\xc0N\xb1\x18z\
+\x0c/\xff|\xf1}\x07\xe3\xd5\xf3\xd8\xbb\xef\xdb\x86\x11\
+-\x10O\xa5\xc2\xfcl\xf0C\xff\x0e\xae\xe3;\xc5/\
+\xd1\x02\xfd\xc9d\xb8b\x06\x93\xe6\xd1\x1d\xc7\xb5\x82b\
+\xf38\x5c\xff\x8a\xb2\xfe\xbdK@\x09*Q\x95\x03\x97\
+4\xe8\x1d:A\xf0\xc1\xe93'/\xf3\xa3\xd9ts\
+\xe3\x87\xbe\xfa\xe6\xebS\xe4n\x88\xca\x1a\xd4\x97\xe6 \
+|\xbb\xae7\xa1\xa0\xb5\xfd\x19Z\x965\xde\xc8\x8e\xa5\
+\x17+\x0cJ#ci\xc2\xc4S\xfc\x7f_\x99\xfc\xb8\
+\xf1\xf2\xce!\xd1\xac\xad\x15?\xae\xeb\x83\xf8b;+\
+\xeb:a\xe4\x071N}\xf6\xec\xf7\x0fhRq\x5c\
+\x07[o\x17\x1em\xb7l\x06\xaf\xde\x1d\x07\xc7\xf8\xe6\
+~\xb8\xff\x18y\x12\xa8\xd2\x1c\xe9\xcb\x04I\x7f\x04\x18\
+\x00*-\x12\x92\xf2.p\xe1\x00\x00\x00\x00IEN\
+D\xaeB`\x82\
+\x00\x00\x02$\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xc6IDATx\xda\xa4\
+S\xbbN\x02A\x14\xbd\xfb\x80\x04\x88,\xcaK\x13\x02\
+H\x01\xb4\x84\x92\xd2B\x1bbO\xecL\xa8-\xec\xf8\
+\x05\xfd\x01\x0a\xfd\x03\x1aH4D\x8d\x09\x856\x1b\xb4\
+\xa0\xb1 \x94\x84\x87nx\x84\x00\x01<\x97\xc0\x06\xd8\
+\xed\x98\xe4\xe4\xce\x9d=s\xee\xb9;3\xc2b\xb1\xa0\
+}\x86H{\x0e9\x97\xcb\x1d\x8a\xa2x\x86\xb9\x1b\xe8\
+\xce\xe7\xf3\xd7\xd9l\xf6W\xaf\xd7uR$\x12!I\
+\x92LyR<\x1e\xbf\xccd2\xd7\xc0\x8d\xd3\xe9T\
+*\x95J\xbf\xdb\xed\xd6\xf0Q\x17\x18\x0e\x874\x9dN\
+\x0d\xbc\xd1hT\x93\x1b\x8d\xc61D\xce\x99\xc4\x11\xf9\
+\x93\xa2(\xd9M\x9b\xe3\xf1\x98Z\xad\x96m\x97\xc7\xdf\
+\xe0L\x8ay<\x1e%\x10\x08\x9c\x96J\xa5\xb7b\xb1\
+\xf8i\xb3\xd9\x1edYV'\x93I\x12\x9c|\xbf\xdf\
+W\xb1\xc1\xc0\xd34\xed[\x80\x1d\x0f\xec\xa6A\xf4\x01\
+-\x08\x16\xd1k'\x91Hp\x01v\x92\xafV\xab\x84\
+\x9eMy2\x16;\xe8\xefq\xd3\xb2\xd7\xeb\xa5\xc1`\
+\xa0\xe7n\xb7\x9b\x9a\xcd\xa6\x81\x07\x01\x92\xcd\x8e\xc6b\
+\xb1\x10l\xeb9\xacS4\x1a]nX\x0f8\x22\xfe\
+\xd1\x06\x01\xab\xd5J\xbd^ok-\x18\x0c\x12.\xdc\
+\x116]\xb0\x1e\xd0A\xfe\x8c\xf8K\x0e\x87\x83\xff\xe4\
+Vu\x9c\xc2\x1aY\xbb\xddN>\x9f\x8fR\xa9\xd4U\
+\xb9\x5c~A\xd5\x05G\xce\x01\x12L\xaf'\xf7&/\
+\xcd\xa5Q\xe9\x84'\xe1p\xf8@U\xd5\xbb5'\x99\
+L\xde\x22\xdcKf\x02\xfc>\xb8?X\xfe\xc1\x5c]\
+!\xe6\xf7\xfb]\xa1P(\x5c(\x14\xdeq\x8c\x1f\xed\
+v\xfbk\xd3\x01\xcfY\x90K[\xb9\x9bU\x5c\x02\xae\
+\x5c\x00\xdf\x0b\x17\xa0A\x5c\x05\xea\xbb\x02\xc2\xea\x81I\
+&\x107\xc0\xbc)\xdfra\xdf\xe7\xfc/\xc0\x00g\
+y\xed\x91\x1b\x1bx)\x00\x00\x00\x00IEND\xae\
+B`\x82\
+\x00\x00\x05\xa3\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x03iiTXtXML\
+:com.adobe.xmp\x00\x00\
+\x00\x00\x00<?xpacket beg\
+in=\x22\xef\xbb\xbf\x22 id=\x22W5M\
+0MpCehiHzreSzNTc\
+zkc9d\x22?> <x:xmpm\
+eta xmlns:x=\x22ado\
+be:ns:meta/\x22 x:x\
+mptk=\x22Adobe XMP \
+Core 5.0-c060 61\
+.134777, 2010/02\
+/12-17:32:00    \
+    \x22> <rdf:RDF \
+xmlns:rdf=\x22http:\
+//www.w3.org/199\
+9/02/22-rdf-synt\
+ax-ns#\x22> <rdf:De\
+scription rdf:ab\
+out=\x22\x22 xmlns:xmp\
+Rights=\x22http://n\
+s.adobe.com/xap/\
+1.0/rights/\x22 xml\
+ns:xmpMM=\x22http:/\
+/ns.adobe.com/xa\
+p/1.0/mm/\x22 xmlns\
+:stRef=\x22http://n\
+s.adobe.com/xap/\
+1.0/sType/Resour\
+ceRef#\x22 xmlns:xm\
+p=\x22http://ns.ado\
+be.com/xap/1.0/\x22\
+ xmpRights:Marke\
+d=\x22False\x22 xmpMM:\
+DocumentID=\x22xmp.\
+did:190B26F4E356\
+11E0816FDD6C3AA8\
+02FC\x22 xmpMM:Inst\
+anceID=\x22xmp.iid:\
+190B26F3E35611E0\
+816FDD6C3AA802FC\
+\x22 xmp:CreatorToo\
+l=\x22Adobe Photosh\
+op CS3 Windows\x22>\
+ <xmpMM:DerivedF\
+rom stRef:instan\
+ceID=\x22uuid:AC1F2\
+E83324ADF11AAB8C\
+5390D85B5B3\x22 stR\
+ef:documentID=\x22u\
+uid:C9D349664A3C\
+DD11B08ABBBCFF17\
+2156\x22/> </rdf:De\
+scription> </rdf\
+:RDF> </x:xmpmet\
+a> <?xpacket end\
+=\x22r\x22?>\xf9m\x9e\xa2\x00\x00\x01\xd0ID\
+ATx\xda\xa4SKK\x02Q\x14\xbew\xb4f\x14\
+\x1bS1+w\x11\x12!i\xb4\x087\x82\xe0J\xe8\
+\xbfH\x10\xb4\x12\x5c\x07\xe1op\xed\xca@\x10\x17\xfd\
+\x82\x10\xc3E\x8bh\x17\xf8 \xdf\xe9\xcc\xa83}g\
+\x9a1w\x0a]\xf88g\xee\x9c\xf7\xfd\x0e7\x0c\x83\
+\xfd\xe7\xf0\x5c.\xc78\xe77\xd0\x15\x04\xfb\x80\x1c\x01\
+S@\x05\x96\x80\x03\x10\x017 \xc3\xf6\x04R\x82\xed\
+S>\x9fg\xce\xe5\x92l\xd8q6\x9b\xbdm6\x9b\
+\xf5n\xb7\xfb\xd9\xef\xf7\xbfz\xbd\xded:\x9djn\
+\xb7{\xd7\xef\xf7{|>_ \x18\x0c\x86\xa3\xd1\xe8\
+e\xa1Px\xb4+p.\x16\x0bS\x09\x04\x02\x91d\
+2\x19\xd9X2\xe7\xcc\xf61\x03\xcc\xe7s\xf3^\xd7\
+u\xb6\xcd<(\x00|\xf8*\xc0l6\x13\x1d\x0e\x87\
+\x19\x80\xb0\xe9\x08\x82\xc04M\xe3h\x9d\xe6\xa2\x0a(\
+'\x9eJ\xa5\xae\xa9\xacma\xd9\xc7\xcd\x80\xaa\xaa\x9e\
+&\x12\x894\xb5B\x03\xdd\x04\xb2#{\xf23[\x80\
+\x22c\xd2\x07\xeb\x83\xd9t\xc8\x9e\xfc\xcc\x00\x8a\xa2L\
+\x06\x83A\x07\x97\xe1m\x03\x8c\xc7\xe3\x0e\xf9\xd9-\xbc\
+W\xab\xd5g\xe8\xfa6\xfd\x93\x1d\xd9\x93\x9f\xcd\x83z\
+\xb1X,\x834<\x93\xc9\xa4@\x98C<\x95\x80\x0c\
+\xab\x8c\x92$\xd1\x13\xeb X\xabR\xa9<\x97J\xa5\
+\xb2\xcb\xe5\xaa\x9b\xcf\x9aN\xa7Y\xbb\xdd\x96F\xa3\xd1\
+\x15\xbe\xcf\x80}\xbao4\x1a\x0f\xc3\xe1\x90y\xbd^\
+\x16\x8b\xc5\xeepG$\x19\x00o\xb2,\xbf\x84B!\
+\xa5V\xab\xfd\xf5\xe5\xf1xV\x10E\xf1\x1cY\xef\x91\
+\xd1 I\xdf\xeb\xff\xedC\xc4\xb3\x19%\xd8\xcb\x02\xec\
+\x91\x0e\xc2\x1cA^\x00\xaf X\xcbZ\xb0\xb1\xb5l\
+\xdf4\x8b\xf5\x00$w\xac\xad\x13-\x9d\xaf\x0d\x9e\xca\
+'\xcek\xd6\x96j\xbf\x05\x18\xecG\x80\x01\x00\xe0C\
+5'\xb9\x19\x9d\xea\x00\x00\x00\x00IEND\xaeB\
+`\x82\
+\x00\x00\x01\xbe\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01`IDATx\xdab\
+\xfc\xff\xff?\x03%\x80\x89\x81B0\x0c\x0c`Y\xc1\
+\xc8\xa8\xc8\xc8\xc0\xd0\x0ad\xab\x01\xf1-`\x90V\x03\
+\xf1\xfd\xcf@\x0e'T\xd1\xe6\xd0P\x06%%%\x06\
+fffA&&&g\xa0\x900\x10\xbf\xfd\xf7\xef\
+\xdf^f\x1f\x06\x86\xe9F\xf6\xf6N\x0e\xc1\xc1\xaaL\
+llb\x0f\x1f>T\xfe\xc3\xc0\xb0\xf6\x1f\x03\x831\
+\xd0y\x9b\xdf\x89\x89\xcdz\xa2\xa0\xc0\xf0\xf5\xebW\x86\
+\xdf\xbf\x7f\xfbGEE%\x03q\x01\x1f\x1f\x1f\xff\xe1\
+\xc3\x87?\xb3\x00mRU\x10\x17\x17\xff\xfe\xe4\x09\x03\
+\x88\xde\x0b\xe4C-\x9e\xf9\x93\x81\xe1\xf93QQ\x10\
+;\xed\xd7\xaf_\x0c\xaf^\xbd\xe2\xd4\xd0\xd0p\x07\x19\
+\x06\xa2\x1f<x\xb0\x9d\xd9\x9a\x81\xc1\x91\xe9\xcb\x17Q\
+\xa1_\xbfx\xce\xdd\xba\xf5\xf2\xce\xc7\x8fg\xa7\x03]\
+\xf0\x86\x81\xe1\xac\x04\x03C\xe4\xb2\xd7\xafg}`d\
+<\xfb\xfa\xf5\xeb\xb3o\xdf\xbeU\x17\x11\x11\xe1\x97\x91\
+\x91Q\xdc\xb2e\xcb\xbe\xcd\x9b7\x9f`T``\xd0\
+\x07z\xaa\x86\x85\x81A\x11\xe8\xf4\xfb\xbb\x18\x18&=\
+f`\xb8\x0b\xb4\xf5\x07\x10\x03\x85\x18\x80A\xc4\xc0\x0a\
+\xc4\xec,,,b\xec\xec\xecf@\xb6\x00\x10\x7f\xf8\
+\xf9\xf3\xe7\x11\x90$\x17\x10\xf3Bc\xe4/T\xd3o\
+(\xfd\x0fj\x00H\x8e\x05\x093\x031(\x09\x7fg\
+\x1cM\xca\x94\x1b\x00\x10`\x00\xc7\xc2x1&l\xf2\
+\xc7\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02i\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\x0bIDATx\xda\xa4\
+S\xbfk\x14A\x14\xfevow\xcf\x0d\x9c\xa49\xa3\
+\x16\x12\x02\x11\x0b!\xc2\xb4\xdaH\x08\x18\xc1B\x0b\x05\
+ccsb\x95\xc6\xff\xc12\x95\x90\x22V\x0b*\x12\
+\x90\x04,$]\xda\xbb &\xc4\xa8\x84\xa0M\xce\xc4\
+\xc8\xe6.\xb7?gg}on\xef<\x85\xa0\x90\x07\
+\x1fo\xde\xcc\x9bo\xde\xaf1\xf2<\xc7I\xc4\x9ax\
+\xba\x0e\xc30\xc0D\xcd\x95g8;\xf9X\xdb\xc3\xd5\
+j\xdf\x89\xecyR\xabRJO\xa6)\xd28\xd6H\
+\xa2\x08\xd6 \xdb\x99\xeb\x8f\xfa\xeb#\xdf\x87[\xa9\xf4\
+LQ\x80\xc5\x1b\xbcc\x1e\x17\x1a\xbf\x14\xb4ZZ3\
+f\xa6\xcf\x0b\xd2\xb3\x14\xea\xcc\x7f\x11\xb0dR\x22\xee\
+tt\xb8\x87\x87\x19\xeeO_\x10i\x92\xfcAbR\
+\xee\xf3\x84:k\xde\x18\xb05\xb2,\xab3A\x18J\
+\xec\xec\x04\xb8wcL\x93\xe4\x05\x89E\x87\xe2\xe1\xdd\
++\xe2\xf9\xab\xf7\xfd|\x1f\xdc\x9e\x10A \xc1\x0d\xea\
+\x22\x87\xef'\x88\xa2\x0c\xdb\xdb)\xeeL\x8d\x8b\x17K\
+\xebL\x02\x8b+\xd9j\xa5\xba\xa2=i\xb7S4\xf7\
+\x02\xb4\x83\x10A\x18\x22\xa5\x1aP$\xfa\xacT*\xe1\
+\xeb\xae\x8d\xc9\xabc\xe2\xed\xca\xe6\xac\x95\x90\x83\xe3\x94\
+\xc0\xba'\x072\xc3wSA\x0e9P\xae\x0d\xa5\x88\
+4\xce\xd0I\x94>\x1f\xad\xbax\xb3\xdchP{\xe7\
+\x8c\x91\xda\x12\xe7,\xc8hP\xc3k\xe8\xd6@\xfc]\
+\xd0\xca\xad)\xb1\x1f*\x8c\x9e6\xd1\x5c|\xa7/\xdb\
+\xe5\xb2g\x91sM\xd1\x13\xa6i\xf6\x06J\xdb=\xe1\
+<\xa9\x1b\xf5\x03\xeb\x14*\xc3\xc07\xefu\xf7\xb2\xe3\
+\xe8y\xb0:\x8d\x97\xda)\xdd\xdd\xd0\xb0\xcf]\xd6\xe8\
+O\xe1\xc5\x9bZ\xbb\x06\xe0/x\xfa2~~\xf1\x8e\
+>,j\x7f\xe3_\xb3nV/\xc1\xba\xf6\xa4\xae\xa3\
+\xf9\xf1iNm-{\xd9\xde\xc7\xdf\x7f\xa1\x18&\x97\
+\xd3,0T\xeckQ\xfb[\x90\xcd\xcd\xcf\x88\xfc5\
+\xb5\xb6\xb0A[\xe3\xdc\xa8\x02!G\xc0\xb0\x09\x0e\xa1\
+\x5c\xac\x8f\x9bP.NJ\x88\x09\x09\xaf\x8d\x93~\xe7\
+_\x02\x0c\x00\xa0\xa21\xf7\x9c5\x01j\x00\x00\x00\x00\
+IEND\xaeB`\x82\
+\x00\x00\x02Z\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xfcIDATx\xda\xc4\
+S\xbfk\x14A\x18}\xb3;\xfb\xf3\xee\xbc=0\xe6\
+\xce\xe38\x0e\x22),L\xa1\x12\x0e\xed\xd2&'\x04\
+\xb4\xc8\x1f \xfe\x0b\x1a0`0 \xb1\xb11\x85(\
+)RX\x04\x0c\xe9\x0cZ\x88\x82\x98B\x10\xb4\x08\x16\
+\x12\xc2\x81\x09\xf1\xcc\x8f\xbd\xbb\x9d\x99\xdd\xf1\xdb-\xd2\
+\xca\x91\x22\x1f<f\x8ay\x8f\xf7\x1e\xdf0\xad5N\
+3\x06N9\xfc\xf6\xdc\xdc$\x9d\x17\x07\xe4\xb5\xc9\xf9\
+z&\x10+U]\x9d\x9f\x7f>\x08{zv\xf6\xde\
+\x89\x03\xa5\x94\x91P\x0f7\x16\xfa0)\x90\xcd\x81\x84\
+j\x89c\xa0\xe8\x01yG\xc3\xb7\x81\xabu\xc0\x97\xdf\
+\xe0\x1a\x87\xe8\xf7z\x9c\x00)D&\xc0\x14\x09\x5co\
+0\xe4\xe8qJR\x09`\x92z*(\x14\x15\xc5\x80\
+\xd12\xb0\xfd\xf37\xee\xb4Zx\xba\xbc\xecQ\x84k\
+\xdd0\xdc\xe4RJC%\x09\xfe\xfeYB\xb9v\x05\
+\x97.\x8cS\xb3\x0c\x81\xaf\xd19\xea\xa2\x1bv\xa0\xc5\
+\x1e~m\xedC\x88>\xda\xbb\xbb\xf8\xb2\xb2\xf2\xe4r\
+\xabu\x9fD\x0c\xae\x840S\x07\x9b?\xdeck\xe7\
++\xa6\x9b\x0a\xcd\xd1q\xc8\xd8@\xed\xbc\x8fB\xad\x80\
+R\xae\x81\xa2oP<v\xd2\xc3\xf7\xb5\xb5\xc7\x8d\x89\
+\x89\x87\x5c\x08\x919h\xef\x1c\xa2\xe3J\xbc\xd8\x7f\x89\
+\xd5\x0foP\x1b\xaa\xa3Z\x1aF\xe0\xb9p\xa0a\xca\
+\x08\x8a\x1c\xccLM\xa1V\xa9\xa0\xdcl>b\x8c\xbd\
+\xe32\x8a2\x81J\xfe\x16l\xdb\x85o\xe5P0\xf3\
+\x80\x0e\xd0C\x00\xd7\x0b\xe0\x14\xf3\xf0\xcf\xb9\xd8\xfb\xfc\
+*#\x07cc\x0bD~\xebx\xde\xa7\xd4\x81\x19S\
+\x04\xc7\xf1\x08\x0el\x82\xc9-h\xcd\xd0\x8f4\x8e\x8f\
+%\xdd%\x84\xb4\x10\xdbCx\xb0\xb8\x88\xe1j5\x8c\
+z\xbd\x8f\xdc\xb2\xc0\x8f\x0e\x0el\x93s\xac?\x9b\xf9\
+\xff\x02\xdc\x9c$\x976^ol\x18)9\x1d\x96\x1f\
+\x19\xb9k\xe6r\xf5A\x16)\x0e\xc3\xed\xa4\xdb]\xca\
+\x04\x08\x0e\xa14\xc0\xbf\xa0-A\x87\x10e\x02g\xfe\
+\x1b\xff\x090\x00a\xe3\xce6\x02\xb7\x87\x0e\x00\x00\x00\
+\x00IEND\xaeB`\x82\
+\x00\x00\x01\xe3\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\x85IDATx\xdab\
+4.\xdfm\xc6\xc0\xc0\x00\xc2\xa7\xa0\x18\x0e>|\xf8\
+\x00\xc6\xff\x7f~bx\xb7\xa1\x98\x01\x1d\xfc\xff\xff\x9f\
+\x81\x09H\x98\x9f\xe9pI\x00\xd1 \x01d\xcc\xcf\xcf\
+\xcf\xc0\xc1\xc1\xc1\x80\x0f\xb0\x00\x15\x9e6*\xdb\xc5\x08\
+d\xff\x05bq \xff\xe5\xbf\x7f\xff\xc0\x06\x80h\x90\
+!\xbc\xbc\xbc\x0c\x8c\xa6\xe1\x0coO\xaf\xc40\x80\xd1\
+\xb0t'\x8c-\x01\xd4\xe4\x06\xa4w\x015\xbe\x80\x19\
+\x00\xa3al\x90!0\x17\xbe?\xbb\x9a\x81\x05\xc9\xb0\
+\x17 \xcd@\x09w \xbd\x13\xca\xc7\x00\x82\xc6\xa1p\
+CA\x80\x09M\x1ed3H\xb3'\x10K2\x10\x01\
+\x98\xb0\x88\x81\x0c\xd9\x01\xc4D\x19\xc2\x84C\xfc9\xd0\
+\x80\xed@\xda\x9b\x90!\x8c0\x06\x8f\xac\x1e\x83\x84U\
+\x0c\x03\x97\xb4\x0e\x03R\x00J\x01\xb1\x0f\x10o\x01\xf2\
+\x9f\xa1\x07\xec\xfd\xd9\xe1\x08\x03\x90\x0d\x12\xb3\x88b\xe0\
+\x94\xd2\x86)\x04\x19\xe2\x07\xc4\x9b\x80\xf8\x19A\x03`\
+\x80[F\x97A\xd4<\x92\x81CR\x0b\xa4X\x1a(\
+\xe4\x0f\xd4\xb8\x11\xc8~J\x94\x010\x00\xf2\x9200\
+\x11\x01\x0d\x92\x06j\x0c\x04\xe2\xf5@\xfc\x94h\x03`\
+\x00\xe4%`\x1a\x90a\x13\xd7H\x01rY\x81\x86\xec\
+\x7f0'b\x0f\x134 \x99A\x82@\x0cJ\xf8\xdc\
+@\xcc\x07\xc4\x02@,\x04\xc4\x22@,\xf6\xfd\xd9U\
+\x89g\x9b\x1b\xfe\xfe\xfa\xf5\x8b\x0fh\xb3\xfb\xef\xdf\xbf\
+\xbd\xc0y\x81\x81D\xf0\xf3\xf3\x9b\x83\xa2\x91s9\x18\
+\x19\x19\xf7\x82\xa3\x11\x14 \x94\x00\x80\x00\x03\x00\xbd\x03\
+\x05*\xd1F{M\x00\x00\x00\x00IEND\xaeB\
+`\x82\
+\x00\x00\x029\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xdbIDATx\xda\xa4\
+S;/\x04Q\x14>3sf\x16;k=\xc2\x16\
+\x1e\x11\x91\xf5\xaa4\xa2E\xa2P\xe8\xc8\x86\x82NT\
+tJ\xa1\xa1\x12\x9d(4\xaa\xa5\x12\x09\x11\x09~\x80\
+D\x87Dd\xb5\x96\xc1\xda\xd9\xb1\x8fy\xb9\xf7\xae;\
+vl\xb2\x0a'\xf9r\xcf\xeb;s\xee9w\x04\xd7\
+u\xe1?\x82skO \x8ab\x18\x11W\x89\x1d#\
+\x88\xfc\xc1I\x12\xc4-\xcbZq\x1c\xe7\x03\x1d\xc7\x06\
+\x82\xd5\x81\xa8\xbc\x18\x1b\xab\x85\xa6:\xa9\x22\xfb%e\
+G\xe2g\xe9\xc5\xab[\x93\x9aK\xa2a\x18@\x10\x9b\
+\x1a\x0dB\xbd\xea\x02\xa9\x5c\x114gr\xa4\x86q(\
+\x17u]\xa7\x95\x22\x8da\x91%\x94\xca\xc4\xd2\x0d;\
+\x8f\xb6\xfa}\xfe\xc6\xb0\x04\x84\xc7\xae\x8a\x99L\x9a9\
+\xc9}\xca\x0a\xf0\xd8o?\x1d<\x8f\xa1a|2\xc5\
+\xb6m\x06.\xa6i\x02\x8f%\x12\x8f$V,\x22I\
+\x08\xaa\xaaz1\xcc\xe5r^\x07\x14C\xd3\x17e\x83\
+\x9b\x5c\xbe\xf7\xf4\x83\x8d(\xe4\xf3y\xe0<\xb4,\xd7\
+k+\x9b\xcdC{\xfb\x88\x97\x9cH\x9c\xb3\xb3\xb3s\
+\xf4g\xef\xf8L\xd6.\x01\xe7\xa1  S\xb2\xd9\x02\
+i\xab\x00\xfb\xeb5^\xf2`\xac\x18\xdb_\xffY\xad\
+\xa6U\x91\x02\x02p\x1ey?\xd5L)\x14\x1c\x90e\
+\x05\xd2\xe9\xcf\x92\xaf\x15c\xa5>E\x09\xf8b\xa8(\
+\xa1\xef\xe1(\xd4\xf4\xdd\xbd\xadm\x90\x9d\xb2,\x94\xcd\
+\x85\xf30\x10`JRK\x89\x91\xa6z\xc5\x97t\xb8\
+)\x7f\xaf\xd3\xf4\xbf\xe5W\x13\x08/\xc9>lh\xd7\
+\xd0\xd23\xd3\xfa\xae\xc3PwG5\x84\x82\xc8\x86T\
+\x1c\x140p\x9bBK\x01\xec\x1dg\xe0\xe9U\xdc\xbd\
+;\x9f=\xa5\xbd5\x04\xeb\xa2]}\xc3;\x0bjC\
+\xef8\x80\xd0\x5c\xf9_r\x9f3ow'\xb7\x97\xf3\
+\xdbF\xea\xfe\x81\x16\xa0\xd3\x08\x95\x0d\xe0o\xa1/K\
+\xff\x12`\x00\xa0\xd5\xe5\x1b\xde\xef\x9cz\x00\x00\x00\x00\
+IEND\xaeB`\x82\
+\x00\x00\x02\xf9\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\x9bIDATx\xda\x9c\
+S\xdfKSq\x14\xbf\xdf{\xef6\x96n\xfej\xcc\
+9]\xcb\xe6\x8f\x95A\xa8%\x85$\xca$a\x06\x15\
+\xf4\x83 \xb2\x1ez\xecA\xa2\xbf\xa1'{\x0e\xea\xa1\
+\x22\x08\x1f\x1c\x14\x81\xb5\xa0Lt`\xebi\xc5\xe6&\
+\xbai\xba\xe6\xa6\xd9v7w\xb7\xfb\xbd\xb7slW\
+t\xd1K\x07>\x9c\xf3\xfd~\xcf\xe7\x9c\xef9\xdf\xf3\
+%'\xeeM2(\x84\x90r}\x0a\x14bNQ\x94\
+9\xa6$`\xef\xd3,\xf3\xb7\xd8\x01np\xe8\xf1?\
+p\x8d\xa0\x86\xf5-\xdc+\x9d\xed\x13\xbe\xcc\xeek\xac\
+\xd3\xb7^;csfE\xa9\xb6\xf3\xfe\xbbgw\x5c\
+G\xba\x87\xbb\x1a\xaa\xa7\x83\xc9\xd8\xcb\xd9e\xdbJ*\
+\x17\x06\xbf)\x80\xb4sS\xb5\x04\x90\xa1\xfe\x0e\xf3\xf1\
+\xd1\xf3m\x83`k\xa9\xac\x14\xf7f\xe2X\xa2\x01U\
+\x18{=\xef\xfd\xf05\x11\x00{\x87\xc8\x97jio\
+\xb1\x18ZG\x87\xdb\x06\x8b\x92\x8c\x1b\xf9\xf2\xab\xca\xb2\
+B1!\xfa\xac\xa4\xb2b$\x9e\x89\xc2:\xc4\xca\xb2\
+\x8c\x0d\xe9\xbc=\xd0|L\x94dY\xa2\x8a\x04\xa0\xff\
+\x80\x84>\xe8\x8b\x1c\xe4\xe2\x0dz\x01\xd6\xf9\xb5t\xe5\
+!SEao\xd6\x22\x95\x0bB\x9e\x0aB^\x82\x96\
+P\xb1\x08\x01p\xff[t\xb3\x1a\xc8V0{Y\x0c\
+\x10x\xe8\xbe\xfa\xd8\x1b\x09\x80\x03E\xe4D\x9a_\xd9\
+\xd8^\x0b\xc7\x85\xe8\xeaF.\xf5+[\xd8\xce\x8b\x94\
+RI&\x88\xf1\xd9\xd8\x22r\x90\xcbC\xa4\x99\xa3w\
+_\xb1#\x03\x8e\x0e\xa8_\x86lB2#n\xed\xd4\
+LJ\xcf\x8c\xa3\xa10D\x1d\x85\x0b=M\x0e\xe0L\
+\x80=\x83%L\x03\x1c\xcd\xe6\xca\xa6\xf4v\x91\x01r\
+\x1a\x9d\x15|VE\xa50\xbbq\xb4<\xabi\xb5\x18\
+\xd3\x908\x0e\xc36\xad6\xd1\xff\xc4\x1b^\xd2\xf2\x84\
+\xb0\x84\xe1\x09\xcb\xf0\xec^\x90?\xe08\xa21\x19\xb5\
+\x86\x17S\x0bq\xe4 \x97\xab\xe9\xba\x8c\x01\xd67\x05\
+\xb1>\xb1\x95c\xfa;\x1a\x1a)4\x97RE!\x0c\
+\xc6#\x1cdb\xf5:^o2\xe8\xf4\x8f&\x83\xa1\
+@\xecg\x048\x1fq\x04\xd4\xba\x98\xda\xee+\x1a]\
+\xbd\xd3mwv9/\x9d\xb6[z\xda\xcdU\x1e_\
+\x8c\xf3\xf8\x16c\xd7\xfbZ\x1c5\x15\x9a\xc4\x84/\x1a\
+\x8f\x06\xbf\x04\xc5\x1f\xc17\x9b\xfe\xf1\xa2Z\x96:\xc6\
+u\x80\x83\x95\xed.[\x85s\xe80g0\x99\xe0\xb8\
+j\xf5\xe9\x8d\xb3\xd6\x9b\xcf?\xd1\xcc\xfaB68\xb9\
+$\x84\xde\x7f\x07\xbf$ \x85\xe3\xac\x06\xc0n\x1f(\
+a\xf7\x7f\xd4]\x1c;It\xc6s\x8a\x98~\xbb\xe1\
+\x19\xfd\x5c\xda\xc6\x89\xcc\x02r8\xa0D\xfd\x96\xff+\
+\xbf\x05\x18\x00wA~.Fc\xa1t\x00\x00\x00\x00\
+IEND\xaeB`\x82\
+\x00\x00\x02\xad\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02OIDATx\xda\x8c\
+SKk\x13Q\x18=\xf3\xc8d\x82-\xb1B\x22E\
+\x90fa\xa0\x08YX\x17n\xb4\xabV\x10\xb1 X\
+\xd4e7u\xe5Op\xe1\x1f\xf0U\xa9\xba(\xddT\
+\x5c\xc4\x85\xe2Fp\xdd\x08\xc6.\x1a\xa4\xa1\x15j \
+j\x1f\x12mf\x92y\xdd\xcc\xf8}\x93L2\xd9\xf5\
+\x833\xf7y\xcew\xe6~\xf7JK\xd3\x08C\x92\xd0\
+\x8f\xdd\xd4\xa4\xf6\xe3\xc4\xf9\xeb\xd4\xcd\xf4\xa6\x0e'Z\
+\xdf>\xe4\xac-7\xda\x13\x04\xddV\x1d\xd0\xf0\x920\
+\xc5\x9dS{[j\xe1\xeaL\xf6\xd2\xc2\xfdq\x1e\x7f\
+^y\xfa\xbb\xfe\xb1\xf8\x00i\x88\xde\xde\xaf\x84\xc50\
+\xf1\xb3\xe9\xbe@yv~a\xaaZ\xad\x22{\xf7\x05\
+t]C:=\x12.\x1c\x1d\x99\xb0m\x17\x07\xaf\xef\
+!\x9f\xcf\xe3Sq\x95\x05.\x86\x0e:\xfe\xc0\x82\xeb\
+\xbah6\x9b8x|\x13\x9a\xa6\x85\x90e\x19\x9e\xe7\
+\x85k\xc9d2l\xe3\x1c\xb5\xd3\x19\x0c:4\xc8\xe5\
+r0\x0c#\x1c\xd7\xe41X\xb2\xde_\xd7u\x1de\
+[\x83\x99\xca\xe8\x7f2\x93\xf0\xfd\xce\xb0\x03\x16\xe0l\
+\xbc\x91\xc3\xc3\x08\x16\x1f\xaeB\xd0\xbc\xeb\xfbp\x84@\
+yc\x03\x95\xcd\xcd\xd1\xda\xc4\xe5s\xc2\xf3vdv\
+\x10\x81\xc9q\xb8\x84\x80\x88\x82[\x82O\xf6M\xd3\xc4\
+\xa37\xebgin\x86r\xe4eA\x0e\xfa\xa0\x0c\x11\
+\xd9\xb2,\xda\xdc\x82L\xf5U\xe8\x1c\x18z\x22\x81F\
+\xa3\x81\xa5\xb55\xcc\x16\x0a\xcf\xab\x95\xca\xbc*bg\
+\xc0D\xdb\xb6\xd1n\xb7\xe18\x0e\xcc\xa4\xde\x17\x88\xe2\
+\xf6\xdc\x1cl\xda'\xd3\x81\xbe+\x95\x9a\xaa\x10\x03\x01\
+\xce\xcaU\xf0\xc9\xb6DD\x9f.\x0bS\x15\xbee1\
+\x11v\x22)\x0aWD\x19r\xc0Y\x99\xa8\xd0\x22\x87\
+O\xd7\x8d\x1dp)IuHD\xa5\xbe\xeb8\xb2\xea\
+\xc5\x04\xf8v\xca=rX\x15\x11t\x05#\x071\x11\
+\xfe\x92\x80\xa2\xd6L\xe0Ljp\xc1\xe3\xff\xcbU\xe0\
+'\xc2\x0e$Z\xf3\xd9\x0d\xffR\xd0\x15n\x19FB\
+}\xfb\x0b\xb8q\x1a\x18\xd7\xba$%\xe6 \xe1Y\xb8\
+s\xed\x02\xe2\xc1f\xbe\xef\x1e\xee\xed\xe8\x99\x15r\xbb\
+\xcf\x8f)\xf5~\x1f\xa3\xb7Nv3%\xe8\x80\x02\xca\
+\xc0\xb8\x92\x8d\x8c\x05Cmq\xbd\xfe\xf3\xcb\xbf\xfa\x13\
+\xea\x1a\xa1\x00![ka{\xf9U\x09\xc7\x89\xbf\x01\
+\xb6\x99C\x10\xff\x05\x18\x00\xbcv)\xa3\x8f\x8b\x0c\xb4\
+\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x03*\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\xccIDATx\xda\xa4\
+S]HSq\x14?\xf7\xee\xaamB\xb8\xd0\x92\xbd\
+\x141\xddr\xa8\xc3\x81\x1f\xad\x0f\x9b\x19\xea\xa0\xc7\x22\
+\x10\xa4z\x10\xa4\x22\x18\x08BQF\xe1\xa3\xa4C\xd8\
+\x83(\x14\xc4\xb2/\x86\x16\xe8J\x03\xd9\x0c\xc5\xad)\
+d\xb8\x8a\xc2\xf6\xd0\x9d\xfb0u_\xde\xfd;gn\
+\xe5{\x17~\xf7\x1c\xce\xefw\xce=\xf7\x7f\xce\x9fc\
+\x8c\xc1\xff<\x02\xbd\xccf3\xf0<\x0fyyy\xc0\
+q\x1cPQ\x99L\xd6\x80TUV\xe7\x93$\xc9\x9d\
+\xe3R\xa9\x14\xa4\xd3\xe9\x7f\x05r\x0f\x92\xc7\xd1T\xa3\
+u`\x82\xden\xb7\x0f\x91\xb8\xbd\xbd\xbd\x0bc?\x90\
+;\x8f\xf6#ZW.\x87\xdf\x93l,//\xbf`\
+\xb3\xd9\x86\x94Je\x07&\xf2\xc1\xa0\x08\xd1h\x84\xbe\
+\xc8S\x8c8\xd2\x906\x97\xc7QK---\xe4_\
+G\xc1\x80(\xfe\x02\x95J\x05\x1e\x8f\xd7\xaf\xd7\xeb\xd5\
+Dx\xbd^\xbfV\xabU\x87\xc3!()9\x08\x9d\
+\x9d\x9d70<\xf8\xb7\x83\x8d\x8d\x0d\x88\xc7\xe3/-\
+\x16\xcb\x9d\xfc\xfc|\x10E\x11**\x8e\xa9\xd3i\x09\
+\x08\xe4on\xfe\x06\xe2HCZ\xca\xb979\xb9[\
+\x00\xbb8\x9dL&/\x06\x02\x81-\xfc\xda\x17A\x10\
+`nnn\xa5\xad\xcd<D \x9fb\xc4\x91\x86\xb4\
+\x94\x93\xfbw\xa8\xa9\xa9\xe9^X\x98g\xd3\xd3\xef\x98\
+\xdb\xedb>\x9f\x8fUVV\xf5\xe1$h\x1a@>\
+\xc5\x88#\xcd\xe2\xe8\x08\x9bV(\x96]\x1c\xd7\x98\xe9\
+ \x91H\xc8\xe2\xf1\x04\xec\xecH Ii\x1c\xa5\x80\
+\x89B\x8aFE \x9fb\xc4\x05\x83\xeb\xb0\xb4\xea\x87\
+\xc6\xeen\x9d\x08\xd0\x9b\xe9\xa0\xac\xac\xacY\xadV\xdf\
+\x22\x0c\x0eZ\xbfy<\xcb\xcc\xe1pz\x0c\x86\xda\xdb\
+\x04\xf23\xb1\xb1\xdem\xa3\xd18\x1e\x8b\xc5X\x93J\
+\xf5l\x04\xe0\x9c\x90\xed`\x0a\x0b\xad\xe2\x09_3\x18\
+\xea\x8f\x84Ba\xd0h\xb4\xfa\x89\x89\xf7z\xe2\xa3\xd1\
+uX\xfb\xfa\x0a\x84\xa4S\xee\x1c;e\xd6\xe9t\xfd\
+\x91x|\xf4\x12.X\xa6\x00\x9e*\x99+V\xeb\xb0\
+\x85\xc6\xa8T\x1e\x80\xa9\xa97\xdfkk\x1b\x0e\x13!\
+\xae\xbd\x8e\xc1\xb6Cn2\x9d\x84\xa7co\xa1x\x7f\
+\xa88\x12\xe1}N\x85b\xf7\x10qI\x08\xad&S\
+\xf3\xe3\xf9\xf9\x15\xa6\xd1\x1c{XTT\xf4\xc0\xe5Z\
+b3\x93\xc3\xcczW\xf0\xc7\x02=\xec\xd1@=;\
+{\xa2\xf49i\xb39\xbb\x052;\x8dc\x92\xcb\xe5\
+m\x85\x85\x85}\x05\x05\x05G\xc9z>\xcc\xb2I{\
+\x13\xa3\xe4\xfe\x1e\xce]W\xbd\xef\x09iH\xbbw\xff\
+sw\xe2\x10B\x870\x10\xf0bu\x5cn\x95\xcd\xb2\
+\xcd\xcf\xec\xfeM\xfe\xd3\x99:\xe8\xcar\x95\x88\xd2\xdc\
+=\xca\xac2\xde2\x1a\xa7\x22\x8b\xbd\x17\xec\xe7U3\
+7\x1e\xde\x02\xdb\x8b\x19\xb6\x98\x8dI\x88-\xc46\x22\
+\xfdG\x80\x01\x00\x05|\x84e\xc3\x14\x9e\x1a\x00\x00\x00\
+\x00IEND\xaeB`\x82\
+\x00\x00\x02_\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\x01IDATx\xda|\
+\x93\xcfK\x14a\x18\xc7\xbf\xf3#Dl\x88!T\xd4\
+:\x06\xe1R\x07\xf1\xb0\xc5\x0a\xb2\x9d<t\x08\xa2\xbf\
+\xc1S'!\x08TX:t\x0b\x22H\xe8fl\xa7\
+\xe8\x1e\x0b\x8a \xe2Am\xda\xca\x84\x04/\xe2h\xe9\
+\xe6\xba+\xad;\xf3\xbeo\xcf\xf3\xee\xac;\x8d\xdb>\
+\xf0\xec\xfb\xee<\xf3\xfd\xbc\xdf\xe7}\xe75\x1e\xce\xcc\
+\x80\xc30\x8c\xfb4\x0c\xa0s,H)\xb7\xa5\x10P\
+Jaky\x196O8h\x1c\x9c\x9f\x9d\x9d\xabS\
+1\xe0\x94\x12\x82j\xcd\xba\xe7y\x98/\x14&y-\
+\xca\x1f\xfc\xecf&\x03\x93iQ\x1a\x92EA\xa0\xb3\
+^\xab\xe1\xcf\xe9)\xaa\xd5**\x95\x8a\x1e\xdf\xe7r\
+s\xf4\xde=\xd2\xdehZ\xb2\x05\x89\xa30\x18m\xd2\
+\xef%\xcbj\x99\x0eC\x84\x04.\x95Jx\x95\xcf#\
+;<\xfc\xfae>?M\x95g\x1a [\x00\x93\xc5\
+\xa6\xc6\xe0\x02$\x9b\xcd\xeav\x1c\xc7\xc1G\xcf\xfb}\
+\xee \x8c;\x88\x01\xdaA\xd8\x89\x9eR\xbb\xad\x16\xa8\
+\x90l!\x1eI\x08/B\x9a\xb6\x80F\x0b\xa6\x09D\
++\xb5\x83X\x0d\x80\xd9j!\x068w\xd0\x01b\xd1\
+\x18\xfe\x07\xa0\xf7@\xefC\xc3\xcf\x05\xc8\x93\xcdi\x14\
+O\xbea\xf7\xd6\xafG\xce\xb1\xfbB\xc8\x80Z\xa03\
+O:`Y;H\xf1\xe8\x0bF\xef\x8ebs\xf7\xdd\
+\xb5\x92\xe3SI$Z`\x07tTI\xc8\xe3\xd5)\
+l\x1c\x15\xf9{EY\x94\xa1\xce\xa4!\xbb\xc4\x1a\xfd\
+]\xb7\xcb\xbe\x8f\x9e\xde\xde\x7fNA& \x9f\xf6?\
+\xc3\x1d\xbb\xaaW9\x0c\x0f\x91ypg\x88\xa6C\x8b\
+\x1f\x16`o/-\xe1z:\x8dn\xd7\xb5\xa3\x8d\xd0\
+\xa28d\xe4\xcaml\x14<\x0d\x08\xc6\x81\xad\xb7\xdf\
+\xf7\xc2\xae\xbaO\xb7b\x9d\x9fuS\xf6\xf5\xa7\xd39\
+\x15\x0b\x02(!\xa5\xa2\x8fG\xd1\xe5Rt\xc9\xd4\xc8\
+\x9b\x8c\x1a\xdcI)\xeb\xa9\xbb\xc7\x1a\xd6\xdaM\xc0\xc9\
+\xc1\xc1\xf1\xe5T\xeay\xa7\xbb|\x96\xf2'\xe4J\xad\
+\x1f?\xd5\xd7\x08\x10\xfe\x15`\x00\xefX\x1e\xcd\xe7\xe1\
+\x8b\x7f\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02\xb0\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02RIDATx\xda\x8c\
+R=OSQ\x18~\xee\xe9-\xfdH[\xc2@\xbf\
+\x88\xc4P4\xd2&.n\xc0TY\x1cd\x22,\x0c\
+\x0c&\xc4\xd1\xc9\xcd\xa2\xe8\xe0H\x8c\x89L\x1aI\xba\
+\x95\x1f` &$\x0c\xd5\x85\x06\x16\x13\x89\x0e\xad\x86\
+\x8f\xa6-\xb4\xb7\xb7\xa5\xf7\xde\xfa\xbe\xa7\xbd\xb7*\x89\
+\xf1M\x9e\xbe\xe7\xf6\x9c\xe7y?\x95\x85L\x06l\x8a\
+\xa2\xdc'\x17\xc3\xbf\xed\xa3eYG\x96i\xa2\xdb\xed\
+\xe2\xcb\xde\x1eT>\xb0\x91\x8fo\xae\xaen\x5c\xd2e\
+\x87aY0\xe9\xce\xbe/\x14\x0a\xd8\xdc\xde~\xc8\xb1\
+\x08_\xf9\xbf[\xb3\xb3\x10\xac\xd6\x87b1\xa9\xd3\x91\
+\xb8l\xb5\xa0k\x1a\x1a\x8d\x06\xea\xf5\xba\xf4\xb9\xb5\xb5\
+\x0dzw\x97\xb87\xec\x94T\x93\xc8}SXZ\xd0\
+\xaf\xdb\xe5\x1a$m\x180H\xb8R\xa9\xe0u6\x8b\
+t2\xf9\xe6U6\xfb\x84n^H\x01k  \x98\
+,\xa4\x0c\xae\x88\xa4\xd3iYN0\x18\xc4\x87B\xa1\
+\xeadP)\x97\x11\x1a\x19\xe9\xf7Q\xc1\xe7\x83\x03\x9c\
+S\xca\xc9\xc9IDFG\xafd\x22\x8fT\xae\x13\xb5\
+F\xa9\x95\x8f\x8fa\x1a\x86\x8c\xfd\x83\xce\x0bss\xf8\
+V,\xa2Z\xab\xc9L\xbcn7\x86T\x15\xaa\x10\x1c\
+E\xbe%\xb0\x97SXjj\xda8\x01\xefr9\xa9\
+\xfa\xf3\xf4\x14\xf7ff\xf0\xe9\xf0\x10^\xaf\x17>\x82\
+m\xae\x9e\x80pJ\xd0\x9b\xcd\xc4\xf7\x9d\x9dg\x7f\x0f\
+\x9cGx'\x95\xea\x8d\x94`\xf7\xc4E\xde\xf8]\xa0\
+\xa5\xeb\xa5\xe8\xf4\xf4s\xfex\xb4\xbc\xcc\xdd\xc5\xd2\xfc\
+<\xc6\xa2Q\xe4\xf7\xf7qsb\x02~\xbf\xdfi\xac\
+\x8b\xca \x81A\x0f\xa8\x84\xb7C\x1eO\xe6z\x22q\
+\xf1xe\x05\xedv\x1b\xd7b1\xbc\xdf\xdaB<\x12\
+A(\x10\x80=\x1d\x86,\xa1\xd3\x11\xf6\xbe\x88\xd0\xf0\
+0\xc2\x14\x8d\xd3\xe2\x06\x8d\x11\xe9\xe9\xfa:nOM\
+a<\x1e\xa7\xd9\x8a?\x04\x149\x10C\x18<\x15\xd9\
+D]\x87AQ\xecEz\xb0\xb8\x08\x8bW\x98\xce\xec\
+EoC\xe8\xa37B\x16\xb1K\xd0\xce\xce \x8ev\
+wQ)\x95xm\xd5\xfe28\x91\xa4\xb7\xa3\xf73\
+\xe1\xff\xf9-s\x98\xcb\x01|\xc5|>|^\xadz\
+\x06;= p\xd3\x18*5P\xa5]\xe0)\xf0[\
+\xe60\x97\xa3\xfa\x08\xe1\x8b\x93\x93Z \x95z\x89\xff\
+0K\xd7k\xcc\xe1v\xfc\x12`\x00\x05\xfc+\xe7\xc0\
+x[\xc6\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x05\xc6\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x03iiTXtXML\
+:com.adobe.xmp\x00\x00\
+\x00\x00\x00<?xpacket beg\
+in=\x22\xef\xbb\xbf\x22 id=\x22W5M\
+0MpCehiHzreSzNTc\
+zkc9d\x22?> <x:xmpm\
+eta xmlns:x=\x22ado\
+be:ns:meta/\x22 x:x\
+mptk=\x22Adobe XMP \
+Core 5.0-c060 61\
+.134777, 2010/02\
+/12-17:32:00    \
+    \x22> <rdf:RDF \
+xmlns:rdf=\x22http:\
+//www.w3.org/199\
+9/02/22-rdf-synt\
+ax-ns#\x22> <rdf:De\
+scription rdf:ab\
+out=\x22\x22 xmlns:xmp\
+Rights=\x22http://n\
+s.adobe.com/xap/\
+1.0/rights/\x22 xml\
+ns:xmpMM=\x22http:/\
+/ns.adobe.com/xa\
+p/1.0/mm/\x22 xmlns\
+:stRef=\x22http://n\
+s.adobe.com/xap/\
+1.0/sType/Resour\
+ceRef#\x22 xmlns:xm\
+p=\x22http://ns.ado\
+be.com/xap/1.0/\x22\
+ xmpRights:Marke\
+d=\x22False\x22 xmpMM:\
+DocumentID=\x22xmp.\
+did:A383DFD8A324\
+11E0BDD0C34FC039\
+BF22\x22 xmpMM:Inst\
+anceID=\x22xmp.iid:\
+A383DFD7A32411E0\
+BDD0C34FC039BF22\
+\x22 xmp:CreatorToo\
+l=\x22Adobe Photosh\
+op CS3 Windows\x22>\
+ <xmpMM:DerivedF\
+rom stRef:instan\
+ceID=\x22uuid:AC1F2\
+E83324ADF11AAB8C\
+5390D85B5B3\x22 stR\
+ef:documentID=\x22u\
+uid:C9D349664A3C\
+DD11B08ABBBCFF17\
+2156\x22/> </rdf:De\
+scription> </rdf\
+:RDF> </x:xmpmet\
+a> <?xpacket end\
+=\x22r\x22?>S\xf3\x1b\x9f\x00\x00\x01\xf3ID\
+ATx\xda\x9cS=O\xdb@\x18~\xee\xce\xb1\xe3\
+\xa0|\xa8\x0dj\xf8(3C\x97N\x1d`\xe8\xc2\xc8\
+\x98\xff\xd0l\x8d2\xf0O\x083\x13?\xa0\xea\xc0\xdc\
+\xa5\x95\xbaU\xeaR\x81DC\xd3\x86\x90\xc4$\xfe\x8c\
+\xcf\xe6\xbd3q\x8a\x98\x82\xa5\xf7\x1e\x9f\xce\xcf\xc7{\
+\xbec\xcdf\xf3\x10\xc0\x06\x9e\xf7\xf4\x8d$I6\xbb\
+\xdd\xee\xc9|>_\x89Y(\x14\xd0j\xb5>(\x01\
+\x16E\x11\xda\xed6lZ(\xf9>\xd6<Oc1\
+\x8e\x01\xc60\x95\x12W\xae\x0b\xa7`\xc2\xb5\x8a(7\
+\x1a\xe8\x9e\x1cCq\x0d)%\xa7\x17l\xce&8*\
+F$M*UU&\x0d&&\xa3[\xf4\xaf\xff@\
+\xca\x18,$\xbd\x19p\xca\xa5\x22Cq\x95\x00\xa3\xc2\
+l\xad\x88\x1f\xbb\xdbH\xd3\x14)-&I\x8a\xdeu\
+\x0f\xbdQ\x04\xb6\xbd\x0e\xc198\x17\x1a=YVd\
+U\xcc\x88\xe3\x98\xabI\xd9t\xf1n\xeb_\xde\xa3\xe3\
+8\xa8\x87\x7f\xf1\xb6\x0ep\xa6;\xc9\xf1\xf7EE\x0b\
+(n\x9e\xc0\x81\x85/F]G\xf3\x83\x00\x97}\x9f\
+\xd2\xbc~\xe4\xacQp\xcc\xcc\xca\xd3\x04\x95Z\x80\xbd\
+\xf7#\xed>\x1c\x8e\xb0\xfb\xc6\xd3\x8e\x9c\x06\xed\xce\x1f\
+R\xd0\xfc\xe2\xac\xbaL\xb0\x10\x18:\x16>}]G\
+\x18\xceq3\xb0\xc1\xe8C!\xfew\x16\x84\x5c\xd7\x9d\
+o=\x12\xd0-X\x15\x81\x9d\xbd*|?\xc0\x0bW\
+\xe4\xcel\x8140\x9e\xe1\xcfK\xb1\x10X\xb6p;\
+\xe6\xf8|nS\x02\x0bHk\x99c\xee\x9a!\xcb\x94\
+0u\x07O[@\xad\x0a~\xb0\x0f\xee\xd3\xcfF\xaa\
+?L\xa8R*\xc9\xb2\x14\xd0H/\xbf\xbe-\x05\xc2\
+0\x14j\xe7\xc5\xc0\xc3\xf7\x8f\xa7(\xbdj\xc0xY\
+\x86\xa8\x95\xc0JV\x16=\x92\xe0S:dw\x01\x1d\
+\xa4\x106i(\x8e\xe2\x1a\xe3\xf1\xd8R\xf1:\x9d\xce\
+JwAq\x14\x97\xd9\xb6\xdd\xa2\xc9\xces\xae\x22\xa5\
+\xb8b\xfa\xc0\xd3\x0eP\x19+\xf2\xe9\xa6ar/\xc0\
+\x00V\x9c\x1c\x9a.}\xcf\x86\x00\x00\x00\x00IEN\
+D\xaeB`\x82\
+\x00\x00\x02\x95\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x027IDATx\xda\x8c\
+S\xcfk\x13Q\x10\xfe\xf6\xedF-&\xa4\x876\xda\
+B\x11\x11Q\xda^\x84B<\xc7\xab\xbdh\xbdx\x90\
+V<\x08\x1e\xfc\x0bl\xa1x\xf0\xe2E\x94\xf6T\xa4\
+\x90\x83\xe8?\x10\x8bB\xa1b\xfcQY\x0d\x0dj\xea\
+\xc5\x16k\x0c\xd9\xa4&aC\xb3\xfb\xe2\xcc\xcb\xbe\xee\
+\x16A\x1c\x98\xcc\xee\xce|\xdf{\xf3\xcd\xc4\x98\x9a\x9d\
+\x05\x9ba\x18\x93\x14\x86\xf0o{)\xa5\xdc\x94\xbe\x8f\
+n\xb7\xab>X\xfa\x81\xe2\xf0\xf2\xdc\xdc\xe2\x1e%;\
+\xecR\xc2\xa7\x9c\xce\xdb\xb6\x8d\xe5\x95\x95\x9b|\x16y\
+I3\x0af\x0b\xdc\x90\x0c\xeat\x94\xef\xb5\xdbp[\
+-4\x9bM4\x1a\x0d\x15\x9f\xcd\xcf/R\xdd\x05\xc2\
+\x9d\xd6\x04\x96O\xe0\xc0\x0c\xa6\x16\xf4\x1b3\xcd\xf0\xd2\
+\x9e\x07\x8f\x88\x1d\xc7\xc1\xc3l\x16\x99\xd1\xd1\x85\x07\xd9\
+\xec\x1d\xca\xdcU\x042$\x10\x0c\x16\x8a\x06\x7f\x91d\
+2\x19\xd5N\x22\x91@\xce\xb6k\xfb \x8f\x08\x02'\
+\x1d\x0d|r\xde+\x92\x02\xc5\x8b\xb9s8\x12\x8b\xe1\
+\x90e\xc1\x12\x82\x85\xee\xf1Q\xad\xc6Y>\xb1G[\
+\xb8\xbdv\x0d\xd3gn\xe1\xf1\x97Gx1\xb9\x81\x1f\
+\xf5:J\xa5\x12\x92\xc9$\xaa\xd5*\xd2\xe94\x08c\
+\x84\x1a\x84\x04\xaa\x85W\x97\xbe\xe2\xfc\xd3SX\xa3(\
+\xe9\xca\xc3\xfd\xfd8>1\xa1&\xd3\x1e\x19\x81I5\
+\x84\x11\xfb\x04^\x84@\x8b\x98\xbf\xf2\x0d<\x91\xa8i\
+ML\x8a^\x84@0A\xe0J\x83\xf5\xf2kE\xf2\
+\xa1\xf2\x06\xe9''\xa1\x85\xd5\xd3\x89\x91\x16\x5c\xabq\
+B\xcf\x9d\x5c\xdd`&w\x19\x0b\x1f\xef\xe3\xc6\xf3)\
+\xac_\xfd\x8e\x8a\xeb\xe2]\xb1\x88-\xea\xffm\xa1\xd0\
+k\x81j5\xee`\x0b\x94,N\xff\xc4\xd9\xa5\x146\
+f\xcajlC\xf18\x8e\x8d\x8f+=N\x0c\x0c\xa8\
+5\x8c\xb6`\xed\xee\xec\xe0\xe8\xe0\xe0\x81E\xfa|\xfd\
+\x17x\x81Y\x05\xd1\x93\x97^\xa4>E\xb5\xc0\xcf\xad\
+J\x05bsu\x15\xce\xf66\xaf\xad\x15\xfc\xa9T\x91\
+&\xd3\xef\x82H\xf4w\xaee\x0cc\xf9\x80\xbe\xad|\
+>\xb5[\xab\x1d\x0e\x17\x22\x04\x98\x14\xd9-\x12\xd0\xa2\
+\x85\xe2)p-c\x18\xcb\xa7\xf6\x91\xa7~\x97\xcb\xf5\
+\xf8\xd8\xd8=\xfc\x87I\xd7\xad3\x86\xe5\xf8#\xc0\x00\
+C\x847\xef\xe8\xa9\xbf\xc7\x00\x00\x00\x00IEND\
+\xaeB`\x82\
+\x00\x00\x02\xfe\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\xa0IDATx\xda\xa4\
+S\xcfO\x13A\x14~\xb3\xbb\xdd.\xdbm+\x05\x81\
+\x12\xa2h\xb1\xd4`\x83\x881\x1e\x94h4Jb#\
+\x89G\xff\x02\x13\xb9\x98\xe8\xc5\x9b\x89w\x12\x8c'\x0f\
+\x9a\xf8\x07\x18\x88\x88Gc%1$\x9a \xd2\x00E\
+Q\xf9Q\xa1\x14\xbamw\xb7tgg\x9d\x19Z*\
+'\x0fN\xf2\xed\xbc}\xef}\xdf\xbe}\xf3\x06\xb9\xae\
+\x0b\xff\xb3$\xfe\x88\xbf\x06@\x02\x80 \xd27\xd4\x06\
+\x08%\xa8q\x8e\xa2\xa3\x9a\xb7J1\x0d\xaeK\x13\xdd\
+\xdf@\x1c\xba\x11\xc0\xb3\x89=\x81\xbf\xd6\xa0\xda \xdd\
+={\xba\xa3;\x1ain\xd5|^\x1f+\xb0T\xda\
+5\x16\xbee/}\xfe\xb26dZ\xf6S\x9a\xf7\xf6\
+@\x055r(\xa8<\xbc\x95\x88\xf7\x11\x87h\x1b\x99\
+,l\xd4c\x81\xe8\xb1P \xd2\x19\x0a\x8fO\xce\x05\
+w\xf2&\xd4D\xaa\x02nXU\xc4\xe1\xa1\xc1\x93}\
+\x05\xbd\xa8\xe9z\x01&\x9e\xc4\x0f\x94\xf6`$\x0dk\
+9Y\xbbv\xb9\xabo\xfc\xcd\xd7a\xab\xec\xccPw\
+F\xe0Q\xe2$zO\x85\xbb\x0b\x85\xa2f\x18&\xb0\
+\xc6\x8e\xbeLqL&3<%vT\x06\x16\xdb\xb5\
+,-\x1a\x09u3\xce~\x05\xae\x83\xcf\xb7\xb7i\xad\
+z\xbe\xb0\xff\xc5\xb1\xf7\x06'\x0c\xf4\xe6\xa0E]\x87\
+\xf4R\x1eR)\x1dDI\x84`\xb0\xb1\x95qh\xda\
+\xb3\xbd_ \xb8C\x14@u\x1c\x070v@/\x94\
+\xc0\xb4\xca\xd0\x1fS\xe0\xf6\xf5FH-\x9b\xf0\xea\x9d\
+\x09\x82\xe4\x05v\xe8\xb6\x8dU\xc6\xa9\xf7\x80`\x841\
+F\xd6.\x06\xbdX\x06B\x10 Q\x82Gw\x8e\xf0\
+\xf0\xe3\x17\x1b y\xb5\xfd\xea\x08\x92\x10\xe3\xd4\x05\x1c\
+\xbc\x9a\xdb\xb6L\xa3\x22j\xa2\xec\x03\xb1\x9ax\xf3\xfe\
+O\xbe\xcbj\xe3\x81\x86\xda\xe5\x8a\xc98\xcc\xae6\x11\
+O\xaf\xfc\xcam*j\x00d\xc5\xcf\x81\xe8`M=\
+?\xc3\xc1\xec\x9a\x9f!\x9f+f\x19\xa7.\xe0\xe0\xb1\
+\x95\xc5\xe54\xad\xcd\xf0(\x01\xf0x\xfd \xc9j}\
+\x5c\xa9\xcd|\x0c\xd8\x06ckeu\x91q\xea\xbf\xe0\
+\x92L\xc52Gg\x93\xc9`\xcf\xc0\xd5x\x83\xff\x90\
+OR4\xb82\xfc\x9d\x87\xfd\x87\x8f\xf3\xdd\xd4w\x8c\
+\x85\x8fS\xb3\xb8l\x8e\xd2\xb1\xe7\xe7\x8b\xd8\x99#D\
+\x9b&w\x01x.\xde\xf0\xa8\xb1{\xed\xb1\xde\x13-\
+]=Mj0\xd4\xb0G\xdc\xb66\x97\xe6r\xeb\xf3\
+3i\xdb\x9c\x1f\x01;9\xe1V\x96\xf8\xbc\xd4\x04X\
+%M\x14\xcd t\xb6\x81\xd0\x7f\x01P{\x0fU\x0c\
+W\xdb\x96\x01w}\x0e\xc8\xa7\x0f@~lRG\x96\
+b\x8brqM\x80\xf5B\xadB\xfa\xc7\x0d\xa6W\x11\
+\x0cV\x18\xe5\x92?\x02\x0c\x00\xa3\x80,&\x09\xee\xf9\
+\x88\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x027\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xd9IDATx\xdab\
+d \x02\xd8\xdb\xdb3\x88\x8a\x8a\x22\x0b\xf9\x02\xb1\xe4\
+\xeb\xd7\xaf\x9f\xb3\xe0\xd2d\xc5\xc8\xc8\xc0\xcc\xcc\xccp\
+KX\x98\xe1\xe9\xd3\xa7\x0c\x9f?\x7ff\xe0\xe1\xe1a\
+\xe0\xe4\xe4d\x90\x93\x93\xd3\xec\xe8\xe8\xe8\x14\x16\x16N\
+gB\xd7h\x0e\xd4\xb8\x1a\x88W\x01\xd96@\x03\x90\
+\xc1\xdf\xbf\x7fA.)KMM\x8d\xb6\xb0\xb0(\x07\
+\x0a!\x5c`\x0c\xd4\x94\x05\xa4\xad\x81\x98\x1b\x8b\x8b@\
+\x9a\xc5\xc4\xc4\xca\xd2\xd3\xd3\xa3\xa3\xa2\xa2\x96\xde\xb9s\
+\xa7\x0b$\xce\xa2\x03$\x92\x81\x9a-\x804'\x0e\xef\
+\xc04gggG'$$,\xbd{\xf7n\x17\x5c\
+\x12\xe4\xd4\xbd@\x03\x8e\x03\xf1\x05 \xbe\x01\xc4\x8f\x81\
+\xf8\x09\x10W\xb2\xb33\x88\x88\x880\x00\x9d[\xb6e\
+\xcb\x96\x8bJJJe\xe8\x86\xb3\x10\x88\x00n))\
+\xa9\xec\xd2\xd2\xd2\xe8\xdc\xdc\xdc\xa5\xf7\xef\xdf\xef\x22\xc5\
+\x80\x82\xec_\xbflL\xdd\xdd\x05\x8bKJ\xb0j\xc6\
+\xe9\x853\x8c\x8c\xc6\xfb\x18\x18\xce\xfc\xef\xe8\xf8\x0f\xa2\
+q\x84+v\x17\xfcg`(\xe1a`\xb0U\xf4\xf7\
+W\x99VQqV\x8d\x81a\xe7n\x06\x86\xaf\xc8j\
+\x16\x03\xf1\x22l\x06\x005\x97\xfdd`\xb0SIM\
+\xf5>8k\xd6Y\xa0P:P\xec,#\x16\x8d\x18\
+.\x00*\xac\xf8\x01L\xb5\x06\xf9\xf9\x1e;&L\x00\
+i\xda)\x0d\xd4\x8cK#J\x18\xecad\xac\x06\x86\
+\xc3\x9e_UU\xffW\x02\xfd\x0c\x14k]\x0f\x14\x8f\
+ &\xa3\xac``h\x00j8\xfc\xb7\xa9\xe9?\xd0\
+\x963@\xdbZC\x19H\x00\xb3\x18\x18N\x83B{\
+.Ps)\x03\xc3D\xa0\x90\x08\x10\x0b\x01\xb1\x00\x10\
+\xf3\x011/4\x16@\x09\x95\x1d\x88Y\xa1^\x07\xe5\
+#Ff\xa0j\xfe\x17{\xf6\x08_g`8\xd6\x0b\
+6\x0f\xae\x90\x0d\xaa\x18\x84\x99a\x1a\xa0\x18\x0e\x00\x02\
+\x0c\x00\x22\x1e\x91D2\xef\x8cO\x00\x00\x00\x00IE\
+ND\xaeB`\x82\
+\x00\x00\x03=\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\xdfIDATx\xda\xa4\
+SKO\x13Q\x14>3\x9di\xa7C\xa9\xb4\xb4\x05\
+\x0a\xb1\x91\x97\x90\x80\x0bk\x80\xe0k\xe3#\x91\xa8\x09\
+\x1a\x17\xba4q\xeb\x1f0\xc4\x90\xb02\xbap\xe7\xca\
+\x85\xd8\x05&\xc4\x84hLt\xa1i`c\xc0\xc4D\
+j\xa4<Bii\xc5\xd2a\xa63\x9d\xf7xn\xcb\
+\xcb\xb8p\xe1I\xce\xcc\x9d\xf3\x9d\xf3\xdd{\xbe3\x97\
+r\x1c\x07\xfe\xc7\x18\xf2\x18x\xba\x0c\x0c\xcb\x02\xc30\
+@\xbb\x5cQ\x8a\xa2F1<\x8c\xde\xbd\x9b\xf7\x03}\
+\x0e7\x9b\xb6-+g\x9a&\x98\x86q@p\xc8\xae\
+2.g\xbc\xb3\x8d\x0f\xb5F\xb8\xa0\x9fgx\x0a\x83\
+\xa2b\xf6nl\xa9g\xd3\x19\xf9\xaen\xc1\x18\x86f\
+\xfe8A\xd5\x1c\xe7\xaa\xd7\x0d\x13#g\x22\xfde\xc9\
+\x02Kw@\xd4\x8d=\x94?\x1a\xe4\xf8\xbecum\
+3\xc9\xfc\x84dT\xdb\x9e\xd9'pl;J\x835\
+~y0\xda\xbf\xb5\xa9@Y5\xd5t\xae\x9c\xcd\x97\
+T\x81\xe0\xcd\x01\xae\xa13\xeak\xad\xc8\x0c72\xdc\
+\xd4\xff\xea\xfd\xfa\xb8a\xdb\xf3\xd8R\x8e&\x09\xa6\xae\
+\x8f\xc6\x9a\xb8P!'A\xb1$\xab\x1f\x17\xb2\xdf\xb2\
+\x05q\x0c\x89O\x11'k\x12\xdbFl3#BG\
+\xab7Dj,\xd4\xa1J\xa0k\xda\xe9 \xef\x0a\x96\
+wTH\xad\x15\xb3\x86\xae?A\xf6\x04\xc1\x14I\x02\
+\xfcN\x90Xjm;+\xedT \xe4g\x83\xa4\x06\
+\xbdF`\xa8j\x17\xd8\x0e_\xc1\x9e\xb3yA@\xf6\
+\x84\xae\xaa\xf03\x93\x01E\x14A*\x95\xc8)\x13\x1b\
+\x9b%A3-pQ\x14Oj\xd0k\x1a \x93,\
+j\xa6\xa8\xd9Nu\x8d\xa3\x02\x22\x13\x8e\x13\xb5u\x9e\
+\xe12)\x8b\xe2\xa4\x0b\xc7\x5cA@\xd6L\x92w0\
+\x05\xdc\xeds~G\xf3\xd3n\xb7\xa7\xde\xcf\xe9\xc5B\
+\xe9\x0a\x1e\xf9-\xeb\xf1\x108\xbe\xebC\xe1\x88\xbfA\
+\xb0(\xd0\x04U\xc1\x9a%\x02\xd6Z\xd0\xb4O\xeb\xd9\
+b\xaaD\xb1+\xf5\xb1h\x05\x8b\xcf\xe1\xce'UE\
+!\x18\x5c\xb81\x1c\xc7\xf7PS_g\x07\xe6\xc0j\
+\xe6\xd76~\xcf\x1a\xfb\x1a\xe8z\xb2\xb0\xba\xf1Ut\
+s\xe9\xa2\xf7\xc8J\xf3\xf9\x01/\x17\x0e\x5c\xb2L3\
+N\x8e\xba\xaa\xd0\x10\xbfu1\x9e\xae\xd0@\xfbxX\
+^\x5cKc\xcd\xb4\xb97\x05\xecY\xd0\x15e*\xf3\
+\xe6\xc3\x17\x81\xf1,\x17\xbc\x81\xb438(\x05o^\
+\xafG\xf1@b\xdc0/\xd2\xd0\x12\xe6a\xe1\xc5\xeb\
+y]\x96g\xb1\x85\x5c\xf9\xdd\xc3\x9a\x06\xd2\xcb\xdb@\
+GzV\xe8\xe3\xd7*\xfaT\xa5\x97jo\xf7Q\xb1\
+\x98\xdbinql$`9\x16\x02.\x07\xf26\x0a\
+q\xffN<\xf9\xe89)\xfbn\x16\x16')r\x1b\
+\x89\xdahu\xe8a\xca\x1bh\x84pO\x1d\xf8\xa2,\
+\xa5\x8b\x16DN\xdc\x83\xc6\xae\xee\xbf\xaeaq)e\
+\xcf=~p\x98\xc0M\xfeyt/\x99\xe0?n1\
+\x99\xb2I\xe4\xfb-\xc0\x00\x96\x11\xa6p\xd38\xf1\xe0\
+\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02\x90\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x022IDATx\xda\xa4\
+S\xcfk\x13A\x14~3\xd9\xddd\x93mcC\xda\
+b\x8c\xc5\xe6\xa2m@\x94Y/\xfe\x04\x11)\xd1K\
+\x0f\xb5\xa8\xb9\x07/\xd2\x8bw\xff\x03s\xed\xa1\xb7=\
+\x08\xd2S\xbc\x88G\x0f\x22f[0\xa25\x05\xa1j\
+0X\xab\xb1n\x9a\xec\xef\xbeY\xb6e\xa3X\x0f]\
+\xf8\xf8f\xde\xcc\xfb\xde7;o\x88\xef\xfbp\x98O\
+P\x1f5\x81\x10\x02\x5c\xc8\xf7< \x94\xee\xcf\x95t\
+:\xd8\x84\xf3E\xa4\x17\x8e\xe3h\x8em\x83m\x9a\x01\
+\xac~\x1f\x84\x83\xd4\xfb\xdd.\x88\x89\x04\x1f\xb2\x10\xfc\
+\xd3\xa2{\xe8A\x02\xae\xeb\x82\xd5\xeb\x01\xafZ.\xe5\
+\x18\xf2\x02Z+\x0f\x0a\xf8\xfe\x22\xda\xads\x0e\x22\x91\
+9g\x14\xa9s\xbb\x9d\x8e\x03wK\x13\xcc\xb6\xac\x01\
+\x11\x8a\x01v\xe7F\x81/0\x8b\x9f\x0dy~\xa6\xc0\
+\x92\x12\xbd<w}\x92]=\x97+\x96.\x1cg[\
+[&4\x9b\x06\xcc\xcfL\x06\x22~(B\xa6\x1e\xbe\
+\xe6\x95X\xd4V\x8cR\xaa\xa4\xe2\xf2\x91!YI+\
+\xb2\x92\x92\xa5\x94(\xc4\xc4\xbd\xf5\x5cN\x86\xc7\xb5\x86\
+\x8eyU\xda3\x8c\x0aZT\xf9\x1f-\xcf\x9ef\x9c\
+o\xdd,\x9e\xfd\xbdm\xd8\xd3'G\xf2\xad\xf6\xa6\xf9\
+\xb9\xdd\x16\xd77>\x01\xc7\xc7/-x\xb5\xba\x01\xd7\
+.\xa2k\xd3\x5c \xf9\xfb\xcf\xeaxM*\x0a\xff\xe5\
+\x84\x08X63\x9c\x113\xe9,M\xc4\x93{\xf1\x13\
+\xa324\x9e\xaf\xea\x98W\xa5\x9e\xe7\xa9=\xbc.D\
+\x05\xcf\x168)\xcc^\x09\x9c\x1c-\x9d?\xf3\x8b\x8a\
+\xe0N\xe4\x93?G\xb2\xd0\x1a\xca\x82xl\x0c\xf4\xda\
+K\x1d\xabW\xb1\xa0F\xc6\xef=\x05sg\x87\x0b\x0f\
+8\xc1\xb1\x1ee\xb8=\xc7R1\x80\xae\xf6$\xa8,\
+J\x92&a\x8f\x08\xae\xe3\x00\xba\xe0\x02\xaa\xd5X\x06\
+a|\xbaB\xc7\xa6\xc0\xfb\xf6\x1e8\xf3\xee\xf4\xf0*\
+e\x02\xd0Y\xd2\x82d\xf8\xb1\xae\x19o\x96\xc1\xfe\xfa\
+\x16\xc8\xffz\x9d\x8e\x9e\x02\xe1\xd2\x83z\xd0\x22\xdf?\
+T\xbd\xb5\x9a\xe6\xa2\xf8\xfe[\xf8\xa3+\x15\xc4p\x08\
+\x99\x07\xbd\xcd5p\xda\xef\x9a\xd0\xef\xacx+K<\
+\xb3\x88\xd8\x0eaD\x1d\xf0\xb1\x84\x88\x87\x10\xffa\xca\
+A\x98!,r\xd8\xe7\xbc+\xc0\x00\x0d+.?\xd1\
+\xfb\xb1O\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02\xad\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02OIDATx\xda\xa4\
+\x93Kh\x13Q\x18\x85\xcftf\xd2$\x8ey\xb4\xa4\
+E\x85\xc6\x17)\x8a\x0aUD\x17b\xbaq\xe1\xca\x85\
+\x0b\xadAh\x11\xc4\x9dT,R+\xb8\x11AEp\
+\xe5B\x05W\x0d\xb8p\xd7U\xdd$j\xa0h\x1f\xa1\
+\xc1W\xd3'\xc6&i&\xd1\xc4$\xed$\x99\xb9\xde\
+;iF\x13\xb3\xeb\x85\x8f\xf9\xef\xfc\xe7?\xc3\x1d\xce\
+\xe5\x08!\xd8\xca\xe2\xbc\x03\xef\xc1\xf3\x02\x85\xd7_t\
+u\xed\xae68.@\xf16\x1b\xa2\x1f\x0d>\x1fn\
+\xefe\xb5\xd0\xd8L&\xe3\x90$\x1bDQ|\xd6\xed\
+\x16\xbd#\x03\xae\xff\x0c.\xdf\x8d\x19\xc6-\x8dME\
+Q\x90N\xa7(\xb2\xff\xc3l\xcaw\xf5\xde\x02\xd62\
+\xe5:M>\x9fG\x9d\x01!\xdayUU\x17)\xa4\
+\x86C\xd2\x88d.\x8d.\xac\xc8H\xc8\x1bu\x06\xb9\
+\x5c\xf6\xef\xe6\xf8\x85q\xc6bhF&\x9a\xa6\x19\xcc\
+|\xc9\x90\x13}o\xc8\xf4\xe7\x9f\x84\xad\xc9Oi\xb2\
+\xbaV\xd4k\xaag\x0f\xf6/ \x14\x0aE\xe6\xb3\xe7\
+\xe4\x11'*\x95\x8an\xfam9\x87\x91'a<\xbd\
+s\x14=\x07\x1c\xf8\x18\x91\xd1\x7f;\x84]\x9dV\x8c\
+\xbf8\x83\xcd\x99\xea\x11\x14\xa5\x0c\x06\x1b.\x95JX\
+\x8ee\xf1\xf2u\x14\xf7\xaf\x1f\xc6\xc1\xbdVL\x84\x13\
+\xf0\xdd\x0c\xc0\xe54a\xe9{\xd6\xe7\x1b\x0a\xeaz\xc3\
+\x80\x90\x160\x98A\xe6\xd7:B\xd3I\x5c:\xdb\x09\
+\x97]\xc5T$\x81[\x8f&\xf1p\xd0C5\x1c4\
+\x8d\xf3O\x84e\x1f\xad\x83\x86\x01\xcf\x9b\xc1(\x97U\
+\xac&\x8b\xe8\xf1X\xd1f\x13\x11K*\x18\x1d\xfb\x81\
+\xe1+\xfbph\xbf\x1d\xf1\x94Fu\x16\x96\x10?\xa5\
+\xb7f \x98L\x92^\x94J*\x5c\x8eV*\xe2P\
+\xd8 \x88D\xd7\xd1\x7f\xce\x8d\x8e6\x91\x85\x0a5]\
+\xa5\xc2\xd3\x8f\x15\x8c#\x08f\xb3m3]\x22,\x16\
+\x01\xaaF\xa8A\x19\xa7\x8fu@\xb2\xf2\x86\xb0\xa6\x9b\
+\x0b\xdc\xc0\xef\xd4\x14\x9b\xa8\x1ea\xfe\xed5\xd6\x5c\x0a\
+\xcfi4}f\xb4\x9a,p\xef\xd8\x0e\xa7}\x9b\xbe\
+g\xcc\xce\x13]\xc3\xb4\xd5\xe1\x7f\xee\x02\xa5\xbd\xfb\xd4\
+\xe3\x8b;=}C\xe0xw\xd3\x1bC\xd4\x95x\xf4\
+\xd5\x83\xaf\xef\x06\xc7\xe8\x8e\xa5\xa8@3\xa0\xd6\x0c\xac\
+\x14[\xb3X7,\x16\x12\x85\xc2bY\xa6\x06\x9an\
+\xb0\xd5\xeb\xfcG\x80\x01\x00\xa4`\x22K\x8d\x9am\xcc\
+\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02^\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\x00IDATx\xda\x8c\
+\x93\xbfk\x14A\x1c\xc5\xdf\xcc\xed]\x90\x035E\x10\
+\xe3\x05\x1b\x03b `\xa3\x11\xd2\x04\x85\x83\x83\x98F\
+\xb0\xb0W\xfc\x1b\x84\x10H#\xd8\xca\xa5\x16\x09\xd8X\
+\xda\xa4\x90\x10$\xa9\x22{\xc5%\x84\xfc*.\x9dd\
+\xef\x12oc\xf6\xf6\x97\xef\xbb\xee,\x9b\xe5\x0a\xbf\xf0\
+\x18fv\xbfo\xdegvV\xbdX\x5c\x84Rj\x1e\
+\xc0m\x0c\xaf\xefa\x18\x1eDa\x88r\xa5\x92,x\
+\xed\x1f\x08v\xb7\xb0\xff\xcb\x87\x15E\x91\xac\xdd\xf9\xbc\
+\xb4\xb4\xe2\x05\x01\x06\x9c\xfb|9\x8ac\xd8\xb6\x8dO\
+kko\xf9\x5cQ\xfb\xc6\xd1\xba\xff\x04z\xf2\x11\xc6\
+~nB\x8b3\xa5b6F4\x88\x06\x03\x0c./\
+\xe1\xba.\xfa\xfd>\xbe./\xaf\xf0\xf93\xf6M\x16\
+\xa3\x8d=\xa4Q\xc0&\x8a\x14\x0a%\xaabY8\xea\
+t\xd0\xda\xdbC\xfb\xf8\x18\xef\x9aM<\xa8\xd5\x9ag\
+\xdd\xee\x07\xf6\xbc\xa6\xee\xe5M,1`i\xcdf\xad\
+5\xc0$\xbf\xb9\xfb\xf3\xd9Y\xd4gf2\xa47q\
+\xbc@\xa4\x85\x22\x92\x0e|\x1f\x94\xb4&\x09\x12\x13\xf2\
+\xff/Rf\xa0\xd2f1\x91\x03\xcc#]+\x971\
+\xc2\xd1q\x1c|\x5c]\xc5\xd3\xa9\xa9f\xdb\xb6_\xee\
+\xb4ZD\xa0A\x86@!\xc5\xc8#\x89\x89T\xa3^\
+\x87|\xa9j\xb5\x8ao\xdb\xdb\xbd\xe4\x0c\xfc\xd4@\xa5\
+\x08R\xf2i\x0d\x12\x0a&\xffv\xd3I\xea\xab\x06|\
+9\x89\x9d\x1a\xa8\x5c\x82\xa2\xc9U\x03\xcf\xcb\x12Hl\
+\xb9Vr7\x8aHy\x93R\xa9\x94\x19\xe8\x83\xf5u\
+\xf4\x1cgD&fW^]\x18$\x9d;\x5c3\x8a\
+\x98\x5cKz\xebO\xb7{\xd7999\xbf>=\xfd\
+\xde0\xde\x1a\x1f\x7f\xfc\xaa\xd1\x983Hi\xee,\x89\
+l\xed\x1b\x04\xea\xcc=<\xfc\x92^\x8e\xa4j\x13\x13\
+1's\x06\xa9h\x22\xebD\xd7\xee\xe9ib\xd0K\
+e\xeaf\xdfu\xbd\x0c\x89\x8a\xe5^\xc8\xd9\xc8\x05\x13\
+\x13J\xb0;\x1b\x1b\xa3\xd6\x90\xdf\xf7F\x11iXE\
+\x17\x17\xe7\x1cF\xff\x0a0\x00/\x1c\x22<\xdf\xc8\x0e\
+%\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x024\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xd6IDATx\xda\xc4\
+\x93MK\x1bQ\x14\x86\xdf\xd1\xe8(\x11[\xc16R\
+?\xb0\xd5E\xdc\x09\x03\xd2U\xbbq#\xba\xb2\xeej\
+]\xe8\x1f\xc8\xce\xb5\xbf\xc0\x80+\x11\xa5\xc2\x80\x0bW\
+\x82+Q\x10\xa4\x8b\xd2\x04B\x08\x1aE\x05\x17j\xa3\
+\x94`4\x99\xb93s3=\xe7&~&\xbb,\xbc\
+\xf0\xce\xc7\xc3=\xef9g\xe6\x5c\xcd\xf7}\xd4\xb2\xea\
+P\xe3\x0a\xf0\xe5\xebJ\x06\x9a\xa6-\xd2\xe3\x9e\xe7\xba\
+\xa6+\x04\x9a\x82A\xb5\xe1%wl\x1b\xc2\xb2P\x94\
+\x12\xe9\xb9\xa1\x92\x81\xf4<\xbe\x19J\xa5\x96LQ(\
+ \xd0\xd8X\xc1\xab\xb6\xc0\xce\xac\xa9\xb1N\xc3u\x9c\
+\x08m\x9e\xe4,\xf7\xfc\xc7\xe8#\xafj\xc0e\xb1n\
+n$f\xbe}2\x1c!\x22\xf4q'\xed|^\xf1\
+l\xd6\xc3\xf7\xd1\xde\x07^a\xc0\xd9X\xb6\xed!\x95\
+\xba\xc5\xf4D\xd8\xa0\xc0\x08\x05\xa8JNN\xce\xb1\xb9\
+\x99\xc0\xf0P\xbb\xe2OMJ\x06\xd4\xaf\x92\x90\xb8\xcd\
+\xdb\xd8\xda=\xc5\xf8H\xbf\xe1XV\x84\xf9\x1d\x19\xbb\
+Z\x1db\xc9\x0b|\x1e|\xa78\xb7VQ\xc1_\xcb\
+C<g\xa3{ \x84\x9f\xe6\xef8e\x8b2\xbf\x0c\
+\x04\x91iiC\xf3\xc7Nl\xed\xa4\x15w\x9e\x19\x94\
++HJ\x1d\xfd\xe1\x0e\xac/\xef\xc4)K\x94\xb2\xa8\
+\xbfq\xa6\xbfA\xfd\x87\x10\xfel\xfcR\x9cZ0\x9f\
+\xcd\x01g\xe1\xa5\xb7\xe8\xd8^X\x8b\xd3\xbf\x8fj\xd9\
+c\xb3\xf8\xb6\xaf\xb4Io\xc6\xbf\xd5G\x9eK\xacC\
+\x9c'\x81y\x1f\x1a\x8fr 4\x80\x86/\xb31\xde\
+\x5c\xbc>\x8c\xca\xf4\x86)3\x07\xa8\x7f\x1f\xae\xca\xef\
+\x97\x8aU\x83t\x95\xee\xc2ej\x1f\x22\x97\x90\xb1\xa5\
+\x83\xf2\xf00\x07\xf1#\xe21\xe2l\xd4C\xca\x93\x0a\
+\x5c8\xfb\xaa\x0a\xa8\xb4Vzi(\xab\xda\xf9(\x92\
+x\x5c\xdd'\xf2(\xd6\xd7^\xfd4\xfe\x17`\x00\x91\
+\xb0J\xfa\x7f\xc9\xe7d\x00\x00\x00\x00IEND\xae\
+B`\x82\
+\x00\x00\x02U\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xf7IDATx\xdab\
+\xfc\xff\xff?\x03%\x80\x89\x81B\xc0R]]-\xc8\
+\xc4\xc4\xe4\x0cd\x0b\x03\xf1\xdb\x7f\xff\xfe\xed\xfd\xfb\xf7\
+\xef\xfb{\xf7\xee1\x80\x5c\x07\xc2&\x1a\xd7\xc1\x18\x04\
+fm\x0aa\xf0\xb8v\xcd\xd2\xf1\xda\xb5\xb2\x17\x0c\x0c\
+\x13\x99^\xbf~\xed\xe6\xe7\xe7\x97\xd2\xd8\xd88\x03D\
+\x83\xf8O\x9e<\xc1i#\xd0@\x95K\xbc\xbc\xce\x8a\
+\xf5\xf5\x01\xaf\x19\x18\x1aY\x1e<x \xa1\xa1\xa1\xe1\
+\xfe\xf5\xebW\x06\x10\x0d\xe4o\xe7\xe7\xe7O\x83\xaa\x7f\
+\x0e\xc4\x9b\x11\x9a\x19\xec\xbf}\xfb\xa6\xdb\xb1\x7f\x7f\xb3\
+\xbb\xb2r\x7f\xe4\xff\xff;\x98\x80\x1a\xde\xaf]\xbbv\
+\xdf\xa7O\x9f\x18@4\x88\x0fd\xcf\x02ze\xd6\xef\
+\xdf\xbf%\xff\xfc\xf9\x03v>X\xf3W\x86\xb2\xb5s\
+\xf4'kkk\xd7\x9d\xf9\xf1c\xc1_\x06\x86],\
+/_\xbe\xdc\x96\x93\x93\xc3\x0c\xb4`\x17\x10\xbfbf\
+f\xde\x06\xf4\x06\x83\x85\x85\x05\xd8V+\xbd\xbbp\xcd\
+\xee\xfe\x15^\xf3ft\xec\xd7V`?r\xe8,\xfb\
+%p \x02\x03\xec\x0d\xd0\xa6\xf9\xc8\xfe\x94\x92\x92b\
+\xf8\xf1\xe3\x07\x83\xb4\xc0\xc7}\x16:wP4\x7f\xf9\
+\xf2\xbf\xed\xdf?\x86\xfd\xf0X\xc0\x16P\x8d\xe17\x80\
+\xe4\x0d\x86\x7f\xff\x19\x98\xbe}eD\xd7\xbc\x07%\x1a\
+\xd15\xbb\x18\xfe`x\xff\x19\xc2\xfe\xf9\x9b12\xaf\
+\xec\x86\xd7\xb4.\x0d\xac\x9a\xe1\x06\x80\xe2\x1a\x18h`\
+\x81\x8dG\xfe\x021<\xdc\x1b\xae?\xd2X\xc3/\xc0\
+0I@\x90\xe106\xd72\xa2\x0b\xf0\xf0\xf0\x801\
+\xd8\x05?\x7fJ9\xea\x7f}\xa6*\xff\x9bA@\xf0\
+?\xc3\xde\x13\x0c\x0c{N\x10\x91<\xf9\xf8\xf8\x18\x04\
+\x05\x05A8\x0dD;\x98\xb0\x92\x9e\xc6\xd9\xd9\xd9\x19\
+899\xa5\xd8\xd8\xd8\xf0\xaacF\xf2\x0a;\x10s\
+\x031/\x10\xf3\x03\xc3\x85\x11\x88\x83\x81\xd1|\x0dH\
+s#\xa9\xfd\x8f-\x0c@4\x1b\xd4\x10\x10\xcd\x0a\x15\
+\x03&6\x86?P\xfc\x1b\x8a\xff \x1b\x02\x10`\x00\
+\xc8\x1f\xfcq|\xf3>4\x00\x00\x00\x00IEND\
+\xaeB`\x82\
+\x00\x00\x02\xcf\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02qIDATx\xda\x8c\
+RKh\x13Q\x14=\xf3M'\xb1\x99\xa6\xd2@K\
+\x8b\x0b\xa5\xd2F\xd2\xa9\x11\xeb\x0f*X\xea\xc6.\x8b\
+;]\xb9q\xe7J7EE\xdc\x88\x0bA\xa9\x8a(\
+EA\xec\xc6\x85\x88\x0b\xa1`\x15\xd1\x82\xd0\xd0X\xda\
+\x9a \xf9\xd8T\x13\x9bN\xda4M\x9ad\xc6\xf7\xde\
+d\xec\x14\x8a\xf8\xe02o\xde\xbd\xe7\xbcs\xef;\x5c\
+\xff\xd5\x09\xd4\xd7\x10\x896\xfc{\x91b3\x06\xd3D\
+>1\x83\xf8\xe4S\x88\xe4\xc0N\xb6?\xb9\xd4?\xba\
+Q\xae\xa2f\x18\xa8\xd5L\x18\x06\xc9\x99V>\x9a\xc8\
+\xe0\xc1D\xfc\x22\xd9r\xf4W\xdd\x13D\xcf\xb9\xdb\xe0\
+Y\x81\x15B\xb9RE\xbeX\x82^(!\xb7ZD\
+&\xb7\x8e\xa5\xdf\x05\xa4\xb3kX+\x14\xf1\xfc\xf2\xa9\
+QRw\x9a\x10t\xda\xb7n#\xe08\x0e<\x0f\x88\
+\x22\x0fI\x12 \xcb<\x04\x81\x07=\xcf\xe6t\x8c\xbd\
+\xfc\x80\xc1N\xd7]n=;B\x024\x9c-\x08T\
+\x9cEb2\x12{mn\x02\xc1\xae}\xe4\x0e\x13m\
+-\x8dx\xbb\xb01m\xe7D\x98\xc6\xdf=\xc1\x120\
+Gz\xc7\x8e$\xb5Z\xbd\xd64D\x07\x81\xb9E@\
+$\xac\xfcJcue\x19\x1e\xb5\x19>\x7f+#\xd1\
+3i\xe4s\xcb\x90\x15\x15 \x0a\x08Ft\xcc\xc0@\
+=$\xaa \x1e\xfb\x863\xc7CHD\xe71\xf3\xf9\
+=\x22S\x93H}_\xc0\xf0@\x1f\x96R1\xa6\x90\
+\xd6\xda8'\x81Hg\xe0\xf1\xaa\xb8\xf5p\x0cn\xb5\
+\x09\x95J\x05\xda\xb1\x93PT\x1fn\xde{\xcc\xce\x04\
+\x81\xb3j\xeb8\xe7\x0c$\xda\xc2\x81\xd0!t\xf7\x86\
+\xd8\xc0\xde\xbdy\xc5n\x0ch!t\xf7\x1cd\xb3\xa1\
+\xaf\xc2\x14\xec0D\xc9z\x85\xadA\x96K%\xf6*\
+\xc9\xe8\x1c~.&\xd1\xd2\xda\x81\xa0\xa6m#p\xfa\
+@\xa2\x16\xa3\x00\x9b\xc4\xebk\xc6\xeb\xf1g\xf8\x1a\xfe\
+\x82\x0b\xc3C\x88\xcdGX\x8e\xd6\xda81\x9f\x8c@\
+\xed\x08\xd4\x15X`\xcb\xad&N\x0c\x0c2;OO\
+}\xc2\xf5;\xf7\xb1w\x7f\x00\xb4M[A>5\x0b\
+1\xfc\xe2\x1a\xb4\xb3#hj\xef\xf2\xd8\x0a,sY\
+_\xaa\xa4\xb7\xef(\xb4\xc3GX[4\xcd\x19\x15\x8f\
+\xfec\x0e\xe1\xf1\x1b\xa0NQ\xc8\xc6\x8fji\xb7H\
+|\xac\x88\x12\x14I\x86[\x92\xe0\x96exH\xecj\
+\x90\xd1\xd8\xe0\x82Wq\xc1%\x11\x0b\x90Z\x86!X\
+j\x08\x85\x84_O\xcef\xce_y\xf4\x11\xff\xb1\xf4\
+\xc5h\x86bHT\xff\x080\x00\x0e`\x13:{\x17\
+\xe5\xcd\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x01\xb2\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01TIDATx\xda\xa4\
+\x93\xbfJ\xc3P\x14\xc6On\x12\xa1\x18D\xc7*\x1d\
+\x04\xb5\x94\x98*\xe8\x22.\x8e.\x8e\x82\x9b\xb3Oa\
+^B\x9c]]}\x017\x05\x8bC\x08\x04qP\x17\
+\x87:\xd8\xda\x12\x13s\xcf\x8d\xf7\x9c\x06]\x22i\xed\
+\x85\xc3\xfd\x86\xdfw8\xdf\xfdc\xe4y\x0e\xd3,\x01\
+S.\xe3\xf4\xd0=\xd0\xfb\xe2?\xbc\xaf\xfeexe\
+)\x95/\xf9\x17\xd7\xe7\xa8\xb2\xb1\x9d\xa6\xb0\xc1?\xde\
+;!m\xa1RB\xca\x14\x9e\x1e\x22\x18~\xf4`}\
+{\x07\xc2\xce\x0d\x83e\xda\x99\x9b\x87\xe5f\x0b\xc87\
+j\x80\xcaT\x880\xe8\xbf\xc3j\xbb\x0dI:\x84\x15\
+\xcfcS\x99~\x0c\x02 \x9e|\xdc@\xa2\x12\x88\x12\
+Z\x9b[\x90|}V\x8eO\x1c\xf1\xe4\xe3[\xd0\xc2\
+D)!\xb8\xbb\x05\xa9\xf7\xaa\x22\x8ex\xf9;\x01\x9a\
+RwD=\x16\x01U\x8b9\x9e\x00\x8b\x06\x12y\x82\
+\xa6\xb7\x01qZ\x1d\x818\x9e@\x8e\x1a\x88\x8c\x22\xe8\
+\x8e\xe1}g\xac\x08\xc4\x11\x9f\x15\x11\xf4\x15\xa2E\xa7\
+:\xeb8\xf0\x1cEP\xb3m\xde\xff\xd2\xc4)\x8e\x8b\
+\x16G\x18\xc4I\xcd\x12\x06\xd4\x1b\x0d\xa8\x17\x19\xd7\x5c\
+\xf7'o\x99&\x9e|\xac_\xde\xe2\xee\xd1\xfe\xee\xd9\
+\xa4\xef\xb8\x9f@\x97\xff\x82\xae\x19]\x0b\xf4B'\xf0\
+\xa3\xae\x9e\xfe\xc9\xa91\xedw\xfe\x16`\x00s\x8d\x0e\
+G\x22\xb7Z`\x00\x00\x00\x00IEND\xaeB`\
+\x82\
+\x00\x00\x02\x82\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02$IDATx\xda\x84\
+S\xcfk\x13Q\x10\xfe6\xbb\x89Y\xd2\x92\xdaT\x22\
+\x0dUk{\x11\xc9A\x16\xf4*\x1e<\xe9\xc9\x83G\
+E\x90\x82\xf8'\xe4f\xff\x06A*\x82`z\x10\xb5\
+\x18\x85\x06\xaah\x8f1\xd9\x80H+Z\x11\x0bZ\x12\
+06\xddd\xb3\xbfw\x9d\x09\xd944\xa9~0\xbc\
+7\xf3\xcd|;\xef\xbdY!\x08\x020.>\xaa#\
+\x84 \x08\x0fhQ\xb0\x0f\x95\xf2\x16B\xe7\xfd\xadt\
+\x9f\x90\xc2\x8d\xa9\xeb\x88\xc5\xe3\xa1\xab\x5c\xbf<\xad8\
+N\x00I\x12\xf0tm\xa7_`\x9b&\x06\xd1\x17\xb0\
+\x0c\x03\x9e\xeb\x22\xda\x13\xe9t<h\x9a\x87\xf1q\x11\
+.\xc5\x19\x0e\x15\xbb\x8e3Z\x80\xc1\x02~\xa7\x83\x88\
+$\xc10\x5c\xb4Z\x0eD1\x0a\xc7\xb6\xe1\x13\x17\xf8\
+>\x0e\xa2/@g\xec\x9e;\xf0<\xf8d\x96\xe5\xc1\
+4]Z\x05\xb8\x96\xc5)\x95^\x9eJ\xcb\xc2\x90\x00\
+\xb5\xb6B\xa4r\xe3ZV\xd9\xdd\xb5\xd1l\x1ad-\
+2\x07\xd9SqebB\xc6\xdbRM\xa5\x0b^\x19\
+\xec 2\xd0A\x91\xbe\x94{\x98/\xd3\x8d[\xd8\xda\
+\xdaF\xa3\xd1 \xd3 \xcbQ\x14\xd7\x7f\xa8\xccs\xde\
+H\x81P\xc4\xb6\xcc\xdc\xf2\x8b\xaazrv\x0a\x81 \
+ 33\x89\xd5w_U\x8e\x1f,\x1e\x12`\xf8\xbe\
+_\xd4\x9b{\xb9g\xcfK\xea\xd1L\x0a/\x0b\x15\x95\
+}\x8ec\x04\xa4QAN6\xdam\x14\xf2o\x16\x85\
+H$'\x8f\x8d\x8d,\xee\x0e]8\x89\xd3wW\xf7\
+\xdb\x12\xc5\xee\xd3\xd94\x1b1YF4\x16\xeb\xbe\x0c\
+\xa3]\xceC+=9\xfc\x08\xbd\xbb\xc8P\xd1R\x22\
+\x99\xac\xf0\xca\xfe\x7f;\xa0\xe7A\xf2\xca\x22\xa2\xc7\xcf\
+\xb2\xbbt\xe1R\xf6\xaa8\x7f:\xad\x7f\xf9^\xff\xb8\
+\xfe\xe9\x15\xc5n;\xb5\x0d\xec\xbd\xce!\xac\x19\xea\x80\
+Ic\xbb\xcac}N\x9b\x9dK\x17j\x02vf\xe6\
+\xd2\xecs\x9c\xf9\x7f\xbd\x02\xefe}\xed^\xcai7\
+7~\x957\xeb\xc7\x8e\x00\xbf\xab\x9bu\xf6)>E\
+|\x82L<\xec\x08L$\xc9R\xc2\xe4\xfc\x89\xc8\xf9\
+;7\x11K\x9c\x81\xad\x7f\xf6?\xdc\x7f\x1c\xfc\xf9\xf6\
+\x93\xb8\x06Y\x93j\xfa\x7f\xd4_\x01\x06\x00zl0\
+\x8b\x82\xa5\xcd\x98\x00\x00\x00\x00IEND\xaeB`\
+\x82\
+\x00\x00\x01\xb3\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01UIDATx\xda\xc4\
+S\xb1n\x830\x10=G\x05\x85\x94f\x02\x86\x8c]\
+\xbaD]\xdb\xff`\xce\xce\xc6\xdc\x091u\xc9\xc2\x10\
+e\xc8\xc4?\xe4#\xe8\xdcJ\x1d*!\xb1\xa1\x0c!\
+\xb4@\x22B\x94\xfaYe !j%\x86\x9etz\
+w\xf6\xbbw6\x9c\xd9\xf1x\xa4.\xd6\xa3\x8e\xd6Y\
+\xe0\xaa\x0e\x1c\xc7!\xc6\xd8-\x0f\x1f\xb8\xdf\x5c\xe0\x7f\
+q\x7f\xe1\xd7\x0e]\xd7m\x0aTU\x05x\xb4m\xfb\
+\xc90\x8cq[\xf5j\xb5z\xf3<\xef\x99\x87\xe1\xd9\
+\x09\xca\xb2\x04\x0c5M\x1b\xff\x885,\x8ec\x1a\x8d\
+Fc\xce\x1b\xb6~\x83\xddn\x07g(>\xf5\xcdf\
+C\xcb\xe5R\xc4\xe0\x80{Q\xe0p8\xd0l6\xa3\
+\xf5zM\xfb\xfd^\xa0\xef\xfb\x94\xe79a\xef7\x81\
+\x1e\x8a\xd0q>\x9fS\x18\x86\x02\x91\x9b\xa6)\x04\xc1\
+i\x15(\x8a\x02.N0\x99L(I\x12Z,\x16\
+\x02\x91+\x8a\x22N\x00\x0e\xb8g\x02\xdb\xed\x16.\x04\
+\x06\x83\x01Y\x96Ei\x9a\x0aD\x8e\xee\xd8\x03\x07\xdc\
+3\x81 \x08\xd0-\x8b\xa2\xe8]\x96e\xd2u\x9d\xa6\
+\xd3\xa9@I\x92\x08k\xd8\x03\x07\xdc\xdaX\xfd\x16\xf8\
+\x10\xe9\xaa\xaa\xde\xf7\xfb\xfd;\x1e_\xb7\xcd\x01\xe7\xe6\
+\xfc\xfe\x1fY\x96\xbd\xf28>\x15@\x11\xfe1\xfb\xc3\
+\x04\x7f\xf2\xba\xac!\xf0o\x8f\xe9[\x80\x01\x00i/\
+\xeea\x09o\xb4\xd2\x00\x00\x00\x00IEND\xaeB\
+`\x82\
+\x00\x00\x02\xe4\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\x86IDATx\xdal\
+S\xcdk\x13A\x14\x7f\xbb\xb3\xbbiMT\x92\xfa\x11\
+\xbd\x08\x05k\xacz\x9a\x9c*m\xf0\x10Y/\xc6\xa0\
+\xe0A\xbc\x14\xb5\x87\x9e\x83\x97\x1cs\x08\xf8\x17\xb4\x0a\
+\x0a\x11\x0f\x8a\x94\x5ct\xc1\x83\x89\xa0($\x07\xb1-\
+\x85b\xc1\x8b\x1fmMIbLwg?|o\xcd\
+\xb6\xd1f\xe0\xed\xec\xfb\xbdy\xbf\x99\xf7\xe67\xd2\xa1\
+\xd4m\x90\x19\x03\xa608\x91\xc9\x81$I\xa0\xa8*\
+0\xc6t\x00(\xa0\xe5\x1d\xc71l!\xc0\xf3<\xf8\
+R\xbe\x07\x8e\xed\x80\xeb8\xb0Q\x99\x07e$u\x0b\
+TM\x035\x14\x82\xbe\xa1cR\xe1\xea\x85c\xfc\xf9\
+\xebo\x85\x1ef\xd0'\x9e\x9e\x05a\x9a ,\xcb\x07\
+e\xd8;t\xdc\xadpe*\xce\xdbm\x17h&\x9f\
+\xf0\x01kA\xe9w\xda\xcd&\xac7\x1aY\xfa/\xae\
+\xad\xd5s\xd3\x93\xbcx\xffM\xbd\x17\xce\x1e\x89\xc5\x0c\
+\x0d\xcb\x1bH\x80\xf5\xe9\xaa\xa2d\xf7\x87\xc33\xedN\
+\x87\xa0\x9a\x10^\x10N\x22\x0e\x18\x9f\xc3u\x0bA9\
+\xbb\x04\x98l[\x96_\xeb\x90,\x83<<\x0c\xcdn\
+\x17\x84p\xfc\xf0A\xf45\xc4q\x0dG\x97\xe3\xfa\x9d\
+\x9e\xc8\xb4\xb3\xc0\x1a\xb3\xe9\x04\xa7\xc6`\xf3jL\x92\
+jC\x8a\x02\x9b\x8d&\xd0L>\xe1\x14\xbfx\xfe8\
+\xa7\xf5\x94G\x04\xd2\xe8\xddj\xed\xfa\xe5$o4,\
+\x88FU0\xf1\x8a~\xfe\xfa\x0d\xa6\xb0\xa1\xd9\xda\x86\
+HX\xf3\xaf\x8f6u\xf1\xb3\xbe\xd9\x81S\xa31\xa8\
+VV\xeb\x9f\x8bSIE\x98V\xbe\xf4\xf4m\xe1\xc6\
+\xb5\x09\xfe\xf8\xd9\xbbz\x7f\x83\xce\xa5\xce\xf2\xf7\xd5\xc5\
+\x7f\xb0\xb1\x89\xd3\xfc\x95\xb1XG\xbd\xe4\xfd\x1e \xbb\
+/\x92GO*~\x0fP@I\x9a\xe9\xc8-\xa6\xf9\
+\xf7\xdd\x8f-U>\xfa\xc9(6c\xa7\x89>\xc9_\
+ad\xb7\x91\x8c\xd4H\xeal\xca!_4&\xaa\x8e\
+\xca\xc0$:\xcd\x82\xa2i\xbb\xb7\xd0\xfaP\x02vt\
+\x1c\xa4\x911\xc3\x11\xc2p]w\x0e\x198\xee\x06-\
+\x16\x0a\x14WC\x86\xba\xedy3\x0cu`}\xfd\x04\
+\xdd\x1f\xcb\x08\xa7A\x0a\x98\xd4\xf8\x19`\xe3\x19\x90\x0f\
+'t\xdc\xad\xb0o\xfa&\xdf\xc2\xdc\x03\xa8\x1b\xf3a\
+\xc9?\xb6\xbb\xb1b8\xcbe\x10\xdf\x97\x02\xed\xec\x95\
+&\x12\x802\x99\xd3\xd5\xec\x83Z\xe4\x85\xe7\xd1L>\
+\xe1\xff\x0f\x22\xa0\x130\xb4\x08Z\x944\x13\xf4EN\
+d8\x9c\xbct\x07V_\xce\xbb+\xe5\xe0&l\xb4\
+\x16\xda\x16)\x1f\x09\x1c\xa9\xf7\xa04\x12a\xcf\x06=\
+\xb0`\xb8h&Z\x17\xcdB\x02\xf7\x8f\x00\x03\x00s\
+\x0b@\xa4\x95\xffZ\x8d\x00\x00\x00\x00IEND\xae\
+B`\x82\
+\x00\x00\x024\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xd6IDATx\xda\x8c\
+\x93\xbdN\x02A\x10\xc7\xe7\x96#\xc6\x0f\x0a\x0b4~\
+\x956\x0a\x15\x0d\x85\x15\xb6\xda\x99\xe8\x03X\x18+_\
+@H\x88\x85\xb51\xd1RI\xe8|\x01\x831!\xb1\
+\x14r6PH\xac\x0c`\x83\x22\x90;\xbd\xbb]g\
+\x96[\xef<\x89q\x92\xb9\xbd\xdb\xd9\xf9\xcd\x7fv\xf7\
+\xb4\xadl\x16\xc84M\xdb\xc4a\x0e\xfe\xb6[\xcey\
+\x83\xbb.\x08!\x80?\xdf\x81N/d8\xce\x17r\
+\xb9\xf3O\x0c\xda\xe4\x9c\x83\x8b1\x157\x0c\x03\x0a\xa5\
+\xd2\x1e\xd5B\x7f\xa49\xb6\xb8\x06\x8ch\x9ek\x9c\x92\
+l[\xfa\xa7e\x819\x18@\xbf\xdf\x87^\xaf'\xc7\
+\xab|\xfe\x1c\xd7\xadc\xee\xb2\x92\xa4\xbb\x98\xec\x99F\
+h\x86\xcfh$\xe2\x8bv\x1cp\x10\xdc\xe9t\xe0\xb4\
+X\x84\xcc\xca\xca\xd9I\xb1x\x88\x91#\x09\xe0>\x80\
+Q2\x93\x18\xf8\x05\xc9d2\xb2\x9dX,\x06\xd7\x86\
+\xf1\xfa\xad\xc0\x09*\x08\x00FAH\x89|\xc5v\xfd\
+\x160\x10n!ha\x08\x15\xc1\x9c\x91\x80a\x0b\x8c\
+\x01x\x95FA\x22C\x00\xf3[\x08\x00\xbe\x15\xfc\x01\
+\x89\xe0\xe8\x04\x00\x8c\x00\x9e\xcb=P\xfb@J\xd4\xa6\
+*'H\x14\xe7i-\xe5\xa4\xee\xef\xb1\x05<\xf3\xb0\
+\x02\xaa\xcd\x86M\xfdR\x22[\xb0m\xb6}s\x03s\
+\xedv\xa8\x05R\x80G\x15\x86<\xec\xefC\xb7RQ\
+G\x05\xbb\xf5\xfa\xc1\x94i\xee\xe0\x1d\xad\xe8\xddV\x0b\
+&\xe3\xf1\x1f\xa7\xc0C\x90f\xb5\x0a\x1b\xc9\xa4/#\
+\x91X\xc0\xe7\xc2e\xa1\x00z\xa3\x5c\x86\xa5t\x1a\xc6\
+\xa7\xa7uU\x81\x92\x82\x90\xb1T\x0a.\x94\x02\xf4\xa7\
+Z\xad9aY-L\x90\x93\xe3\xe83\xb3\xe9t^\
+\x04\x0c\x01\xc2\xe5\x5c\xe0\xe5\x11\xf8s\x09\xfc\xc9\x84\xe5\
+8\xe2\x03\xbfi-\xe5P\xae\xae\x00\xef//oS\
+\xab\xab\xc7\xf0\x0f\xe3\xa6\xf9\xe6\x01\x9c/\x01\x06\x00\xc2\
+5\x11x\xfc\xd3\x22\xfc\x00\x00\x00\x00IEND\xae\
+B`\x82\
+\x00\x00\x05\xff\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x03iiTXtXML\
+:com.adobe.xmp\x00\x00\
+\x00\x00\x00<?xpacket beg\
+in=\x22\xef\xbb\xbf\x22 id=\x22W5M\
+0MpCehiHzreSzNTc\
+zkc9d\x22?> <x:xmpm\
+eta xmlns:x=\x22ado\
+be:ns:meta/\x22 x:x\
+mptk=\x22Adobe XMP \
+Core 5.0-c060 61\
+.134777, 2010/02\
+/12-17:32:00    \
+    \x22> <rdf:RDF \
+xmlns:rdf=\x22http:\
+//www.w3.org/199\
+9/02/22-rdf-synt\
+ax-ns#\x22> <rdf:De\
+scription rdf:ab\
+out=\x22\x22 xmlns:xmp\
+Rights=\x22http://n\
+s.adobe.com/xap/\
+1.0/rights/\x22 xml\
+ns:xmpMM=\x22http:/\
+/ns.adobe.com/xa\
+p/1.0/mm/\x22 xmlns\
+:stRef=\x22http://n\
+s.adobe.com/xap/\
+1.0/sType/Resour\
+ceRef#\x22 xmlns:xm\
+p=\x22http://ns.ado\
+be.com/xap/1.0/\x22\
+ xmpRights:Marke\
+d=\x22False\x22 xmpMM:\
+DocumentID=\x22xmp.\
+did:C43B52F403BD\
+11E18A2098D75C57\
+074B\x22 xmpMM:Inst\
+anceID=\x22xmp.iid:\
+C43B52F303BD11E1\
+8A2098D75C57074B\
+\x22 xmp:CreatorToo\
+l=\x22Adobe Photosh\
+op CS3 Windows\x22>\
+ <xmpMM:DerivedF\
+rom stRef:instan\
+ceID=\x22uuid:AC1F2\
+E83324ADF11AAB8C\
+5390D85B5B3\x22 stR\
+ef:documentID=\x22u\
+uid:C9D349664A3C\
+DD11B08ABBBCFF17\
+2156\x22/> </rdf:De\
+scription> </rdf\
+:RDF> </x:xmpmet\
+a> <?xpacket end\
+=\x22r\x22?>\xb8B\xe1S\x00\x00\x02,ID\
+ATx\xda\xa4\x93\xcfk\x13A\x14\xc7\xbf3\x99\xdd\
+nL\xb6\xdaT\xa8D,x\x11\x95\x8a\xa0D/j\
+\xd4ZA\xfa\x07x\xc8\xa1x\x11\x05A\x0f=x\xd5\
+\x83\x17O\xe2MAQ\x10\xd4\x8b\x82\x82PP\x1b*\
+\x8a\x04\x05\xad?\x0aE\x03\xb1\x86\xa61\xc44M7\
+\xd9\x1f\x19\xdf4\x9b\x98\xc4K\xc0\x81/\xbcy3\xef\
+\xbd\xcf{;\xcb\xa4\x94\xf8\x9f%\x12\x079v\x0d3\
+\x8c\x0c7\x1c\x01\xce`\xe8\xd8\xcb\x808m\x87\xfc{\
+9*\x93\xac\xdax\xe7\xd5\x1b\x05?e\x80\xd9\x8c\x04\
+{r\x91wd\xe4\x8c\xc5\xcc\xc1\xe8\xe9\x1dGN\x1d\
+\xcf.\xfe\x0a*_t\xd3F\xeb\xeb\xcb\xdbS\xe5B\
+\xf6F]\xcaT\x07\x81ewC\xc9\xb1=\x07&\xc6\
+\xdf<\x9f*~\xf9\xf0\xf6\xb1\xf2\xec\xdc\xbd\xffX\xec\
+\xd0\xc4\xf8\xcc\xc3+i\xdav$\xe0\xba`h\xaal\
+Ai\x8bd\xc6Pf\xfe\xfd\x82.p^I\xd9\xca\
+\xa7\xce\xd4\x1d\x11`\xd0|\x89\x0d!\xbf.\x891\x86\
+t\xae\x1e\xae\x94\x969\xa4S\x0bS\x03\x85e@\xd7\
+\x9c\x9aU^\xe1eK\x86\xa3\x11\x063\xa8Z\xf5[\
+h\xa39\x1b\xd4\xb1m\xb5&\xb5\xd2\xef\x22\x04\x87C\
+\x97\x1e\xb8\x9e\xdc*8\xfb1\xf7y\x16\xea\x8cHo\
+\xd2\xdd\x8f\xa4\xeb*\x88M_\x0a4\x09\xae\x1e>s\
+w\xd2Y\xb5`W\xab\xb0-R\xcdB\xb10\x8f>\
+\x1dXg4\x14\x0c\x0bL\xdf\xbfs\x8d\x92_\xe8&\
+@*\x99\xa4\xca\x1cB\x08j\x87\xc3\xf3\x5c\x14\x8b\x16\
+\x02T\xc3\xd0(\x98\x12\x85L\xad\xf3\x1d\xb4ob\xf1\
+8\xba\x09\xfa\xf4\x95\x7f\x08\xbe\xbdnK\xe0\xb8\xad!\
+\xca^\x09(F\xb6\x86\xb8\x90k=eo\xec\x5co\
+\x04/\xf2\xd2aM\x82\xcb\x8f$\x12\xfb\xd6l\xbdW\
+\x82\xf4O\xa9\xa9\x04\xf7\xe8I\x89t^\xe2\xd6+\x86\
+\x13\xdb1\x18\x1b\x1d\x85g;p\x89\xc0%\x02\x97\x08\
+\xfa\xfb]\xe8\x14h\x18\x7f\xb5X\xc0\xc0\xb39 [\
+\x92kC\x8c\x90\x11\xfd\xbe\x04\x9e8z\xf2)a\xe6\
+#\xebY%2\x00\x1e\x0e\xc1\x9cI\xc9\xcd\xfe;C\
+\x13{\xa9\x02+[\xc2\x08\x99Y\xe5S?\x8c\xd9\xfd\
+EzXj\xfc\xe5?\x02\x0c\x00R\x16\xfb\xb0J\x9c\
++Z\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x01\xc2\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01dIDATx\xda\xec\
+\x921H\x02a\x14\xc7\xff\xdf\xdd\x99\xa9tZY\x12\
+\xb9h\x18\xba\xa65\x97en5\xb584T\xd4\xda\
+\xde\xe2\xd2\xdc\x185\xd6|4\x06J.\x82-\x15\xb5\
+\x18$\x98\x88&I\x91(\x97\xdd\xe9\xdd\xf5\x8e\x14\xda\
+\xdd\xa2\x07?\xde\xe3{\xef\xfb\xf3\xbd\xf7>f\x18\x06\
+\x061\x0e\x03\xda\x1f\x10\x10\xd8\xb9\x1bh\xeb\xc0\x08\x0f\
+0\xe6\x03\xc3!\x9d\xcf\x12O0p\x00\xc3x\xde\xb8\
+X\x82\xdf\xef\x07\xcf\xf3\xa3\x1c\xc7-Sn\x9cx\xd7\
+u\xfd\x8a\xc7\x9a\xfd\x06\x9aqK\xc55h8^\x08\
+E\xa2\xab\xe1\x95\xc0\x10g\x99\xac\xbeTg\x16\xaf\xe7\
+$\xc7\xe70dYF\xa7\xd3YO$\x12\xdb\xc4\xbe\
+(\x8a\xcel6\xdb\x12\xd0\xea\xd6H\xed\x04\x0a\x22\xe4\
+\x03\xcei\xd1SQ+0=r\xdd\xc0\xc4\x9bk\xd7\
+|\xaa\xaa\xaa\xa8\xd7\xeb\xb6`0\x187\xc5L_*\
+\x95.\x054\xb5)T\xf4=\xa4\x14`\xcbV\xb8\x7f\
+\xb8\xf3\x8a!\x97\xa7\xf9\xd8x\xa5\x5c!\x9f\xcf\x9f\xf6\
+\xfb%\x91MI\x922\xb1X,\x9aN\xa73$\xf0\
+\xc1\x90t\x00g_@Qs\xc3\xcb\x85\x11\xe7w \
+\xc0G\xed\x14\x91\xd2\x8eP\xd6\xcb\xbd\xfb\x16A\x10\xc6\
+\xacV\xeb<\xc5.\xa2\xa1(J\xeeG )\x9b\x05\
+vB$\x18ASE\x97\xd0zq\x7fc\xbc9\xf8\
+_\xdbk\xb3\xff\xaf<\xb8\xc0\xb7\x00\x03\x00\x88\xe2\x83\
+\xb2\xf3\x16\xdd/\x00\x00\x00\x00IEND\xaeB`\
+\x82\
+\x00\x00\x02,\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xceIDATx\xda\xa4\
+S\xbdN\xc30\x10>\xc7&IK\x08\x08\x10P~\
+\xfa\x08\x0cL\x80\x84\x08\x1b\x12\x03\x8f\xc0\xc4;\xf0\x06\
+\xbc\x02\xe2\x01\x10\x8c\x0c\xec\xed\x02\x0bbCH\x88\xa1\
+\xeaP\x84D)\xfdI\x9bF6\xe6\xce\x90\xd2\x92V\
+\x0c\x9ct\xb2}\xf7}\xdf\xf9\xce2;<\xaej@\
+c\x8c\x15\xa5\x94\x01:DQ\x07~\x9b\xebf@\x08\
+A^\xd0ZoS\xec\xf4h\x9a\x89n72\xe48\
+\xee\x06J}\xc0(KD9\xb7\x02\xdbvz\x22\xa2\
+\xd3\xe9\x14Q\x00\xc9\xb2\x80+\x05\x19\xba\xfe\xe6\xa5\xf6\
+\x88+b\xa1\x00\x05\x0aF@\xeb\x8f\xa0\xd9l\xd1~\
+\xdb\xb6m\xc69O\xc0\xd0G4\xa6\x94bq\x1c\x1b\
+A\xcf\xf3\x02#@W\x0bC#\xc0\xa2\x88\x03\x09\xf8\
+\xfed\xaa\x85F\xa3N\x02F\xc4\x10\x85)\x04\xa2R\
+\xa9$\x18\x9dT\xc3\x1eqhn_\xff\x11\xd4j\xb5\
+\x01\x5c\x18\x86\xb8\xac\xd2\x0c\xa2T\xb5R\xa9\x04\xf9|\
+\x1e\xb2\xd9,\xb4\xdbm(\x97\xcb#\x87+\xa4T\xa9\
+^\xc9\xaa\xd5&H\xe9@\xbdN\xab\x82a31\x02\
+\xea'\xa7\xfb\x93R\xbaHVfU\x03\xfcA\x9c\xb0\
+,;u-\xcf\x9b\xc7!}\xcd@\x88\x0c\x0eu\x05\
+Z\xad\x97\xa1-X\xbe\xbf\x08q\xe3\x11\xc6\xc6\xc6\x99\
+\xe3\xf801\xb1\xd0#\xf7\xaa\xe0\x99\xe2\x94'\x1c\xe1\
+\x89g\x04(\xf9\xf6t\x86\x93\x1f\xd7\xae\xeb\xe33:\
+C+Q\x9c\xf2\x84#|R\xc4b\xcc*\xb4^\xef\
+f\xbb\xf5\x87[\xcem]\xb9?\x01\xcb\xe2\x9a\xfc\xf7\
+\x9e\xf2\x84C\xfc\x1c\xf1\x8c\xc2\xd6AI\xaf\xee^\x5c\
+O\xe56\x17\xf0\xb8\xf8\x97#.\x87\xf8\x1b\xe2\xa1\xd1\
+\xe7\xca\xc0\xccR\xb01\xbb\xbcs\xfe\xfe|\x13\xdc]\
+\xed\x8f|\xf3\xb5\xbdK\x98\xcam\xd0GZ\xef\xbd)\
+\xa9\xfc\xc7>\x05\x18\x00i\x93\xd4\x80\xf4\xde:\xf1\x00\
+\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02\xbf\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02aIDATx\xda\xa4\
+S_HSa\x14?\xdf\xbdw\x11\xdb\x8a\x1e\xf2A\
+\x1f\x12E\x0bt\x19q{\xc9\x06\x15\x85\xba\x06Np\
+\xeem\x0f\x85\x12\xe6\x83\xb1\x9e\x0a!f\xf5`O\xb6\
+7\xb9A L\xa5E\xbd4\xbb\x82+$G/[\
+\x7f@\xf6\xb0\xb0\x1eb#\xc9tk\xb3\xb6\xb9\xfb}\
+\x9d\xefn\xd6&\xad\x1e:\xf0\xe3|\xf7|\xe7w\xfe\
+}\xe7\x12\xc6\x18\xfc\x8f\x90\x9dC'!\xe0A}\xf2\
+\xcf~V\xc4\xa8\x06\xe0\xdb\x04x\xf9\x19?>a\xe2\
+\x02j\x81\x13\x1f!\x02\xb5\xc9\x5cF\x1bfg\x9dy\
+\x80kX\xef\xe9\xca\x0b\xe1\x1fD](\xfaA\x22\x01\
+M>\x9f\xe3\x07\xc0u\x0cr\xeeW\x80Z\xa4\x8a\xc9\
+X\xb7\xd1\xaf\x90\xc9@bq\x11\xea\xfa\xfb\xbb\xd3\x8c\
+y\xf1\xbe\xfb\xaf\x01*{oR\x94\xbe\xcc\xea*d\
+\xb3Y\xd8\x9b\xcbA\x97\xcbu\x0a\x83\xde\xe1I\xa4]\
+\x04/\xa2\xad\x5c\x81\x80\xe5\x8a-\x8a\xe2\xf8\xba\xb4\x04\
+9M\x83\xb7\xa1\xd0+n\xc3\xe1\x89x?\xc6\xfd\xa4\
+x\xf53\xda\xcf\xcc\xcd\xc9\x90L\x82\x86\x99\xbe\xa7R\
+\xb0C\x0e\xce\xccD\x8a\x00\xe3\x98Q\xadd\x90Pu\
+\xdf=\xe8t\xbbKQ\xe4T8\x0c\x1bkk\x90\xa7\
+\x14V\x16\x16\xc2\xebh\xbfw\xf3\x80\x1ao7\xe8\x8e\
+\xf6\xc0\x16\xc06\x03i\xba:\x80\x8ao]\x9f\x1f\x1a\
+\x1a\xe9\xf4x\xe4o\xb1\x18\x18M&\xc8\x00\x18\xe6\x9d\
+F5\xdef\x98B'\x19]\xa3A\xa7\xf12lQ\
+\x0c@\xc8\xef\x00\x8c\xedC\xb5gxyY\x0eY\xad\
+\xd1\x13v\xbbl\x96$\xbe0\xe2\xfbV\x89g\x94\x07\
+/\x5c\x94\xef\xcf?\x00\xd0J\x8dT\x0eQ$\x84\xf4\
+\xc4b\xb1I\x8b\xc52\xd6'\x08\x1b\xb9`\x10z\x07\
+\x06\xe4\xe9K\xa6\xc6x\x8b\x14\xc1~ \xad\xa5\x81k\
+\x94\x08V\x13E\x0e\x01R\xaa\xe2\xac\xdf\xef\xbf\xebv\
+\xbb\x15<\x07z)\xdd\xb4S\xaa\xcf\xe4\xc6\xad\xfd\x8d\
+\x1d\x83\xe7\x0f\xee~\xe3\x17\x8f\x9fGu\xa6(\x8aG\
+m6\xdbUUU\x9fPJ\x9f!4n?\x82h\
+E<\xbdb\x9a\x82f\x91\xf7\x0e\x16\xd71y\xe5\xe1\
+\xbb\xa8\x1e\xe1\x83\xa6\xebC\x92$M\x08\x82\xe0\xc0\xf3\
+qDGy\x17\x0e#\x9a\xf9=\xa2\x1eQ\x07^\xf3\
+\x9b\x86\x8f\xed\x0c\xc6\xcd\xaf\xf1\xdb\xc0\x17\x91\xcf ]\
+,\x16'\xcb\x7f&+\xad~\x0d|)D\x92\x13q\
+\x06\x06\x12)\xdb\xd8O\x01\x06\x00\x8b \xf5\xb9Xl\
+\x045\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x020\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xd2IDATx\xda\xa4\
+\x931H\x1cA\x14\x86\xff\xd9\x9d[\xf7D\xc5\x22!\
+ \x9c\xc7\x1aA\x02*X\x041]\x88\x88il\xb4\
+\x09I\x1bH\x91&\x85\x956\x81\x04\x03\x0b\xf66\xda\
+\x04\x02\x81\x80e:\x0b\x9b\x14\xa9.e\xbc;\x0c\x06\
+Br'\xde\xee\x9d7\xb7\xb73\xe3\x9b\x91\x84\xc8&\
+\x07\x87\x03o\x99\x99\x9d\xef\x7f\xff\x9b\xdd\xc7\xb4\xd6\xb8\
+\xce\xe0O\xb7\xea\xab\x8c\xb1\x90\xe6A\x9fl\x95\x92\xaf\
+s!\xda\xe1\xc3{\xa3A\xe1V\x0e_\xcam\xdc\xbd\
+\xe3cnj\x00\xdce=\xe9\xd2\xd7N\x10\xbe\xfd\x15\
+\xf2f\xb3I\xf0M(*%\x8e\xdb\x98\x9d\x1c\x06\x83\
+\x82\x94\xbd\xd3O\xdf\xce\xc1\xb0N\x145,\xac\x94\x84\
+\xe8\x08@\xa7H\xd3l,=\xfb\x8c\xef?\xcf\xff\xac\
+%e0\xac\x13\xc7\x11\xb4RPRA\x08\xf1O\xd8\
+\x849\xb7\xf6\xe2\x13N~\xb4\xae\xec\xf1V\xeb\x9c\x1c\
+\x90\x00\x89$Ib\x95\x17\x1e\x1f\xfc\xd7\xfa\xca\xf3C\
+\xeclL\x22(\x8c\xc2\xb0N\xa7\xd3%\x07\xda\x96\x91\
+v\xa5\x151{\xbd\xe2\xe5\xde\x18\xce\xce\x22;\xe7Z\
+;\xb0\xff\x02\x85\xa42\xea\xf5\x08A\xf0 \x93\xb9R\
+\xb9t51q\x1f\xef^\x03\xb5\x9a\x07\xc3r\xd7\xf5\
+\xad@7\xa52\xb4\x0b\xce=\xbc\x7f\xc33\x02\xf3\x8f\
+|\x14\x8b\x0b\xf6\xdd\xe9i\x03\xb9\xdc\x00\x0c\xcb=o\
+\x882S\x09\x92\xd1f\x1e\x9e\x97\xa7\xcf\x93d\x04\x0c\
+\xfc!\xcc\xa3\xd1h\xd93f\x18\x96\xfb\xfe\x089\xe0\
+\xa4\xa6I`\x10\xcc\xc9\x93\xad\xec\xe5\xedo{t\xeb\
+\x89M\xf2{\x18\xd6\xa1G\xb5|\x22I\x80cdh\
+\x10\xa5\xb2&\x11\xcfZ\xfc;\x84`W\xd6\xa5#e\
+\x04\xaalfq\xf7\xc9\x8d\xf1\xe5W`n\xb1\xafN\
+\xd0\xf2\xb8\xf6\xed\xe3\xa6\xf9\xe1\x8d\xa7a\xd3X}6\
+SJ\x11\xb3\xeb\xb6\xf3\x85\x00\x03\x00Kb\x16\x94\x80\
+n\x06\x02\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02\x98\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02:IDATx\xda\x94\
+\x92\xbf\x8b\x13Q\x10\xc7\xbf\xfb\x83\xdd\xec&\x9bDD\
+\xf1Rl!\x92&E\x0a+m\x02\x8apxw\xc5\
+\x15Al\xad\x02\xa2\x22XJ\x0a\x8b\x80\x95\x95\x82p\
+X\xdc\x1f\xa0\xc5Y\x08\x82V\x16\x17.M\x08\x829\
+\x11C$\xdem6\xd9\xec\xe56?6ow}o\
+\x135\xc1\xd3;\x07fgXf\xe6\xcd|f\xb8|\
+>\x8f\x99\xacQ]\xc2\xc9\xe4;\xd5-\xe6\x88?\xff\
+\x8c\xc7\xe3\xa5\x8d\x8d\x8d\xe7\x8e\xe3`8\x1c\x82\x10\x0f\
+\xed\xf6!\xf5}D\x22\x0a4MC<\x1eG\x22\x11\
+G\xa1p\xe3\xb6 \x08X(\xc0\x84\x10\x02\xdb\xb6\xd1\
+\xe9t\xc2\x02\x86\xd1\xc7h\xec#\x1a\xd5@<\x02^\
+\xe0\xa1F\x95\x85V\xf8\x7f6\xca\x01\x015\x01\xe7O\
+\x15S=y\x01\x1a>M\x0cf\xc9^\xa8\xf32?\
+B\xa5T*\xbd\xcef\xb3\xab\xbe\xefc0\x18\xccF\
+!\x94A\x04\xb1X\x8c\xce\x9f@\xbd^\x7fCcw\
+\x8e*p\xb1X,\xae\xceC4\xcc\x038#\x17\x92\
+,!\xa6E\x91\xa0\x10\xaf\xad\xac/\xdf-\xdcb\x1b\
+(\x1f\x0bq\xdf\xb4\xe1\xb8.\x14\x0an\xe2')D\
+@Q\xe5\xff\x81\xf8{v\x9f\xf3\x8eep\xf4\x16~\
+m\xc0\xc3c\xe3\x09\xbe\xec5`\xe5\xda7O\x9b\xf1\
+g\xc4'\x102\x99L\x18\xeby\x1e\xaa\xd5j\x8a\xda\
+4\x1b\xa1\xd5j\xe1[\xe3+z\x86\x01\xc7\xea\xc1\xe9\
+\xf6\xb0\xc5\xbdE\xeej\x0e\x1f\x9a\xdb\x83\xbd3\x9d\xa7\
+\xe6\xa9\x1eDF\x9c\x09\xb5\x7fB\xa4I\xf6\xd0\xc1\x8b\
+\xe1&v\xc7\xbbPy\x05\xb6gC\x1cp*\x91\x83\
+\x1d\xdaVEl6\x9bH&\x93p]7X\x84H\
+\xb0oY\xb0]\x07\xb5Q\x0d\xe7\xd7.\x84\x0f\x99\xc4\
+\xc4\xa5\xf5\xcb:u\xf5\xf7/\xdfA,\x97\xcbH\xa7\
+\xd3\x90eY\xfc\xdb1\xe9A\x0a\x8dW\x9f!\x8a\x22\
+\xa4\xe5(>m\xd6\x9a\x93\x88gPF\x15\x96\xa4\xd0\
+\xe3\xd0R\xa9\x94\xca\x02\xd8\xb1H\x92\x14\x8e \xc8\x0a\
+\xd4\xd1\x01\xee\xcbw\x10\x8d)\xb8\xb7\xfd\x00]\xaf\x0b\
+\xff\x90px\xd8\xbfNs\xfba\x01\xaag-\xcbr\
+u]\x7f\xc4`\x06A0\xdb\x018*\xec\x03\x9e\xe7\
+1\xb9\xe2\xaf\xf8e\x9c\xe3\xda\xc1G\x96\xc3N\xe7\x87\
+\x00\x03\x00\xee\x8d87\x1a\x1e4\xb5\x00\x00\x00\x00I\
+END\xaeB`\x82\
+\x00\x00\x03\x00\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\xa2IDATx\xda\x94\
+S]H\x93a\x14~\xb6\xef\xdb\x9a)\xa3e\x81\x08\
+\xb3\xacL3\x9c\x89\x9aN1\x179[\xa2\xfd\xd0\x95\
+\x10]V\xe0@\x22$\xd0\x94\xbc\xaa\x9bn\xec&\xeb\
+\xc2\x92\x91\x10\x99?E\xfe,\x94\x9c^53\xca4\
+\xa5\x1f\xcd_\x9a\xb9$\xe7\xe6\xb6oo\xef\xf9r\x82\
+A\x7f\x0f\x1c\xce\xfb\xbe\xdfs\x9e\xf7|\xe7\x9cWa\
+j\xf8\x02Bu_\xac\xec\x15\x0a\x1cU\x00f\xfc\x05\
+\x0c\xb0\xfb\x83\xe8\x12\xc3\x07\x8d\x86f\x94\x0e\x9d\xa6e\
+qA\xe5=\xeb\xe4\xe8(\xdc\x8b\x8bH\xcf\xcf\x87\x14\
+\x0c\xc253\x03A\x14\xa1R\xa9\xa0R\xab\xd1_W\
+\xb6\x891\x88\xc2\xce\x93\x15\xb2\xc0\x92F\x8f\xc9-9\
+\xd8\xec\x99R\xcdv\xd6y\xd51\xc9ii\xb9\xb9\xe8\
+iiA|b\x22\xfc\x1e\x0f\x5c\xd3\xd3\x08\xf8|\x90\
+\x02\x01\xc4eZ\x0e~xa\xf7Q\x06G\xb8\x95s\
+\x8b\x9d\xd2\x19\x01\xfd\x05ma\xcc\x8e\x98\x94\x8c\x0c\xf4\
+\xb6\xb5!3/O\xf6y\x16\x0b\x82<\xf0\xbb\xdb\x8d\
+\xc0\xea*\xbe\xcdM\xb8<~\x16)\x86$\xa9<+\
+9:\x7fk\xa4\xa8\x15\xc6:\x10\x8f.\x14\x99\x8d\xb8\
+}\xc7\x86\xd2S\x16t\xb7\xb7\xe3\xb0\xd9\x0cGg'\
+\x0epQ\x7f\x88\xe1\xed\x9bw\xab\x9f\xfa\x1f\x0e\x0bJ\
+<Ur\x81\xd8\xa5\x85e\xed\xc7\x097|\x1d\xd7P\
+\x98\x93\x86\x86\xa6v\xbcW\xef\xc7\x8d[6\x1c2\x99\
+\xd0k\xb7#%5\x15\xdd=\xfdh\xb2\xbfB\xfdx\
+\xb4k%\xc0\xceH!4\x82w\xc1\xc9\xd60>\xd0\
+\xca\xeeZ\xb3eO\x18\xe9kf\xf5\xe7\xd2\xd9\xec\x93\
+Z\xf6\xe0r\x01{\xd6t\x939\x9dNF1\xd4\xbd\
+\xf3\x97* R\x85C\xa1\x108\x1f\xbb\xb2\x8ae#\
+H\x92\x84\xbd9'\xe4o\x8f\xef_G\xbc\xe9,\xb4\
+\xbb\xb3d\x1e\xc5\x10F\x92.\xfe\x14 \xb2\xb15\x09\
+\x03\xc7G\xe0p8\xa0\xd3\xe9\xa0\xd1h\xa0\xe6\xed\xda\
+\x93]\x22[\x18J\xa5\x12\x92s~}/ReI\
+\xe0y\xd1k\x04\xb9\x98\xd1h\xdc00\xc1\xb5\xdb\xc2\
+\x10\x04A\xee\xc6\x06\x01\x22\x0d\xd5T!\xa5\xa6\x16\x83\
+\x83\x83\x88\x88\x88X'x\xbd^y\x1f\xf6\x06\x83\xe1\
+\x17\x01\xbf_\xce`_e\xb5,\x94\xca\xab\xfd'\x10\
+\x97b\xd6\x05h(\xe8\xb0\xea\xd16\x5c-\x99\xc3(\
+\x8d0\x1f\x16\xaa\x03!\xbc\x8e\x8a\x8a\x82^\xaf\x97k\
+@1\x84\x95\xc9\x97\x5c`-\x83+\xc7\xa6@\xbf\x9b\
+\x90\x90\xf0\xdb\xdb)C\x91\xbf\x07\x8a\xf1}\x1e\xc2\xb4\
+\xcd\x0a\xd1\xbb\xbc\xcc_\xa0B~$\xff\x02\xe2R\xcc\
+\x8c\xcd\xba\x9dJ$~\x1d~>\x1cW6\x8f\xff\x01\
+[\x18\x1b\xe7\x8e\x04\x16\x7f\x080\x00A\x00Z5\xf6\
+\x03<I\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02\x9e\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02@IDATx\xda\x8c\
+SMo\x12Q\x14=\xcc\x8c\x033\xc3\xc0\xa0\x05\x0b\
+\x89\x8bn\xd8X\xc5\xa4\x91\xbd\x0b\x12\x13jL\xd3\x10\
+\x17\xb2rEb\xe2O`\xc9_06ld\xdfU\
+\x9b\xd8\x05Iw.\x10\xe2\xa6I\x01c\x5c\x10\x87\x00\
+C\x85A>\x9d\x0f\xef\x00\x1a\xb0\xa6\xedI\xee\xdc;\
+\xef\xdd{\xe6\xdd\xf3\xee\xb8R\xa9\x14\x96xF\x16\xc6\
+\xcd\xd0$;r\x02\xee\xcf\xcat:\x0d\xe7\xf3\xf9w\
+\xc3\xe1\x10\xe3\xf1\x18\x86a\xa2\xd3\xf9I\xb1\x05\x8fG\
+\x80,\xcb\xf0\xf9|\xf0\xfb}\xc8d^\xbcfY\x16\
+k\x04\x0e\x0c\xc3@\xbf\xdfG\xb7\xdb\x9d\x13\xb4\xdb\x03\
+L\xa6\x16$I\x86a\x1a`X\x06\xa2$\xac\x1d\x85\
+\xb9\xf2\xa0.\xc0&g\xbb\xac\x85aa7'\xa0\xf4\
+E\xa1\xbd,6\xe7\xb6\x8a\xd5\x16*\xb9\x5c\xee8\x16\
+\x8b\xedZ\x96\x85\xd1h\xb4l\xc5 \x0d<\xf0z\xbd\
+\xd4\xbf\x1f\xf5z\xfd\x84r\xcb\xff#\xd8\xc9f\xb3\xbb\
+\xab\x22\xb65\x1d\xc3\xc9\x0c\xbc\x9b\x87W\x96\xe0'\x11\
+\x13\xc9\xbd\xa7o2\xaf\x9c\x1b(]+bK\xebc\
+8\x9bA \xe1~Y\x0a\x89\x08\x08\xa2\xfbo\xfe\xfd\
+ju\x9d\xe0_\x84\xc3!(\x01\x05]\xbdG7!\
+\xe2\x1e\xbdK\x92\x84\x87\xb5\xda\xa7\xcd\x8b\x0b\xdc\xe9t\
+\xae!\xd8\x0c\xe1{\xfa%\x1e\x1f\x1c\xc0\xdc\xda\xc2\xe7\
+Db\xf1\xe5Z\xed\xedBbT\xae\x14\xd1M\xbd\x9b\
+\x81\x00N\xd3i\xec\x9f\x9fc@k\xc9x\x1c\xd8\xde\
+\xdeq\x0a\xde\x17\x0a\xe0\x9cd\x07\xe4/\x89\xe8W\x02\
+8\xa1\xc2\xe7\x87\x87h\xff\xd0\xa8\x15\x1d\x85b\x11M\
+U\xad,\x05\xacp\x8dF\x03\x8a\xa2`6\x9b\xd9\xeb\
+\x22\x1ahu5<\xfap\x8cr_\x83\xf8\xad\x8aD\
+\xe5#$Q\xc2~r/\xf3\xe0\xec\xac|\xb7\xd7\x03\
+W*\x95\x10\x8dF\xe9\xb8\xeeKz4[-T\x1b\
+_\xc1K\xb7\xa0\x18>\x1a*\x13\xa1\x8d t]\x8f\
+\x17\x83\xc1\xf2\x17\x87\x80\xf2\x04\x1a\x0e9\x12\x89\x88\x1c\
+\xc7\xcd\x87\x85\xe7\xf9y\x0b\xac[\x808\xd1\xc1\xb8]\
+\x90\xbc\x14\x8b\x02X\x8e\x81\xa6i\x82\xaa\xaa!\xaa\x1d\
+\xd0\xb4\xe36YD\x10\x84'\xb6mo\x98&\x8d\xab\
+m/\xff\x04\xb8\x08\xce\x03\x0c\xc38\xdevb\xda\xef\
+\x90N\xa7\xb4\xaf\xfe\x16`\x00D\x1c!\xc5N\x09>\
+\xcb\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02v\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\x18IDATx\xda\xa4\
+\x93\xcf\x8b\x92a\x10\xc7\xe7\xfd\x15\xac\x9b?v_\xd1\
+\xea\xa0\x22aJ\x07\x17^(\xc2\xe8\xd2\xa1.\xd2\xa9\
+\xc3Z\xd0!\xf0\xbcD\xff@\xf7\xba\x87\x17OK\x10\
+\xe8\xc5\xc3\x86l\x11y\xe8$\xee\x1e6c\x0f!\xe5\
+\x92\xf8\xbam\xea\xeb\xaa\xbd\xfa\xdawD]\xb7\xbc\xf9\
+\xc0\x87\x99y\xdf\x99yf\xe6y\x1ea4\x1a\xd12\
+K\xa4%\x97\xfc\xe4\xc5\xcf\x88$Io\xa0G\xc1\xfe\
+p8\xdc\x04\xe5?_\x9f\xcd\x9c\x82\xc1 \xc1gM\
+\x14\xc5\xbb0UplY\xd6{\xf8\x9dH\xea\xd5\x87\
+\xbb7\xae\xafF\xe3w\xd6\xe8\xf4\xb4}i\xef\xa0z\
+[\xd1\xd3\xaf\x85as\x96\xa0\xd3\xe9\x90i\x9a\x0f\x12\
+\x89\xc4S\xb0\xe5p8\x9c\x85B\xa1\xdd\xedv\x0f\xe4\
+j\xf5(\xaaE\xc2\xd4\xef\xf7I\x8b\xd8)\xfd\xf6(\
+\xba~\xb1\x92\x9c\x9f\x0c\xff\xab\xd7\xeb+\xe1p\xf8\x1e\
+'cY\xa9Tv\xc63\x10\x84\xd5\xfd\x9dOU\xea\
+\xf5z\xc4\x92mcx%5\x18\x0cR\xfc\x8de\xb3\
+\xd9L!\xe0$\x93\xc9|h\xb5Z\xc4\x92m@\xc2\
+\xcd\xcd/\x11Q\x94g3\xb0\xac\x01f`\x96\xed\xfa\
+\x16o\x90\x04\xa9R\xa9D\xe8\xd9\x8d\x9e\xe3\xb0=\xa0\
+\x8e\x99\xe40\x93\x86\x8c\xe0\xb2\xa2\xaclL\xcb5\xcd\
+.Y\xc7\x192\x0cc\xd6\x82\xaa\xaaT\xab\xd5\x1a\x98\
+C\xfa\xdc\x11\x8a\x22\xc9\x8b\x8e\xa6\xfd}\xfb\x9c\xedv\
+\xbb)\x14\x0a\x8d\x03\xa6\x0b\x15\x11*\xfa?\x81\xf1c\
+\x9b\xb8\xcf\xf9\xe5\xf3\xf9\x08\x17n\x1dA\xf79\x1fh\
+\xc0~\x07\xf9\x8bn=:$\xff\xc6\xd9\x99+\x8aB\
+N\xa7sJ\xd2f\xb3\x91\xc7\xe3\xa1X,\xf68\x9f\
+\xcf\xefb\xd7\x11K\xb6\x01\x09\x0b\xaf'\xf7&\x8f\x8b\
+\x8bc\xa7\xcb\xac\x04\x02\x01{\xb1X|9\xf5\xd14\
+\xed9\xc4+iQ\x02~\x1f\xdc\x1fJ>\x84^\x9c\
+p\xcd\xeb\xf5\xba\xfc~\x7f \x9b\xcd~\xcc\xe5r\x9f\
+u]\xdf\x9b\xaf\x80uN\xc8[_\xe0n&r\x0c\
+\xaar\x01\x0d\xba\x0b\xfcF\xf2\x22\xf8\xf6o\x02a\xf2\
+\xc0\xa4\x05\x88s\xb0\x9f\xc9\xb7\x5cX\xf69\xff\x15`\
+\x00\x90\xd5\x03\xaeF\x8f\xca\xf0\x00\x00\x00\x00IEN\
+D\xaeB`\x82\
+\x00\x00\x02\xf0\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\x92IDATx\xda|\
+S]HSa\x18~\xcf9\xdfY\x07e)d\xad\
+\x0b5\xc3RJ\x89Ff\xd4\x9a\xd1\xfa\x13\xd9\x85\xcc\
+\xb0\x10\x22\xeb\xa2\x940*\x0aR(\x93$\xb3`\x04\
+#\xf4\xca\xdaE\x17\x11\x91P^\x98xQ\x9a\x83A\
+dDM\xbch\x924\xcb\x896\x9bz\xce\xd9\xe0\xf4\
+\xbe\xdf\xe6I!\xfa\xe09{\xce\xf3>\xcf\xfb}\xef\
+\xc7\x8e\xb0\x01\x00\x04\x82 \xa4~\xd3\xc0\xb5\x1fq)\
+E\xe1A\xdez\x18\xce\xcb1*\x90\xe7 f\x10o\
+\xa9\xc0\xe0\xdf\x8b\x8c\x97\xbd]]\xd5\xf4r\xa5\xb1Q\
+\x9a\x8c\x82x\xae\xde]z\xba\xa5\xfb\xa1\xffN\xc3\x85\
+\xff58`\x00\x5c\xbd\xef\xf3\xb9\xcb\xca\x0a\xb9p\xcf\
+\xe7\xab\xbe\xd6\xd4\xc4B\xe1\xd8\xf4Bl\x06\xe2\xf1E\
+y\xd9,e\xae\x1e\xe1 \xd2\xeb\x1d^o\x95\xc3\xb1\
+=\xa5!rs\xd7\xc1\xd6m\xf6\xa2\x0f\xa1I{\x96\
+5\x03\xc2\xa1\xe0\xa0\xaa\xeb#\x88U'8\x84;\xb7\
+\xdc\xee\xect9\x9d\xa5\x10x\xdc\x01Y\xe5'x!\
+\x16|\x0a\xce\xfafH$\x12\xe0\xf7?\x875\x89\xf9\
+]\xd1\xe8\x1c\x18+F8b\x18\xc6\x8d\x9b\xed\xedN\
+\x97\xcb\x0e\xb2,\xc3\xc2\xcf\x09(q\xd6\xf2b\xe4e\
+'\xd7\xa8\xa6\xe3\xae\xaf\xfb\xfbO\x8e\x86\xc6z\xb0\xc1\
+\x0058\x8a\xe4VKk\xeb\xde\xca\xca=\xa0(\x8a\
+y\xa4\xec\x0c\x8b\xc9%I\xe2 \x0f\x9d$04\xd4\
+F\x93\x8b\xf8h_\xcb\xd8\x9bw\xcf\xda\xce\xdbl6\
+\xd3\x98i+\x80\xef\xc1>\x0e\xe2\xcb:y\xc8K\x19\
+\xca2\xdc\xbd\xbc ?\x07<5\xfb\x1aDQ\xe4&\
+Z\xc7.v\x98\xbb\x17\x17\xff\xe5\xe4\xf1\xd4x\xc4\xb9\
+'#\xcd\x1f\xbf\xfe\x00\xb1\x10\xc3\xa7j\xcbAO$\
+E\x11\xc3\x8c1\x8e\xf1\xe00x\xcfTs\x10_\xd6\
+\xc9C^\xcaP\x96\x9d=\xbe\x1b4=\xc1\x9b\x0bb\
+\xcaD\xeb\xfd\x8b\x1e\xf0\xb8\x1d\x9c\x07\x90\xef\xa88\xcc\
+9y\xd0O\xa3\x03e\x99\xaa\xe9\xe6=\xad\x1c\xc1\xd0\
+\x17\xf9\x8d[\xadV\xd8\xb2i\xa3\xa9\x93\x073\x929\
+\xd2\x97\x89iXR5\x026\x90\xcc\xcbR\x14\x0b\xa8\
+\xaa\x0a\xb3\xb3\xf3\xd0\xdb;h\xea\xe4!/e(+\
+v\xf7}\x82\xb1o3(\xaa\x92\xb0\xaa\x81\xcc\x1b(\
+\x0a\x83\xba\xba*S\x17x\x03U\xa2\x0cei\x96\xac\
+G\x03c\xb6\xf8\xc2\x12\x13\x98\x05DK\x06\x87\xc5\x22\
+\x83\xa6i\x10\x89D`jj\xca\xd4\xc9C^\xcaP\
+\x96>\x83|\xfa\xcf\xec\xc4o \x1b\xa0\x88\xe6\xfa\x05\
+\xf0\xea7c%H\xc3\xe9Q7[\x93\xc9\xcfXw\
+\xa7\xeb\xe3\xa3\x00w\x89\xfe\x11`\x00\xce\x92\xf8\xe0\x98\
+`\x1e\x9f\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02\x1a\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xbcIDATx\xda\xa4\
+S=K#Q\x14=o\xe6e\xf1cc\xb3\x90\xa0\
+\x85\xca\x22\xeb.Q\x88\x8a\x04\x05A!\xa5\x95l\xca\
+\xb5\xddZHc\xe1\xb6[\xa9\xb5\xb6\xfe\x82\x80M\x1a\
+\xc1\x8f\xc2\x0fD%Xh1$\xa3\x12\xa3\x19a\xd5\
+,\x92\x99I\xbc\xf7\x8d\x19\x12e\x17\xd4\x0b\x87\xb93\
+\xf7\xde3\xe7\x1e\xde\x13\xd5j\x15\xef\x09\x91H$>\
+\xd33F\x08\xber\xf6\x8e\xb0#]\xd7\x1dI&\x93\
+\xb3\xa1P(\xe2\xba\x0e\x1c\xc7%\xd8\xb0m\xce\x1dT\
+*\x15x\x22u\x08!\x15\xa4\xfc\x00\xcb\xb2\x8e\x97\x97\
+\x17~Kjh+\x95J\x11\xc30T3\x83H\x15\
+\xfe\x97\x13\x22\xa9T\xaaU\x06\x02\x81J<\x1e\x7f\xd3\
+\xfe\xe9tZH\x92)<\x99\x8df\xfeX=\xc5N\
+\xfe^\xe5\xb1\xf6\x8fX\x99\xfc\xd2h\x9e\x10\xbc\xa2\x22\
+\xd0j\xb2\xea\xe3\xe8\xe2\x16\x03\xc3\xc3^\xbe\xb7\xa7\xfc\
+\xa8\x0fM\xd3\xf8\x9b\xe6\x130\xea\xc3)^\xe3\xcc4\
+\xfd\xfc9\x81\xae\xeb\x1e\x81m\xdb\x1a\x17k\x0d\xe6\xcc\
+\x0c\xfe\x1e\x1eb\xaa{\x14\xa7\xe7'\xc8\xf7\x02=a\
+\x03\xbf6\xe6\xd0\xd5\x16\xc5tdQ\xf5\xf1\xca<+\
+\xcb\xe5\xb2\xce\x7f\xaf\x11\xdc\x1c\x1c`l|\x02,\xde\
+\xccna\xe9\xfb\x15\xa2\x83\xdf\xe8m\x08\xbb\xdb\x19\xbf\
+\x8f=\xe0Y&P+\x10\x9b*\x94\x88\xb9\xb0\xb6\x0f\
+\xc7\xfa\x03\xab\x85\x08\x8b:r\xd9\x9c\xaa\x15/\x1f\xfc\
+>\xf6\x80g_(\xd0\xfb\xfa\xb0\x99\xc9\x00\x9f\x80\xa6\
+p\x18\x0f\xd7\xc0\xbaQP\xb5\xaf\x1d\xfd~\x9f\x94\xd2\
+S@\x87(\xc0r\xe8<\xa8Bt~\xbe\xc1\xac\xd8\
+\xbf\xee\x00\xcd\xa8\xd9`0\xf8\x93\x1c\xed|\xcbA\x22\
+\xe5\xa6\xa0g\xf3\xd3E\x92\xaf\x9c\xe7]\xee\xc4{\xaf\
+\xf3\xa3\x00\x03\x00%0\x12$Q\x12\x04\x0b\x00\x00\x00\
+\x00IEND\xaeB`\x82\
+"
+
+qt_resource_name = b"\
+\x00\x05\
+\x00o\xa6S\
+\x00i\
+\x00c\x00o\x00n\x00s\
+\x00\x0b\
+\x09\x8b\x9c'\
+\x00c\
+\x00o\x00n\x00t\x00r\x00o\x00l\x00.\x00p\x00n\x00g\
+\x00\x16\
+\x04\xaf\x19\xc7\
+\x00a\
+\x00p\x00p\x00l\x00i\x00c\x00a\x00t\x00i\x00o\x00n\x00-\x00d\x00i\x00a\x00l\x00o\
+\x00g\x00.\x00p\x00n\x00g\
+\x00\x14\
+\x04i\x90\xc7\
+\x00d\
+\x00a\x00t\x00a\x00b\x00a\x00s\x00e\x00-\x00-\x00p\x00e\x00n\x00c\x00i\x00l\x00.\
+\x00p\x00n\x00g\
+\x00\x12\
+\x0dk\xa4g\
+\x00c\
+\x00l\x00i\x00p\x00b\x00o\x00a\x00r\x00d\x00-\x00t\x00e\x00x\x00t\x00.\x00p\x00n\
+\x00g\
+\x00\x0f\
+\x0b\xd3g\x87\
+\x00b\
+\x00o\x00o\x00k\x00s\x00-\x00s\x00t\x00a\x00c\x00k\x00.\x00p\x00n\x00g\
+\x00\x17\
+\x02\xc3\x01'\
+\x00c\
+\x00o\x00n\x00t\x00r\x00o\x00l\x00-\x00s\x00t\x00o\x00p\x00-\x00s\x00q\x00u\x00a\
+\x00r\x00e\x00.\x00p\x00n\x00g\
+\x00\x0f\
+\x00l#\xe7\
+\x00z\
+\x00o\x00n\x00e\x00-\x00-\x00a\x00r\x00r\x00o\x00w\x00.\x00p\x00n\x00g\
+\x00\x13\
+\x05\x12\x08\xe7\
+\x00n\
+\x00o\x00d\x00e\x00-\x00s\x00e\x00l\x00e\x00c\x00t\x00-\x00a\x00l\x00l\x00.\x00p\
+\x00n\x00g\
+\x00\x10\
+\x0c\x1etG\
+\x00s\
+\x00c\x00r\x00i\x00p\x00t\x00s\x00-\x00t\x00e\x00x\x00t\x00.\x00p\x00n\x00g\
+\x00\x0f\
+\x02\xacb\x87\
+\x00z\
+\x00o\x00n\x00e\x00-\x00s\x00e\x00l\x00e\x00c\x00t\x00.\x00p\x00n\x00g\
+\x00\x18\
+\x0f\xa1\xdc\xc7\
+\x00l\
+\x00a\x00y\x00e\x00r\x00-\x00s\x00h\x00a\x00p\x00e\x00-\x00p\x00o\x00l\x00y\x00l\
+\x00i\x00n\x00e\x00.\x00p\x00n\x00g\
+\x00\x17\
+\x04F\x0d\x87\
+\x00u\
+\x00i\x00-\x00c\x00h\x00e\x00c\x00k\x00-\x00b\x00o\x00x\x00e\x00s\x00-\x00l\x00i\
+\x00s\x00t\x00.\x00p\x00n\x00g\
+\x00\x0c\
+\x07J\x9a\xc7\
+\x00p\
+\x00r\x00o\x00p\x00e\x00r\x00t\x00y\x00.\x00p\x00n\x00g\
+\x00\x11\
+\x06\x89\xcd\xe7\
+\x00r\
+\x00e\x00p\x00o\x00r\x00t\x00-\x00-\x00m\x00i\x00n\x00u\x00s\x00.\x00p\x00n\x00g\
+\
+\x00\x12\
+\x0c\x160\xe7\
+\x00p\
+\x00r\x00i\x00n\x00t\x00e\x00r\x00-\x00-\x00a\x00r\x00r\x00o\x00w\x00.\x00p\x00n\
+\x00g\
+\x00\x14\
+\x02\x0a\xb5'\
+\x00l\
+\x00a\x00y\x00e\x00r\x00-\x00s\x00h\x00a\x00p\x00e\x00-\x00t\x00e\x00x\x00t\x00.\
+\x00p\x00n\x00g\
+\x00\x0f\
+\x09\x00\xfbg\
+\x00b\
+\x00l\x00o\x00c\x00k\x00-\x00-\x00p\x00l\x00u\x00s\x00.\x00p\x00n\x00g\
+\x00\x09\
+\x02\xc5\xa4\xc7\
+\x00r\
+\x00u\x00l\x00e\x00r\x00.\x00p\x00n\x00g\
+\x00\x0f\
+\x0e\xf8X\xa7\
+\x00s\
+\x00c\x00r\x00i\x00p\x00t\x00-\x00t\x00e\x00x\x00t\x00.\x00p\x00n\x00g\
+\x00\x1d\
+\x0d;u\x07\
+\x00b\
+\x00l\x00u\x00e\x00-\x00d\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00a\x00t\x00t\
+\x00r\x00i\x00b\x00u\x00t\x00e\x00-\x00s\x00.\x00p\x00n\x00g\
+\x00\x0f\
+\x08\x0fK\x87\
+\x00z\
+\x00o\x00n\x00e\x00-\x00r\x00e\x00s\x00i\x00z\x00e\x00.\x00p\x00n\x00g\
+\x00\x14\
+\x0d\xcb\xc0G\
+\x00s\
+\x00t\x00i\x00c\x00k\x00y\x00-\x00n\x00o\x00t\x00e\x00-\x00t\x00e\x00x\x00t\x00.\
+\x00p\x00n\x00g\
+\x00\x13\
+\x0f\xb9>\xc7\
+\x00d\
+\x00a\x00t\x00a\x00b\x00a\x00s\x00e\x00-\x00i\x00m\x00p\x00o\x00r\x00t\x00.\x00p\
+\x00n\x00g\
+\x00\x16\
+\x0a\x9a8'\
+\x00z\
+\x00o\x00n\x00e\x00-\x00r\x00e\x00s\x00i\x00z\x00e\x00-\x00a\x00c\x00t\x00u\x00a\
+\x00l\x00.\x00p\x00n\x00g\
+\x00\x19\
+\x01\xca\xd7\x07\
+\x00c\
+\x00a\x00l\x00c\x00u\x00l\x00a\x00t\x00o\x00r\x00-\x00s\x00c\x00i\x00e\x00n\x00t\
+\x00i\x00f\x00i\x00c\x00.\x00p\x00n\x00g\
+\x00\x0f\
+\x07\xef\x0e\xa7\
+\x00l\
+\x00a\x00y\x00e\x00r\x00-\x00s\x00h\x00a\x00p\x00e\x00.\x00p\x00n\x00g\
+\x00\x17\
+\x04\x9c\xcf\x07\
+\x00l\
+\x00a\x00y\x00e\x00r\x00-\x00s\x00h\x00a\x00p\x00e\x00-\x00p\x00o\x00l\x00y\x00g\
+\x00o\x00n\x00.\x00p\x00n\x00g\
+\x00\x19\
+\x07\xf6\x08G\
+\x00a\
+\x00r\x00r\x00o\x00w\x00-\x00c\x00i\x00r\x00c\x00l\x00e\x00-\x003\x001\x005\x00-\
+\x00l\x00e\x00f\x00t\x00.\x00p\x00n\x00g\
+\x00\x17\
+\x06\xaf\xee\xe7\
+\x00r\
+\x00e\x00p\x00o\x00r\x00t\x00-\x00-\x00e\x00x\x00c\x00l\x00a\x00m\x00a\x00t\x00i\
+\x00o\x00n\x00.\x00p\x00n\x00g\
+\x00\x14\
+\x0a\x13\x0c'\
+\x00t\
+\x00a\x00g\x00-\x00l\x00a\x00b\x00e\x00l\x00-\x00y\x00e\x00l\x00l\x00o\x00w\x00.\
+\x00p\x00n\x00g\
+\x00\x10\
+\x07}0\x07\
+\x00a\
+\x00r\x00r\x00o\x00w\x00-\x00c\x00i\x00r\x00c\x00l\x00e\x00.\x00p\x00n\x00g\
+\x00\x14\
+\x00\x83\xac\xe7\
+\x00a\
+\x00p\x00p\x00l\x00i\x00c\x00a\x00t\x00i\x00o\x00n\x00-\x00w\x00a\x00v\x00e\x00.\
+\x00p\x00n\x00g\
+\x00\x14\
+\x02Gc'\
+\x00d\
+\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00-\x00p\x00e\x00n\x00c\x00i\x00l\x00.\
+\x00p\x00n\x00g\
+\x00\x09\
+\x09(\xa3\xa7\
+\x00t\
+\x00a\x00b\x00l\x00e\x00.\x00p\x00n\x00g\
+\x00\x12\
+\x05\xb4\x8ag\
+\x00a\
+\x00r\x00r\x00o\x00w\x00-\x00s\x00t\x00e\x00p\x00-\x00o\x00u\x00t\x00.\x00p\x00n\
+\x00g\
+\x00\x08\
+\x05\xa8Y\xe7\
+\x00n\
+\x00o\x00d\x00e\x00.\x00p\x00n\x00g\
+\x00\x16\
+\x02M\xd2'\
+\x00r\
+\x00e\x00g\x00u\x00l\x00a\x00r\x00-\x00e\x00x\x00p\x00r\x00e\x00s\x00s\x00i\x00o\
+\x00n\x00.\x00p\x00n\x00g\
+\x00\x0f\
+\x09\xa2\xd2g\
+\x00n\
+\x00o\x00d\x00e\x00-\x00d\x00e\x00l\x00e\x00t\x00e\x00.\x00p\x00n\x00g\
+\x00\x0e\
+\x05.\x04'\
+\x00a\
+\x00r\x00r\x00o\x00w\x00-\x00s\x00k\x00i\x00p\x00.\x00p\x00n\x00g\
+\x00\x10\
+\x0d\x8c\xc4G\
+\x00i\
+\x00m\x00a\x00g\x00e\x00-\x00e\x00x\x00p\x00o\x00r\x00t\x00.\x00p\x00n\x00g\
+\x00\x14\
+\x02\xbd\xa4'\
+\x00l\
+\x00a\x00y\x00e\x00r\x00-\x00s\x00h\x00a\x00p\x00e\x00-\x00l\x00i\x00n\x00e\x00.\
+\x00p\x00n\x00g\
+\x00\x11\
+\x05-\xbe\x07\
+\x00t\
+\x00o\x00g\x00g\x00l\x00e\x00-\x00e\x00x\x00p\x00a\x00n\x00d\x00.\x00p\x00n\x00g\
+\
+\x00\x17\
+\x09_\xee\xe7\
+\x00l\
+\x00a\x00y\x00e\x00r\x00-\x00s\x00h\x00a\x00p\x00e\x00-\x00e\x00l\x00l\x00i\x00p\
+\x00s\x00e\x00.\x00p\x00n\x00g\
+\x00\x13\
+\x03k|g\
+\x00c\
+\x00l\x00i\x00p\x00b\x00o\x00a\x00r\x00d\x00-\x00p\x00a\x00s\x00t\x00e\x00.\x00p\
+\x00n\x00g\
+\x00\x10\
+\x03\xec\xe9\xc7\
+\x00g\
+\x00e\x00a\x00r\x00-\x00-\x00p\x00e\x00n\x00c\x00i\x00l\x00.\x00p\x00n\x00g\
+\x00\x12\
+\x01\xc1\xefG\
+\x00d\
+\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00-\x00p\x00l\x00u\x00s\x00.\x00p\x00n\
+\x00g\
+\x00\x13\
+\x01\x1aQ\xe7\
+\x00d\
+\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00i\x00m\x00p\x00o\x00r\x00t\x00.\x00p\
+\x00n\x00g\
+\x00\x14\
+\x08F\x83\x07\
+\x00r\
+\x00e\x00s\x00o\x00u\x00r\x00c\x00e\x00-\x00m\x00o\x00n\x00i\x00t\x00o\x00r\x00.\
+\x00p\x00n\x00g\
+\x00\x11\
+\x0f\xbd\xd5\x07\
+\x00d\
+\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00t\x00a\x00s\x00k\x00.\x00p\x00n\x00g\
+\
+\x00\x0c\
+\x03v\xc2\x07\
+\x00q\
+\x00u\x00e\x00s\x00t\x00i\x00o\x00n\x00.\x00p\x00n\x00g\
+\x00\x0f\
+\x0d_\xc3\xe7\
+\x00s\
+\x00c\x00r\x00e\x00w\x00d\x00r\x00i\x00v\x00e\x00r\x00.\x00p\x00n\x00g\
+\x00\x14\
+\x02\x1a\xad\x87\
+\x00a\
+\x00r\x00r\x00o\x00w\x00-\x00c\x00i\x00r\x00c\x00l\x00e\x00-\x002\x002\x005\x00.\
+\x00p\x00n\x00g\
+\x00\x14\
+\x0a\xb0\xb0\xa7\
+\x00a\
+\x00r\x00r\x00o\x00w\x00-\x00t\x00r\x00a\x00n\x00s\x00i\x00t\x00i\x00o\x00n\x00.\
+\x00p\x00n\x00g\
+\x00\x0c\
+\x09\xe0\x0eg\
+\x00e\
+\x00x\x00t\x00e\x00r\x00n\x00a\x00l\x00.\x00p\x00n\x00g\
+\x00\x11\
+\x01_\xdb\x07\
+\x00d\
+\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00c\x00o\x00p\x00y\x00.\x00p\x00n\x00g\
+\
+\x00\x12\
+\x08ZTG\
+\x00c\
+\x00o\x00n\x00t\x00r\x00o\x00l\x00-\x00d\x00o\x00u\x00b\x00l\x00e\x00.\x00p\x00n\
+\x00g\
+\x00\x0f\
+\x0a\xe7\xdb\x07\
+\x00n\
+\x00o\x00d\x00e\x00-\x00d\x00e\x00s\x00i\x00g\x00n\x00.\x00p\x00n\x00g\
+\x00\x16\
+\x02w@'\
+\x00b\
+\x00l\x00u\x00e\x00-\x00d\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00n\x00o\x00d\
+\x00e\x00.\x00p\x00n\x00g\
+\x00\x08\
+\x06HGg\
+\x00z\
+\x00o\x00n\x00e\x00.\x00p\x00n\x00g\
+\x00\x0e\
+\x09\xee\x04'\
+\x00a\
+\x00r\x00r\x00o\x00w\x00-\x00s\x00t\x00e\x00p\x00.\x00p\x00n\x00g\
+\x00\x10\
+\x0a\xa2\x9b\xc7\
+\x00u\
+\x00i\x00-\x00c\x00h\x00e\x00c\x00k\x00-\x00b\x00o\x00x\x00.\x00p\x00n\x00g\
+\x00\x0e\
+\x05\xed5\xe7\
+\x00a\
+\x00r\x00r\x00o\x00w\x00-\x00m\x00o\x00v\x00e\x00.\x00p\x00n\x00g\
+\x00\x13\
+\x02\x81\xde\x87\
+\x00d\
+\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00-\x00m\x00i\x00n\x00u\x00s\x00.\x00p\
+\x00n\x00g\
+\x00\x08\
+\x05\x9eY'\
+\x00l\
+\x00o\x00c\x00k\x00.\x00p\x00n\x00g\
+\x00\x0f\
+\x09\x91\x09\x07\
+\x00n\
+\x00o\x00d\x00e\x00-\x00i\x00n\x00s\x00e\x00r\x00t\x00.\x00p\x00n\x00g\
+\x00\x14\
+\x0d\x83\xd8g\
+\x00s\
+\x00e\x00l\x00e\x00c\x00t\x00i\x00o\x00n\x00-\x00r\x00e\x00s\x00i\x00z\x00e\x00.\
+\x00p\x00n\x00g\
+\x00\x0d\
+\x0d\xc8^g\
+\x00p\
+\x00i\x00n\x00-\x00-\x00p\x00l\x00u\x00s\x00.\x00p\x00n\x00g\
+\x00\x08\
+\x00/Z\xe7\
+\x00f\
+\x00i\x00l\x00l\x00.\x00p\x00n\x00g\
+\x00\x12\
+\x08K\xc1\xa7\
+\x00d\
+\x00a\x00t\x00a\x00b\x00a\x00s\x00e\x00-\x00-\x00p\x00l\x00u\x00s\x00.\x00p\x00n\
+\x00g\
+\x00\x11\
+\x0ba\x09\xc7\
+\x00p\
+\x00r\x00o\x00p\x00e\x00r\x00t\x00y\x00-\x00b\x00l\x00u\x00e\x00.\x00p\x00n\x00g\
+\
+\x00\x13\
+\x05\x8a\xeeg\
+\x00d\
+\x00a\x00t\x00a\x00b\x00a\x00s\x00e\x00-\x00d\x00e\x00l\x00e\x00t\x00e\x00.\x00p\
+\x00n\x00g\
+\x00\x0f\
+\x0e\xaf\xb2g\
+\x00n\
+\x00o\x00d\x00e\x00-\x00s\x00e\x00l\x00e\x00c\x00t\x00.\x00p\x00n\x00g\
+\x00\x08\
+\x068Z\xa7\
+\x00h\
+\x00o\x00m\x00e\x00.\x00p\x00n\x00g\
+\x00\x15\
+\x01\xe5\x04'\
+\x00a\
+\x00p\x00p\x00l\x00i\x00c\x00a\x00t\x00i\x00o\x00n\x00-\x00b\x00l\x00o\x00c\x00k\
+\x00.\x00p\x00n\x00g\
+"
+
+qt_resource_struct = b"\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00J\x00\x00\x00\x02\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x0a\xc2\x00\x00\x00\x00\x00\x01\x00\x00\xaaB\
+\x00\x00\x01\x86Et\x06\x08\
+\x00\x00\x01\x0e\x00\x00\x00\x00\x00\x01\x00\x00\x0cQ\
+\x00\x00\x01\x86Et\x87*\
+\x00\x00\x05P\x00\x00\x00\x00\x00\x01\x00\x00HP\
+\x00\x00\x01\x86Es\xa6\x16\
+\x00\x00\x07\xa8\x00\x00\x00\x00\x00\x01\x00\x00o\xd3\
+\x00\x00\x01\x86Es\xf4n\
+\x00\x00\x08\xe6\x00\x00\x00\x00\x00\x01\x00\x00\x88\xad\
+\x00\x00\x01\x86Es\xf3\x0e\
+\x00\x00\x07~\x00\x00\x00\x00\x00\x01\x00\x00mp\
+\x00\x00\x01\x86Es\xf0\xbe\
+\x00\x00\x04\x00\x00\x00\x00\x00\x00\x01\x00\x006\x19\
+\x00\x00\x01\x86Es\xcfV\
+\x00\x00\x0b\x90\x00\x00\x00\x00\x00\x01\x00\x00\xba&\
+\x00\x00\x01\x86Es\xa2\x98\
+\x00\x00\x02\x82\x00\x00\x00\x00\x00\x01\x00\x00 \x96\
+\x00\x00\x01\x86Et\x1fA\
+\x00\x00\x08l\x00\x00\x00\x00\x00\x01\x00\x00\x80'\
+\x00\x00\x01\x86Es\xa8\x9e\
+\x00\x00\x05~\x00\x00\x00\x00\x00\x01\x00\x00J\x9a\
+\x00\x00\x01\x86Es\xf0\xae\
+\x00\x00\x06\x04\x00\x00\x00\x00\x00\x01\x00\x00T<\
+\x00\x00\x01\x86EtL\x85\
+\x00\x00\x09\x5c\x00\x00\x00\x00\x00\x01\x00\x00\x8f\xa0\
+\x00\x00\x01\x86Es\xbc\x83\
+\x00\x00\x0a\x0e\x00\x00\x00\x00\x00\x01\x00\x00\x9bN\
+\x00\x00\x01\x86Es\xf0\x9f\
+\x00\x00\x01\x84\x00\x00\x00\x00\x00\x01\x00\x00\x13B\
+\x00\x00\x01\x86Et\x87\xca\
+\x00\x00\x06\xa2\x00\x00\x00\x00\x00\x01\x00\x00`p\
+\x00\x00\x01\x86Et\x1f\x00\
+\x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\x0a\xb2\
+\x00\x00\x01\x86Es\xe4:\
+\x00\x00\x02\xd4\x00\x00\x00\x00\x00\x01\x00\x00%\xc1\
+\x00\x00\x01\x86EtO)\
+\x00\x00\x07,\x00\x00\x00\x00\x00\x01\x00\x00g\x91\
+\x00\x00\x01\x86Es\xdc)\
+\x00\x00\x08*\x00\x00\x00\x00\x00\x01\x00\x00z\xea\
+\x00\x00\x01\x86EtJ\x11\
+\x00\x00\x07X\x00\x00\x00\x00\x00\x01\x00\x00jB\
+\x00\x00\x01\x86Et\x0d\x91\
+\x00\x00\x01\xde\x00\x00\x00\x00\x00\x01\x00\x00\x16\x99\
+\x00\x00\x01\x86Ett\x96\
+\x00\x00\x00^\x00\x00\x00\x00\x00\x01\x00\x00\x03\xa6\
+\x00\x00\x01\x86Es\xec'\
+\x00\x00\x04\x5c\x00\x00\x00\x00\x00\x01\x00\x009\xaf\
+\x00\x00\x01\x86Et\x1f\x0f\
+\x00\x00\x00,\x00\x00\x00\x00\x00\x01\x00\x00\x01\xda\
+\x00\x00\x01\x86Es\xa2\xf3\
+\x00\x00\x012\x00\x00\x00\x00\x00\x01\x00\x00\x0e\x80\
+\x00\x00\x01\x86Et7\x22\
+\x00\x00\x06\xd0\x00\x00\x00\x00\x00\x01\x00\x00bW\
+\x00\x00\x01\x86Eto_\
+\x00\x00\x06Z\x00\x00\x00\x00\x00\x01\x00\x00[\xa5\
+\x00\x00\x01\x86Es\xacM\
+\x00\x00\x0b*\x00\x00\x00\x00\x00\x01\x00\x00\xb2\x16\
+\x00\x00\x01\x86Es\xecd\
+\x00\x00\x0a:\x00\x00\x00\x00\x00\x01\x00\x00\x9d\x86\
+\x00\x00\x01\x86Et%#\
+\x00\x00\x05\xee\x00\x00\x00\x00\x00\x01\x00\x00R\x14\
+\x00\x00\x01\x86Et7q\
+\x00\x00\x05\xc4\x00\x00\x00\x00\x00\x01\x00\x00O\x8a\
+\x00\x00\x01\x86Es\xac\x9d\
+\x00\x00\x09\xec\x00\x00\x00\x00\x00\x01\x00\x00\x98f\
+\x00\x00\x01\x86Es\xab\x07\
+\x00\x00\x0bz\x00\x00\x00\x00\x00\x01\x00\x00\xb72\
+\x00\x00\x01\x86Et\x16.\
+\x00\x00\x09\x8e\x00\x00\x00\x00\x00\x01\x00\x00\x92s\
+\x00\x00\x01\x86Et\x87\xec\
+\x00\x00\x020\x00\x00\x00\x00\x00\x01\x00\x00\x1b\x81\
+\x00\x00\x01\x86EtL\xc8\
+\x00\x00\x04\xc8\x00\x00\x00\x00\x00\x01\x00\x00?t\
+\x00\x00\x01\x86EtL\xb7\
+\x00\x00\x02\x12\x00\x00\x00\x00\x00\x01\x00\x00\x18|\
+\x00\x00\x01\x86EtI\x1b\
+\x00\x00\x05*\x00\x00\x00\x00\x00\x01\x00\x00E*\
+\x00\x00\x01\x86Es\xa8\xee\
+\x00\x00\x048\x00\x00\x00\x00\x00\x01\x00\x007\xaa\
+\x00\x00\x01\x86Et\x1fQ\
+\x00\x00\x04\x90\x00\x00\x00\x00\x00\x01\x00\x00<6\
+\x00\x00\x01\x86Es\xa8\xad\
+\x00\x00\x03P\x00\x00\x00\x00\x00\x01\x00\x00,\xc6\
+\x00\x00\x01\x86Et\x87\xbd\
+\x00\x00\x07\xd4\x00\x00\x00\x00\x00\x01\x00\x00r\x87\
+\x00\x00\x01\x86EtM\x91\
+\x00\x00\x0a\xd8\x00\x00\x00\x00\x00\x01\x00\x00\xacv\
+\x00\x00\x01\x86Es\xec=\
+\x00\x00\x09\x0e\x00\x00\x00\x00\x00\x01\x00\x00\x8b\x0f\
+\x00\x00\x01\x86Es\xe1\xfc\
+\x00\x00\x02\xb0\x00\x00\x00\x00\x00\x01\x00\x00#\x02\
+\x00\x00\x01\x86Es\xb6\x88\
+\x00\x00\x05\xac\x00\x00\x00\x00\x00\x01\x00\x00MS\
+\x00\x00\x01\x86Eth}\
+\x00\x00\x06\xf8\x00\x00\x00\x00\x00\x01\x00\x00d\x94\
+\x00\x00\x01\x86Et\x1e\xef\
+\x00\x00\x00\x10\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x01\x86Es\xe4_\
+\x00\x00\x0aP\x00\x00\x00\x00\x00\x01\x00\x00\xa3\x89\
+\x00\x00\x01\x86Et7\x02\
+\x00\x00\x066\x00\x00\x00\x00\x00\x01\x00\x00Y\xe3\
+\x00\x00\x01\x86Et6\xb7\
+\x00\x00\x08\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x85\xfc\
+\x00\x00\x01\x86Et\x04E\
+\x00\x00\x09\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x94)\
+\x00\x00\x01\x86Es\xac\xbe\
+\x00\x00\x04\xfc\x00\x00\x00\x00\x00\x01\x00\x00B1\
+\x00\x00\x01\x86Eti\xaa\
+\x00\x00\x03\xce\x00\x00\x00\x00\x00\x01\x00\x003\xd9\
+\x00\x00\x01\x86Et\x87\xae\
+\x00\x00\x09\xc6\x00\x00\x00\x00\x00\x01\x00\x00\x96\xaf\
+\x00\x00\x01\x86Ett\x87\
+\x00\x00\x08\x9a\x00\x00\x00\x00\x00\x01\x00\x00\x83h\
+\x00\x00\x01\x86Es\xad}\
+\x00\x00\x098\x00\x00\x00\x00\x00\x01\x00\x00\x8dG\
+\x00\x00\x01\x86Et6\xc5\
+\x00\x00\x0b\x02\x00\x00\x00\x00\x00\x01\x00\x00\xaf\x12\
+\x00\x00\x01\x86EtH\xec\
+\x00\x00\x00\xb6\x00\x00\x00\x00\x00\x01\x00\x00\x08\xb6\
+\x00\x00\x01\x86Es\xc7\x0d\
+\x00\x00\x02X\x00\x00\x00\x00\x00\x01\x00\x00\x1d\x88\
+\x00\x00\x01\x86EtF\xe0\
+\x00\x00\x01^\x00\x00\x00\x00\x00\x01\x00\x00\x10\xb7\
+\x00\x00\x01\x86EtS\xdc\
+\x00\x00\x03\x10\x00\x00\x00\x00\x00\x01\x00\x00*P\
+\x00\x00\x01\x86Es\xb9@\
+\x00\x00\x08H\x00\x00\x00\x00\x00\x01\x00\x00}\xec\
+\x00\x00\x01\x86EtP\xd0\
+\x00\x00\x00\x8c\x00\x00\x00\x00\x00\x01\x00\x00\x06c\
+\x00\x00\x01\x86Es\xdc\x86\
+\x00\x00\x0at\x00\x00\x00\x00\x00\x01\x00\x00\xa5O\
+\x00\x00\x01\x86EtT=\
+\x00\x00\x06|\x00\x00\x00\x00\x00\x01\x00\x00^\x12\
+\x00\x00\x01\x86Et\x18\x1e\
+\x00\x00\x0a\xa2\x00\x00\x00\x00\x00\x01\x00\x00\xa7\x7f\
+\x00\x00\x01\x86EtB\x03\
+\x00\x00\x03t\x00\x00\x00\x00\x00\x01\x00\x00.\xe1\
+\x00\x00\x01\x86Etch\
+\x00\x00\x0bV\x00\x00\x00\x00\x00\x01\x00\x00\xb4\xb8\
+\x00\x00\x01\x86Et7a\
+\x00\x00\x02\xec\x00\x00\x00\x00\x00\x01\x00\x00(4\
+\x00\x00\x01\x86EtS\x9a\
+\x00\x00\x01\xa8\x00\x00\x00\x00\x00\x01\x00\x00\x14\xd3\
+\x00\x00\x01\x86Et\x1f \
+\x00\x00\x03\xa2\x00\x00\x00\x00\x00\x01\x00\x001\x03\
+\x00\x00\x01\x86Es\xec\x88\
+\x00\x00\x08\x02\x00\x00\x00\x00\x00\x01\x00\x00xQ\
+\x00\x00\x01\x86Es\xf7\x97\
+"
+
+def qInitResources():
+    QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
+
+def qCleanupResources():
+    QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
+
+qInitResources()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `revolution-eda-0.4.1/revinit.py` & `revolution-eda-0.5.0/revinit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-#  “Commons Clause” License Condition v1.0
-#
-#  The Software is provided to you by the Licensor under the License, as defined
-#  below, subject to the following condition.
-#
-#  Without limiting other conditions in the License, the grant of rights under the
-#  License will not include, and the License does not grant to you, the right to
-#  Sell the Software.
-#
-#  For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#  granted to you under the License to provide to third parties, for a fee or other
-#  consideration (including without limitation fees for hosting or consulting/
-#  support services related to the Software), a product or service whose value
-#  derives, entirely or substantially, from the functionality of the Software. Any
-#  license notice or attribution required by the License must also include this
-#  Commons Clause License Condition notice.
-#
-#  Software: Revolution EDA
-#  License: Mozilla Public License 2.0
-#  Licensor: Revolution Semiconductor (Registered in the Netherlands)
-#
-
-import sys
-import pathlib
-# version
-__version__ = "0.4.1"
-#import revedaeditor.pdk.callbacks as cb
+#  “Commons Clause” License Condition v1.0
+#
+#  The Software is provided to you by the Licensor under the License, as defined
+#  below, subject to the following condition.
+#
+#  Without limiting other conditions in the License, the grant of rights under the
+#  License will not include, and the License does not grant to you, the right to
+#  Sell the Software.
+#
+#  For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#  granted to you under the License to provide to third parties, for a fee or other
+#  consideration (including without limitation fees for hosting or consulting/
+#  support services related to the Software), a product or service whose value
+#  derives, entirely or substantially, from the functionality of the Software. Any
+#  license notice or attribution required by the License must also include this
+#  Commons Clause License Condition notice.
+#
+#  Software: Revolution EDA
+#  License: Mozilla Public License 2.0
+#  Licensor: Revolution Semiconductor (Registered in the Netherlands)
+#
+
+
+# version
+__version__ = "0.5.0"
```

