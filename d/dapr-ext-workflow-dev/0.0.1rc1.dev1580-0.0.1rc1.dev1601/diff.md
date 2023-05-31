# Comparing `tmp/dapr-ext-workflow-dev-0.0.1rc1.dev1580.tar.gz` & `tmp/dapr-ext-workflow-dev-0.0.1rc1.dev1601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-ext-workflow-dev-0.0.1rc1.dev1580.tar", last modified: Wed May 24 16:45:13 2023, max compression
+gzip compressed data, was "dist/dapr-ext-workflow-dev-0.0.1rc1.dev1601.tar", last modified: Wed May 31 15:44:13 2023, max compression
```

## Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580.tar` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-24 16:44:46.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-24 16:45:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-24 16:44:46.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-24 16:44:46.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-24 16:44:46.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/dapr_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-24 16:44:46.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/dapr_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-24 16:44:46.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-24 16:44:46.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/workflow_activity_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-24 16:44:46.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-24 16:44:46.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/workflow_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-24 16:44:46.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/workflow_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr_ext_workflow_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-24 16:45:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr_ext_workflow_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-24 16:45:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr_ext_workflow_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:45:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr_ext_workflow_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 16:45:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr_ext_workflow_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 16:45:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr_ext_workflow_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-24 16:45:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-24 16:44:46.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1580/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-31 15:43:49.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-31 15:44:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-31 15:43:49.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-31 15:43:49.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-05-31 15:43:49.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/dapr_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-31 15:43:49.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/dapr_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-31 15:43:49.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-31 15:43:49.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-31 15:43:49.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/workflow_activity_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-31 15:43:49.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-31 15:43:49.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/workflow_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-31 15:43:49.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/workflow_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:44:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr_ext_workflow_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-31 15:44:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr_ext_workflow_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 15:44:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr_ext_workflow_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:44:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr_ext_workflow_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-31 15:44:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr_ext_workflow_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 15:44:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr_ext_workflow_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-31 15:44:13.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-31 15:43:49.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1601/setup.py
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/LICENSE` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/PKG-INFO` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow-dev
-Version: 0.0.1rc1.dev1580
+Version: 0.0.1rc1.dev1601
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/__init__.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # Import your main classes here
 from dapr.ext.workflow.workflow_runtime import WorkflowRuntime
 from dapr.ext.workflow.dapr_workflow_client import DaprWorkflowClient
-from dapr.ext.workflow.dapr_workflow_context import DaprWorkflowContext
+from dapr.ext.workflow.dapr_workflow_context import DaprWorkflowContext, when_all, when_any
 from dapr.ext.workflow.workflow_activity_context import WorkflowActivityContext
 
 __all__ = [
     'WorkflowRuntime',
     'DaprWorkflowClient',
     'DaprWorkflowContext',
     'WorkflowActivityContext',
+    'when_all',
+    'when_any'
 ]
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/dapr_workflow_client.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/dapr_workflow_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from __future__ import annotations
 from datetime import datetime
-from typing import Any, TypeVar, Union
-from dapr.conf import settings
+from typing import Any, Optional, TypeVar
 
 from durabletask import client
+
 from dapr.ext.workflow.workflow_state import WorkflowState
 from dapr.ext.workflow.workflow_context import Workflow
+from dapr.ext.workflow.util import getAddress
 
 T = TypeVar('T')
 TInput = TypeVar('TInput')
 TOutput = TypeVar('TOutput')
 
 
 class DaprWorkflowClient:
