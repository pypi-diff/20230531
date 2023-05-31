# Comparing `tmp/coniql-0.2.tar.gz` & `tmp/coniql-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coniql-0.2.tar", last modified: Fri Apr 22 10:28:41 2022, max compression
+gzip compressed data, was "coniql-0.3.tar", last modified: Wed May 31 09:36:56 2023, max compression
```

## Comparing `coniql-0.2.tar` & `coniql-0.3.tar`

### file list

```diff
@@ -1,29 +1,89 @@
-drwxrwxr-x   0 runner    (1001) docker     (121)        0 2022-04-22 10:28:41.521924 coniql-0.2/
--rw-rw-r--   0 runner    (1001) docker     (121)    11357 2022-04-22 10:28:28.000000 coniql-0.2/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (121)     2611 2022-04-22 10:28:41.521924 coniql-0.2/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (121)     1693 2022-04-22 10:28:28.000000 coniql-0.2/README.rst
--rw-rw-r--   0 runner    (1001) docker     (121)      320 2022-04-22 10:28:28.000000 coniql-0.2/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (121)     1729 2022-04-22 10:28:41.525924 coniql-0.2/setup.cfg
--rw-rw-r--   0 runner    (1001) docker     (121)      416 2022-04-22 10:28:28.000000 coniql-0.2/setup.py
-drwxrwxr-x   0 runner    (1001) docker     (121)        0 2022-04-22 10:28:41.521924 coniql-0.2/src/
-drwxrwxr-x   0 runner    (1001) docker     (121)        0 2022-04-22 10:28:41.521924 coniql-0.2/src/coniql/
--rw-rw-r--   0 runner    (1001) docker     (121)       65 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (121)       67 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (121)     3873 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/_version_git.py
--rw-rw-r--   0 runner    (1001) docker     (121)     2597 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/app.py
--rw-rw-r--   0 runner    (1001) docker     (121)     8239 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/caplugin.py
--rw-rw-r--   0 runner    (1001) docker     (121)      756 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/coniql_schema.py
--rw-rw-r--   0 runner    (1001) docker     (121)     3420 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/device_config.py
--rw-rw-r--   0 runner    (1001) docker     (121)     3708 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/plugin.py
--rw-rw-r--   0 runner    (1001) docker     (121)     8074 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/pvaplugin.py
--rw-rw-r--   0 runner    (1001) docker     (121)     8556 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/resolvers.py
--rw-rw-r--   0 runner    (1001) docker     (121)     9060 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/schema.gql
--rw-rw-r--   0 runner    (1001) docker     (121)    11457 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/simplugin.py
--rw-rw-r--   0 runner    (1001) docker     (121)     5928 2022-04-22 10:28:28.000000 coniql-0.2/src/coniql/types.py
-drwxrwxr-x   0 runner    (1001) docker     (121)        0 2022-04-22 10:28:41.521924 coniql-0.2/src/coniql.egg-info/
--rw-rw-r--   0 runner    (1001) docker     (121)     2611 2022-04-22 10:28:41.000000 coniql-0.2/src/coniql.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (121)      563 2022-04-22 10:28:41.000000 coniql-0.2/src/coniql.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1001) docker     (121)        1 2022-04-22 10:28:41.000000 coniql-0.2/src/coniql.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1001) docker     (121)       44 2022-04-22 10:28:41.000000 coniql-0.2/src/coniql.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1001) docker     (121)      205 2022-04-22 10:28:41.000000 coniql-0.2/src/coniql.egg-info/requires.txt
--rw-rw-r--   0 runner    (1001) docker     (121)        7 2022-04-22 10:28:41.000000 coniql-0.2/src/coniql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.137326 coniql-0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.133326 coniql-0.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-31 09:36:47.000000 coniql-0.3/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.133326 coniql-0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-31 09:36:47.000000 coniql-0.3/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.129326 coniql-0.3/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.133326 coniql-0.3/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-31 09:36:47.000000 coniql-0.3/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-31 09:36:47.000000 coniql-0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.133326 coniql-0.3/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 09:36:47.000000 coniql-0.3/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-05-31 09:36:47.000000 coniql-0.3/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.133326 coniql-0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-05-31 09:36:47.000000 coniql-0.3/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-31 09:36:47.000000 coniql-0.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-31 09:36:47.000000 coniql-0.3/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-31 09:36:47.000000 coniql-0.3/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-31 09:36:47.000000 coniql-0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 09:36:47.000000 coniql-0.3/.gitremotes
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-31 09:36:47.000000 coniql-0.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.133326 coniql-0.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 09:36:47.000000 coniql-0.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-31 09:36:47.000000 coniql-0.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-31 09:36:47.000000 coniql-0.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-31 09:36:47.000000 coniql-0.3/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-31 09:36:47.000000 coniql-0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 09:36:47.000000 coniql-0.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 09:36:47.000000 coniql-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-05-31 09:36:56.137326 coniql-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-31 09:36:47.000000 coniql-0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.133326 coniql-0.3/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-31 09:36:47.000000 coniql-0.3/benchmark/asyncClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 09:36:47.000000 coniql-0.3/benchmark/jsThroughputTest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-31 09:36:47.000000 coniql-0.3/benchmark/measureSineWave.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.133326 coniql-0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.133326 coniql-0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-31 09:36:47.000000 coniql-0.3/docs/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-31 09:36:47.000000 coniql-0.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.133326 coniql-0.3/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-31 09:36:47.000000 coniql-0.3/docs/explanations/why-graphql.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-31 09:36:47.000000 coniql-0.3/docs/explanations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.133326 coniql-0.3/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-31 09:36:47.000000 coniql-0.3/docs/how-to/run-a-server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-31 09:36:47.000000 coniql-0.3/docs/how-to.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.137326 coniql-0.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    41828 2023-05-31 09:36:47.000000 coniql-0.3/docs/images/concrete-device-layer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-31 09:36:47.000000 coniql-0.3/docs/images/coniql-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-05-31 09:36:47.000000 coniql-0.3/docs/images/coniql-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-31 09:36:47.000000 coniql-0.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.137326 coniql-0.3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-31 09:36:47.000000 coniql-0.3/docs/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-31 09:36:47.000000 coniql-0.3/docs/reference/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 09:36:47.000000 coniql-0.3/docs/reference/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-31 09:36:47.000000 coniql-0.3/docs/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.137326 coniql-0.3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-31 09:36:47.000000 coniql-0.3/docs/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-31 09:36:47.000000 coniql-0.3/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   136066 2023-05-31 09:36:47.000000 coniql-0.3/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-31 09:36:47.000000 coniql-0.3/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-31 09:36:47.000000 coniql-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:36:56.137326 coniql-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.129326 coniql-0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.137326 coniql-0.3/src/coniql/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-31 09:36:47.000000 coniql-0.3/src/coniql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-31 09:36:47.000000 coniql-0.3/src/coniql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-31 09:36:56.000000 coniql-0.3/src/coniql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-31 09:36:47.000000 coniql-0.3/src/coniql/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12940 2023-05-31 09:36:47.000000 coniql-0.3/src/coniql/caplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-31 09:36:47.000000 coniql-0.3/src/coniql/coniql_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-31 09:36:47.000000 coniql-0.3/src/coniql/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-31 09:36:47.000000 coniql-0.3/src/coniql/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-05-31 09:36:47.000000 coniql-0.3/src/coniql/simplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-05-31 09:36:47.000000 coniql-0.3/src/coniql/strawberry_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-05-31 09:36:47.000000 coniql-0.3/src/coniql/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.137326 coniql-0.3/src/coniql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-05-31 09:36:56.000000 coniql-0.3/src/coniql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-31 09:36:56.000000 coniql-0.3/src/coniql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:36:56.000000 coniql-0.3/src/coniql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 09:36:56.000000 coniql-0.3/src/coniql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-31 09:36:56.000000 coniql-0.3/src/coniql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 09:36:56.000000 coniql-0.3/src/coniql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:56.137326 coniql-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:36:47.000000 coniql-0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-05-31 09:36:47.000000 coniql-0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-31 09:36:47.000000 coniql-0.3/tests/soft_records.db
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-05-31 09:36:47.000000 coniql-0.3/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-31 09:36:47.000000 coniql-0.3/tests/test_caplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-31 09:36:47.000000 coniql-0.3/tests/test_coniql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-31 09:36:47.000000 coniql-0.3/tests/test_metrics.py
```

### Comparing `coniql-0.2/LICENSE` & `coniql-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coniql-0.2/src/coniql/simplugin.py` & `coniql-0.3/src/coniql/simplugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import asyncio
 import math
 import time
 from dataclasses import dataclass, replace
