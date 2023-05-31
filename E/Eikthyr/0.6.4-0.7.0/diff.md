# Comparing `tmp/Eikthyr-0.6.4.tar.gz` & `tmp/Eikthyr-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Eikthyr-0.6.4.tar", last modified: Fri Jan 13 15:20:05 2023, max compression
+gzip compressed data, was "Eikthyr-0.7.0.tar", last modified: Wed May 31 07:47:05 2023, max compression
```

## Comparing `Eikthyr-0.6.4.tar` & `Eikthyr-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 natsuki  (197609) None     (197121)        0 2023-01-13 15:20:05.223962 Eikthyr-0.6.4/
-drwxr-xr-x   0 natsuki  (197609) None     (197121)        0 2023-01-13 15:20:05.218978 Eikthyr-0.6.4/Eikthyr/
--rw-r--r--   0 natsuki  (197609) None     (197121)     1204 2023-01-13 15:07:53.000000 Eikthyr-0.6.4/Eikthyr/__init__.py
--rw-r--r--   0 natsuki  (197609) None     (197121)     4004 2023-01-13 14:50:21.000000 Eikthyr-0.6.4/Eikthyr/cache.py
--rw-r--r--   0 natsuki  (197609) None     (197121)     1746 2023-01-13 14:50:21.000000 Eikthyr-0.6.4/Eikthyr/cmd.py
--rw-r--r--   0 natsuki  (197609) None     (197121)     4944 2023-01-13 14:50:21.000000 Eikthyr-0.6.4/Eikthyr/data.py
--rw-r--r--   0 natsuki  (197609) None     (197121)     1632 2023-01-13 14:50:21.000000 Eikthyr-0.6.4/Eikthyr/envcheck.py
--rw-r--r--   0 natsuki  (197609) None     (197121)      848 2023-01-13 14:50:21.000000 Eikthyr-0.6.4/Eikthyr/logging.py
--rw-r--r--   0 natsuki  (197609) None     (197121)     2952 2023-01-13 14:50:21.000000 Eikthyr-0.6.4/Eikthyr/param.py
--rw-r--r--   0 natsuki  (197609) None     (197121)     1966 2023-01-13 14:50:21.000000 Eikthyr-0.6.4/Eikthyr/run.py
--rw-r--r--   0 natsuki  (197609) None     (197121)     2267 2023-01-13 14:50:21.000000 Eikthyr-0.6.4/Eikthyr/specialtask.py
--rw-r--r--   0 natsuki  (197609) None     (197121)     7076 2023-01-13 14:50:21.000000 Eikthyr-0.6.4/Eikthyr/task.py
-drwxr-xr-x   0 natsuki  (197609) None     (197121)        0 2023-01-13 15:20:05.222964 Eikthyr-0.6.4/Eikthyr.egg-info/
--rw-r--r--   0 natsuki  (197609) None     (197121)      730 2023-01-13 15:20:05.000000 Eikthyr-0.6.4/Eikthyr.egg-info/PKG-INFO
--rw-r--r--   0 natsuki  (197609) None     (197121)      373 2023-01-13 15:20:05.000000 Eikthyr-0.6.4/Eikthyr.egg-info/SOURCES.txt
--rw-r--r--   0 natsuki  (197609) None     (197121)        1 2023-01-13 15:20:05.000000 Eikthyr-0.6.4/Eikthyr.egg-info/dependency_links.txt
--rw-r--r--   0 natsuki  (197609) None     (197121)       45 2023-01-13 15:20:05.000000 Eikthyr-0.6.4/Eikthyr.egg-info/requires.txt
--rw-r--r--   0 natsuki  (197609) None     (197121)        8 2023-01-13 15:20:05.000000 Eikthyr-0.6.4/Eikthyr.egg-info/top_level.txt
--rw-r--r--   0 natsuki  (197609) None     (197121)    11357 2023-01-13 14:50:21.000000 Eikthyr-0.6.4/LICENSE
--rw-r--r--   0 natsuki  (197609) None     (197121)      730 2023-01-13 15:20:05.223962 Eikthyr-0.6.4/PKG-INFO
--rw-r--r--   0 natsuki  (197609) None     (197121)      101 2023-01-13 14:50:21.000000 Eikthyr-0.6.4/README.md
--rw-r--r--   0 natsuki  (197609) None     (197121)      774 2023-01-13 15:19:02.000000 Eikthyr-0.6.4/pyproject.toml
--rw-r--r--   0 natsuki  (197609) None     (197121)       38 2023-01-13 15:20:05.223962 Eikthyr-0.6.4/setup.cfg
--rw-r--r--   0 natsuki  (197609) None     (197121)       38 2023-01-13 14:50:21.000000 Eikthyr-0.6.4/setup.py
+drwxr-xr-x   0 natsuki  (197609) None     (197121)        0 2023-05-31 07:47:05.613320 Eikthyr-0.7.0/
+drwxr-xr-x   0 natsuki  (197609) None     (197121)        0 2023-05-31 07:47:05.570402 Eikthyr-0.7.0/Eikthyr/
+-rw-r--r--   0 natsuki  (197609) None     (197121)     1131 2023-05-31 07:20:13.000000 Eikthyr-0.7.0/Eikthyr/__init__.py
+-rw-r--r--   0 natsuki  (197609) None     (197121)     1746 2023-03-02 08:30:47.000000 Eikthyr-0.7.0/Eikthyr/cmd.py
+-rw-r--r--   0 natsuki  (197609) None     (197121)     1632 2023-03-02 08:30:47.000000 Eikthyr-0.7.0/Eikthyr/envcheck.py
+-rw-r--r--   0 natsuki  (197609) None     (197121)      983 2023-03-29 00:57:22.000000 Eikthyr-0.7.0/Eikthyr/logging.py
+-rw-r--r--   0 natsuki  (197609) None     (197121)     2945 2023-03-29 00:57:22.000000 Eikthyr-0.7.0/Eikthyr/param.py
+-rw-r--r--   0 natsuki  (197609) None     (197121)     1894 2023-03-29 00:57:22.000000 Eikthyr-0.7.0/Eikthyr/run.py
+-rw-r--r--   0 natsuki  (197609) None     (197121)     1053 2023-03-29 00:57:22.000000 Eikthyr-0.7.0/Eikthyr/specialtask.py
+-rwxr-xr-x   0 natsuki  (197609) None     (197121)     2239 2023-03-29 00:57:22.000000 Eikthyr-0.7.0/Eikthyr/target.py
+-rw-r--r--   0 natsuki  (197609) None     (197121)     4443 2023-05-31 07:46:02.000000 Eikthyr-0.7.0/Eikthyr/task.py
+drwxr-xr-x   0 natsuki  (197609) None     (197121)        0 2023-05-31 07:47:05.589268 Eikthyr-0.7.0/Eikthyr.egg-info/
+-rw-r--r--   0 natsuki  (197609) None     (197121)      730 2023-05-31 07:47:05.000000 Eikthyr-0.7.0/Eikthyr.egg-info/PKG-INFO
+-rw-r--r--   0 natsuki  (197609) None     (197121)      436 2023-05-31 07:47:05.000000 Eikthyr-0.7.0/Eikthyr.egg-info/SOURCES.txt
+-rw-r--r--   0 natsuki  (197609) None     (197121)        1 2023-05-31 07:47:05.000000 Eikthyr-0.7.0/Eikthyr.egg-info/dependency_links.txt
+-rw-r--r--   0 natsuki  (197609) None     (197121)       45 2023-05-31 07:47:05.000000 Eikthyr-0.7.0/Eikthyr.egg-info/requires.txt
+-rw-r--r--   0 natsuki  (197609) None     (197121)        8 2023-05-31 07:47:05.000000 Eikthyr-0.7.0/Eikthyr.egg-info/top_level.txt
+-rw-r--r--   0 natsuki  (197609) None     (197121)    11357 2022-12-30 05:43:34.000000 Eikthyr-0.7.0/LICENSE
+-rw-r--r--   0 natsuki  (197609) None     (197121)      730 2023-05-31 07:47:05.611733 Eikthyr-0.7.0/PKG-INFO
+-rw-r--r--   0 natsuki  (197609) None     (197121)      101 2022-12-30 05:43:34.000000 Eikthyr-0.7.0/README.md
+-rw-r--r--   0 natsuki  (197609) None     (197121)      774 2023-05-31 07:46:15.000000 Eikthyr-0.7.0/pyproject.toml
+-rw-r--r--   0 natsuki  (197609) None     (197121)       38 2023-05-31 07:47:05.614359 Eikthyr-0.7.0/setup.cfg
+-rw-r--r--   0 natsuki  (197609) None     (197121)       38 2023-03-02 08:30:35.000000 Eikthyr-0.7.0/setup.py
+drwxr-xr-x   0 natsuki  (197609) None     (197121)        0 2023-05-31 07:47:05.607274 Eikthyr-0.7.0/tests/
+-rw-r--r--   0 natsuki  (197609) None     (197121)     1606 2023-03-02 08:30:47.000000 Eikthyr-0.7.0/tests/test_cmd.py
+-rwxr-xr-x   0 natsuki  (197609) None     (197121)     1634 2023-03-29 00:57:22.000000 Eikthyr-0.7.0/tests/test_param.py
+-rwxr-xrwx   0 natsuki  (197609) None     (197121)     2513 2023-03-28 02:59:23.000000 Eikthyr-0.7.0/tests/test_target.py
+-rwxr-xr-x   0 natsuki  (197609) None     (197121)     3184 2023-03-29 00:57:22.000000 Eikthyr-0.7.0/tests/test_task.py
```

### Comparing `Eikthyr-0.6.4/Eikthyr/__init__.py` & `Eikthyr-0.7.0/Eikthyr/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # -*- coding: utf-8 -*-
 