@@ -32,28 +33,23 @@
 
        This is an alternative to the general purpose Dapr client. It uses a gRPC connection to send
        commands directly to the workflow engine, bypassing the Dapr API layer.
 
        This client is intended to be used by workflow application, not by general purpose
        application.
     """
-    def __init__(self, host: Union[str, None] = None, port: Union[str, None] = None):
-        if host is None:
-            host = settings.DAPR_RUNTIME_HOST
-        if not host or len(host) == 0 or len(host.strip()) == 0:
-            host = "localhost"
-        port = port or settings.DAPR_GRPC_PORT
-        address = f"{host}:{port}"
+    def __init__(self, host: Optional[str] = None, port: Optional[str] = None):
+        address = getAddress(host, port)
         self.__obj = client.TaskHubGrpcClient(host_address=address)
 
     def schedule_new_workflow(self,
                               workflow: Workflow, *,
-                              input: Union[TInput, None] = None,
-                              instance_id: Union[str, None] = None,
-                              start_at: Union[datetime, None] = None) -> str:
+                              input: Optional[TInput] = None,
+                              instance_id: Optional[str] = None,
+                              start_at: Optional[datetime] = None) -> str:
         """Schedules a new workflow instance for execution.
 
         Args:
             workflow: The workflow to schedule.
             input: The optional input to pass to the scheduled workflow instance. This must be a
             serializable value.
             instance_id: The unique ID of the workflow instance to schedule. If not specified, a
@@ -66,15 +62,15 @@
             The ID of the scheduled workflow instance.
         """
         return self.__obj.schedule_new_orchestration(workflow.__name__,
                                                      input=input, instance_id=instance_id,
                                                      start_at=start_at)
 
     def get_workflow_state(self, instance_id: str, *,
-                           fetch_payloads: bool = True) -> Union[WorkflowState, None]:
+                           fetch_payloads: bool = True) -> Optional[WorkflowState]:
         """Fetches runtime state for the specified workflow instance.
 
         Args:
             instanceId: The unique ID of the workflow instance to fetch.
             fetch_payloads: If true, fetches the input, output payloads and custom status
             for the workflow instance. Defaults to false.
 
@@ -84,15 +80,15 @@
 
         """
         state = self.__obj.get_orchestration_state(instance_id, fetch_payloads=fetch_payloads)
         return WorkflowState(state) if state else None
 
     def wait_for_workflow_start(self, instance_id: str, *,
                                 fetch_payloads: bool = False,
-                                timeout_in_seconds: int = 60) -> Union[WorkflowState, None]:
+                                timeout_in_seconds: int = 60) -> Optional[WorkflowState]:
         """Waits for a workflow to start running and returns a WorkflowState object that contains
            metadata about the started workflow.
 
            A "started" workflow instance is any instance not in the WorkflowRuntimeStatus.Pending
            state. This method will return a completed task if the workflow has already started
            running or has already completed.
 
