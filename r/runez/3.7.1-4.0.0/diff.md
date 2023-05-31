# Comparing `tmp/runez-3.7.1.tar.gz` & `tmp/runez-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runez-3.7.1.tar", last modified: Wed May  3 18:26:49 2023, max compression
+gzip compressed data, was "runez-4.0.0.tar", last modified: Wed May 31 16:44:30 2023, max compression
```

## Comparing `runez-3.7.1.tar` & `runez-4.0.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:26:49.412461 runez-3.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 18:26:04.000000 runez-3.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-03 18:26:04.000000 runez-3.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-03 18:26:49.412461 runez-3.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-03 18:26:04.000000 runez-3.7.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 18:26:04.000000 runez-3.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:26:49.412461 runez-3.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-03 18:26:04.000000 runez-3.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:26:49.404461 runez-3.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:26:49.408461 runez-3.7.1/src/runez/
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/click.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:26:49.408461 runez-3.7.1/src/runez/colors/
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/colors/named.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/colors/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14267 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/date.py
--rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    38953 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    46357 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/logsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)    24983 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)    43870 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/pyenv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    27665 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    81617 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:26:49.408461 runez-3.7.1/src/runez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-03 18:26:49.000000 runez-3.7.1/src/runez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-03 18:26:49.000000 runez-3.7.1/src/runez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:26:49.000000 runez-3.7.1/src/runez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 18:26:49.000000 runez-3.7.1/src/runez.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:26:49.412461 runez-3.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    25749 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_logsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)    33428 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_pyenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_slotted.py
--rw-r--r--   0 runner    (1001) docker     (123)    31192 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:44:30.655542 runez-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-31 16:43:46.000000 runez-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 16:43:46.000000 runez-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-31 16:44:30.655542 runez-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-31 16:43:46.000000 runez-4.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 16:43:46.000000 runez-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 16:44:30.655542 runez-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-31 16:43:46.000000 runez-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:44:30.647542 runez-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:44:30.651542 runez-4.0.0/src/runez/
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/click.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:44:30.655542 runez-4.0.0/src/runez/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/colors/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/colors/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14267 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38953 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46450 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/logsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24983 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35989 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/pyenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27665 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82250 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-31 16:43:46.000000 runez-4.0.0/src/runez/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:44:30.655542 runez-4.0.0/src/runez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-31 16:44:30.000000 runez-4.0.0/src/runez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-31 16:44:30.000000 runez-4.0.0/src/runez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:44:30.000000 runez-4.0.0/src/runez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 16:44:30.000000 runez-4.0.0/src/runez.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:44:30.655542 runez-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25749 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_logsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26502 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_pyenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_slotted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31192 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-31 16:43:46.000000 runez-4.0.0/tests/test_thread.py
```

### Comparing `runez-3.7.1/LICENSE` & `runez-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/PKG-INFO` & `runez-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runez
-Version: 3.7.1
+Version: 4.0.0
 Summary: Friendly misc/utils/convenience library
 Home-page: https://github.com/codrsquad/runez
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/runez/wiki
 Project-URL: Release notes, https://github.com/codrsquad/runez/wiki/Release-notes
```

### Comparing `runez-3.7.1/README.rst` & `runez-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/setup.py` & `runez-4.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/__init__.py` & `runez-4.0.0/src/runez/__init__.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/__main__.py` & `runez-4.0.0/src/runez/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,18 +46,17 @@
 def cmd_diagnostics():
     """Show system diagnostics sample"""
     parser = runez.cli.parser()
     parser.add_argument("--border", default="colon", choices=NAMED_BORDERS, help="Use custom border.")
     parser.add_argument("--pyenv", default="~/.pyenv", help="Pyenv folder to scan for python installations.")
     args = parser.parse_args()
 
-    from runez.pyenv import PythonDepot, PythonInstallationScanner
+    from runez.pyenv import PythonDepot
 
-    scanner = PythonInstallationScanner(args.pyenv) if args.pyenv else None
-    depot = PythonDepot(scanner=scanner, use_path=True)
+    depot = PythonDepot("~/.pyenv/versions/**", "PATH")
     available = depot.representation()
     print(PrettyTable.two_column_diagnostics(runez.SYS_INFO.diagnostics(), available, border=args.border))
 
 
 def cmd_import_speed():
     """Show average import time of top-level python packages installed in this venv"""
     parser = runez.cli.parser()
```

### Comparing `runez-3.7.1/src/runez/ascii.py` & `runez-4.0.0/src/runez/ascii.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/click.py` & `runez-4.0.0/src/runez/click.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/colors/__init__.py` & `runez-4.0.0/src/runez/colors/__init__.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/colors/named.py` & `runez-4.0.0/src/runez/colors/named.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/colors/terminal.py` & `runez-4.0.0/src/runez/colors/terminal.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/config.py` & `runez-4.0.0/src/runez/config.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/conftest.py` & `runez-4.0.0/src/runez/conftest.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/convert.py` & `runez-4.0.0/src/runez/convert.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/date.py` & `runez-4.0.0/src/runez/date.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/file.py` & `runez-4.0.0/src/runez/file.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/heartbeat.py` & `runez-4.0.0/src/runez/heartbeat.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/http.py` & `runez-4.0.0/src/runez/http.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/inspector.py` & `runez-4.0.0/src/runez/inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import importlib
 import sys
 import time
 from functools import wraps
 
 from runez.convert import to_int
 from runez.program import run
-from runez.pyenv import get_current_version
 from runez.system import abort_if, find_caller, py_mimic, SYS_INFO
 
 
 def auto_import_siblings(skip=None, caller=None):
     """Auto-import all sibling submodules from caller.
 
     This is handy for click command groups for example.
@@ -110,15 +109,15 @@
     """Measure average import time of a given top-level package, works with 3.7+ only"""
 
     def __init__(self, module_name, iterations=3):
         self.module_name = module_name
         self.elapsed = None
         self.cumulative = None
         self.problem = None
-        v = get_current_version()
+        v = SYS_INFO.invoker_python.full_version
         if v < 3.7:
             self.problem = "-Ximporttime is not available in python %s, can't measure import-time speed" % v
             return
 
         cumulative = 0
         started = time.time()
         for _ in range(iterations):
```

### Comparing `runez-3.7.1/src/runez/logsetup.py` & `runez-4.0.0/src/runez/logsetup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1160,15 +1160,16 @@
 
         else:
             logging._srcfile = None
 
         logging.logProcesses = cls.is_using_format("%(process)")
         logging.logThreads = cls.is_using_format("%(thread) %(threadName)")
 
-        if not isinstance(logging.info, _LogWrap) and _R.getframe is not None:
+        getframe = getattr(sys, "_getframe", None)
+        if not isinstance(logging.info, _LogWrap) and getframe is not None:
             logging.critical = _LogWrap(logging.CRITICAL)
             logging.fatal = logging.critical
             logging.error = _LogWrap(logging.ERROR)
             logging.exception = _LogWrap(logging.ERROR, exc_info=True)
             logging.warning = _LogWrap(logging.WARNING)
             logging.info = _LogWrap(logging.INFO)
             logging.debug = _LogWrap(logging.DEBUG)
@@ -1181,19 +1182,20 @@
     def __init__(self, level, exc_info=None):
         self.level = level
         self.exc_info = exc_info
         py_mimic(self, getattr(logging, logging.getLevelName(level).lower()))
 
     @staticmethod
     def log(level, msg, *args, **kwargs):
+        getframe = getattr(sys, "_getframe", None)
         offset = kwargs.pop("_stack_offset", 1)
-        name = _R.getframe(offset).f_globals.get("__name__")
+        name = getframe(offset).f_globals.get("__name__")
         logger = logging.getLogger(name)
         try:
-            logging.currentframe = lambda: _R.getframe(3 + offset)
+            logging.currentframe = lambda: getframe(3 + offset)
             logger.log(level, msg, *args, **kwargs)
 
         finally:
             logging.currentframe = ORIGINAL_CF
 
     def __call__(self, msg, *args, **kwargs):
         kwargs.setdefault("exc_info", self.exc_info)
```

### Comparing `runez-3.7.1/src/runez/program.py` & `runez-4.0.0/src/runez/program.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/prompt.py` & `runez-4.0.0/src/runez/prompt.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/render.py` & `runez-4.0.0/src/runez/render.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/schema.py` & `runez-4.0.0/src/runez/schema.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/serialize.py` & `runez-4.0.0/src/runez/serialize.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez/system.py` & `runez-4.0.0/src/runez/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,19 +277,20 @@
         need_file (bool): If True, consider only callers that have a __file__
         need_package (bool): If True, consider only callers that have a __package__
         regex: If provided, __name__ must match given regex
 
     Returns:
         (_CallerInfo | None): Caller info, if any
     """
