# Comparing `tmp/jaaql-monitor-1.2.58.tar.gz` & `tmp/jaaql-monitor-1.2.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.58.tar", last modified: Wed May 31 17:57:23 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.61.tar", last modified: Wed May 31 20:49:33 2023, max compression
```

## Comparing `jaaql-monitor-1.2.58.tar` & `jaaql-monitor-1.2.61.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 17:57:23.217194 jaaql-monitor-1.2.58/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.58/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-31 17:57:23.217194 jaaql-monitor-1.2.58/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.58/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 17:57:23.210192 jaaql-monitor-1.2.58/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-31 17:57:23.000000 jaaql-monitor-1.2.58/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-31 17:57:23.000000 jaaql-monitor-1.2.58/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 17:57:23.000000 jaaql-monitor-1.2.58/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-31 17:57:23.000000 jaaql-monitor-1.2.58/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 17:57:23.000000 jaaql-monitor-1.2.58/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 17:57:23.215191 jaaql-monitor-1.2.58/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.58/monitor/__init__.py
--rw-rw-rw-   0        0        0    26493 2023-05-06 18:11:59.000000 jaaql-monitor-1.2.58/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-31 17:57:10.000000 jaaql-monitor-1.2.58/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-31 17:57:23.217194 jaaql-monitor-1.2.58/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.58/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:49:33.461475 jaaql-monitor-1.2.61/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.61/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-31 20:49:33.461475 jaaql-monitor-1.2.61/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.61/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 20:49:33.458476 jaaql-monitor-1.2.61/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-31 20:49:33.000000 jaaql-monitor-1.2.61/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-31 20:49:33.000000 jaaql-monitor-1.2.61/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 20:49:33.000000 jaaql-monitor-1.2.61/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-31 20:49:33.000000 jaaql-monitor-1.2.61/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 20:49:33.000000 jaaql-monitor-1.2.61/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 20:49:33.460475 jaaql-monitor-1.2.61/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.61/monitor/__init__.py
+-rw-rw-rw-   0        0        0    27616 2023-05-31 20:48:58.000000 jaaql-monitor-1.2.61/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-31 20:49:18.000000 jaaql-monitor-1.2.61/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-31 20:49:33.462475 jaaql-monitor-1.2.61/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.61/setup.py
```

### Comparing `jaaql-monitor-1.2.58/LICENSE.txt` & `jaaql-monitor-1.2.61/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.58/PKG-INFO` & `jaaql-monitor-1.2.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.58
+Version: 1.2.61
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.58/README.md` & `jaaql-monitor-1.2.61/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.58/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.61/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.58
+Version: 1.2.61
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.58/monitor/main.py` & `jaaql-monitor-1.2.61/monitor/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 ROWS_MAX = 25
 
 METHOD__post = "POST"
 METHOD__get = "GET"
 
 ARGS__encoded_config = ['-e', '--encoded-config']
 ARGS__config = ['-c', '--config']
+ARGS__folder_config = ['-f', '--folder-config']
 ARGS__parameter = ['-p', '--parameter']
 
 
 class JAAQLMonitorException(Exception):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -578,14 +579,37 @@
 
         if parameter_name in state.parameters:
             print_error(state, "The parameter '" + parameter_name + "' has already been supplied")
 
         state.parameters[parameter_name] = parameter_value
 
     for arg, arg_idx in zip(args, range(len(args))):
+        if arg not in ARGS__folder_config:
+            continue
+
+        if arg_idx == len(args) - 1:
+            print_error(state, "The folder config flag is the last argument. You need to supply a file")
+
+        configuration_folder = args[arg_idx + 1]
+
+        for config_file in os.listdir(configuration_folder):
+            full_file_name = os.path.join(configuration_folder, config_file)
+            if config_file.endswith(".email-credentials.txt"):
+                configuration_name = config_file[0:-len(".email.credentials.txt")]
+            elif config_file.endswith(".credentials.txt"):
+                configuration_name = config_file[0:-len(".credentials.txt")]
+            else:
+                raise JAAQLMonitorException("Unrecognised file extension for file " + full_file_name)
+
+            if configuration_name in state.connections:
+                print_error(state, "The configuration with name '" + configuration_name + "' already exists")
+
+            state.connections[configuration_name] = full_file_name
+
+    for arg, arg_idx in zip(args, range(len(args))):
         if arg not in ARGS__encoded_config and arg not in ARGS__config:
             continue
 
         if arg_idx == len(args) - 1:
             print_error(state, "The config flag is the last argument. You need to supply a file")
 
         configuration_name = args[arg_idx + 1]
@@ -594,15 +618,15 @@
             candidate_content_or_file_name = args[arg_idx + 2]
 
         # The following branch of logic will use the supplied configuration name as the file name and set the configuration name to default
         if candidate_content_or_file_name is None or candidate_content_or_file_name.startswith("<") or candidate_content_or_file_name.startswith("-"):
             candidate_content_or_file_name = configuration_name
             configuration_name = DEFAULT_CONNECTION
 
-        if candidate_content_or_file_name in state.connections:
+        if configuration_name in state.connections:
             print_error(state, "The configuration with name '" + configuration_name + "' already exists")
 
         state.connections[configuration_name] = candidate_content_or_file_name
 
         if arg in ARGS__encoded_config:
             content_split = candidate_content_or_file_name.split(":")
```

### Comparing `jaaql-monitor-1.2.58/setup.py` & `jaaql-monitor-1.2.61/setup.py`

 * *Files identical despite different names*

