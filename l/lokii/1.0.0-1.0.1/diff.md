# Comparing `tmp/lokii-1.0.0.tar.gz` & `tmp/lokii-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokii-1.0.0.tar", last modified: Sat May 27 12:40:34 2023, max compression
+gzip compressed data, was "lokii-1.0.1.tar", last modified: Wed May 31 14:39:28 2023, max compression
```

## Comparing `lokii-1.0.0.tar` & `lokii-1.0.1.tar`

### file list

```diff
@@ -1,64 +1,68 @@
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-26 20:12:04.000000 lokii-1.0.0/LICENSE
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     5858 2023-05-27 12:40:34.816118 lokii-1.0.0/PKG-INFO
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4748 2023-05-27 12:36:19.000000 lokii-1.0.0/README.md
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        5 2023-05-26 20:12:04.000000 lokii-1.0.0/VERSION
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.812118 lokii-1.0.0/lokii/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       55 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       78 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/__main__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3224 2023-05-27 12:02:33.000000 lokii-1.0.0/lokii/cli.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2084 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/config.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.812118 lokii-1.0.0/lokii/exec/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/exec/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2679 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/exec/gen_executor.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.812118 lokii-1.0.0/lokii/logger/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/logger/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1238 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/logger/color.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1756 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/logger/context.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      662 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/logger/formatter.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      639 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/logger/progress.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4201 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/main.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.812118 lokii-1.0.0/lokii/model/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/model/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1514 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/model/gen_module.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/lokii/parse/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/parse/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      985 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/parse/graph_analyzer.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3451 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/parse/node_parser.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/lokii/storage/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/storage/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4330 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/storage/data_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      844 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/storage/temp_storage.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/lokii/util/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/util/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1279 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/util/module_file_loader.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      610 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/util/perf_timer_context.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.812118 lokii-1.0.0/lokii.egg-info/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     5858 2023-05-27 12:40:34.000000 lokii-1.0.0/lokii.egg-info/PKG-INFO
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1190 2023-05-27 12:40:34.000000 lokii-1.0.0/lokii.egg-info/SOURCES.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-27 12:40:34.000000 lokii-1.0.0/lokii.egg-info/dependency_links.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       45 2023-05-27 12:40:34.000000 lokii-1.0.0/lokii.egg-info/entry_points.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2021-03-08 06:45:18.000000 lokii-1.0.0/lokii.egg-info/not-zip-safe
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      110 2023-05-27 12:40:34.000000 lokii-1.0.0/lokii.egg-info/requires.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       12 2023-05-27 12:40:34.000000 lokii-1.0.0/lokii.egg-info/top_level.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       38 2023-05-27 12:40:34.816118 lokii-1.0.0/setup.cfg
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1852 2023-05-27 12:39:37.000000 lokii-1.0.0/setup.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/tests/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1815 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/conftest.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/tests/exec/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/exec/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1142 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/exec/test_gen_executor.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/tests/parse/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/parse/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1474 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/parse/test_graph_analyzer.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3920 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/parse/test_node_parser.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/tests/storage/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/storage/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3844 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/storage/test_data_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      369 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/storage/test_temp_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4841 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/test_cli.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/tests/util/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/util/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1007 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/util/test_module_file_loader.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      629 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/util/test_perf_timer_context.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.861541 lokii-1.0.1/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-26 20:12:04.000000 lokii-1.0.1/LICENSE
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     5407 2023-05-31 14:39:28.861541 lokii-1.0.1/PKG-INFO
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4297 2023-05-31 14:39:03.000000 lokii-1.0.1/README.md
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        5 2023-05-31 14:39:03.000000 lokii-1.0.1/VERSION
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       55 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       78 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/__main__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3309 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/cli.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2287 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/config.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/exec/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/exec/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2620 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/exec/node_executor.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/logger/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/logger/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1268 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/logger/color.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1756 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/logger/context.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      664 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/logger/formatter.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      639 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/logger/progress.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4466 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/main.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/model/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/model/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      730 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/model/group_module.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/model/node_module.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/parse/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/parse/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      709 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/parse/base_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2776 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/parse/group_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2783 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/parse/node_parser.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/storage/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/storage/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4529 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/storage/data_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      835 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/storage/temp_storage.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii/util/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/util/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2160 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/util/graph_analyzer.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1464 2023-05-31 14:39:03.000000 lokii-1.0.1/lokii/util/module_file_loader.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      610 2023-05-26 20:12:04.000000 lokii-1.0.1/lokii/util/perf_timer_context.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/lokii.egg-info/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     5407 2023-05-31 14:39:28.000000 lokii-1.0.1/lokii.egg-info/PKG-INFO
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1307 2023-05-31 14:39:28.000000 lokii-1.0.1/lokii.egg-info/SOURCES.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-31 14:39:28.000000 lokii-1.0.1/lokii.egg-info/dependency_links.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       45 2023-05-31 14:39:28.000000 lokii-1.0.1/lokii.egg-info/entry_points.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2021-03-08 06:45:18.000000 lokii-1.0.1/lokii.egg-info/not-zip-safe
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       71 2023-05-31 14:39:28.000000 lokii-1.0.1/lokii.egg-info/requires.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       12 2023-05-31 14:39:28.000000 lokii-1.0.1/lokii.egg-info/top_level.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       38 2023-05-31 14:39:28.861541 lokii-1.0.1/setup.cfg
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1788 2023-05-31 14:39:03.000000 lokii-1.0.1/setup.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/tests/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2451 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/conftest.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/tests/exec/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/exec/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1098 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/exec/test_node_executor.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.857541 lokii-1.0.1/tests/parse/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/parse/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1635 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/parse/test_group_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3165 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/parse/test_node_parser.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.861541 lokii-1.0.1/tests/storage/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/storage/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4091 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/storage/test_data_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      369 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/storage/test_temp_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4211 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/test_cli.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-31 14:39:28.861541 lokii-1.0.1/tests/util/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/util/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      953 2023-05-31 14:39:03.000000 lokii-1.0.1/tests/util/test_graph_analyzer.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1007 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/util/test_module_file_loader.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      629 2023-05-26 20:12:04.000000 lokii-1.0.1/tests/util/test_perf_timer_context.py
```

### Comparing `lokii-1.0.0/LICENSE` & `lokii-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lokii-1.0.0/lokii/cli.py` & `lokii-1.0.1/lokii/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 import argparse
 import logging
 import sys
 