-from typing import AsyncGenerator, Dict, List, Optional, Set, Type
+from typing import Any, AsyncGenerator, Dict, List, Optional, Sequence, Set, Type
 
 import numpy as np
 
 from coniql.coniql_schema import DisplayForm, Widget
-from coniql.device_config import ChannelConfig
 from coniql.plugin import Plugin, PutValue
 from coniql.types import (
     Channel,
     ChannelDisplay,
     ChannelFormatter,
+    ChannelRole,
     ChannelStatus,
     ChannelTime,
     ChannelValue,
     Range,
 )
 
 # How long to keep Sim alive after the last listener has gone
@@ -81,15 +81,15 @@
 
 def make_display(
     min_value: float,
     max_value: float,
     warning_percent: float,
     alarm_percent: float,
     description: str,
-    role: str,
+    role: ChannelRole,
     widget: Widget,
 ) -> ChannelDisplay:
     assert max_value > min_value, "max_value %s is not > min_value %s" % (
         max_value,
         min_value,
     )
     display_range = max_value - min_value
@@ -145,26 +145,29 @@
         self.x = 0.0
         display = make_display(
             min_value,
             max_value,
             warning_percent,
             alarm_percent,
             description="A Sine value generator",
-            role="RO",
+            role=ChannelRole.RO,
             widget=Widget.TEXTUPDATE,
         )
         self.channel.display = display
         self.channel.value = ChannelValue(
             0,
-            ChannelFormatter.for_number(display.form, display.precision, display.units),
+            ChannelFormatter.for_number(display.precision, display.units),
         )
 
     def compute_changes(self):
         self.x += self.step
         value = self.min + (math.sin(self.x) + 1.0) / 2.0 * self.range