-    if _R.getframe is not None:
+    getframe = getattr(sys, "_getframe", None)
+    if getframe is not None:
         ignored = ("importlib", "pluggy", "runez")
         while not maximum or depth <= maximum:
             try:
-                f = _R.getframe(depth)
+                f = getframe(depth)
                 package = f.f_globals.get("__package__")
                 if package or not need_package:
                     name = f.f_globals.get("__name__")
                     top_level = package and package.partition(".")[0]
                     if name.endswith("__main__") or not top_level or (not top_level.startswith("_") and top_level not in ignored):
                         filepath = f.f_globals.get("__file__")
                         if filepath or not need_file:
@@ -1553,14 +1554,29 @@
         if _R.rdefault(argv, "diagnostics" not in sys.argv):
             yield "sys.argv", quoted(sys.argv)
 
         if _R.rdefault(prefix, SYS_INFO.venv_bin_folder):
             yield "sys.prefix", sys.prefix
 
     @cached_property
+    def invoker_python(self):
+        """The python that is either currently running us, or that created the venv we're running from"""
+        from runez.pyenv import PyInstallInfo, PythonInstallation
+
+        info = PyInstallInfo(version=sys.version_info[:3])
+        if self.is_running_in_venv:
+            installation = PythonInstallation.from_folder(sys.base_prefix, _info=info)
+
+        else:
+            installation = PythonInstallation.from_exe(sys.executable, _info=info)
+
+        PyInstallInfo.cached_by_path["invoker"] = installation
+        return installation
+
+    @cached_property
     def is_running_in_docker(self):
         """Are we currently running in a docker container?"""
         if os.path.exists("/.dockerenv") or os.environ.get("container"):
             return True
 
         try:
             with open("/proc/1/cgroup") as fh:
@@ -1571,14 +1587,19 @@
 
         except (OSError, IOError):
             pass
 
         return False
 
     @cached_property
+    def is_running_in_venv(self):
+        """Are we currently running from a virtual environment?"""
+        return sys.prefix != sys.base_prefix
+
+    @cached_property
     def platform_id(self):
         """Simplified platform identification for portable programs, example: linux-x86_64, or macos-arm64"""
         return PlatformId()
 
     @cached_property
     def platform_info(self):
         """Info on the platform we're currently running on"""
@@ -1616,15 +1637,15 @@
     def userid(self):
         """str: User id of user we're currently running as"""
         return os.environ.get("USER") or self.current_process.userid
 
     @cached_property
     def venv_bin_folder(self):
         """Path to current venv/bin folder, if we're running from a virtual environment"""
-        if sys.prefix != sys.base_prefix:
+        if self.is_running_in_venv:
             return os.path.join(sys.prefix, "bin")
 
     def venv_bin_path(self, name):
         """Path to venv/bin/<name>, if we're running from a virtual environment"""
         if self.venv_bin_folder:
             return os.path.join(self.venv_bin_folder, name)
 
@@ -1966,14 +1987,15 @@
         if "." in represented_size:
             represented_size = represented_size.strip("0").strip(".")
 
         return "%s%s%s%s" % (represented_size, delimiter, self.prefixes[exponent - 1], unit)
 
 
 class _LazyCache:
+
     @cached_property
     def rm(self):
         import runez
 
         return runez
 
     @cached_property
@@ -2001,28 +2023,24 @@
         return re.compile(r"^\s*(%s)\s*$" % "|".join((base_number, base_date)))
 
     @cached_property
     def rx_duration(self):
         return re.compile(r"^\s*(\d+[ywdhms]\s*)+$")
 
     @cached_property
-    def rx_family(self):
-        return re.compile(r"^([a-z]+\d?)[:-]?$")
-
-    @cached_property
     def rx_format_markers(self):
         return re.compile(r"{([a-z]\w*)}", re.IGNORECASE)
 
     @cached_property
-    def rx_spaces(self):
-        return re.compile(r"[\s\n]+", re.MULTILINE)
+    def rx_python_mm(self):
+        return re.compile(r"^python(\d(\.\d+)?)?$")
 
     @cached_property
-    def rx_spec(self):
-        return re.compile(r"^([a-z][a-z\d]*?)?([:-])?(\d[^:-]*)$", re.IGNORECASE)
+    def rx_spaces(self):
+        return re.compile(r"[\s\n]+", re.MULTILINE)
 
     @cached_property
     def rx_words(self):
         return re.compile(r"[^\w]+")
 
     @cached_property
     def rx_tz(self):
