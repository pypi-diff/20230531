# Comparing `tmp/mongo_tooling_metrics-1.0.6.tar.gz` & `tmp/mongo_tooling_metrics-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_tooling_metrics-1.0.6.tar", max compression
+gzip compressed data, was "mongo_tooling_metrics-1.0.7.tar", max compression
```

## Comparing `mongo_tooling_metrics-1.0.6.tar` & `mongo_tooling_metrics-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      877 2023-01-18 19:43:29.172133 mongo_tooling_metrics-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      692 2023-01-18 19:43:29.172133 mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/__init__.py
--rw-r--r--   0        0        0     1141 2023-01-18 19:43:29.172133 mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/base_hook.py
--rw-r--r--   0        0        0     2236 2023-01-18 19:43:29.172133 mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/base_metrics.py
--rw-r--r--   0        0        0     5338 2023-01-18 19:43:29.172133 mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/client.py
--rw-r--r--   0        0        0      584 2023-01-18 19:43:29.172133 mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/errors.py
--rw-r--r--   0        0        0      563 2023-01-18 19:43:29.172133 mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/lib/hooks.py
--rw-r--r--   0        0        0     6931 2023-01-18 19:43:29.172133 mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/lib/sub_metrics.py
--rw-r--r--   0        0        0     6015 2023-01-18 19:43:29.172133 mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/lib/top_level_metrics.py
--rw-r--r--   0        0        0      787 2023-01-18 19:43:29.172133 mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/lib/utils.py
--rw-r--r--   0        0        0      977 2023-01-18 19:43:29.172133 mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/registry.py
--rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 mongo_tooling_metrics-1.0.6/setup.py
--rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 mongo_tooling_metrics-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      877 2023-01-25 18:05:12.167707 mongo_tooling_metrics-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      692 2023-01-25 18:05:12.167707 mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/__init__.py
+-rw-r--r--   0        0        0     1141 2023-01-25 18:05:12.167707 mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/base_hook.py
+-rw-r--r--   0        0        0     2236 2023-01-25 18:05:12.167707 mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/base_metrics.py
+-rw-r--r--   0        0        0     5338 2023-01-25 18:05:12.167707 mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/client.py
+-rw-r--r--   0        0        0      584 2023-01-25 18:05:12.167707 mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/errors.py
+-rw-r--r--   0        0        0      563 2023-01-25 18:05:12.167707 mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/lib/hooks.py
+-rw-r--r--   0        0        0     7460 2023-01-25 18:05:12.167707 mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/lib/sub_metrics.py
+-rw-r--r--   0        0        0     6316 2023-01-25 18:05:12.167707 mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/lib/top_level_metrics.py
+-rw-r--r--   0        0        0      787 2023-01-25 18:05:12.167707 mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/lib/utils.py
+-rw-r--r--   0        0        0      977 2023-01-25 18:05:12.167707 mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/registry.py
+-rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 mongo_tooling_metrics-1.0.7/setup.py
+-rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 mongo_tooling_metrics-1.0.7/PKG-INFO
```

### Comparing `mongo_tooling_metrics-1.0.6/pyproject.toml` & `mongo_tooling_metrics-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mongo_tooling_metrics"
-version = "1.0.6"
+version = "1.0.7"
 description = "A slim library which leverages Pydantic to reliably collect type enforced metrics and store them to MongoDB."
 authors = ["Tausif Rahman <tausif.rahman@mongodb.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 distro = "^1.5.0"
 pydantic = "^1.8.2"
```

### Comparing `mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/__init__.py` & `mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/base_hook.py` & `mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/base_hook.py`

 * *Files identical despite different names*

### Comparing `mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/base_metrics.py` & `mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/client.py` & `mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/client.py`

 * *Files identical despite different names*

### Comparing `mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/errors.py` & `mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/errors.py`

 * *Files identical despite different names*

### Comparing `mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/lib/hooks.py` & `mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/lib/hooks.py`

 * *Files identical despite different names*

### Comparing `mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/lib/sub_metrics.py` & `mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/lib/sub_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Common sub metrics that are used internally at MongoDB."""
 
+import argparse
 import configparser
 from datetime import datetime
 import multiprocessing
+import optparse
 import os
 import socket
-from typing import Any, Dict, List, Optional
+import sys
+from typing import Any, Dict, List, Optional, Union
 
 import distro
 import git
 from mongo_tooling_metrics.base_metrics import SubMetrics
 
 
 class HostInfo(SubMetrics):
@@ -139,38 +142,56 @@
             return None
 
     def is_malformed(self) -> bool:
         """Confirm whether this instance has all expected fields."""
         return None in [self.artifact_dir, self.build_artifacts]
 
 
+class CommandInfo(SubMetrics):
+    """Class to store command-line information."""
+
+    command: List[str]
+    options: Optional[Dict[str, Any]]
+    positional_args: Optional[List[str]]
+
+    @classmethod
+    def generate_metrics(cls, parser: Union[argparse.ArgumentParser, optparse.OptionParser]):
+        """Get command line information to the best of our ability."""
+        try:
+            # The SCons parser is of type 'optparse.OptionParser' which does not
+            # have 'parse_known_args' but has 'parse_args' -- which has the same effect
+            known_args, unknown_args = parser.parse_known_args(sys.argv[1:]) if isinstance(
+                parser, argparse.ArgumentParser) else parser.parse_args(sys.argv[1:])
+            return cls(command=sys.argv, options=vars(known_args), positional_args=unknown_args)
+        except:
+            return cls(command=sys.argv, options=None, positional_args=None)
+
+    def is_malformed(self) -> bool:
+        """Confirm whether this instance has all expected fields."""
+        return None in [self.options, self.positional_args]
+
+
 SCONS_ENV_FILE = "scons_env.env"
 SCONS_SECTION_HEADER = "SCONS_ENV"
 
 
 class SConsInfo(SubMetrics):
-    """Class to store the SCons enviornment and options."""
+    """Class to store the SCons specific information."""
 
     env: Optional[Dict[str, Any]]
-    options: Optional[Dict[str, Any]]
 
     @classmethod
     def generate_metrics(
         cls,
         artifact_dir: str,
         env_vars: "SCons.Variables.Variables",
         env: "SCons.Script.SConscript.SConsEnvironment",
-        parser: "SCons.Script.SConsOptions.SConsOptionParser",
-        args: List[str],
     ):
         """Get SCons info to the best of our ability."""
-        return cls(
-            env=cls._get_scons_env_vars_dict(artifact_dir, env_vars, env),
-            options=cls._get_scons_options_dict(parser, args),
-        )
+        return cls(env=cls._get_scons_env_vars_dict(artifact_dir, env_vars, env))
 
     @staticmethod
     def _get_scons_env_vars_dict(
         artifact_dir: str,
         env_vars: "SCons.Variables.Variables",
         env: "SCons.Script.SConscript.SConsEnvironment",
     ) -> Optional[Dict[str, Any]]:
@@ -191,22 +212,10 @@
             config = configparser.ConfigParser()
             config.read(scons_env_filepath)
             str_dict = dict(config[SCONS_SECTION_HEADER])
             return {key: eval(val) for key, val in str_dict.items()}  # pylint: disable=eval-used
         except:
             return None
 
-    @staticmethod
-    def _get_scons_options_dict(
-        parser: "SCons.Script.SConsOptions.SConsOptionParser",
-        args: List[str],
-    ) -> Optional[Dict[str, Any]]:
-        """Get the scons cli options set by users."""
-        try:
-            scons_options, _ = parser.parse_args(args)
-            return vars(scons_options)
-        except:
-            return None
-
     def is_malformed(self) -> bool:
         """Confirm whether this instance has all expected fields."""
-        return None in [self.env, self.options]
+        return self.env is None
```

### Comparing `mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/lib/top_level_metrics.py` & `mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/lib/top_level_metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,138 +2,144 @@
 from datetime import datetime
 import os
 import sys
 from typing import List, Optional
 from mongo_tooling_metrics import get_hook, __version__
 from mongo_tooling_metrics.base_metrics import TopLevelMetrics
 from mongo_tooling_metrics.lib.hooks import ExitHook
-from mongo_tooling_metrics.lib.sub_metrics import BuildInfo, GitInfo, HostInfo, SConsInfo
+from mongo_tooling_metrics.lib.sub_metrics import CommandInfo, BuildInfo, GitInfo, HostInfo, SConsInfo
 
 
 class ResmokeToolingMetrics(TopLevelMetrics):
     """Class to store resmoke tooling metrics."""
 
     source: str
     utc_starttime: datetime
     utc_endtime: datetime
     host_info: HostInfo
     git_info: GitInfo
     exit_code: Optional[int]
-    command: List[str]
+    command_info: CommandInfo
     module_info: List[GitInfo]
     tooling_metrics_version: str
 
     @classmethod
     def generate_metrics(
         cls,
         utc_starttime: datetime,
+        parser: argparse.ArgumentParser,
     ):
         """Get resmoke metrics to the best of our ability."""
         exit_hook = get_hook(ExitHook)
         return cls(
             source='resmoke',
             utc_starttime=utc_starttime,
             utc_endtime=datetime.utcnow(),
             host_info=HostInfo.generate_metrics(),
             git_info=GitInfo.generate_metrics('.'),
             exit_code=None if exit_hook.is_malformed() else exit_hook.exit_code,
-            command=sys.argv,
+            command_info=CommandInfo.generate_metrics(parser),
             module_info=GitInfo.modules_generate_metrics(),
             tooling_metrics_version=__version__,
         )
 
     def is_malformed(self) -> bool:
         """Confirm whether this instance has all expected fields."""
-        sub_metrics = self.module_info + [self.git_info] + [self.host_info]
+        sub_metrics = self.module_info + [
+            self.git_info,
+            self.host_info,
+            self.command_info,
+        ]
         return self.exit_code is None or any(metrics.is_malformed() for metrics in sub_metrics)
 
 
 class SConsToolingMetrics(TopLevelMetrics):
     """Class to store scons tooling metrics."""
 
     source: str
     utc_starttime: datetime
     utc_endtime: datetime
     host_info: HostInfo
     git_info: GitInfo
     exit_code: Optional[int]
     build_info: BuildInfo
     scons_info: SConsInfo
-    command: List[str]
+    command_info: CommandInfo
     module_info: List[GitInfo]
     tooling_metrics_version: str
 
     @classmethod
     def generate_metrics(
         cls,
         utc_starttime: datetime,
         artifact_dir: str,
         env_vars: "SCons.Variables.Variables",
         env: "SCons.Script.SConscript.SConsEnvironment",
         parser: "SCons.Script.SConsOptions.SConsOptionParser",
-        args: List[str],
     ):
         """Get scons metrics to the best of our ability."""
         exit_hook = get_hook(ExitHook)
         return cls(
             source='scons',
             utc_starttime=utc_starttime,
             utc_endtime=datetime.utcnow(),
             host_info=HostInfo.generate_metrics(),
             git_info=GitInfo.generate_metrics('.'),
             build_info=BuildInfo.generate_metrics(utc_starttime, artifact_dir),
-            scons_info=SConsInfo.generate_metrics(artifact_dir, env_vars, env, parser, args),
+            scons_info=SConsInfo.generate_metrics(artifact_dir, env_vars, env),
+            command_info=CommandInfo.generate_metrics(parser),
             exit_code=None if exit_hook.is_malformed() else exit_hook.exit_code,
-            command=sys.argv,
             module_info=GitInfo.modules_generate_metrics(),
             tooling_metrics_version=__version__,
         )
 
     def is_malformed(self) -> bool:
         """Confirm whether this instance has all expected fields."""
         sub_metrics = self.module_info + [
             self.git_info,
             self.host_info,
             self.build_info,
             self.scons_info,
+            self.command_info,
         ]
         return self.exit_code is None or any(metrics.is_malformed() for metrics in sub_metrics)
 
 
 class NinjaToolingMetrics(TopLevelMetrics):
     """Class to store ninja tooling metrics."""
 
     source: str
     utc_starttime: datetime
     utc_endtime: datetime
     host_info: HostInfo
     git_info: GitInfo
     exit_code: Optional[int]
     build_info: BuildInfo
-    command: List[str]
+    command_info: CommandInfo
     module_info: List[GitInfo]
     tooling_metrics_version: str
 
     @classmethod
     def generate_metrics(
         cls,
         utc_starttime: datetime,
+        parser: argparse.ArgumentParser,
     ):
         """Get scons metrics to the best of our ability."""
         artifact_dir = cls._get_ninja_artifact_dir()
         exit_hook = get_hook(ExitHook)
         return cls(
             source='ninja',
             utc_starttime=utc_starttime,
             utc_endtime=datetime.utcnow(),
             host_info=HostInfo.generate_metrics(),
             git_info=GitInfo.generate_metrics('.'),
             build_info=BuildInfo.generate_metrics(utc_starttime, artifact_dir),
+            command_info=CommandInfo.generate_metrics(parser),
             exit_code=None if exit_hook.is_malformed() else exit_hook.exit_code,
-            command=sys.argv,
             module_info=GitInfo.modules_generate_metrics(),
             tooling_metrics_version=__version__,
         )
 
     @classmethod
     def _get_ninja_file(cls) -> Optional[str]:
         """Get the ninja file from sys.argv -- return 'None' if this fails."""
@@ -167,9 +173,10 @@
 
     def is_malformed(self) -> bool:
         """Confirm whether this instance has all expected fields."""
         sub_metrics = self.module_info + [
             self.git_info,
             self.host_info,
             self.build_info,
+            self.command_info,
         ]
         return self.exit_code is None or any(metrics.is_malformed() for metrics in sub_metrics)
```

### Comparing `mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/lib/utils.py` & `mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/lib/utils.py`

 * *Files identical despite different names*

### Comparing `mongo_tooling_metrics-1.0.6/src/mongo_tooling_metrics/registry.py` & `mongo_tooling_metrics-1.0.7/src/mongo_tooling_metrics/registry.py`

 * *Files identical despite different names*

### Comparing `mongo_tooling_metrics-1.0.6/setup.py` & `mongo_tooling_metrics-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'gitpython>=3.1.29,<4.0.0',
  'pydantic>=1.8.2,<2.0.0',
  'pymongo>=4.3.3,<5.0.0',
  'setuptools>=58.1.0,<59.0.0']
 
 setup_kwargs = {
     'name': 'mongo-tooling-metrics',
-    'version': '1.0.6',
+    'version': '1.0.7',
     'description': 'A slim library which leverages Pydantic to reliably collect type enforced metrics and store them to MongoDB.',
     'long_description': 'None',
     'author': 'Tausif Rahman',
     'author_email': 'tausif.rahman@mongodb.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mongo_tooling_metrics-1.0.6/PKG-INFO` & `mongo_tooling_metrics-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-tooling-metrics
-Version: 1.0.6
+Version: 1.0.7
 Summary: A slim library which leverages Pydantic to reliably collect type enforced metrics and store them to MongoDB.
 Author: Tausif Rahman
 Author-email: tausif.rahman@mongodb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