+        assert self.channel.display is not None
+        assert self.channel.display.alarmRange is not None
+        assert self.channel.display.warningRange is not None
         if not self.channel.display.alarmRange.contains(value):
             status = ChannelStatus.alarm("Outside alarm range")
         elif not self.channel.display.warningRange.contains(value):
             status = ChannelStatus.warning("Outside warning range")
         else:
             status = ChannelStatus.valid()
         return self.apply_changes(value, status=status)
@@ -201,23 +204,21 @@
         self.start = time.time()
         display = make_display(
             min_value,
             max_value,
             warning_percent=100.0,
             alarm_percent=100.0,
             description="A Sine waveform generator",
-            role="RO",
+            role=ChannelRole.RO,
             widget=Widget.PLOTY,
         )
         self.channel.display = display
         self.channel.value = ChannelValue(
             np.zeros(self.size, dtype=np.float64),
-            ChannelFormatter.for_ndarray(
-                display.form, display.precision, display.units
-            ),
+            ChannelFormatter.for_ndarray(display.precision, display.units),
         )
 
     def compute_changes(self) -> Channel:
         t = time.time() - self.start
         x0 = t / self.period
         x = 2 * math.pi * (x0 + np.arange(self.size) / self.wavelength)
         value = self.min + (np.sin(x) + 1.0) / 2.0 * self.range