@@ -2058,15 +2076,14 @@
     _R stands for "runez, internal class"
 
     This internal class allows to make global settings such as runez.DRYRUN usable internally:
     - without having to `import runez` internally (can't do that due to circular import)
     - respecting any external modifications clients may have done (like: runez.DRYRUN = foo)
     """
 
-    getframe = getattr(sys, "_getframe", None)
     lc = _LazyCache()
 
     @classmethod
     def abort_exception(cls, override=None):
         """AbortException can be modified from client"""
         if isinstance(override, type) and issubclass(override, BaseException):
             return override
```

### Comparing `runez-3.7.1/src/runez/thread.py` & `runez-4.0.0/src/runez/thread.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/src/runez.egg-info/PKG-INFO` & `runez-4.0.0/src/runez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runez
-Version: 3.7.1
+Version: 4.0.0
 Summary: Friendly misc/utils/convenience library
 Home-page: https://github.com/codrsquad/runez
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/runez/wiki
 Project-URL: Release notes, https://github.com/codrsquad/runez/wiki/Release-notes
```

### Comparing `runez-3.7.1/src/runez.egg-info/SOURCES.txt` & `runez-4.0.0/src/runez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_cached_property.py` & `runez-4.0.0/tests/test_cached_property.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_click.py` & `runez-4.0.0/tests/test_click.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_colors.py` & `runez-4.0.0/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_config.py` & `runez-4.0.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_convert.py` & `runez-4.0.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_date.py` & `runez-4.0.0/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_file.py` & `runez-4.0.0/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_heartbeat.py` & `runez-4.0.0/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_http.py` & `runez-4.0.0/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_inspector.py` & `runez-4.0.0/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_logsetup.py` & `runez-4.0.0/tests/test_logsetup.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_program.py` & `runez-4.0.0/tests/test_program.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_prompt.py` & `runez-4.0.0/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_pyenv.py` & `runez-4.0.0/tests/test_pyenv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,286 +1,184 @@
 import os
-import re
 import sys
-from unittest.mock import patch
 
 import pytest
 
 import runez
 from runez.http import RestClient
-from runez.pyenv import PypiStd, PythonDepot, PythonInstallation, PythonInstallationScanner, PythonSpec, Version
+from runez.pyenv import PypiStd, PythonDepot, PythonInstallation, PythonSpec, Version
 
 
-RE_VERSION = re.compile(r"^(.*)(\d+\.\d+.\d+)$")
 PYPI_CLIENT = RestClient("https://example.com/pypi")
 
 
-def mk_python(basename, prefix=None, base_prefix=None, executable=True, content=None, folder=None, version=None):
-    if version is None:
-        m = RE_VERSION.match(basename)
-        if m:
-            if not folder:
-                folder = os.path.join(".pyenv/versions", basename)
+def mk_python(basename, prefix=None, base_prefix=None, executable=True, content=None):
+    if basename[0].isdigit():
+        version = Version(basename)
+        folder = runez.to_path(".pyenv/versions") / basename / "bin"
+
+    else:
+        version = Version(os.path.basename(basename))
+        if basename.startswith("./"):
+            folder = runez.to_path(os.path.dirname(basename[2:]))
 
-            version = m.group(2)
-            basename = "python"
+        else:
+            folder = runez.to_path(".pyenv/versions") / os.path.dirname(basename) / "bin"
 
-    if not folder:
-        folder = ".pyenv/versions"
-
-    path = runez.resolved_path(folder)
     if not prefix:
-        prefix = path
+        prefix = str(folder)
 
     if not base_prefix:
         base_prefix = prefix
 
-    path = os.path.join(path, "bin", basename)
+    path = folder / ("python%s" % version.mm)
     if not content:
         content = [version, prefix, base_prefix]
 
     content = "#!/bin/bash\n%s\n" % "\n".join("echo %s" % s for s in content)
     runez.write(path, content, logger=None)
+    runez.symlink(path, folder / "python", logger=None)
     if executable:
         runez.make_executable(path, logger=None)
 
 
-def check_find_python(depot, spec, expected):
-    p = depot.find_python(spec)
-    assert str(p) == expected
-
-
-def test_depot(temp_folder, monkeypatch, logged):
-    # Create some pyenv-style python installation mocks (using version 8 so it sorts above any real version...)
+def test_depot(temp_folder, logged):
+    # Create some pyenv-style python installation mocks (using version 8, so it sorts above any real version...)
     mk_python("8.6.1")
     mk_python("8.7.2")
-    runez.symlink("8.6.1", ".pyenv/versions/8.6", must_exist=False, logger=None)
+    mk_python("miniforge3-22.11.1-4/9.11.2")
+    mk_python("pypy-9.8.7/9.8.7")
+    mk_python("8.5.4", content=["invalid"])
+    mk_python("8.5.5", content=["invalid-version", "prefix", "prefix"])
+    runez.symlink(".pyenv/versions/8.6.1", ".pyenv/versions/8.6", logger=None)
+    runez.symlink(".pyenv/versions/8.6.1", ".pyenv/versions/python8.6", logger=None)
+
+    depot = PythonDepot(".pyenv/versions/**")
+    assert len(depot.available_pythons) == 4
+
+    assert str(depot.find_python("8.5.4")) == "8.5.4 [not available]"
+    invalid = depot.find_python(".pyenv/versions/8.5.4")
+    assert str(invalid) == ".pyenv/versions/8.5.4 [internal error: _pv returned 'invalid']"
+    bad_version = depot.find_python(".pyenv/versions/8.5.5")
+    assert str(bad_version) == ".pyenv/versions/8.5.5 [invalid version 'invalid-version']"
+
+    versions = [p.mm_spec.canonical for p in depot.available_pythons]
+    assert versions == ["pypy:9.8", "cpython:8.7", "cpython:8.6", "conda:9.11"]
 
-    # Verify that if invoker is one of the pyenv-installations, it is properly detected
-    depot = mocked_invoker(pyenv=".pyenv", base_prefix=".pyenv/versions/8.6.1", version_info=(8, 6, 1))
+    # Verify that latest available is found (when under-specified)
     p8 = depot.find_python("8")
-    p86 = depot.find_python("8.6")
-    assert str(p8) == ".pyenv/versions/8.7.2 [cpython:8.7.2]"  # Latest version 8 (invoker doesn't take precedence)
-    assert p8.folder == runez.to_path(".pyenv/versions/8.7.2/bin").absolute()
-    assert p86 is depot.invoker
-    assert str(depot) == "2 scanned"
-    assert depot.scanned == [p8, p86]
-    assert depot.from_path == []
-    assert not logged
+    assert not p8.is_virtualenv
+    assert repr(p8) == ".pyenv/versions/8.7.2 [cpython:8.7]"
+    assert str(p8) == ".pyenv/versions/8.7.2 [cpython:8.7.2]"
+
+    # Verify that preferred python is respected
+    depot.set_preferred_python("8.6")
+    assert repr(depot.find_python("8")) == ".pyenv/versions/8.6.1 [cpython:8.6]"
+    assert p8 == depot.find_python("8.7")
+
+    # Verify min spec
+    assert str(depot.find_python("conda:9.1+")) == ".pyenv/versions/miniforge3-22.11.1-4 [conda:9.11.2]"
+
+    # There's only one symlink of the form 'python*'
+    depot2 = PythonDepot(".pyenv/versions/python*")
+    assert len(depot2.available_pythons) == 1
+    assert str(depot2.available_pythons[0]) == ".pyenv/versions/python8.6 [cpython:8.6.1]"
 
-    mk_python("8.8.3", executable=False)
-    mk_python("8.9.0")
-    mk_python("miniconda3-4.7.12")
-
-    # Create some PATH-style python installation mocks (using version 9 so it sorts higher than pyenv ones)
-    mk_python("python", folder="path1", version="9.5.1")
-    mk_python("python3", folder="path1", content=["foo"])  # Invalid: mocked _pv.py does not return the right number of lines
-    mk_python("python", folder="path2", content=["foo; bar"])  # --version fails
-    mk_python("some-other-python-exe-name", folder="path3", version="8.5.0")
-    mk_python("python3", folder="path3")  # Invalid version
-    with runez.CurrentFolder("path3/bin"):
-        runez.symlink("some-other-python-exe-name", "python", logger=None)
-
-    monkeypatch.setenv("PATH", "bar:path1/bin:path2/bin:path3/bin")
-    scanner = PythonInstallationScanner(".pyenv")
-    assert str(scanner) == "portable python [.pyenv]"
-    depot = PythonDepot(scanner=scanner, use_path=True)
-    assert str(depot) == "4 scanned, 2 from PATH"
-    r = depot.representation()
-    assert "Installed portable python:" in r
-    assert "Available pythons from PATH:" in r
-
-    depot.find_preferred_python("8.7.2,8.9.0", "8.7", "8.10")
-    assert depot.preferred_python.version == "8.7.2"
-
-    depot.find_preferred_python("8.7.2,8.9.0", "8.7", "8.8")
-    assert depot.preferred_python.version == "8.9.0"
-    assert depot.find_python(None) is depot.preferred_python
-    assert depot.find_python("8") is depot.preferred_python
-
-    depot.find_preferred_python("8.7.2,8.9.0", "10.7", "10.8")
-    assert depot.preferred_python is None
-
-    depot.find_preferred_python("")
-    assert depot.preferred_python is None
-
-    assert len(depot.from_path) == 2
-    assert len(depot.scanned) == 4
-    assert depot.scan_path_env_var() is None  # Already scanned to try and find invoker
-    p95 = depot.find_python("9.5.1")
-    assert str(p95) == "path1/bin/python [cpython:9.5.1]"
-
-    check_find_python(depot, "9", "path1/bin/python [cpython:9.5.1]")
-    check_find_python(depot, "42.4", "42.4 [not available]")
-    check_find_python(depot, "foo", "foo [not available]")
-    check_find_python(depot, "python:43.0.0", "python:43.0.0 [not available]")
-
-    with pytest.raises(runez.system.AbortException):
-        depot.find_python("/bar", fatal=True)
-
-    pbar = depot.find_python("/bar")
-    assert str(pbar) == "/bar [not an executable]"
-    assert pbar.problem
-    assert not pbar.satisfies(depot.spec_from_text("python"))
+    assert not logged
 
-    p8 = depot.find_python("8")
-    p8a = depot.find_python(PythonSpec("8"))
-    assert p8a is p8
-    p86 = depot.find_python("8.6")
-    p87 = depot.find_python("8.7")
-    p88 = depot.find_python("8.8")
-    p89 = depot.find_python("8.9")
-    c = depot.find_python("conda")
-    c47 = depot.find_python("conda:4.7")
-    assert c47 is c
-    assert depot.find_python(PythonSpec("conda47")) is c47
-    assert depot.scanned == [p89, p87, p86, c47]
-
-    assert p8.major == 8
-    assert p88.major == 8
-    assert str(p8) == ".pyenv/versions/8.9.0 [cpython:8.9.0]"
-    assert str(p88) == "8.8 [not available]"
-    assert str(c47) == ".pyenv/versions/miniconda3-4.7.12 [conda:4.7.12]"
-    assert p8 is p89
-    assert p8 == p89
-    assert p8 != p88
-    assert p8 != pbar
-    assert p8.satisfies(PythonSpec("python"))
-    assert p8.satisfies(PythonSpec("python8"))
-    assert p8.satisfies(PythonSpec("py8.9.0"))
-    assert not p8.satisfies(PythonSpec("py8.9.1"))
-    assert c47.satisfies(PythonSpec("conda47"))
-    assert len({p8, p89}) == 1
-    assert len({p8, p89, p88}) == 2
 
+def test_depot_adhoc(temp_folder):
+    depot = PythonDepot(".pyenv/versions")
+    assert depot.representation() == "No python installations found in '.pyenv/versions'"
 
-def test_depot_adhoc(temp_folder, monkeypatch):
-    depot = PythonDepot(use_path=False)
     p11 = depot.find_python("11.0.0")
-    pfoo = depot.find_python("/foo")
     assert p11.problem == "not available"
 
     # Only paths are cached
     p11b = depot.find_python("11.0.0")
     assert p11 is not p11b
     assert p11 == p11b
-    assert depot.find_python("/foo") == pfoo
+    pfoo = depot.find_python("/foo")
+    assert depot.find_python("/foo") is pfoo
 
-    # Edge case: check we can still compare incomplete objects (missing spec.version here for 'pfoo')
-    assert pfoo == pfoo
-    assert not (pfoo < pfoo)
-    assert not (pfoo > pfoo)
-    assert pfoo < p11
-    assert p11 > pfoo
-    assert not (p11 < pfoo)
-    assert not (pfoo > p11)
-
-    # Edge case: comparison still works even when there is no spec, arbitrarily sort no spec lower...
-    pfoo.spec = None
-    assert pfoo < p11
-
-    mk_python("python", folder="some-path", version="11.0.0")
-    py_path = os.path.realpath("some-path/bin/python")
-    p11 = depot.find_python(py_path)
-    assert depot.find_python("./some-path/") == p11
-    assert depot.find_python("some-path/bin") == p11
-    assert str(p11) == "some-path/bin/python [cpython:11.0.0]"
-
-
-def test_empty_depot():
-    depot = PythonDepot(use_path=False)
-    assert str(depot) == "0 scanned"
-    assert depot.from_path == []
-    assert depot.scanned == []
-
-    assert depot.find_python(depot.invoker) is depot.invoker
-    assert depot.find_python(PythonSpec(depot.invoker.executable)) is depot.invoker
-    assert depot.find_python(PythonSpec("invoker")) is depot.invoker
-    assert depot.find_python("invoker") is depot.invoker
-    assert depot.find_python(depot.invoker.spec.family) is depot.invoker
-    assert depot.representation() == ""
+    mk_python("./some-path/bin/13.1.2")
+    assert str(depot.find_python("some-path/bin/python13.1")) == "some-path/bin/python13.1 [cpython:13.1.2]"
+    assert str(depot.find_python("./some-path/")) == "some-path [cpython:13.1.2]"
+    assert str(depot.find_python(runez.to_path("some-path"))) == "some-path [cpython:13.1.2]"
+    assert str(depot.find_python("some-path/bin/python")) == "some-path/bin/python [cpython:13.1.2]"
+    assert str(depot.find_python("some-path/bin")) == "some-path/bin/python [cpython:13.1.2]"
+
+
+def test_depot_path(temp_folder):
+    depot = PythonDepot("PATH")
+    assert depot.available_pythons
+
+
+def test_empty_depot(temp_folder):
+    depot = PythonDepot()
+    assert depot.representation() == "No PythonDepot locations configured"
+    assert not depot.available_pythons
+    invoker = runez.SYS_INFO.invoker_python
+    assert ", invoker" in repr(invoker)
+    assert ", invoker" in str(invoker)
+
+    mm = invoker.mm
+    assert depot.find_python(None) is invoker
+    assert depot.find_python("invoker") is invoker
+    assert depot.find_python(invoker.executable) is invoker
+    assert depot.find_python(runez.to_path(invoker.executable)) is invoker
+    assert depot.find_python(PythonSpec("cpython", mm)) is invoker
+    assert depot.find_python("python") is invoker
+    assert depot.find_python("py%s" % mm) is invoker  # eg: py3.10
+    assert depot.find_python("py%s" % mm.text.replace(".", "")) is invoker  # tox style: py310
+    assert depot.find_python(mm.text) is invoker
+    assert depot.find_python("python") is invoker
+    assert depot.find_python("python%s" % mm.major) is invoker
 
     p = depot.find_python("foo")
     assert str(p) == "foo [not available]"
     assert repr(p) == "foo [not available]"
+    assert p.short_name == "foo"
+    assert p.major is None
     assert p.problem == "not available"
-    assert str(depot) == "0 scanned"
+    assert p.mm_spec is None
+    assert p.major is None
+    assert p.full_version is None
+
+    # Disabling invoker still finds it explicitly, but not by generic spec
+    depot.invoker = None
+    assert depot.find_python("invoker") is invoker  # Found only if explicitly referred to
+    assert str(depot.find_python("python")) == "python [not available]"
+    assert str(depot.find_python(mm.text)) == "%s [not available]" % mm
+
+
+def test_invoker(monkeypatch):
+    from runez.pyenv import PyInstallInfo
+
+    # Simulate case where runez was installed globally (not in a venv)
+    monkeypatch.setattr(PyInstallInfo, "cached_by_path", {})
+    monkeypatch.setattr(runez.SYS_INFO, "is_running_in_venv", False)
+    monkeypatch.delattr(runez.SYS_INFO, "invoker_python")
+    invoker = runez.SYS_INFO.invoker_python
+    assert invoker.executable == sys.executable
+    assert not invoker.is_virtualenv
+    assert invoker.is_invoker
+    assert invoker.major == sys.version_info[0]
+    assert not invoker.problem
+
+
+def test_installation_short_name():
+    python = PythonInstallation("/System/Library/Frameworks/Python.framework/Versions/2.7")
+    assert python.short_name == "/usr/bin/python2"
 
+    python = PythonInstallation("/Library/Developer/CommandLineTools/Library/Frameworks/Python3.framework/Versions/3.7")
+    assert python.short_name == "/usr/bin/python3"
 
-def mocked_invoker(**sysattrs):
-    major = sysattrs.pop("major", 3)
-    pyenv = sysattrs.pop("pyenv", None)
-    use_path = sysattrs.pop("use_path", False)
-    exe_exists = sysattrs.pop("exe_exists", True)
-    sysattrs.setdefault("base_prefix", "/usr")
-    sysattrs.setdefault("prefix", sysattrs["base_prefix"])
-    sysattrs["base_prefix"] = runez.resolved_path(sysattrs["base_prefix"])
-    sysattrs["prefix"] = runez.resolved_path(sysattrs["prefix"])
-    sysattrs.setdefault("executable", "%s/bin/python" % sysattrs["base_prefix"])
-    sysattrs.setdefault("version_info", (major, 7, 1))
-    sysattrs.setdefault("version", ".".join(str(s) for s in sysattrs["version_info"]))
-    scanner = None if not pyenv else PythonInstallationScanner(pyenv)
-    with patch("runez.pyenv.os.path.realpath", side_effect=lambda x: x):
-        with patch("runez.pyenv.sys") as mocked:
-            for k, v in sysattrs.items():
-                setattr(mocked, k, v)
-
-            if isinstance(exe_exists, bool):
-                with patch("runez.pyenv.is_executable", return_value=exe_exists):
-                    return PythonDepot(scanner=scanner, use_path=use_path)
-
-            with patch("runez.pyenv.is_executable", side_effect=exe_exists):
-                return PythonDepot(scanner=scanner, use_path=use_path)
-
-
-def test_invoker():
-    depot = PythonDepot(use_path=False)
-    assert depot.find_python(None) is depot.invoker
-    assert depot.find_python("") is depot.invoker
-    assert depot.find_python("py") is depot.invoker
-    assert depot.find_python("python") is depot.invoker
-    assert depot.find_python(depot.invoker.executable) is depot.invoker
-    assert depot.find_python("invoker") is depot.invoker
-    assert depot.find_python("%s" % sys.version_info[0]) is depot.invoker
-    assert "invoker" in str(depot.invoker)
-    assert str(depot.invoker) == repr(depot.invoker)  # Identical when coloring is off
-
-    # Linux case with py3
-    depot = mocked_invoker()
-    assert depot.invoker.executable == "/usr/bin/python3.7"
-    assert depot.invoker.folder == runez.to_path("/usr/bin")
-    assert depot.invoker.major == 3
-
-    # Linux case without py3
-    depot = mocked_invoker(major=2, base_prefix="/usr/local")
-    assert depot.invoker.executable == "/usr/local/bin/python2.7"
-    assert depot.invoker.major == 2
-
-    # Linux case with only /usr/bin/python
-    depot = mocked_invoker(major=2, exe_exists=lambda x: "python2" not in x and "python3" not in x)
-    assert depot.invoker.executable == "/usr/bin/python"
-    assert depot.invoker.major == 2
-
-    # Use sys.executable when prefix can't be used to determine invoker
-    depot = mocked_invoker(major=2, base_prefix=None, executable="/foo", exe_exists=False)
-    assert depot.invoker.executable == "/foo"
-    assert depot.invoker.major == 2
-
-    # macos silly path choices
-    depot = mocked_invoker(major=2, base_prefix="/System/Library/Frameworks/Python.framework/Versions/2.7")
-    assert depot.invoker.executable == "/usr/bin/python2"
-    assert depot.invoker.major == 2
-
-    depot = mocked_invoker(base_prefix="/Library/Developer/CommandLineTools/Library/Frameworks/Python3.framework/Versions/3.7")
-    assert depot.invoker.executable == "/usr/bin/python3"
-    assert depot.invoker.major == 3
-
-    depot = mocked_invoker(base_prefix="/usr/local/Cellar/python@3.7/3.7.1_1/Frameworks/Python.framework/Versions/3.7")
-    assert depot.invoker.executable == "/usr/local/bin/python3"
-    assert depot.invoker.major == 3
+    python = PythonInstallation("/usr/local/Cellar/python@3.7/3.7.1_1/Frameworks/Python.framework/Versions/3.7")
+    assert python.short_name == "/usr/local/bin/python3"
 
 
 def test_pypi_standardized_naming():
     assert not PypiStd.is_acceptable(None)
     assert not PypiStd.is_acceptable(1)
     assert not PypiStd.is_acceptable("")
     assert not PypiStd.is_acceptable("a")  # Don't bother with one letter packages
@@ -298,17 +196,18 @@
     assert PypiStd.std_package_name(None) is None
     assert PypiStd.std_package_name(5) is None
     assert PypiStd.std_package_name("") is None
     assert PypiStd.std_package_name("-a-") is None
     assert PypiStd.std_package_name("a") is None
     assert PypiStd.std_package_name("foo") == "foo"
     assert PypiStd.std_package_name("Foo") == "foo"
-    assert PypiStd.std_package_name("A__b-c_1.0") == "a-b-c-1-0"
+    assert PypiStd.std_package_name("A__b-c_1.0") == "a-b-c-1.0"
     assert PypiStd.std_package_name("some_-Test") == "some-test"
-    assert PypiStd.std_package_name("a_-_-.-_.--b") == "a-b"
+    assert PypiStd.std_package_name("a_-_-.-_.--b") == "a-.-.-b"
+    assert PypiStd.std_package_name("a_-_-.-_.--b", allow_dots=False) == "a-b"
 
     assert PypiStd.std_wheel_basename(None) is None
     assert PypiStd.std_package_name(10.1) is None
     assert PypiStd.std_wheel_basename("") is None
     assert PypiStd.std_wheel_basename("a.b_-_1.5--c") == "a.b_1.5_c"
     assert PypiStd.std_wheel_basename("a.b_-___1.5--c") == "a.b_1.5_c"
 
@@ -392,237 +291,116 @@
     black = sorted(PypiStd.ls_pypi("black"))  # All versions are pre-releases
     assert len(black) == 3
     assert black[0].version.prerelease
 
     funky = sorted(PypiStd.ls_pypi("funky-proj", source=None))
     assert len(funky) == 2
     assert funky[0].package_name == "funky.proj"
-    assert funky[0].pypi_name == "funky-proj"
+    assert funky[0].pypi_name == "funky.proj"
     assert funky[1].is_dirty
     assert black[0] < funky[0]  # Alphabetical sort when both have no source
     assert funky[0] < sample[4]  # Arbitrary: no-source sorts lowest...
 
 
-def test_sorting(temp_folder):
-    mk_python("3.6.1")
-    mk_python("3.7.2")
-    mk_python("3.8.3")
-    mk_python("conda-4.6.1")
-    mk_python("miniconda3-4.3.2")
-    depot = PythonDepot(scanner=PythonInstallationScanner(".pyenv"), use_path=False)
-    assert str(depot) == "5 scanned"
-    versions = [p.spec.canonical for p in depot.scanned]
-    assert versions == ["conda:4.6.1", "conda:4.3.2", "cpython:3.8.3", "cpython:3.7.2", "cpython:3.6.1"]
-
-
-def check_spec(text, canonical):
-    d = PythonSpec(text)
-    assert d.text == runez.stringified(text).strip()
-    assert str(d) == canonical
-
-
 def test_spec():
-    invoker = PythonSpec("invoker")
-    assert invoker.family
-    assert invoker.version
-    assert str(invoker) == "invoker"
-    assert PythonSpec.speccified(None) == []
-    assert PythonSpec.speccified([]) == []
-    assert PythonSpec.speccified([None, "", None]) == []
-    assert PythonSpec.speccified([""]) == []
-    assert PythonSpec.speccified(["", "foo"]) == [PythonSpec("foo")]
-    assert PythonSpec.speccified(["", "foo"], strict=True) == []
-    assert PythonSpec.speccified(["", "foo", "3.7"], strict=True) == [PythonSpec("3.7")]
-    assert PythonSpec.speccified([2.7, 3.9]) == [PythonSpec("2.7"), PythonSpec("3.9")]
-    assert PythonSpec.speccified("27") == [PythonSpec("2.7")]
-    assert PythonSpec.speccified("39,2.7") == [PythonSpec("3.9"), PythonSpec("2.7")]
-    assert PythonSpec.speccified("2.7.7a", strict=True) == []
-
-    pnone = PythonSpec(None)
-    assert pnone == invoker
-    assert PythonSpec.to_spec(None) == invoker
-    assert PythonSpec.to_spec(pnone) is pnone
-    p32a = PythonSpec("py32")
-    p32b = PythonSpec("python3.2")
-    assert p32a == p32b
-    assert pnone != p32a
-    assert pnone > p32a
-    assert not (pnone < p32a)
-    assert len({p32a, p32b}) == 1
-    assert len({p32a, p32b, pnone}) == 2
-
-    assert not p32a.satisfies(pnone)
-    assert not pnone.satisfies(p32a)
-
-    invoker = PythonSpec("invoker")
-    assert str(invoker) == "invoker"
-    assert invoker.version.major == sys.version_info[0]
-
-    p38plus = PythonSpec("3.8+")
-    assert not p32a.satisfies(p38plus)
-    assert not p32b.satisfies(p38plus)
-
-    p38 = PythonSpec("3.8")
-    c38a = PythonSpec("conda:38")
-    c38b = PythonSpec("conda:3.8")
-    assert p38.satisfies(p38plus)
-    assert c38a != p38
-    assert c38a.version == p38.version
-    assert c38a == c38b
-
-    p310 = PythonSpec("3.10.0")
-    p310rc = PythonSpec("3.10.0rc1")
-    assert p310rc < p310
-    assert p310 > p310rc
-
-    p39 = PythonSpec("3.9")
-    p395 = PythonSpec("3.9.5")
-    assert p39.satisfies(p38plus)
-    assert p395.satisfies(p38plus)
+    p3 = PythonSpec.from_text("3")
+    p3plus = PythonSpec.from_text("3+")
+    assert str(p3) == "cpython:3"
+    assert str(p3plus) == "cpython:3+"
+    assert not p3.is_min_spec
+    assert p3plus.is_min_spec
+
+    p38 = PythonSpec.from_text("3.8")
+    assert p38.satisfies(p3)
+    assert p38.satisfies(p3plus)
+
+    p38plus = PythonSpec.from_text("3.8+")
+    c38 = PythonSpec.from_text("conda:3.8")
+    assert c38 != p38
+    assert c38.version == p38.version
+    assert p38 == PythonSpec.from_text("py38")
+    assert not c38.satisfies(p38)
+    assert not p38.satisfies(c38)
+
+    p310 = PythonSpec.from_text("3.10")
+    assert p310 == PythonSpec.from_text("py310")
+    assert not p38.satisfies(p310)
+    assert not p310.satisfies(p38)
+    assert p310.satisfies(p38plus)
+    assert p310.satisfies(p310)
+    assert PythonSpec.from_text("3.10.1").satisfies(p310)
+    assert PythonSpec.from_text("3.10.0rc1").satisfies(p310)
 
     assert p38.represented() == "3.8"
     assert p38.represented(compact=None) == "cpython:3.8"
     assert p38.represented(compact=False) == "cpython:3.8"
     assert p38.represented(compact=True) == "3.8"
     assert p38.represented(compact="cpython") == "3.8"
     assert p38.represented(compact=["cpython", "conda"]) == "3.8"
     assert p38.represented(color=str, compact=None) == "cpython:3.8"
 
-    assert c38a.represented() == "conda:3.8"
-    assert c38a.represented(compact=True) == "3.8"
-    assert c38a.represented(compact="cpython") == "conda:3.8"
-    assert c38a.represented(compact=["cpython", "conda"]) == "3.8"
-    assert c38a.represented(color=str, compact=None) == "conda:3.8"
-
-    check_spec("", "invoker")
-    check_spec(" ", "invoker")
-    check_spec(" : ", "?:")
-    check_spec(" - ", "?-")
-    check_spec(" pY 3 ", "?pY 3")
-    check_spec(2, "cpython:2")
-    check_spec("2", "cpython:2")
-    check_spec("3", "cpython:3")
-    check_spec("3+", "cpython:3+")
-    check_spec("P3", "cpython:3")
-    check_spec("py3", "cpython:3")
-    check_spec("cpython:", "cpython:")
-    check_spec("cpython-", "cpython:")
-    check_spec("cpython3", "cpython:3")
-    check_spec("python3", "cpython:3")
-    check_spec(3.7, "cpython:3.7")
-    check_spec(" p3.7 ", "cpython:3.7")
-    check_spec(" cpython:3.7 ", "cpython:3.7")
-    check_spec(" p3.7+ ", "cpython:3.7+")
-    check_spec(" p3.7++ ", "?p3.7++")
-
-    # Various convenience notations
-    check_spec("37", "cpython:3.7")
-    check_spec("3.7", "cpython:3.7")
-    check_spec("py37", "cpython:3.7")  # tox.ini style
-    check_spec("py3.7", "cpython:3.7")
-    check_spec("python37", "cpython:3.7")
-    check_spec("python3.7", "cpython:3.7")
-
-    # One separator OK
-    check_spec(":37", "cpython:3.7")
-    check_spec("-37", "cpython:3.7")
-    check_spec("py:3.7", "cpython:3.7")
-    check_spec("py-3.7", "cpython:3.7")
-
-    # More than one separator not OK
-    check_spec("::37", "?::37")
-    check_spec(":-37", "?:-37")
-    check_spec("--37", "?--37")
-    check_spec("py::3.7", "?py::3.7")
-    check_spec("py:-3.7", "?py:-3.7")
-    check_spec("py--3.7", "?py--3.7")
-
-    # Non-cpython families
-    check_spec("pypy", "pypy:")
-    check_spec("pypy:", "pypy:")
-    check_spec("pypy:+", "?pypy:+")  # Need actual version for '+' marker to count
-    check_spec("pypy36", "pypy:3.6")
-    check_spec("pypy36+", "pypy:3.6+")
-    check_spec("pypy:37", "pypy:3.7")
-    check_spec("pypy:3.8", "pypy:3.8")
-    check_spec("conda:", "conda:")
-    check_spec("conda:38", "conda:3.8")
-    check_spec("conda:3.9.1", "conda:3.9.1")
-    check_spec("miniconda-3.18.3", "miniconda:3.18.3")
-    check_spec("miniconda3-4.7.12", "miniconda3:4.7.12")
-
-    # Up to 3 version components are valid
-    check_spec("391", "cpython:3.91")
-    check_spec("3.9.1", "cpython:3.9.1")
-    check_spec("py391", "cpython:3.91")
-    check_spec("3777", "cpython:3.777")
-    check_spec("3.7.7.7", "cpython:3.7.7.7")
-
-    # Invalid marked with starting '?' for canonical form
-    check_spec(" + ", "?+")
-    check_spec(" cpython+ ", "?cpython+")
-    check_spec(" python+ ", "?python+")
-    check_spec("cpython:3.7a", "?cpython:3.7a")
-    check_spec("miniconda3--4.7.1", "?miniconda3--4.7.1")
-    check_spec("foo3.7", "foo:3.7")
-    check_spec("python3:", "python3:")  # Separator is in the wrong place, consider 'python3' to be the family name...
-
-    # Paths remain as-is
-    check_spec("foo/python2.7", runez.short(runez.resolved_path("foo/python2.7")))
-    check_spec("/foo/python2.7", "/foo/python2.7")
-    check_spec("~/.pyenv/3.8.1", "~/.pyenv/3.8.1")
-
-
-class CustomScanner(PythonInstallationScanner):
-    def unknown_python(self, spec):
-        # Pretend an auto-installation for example
-        return PythonInstallation(runez.resolved_path(self.location / spec.text / "bin" / "python"), spec)
-
-
-def test_venv(temp_folder, logged):
-    depot = PythonDepot(use_path=False)
-    import sys
-    p = depot.find_python(sys.executable)
-    assert p is depot.invoker
+    assert c38.represented() == "conda:3.8"
+    assert c38.represented(compact=True) == "3.8"
+    assert c38.represented(compact="cpython") == "conda:3.8"
+    assert c38.represented(compact=["cpython", "conda"]) == "3.8"
+    assert c38.represented(color=str, compact=None) == "conda:3.8"
+
+
+def test_spec_equivalent():
+    def check_equivalent_specs(*text):
+        specs = [PythonSpec.from_text(x) for x in text]
+        assert len(specs) == len(text)
+        assert len(set(specs)) == 1
+
+    check_equivalent_specs("3", "py3", "python3", "cpython:3", "python", "py")
+    check_equivalent_specs("3+", "py3+", "python3+", "cpython:3+")
+    check_equivalent_specs("3.10", "310", "py3.10", "py310", "python3.10", "python310", "cpython:3.10")
+    check_equivalent_specs("3.10+", "310+", "py3.10+", "py310+", "python3.10+", "python310+", "cpython:3.10+")
+    check_equivalent_specs("3777", "py3.777", "python3.777", "cpython:3.777")
+
+
+def test_spec_invalid():
+    def check_spec_invalid(text):
+        assert PythonSpec.from_text(text) is None
+
+    check_spec_invalid(None)
+    check_spec_invalid("foo")
+    check_spec_invalid("foo:3")
+    check_spec_invalid("cpython")
+    check_spec_invalid("cpython:")
+    check_spec_invalid("cpython:3.10.0rc1")
+    check_spec_invalid("cpython:+")
+    check_spec_invalid("cpython: 3")
+    check_spec_invalid("cpython :3")
+    check_spec_invalid("python:3")
+    check_spec_invalid("p3.9")
+    check_spec_invalid("pY3")
+    check_spec_invalid("3.9.9a")
+    check_spec_invalid("3.9.9++")
+
 
+def test_venv(temp_folder):
     # Simulate an explicit reference to a venv python
-    mk_python("8.6.1")
-    mk_python("8.6.1", prefix="foo", base_prefix=".pyenv/versions/8.6.1", folder=".venv")
-    assert str(depot) == "0 scanned"
-    pvenv = depot.find_python(".venv/bin/python")
-    assert str(depot) == "0 scanned"
-    assert depot.find_python(".venv") == pvenv
-    assert str(pvenv) == ".pyenv/versions/8.6.1 [cpython:8.6.1]"
-
-    # Edge case: version is found via .pyenv first
-    depot = PythonDepot(scanner=CustomScanner(".pyenv"), use_path=False)
-    assert str(depot) == "1 scanned"
-    pvenv = depot.find_python(".venv/bin/python")
-    assert str(pvenv) == ".pyenv/versions/8.6.1 [cpython:8.6.1]"
-    assert depot.scanned == [pvenv]
-
-    p95 = depot.find_python("9.5.1")
-    assert p95.problem is None
-    assert str(depot) == "2 scanned"
-    assert depot.scanned == [p95, pvenv]
-    assert not logged
+    mk_python("./some-venv/bin/8.6.1", prefix="foo", base_prefix=".pyenv/versions/8.6.1")
 
+    depot = PythonDepot()
+    assert not depot.available_pythons
+    pvenv = depot.find_python("./some-venv/bin/python")
+    assert repr(pvenv) == "some-venv/bin/python [cpython:8.6]"
+    assert str(pvenv) == "some-venv/bin/python [cpython:8.6.1*]"
+    assert pvenv.is_virtualenv
+    assert depot.find_python("./some-venv") == pvenv
+
+
+def test_venv_from_project():
+    depot = PythonDepot()
+    assert not depot.available_pythons
 
-def test_unknown():
-    depot = PythonDepot(use_path=False)
-    p = depot.find_python("foo")
-    assert str(p) == "foo [not available]"
-    assert p.executable == "foo"
-    assert p.folder is None
-    assert p.major is None
-    assert p.problem == "not available"
-    assert p.spec.canonical == "foo:"
-    assert p.spec.text == "foo"
-    assert p.major is None
-    assert p.version is None
+    pvenv = depot.find_python(sys.executable)
+    assert pvenv.is_virtualenv
 
 
 @pytest.mark.parametrize(
     ("given_version", "expected"),
     [
         ("1.2", (1, 2, 0, 0, 0, 0, "")),
         ("1.2rev5", (1, 2, 0, 0, 0, 5, "rev")),
@@ -635,57 +413,65 @@
         ("1.0b2.post345", (1, 0, 0, 0, 0, 0, "", "b", 2, "post", 345, "z", 0)),
         ("1.0b2.post345.dev456", (1, 0, 0, 0, 0, 0, "", "b", 2, "post", 345, "dev", 456)),
         ("1.0rc1.dev456", (1, 0, 0, 0, 0, 0, "", "rc", 1, "", 0, "dev", 456)),
         ("1.0.post456.dev34", (1, 0, 0, 0, 0, 456, "post", "", 0, "post", 456, "dev", 34)),
     ]
 )
 def test_pep_sample(given_version, expected):
-    version = Version(given_version, strict=True)
+    version = Version(given_version)
     assert version.is_valid
+    assert version.ignored is None
     assert str(version) == given_version
     actual = version.components
     if version.prerelease:
         actual += version.prerelease
 
     assert actual == expected
 
 
 def test_version():
-    loose = Version("v1.0.dirty", strict=False)
+    loose = Version("v1.0.dirty", canonical=None)
     assert loose.is_valid
     assert loose.ignored == ".dirty"
     assert str(loose) == "1.0"
+    assert loose.pep_440 == "1.0"
 
-    invalid = Version("v1.0.dirty", strict=True)
+    invalid = Version("v1.0.dirty")
     assert not invalid.is_valid
     assert str(invalid) == "v1.0.dirty"
     assert invalid.ignored == ".dirty"
     assert loose > invalid
 
-    dev101 = Version("0.0.1.dev101")
+    dev101 = Version("0.0.1dev101")
     assert not dev101.is_final
     assert dev101.is_valid
+    assert not dev101.is_dirty
     assert dev101.prerelease
+    assert str(dev101) == "0.0.1dev101"
+    assert dev101.pep_440 == "0.0.1.dev101"
 
     none = Version(None)
     assert str(none) == ""
     assert not none.is_valid
     assert not none.is_final
     assert none.mm is None
 
     empty = Version("")
     assert str(empty) == ""
     assert not empty.is_valid
     assert empty == none
     assert empty.major is None
 
     ep = Version("123!2.1+foo.dirty-bar")
+    assert str(ep) == "123!2.1+foo.dirty-bar"
+    assert ep.pep_440 == "123!2.1+foo.dirty-bar"
     assert ep.is_valid
+    assert ep.is_dirty
     assert ep.epoch == 123
-    assert ep.main == "2.1.0"
+    assert ep.main == "2.1"
     assert ep.local_part == "foo.dirty-bar"
     assert ep.mm == "2.1"
 
     foo = Version("foo")
     assert str(foo) == "foo"
     assert not foo.is_valid
     assert not foo.components
@@ -693,18 +479,20 @@
     assert foo.major is None
 
     bogus = Version("1.2.3.4.5.6")
     assert str(bogus) == "1.2.3.4.5.6"
     assert not bogus.is_valid
     assert not bogus.components
     assert not bogus.prerelease
+    assert bogus.mm is None
 
     v1 = Version("1")
     assert v1.components == (1, 0, 0, 0, 0, 0, "")
     assert str(v1) == "1"
+    assert v1.main == "1"
     assert v1.mm == "1.0"
     assert empty < v1
     assert v1 > empty
     assert v1 != empty
     assert v1 < 2
     assert v1 < 1.1
     assert v1 < "1.1"
@@ -714,58 +502,63 @@
     assert v1 > "0"
 
     # All versions are bigger than anything not parsing to a valid version
     assert v1 > ""
     assert v1 > []
     assert v1 > [5, 2, 3, 4, 5, 6]
 
-    v1foo = Version("1foo")  # Ignore additional text
+    v1foo = Version("1foo", canonical=None)  # Ignore additional text
     assert v1 == v1foo
 
-    vrc = Version("1.0rc4-foo")
-    vrc_strict = Version("1.0rc4-foo", strict=True)
-    vdev = Version("1.0a4.dev5-foo")
+    vrc = Version("1.0rc4-bar", canonical=None)
+    vdev = Version("1.0a4.dev5-foo", canonical=None)
+    assert vdev.pep_440 == "1.0a4.dev5"
+    assert vdev.ignored == "-foo"
     assert vrc.is_valid
     assert not vrc.is_final
-    assert not vrc_strict.is_valid
     assert not vdev.is_final
     assert vdev.prerelease == ("a", 4, "", 0, "dev", 5)
     assert vrc.suffix == "rc"
     assert vdev.suffix == "a.dev"  # Try and convey the fact that we have .a.dev version
 
     assert vdev < vrc
     assert str(vrc) == "1.0rc4"
     assert str(vdev) == "1.0a4.dev5"
     assert vdev.suffix == "a.dev"
     assert vdev.prerelease == ("a", 4, "", 0, "dev", 5)
     assert vrc.major == 1
     assert vrc.minor == 0
     assert vrc.patch == 0
-    assert vrc.main == "1.0.0"
-    assert Version.from_text("foo, version 1.0a4.dev5\nbar baz") == vdev
+    assert vrc.main == "1.0"
 
     incomplete_dev = Version("0.4.34dev")
     assert not incomplete_dev.is_final
     assert incomplete_dev.is_valid
     assert incomplete_dev.main == "0.4.34"
     assert incomplete_dev.prerelease == ("", 0, "", 0, "dev", 0)
     assert incomplete_dev.suffix == "dev"
 
-    # .from_text() can be used to filter out invalid versions as None
-    assert Version.from_text("Python 3.8.6", strict=True) is None
-    assert Version.from_text("Python 3.8.6") == Version("3.8.6")
-    assert Version.from_text("foo") is None
-    assert Version.from_text("1.0rc4") == vrc
-
     # Version() can be used in sets/dicts
     s = set()
     s.add(vrc)
     assert vrc in s
 
 
+def test_version_extraction():
+    x = Version.extracted_from_text("foo, version 1.0a4.dev5\nbar baz")
+    assert str(x) == "1.0a4.dev5"
+
+    p38 = Version("Python 3.8.6")
+    assert not p38.is_valid
+
+    p38 = Version.extracted_from_text("Python 3.8.6")
+    assert str(p38) == "3.8.6"
+    assert p38.is_valid
+
+
 def test_version_comparison():
     v10rc5 = Version("1.0rc5")
     assert v10rc5 > "0.9"
     assert v10rc5 > "1.0rc2"
     assert v10rc5 > "1.0rc2.dev10"
     assert v10rc5 > "1.0a5"
     assert v10rc5 < "1.0rc15"
@@ -877,15 +670,15 @@
         Version("1.0+foo.z"),
         Version("1.0+foo.z.8"),
         Version("1.0+foo.5"),
         Version("1.0+foo.7"),
     ])
 
 
-def test_version_pep_440():
+def test_version_ordering():
     verify_ordering([
         Version("1.dev0"),
         Version("1.0.dev456"),
         Version("1.0a1"),
         Version("1.0a2.dev456"),
         Version("1.0a12.dev456"),
         Version("1.0a12"),
@@ -905,12 +698,49 @@
         Version("1.1.dev1"),
     ])
 
 
 def verify_ordering(expected):
     # Jumble the given list of versions a bit, then sort them and verify they sort back to 'expected'
     given = sorted(expected, key=lambda x: x.text)
-    x = given.pop(len(given) // 2)
-    given.append(x)
+    mid_item = given.pop(len(given) // 2)
+    given.append(mid_item)
 
     assert given != expected
     assert sorted(given) == expected
+
+
+def test_version_pep_440():
+    vpost = Version("1.2.post")
+    assert vpost.is_valid
+    assert not vpost.prerelease
+    assert str(vpost) == "1.2.post"
+    assert vpost.pep_440 == "1.2.post0"
+
+    vrev5 = Version("1.2rev05")
+    assert str(vrev5) == "1.2rev05"
+    assert vrev5.is_valid
+    assert vrev5.pep_440 == "1.2.post5"
+    assert vrev5 > vpost
+
+    vrev5_canonical = Version("1.2rev05", canonical=True)
+    assert str(vrev5_canonical) == "1.2.post5"
+    assert vrev5_canonical.pep_440 == vrev5_canonical.text
+    assert vrev5_canonical == vrev5
+
+    vr6 = Version("1.2r6")
+    assert str(vr6) == "1.2r6"
+    assert vr6.is_valid
+    assert vr6.pep_440 == "1.2.post6"
+    assert vr6 > vrev5
+
+    vrev5dev3 = Version("1.2rev05.dev3")
+    assert vrev5dev3.prerelease
+    assert str(vrev5dev3) == "1.2rev05.dev3"
+    assert vrev5dev3.pep_440 == "1.2.rev5.dev3.post5"
+    assert vpost < vrev5dev3
+    assert vrev5 > vrev5dev3
+    assert vr6 > vrev5dev3
+
+    vrc1 = Version("v1.39.4-rc.1")
+    assert str(vrc1) == "1.39.4-rc.1"
+    assert vrc1.pep_440 == "1.39.4rc1"
```

### Comparing `runez-3.7.1/tests/test_render.py` & `runez-4.0.0/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_schema.py` & `runez-4.0.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_serialize.py` & `runez-4.0.0/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_slotted.py` & `runez-4.0.0/tests/test_slotted.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_system.py` & `runez-4.0.0/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_testing.py` & `runez-4.0.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.1/tests/test_thread.py` & `runez-4.0.0/tests/test_thread.py`

 * *Files identical despite different names*

