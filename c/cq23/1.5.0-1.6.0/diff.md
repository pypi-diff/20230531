# Comparing `tmp/cq23-1.5.0.tar.gz` & `tmp/cq23-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-1.5.0.tar", last modified: Wed May 31 11:09:02 2023, max compression
+gzip compressed data, was "cq23-1.6.0.tar", last modified: Wed May 31 12:43:34 2023, max compression
```

## Comparing `cq23-1.5.0.tar` & `cq23-1.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.890365 cq23-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-31 11:09:02.890365 cq23-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-31 11:08:55.000000 cq23-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 11:08:55.000000 cq23-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-31 11:09:02.894365 cq23-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.882365 cq23-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.886365 cq23-1.5.0/src/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-31 11:08:55.000000 cq23-1.5.0/src/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-31 11:08:55.000000 cq23-1.5.0/src/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-31 11:08:55.000000 cq23-1.5.0/src/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.886365 cq23-1.5.0/src/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-31 11:08:55.000000 cq23-1.5.0/src/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.886365 cq23-1.5.0/src/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-31 11:08:55.000000 cq23-1.5.0/src/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.890365 cq23-1.5.0/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-31 11:09:02.000000 cq23-1.5.0/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-31 11:09:02.000000 cq23-1.5.0/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:09:02.000000 cq23-1.5.0/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 11:09:02.000000 cq23-1.5.0/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 11:09:02.000000 cq23-1.5.0/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 11:09:02.000000 cq23-1.5.0/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.890365 cq23-1.5.0/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 11:08:55.000000 cq23-1.5.0/src/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-31 11:08:55.000000 cq23-1.5.0/src/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.890365 cq23-1.5.0/src/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-31 11:08:55.000000 cq23-1.5.0/src/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.890365 cq23-1.5.0/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-31 11:08:55.000000 cq23-1.5.0/src/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-31 11:08:55.000000 cq23-1.5.0/src/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-31 11:08:55.000000 cq23-1.5.0/src/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:02.890365 cq23-1.5.0/src/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:08:55.000000 cq23-1.5.0/src/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-31 11:08:55.000000 cq23-1.5.0/src/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:34.859208 cq23-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-31 12:43:34.859208 cq23-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-31 12:43:26.000000 cq23-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 12:43:26.000000 cq23-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-31 12:43:34.859208 cq23-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:34.855208 cq23-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:34.855208 cq23-1.6.0/src/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:26.000000 cq23-1.6.0/src/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-31 12:43:26.000000 cq23-1.6.0/src/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-31 12:43:26.000000 cq23-1.6.0/src/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-31 12:43:26.000000 cq23-1.6.0/src/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:34.855208 cq23-1.6.0/src/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:26.000000 cq23-1.6.0/src/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-31 12:43:26.000000 cq23-1.6.0/src/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:34.855208 cq23-1.6.0/src/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:26.000000 cq23-1.6.0/src/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-31 12:43:26.000000 cq23-1.6.0/src/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:34.855208 cq23-1.6.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-31 12:43:34.000000 cq23-1.6.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-31 12:43:34.000000 cq23-1.6.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:43:34.000000 cq23-1.6.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 12:43:34.000000 cq23-1.6.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 12:43:34.000000 cq23-1.6.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 12:43:34.000000 cq23-1.6.0/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:34.855208 cq23-1.6.0/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:26.000000 cq23-1.6.0/src/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 12:43:26.000000 cq23-1.6.0/src/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-31 12:43:26.000000 cq23-1.6.0/src/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:34.859208 cq23-1.6.0/src/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:26.000000 cq23-1.6.0/src/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-31 12:43:26.000000 cq23-1.6.0/src/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:34.859208 cq23-1.6.0/src/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:26.000000 cq23-1.6.0/src/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-31 12:43:26.000000 cq23-1.6.0/src/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-31 12:43:26.000000 cq23-1.6.0/src/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-31 12:43:26.000000 cq23-1.6.0/src/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:34.859208 cq23-1.6.0/src/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:43:26.000000 cq23-1.6.0/src/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-31 12:43:26.000000 cq23-1.6.0/src/zip/command.py
```

### Comparing `cq23-1.5.0/PKG-INFO` & `cq23-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.5.0
+Version: 1.6.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.5.0/setup.cfg` & `cq23-1.6.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 1.5.0
+version = 1.6.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls = 
@@ -18,14 +18,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	docker>=6.0.1
+	boto3>=1.29.143
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	cq23 = main.command:route_command
```

### Comparing `cq23-1.5.0/src/admin/aws.py` & `cq23-1.6.0/src/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-1.5.0/src/admin/builder.py` & `cq23-1.6.0/src/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-1.5.0/src/admin/worker.py` & `cq23-1.6.0/src/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-1.5.0/src/check/command.py` & `cq23-1.6.0/src/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.5.0/src/cleanup/command.py` & `cq23-1.6.0/src/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.5.0/src/cq23.egg-info/PKG-INFO` & `cq23-1.6.0/src/cq23.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.5.0
+Version: 1.6.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.5.0/src/cq23.egg-info/SOURCES.txt` & `cq23-1.6.0/src/cq23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cq23-1.5.0/src/main/command.py` & `cq23-1.6.0/src/main/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.5.0/src/main/utils.py` & `cq23-1.6.0/src/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-1.5.0/src/new_client/command.py` & `cq23-1.6.0/src/new_client/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.5.0/src/run_game/command.py` & `cq23-1.6.0/src/run_game/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.5.0/src/run_game/docker_tools.py` & `cq23-1.6.0/src/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-1.5.0/src/run_game/gcs.py` & `cq23-1.6.0/src/run_game/gcs.py`

 * *Files identical despite different names*

### Comparing `cq23-1.5.0/src/zip/command.py` & `cq23-1.6.0/src/zip/command.py`

 * *Files identical despite different names*

