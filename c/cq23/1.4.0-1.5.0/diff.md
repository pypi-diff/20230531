# Comparing `tmp/cq23-1.4.0.tar.gz` & `tmp/cq23-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-1.4.0.tar", last modified: Sat May 27 04:34:11 2023, max compression
+gzip compressed data, was "cq23-1.5.0.tar", last modified: Wed May 31 11:09:02 2023, max compression
```

## Comparing `cq23-1.4.0.tar` & `cq23-1.5.0.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.879390 cq23-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-27 04:34:11.879390 cq23-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-27 04:34:03.000000 cq23-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-27 04:34:03.000000 cq23-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-27 04:34:11.879390 cq23-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.875390 cq23-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.875390 cq23-1.4.0/src/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:03.000000 cq23-1.4.0/src/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-27 04:34:03.000000 cq23-1.4.0/src/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.875390 cq23-1.4.0/src/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:03.000000 cq23-1.4.0/src/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-27 04:34:03.000000 cq23-1.4.0/src/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.875390 cq23-1.4.0/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-27 04:34:11.000000 cq23-1.4.0/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-27 04:34:11.000000 cq23-1.4.0/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 04:34:11.000000 cq23-1.4.0/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-27 04:34:11.000000 cq23-1.4.0/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-27 04:34:11.000000 cq23-1.4.0/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-27 04:34:11.000000 cq23-1.4.0/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.875390 cq23-1.4.0/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:03.000000 cq23-1.4.0/src/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-27 04:34:03.000000 cq23-1.4.0/src/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-27 04:34:03.000000 cq23-1.4.0/src/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.875390 cq23-1.4.0/src/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:03.000000 cq23-1.4.0/src/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-27 04:34:03.000000 cq23-1.4.0/src/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.879390 cq23-1.4.0/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:03.000000 cq23-1.4.0/src/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-27 04:34:03.000000 cq23-1.4.0/src/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-27 04:34:03.000000 cq23-1.4.0/src/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-27 04:34:03.000000 cq23-1.4.0/src/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.879390 cq23-1.4.0/src/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:03.000000 cq23-1.4.0/src/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-27 04:34:03.000000 cq23-1.4.0/src/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.890365 cq23-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-31 11:09:02.890365 cq23-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-31 11:08:55.000000 cq23-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 11:08:55.000000 cq23-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-31 11:09:02.894365 cq23-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.882365 cq23-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.886365 cq23-1.5.0/src/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-31 11:08:55.000000 cq23-1.5.0/src/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-31 11:08:55.000000 cq23-1.5.0/src/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-31 11:08:55.000000 cq23-1.5.0/src/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.886365 cq23-1.5.0/src/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-31 11:08:55.000000 cq23-1.5.0/src/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.886365 cq23-1.5.0/src/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-31 11:08:55.000000 cq23-1.5.0/src/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.890365 cq23-1.5.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-31 11:09:02.000000 cq23-1.5.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-31 11:09:02.000000 cq23-1.5.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:09:02.000000 cq23-1.5.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 11:09:02.000000 cq23-1.5.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 11:09:02.000000 cq23-1.5.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 11:09:02.000000 cq23-1.5.0/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.890365 cq23-1.5.0/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 11:08:55.000000 cq23-1.5.0/src/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-31 11:08:55.000000 cq23-1.5.0/src/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.890365 cq23-1.5.0/src/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-31 11:08:55.000000 cq23-1.5.0/src/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.890365 cq23-1.5.0/src/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-31 11:08:55.000000 cq23-1.5.0/src/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-31 11:08:55.000000 cq23-1.5.0/src/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-31 11:08:55.000000 cq23-1.5.0/src/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.890365 cq23-1.5.0/src/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-31 11:08:55.000000 cq23-1.5.0/src/zip/command.py
```

### Comparing `cq23-1.4.0/PKG-INFO` & `cq23-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.4.0
+Version: 1.5.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.4.0/setup.cfg` & `cq23-1.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 1.4.0
+version = 1.5.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-1.4.0/src/check/command.py` & `cq23-1.5.0/src/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.4.0/src/cleanup/command.py` & `cq23-1.5.0/src/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.4.0/src/cq23.egg-info/PKG-INFO` & `cq23-1.5.0/src/cq23.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.4.0
+Version: 1.5.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.4.0/src/cq23.egg-info/SOURCES.txt` & `cq23-1.5.0/src/cq23.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 README.md
 pyproject.toml
 setup.cfg
+src/admin/__init__.py
+src/admin/aws.py
+src/admin/builder.py
+src/admin/worker.py
 src/check/__init__.py
 src/check/command.py
 src/cleanup/__init__.py
 src/cleanup/command.py
 src/cq23.egg-info/PKG-INFO
 src/cq23.egg-info/SOURCES.txt
 src/cq23.egg-info/dependency_links.txt
```

### Comparing `cq23-1.4.0/src/main/command.py` & `cq23-1.5.0/src/main/command.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import sys
 
+from admin.builder import command as builder
+from admin.worker import command as worker
 from check.command import check
 from cleanup.command import cleanup
 from new_client.command import new_client
 from run_game.command import run_game
 from zip.command import zip
 
 from .utils import restore_cwd
@@ -29,13 +31,15 @@
 
     first_arg_mapping = {
         "new": new_client,
         "run": run_game,
         "cleanup": cleanup,
         "zip": zip,
         "check": check,
+        "worker": worker,
+        "builder": builder,
     }
 
     if not command_args or command_args[0].lower() not in first_arg_mapping.keys():
         help_message()
     else:
         first_arg_mapping[command_args[0].lower()](*command_args[1:])
```

### Comparing `cq23-1.4.0/src/new_client/command.py` & `cq23-1.5.0/src/new_client/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.4.0/src/run_game/command.py` & `cq23-1.5.0/src/run_game/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.4.0/src/run_game/docker_tools.py` & `cq23-1.5.0/src/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-1.4.0/src/run_game/gcs.py` & `cq23-1.5.0/src/run_game/gcs.py`

 * *Files identical despite different names*

### Comparing `cq23-1.4.0/src/zip/command.py` & `cq23-1.5.0/src/zip/command.py`

 * *Files identical despite different names*

