# Comparing `tmp/jaaql-monitor-1.2.47.tar.gz` & `tmp/jaaql-monitor-1.2.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.47.tar", last modified: Sat May  6 11:45:41 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.58.tar", last modified: Wed May 31 17:57:23 2023, max compression
```

## Comparing `jaaql-monitor-1.2.47.tar` & `jaaql-monitor-1.2.58.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:45:41.951510 jaaql-monitor-1.2.47/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.47/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:45:41.950511 jaaql-monitor-1.2.47/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.47/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 11:45:41.946513 jaaql-monitor-1.2.47/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:45:41.000000 jaaql-monitor-1.2.47/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-06 11:45:41.000000 jaaql-monitor-1.2.47/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:45:41.000000 jaaql-monitor-1.2.47/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-06 11:45:41.000000 jaaql-monitor-1.2.47/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 11:45:41.000000 jaaql-monitor-1.2.47/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 11:45:41.949511 jaaql-monitor-1.2.47/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.47/monitor/__init__.py
--rw-rw-rw-   0        0        0    25619 2023-05-06 11:45:27.000000 jaaql-monitor-1.2.47/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-06 11:45:31.000000 jaaql-monitor-1.2.47/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-06 11:45:41.951510 jaaql-monitor-1.2.47/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.47/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 17:57:23.217194 jaaql-monitor-1.2.58/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.58/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-31 17:57:23.217194 jaaql-monitor-1.2.58/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.58/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 17:57:23.210192 jaaql-monitor-1.2.58/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-31 17:57:23.000000 jaaql-monitor-1.2.58/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-31 17:57:23.000000 jaaql-monitor-1.2.58/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 17:57:23.000000 jaaql-monitor-1.2.58/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-31 17:57:23.000000 jaaql-monitor-1.2.58/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 17:57:23.000000 jaaql-monitor-1.2.58/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 17:57:23.215191 jaaql-monitor-1.2.58/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.58/monitor/__init__.py
+-rw-rw-rw-   0        0        0    26493 2023-05-06 18:11:59.000000 jaaql-monitor-1.2.58/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-31 17:57:10.000000 jaaql-monitor-1.2.58/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-31 17:57:23.217194 jaaql-monitor-1.2.58/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.58/setup.py
```

### Comparing `jaaql-monitor-1.2.47/LICENSE.txt` & `jaaql-monitor-1.2.58/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.47/PKG-INFO` & `jaaql-monitor-1.2.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.47
+Version: 1.2.58
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.47/README.md` & `jaaql-monitor-1.2.58/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.47/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.58/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.47
+Version: 1.2.58
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.47/monitor/main.py` & `jaaql-monitor-1.2.58/monitor/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 ROWS_MAX = 25
 
 METHOD__post = "POST"
 METHOD__get = "GET"
 
 ARGS__encoded_config = ['-e', '--encoded-config']
 ARGS__config = ['-c', '--config']
+ARGS__parameter = ['-p', '--parameter']
 
 
 class JAAQLMonitorException(Exception):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
@@ -100,14 +101,15 @@
         self.is_verbose = False
         self.single_query = False
         self.is_debugging = False
         self.file_name = None
         self.cur_file_line = 0
         self.file_lines = []
         self.override_url = None
+        self.parameters = {}
 
         self.do_exit = True
 
         self.database_override = None
         self.is_transactional = True
 
     def set_current_connection(self, connection: ConnectionInfo):
@@ -359,30 +361,29 @@
 
     print_buffer = dump_buffer(state, "")
     if len(lines_with_line_number) != 0:
         line_err_num = int(lines_with_line_number[0].split("LINE ")[1].split(":")[0])
         state.cur_file_line = line_err_num
         buffer_lines = state.fetched_query.strip().replace("\r\n", "\n").split("\n")
         start_line_num = max(0, line_err_num - 10) + 1
-        end_line_num = min(line_err_num + 3, len(buffer_lines)) + 1
+        end_line_num = min(line_err_num, len(buffer_lines)) + 1
         buffer_lines = buffer_lines[start_line_num - 1:end_line_num - 1]
 
         marker_line = marker_lines[0]
         marker_line = marker_line[lines_with_line_number[0].index(":"):]
         marker_line = "     " + marker_line
 
+        err = "\n".join(err.replace("\r\n", "\n").split("\n")[:-4])
+
         buffer_lines = [str(start_line_num + idx).rjust(5, '0') + "> " +
-                        (line + "\n" + marker_line if start_line_num + idx == line_err_num else line)
+                        (line + "\n" + marker_line + "\n" + err if start_line_num + idx == line_err_num else line)
                         for idx, line in zip(range(len(buffer_lines)), buffer_lines)]
 
-        print(len(err.replace("\r\n", "\n").split("\n")))
-
-        err = "\n".join(err.replace("\r\n", "\n").split("\n")[:-2])
-        err = err + "\n" + "\n".join(buffer_lines)
-        err = "\\<b\\>" + err + "\\<\\b\\>"
+        err = "\\<b>" + err + "\\</b>\n\n" + "\n".join(buffer_lines)
+        err = err + "\n\n"
     get_message(state, err, line_offset, print_buffer)
 
 
 def print_error(state, err, line_offset: int = 0):
     get_message(state, err, line_offset, dump_buffer(state, ""))
 
 
@@ -417,14 +418,17 @@
 
     if res.status_code != 200:
         print_error(state, "Error registering jaaql account '%s' with username '%s', received status code %d and message:\n\n\t%s" %
                     (credentials_name, connection_info.username, res.status_code, res.text))
 
 
 def on_go(state):
+    for parameter, value in state.parameters.items():
+        state.fetched_query = state.fetched_query.replace("{{" + parameter + "}}", value)
+
     send_json = {"query": state.fetched_query}
     cur_conn = state.get_current_connection()
     if cur_conn.database is not None:
         send_json["database"] = cur_conn.database
     if state.database_override is not None:
         send_json["database"] = state.database_override
     if not state.is_transactional:
@@ -556,14 +560,32 @@
     state.is_debugging = len([arg for arg in args if arg in ['-d', '--debugging']]) != 0
     state.single_query = len([arg for arg in args if arg in ['-s', '--single-query']]) != 0
 
     if state.is_verbose:
         print_version()
 
     for arg, arg_idx in zip(args, range(len(args))):
+        if arg not in ARGS__parameter:
+            continue
+
+        if arg_idx == len(args) - 1:
+            print_error(state, "The parameter flag is the last argument. You need to supply a parameter name")
+
+        if arg_idx == len(args) - 2:
+            print_error(state, "The parameter name is the last argument. You need to supply a parameter value")
+
+        parameter_name = args[arg_idx + 1]
+        parameter_value = args[arg_idx + 2]
+
+        if parameter_name in state.parameters:
+            print_error(state, "The parameter '" + parameter_name + "' has already been supplied")
+
+        state.parameters[parameter_name] = parameter_value
+
+    for arg, arg_idx in zip(args, range(len(args))):
         if arg not in ARGS__encoded_config and arg not in ARGS__config:
             continue
 
         if arg_idx == len(args) - 1:
             print_error(state, "The config flag is the last argument. You need to supply a file")
 
         configuration_name = args[arg_idx + 1]
```

### Comparing `jaaql-monitor-1.2.47/setup.py` & `jaaql-monitor-1.2.58/setup.py`

 * *Files identical despite different names*

