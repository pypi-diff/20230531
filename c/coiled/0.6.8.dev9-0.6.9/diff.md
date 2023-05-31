# Comparing `tmp/coiled-0.6.8.dev9.tar.gz` & `tmp/coiled-0.6.9.tar.gz`

## Comparing `coiled-0.6.8.dev9.tar` & `coiled-0.6.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/_version.py
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/analytics.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/coiled.yaml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/compatibility.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/context.py
--rw-r--r--   0        0        0   102090 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/exceptions.py
--rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/magic.py
--rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/software.py
--rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/types.py
--rw-r--r--   0        0        0    50564 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/websockets.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/_beta/__init__.py
--rw-r--r--   0        0        0    88536 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/_beta/cluster.py
--rw-r--r--   0        0        0    57546 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/_beta/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/_beta/cwi_log_link.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/_beta/states.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/_beta/widgets/__init__.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/_beta/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/_beta/widgets/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/config.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/core.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/login.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    12832 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/cli/setup/util.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/coiled/v2/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/README.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/pyproject.toml
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 coiled-0.6.8.dev9/PKG-INFO
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_version.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/analytics.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/coiled.yaml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/compatibility.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/context.py
+-rw-r--r--   0        0        0   102090 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/exceptions.py
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/magic.py
+-rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/software.py
+-rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/types.py
+-rw-r--r--   0        0        0    51919 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/websockets.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/__init__.py
+-rw-r--r--   0        0        0    88669 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/cluster.py
+-rw-r--r--   0        0        0    57690 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/cwi_log_link.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/states.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/widgets/__init__.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/widgets/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/config.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/core.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/login.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    12830 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/v2/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.9/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.9/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.9/README.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 coiled-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 coiled-0.6.9/PKG-INFO
```

### Comparing `coiled-0.6.8.dev9/coiled/__init__.py` & `coiled-0.6.9/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/analytics.py` & `coiled-0.6.9/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cluster.py` & `coiled-0.6.9/coiled/cluster.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,14 +26,14 @@
             with Client(self.cluster) as client:
                 client.run_on_scheduler(
                     lambda: dask.config.set({"distributed.adaptive.target-duration": target_duration})
                 )
 
     async def scale_up(self, n):
         logger.info(f"Adaptive scaling up to {n} workers.")
-        await self.cluster.scale_up(n)
+        await self.cluster.scale_up(n, reason=f"Adaptive scaling up to {n} workers.")
 
     async def scale_down(self, workers):
         if not workers:
             return
         logger.info(f"Adaptive is removing {len(workers)} workers: {workers}.")
         await self.cluster.scale_down(workers)
```

### Comparing `coiled-0.6.8.dev9/coiled/coiled.yaml` & `coiled-0.6.9/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/context.py` & `coiled-0.6.9/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/core.py` & `coiled-0.6.9/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/exceptions.py` & `coiled-0.6.9/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/magic.py` & `coiled-0.6.9/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/scan.py` & `coiled-0.6.9/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/software.py` & `coiled-0.6.9/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/types.py` & `coiled-0.6.9/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/utils.py` & `coiled-0.6.9/coiled/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1436,7 +1436,62 @@
     system = platform.system()
     if system == "Linux" and sys.prefix == "/usr":
         return True
     if system == "Darwin" and (sys.prefix.startswith("/Library") or sys.prefix.startswith("/System")):
         return True
     # Default to False
     return False
