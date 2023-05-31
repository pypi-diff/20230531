# Comparing `tmp/wicked_expressions-0.6.2.tar.gz` & `tmp/wicked_expressions-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicked_expressions-0.6.2.tar", max compression
+gzip compressed data, was "wicked_expressions-0.6.3.tar", max compression
```

## Comparing `wicked_expressions-0.6.2.tar` & `wicked_expressions-0.6.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1061 2023-05-30 11:35:04.948978 wicked_expressions-0.6.2/LICENSE
--rw-r--r--   0        0        0     2119 2023-05-30 11:35:04.948978 wicked_expressions-0.6.2/README.md
--rw-r--r--   0        0        0     1219 2023-05-30 11:36:41.251602 wicked_expressions-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      321 2023-05-30 11:36:41.231601 wicked_expressions-0.6.2/wicked_expressions/__init__.py
--rw-r--r--   0        0        0      709 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/api.bolt
--rw-r--r--   0        0        0     9460 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/comparison.bolt
--rw-r--r--   0        0        0      305 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/config.bolt
--rw-r--r--   0        0        0     1850 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/internal_api.bolt
--rw-r--r--   0        0        0      341 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/nbtlib.bolt
--rw-r--r--   0        0        0     8436 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/raw_operations.bolt
--rw-r--r--   0        0        0      375 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/rebindable.bolt
--rw-r--r--   0        0        0      596 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/safe_load.bolt
--rw-r--r--   0        0        0     3118 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/sources.bolt
--rw-r--r--   0        0        0     1181 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/utils.bolt
--rw-r--r--   0        0        0     1221 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/var.bolt
--rw-r--r--   0        0        0     5253 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/var_sources.bolt
--rw-r--r--   0        0        0        0 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/py.typed
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-31 13:33:30.701034 wicked_expressions-0.6.3/LICENSE
+-rw-r--r--   0        0        0     2119 2023-05-31 13:33:30.701034 wicked_expressions-0.6.3/README.md
+-rw-r--r--   0        0        0     1219 2023-05-31 13:35:09.455099 wicked_expressions-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-05-31 13:35:09.435098 wicked_expressions-0.6.3/wicked_expressions/__init__.py
+-rw-r--r--   0        0        0      709 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/modules/api.bolt
+-rw-r--r--   0        0        0     9403 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/modules/comparison.bolt
+-rw-r--r--   0        0        0      305 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/modules/config.bolt
+-rw-r--r--   0        0        0     1850 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/modules/internal_api.bolt
+-rw-r--r--   0        0        0      341 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/modules/nbtlib.bolt
+-rw-r--r--   0        0        0     8436 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/modules/raw_operations.bolt
+-rw-r--r--   0        0        0      375 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/modules/rebindable.bolt
+-rw-r--r--   0        0        0      596 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/modules/safe_load.bolt
+-rw-r--r--   0        0        0     3118 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/modules/sources.bolt
+-rw-r--r--   0        0        0     1181 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/modules/utils.bolt
+-rw-r--r--   0        0        0     1221 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/modules/var.bolt
+-rw-r--r--   0        0        0     5253 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/modules/var_sources.bolt
+-rw-r--r--   0        0        0        0 2023-05-31 13:33:30.709034 wicked_expressions-0.6.3/wicked_expressions/py.typed
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.6.3/PKG-INFO
```

### Comparing `wicked_expressions-0.6.2/LICENSE` & `wicked_expressions-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.2/README.md` & `wicked_expressions-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.2/pyproject.toml` & `wicked_expressions-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wicked_expressions"
-version = "0.6.2"
+version = "0.6.3"
 description = "Extension of bolt-expressions written in Bolt."
 authors = ["Yeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/wicked-expressions"
 readme = "README.md"
```

### Comparing `wicked_expressions-0.6.2/wicked_expressions/modules/api.bolt` & `wicked_expressions-0.6.3/wicked_expressions/modules/api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.2/wicked_expressions/modules/comparison.bolt` & `wicked_expressions-0.6.3/wicked_expressions/modules/comparison.bolt`

 * *Files 1% similar despite different names*

```diff
@@ -47,20 +47,19 @@
     def autonest(self):
         nest_path = ~/nested_{self.incr()}
 
         with runtime.scope() as commands:
             yield True
         if not commands:
             return
-        if score foo tmp matches 10:
-            if len(commands) == 1:
-                runtime.commands.append(commands[0])
-            else:
-                execute function nest_path:
-                    runtime.commands.extend(commands)
+        if len(commands) == 1:
+            runtime.commands.append(commands[0])
+        else:
+            execute function nest_path:
+                runtime.commands.extend(commands)
 
     @contextmanager
     def __branch__(self):
         score_count = 0
 
         if isinstance(self.arg_0, self.ScoreSource):
             score_count += 1
```

### Comparing `wicked_expressions-0.6.2/wicked_expressions/modules/internal_api.bolt` & `wicked_expressions-0.6.3/wicked_expressions/modules/internal_api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.2/wicked_expressions/modules/raw_operations.bolt` & `wicked_expressions-0.6.3/wicked_expressions/modules/raw_operations.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.2/wicked_expressions/modules/safe_load.bolt` & `wicked_expressions-0.6.3/wicked_expressions/modules/safe_load.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.2/wicked_expressions/modules/sources.bolt` & `wicked_expressions-0.6.3/wicked_expressions/modules/sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.2/wicked_expressions/modules/utils.bolt` & `wicked_expressions-0.6.3/wicked_expressions/modules/utils.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.2/wicked_expressions/modules/var.bolt` & `wicked_expressions-0.6.3/wicked_expressions/modules/var.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.2/wicked_expressions/modules/var_sources.bolt` & `wicked_expressions-0.6.3/wicked_expressions/modules/var_sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.2/PKG-INFO` & `wicked_expressions-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicked-expressions
-Version: 0.6.2
+Version: 0.6.3
 Summary: Extension of bolt-expressions written in Bolt.
 Home-page: https://github.com/reapermc/wicked-expressions
 License: MIT
 Keywords: beet,bolt,minecraft,minecraft-commands,mcfunction
 Author: Yeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