-from pathlib import Path
-from typing import Optional
-
 from lokii import Lokii
 from lokii.logger.context import LoggingContext
 from lokii.config import CONFIG
 
 LOKII_ASCII = r"""
- __         ______     __  __     __     __    
-/\ \       /\  __ \   /\ \/ /    /\ \   /\ \   
-\ \ \____  \ \ \/\ \  \ \  _"-.  \ \ \  \ \ \  
- \ \_____\  \ \_____\  \ \_\ \_\  \ \_\  \ \_\ 
-  \/_____/   \/_____/   \/_/\/_/   \/_/   \/_/ 
+▄▄▄▄▄   ▄▄▄▄▄▄▄▄▄▄▄▄▄ ▄▄▄▄▄▄▄▄▄▄▄
+█   █   █       █   █ █ █   █   █
+█   █   █   ▄   █   █▄█ █   █   █
+█   █   █  █ █  █      ▄█   █   █
+█   █▄▄▄█  █▄█  █     █▄█   █   █
+█       █       █    ▄  █   █   █
+█▄▄▄▄▄▄▄█▄▄▄▄▄▄▄█▄▄▄█ █▄█▄▄▄█▄▄▄█ 
 """
-LOKII_EPILOG = f""""""
 
 
 class Command:
-    def __init__(self, argv: Optional[str] = None) -> None:
+    def __init__(self, argv=None) -> None:
         self.argv = argv.split() if argv else sys.argv[:]