+
+
+NOT_INTERESTING_STACK_CODE = (
+    "distributed/utils.py",
+    "coiled/context.py",
+    "tornado/gen.py",
+    "backoff/_async.py",
+    "aiohttp/client.py",
+    "yarl/_url.py",
+)
+
+NOT_INTERESTING_FUNCTION = (
+    "_depaginate",
+    "_do_request",
+    "_sync",
+    "sync",
+)
+
+
+def is_interesting_stack_frame(filename, function):
+    if any(f in filename for f in NOT_INTERESTING_STACK_CODE):
+        return False
+    if "coiled" in filename and (any(f in function for f in NOT_INTERESTING_FUNCTION) or function.endswith("_page")):
+        return False
+    return True
+
+
+def truncate_traceback(exc_traceback):
+    curr = exc_traceback
+    frames = []
+    shown = set()
+
+    while curr:
+        filename = curr.tb_frame.f_code.co_filename
+        function = curr.tb_frame.f_code.co_name
+
+        if len(frames) == 0:
+            # always keep first frame
+            frames.append(curr)
+            shown.add((filename, function))
+        elif function.startswith("_") and (filename, function[1:]) in shown:
+            # ignore _foo if we've already included foo
+            pass
+        elif is_interesting_stack_frame(filename, function):
+            frames.append(curr)
+            shown.add((filename, function))
+
+        curr = curr.tb_next
+
+    curr = None
+    for tb in reversed(frames):
+        tb.tb_next = curr
+        curr = tb
+
+    return curr
```

### Comparing `coiled-0.6.8.dev9/coiled/websockets.py` & `coiled-0.6.9/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/_beta/__init__.py` & `coiled-0.6.9/coiled/_beta/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/_beta/cluster.py` & `coiled-0.6.9/coiled/_beta/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     cluster_firewall,
     get_details_url,
     get_grafana_url,
     get_instance_type_from_cpu_memory,
     is_system_python,
     parse_identifier,
     parse_wait_for_workers,
+    truncate_traceback,
     validate_vm_typing,
 )
 
 from ..core import Async, AWSSessionCredentials, Sync
 from .core import (
     CloudBeta,
     CloudBetaSyncAsync,
@@ -583,15 +584,15 @@
                 ):
                     logger.warning(f"Received KeyboardInterrupt, deleting cluster {self.cluster_id}")
                     self.cloud.delete_cluster(self.cluster_id, account=self.account)
                 raise
             except Exception as e:
                 error = e
                 self.close()