+# Load dotenv before everything
 from dotenv import load_dotenv as _load_dotenv, find_dotenv as _find_dotenv
 _load_dotenv(_find_dotenv(usecwd=True), override=True)
 
 # Deal with luigi's annoying deprecation warning
 import warnings as _warnings
 with _warnings.catch_warnings():
     _warnings.simplefilter("ignore")
     import luigi as lg
 
-from . import data
-from .data import Target, WrapperTarget
-from .data import ConfigData
+from . import param
+from .param import PathParameter, WhateverParameter, TaskParameter, TaskListParameter
+from luigi import Parameter, BoolParameter, IntParameter, FloatParameter, ListParameter, DictParameter
+
+from . import target
+from .target import Target, BinaryTarget
 
 from . import cmd
 from .cmd import chdir, mkcd, withEnv, cmdfmt, getenv
 
 from . import task
-from .task import Task, STask, NITask
+from .task import BaseTask, Task
+from .specialtask import InputTask
 
 from . import envcheck
 from .envcheck import EnvCheck
 
-from . import param
-from .param import WhateverParameter, TaskParameter, TaskListParameter, TargetParameter, PathParameter
-from luigi import Parameter, BoolParameter, IntParameter, FloatParameter, ListParameter, DictParameter
-
-from . import specialtask
-from .specialtask import InputTask, TargetWrapperTask, StampTask
-
 from . import logging
 from .logging import logger
 
 from . import run
 from .run import run
 
 from luigi import Config