@@ -110,15 +106,15 @@
         state = self.__obj.wait_for_orchestration_start(instance_id,
                                                         fetch_payloads=fetch_payloads,
                                                         timeout=timeout_in_seconds)
         return WorkflowState(state) if state else None
 
     def wait_for_workflow_completion(self, instance_id: str, *,
                                      fetch_payloads: bool = True,
-                                     timeout_in_seconds: int = 60) -> Union[WorkflowState, None]:
+                                     timeout_in_seconds: int = 60) -> Optional[WorkflowState]:
         """Waits for a workflow to complete and returns a WorkflowState object that contains
            metadata about the started instance.
 
            A "completed" workflow instance is any instance in one of the terminal states. For
            example, the WorkflowRuntimeStatus.Completed, WorkflowRuntimeStatus.Failed or
            WorkflowRuntimeStatus.Terminated states.
 
@@ -142,15 +138,15 @@
         """
         state = self.__obj.wait_for_orchestration_completion(instance_id,
                                                              fetch_payloads=fetch_payloads,
                                                              timeout=timeout_in_seconds)
         return WorkflowState(state) if state else None
 
     def raise_workflow_event(self, instance_id: str, event_name: str, *,
-                             data: Union[Any, None] = None):
+                             data: Optional[Any] = None):
         """Sends an event notification message to a waiting workflow instance.
            In order to handle the event, the target workflow instance must be waiting for an
            event named value of "eventName" param using the wait_for_external_event API.
            If the target workflow instance is not yet waiting for an event named param "eventName"
            value, then the event will be saved in the workflow instance state and dispatched
            immediately when the workflow calls wait_for_external_event.
            This event saving occurs even if the workflow has canceled its wait operation before
@@ -167,15 +163,15 @@
             instanceId: The ID of the workflow instance that will handle the event.
             eventName: The name of the event. Event names are case-insensitive.
             data: The serializable data payload to include with the event.
         """
         return self.__obj.raise_orchestration_event(instance_id, event_name, data=data)
 
     def terminate_workflow(self, instance_id: str, *,
-                           output: Union[Any, None] = None):
+                           output: Optional[Any] = None):
         """Terminates a running workflow instance and updates its runtime status to
            WorkflowRuntimeStatus.Terminated This method internally enqueues a "terminate" message in
            the task hub. When the task hub worker processes this message, it will update the runtime
            status of the target instance to WorkflowRuntimeStatus.Terminated. You can use
            wait_for_workflow_completion to wait for the instance to reach the terminated state.
 
            Terminating a workflow instance has no effect on any in-flight activity function
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/dapr_workflow_context.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/dapr_workflow_context.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import Any, Callable, TypeVar, Union
-from durabletask import task
+from typing import Any, Callable, List, Optional, TypeVar
 from datetime import datetime
-from dapr.ext.workflow.workflow_context import WorkflowContext, Workflow
 
+from durabletask import task
+
+from dapr.ext.workflow.workflow_context import WorkflowContext, Workflow
 from dapr.ext.workflow.workflow_activity_context import WorkflowActivityContext
 
 T = TypeVar('T')
 TInput = TypeVar('TInput')
 TOutput = TypeVar('TOutput')
 
 
@@ -51,19 +52,30 @@
         return self.__obj.create_timer(fire_at)
 
     def call_activity(self, activity: Callable[[WorkflowActivityContext, TInput], TOutput], *,
                       input: TInput = None) -> task.Task[TOutput]:
         return self.__obj.call_activity(activity=activity.__name__, input=input)
 
     def call_child_workflow(self, workflow: Workflow, *,
-                            input: Union[TInput, None],
-                            instance_id: Union[str, None]) -> task.Task[TOutput]:
+                            input: Optional[TInput],
+                            instance_id: Optional[str]) -> task.Task[TOutput]:
         def wf(ctx: task.OrchestrationContext, inp: TInput):
             daprWfContext = DaprWorkflowContext(ctx)
             return workflow(daprWfContext, inp)
         return self.__obj.call_sub_orchestrator(wf, input=input, instance_id=instance_id)
 
     def wait_for_external_event(self, name: str) -> task.Task:
         return self.__obj.wait_for_external_event(name)
 
     def continue_as_new(self, new_input: Any, *, save_events: bool = False) -> None:
         self.__obj.continue_as_new(new_input, save_events=save_events)
+
+
+def when_all(tasks: List[task.Task[T]]) -> task.WhenAllTask[T]:
+    """Returns a task that completes when all of the provided tasks complete or when one of the
+    tasks fail."""
+    return task.when_all(tasks)
+
+
+def when_any(tasks: List[task.Task]) -> task.WhenAnyTask:
+    """Returns a task that completes when any of the provided tasks complete or fail."""
+    return task.when_any(tasks)
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/version.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/version.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/workflow_activity_context.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/workflow_activity_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/workflow_context.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/workflow_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from __future__ import annotations
-
 from abc import ABC, abstractmethod
 from datetime import datetime
-from typing import Any, Callable, Generator, TypeVar, Union
+from typing import Any, Callable, Generator, Optional, TypeVar, Union
+
 from durabletask import task
 
 from dapr.ext.workflow.workflow_activity_context import Activity
 
 T = TypeVar('T')
 TInput = TypeVar('TInput')
 TOutput = TypeVar('TOutput')
@@ -98,15 +98,15 @@
         Task
             A Durable Timer Task that schedules the timer to wake up the orchestrator
         """
         pass
 
     @abstractmethod
     def call_activity(self, activity: Activity[TInput, TOutput], *,
-                      input: Union[TInput, None] = None) -> task.Task[TOutput]:
+                      input: Optional[TInput] = None) -> task.Task[TOutput]:
         """Schedule an activity for execution.
 
         Parameters
         ----------
         activity: Activity[TInput, TOutput]
             A reference to the activity function to call.
         input: TInput | None
@@ -119,16 +119,16 @@
         Task
             A Durable Task that completes when the called activity function completes or fails.
         """
         pass
 
     @abstractmethod
     def call_child_workflow(self, orchestrator: Workflow[TInput, TOutput], *,
-                            input: Union[TInput, None] = None,
-                            instance_id: Union[str, None] = None) -> task.Task[TOutput]:
+                            input: Optional[TInput] = None,
+                            instance_id: Optional[str] = None) -> task.Task[TOutput]:
         """Schedule child-workflow function for execution.
 
         Parameters
         ----------
         orchestrator: Orchestrator[TInput, TOutput]
             A reference to the orchestrator function to call.
         input: TInput
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/workflow_runtime.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/workflow_runtime.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,31 +9,35 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from typing import TypeVar
+from typing import Optional, TypeVar
+
 from durabletask import worker, task
+
 from dapr.ext.workflow.workflow_context import Workflow
 from dapr.ext.workflow.dapr_workflow_context import DaprWorkflowContext
 from dapr.ext.workflow.workflow_activity_context import Activity, WorkflowActivityContext
+from dapr.ext.workflow.util import getAddress
 
 T = TypeVar('T')
 TInput = TypeVar('TInput')
 TOutput = TypeVar('TOutput')
 
 
 class WorkflowRuntime:
     """WorkflowRuntime is the entry point for registering workflows and activities.
     """
 
-    def __init__(self):
-        self.__worker = worker.TaskHubGrpcWorker()
+    def __init__(self, host: Optional[str] = None, port: Optional[str] = None):
+        address = getAddress(host, port)
+        self.__worker = worker.TaskHubGrpcWorker(host_address=address)
 
     def register_workflow(self, fn: Workflow[TInput, TInput]):
         def orchestrationWrapper(ctx: task.OrchestrationContext, inp: TInput):
             """Responsible to call Workflow function in orchestrationWrapper"""
             daprWfContext = DaprWorkflowContext(ctx)
             return fn(daprWfContext, inp)
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr/ext/workflow/workflow_state.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr/ext/workflow/workflow_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from durabletask import client
 from enum import Enum
 
+from durabletask import client
+
 
 class WorkflowStatus(Enum):
     UNKNOWN = 0
     RUNNING = 1
     COMPLETED = 2
     FAILED = 3
     TERMINATED = 4
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr_ext_workflow_dev.egg-info/PKG-INFO` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr_ext_workflow_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow-dev
-Version: 0.0.1rc1.dev1580
+Version: 0.0.1rc1.dev1601
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/dapr_ext_workflow_dev.egg-info/SOURCES.txt` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/dapr_ext_workflow_dev.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.rst
 setup.cfg
 setup.py
 dapr/ext/workflow/__init__.py
 dapr/ext/workflow/dapr_workflow_client.py
 dapr/ext/workflow/dapr_workflow_context.py
+dapr/ext/workflow/util.py
 dapr/ext/workflow/version.py
 dapr/ext/workflow/workflow_activity_context.py
 dapr/ext/workflow/workflow_context.py
 dapr/ext/workflow/workflow_runtime.py
 dapr/ext/workflow/workflow_state.py
 dapr_ext_workflow_dev.egg-info/PKG-INFO
 dapr_ext_workflow_dev.egg-info/SOURCES.txt
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/setup.cfg` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/setup.cfg`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1580/setup.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1601/setup.py`

 * *Files identical despite different names*