@@ -257,39 +258,39 @@
 
         display = make_display(
             min_value,
             max_value,
             warning_percent=100.0,
             alarm_percent=100.0,
             description="A ramp waveform generator",
-            role="RO",
+            role=ChannelRole.RO,
             widget=Widget.PLOTY,
         )
         self.channel.display = display
         self.channel.value = ChannelValue(
             self.ramps[: self.size],
-            ChannelFormatter.for_ndarray(
-                display.form, display.precision, display.units
-            ),
+            ChannelFormatter.for_ndarray(display.precision, display.units),
         )
 
     def compute_changes(self) -> Channel:
         self.i += 1
         if self.i >= self.ramp_length:
             self.i = 0
         value = self.ramps[self.i : self.i + self.size]
         return self.apply_changes(value)
 
 
 class SimPlugin(Plugin):
-    def __init__(self):
+    def __init__(self) -> None:
         # {pv: Sim}
         self.sims: Dict[str, Sim] = {}
         # {pv: {queue_for_each_listener}}
         self.listeners: Dict[str, Set[asyncio.Queue[Channel]]] = {}
+        # Set of asyncio tasks running
+        self.task_references: Set[asyncio.Task[Any]] = set()
 
     async def _start_computing(self, pv: str):
         sim = self.sims[pv]
         next_compute = time.time()
         last_had_listeners = next_compute
         while next_compute - last_had_listeners < SIM_DESTROY_TIMEOUT:
             next_compute += sim.update_seconds
@@ -298,48 +299,47 @@
             for q in self.listeners[pv]:
                 last_had_listeners = next_compute
                 await q.put(changes)
         # no-one listening, remove sim
         del self.sims[pv]
         del self.listeners[pv]
 
-    async def get_channel(
-        self, pv: str, timeout: float, config: ChannelConfig
-    ) -> Channel:
+    async def get_channel(self, pv: str, timeout: float) -> Channel:
         if pv not in self.sims:
             if "(" in pv:
                 assert pv.endswith(")"), "Missing closing bracket in %r" % pv
                 func, param_str = pv[:-1].split("(", 1)
                 parameters = [float(param.strip()) for param in param_str.split(",")]
             else:
                 func = pv
                 parameters = []
             cls = CHANNEL_CLASSES[func]
             inst = cls(*parameters)
             display = inst.channel.display
             assert display
-            # Use config values in preference to defaults
-            display.description = config.description or display.description
-            display.form = config.display_form or display.form
-            display.widget = config.widget or display.widget
             self.sims[pv] = inst
             self.listeners[pv] = set()
-            asyncio.create_task(self._start_computing(pv))
+            task = asyncio.create_task(self._start_computing(pv))
+            self.task_references.add(task)
+
+            def _on_completion(t):
+                self.task_references.remove(t)
+
+            task.add_done_callback(_on_completion)
+
         return self.sims[pv].channel
 
-    async def subscribe_channel(
-        self, pv: str, config: ChannelConfig
-    ) -> AsyncGenerator[Channel, None]:
+    async def subscribe_channel(self, pv: str) -> AsyncGenerator[Channel, None]:
         q: asyncio.Queue[Channel] = asyncio.Queue()
         try:
-            channel = await self.get_channel(pv, 0, config)
+            channel = await self.get_channel(pv, 0)
             self.listeners[pv].add(q)
             yield channel
             while True:
                 yield await q.get()
         finally:
             self.listeners[pv].remove(q)
 
     async def put_channels(
-        self, pvs: List[str], values: List[PutValue], timeout: float
+        self, pvs: List[str], values: Sequence[PutValue], timeout: float
     ):
         raise RuntimeError(f"Cannot put {values!r} to {pvs}, as they aren't writeable")
```