```

### Comparing `Eikthyr-0.6.4/Eikthyr/cmd.py` & `Eikthyr-0.7.0/Eikthyr/cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2021-2022, Hojin Koh
+# Copyright 2021-2023, Hojin Koh
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `Eikthyr-0.6.4/Eikthyr/envcheck.py` & `Eikthyr-0.7.0/Eikthyr/envcheck.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2021-2022, Hojin Koh
+# Copyright 2021-2023, Hojin Koh
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `Eikthyr-0.6.4/Eikthyr/logging.py` & `Eikthyr-0.7.0/Eikthyr/logging.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2021-2022, Hojin Koh
+# Copyright 2021-2023, Hojin Koh
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,7 +16,12 @@
 from logzero import setup_logger
 logger = setup_logger('Eikthyr')
 
 # Disable annoying config warnings from luigi
 import warnings
 from luigi.parameter import UnconsumedParameterWarning
 warnings.simplefilter("ignore", UnconsumedParameterWarning)
+
+# Deal with luigi's annoying deprecation warning
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    import luigi
```

### Comparing `Eikthyr-0.6.4/Eikthyr/run.py` & `Eikthyr-0.7.0/Eikthyr/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2021-2022, Hojin Koh
+# Copyright 2021-2023, Hojin Koh
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,35 +16,31 @@
 import time
 from datetime import timedelta
 
 import luigi as lg
 from luigi.interface import _WorkerSchedulerFactory
 from luigi import worker
 