-        self.prog_name = Path(self.argv[0]).name
+        self.prog_name = "lokii"
 
     def execute(self) -> None:
         """
         Given the command-line arguments, this creates a parser appropriate
         to that command, and runs it.
         """
 
         formatter_class = argparse.RawDescriptionHelpFormatter
         parser = argparse.ArgumentParser(
             prog=self.prog_name,
-            description=f"{LOKII_ASCII}\n{self.prog_name} version {CONFIG.version}",
-            epilog=LOKII_EPILOG,
+            description="%s\n%s version %s"
+            % (LOKII_ASCII, self.prog_name, CONFIG.version),
             formatter_class=formatter_class,
         )
 
         parser.add_argument(
-            "--version", action="version", version=f"%(prog)s {CONFIG.version}"
+            "--version", action="version", version="%(prog)s " + CONFIG.version
         )
 
         parser.add_argument(
             "-v",
             "--verbose",
             action="store_true",
             help="set logging level to DEBUG that shows all events",
@@ -103,11 +101,11 @@
                 print(LOKII_ASCII)
                 lokii_gen = Lokii(arguments.source_folder, arguments.out_folder)
                 lokii_gen.generate(arguments.purge)
             except Exception as err:
                 logging.critical(str(err), exc_info=True)
 
 
-def exec_cmd(argv: Optional[str] = None) -> None:
+def exec_cmd(argv=None) -> None:
     """A simple method that runs a Command."""
     command = Command(argv)
     command.execute()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lokii-1.0.0/lokii/config.py` & `lokii-1.0.1/lokii/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,64 @@
-import os
-from pathlib import Path
+from os import path, environ, cpu_count
 
-root = Path(__file__).resolve().parent.parent
+root = path.dirname(path.dirname(__file__))
 # read app version from root of the project
-VERSION = (root / "VERSION").read_text(encoding="utf-8").strip()
+f = open(path.join(root, "VERSION"), "r")
+VERSION = f.read().strip()
+f.close()
 
 # temp directory that contains generated runtime files and database
-TEMP_DIR_PATH = os.environ.get("LOKII__TEMP_DIR_PATH", ".temp")
+TEMP_DIR_PATH = environ.get("LOKII__TEMP_DIR_PATH", ".temp")
 # duckdb database that stores generated data in relational tables
-TEMP_DB_FILE = os.environ.get("LOKII__TEMP_DB_FILE", "lokii.duckdb")
+TEMP_DB_FILE = environ.get("LOKII__TEMP_DB_FILE", "lokii.duckdb")
 # name of the temp data file that contains generated runtime files
-TEMP_DATA_DIR = os.environ.get("LOKII__TEMP_DATA_DIR", "data")
+TEMP_DATA_DIR = environ.get("LOKII__TEMP_DATA_DIR", "data")
 
-# file extension to look for when finding generation config files
-GEN_FILE_EXT = os.environ.get("LOKII__GEN_FILE_EXT", ".gen.py")
+# file extension to look for when finding generation node files
+GEN_NODE_EXT = environ.get("LOKII__GEN_NODE_EXT", ".node.py")
+# file extension to look for when finding generation group files
+GEN_GROUP_EXT = environ.get("LOKII__GEN_GROUP_EXT", ".group.py")
 # -
-GEN_CONCURRENCY = os.environ.get("LOKII__GEN_CONCURRENCY", os.cpu_count())
+GEN_CONCURRENCY = environ.get("LOKII__GEN_CONCURRENCY", cpu_count())
 # -
-GEN_BATCH_SIZE = os.environ.get("LOKII__GEN_BATCH_SIZE", 100_000)
+GEN_BATCH_SIZE = environ.get("LOKII__GEN_BATCH_SIZE", 100000)
 # -
-GEN_CHUNK_SIZE = os.environ.get("LOKII__GEN_CHUNK_SIZE", 200)
+GEN_CHUNK_SIZE = environ.get("LOKII__GEN_CHUNK_SIZE", 200)
 
 
 class __Config:
     class __TempConfig:
         """
         Global configuration for storing temp file paths.
         """
 
         @property
         def dir_path(self) -> str:
             return TEMP_DIR_PATH
 
         @property
         def db_path(self) -> str:
-            return os.path.join(TEMP_DIR_PATH, TEMP_DB_FILE)
+            return path.join(TEMP_DIR_PATH, TEMP_DB_FILE)
 
         @property
         def data_path(self) -> str:
-            return os.path.join(TEMP_DIR_PATH, TEMP_DATA_DIR)
+            return path.join(TEMP_DIR_PATH, TEMP_DATA_DIR)
 
     class __GenConfig:
         """
         Global configuration for storing generation information.
         """
 
         @property
-        def file_ext(self) -> str:
-            return GEN_FILE_EXT
+        def node_ext(self) -> str:
+            return GEN_NODE_EXT
+
+        @property
+        def group_ext(self) -> str:
+            return GEN_GROUP_EXT
 
         @property
         def concurrency(self) -> int:
             return int(GEN_CONCURRENCY)
 
         @property
         def batch_size(self) -> int:
```

### Comparing `lokii-1.0.0/lokii/exec/gen_executor.py` & `lokii-1.0.1/lokii/exec/node_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-from __future__ import annotations
-
 import math
 from functools import partial
 from typing import Callable
+
 from pathos.pools import ProcessPool
 
 from lokii.config import CONFIG
+from lokii.model.node_module import GenNodeModule
 from lokii.logger.progress import ProgressLogger
-from lokii.model.gen_module import GenRun
 from lokii.storage.data_storage import DataStorage
 from lokii.storage.temp_storage import TempStorage
 
 
 def _exec_chunk(func: Callable, args: list[dict]):
     return [func(arg) for arg in args]
 
 
-class GenExecutor:
-    def __init__(self, run: GenRun, data_storage: DataStorage):
+class NodeExecutor:
+    def __init__(self, node: GenNodeModule, data_storage: DataStorage):
         """
         Reads and validates dataset configuration from filesystem structure.
 
-        :param run: root path of the dataset generation
+        :param node: root path of the dataset generation
         :param data_storage: root path of the dataset generation
         """
-        self.run = run
+        self.run = node
         self.data_storage = data_storage
-        self.__temp_storage = TempStorage(self.run.node_name)
-        self.__logger: ProgressLogger
+        self.__temp_storage = TempStorage(self.run.name)
 
         # total times the gen function will be called
         self.t_count = 0
         # total generated item count
         self.g_count = 0
 
     def prepare_node(self) -> int:
@@ -63,12 +61,12 @@
         # return generated file paths
         return self.__temp_storage.batches
 
     def _exec_batch(self, args: list[dict]) -> list[dict]:
         chunk_size = CONFIG.gen.chunk_size
         chunk_args = [args[i : i + chunk_size] for i in range(0, len(args), chunk_size)]
 
-        gen_func = partial(_exec_chunk, self.run.func)
+        gen_func = partial(_exec_chunk, self.run.item)
         with ProcessPool(nodes=CONFIG.gen.concurrency) as pool:
             for chunk in pool.uimap(gen_func, chunk_args):
                 # remove null items from generated chunk
                 yield [i for i in chunk if i is not None]
```

### Comparing `lokii-1.0.0/lokii/logger/color.py` & `lokii-1.0.1/lokii/logger/color.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,19 +22,20 @@
 _ansi_reset_all = "\033[0m"
 
 
 def style(
     text: str, fg: str = None, bg: str = None, bold: bool = False, reset: bool = True
 ):
     bits = []
+    bit_temp = "\033[%dm"
     if fg:
-        bits.append(f"\033[{_ansi_colors[fg]}m")
+        bits.append(bit_temp % _ansi_colors[fg])
     if bg:
-        bits.append(f"\033[{_ansi_colors[bg] + 10}m")
-    bits.append(f"\033[{1 if bold else 22}m")
+        bits.append(bit_temp % (_ansi_colors[bg] + 10))
+    bits.append(bit_temp % (1 if bold else 22))
     bits.append(text)
     if reset:
         bits.append(_ansi_reset_all)
     return "".join(bits)
 
 
 default_formats = {
```

### Comparing `lokii-1.0.0/lokii/logger/context.py` & `lokii-1.0.1/lokii/logger/context.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.0/lokii/logger/formatter.py` & `lokii-1.0.1/lokii/logger/formatter.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 
 
 class MultiFormatter(Formatter):
     """Format log messages differently for each log level"""
 
     def __init__(self, formats: dict[int, str] = None, **kwargs):
         base_format = kwargs.pop("fmt", None)
-        super().__init__(base_format, **kwargs)
+        super(MultiFormatter, self).__init__(base_format, **kwargs)
         fmts = formats or default_formats
         self.formatters = {lvl: Formatter(fmt, **kwargs) for lvl, fmt in fmts.items()}
 
-    def format(self, record: LogRecord):
-        formatter = self.formatters.get(record.levelno)
-        return super().format(record) if formatter is None else formatter.format(record)
+    def format(self, r: LogRecord):
+        fmt = self.formatters.get(r.levelno)
+        return super(MultiFormatter, self).format(r) if fmt is None else fmt.format(r)
```

### Comparing `lokii-1.0.0/lokii/logger/progress.py` & `lokii-1.0.1/lokii/logger/progress.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.0/lokii/main.py` & `lokii-1.0.1/lokii/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 import os
 import shutil
 import uuid
 
 from lokii.config import CONFIG
-from lokii.model.gen_module import GenRun
-from lokii.parse.node_parser import NodeParser
-from lokii.parse.graph_analyzer import GraphAnalyzer
 from lokii.storage.data_storage import DataStorage
-from lokii.exec.gen_executor import GenExecutor
+from lokii.model.node_module import GenNodeModule
+from lokii.parse.node_parser import NodeParser
+from lokii.parse.group_parser import GroupParser
 from lokii.util.perf_timer_context import PerfTimerContext
+from lokii.util.graph_analyzer import GraphAnalyzer
+from lokii.exec.node_executor import NodeExecutor
 
 
 class Lokii:
     def __init__(self, source_folder: str, out_folder: str):
         """
         Generates massive amount of relational mock data.
 
@@ -22,67 +23,73 @@
         """
         self.__source_folder = source_folder
         self.__out_folder = out_folder
         self.__gen_id = str(uuid.uuid4())
 
         Lokii.setup_env()
         self.__data_storage = DataStorage()
-        self.__gen_parser = NodeParser(self.__source_folder)
+        self.__node_parser = NodeParser(self.__source_folder)
+        self.__group_parser = GroupParser(self.__source_folder)
 
     def generate(self, purge: bool = False):
         with PerfTimerContext() as t:
-            gen_runs = self.__gen_parser.parse()
-            analyzer = GraphAnalyzer(list(gen_runs.values()))
-            run_exec_order = analyzer.execution_order()
+            nodes = self.__node_parser.parse()
+            # create dependency map from node source queries
+            dep_map = [
+                (n.name, [d for d in self.__data_storage.deps(n.source) if d in nodes])
+                for n in nodes.values()
+            ]
+            analyzer = GraphAnalyzer(dep_map)
+            exec_order = analyzer.execution_order()
 
             total_target_count, total_item_count = 0, 0
-            for run_key in run_exec_order:
-                run = gen_runs[run_key]
-                dep_keys = analyzer.dependencies(run_key)
-                if self.is_dataset_valid(run, dep_keys):
-                    logging.info(f"{run_key} not changed. Using existing dataset.")
+            for name in exec_order:
+                run = nodes[name]
+                dep_keys = analyzer.dependencies(name)
+                if self.is_node_valid(run, dep_keys):
+                    logging.info("%s not changed. Using existing dataset." % name)
                     continue
 
                 # generate dataset
-                target_count, item_count, file_paths = self.generate_dataset(run)
+                target_count, item_count, file_paths = self.generate_node(run)
                 total_target_count += target_count
                 total_item_count += item_count
 
                 # save generation metadata in database
-                self.__data_storage.save(self.__gen_id, run.run_key, run.node_version)
+                self.__data_storage.save(self.__gen_id, run.name, run.version)
                 # insert generated data in database
-                self.__data_storage.insert(run.node_name, file_paths)
+                self.__data_storage.insert(run.name, file_paths)
 
         logging.info("Generation completed!")
         logging.info("Total target item count: {:,}".format(total_target_count))
         logging.info("Generated {:,} items in {}".format(total_item_count, t))
         self.__data_storage.export(self.__out_folder, "csv")
         Lokii.clean_env(purge)
 
-    def generate_dataset(self, gen_run: GenRun) -> (int, int, list[str]):
+    def generate_node(self, node: GenNodeModule) -> (int, int, list[str]):
         with PerfTimerContext() as t:
-            logger = logging.getLogger(gen_run.run_key)
+            logger = logging.getLogger(node.name)
 
-            executor = GenExecutor(gen_run, self.__data_storage)
+            executor = NodeExecutor(node, self.__data_storage)
             target_count = executor.prepare_node()
 
             logger.info("Generation started for target {:,} items".format(target_count))
             generated_file_paths = executor.exec_node()
             item_count = executor.g_count
 
         logger.info("{:,} items generated in {}".format(item_count, t))
         return target_count, item_count, generated_file_paths
 
-    def is_dataset_valid(self, run: GenRun, dep_keys: list[str]):
-        metadata = self.__data_storage.meta([*dep_keys, run.run_key])
-        curr = [m for m in metadata if m["run_key"] == run.run_key]
+    def is_node_valid(self, node: GenNodeModule, dep_keys: list[str]):
+        metadata = self.__data_storage.meta(dep_keys)
+        curr = [m for m in metadata if m["name"] == node.name]
         if len(curr) == 0:
             # no dataset generated before with this run key
             return False  # must generate
-        if curr[0]["version"] != run.node_version:
+        if curr[0]["version"] != node.version:
             # code version is different from previous run
             return False  # must regenerate
         for dep_meta in metadata:
             if dep_meta["gen_id"] == self.__gen_id:
                 # dependent dataset changed in current generation
                 return False  # must regenerate
         # no code changes, no dependencies changed
```

### Comparing `lokii-1.0.0/lokii/storage/data_storage.py` & `lokii-1.0.1/lokii/storage/data_storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,76 +2,78 @@
 from functools import partial
 
 import duckdb
 from typing import TypedDict
 
 from lokii.config import CONFIG
 
-CONN: duckdb.DuckDBPyConnection
+CONN = None  #: duckdb.DuckDBPyConnection
 
-
-class NodeMetadata(TypedDict):
-    run_key: str
-    version: str
-    gen_id: str
+NodeMetadata = TypedDict("NodeMetadata", {"name": str, "version": str, "gen_id": str})
 
 
 class DataStorage:
     def __init__(self):
         """
         Temporary filesystem storage implementation for storing data generated between batches.
         It only stores data temporary and deletes all files after
         """
         self.connect = partial(duckdb.connect, database=CONFIG.temp.db_path)
         with self.connect() as conn:
             # create node meta table to store run generation information
             q = (
-                "CREATE TABLE IF NOT EXISTS main.__meta"
-                "(run_key TEXT, version TEXT, gen_id TEXT, PRIMARY KEY(run_key));"
+                "CREATE TABLE IF NOT EXISTS __meta"
+                "(name TEXT, version TEXT, gen_id TEXT, PRIMARY KEY(name));"
             )
             conn.execute(q).fetchall()
 
+    def deps(self, query: str) -> list:
+        with self.connect() as conn:
+            names = conn.get_table_names(query)
+            return list(names)
+
     def count(self, query: str) -> int:
         with self.connect() as conn:
-            q = f"WITH _t AS ({query}) SELECT COUNT() FROM _t;"
+            q = "WITH _t AS (%s) SELECT COUNT() FROM _t;" % query
             (count,) = conn.execute(q).fetchone()
             return count
 
     def exec(self, query: str, index: int, size: int) -> list[dict]:
         with self.connect() as conn:
-            q = f"WITH _t AS ({query}) SELECT * FROM _t LIMIT {size} OFFSET {index * size};"
-            data = conn.execute(q).df()
+            args = (query, size, index * size)
+            q = "WITH _t AS (%s) SELECT * FROM _t LIMIT %d OFFSET %d;" % args
+            data = conn.execute(q).fetch_df()
             return data.to_dict("records")
 
-    def save(self, gen_id: str, run_key: str, version: str) -> None:
+    def save(self, gen_id: str, name: str, version: str) -> None:
         """
         Generation id and node version will be stored in a meta table that can be used to check
         if gen run data is valid for consecutive runs.
 
         :param gen_id: identification of the generation process
-        :param run_key: identification of the generation run
-        :param version: node version of the module
+        :param name: identification of the node
+        :param version: the code version of the module
         """
         with self.connect() as conn:
-            q = f"""
-            INSERT OR REPLACE INTO main.__meta(run_key, version, gen_id)
-            VALUES ('{run_key}', '{version}', '{gen_id}');
+            q = """
+            INSERT OR REPLACE INTO __meta(name, version, gen_id)
+            VALUES ('%s', '%s', '%s');
             """
-            conn.execute(q).fetchall()
+            conn.execute(q % (name, version, gen_id)).fetchall()
 
-    def meta(self, run_keys: list[str]) -> list[NodeMetadata]:
+    def meta(self, names: list[str]) -> list[NodeMetadata]:
         """
         Fetches generation metadata information about given runs.
-        :param run_keys: list of run ids
+        :param names: list of node names
         :return: list of node meta dict
         """
         with self.connect() as conn:
-            keys = ",".join([f"'{k}'" for k in run_keys])
-            q = f"SELECT run_key, version, gen_id FROM main.__meta WHERE run_key IN ({keys});"
-            data = conn.execute(q).df()
+            keys = ",".join(["'%s'" % n for n in names])
+            q = "SELECT name, version, gen_id FROM __meta WHERE name IN (%s);"
+            data = conn.execute(q % keys).fetch_df()
             return data.to_dict("records")
 
     def insert(self, name: str, files: list[str]) -> None:
         """
         Creates a table for given node name in local relational database. If there is a table
         with the same node name it will drop all data and create a fresh one. Given files will
         be concatenated and inserted in the fresh table.
@@ -80,20 +82,20 @@
         :param files: list of generated file paths
         """
         with self.connect() as conn:
             if "." in name:
                 # create schema if node name defines `schema.table` syntax
                 assert len(name.split(".")) == 2, "Nested schemas are not supported."
                 schema = name.split(".")[0]
-                q = f"CREATE SCHEMA IF NOT EXISTS {schema};"
-                conn.execute(q).fetchall()
+                q = "CREATE SCHEMA IF NOT EXISTS %s;"
+                conn.execute(q % schema).fetchall()
 
             # concatenate and insert file contents in a fresh table
-            q = f"CREATE OR REPLACE TABLE {name} AS SELECT * FROM read_json_auto({files});"
-            conn.execute(q).fetchall()
+            q = "CREATE OR REPLACE TABLE %s AS SELECT * FROM read_json_auto(%s);"
+            conn.execute(q % (name, files)).fetchall()
 
     def export(self, out_path: str, fmt: str) -> None:
         """
         Exports all generated tables to given file format.
 
         :param out_path: folder path of the exported files
         :param fmt: file format of the exported files
@@ -104,10 +106,10 @@
             tables = [f for (f,) in tables if "__meta" != f]
 
             # create out folder if not exists
             if not os.path.exists(out_path):
                 os.makedirs(out_path)
 
             for t in tables:
-                path = os.path.join(out_path, f"{t}.{fmt}")
+                path = os.path.join(out_path, ".".join([t, fmt]))
                 # export to output path
-                conn.execute(f"COPY {t} TO '{path}'").fetchone()
+                conn.execute("COPY %s TO '%s'" % (t, path)).fetchone()
```

### Comparing `lokii-1.0.0/lokii/storage/temp_storage.py` & `lokii-1.0.1/lokii/storage/temp_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     def __init__(self, node_name: str):
         """
         Temporary filesystem storage implementation for storing data generated between batches.
         It only stores data temporary and deletes all files after node generation completed.
         :param node_name: name of the node
         """
         self.node_name = node_name
-        self.batches: list[str] = []
+        self.batches = []
         self.item_count = 0
 
     def dump(self, batch_data: list[dict]) -> None:
         storage_key = self.node_name + str(len(self.batches))
-        storage_path = os.path.join(CONFIG.temp.data_path, f"{storage_key}.json")
+        storage_path = os.path.join(CONFIG.temp.data_path, "%s.json" % storage_key)
 
         with open(storage_path, "w") as _f:
             _f.write(json.dumps(batch_data))
 
         self.batches.append(storage_path)
         self.item_count = len(batch_data)
```

### Comparing `lokii-1.0.0/lokii/util/module_file_loader.py` & `lokii-1.0.1/lokii/util/module_file_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,51 @@
-from __future__ import annotations
-
 import os
 import sys
 import hashlib
 import inspect
 from types import ModuleType
-from importlib.util import spec_from_file_location, module_from_spec
 
 
 class ModuleFileLoader:
+    """
+    :type module: ModuleType or None
+    :type version: str or None
+    """
+
     def __init__(self, file_path: str):
         """
         Loads module from given path.
 
         :param file_path: file path of the module
         """
         self.path = os.path.abspath(file_path)
         self.filename = os.path.basename(file_path)
 
-        self.module: ModuleType | None = None
-        self.version: str | None = None
+        self.module = None
+        self.version = None
 
     def load(self) -> None:
         if not os.path.exists(self.path):
-            raise FileNotFoundError(f"No module file found at: {self.path}")
+            raise FileNotFoundError("No module file found at: %s" % self.path)
+
+        try:
+            import importlib.util
+
+            # read file spec from given path. filename is used as module name
+            spec = importlib.util.spec_from_file_location(self.filename, self.path)
+            module = importlib.util.module_from_spec(spec)
+
+            # introduce module to system
+            sys.modules[self.filename] = module
+            spec.loader.exec_module(module)
+            self.module = module
+        except ImportError:
+            from imp import load_source
 
-        # read file spec from given path. filename is used as module name
-        spec = spec_from_file_location(self.filename, self.path)
-        module = module_from_spec(spec)
-
-        # introduce module to system
-        sys.modules[self.filename] = module
-        spec.loader.exec_module(module)
-        self.module = module
+            module = load_source(self.filename, self.path)
 
         # acquire module source code as str
         src = inspect.getsource(module).encode("utf-8")
         h = hashlib.blake2b(digest_size=20)
         h.update(src)
 
         # hash source code to detect changes
```

### Comparing `lokii-1.0.0/lokii/util/perf_timer_context.py` & `lokii-1.0.1/lokii/util/perf_timer_context.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.0/lokii.egg-info/SOURCES.txt` & `lokii-1.0.1/lokii.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,38 +11,42 @@
 lokii.egg-info/SOURCES.txt
 lokii.egg-info/dependency_links.txt
 lokii.egg-info/entry_points.txt
 lokii.egg-info/not-zip-safe
 lokii.egg-info/requires.txt
 lokii.egg-info/top_level.txt
 lokii/exec/__init__.py
-lokii/exec/gen_executor.py
+lokii/exec/node_executor.py
 lokii/logger/__init__.py
 lokii/logger/color.py
 lokii/logger/context.py
 lokii/logger/formatter.py
 lokii/logger/progress.py
 lokii/model/__init__.py
-lokii/model/gen_module.py
+lokii/model/group_module.py
+lokii/model/node_module.py
 lokii/parse/__init__.py
-lokii/parse/graph_analyzer.py
+lokii/parse/base_parser.py
+lokii/parse/group_parser.py
 lokii/parse/node_parser.py
 lokii/storage/__init__.py
 lokii/storage/data_storage.py
 lokii/storage/temp_storage.py
 lokii/util/__init__.py
+lokii/util/graph_analyzer.py
 lokii/util/module_file_loader.py
 lokii/util/perf_timer_context.py
 tests/__init__.py
 tests/conftest.py
 tests/test_cli.py
 tests/exec/__init__.py
-tests/exec/test_gen_executor.py
+tests/exec/test_node_executor.py
 tests/parse/__init__.py
-tests/parse/test_graph_analyzer.py
+tests/parse/test_group_parser.py
 tests/parse/test_node_parser.py
 tests/storage/__init__.py
 tests/storage/test_data_storage.py
 tests/storage/test_temp_storage.py
 tests/util/__init__.py
+tests/util/test_graph_analyzer.py
 tests/util/test_module_file_loader.py
 tests/util/test_perf_timer_context.py
```

### Comparing `lokii-1.0.0/setup.py` & `lokii-1.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python
 
-from pathlib import Path
-
+from os import path
 from setuptools import setup, find_packages
 
-root = Path(__file__).resolve().parent
-VERSION = (root / "VERSION").read_text(encoding="utf-8").strip()
-README = (root / "README.md").read_text(encoding="utf-8")
+root = path.dirname(__file__)
+with open(path.join(root, "VERSION"), "r") as f:
+    VERSION = f.read().strip()
+with open(path.join(root, "README.md"), "r") as f:
+    README = f.read().strip()
 
 setup(
     name="lokii",
     version=VERSION,
     packages=find_packages(where="."),
     description="Generate, Load, Develop and Test with consistent relational datasets!",
     long_description=README,
@@ -31,25 +32,22 @@
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
         "Typing :: Typed",
     ],
     author="Doruk Eren Aktaş",
     author_email="dorukerenaktas@gmail.com",
-    py_modules=["lokii"],
     entry_points={
         "console_scripts": ["lokii=lokii.cli:exec_cmd"],
     },
     url="https://github.com/dorukerenaktas/lokii",
     data_files=[("", ["VERSION"])],
     install_requires=[
         "pandas==2.0.1",
         "pathos==0.3.0",
-        "networkx==3.1",
         "tqdm==4.65.0",
         "duckdb==0.8.0",
         "typing==3.7.4.3",
-        "typing-extensions==4.6.2",
     ],
     license="MIT License",
     zip_safe=False,
 )
```

### Comparing `lokii-1.0.0/tests/exec/test_gen_executor.py` & `lokii-1.0.1/tests/exec/test_node_executor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 from unittest.mock import Mock
 
 import pytest
 import os
 
-from lokii.model.gen_module import GenRun, GenRunConf
 from lokii.storage.data_storage import DataStorage
-from lokii.exec.gen_executor import GenExecutor, _exec_chunk
-
-conf: GenRunConf = {"source": "SELECT 1", "wait": [], "func": lambda x: x}
+from lokii.exec.node_executor import NodeExecutor, _exec_chunk
+from lokii.model.node_module import GenNodeModule
 
 
 @pytest.mark.usefixtures("setup_test_env")
 def test__exec_chunk_should_call_func_for_list_length():
     func = Mock()
     _exec_chunk(func, [{"data": f} for f in range(100)])
     assert func.call_count == 100
 
 
 @pytest.mark.usefixtures("setup_test_env")
 def test_prepare_node_should_return_total_target_count_for_query():
     data_storage = DataStorage()
-    gen_run = GenRun("n1", "v1", 0, conf)
-    executor = GenExecutor(gen_run, data_storage)
+    node = GenNodeModule("SELECT 1", lambda x: x, name="n1")
+    executor = NodeExecutor(node, data_storage)
     assert executor.prepare_node() == 1
 
 
 @pytest.mark.usefixtures("setup_test_env")
 def test_exec_node_should_return_generated_list_of_files():
     data_storage = DataStorage()
-    gen_run = GenRun("n1", "v1", 0, conf)
-    executor = GenExecutor(gen_run, data_storage)
+    node = GenNodeModule("SELECT 1", lambda x: x, name="n1")
+    executor = NodeExecutor(node, data_storage)
     executor.prepare_node()
     files = executor.exec_node()
     assert len(files) == 1
     assert os.path.exists(files[0])
```

### Comparing `lokii-1.0.0/tests/storage/test_data_storage.py` & `lokii-1.0.1/tests/storage/test_data_storage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,119 @@
 import os.path
 
-import duckdb
 import pytest
 
 from lokii.config import CONFIG
 from lokii.storage.data_storage import DataStorage
 from lokii.storage.temp_storage import TempStorage
 
+pytestmark = [pytest.mark.usefixtures("setup_test_env")]
+
 
-@pytest.mark.usefixtures("setup_test_env")
 def test_init_should_create_database_and_meta_table():
     storage = DataStorage()
     with storage.connect() as conn:
         assert os.path.exists(CONFIG.temp.db_path)
         assert "__meta" in conn.execute("SHOW TABLES;").fetchone()
 
 
-@pytest.mark.usefixtures("setup_test_env")
+@pytest.mark.parametrize(
+    "query, expect",
+    [
+        ("SELECT * from customers", ["customers"]),
+        ("SELECT 100", []),
+        (
+            """
+                SELECT i.range, t, o.officeCode
+                    FROM offices o
+                    CROSS JOIN VALUES('manager', 'employee') as data(t)
+                    CROSS JOIN range(3) as i
+                """,
+            ["offices"],
+        ),
+    ],
+)
+def test_deps_should_return_dependencies_from_query(query, expect):
+    storage = DataStorage()
+    deps = storage.deps(query)
+    assert expect == deps
+
+
 def test_count_should_return_row_count_for_query_result():
     storage = DataStorage()
     assert storage.count("SELECT unnest([1, 2, 3])") == 3
 
 
-@pytest.mark.usefixtures("setup_test_env")
 def test_exec_should_return_query_result_for_given_page():
     storage = DataStorage()
     q = "SELECT * FROM range(0, 25)"
     first_page = storage.exec(q, 0, 20)
     second_page = storage.exec(q, 1, 20)
     assert len(first_page) == 20
     assert first_page[0]["range"] == 0
     assert len(second_page) == 5
     assert second_page[0]["range"] == 20
 
 
-@pytest.mark.usefixtures("setup_test_env")
 def test_save_should_insert_record_to_meta_table():
     storage = DataStorage()
     with storage.connect() as conn:
         storage.save("test_gen1", "test_key1", "test_v1")
-        records = conn.execute("SELECT * FROM main.__meta").fetchall()
+        records = conn.execute("SELECT * FROM __meta").fetchall()
         assert len([r for r in records if "test_key1" in r]) == 1
 
 
-@pytest.mark.usefixtures("setup_test_env")
 def test_save_should_replace_record_with_same_key():
     storage = DataStorage()
     with storage.connect() as conn:
         storage.save("test_gen1", "test_key1", "test_v1")
         storage.save("test_gen2", "test_key1", "test_v4")
-        records = conn.execute("SELECT * FROM main.__meta").fetchall()
+        records = conn.execute("SELECT * FROM __meta").fetchall()
         assert len([r for r in records if "test_key1" in r]) == 1
 
 
-@pytest.mark.usefixtures("setup_test_env")
 def test_meta_should_return_data_for_given_keys():
     storage = DataStorage()
-    storage.save("test_gen1", "test_key1", "test_v1")
-    storage.save("test_gen1", "test_key2", "test_v1")
-    storage.save("test_gen2", "test_key3", "test_v4")
-    deps = storage.meta(["test_key2", "test_key3"])
+    storage.save("test_gen1", "test_node1", "test_v1")
+    storage.save("test_gen1", "test_node2", "test_v1")
+    storage.save("test_gen2", "test_node3", "test_v4")
+    deps = storage.meta(["test_node2", "test_node3"])
     assert len(deps) == 2
-    assert len([d for d in deps if d["run_key"] == "test_key2"]) == 1
-    assert len([d for d in deps if d["run_key"] == "test_key3"]) == 1
+    assert len([d for d in deps if d["name"] == "test_node2"]) == 1
+    assert len([d for d in deps if d["name"] == "test_node3"]) == 1
 
 
-@pytest.mark.usefixtures("setup_test_env")
 @pytest.mark.parametrize("node, expect", [("s1.n2", "s1"), ("s2.n2", "s2")])
 def test_insert_should_create_schema_if_node_name_contain_dot(node, expect):
     storage = DataStorage()
     with storage.connect() as conn:
         _temp = TempStorage("_")
         _temp.dump([{"data": i} for i in range(10)])
         storage.insert(node, _temp.batches)
         res = conn.execute(
-            f"SELECT * FROM information_schema.schemata WHERE schema_name = '{expect}';"
+            "SELECT * FROM information_schema.schemata WHERE schema_name = '%s';"
+            % expect
         ).fetchone()
         assert expect in res
 
 
-@pytest.mark.usefixtures("setup_test_env")
 @pytest.mark.parametrize("loop, expect", [([7], 7), ([12, 10, 7], 29)])
 def test_insert_should_create_table_from_generated_files(loop, expect):
     storage = DataStorage()
     with storage.connect() as conn:
         _temp = TempStorage("_")
         for count in loop:
             _temp.dump([{"data": i} for i in range(count)])
         storage.insert("n1", _temp.batches)
-        assert expect in conn.execute(f"SELECT COUNT() FROM n1;").fetchone()
+        assert expect in conn.execute("SELECT COUNT() FROM n1;").fetchone()
 
 
-@pytest.mark.usefixtures("setup_test_env")
 @pytest.mark.parametrize("nodes, fmt", [(["n1", "n2"], "csv")])
 def test_export_should_create_export_data_files(nodes, fmt):
     _temp = TempStorage("_")
     _temp.dump([{"data": i} for i in range(100)])
     storage = DataStorage()
     for node in nodes:
         storage.insert(node, _temp.batches)
     storage.export("data", fmt)
     for node in nodes:
-        assert os.path.exists(os.path.join("data", f"{node}.{fmt}"))
+        assert os.path.exists(os.path.join("data", ".".join([node, fmt])))
```

### Comparing `lokii-1.0.0/tests/util/test_module_file_loader.py` & `lokii-1.0.1/tests/util/test_module_file_loader.py`

 * *Files identical despite different names*

### Comparing `lokii-1.0.0/tests/util/test_perf_timer_context.py` & `lokii-1.0.1/tests/util/test_perf_timer_context.py`

 * *Files identical despite different names*