-                raise e
+                raise e.with_traceback(truncate_traceback(e.__traceback__))
             finally:
                 if error:
                     self.sync(
                         self.cloud.add_interaction,
                         "cluster-create",
                         success=False,
                         additional_data={
@@ -1414,29 +1415,30 @@
             return
         if status == "up":
             return await self.scale_up(**recommendations)
         if status == "down":
             return await self.scale_down(**recommendations)
 
     @track_context
-    async def scale_up(self, n: int) -> None:
+    async def scale_up(self, n: int, reason: Optional[str] = None) -> None:
         """
         Scales up *to* a target number of ``n`` workers
 
         It's documented that scale_up should scale up to a certain target, not scale up BY a certain amount:
 
         https://github.com/dask/distributed/blob/main/distributed/deploy/adaptive_core.py#L60
         """
         if not self.cluster_id:
             raise ValueError("No cluster available to scale! " "Check cluster was not closed by another process.")
         target = n - len(self.plan)
         response = await self.cloud._scale_up(
             account=self.account,
             cluster_id=self.cluster_id,
             n=target,
+            reason=reason,
         )
         if response:
             self._plan.update(set(response.get("workers", [])))
             self._requested.update(set(response.get("workers", [])))
 
     def _set_adaptive_options(self, **kwargs):
         # legacy version got dict with data about account limit and worker size
```

### Comparing `coiled-0.6.8.dev9/coiled/_beta/core.py` & `coiled-0.6.9/coiled/_beta/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1346,23 +1346,27 @@
             system=system,
             since_ms=since_ms,
             until_ms=until_ms,
             filter=filter,
         )
 
     @track_context
-    async def _scale_up(self, cluster_id: int, n: int, account: Optional[str] = None) -> Dict:
+    async def _scale_up(
+        self, cluster_id: int, n: int, account: Optional[str] = None, reason: Optional[str] = None
+    ) -> Dict:
         """
         Increases the number of workers by ``n``.
         """
         account = account or self.default_account
+        data = {"n_workers": n}
+        if reason:
+            # pyright is annoying
+            data["reason"] = reason  # type: ignore
         response = await self._do_request(
-            "POST",
-            f"{self.server}/api/v2/workers/account/{account}/cluster/{cluster_id}/",
-            json={"n_workers": n},
+            "POST", f"{self.server}/api/v2/workers/account/{account}/cluster/{cluster_id}/", json=data
         )
         if response.status >= 400:
             await handle_api_exception(response)
 
         workers_info = await response.json()
 
         return {"workers": {w["name"] for w in workers_info}}
```

### Comparing `coiled-0.6.8.dev9/coiled/_beta/cwi_log_link.py` & `coiled-0.6.9/coiled/_beta/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/_beta/states.py` & `coiled-0.6.9/coiled/_beta/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/_beta/widgets/__init__.py` & `coiled-0.6.9/coiled/_beta/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/_beta/widgets/rich.py` & `coiled-0.6.9/coiled/_beta/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/_beta/widgets/util.py` & `coiled-0.6.9/coiled/_beta/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/config.py` & `coiled-0.6.9/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/core.py` & `coiled-0.6.9/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/curl.py` & `coiled-0.6.9/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/env.py` & `coiled-0.6.9/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/login.py` & `coiled-0.6.9/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/package_sync.py` & `coiled-0.6.9/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/utils.py` & `coiled-0.6.9/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/cluster/__init__.py` & `coiled-0.6.9/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/cluster/better_logs.py` & `coiled-0.6.9/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/cluster/logs.py` & `coiled-0.6.9/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/cluster/ssh.py` & `coiled-0.6.9/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/cluster/utils.py` & `coiled-0.6.9/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/notebook/__init__.py` & `coiled-0.6.9/coiled/cli/notebook/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 
     This creates an easy "make my laptop bigger" command, since you'll have
     the same files and environment, just on a bigger machine in the cloud.
     """
     pass
 
 
-notebook.add_command(start_notebook, "up")
-notebook.add_command(stop_notebook, "down")
+notebook.add_command(start_notebook, "start")
+notebook.add_command(stop_notebook, "stop")
 notebook.add_command(monitor_sync, "monitor")
```

### Comparing `coiled-0.6.8.dev9/coiled/cli/notebook/notebook.py` & `coiled-0.6.9/coiled/cli/notebook/notebook.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
     gpu: bool,
     open: bool,
 ):
     """
     Launch or re-open a notebook session, with optional file syncing.
 
     If a notebook session with the same ``name`` already exists, it's not re-created.
-    If file sync was initially not enabled, running ``coiled notebook-beta up --sync``
+    If file sync was initially not enabled, running ``coiled notebook start --sync``
     will begin file sync without re-launching the notebook.
     """
 
     print(
         "[red]Warning:[/red] [bold]coiled notebook[/bold] "
         "is an experimental feature and is subject to breaking changes."
     )
@@ -285,15 +285,15 @@
                     ],
                     check=True,
                 )
 
     print(f"[bold]Jupyter available at {url}[/]")
     print()
 
-    stop_command = f"coiled notebook down --name {name}"
+    stop_command = f"coiled notebook stop --name {name}"
     if account:
         stop_command = f"{stop_command} --account {account}"
 
     print(f"To stop this notebook server: [green]{stop_command}[/]")
     if open:
         webbrowser.open(url, new=2)
```

### Comparing `coiled-0.6.8.dev9/coiled/cli/setup/__init__.py` & `coiled-0.6.9/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/setup/amp.py` & `coiled-0.6.9/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/setup/aws.py` & `coiled-0.6.9/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/setup/entry.py` & `coiled-0.6.9/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/setup/gcp.py` & `coiled-0.6.9/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/cli/setup/prometheus.py` & `coiled-0.6.9/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/coiled/v2/__init__.py` & `coiled-0.6.9/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/LICENSE` & `coiled-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/README.md` & `coiled-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/pyproject.toml` & `coiled-0.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.8.dev9/PKG-INFO` & `coiled-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.6.8.dev9
+Version: 0.6.9
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.6.8.dev9 Project-URL: Homepage,
-https://coiled.io Maintainer-email: Coiled
+Metadata-Version: 2.1 Name: coiled Version: 0.6.9 Project-URL: Homepage, https:
+//coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.7 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: pip Requires-Dist: pip>=19.3
 Requires-Dist: prometheus-client Requires-Dist: rich>=11.2.0 Requires-Dist:
 setuptools>=49.3.0 Requires-Dist: typing-extensions Requires-Dist: wheel
```