-from .cache import startCache
 from .logging import logger
 
 class _EikthyrFactory(_WorkerSchedulerFactory):
     def create_worker(self, scheduler, worker_processes, assistant=False):
         # Based on the suggestions in https://github.com/spotify/luigi/issues/2992
         return worker.Worker(scheduler=scheduler, worker_processes=worker_processes, assistant=assistant,
                 check_complete_on_run=True,
                 check_unfulfilled_deps=False,
                 keep_alive=True,
                 max_keep_alive_idle_duration=timedelta(seconds=1)
                 )
 
 def run(tasks, print_summary=True, workers=1):
-    if workers > 1:
-        startCache()
     if isinstance(tasks, lg.Task):
         tasks = (tasks,)
     t0 = time.time()
     rtn = lg.build(tasks, local_scheduler=True, log_level='WARNING', detailed_summary=True,
             workers=workers, worker_scheduler_factory=_EikthyrFactory())
     if print_summary:
         logger.info("Total Time Spent: {:.3f}s".format(time.time() - t0))
         logger.debug(rtn.summary_text)
     if rtn.status != lg.LuigiStatusCode.SUCCESS and rtn.status != lg.LuigiStatusCode.SUCCESS_WITH_RETRY:
         raise RuntimeError("Luigi task run failed")
     return rtn
-
```

### Comparing `Eikthyr-0.6.4/Eikthyr/specialtask.py` & `Eikthyr-0.7.0/Eikthyr/param.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,90 @@
 # -*- coding: utf-8 -*-
-# Copyright 2021-2022, Hojin Koh
+# Copyright 2021-2023, Hojin Koh
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-import os
-import re
+import pickle
+from base64 import b85encode, b85decode
 from pathlib import Path
 
 import luigi as lg
 from luigi.task import flatten
 
-from .data import Target
-from .logging import logger
-from .param import PathParameter, TargetParameter
-from .task import Task
-
-# Wrapper for an input file
-class InputTask(Task):
-    src = PathParameter()
-
-    def requires(self):
-        return []
-
-    def generates(self):
-        return Target(self, self.src)
-
-    def task(self):
-        if not Path(self.src).exists():
-            raise OSError(1, "Input file not found", self.src)
-        self.output().writeMeta()
-
-# Wrapper for a single target
-class TargetWrapperTask(Task):
-    src = TargetParameter()
-
-    def requires(self):
-        return self.src.task
-
-    def output(self):
-        return self.src
-
-    def run(self):
-        pass
-
-    def complete(self):
-        return self.src.task.complete()
-
-# Stamp: if code don't change, no need to re-run
-class StampTask(Task):
-    pathStamp = PathParameter(os.getenv('EIKTHYR_DIR_STAMP', '.stamp'), positional=False)
-
-    # This task doesn't care about the whether the upstream sources changed
-    checkInputHash = False
-
-    def getStampFileName(self):
-        return re.sub('pathStamp=[^ ]+, ', ' ', repr(self))
-
-    def generates(self):
-        # Let's turn ourself into a filename
-        return Target(self, Path(self.pathStamp).resolve() / self.getStamp())
-
-    def run(self):
-        rtn = yield from super().run()
-        with self.output().fpWrite() as fpw:
-            if self.checkInputHash:
-                fpw.write(''.join(self.getSrcHash()))
-            fpw.write(self.getCodeHash())
-            fpw.write(self.getSignature())
-        return rtn
+class PathParameter(lg.PathParameter):
+    """An extended type of PathParameter from the luigi one.
+
+    This class has an additional serializeShort for displaying the task.
+    If the specified path is inside the current directory, this class displays it as a relative path.
+    """
+
+    def serializeShort(self, x):
+        pathForShow = Path(x)
+        if pathForShow.is_absolute():
+            if pathForShow.is_relative_to(Path.cwd()):
+                pathForShow = pathForShow.relative_to(Path.cwd())
+        return str(pathForShow)
+
+# TODO: Test
+class WhateverParameter(lg.Parameter):
+    """A special type of parameter to contain anything.
+
+    When serialize/deserialize, this class pickle all its contents.
+    """
+
+    def _warn_on_wrong_param_type(self, param_name, param_value):
+        return
+
+    def serialize(self, x):
+        return str(b85encode(pickle.dumps(x)), encoding='ASCII')
+
+    def parse(self, x):
+        return pickle.loads(b85decode(bytes(x, encoding='ASCII')))
+
+    def serializeShort(self, x):
+        return self.serialize(x)
+
+# TODO: Test
+class TaskParameter(WhateverParameter):
+    """A task, presumed to be pulled in as a dependency."""
+
+    def _warn_on_wrong_param_type(self, param_name, param_value):
+        pass # TODO: lg.Task?
+
+    def serializeShort(self, x):
+        aRepr = []
+        for out in flatten(x.output()):
+            if hasattr(out, 'pathRel'):
+                aRepr.append(out.pathRel)
+            elif hasattr(out, 'path'):
+                aRepr.append(out.path)
+            else:
+                aRepr.append(repr(out))
+        return ';'.join(sorted(aRepr))
+
+# TODO: Test
+class TaskListParameter(WhateverParameter):
+    """A list of tasks, presumed to be pulled in as dependencies."""
+
+    def _warn_on_wrong_param_type(self, param_name, param_value):
+        pass # TODO: lg.Task?
+
+    def serializeShort(self, xs):
+        aRepr = []
+        for out in flatten((x.output() for x in xs)):
+            if hasattr(out, 'pathRel'):
+                aRepr.append(out.pathRel)
+            elif hasattr(out, 'path'):
+                aRepr.append(out.path)
+            else:
+                aRepr.append(repr(out))
+        return ';'.join(sorted(aRepr))
```

### Comparing `Eikthyr-0.6.4/Eikthyr.egg-info/PKG-INFO` & `Eikthyr-0.7.0/Eikthyr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eikthyr
-Version: 0.6.4
+Version: 0.7.0
 Summary: An wrapper to provide more utilities and completion checks to the luigi workflow library.
 Author-email: Hojin Koh <hojin-koh@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/hojin-koh/Eikthyr
 Project-URL: Bug Tracker, https://github.com/hojin-koh/Eikthyr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `Eikthyr-0.6.4/LICENSE` & `Eikthyr-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Eikthyr-0.6.4/PKG-INFO` & `Eikthyr-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eikthyr
-Version: 0.6.4
+Version: 0.7.0
 Summary: An wrapper to provide more utilities and completion checks to the luigi workflow library.
 Author-email: Hojin Koh <hojin-koh@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/hojin-koh/Eikthyr
 Project-URL: Bug Tracker, https://github.com/hojin-koh/Eikthyr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `Eikthyr-0.6.4/pyproject.toml` & `Eikthyr-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Eikthyr"
-version = "0.6.4"
+version = "0.7.0"
 authors = [
     { name="Hojin Koh", email="hojin-koh@users.noreply.github.com" },
 ]
 description = "An wrapper to provide more utilities and completion checks to the luigi workflow library."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["luigi", "plumbum", "colorama", "logzero", "python-dotenv"]
```

