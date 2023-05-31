# Comparing `tmp/thoughtful-2.0.0rc1.tar.gz` & `tmp/thoughtful-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtful-2.0.0rc1.tar", max compression
+gzip compressed data, was "thoughtful-2.0.0rc2.tar", max compression
```

## Comparing `thoughtful-2.0.0rc1.tar` & `thoughtful-2.0.0rc2.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0    11358 2022-12-14 17:25:44.942523 thoughtful-2.0.0rc1/LICENSE
--rw-r--r--   0        0        0     2992 2023-03-22 17:30:28.308693 thoughtful-2.0.0rc1/README.md
--rw-r--r--   0        0        0     1964 2023-05-30 13:53:35.915637 thoughtful-2.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0      222 2023-03-07 23:35:15.321689 thoughtful-2.0.0rc1/thoughtful/__init__.py
--rw-r--r--   0        0        0       57 2023-05-30 13:53:49.372018 thoughtful-2.0.0rc1/thoughtful/__version__.py
--rw-r--r--   0        0        0     1070 2023-05-25 17:53:34.765146 thoughtful-2.0.0rc1/thoughtful/environment_variables.py
--rw-r--r--   0        0        0      143 2022-12-14 17:25:44.949518 thoughtful-2.0.0rc1/thoughtful/supervisor/__init__.py
--rw-r--r--   0        0        0     4464 2023-05-26 20:50:27.370219 thoughtful-2.0.0rc1/thoughtful/supervisor/default_instances.py
--rw-r--r--   0        0        0     8598 2023-05-24 14:25:56.931578 thoughtful-2.0.0rc1/thoughtful/supervisor/main_context.py
--rw-r--r--   0        0        0    10567 2022-12-14 17:25:44.949966 thoughtful-2.0.0rc1/thoughtful/supervisor/manifest.py
--rw-r--r--   0        0        0        0 2022-12-14 17:25:44.949991 thoughtful-2.0.0rc1/thoughtful/supervisor/py.typed
--rw-r--r--   0        0        0        0 2022-12-14 17:25:44.950159 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/__init__.py
--rw-r--r--   0        0        0     2872 2023-05-26 19:04:25.164500 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/record.py
--rw-r--r--   0        0        0     1189 2023-05-26 19:04:25.164751 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/record_report.py
--rw-r--r--   0        0        0     2066 2023-05-26 19:04:25.164927 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/report.py
--rw-r--r--   0        0        0    10118 2023-05-26 19:04:25.165217 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/report_builder.py
--rw-r--r--   0        0        0      660 2023-05-26 19:04:25.165378 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/status.py
--rw-r--r--   0        0        0      876 2023-05-26 19:04:25.165550 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/step_report.py
--rw-r--r--   0        0        0     1541 2022-12-14 17:25:44.951007 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/timed_report.py
--rw-r--r--   0        0        0     1754 2023-05-26 19:04:25.165733 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/timer.py
--rw-r--r--   0        0        0     7627 2023-05-26 19:04:25.165919 thoughtful-2.0.0rc1/thoughtful/supervisor/step_context.py
--rw-r--r--   0        0        0     7462 2023-05-25 17:53:34.765671 thoughtful-2.0.0rc1/thoughtful/supervisor/step_decorator_factory.py
--rw-r--r--   0        0        0        0 2023-01-30 21:43:52.785761 thoughtful-2.0.0rc1/thoughtful/supervisor/streaming/__init__.py
--rw-r--r--   0        0        0      736 2023-04-06 19:41:20.157278 thoughtful-2.0.0rc1/thoughtful/supervisor/streaming/action.py
--rw-r--r--   0        0        0     5645 2023-05-30 13:47:08.800861 thoughtful-2.0.0rc1/thoughtful/supervisor/streaming/callback.py
--rw-r--r--   0        0        0     3184 2023-05-24 14:48:54.311303 thoughtful-2.0.0rc1/thoughtful/supervisor/streaming/payloads.py
--rw-r--r--   0        0        0     4257 1970-01-01 00:00:00.000000 thoughtful-2.0.0rc1/setup.py
--rw-r--r--   0        0        0     4592 1970-01-01 00:00:00.000000 thoughtful-2.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-12-14 17:25:44.942523 thoughtful-2.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     2992 2023-03-22 17:30:28.308693 thoughtful-2.0.0rc2/README.md
+-rw-r--r--   0        0        0     1949 2023-05-31 17:45:48.486059 thoughtful-2.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-03-07 23:35:15.321689 thoughtful-2.0.0rc2/thoughtful/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-31 17:45:58.271778 thoughtful-2.0.0rc2/thoughtful/__version__.py
+-rw-r--r--   0        0        0     1070 2023-05-31 17:32:30.137953 thoughtful-2.0.0rc2/thoughtful/environment_variables.py
+-rw-r--r--   0        0        0      143 2022-12-14 17:25:44.949518 thoughtful-2.0.0rc2/thoughtful/supervisor/__init__.py
+-rw-r--r--   0        0        0     4466 2023-05-31 17:33:24.495974 thoughtful-2.0.0rc2/thoughtful/supervisor/default_instances.py
+-rw-r--r--   0        0        0     8580 2023-05-31 17:32:30.138562 thoughtful-2.0.0rc2/thoughtful/supervisor/main_context.py
+-rw-r--r--   0        0        0    10567 2022-12-14 17:25:44.949966 thoughtful-2.0.0rc2/thoughtful/supervisor/manifest.py
+-rw-r--r--   0        0        0        0 2022-12-14 17:25:44.949991 thoughtful-2.0.0rc2/thoughtful/supervisor/py.typed
+-rw-r--r--   0        0        0        0 2022-12-14 17:25:44.950159 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/__init__.py
+-rw-r--r--   0        0        0     2872 2023-05-31 17:32:30.139057 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/record.py
+-rw-r--r--   0        0        0     1189 2023-05-31 17:32:30.139326 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/record_report.py
+-rw-r--r--   0        0        0     2066 2023-05-31 17:32:30.139588 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/report.py
+-rw-r--r--   0        0        0    10118 2023-05-31 17:32:30.139842 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/report_builder.py
+-rw-r--r--   0        0        0      660 2023-05-31 17:32:30.140233 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/status.py
+-rw-r--r--   0        0        0      876 2023-05-31 17:32:30.140535 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/step_report.py
+-rw-r--r--   0        0        0     1541 2022-12-14 17:25:44.951007 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/timed_report.py
+-rw-r--r--   0        0        0     1754 2023-05-31 17:32:30.140774 thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/timer.py
+-rw-r--r--   0        0        0     7609 2023-05-31 17:33:24.496190 thoughtful-2.0.0rc2/thoughtful/supervisor/step_context.py
+-rw-r--r--   0        0        0     7435 2023-05-31 17:33:24.496425 thoughtful-2.0.0rc2/thoughtful/supervisor/step_decorator_factory.py
+-rw-r--r--   0        0        0        0 2023-01-30 21:43:52.785761 thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-06 19:41:20.157278 thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/action.py
+-rw-r--r--   0        0        0     1347 2023-05-31 17:32:30.141532 thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/jwt_auth.py
+-rw-r--r--   0        0        0     3935 2023-05-31 17:32:30.141687 thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/notifier.py
+-rw-r--r--   0        0        0     3184 2023-05-24 14:48:54.311303 thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/payloads.py
+-rw-r--r--   0        0        0     1352 2023-05-31 17:32:30.141964 thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/token.py
+-rw-r--r--   0        0        0     4257 1970-01-01 00:00:00.000000 thoughtful-2.0.0rc2/setup.py
+-rw-r--r--   0        0        0     4592 1970-01-01 00:00:00.000000 thoughtful-2.0.0rc2/PKG-INFO
```

### Comparing `thoughtful-2.0.0rc1/LICENSE` & `thoughtful-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/README.md` & `thoughtful-2.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/pyproject.toml` & `thoughtful-2.0.0rc2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thoughtful"
-version = "2.0.0rc1"
+version = "2.0.0rc2"
 description = "Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor"
 authors = ["Thoughtful Automation <engineering@thoughtfulautomation.com>"]
 license = "Apache-2.0"
 readme = 'README.md'
 homepage = "https://thoughtfulautomation.com"
 repository = "https://github.com/thoughtful-automation/thoughtful"
 documentation = "https://readthedocs.com/projects/thoughtful-supervisor/"
@@ -36,22 +36,21 @@
 moto = "^4.0.5"
 requests = "^2.28.1"
 pyjwt = "^2.7.0"
 
 [tool.poetry.dev-dependencies]
 mkdocs = "^1.2.3"
 datamodel-code-generator = "^0.11.14"
-mkdocstrings = "^0.16.2"
-pytest = "^7.2.0"
+mkdocstrings = "^0.21.2"
+pytest = "^7.2.1"
 pytest-cov = "^2.12.1"
 pytest-watch = "^4.2.0"
 pytest-sugar = "^0.9.4"
 pytest-timeout = "^2.0.2"
 syrupy = "^1.5.0"
-tox = "^3.2.3"
 yapf = "^0.31.0"
 pylint = "^2.11.1"
 pre-commit = "^2.21.0"
 devtools = "^0.8.0"
 isort = "^5.12.0"
 autoflake = "^1.7.8"
 # This specifically needs to be exactly 1.0.0
```

### Comparing `thoughtful-2.0.0rc1/thoughtful/environment_variables.py` & `thoughtful-2.0.0rc2/thoughtful/environment_variables.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/default_instances.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/default_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 
 from thoughtful.environment_variables import EnvironmentVariables
 from thoughtful.supervisor.main_context import MainContext
 from thoughtful.supervisor.manifest import Manifest
 from thoughtful.supervisor.reporting.report_builder import ReportBuilder
 from thoughtful.supervisor.step_context import StepContext
 from thoughtful.supervisor.step_decorator_factory import create_step_decorator
-from thoughtful.supervisor.streaming.callback import StreamingCallback
+from thoughtful.supervisor.streaming.notifier import Notifier
 
 logger = logging.getLogger(__name__)
 
 # Share a streaming callback variable, but we can't set it until a user
 # provides a JWT token.
-streamer = StreamingCallback(
+streamer = Notifier.from_encoded_tokens(
     run_id=EnvironmentVariables().run_id,
     callback_url=EnvironmentVariables().callback_url,
     # The JWT token is set by the user later. If steamer is set to None,
     # then the step decorators can't be updated to stream if streamer is
     # changed to a new instance.
     #
     # See CX-2368 for the proper fix by lifting the streamer out of the contexts
```

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/main_context.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/main_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from urllib.parse import urlparse
 
 import boto3
 
 from thoughtful.supervisor.manifest import Manifest
 from thoughtful.supervisor.reporting.report_builder import ReportBuilder
 from thoughtful.supervisor.reporting.status import Status
-from thoughtful.supervisor.streaming.callback import StreamingCallback
+from thoughtful.supervisor.streaming.notifier import Notifier
 
 logger = logging.getLogger(__name__)
 
 
 class MainContext:
     """
     Supervises an entire digital worker run and generates a work report
@@ -63,15 +63,15 @@
     def __init__(
         self,
         report_builder: ReportBuilder,
         manifest: Union[Manifest, str, pathlib.Path],
         output_dir: Union[str, pathlib.Path],
         upload_uri: Optional[str] = None,
         callback: Optional[Callable] = None,
-        streaming_callback: Optional[StreamingCallback] = None,
+        streaming_callback: Optional[Notifier] = None,
     ):
         """
         Args:
             report_builder (ReportBuilder): A ReportBuilder object that will
                 receive the step reports and provide the run report.
                 messages and logs throughout the process execution.
             manifest (str, Path): A pathlike object that points to the manifest
```

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/manifest.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/manifest.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/record.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/record.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/record_report.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/record_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/report.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/report_builder.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/report_builder.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/status.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/status.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/step_report.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/step_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/timed_report.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/timed_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/timer.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/reporting/timer.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/step_context.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/step_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,29 +40,29 @@
 from types import TracebackType
 from typing import Optional, Type, Union
 
 from thoughtful.supervisor.reporting.report_builder import ReportBuilder
 from thoughtful.supervisor.reporting.report_builder import StepReportBuilder
 from thoughtful.supervisor.reporting.status import Status
 from thoughtful.supervisor.reporting.timer import Timer
-from thoughtful.supervisor.streaming.callback import StreamingCallback
+from thoughtful.supervisor.streaming.notifier import Notifier
 
 
 class StepContext:
     """
     A context manager for a step that is running inside another step.
     This is an alternative to ``@step`` decorator when you don't want
     to write an entire function for a step.
     """
 
     def __init__(
         self,
         builder: ReportBuilder,
         step_id: Union[str, int],
-        streaming_callback: Optional[StreamingCallback] = None,
+        streaming_callback: Optional[Notifier] = None,
     ):
         """
         Args:
             builder: Where the step report will be written.
             *step_id: The step id of this step, ie `"1.1"`
             streaming_callback (StreamingCallback, optional): If set, streams
                 the status of work report steps to that callback handler.
```

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/step_decorator_factory.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/step_decorator_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,20 +63,20 @@
 import logging
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from thoughtful.supervisor.reporting.report_builder import ReportBuilder
 from thoughtful.supervisor.reporting.report_builder import StepReportBuilder
 from thoughtful.supervisor.reporting.status import Status
 from thoughtful.supervisor.reporting.timer import Timer
-from thoughtful.supervisor.streaming.callback import StreamingCallback
+from thoughtful.supervisor.streaming.notifier import Notifier
 
 
 def create_step_decorator(
     report_builder: ReportBuilder,
-    streaming_callback: Optional[StreamingCallback] = None,
+    streaming_callback: Optional[Notifier] = None,
 ) -> Callable:
     """
     A step decorator generator that as input receives a ``ReportBuilder``
     object and a ``Recorder`` object. The returned decorator will use these
     objects to record the execution of the decorated function.
 
     Note that the return type here is `Any`, because proper type hinting
@@ -136,15 +136,15 @@
     return returned_decorator
 
 
 def _run_wrapped_func(
     fn: Callable,
     step_id: str,
     report_builder: ReportBuilder,
-    streaming_callback: StreamingCallback,
+    streaming_callback: Notifier,
     *fn_args: Optional[Any],
     **fn_kwargs: Optional[Any],
 ) -> Any:
     """
     Runs `fn` with the given args `args` and `kwargs`, times how long it
     takes to run, and records the execution of this function under `step_id`
     in the work report.
```

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/streaming/action.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/action.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/thoughtful/supervisor/streaming/payloads.py` & `thoughtful-2.0.0rc2/thoughtful/supervisor/streaming/payloads.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc1/setup.py` & `thoughtful-2.0.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'pydantic>=1.8.2,<2.0.0',
  'pyjwt>=2.7.0,<3.0.0',
  'pyyaml>=5.4.1',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'thoughtful',
-    'version': '2.0.0rc1',
+    'version': '2.0.0rc2',
     'description': 'Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor',
     'long_description': '**thoughtful** is a collection of open-source libraries and tools for Robot Process\nAutomation (RPA) development. The goal of this project is to provide a set of\nfor supervising bot execution, and enabling these bots to do more.\n\n[![PyPi version](https://badgen.net/pypi/v/thoughtful/)](https://pypi.org/project/thoughtful/)\n![Main Branch Tests](https://github.com/Thoughtful-Automation/supervisor/actions/workflows/main-push.yml/badge.svg?branch=main)\n[![Supported Versions](https://img.shields.io/pypi/pyversions/thoughtful.svg)](https://pypi.org/project/thoughtful)\n[![Downloads](https://pepy.tech/badge/thoughtful/month)](https://pepy.tech/project/thoughtful)\n\n[//]: # ([![GitHub release]&#40;https://img.shields.io/github/release/Thoughtful-Automation/supervisor.svg&#41;]&#40;https://GitHub.com/Naereen/StrapDown.js/releases/&#41;)\n\n\nThis project is:\n* Open-source: [GitHub][url:gh]\n* Owned by [thoughtful][url:ta]\n* Licensed under the [Apache License 2.0][url:al]\n\nLinks:\n* [Homepage][url:gh]\n* [Documentation][url:readthedocs]\n* [PyPI][url:pypi]\n\n**thoughtful** is available on [PyPI][url:pypi] and can be installed using pip:\n\n```sh\npip install thoughtful\n```\n\n---\n\n**thoughtful** officially supports Python 3.7+.\n\n---\n\n# Libraries\n\nThis is a list of the available libraries in this project. API Reference\nand User Guide available on [docs][url:readthedocs].\n\n## Supervisor\n\nSupervisor is a Workflow Engine for Digital Workers that constructs\nand broadcasts a detailed and structured telemetric log, called the Run Report.\n\n```python\nfrom thoughtful.supervisor import step, step_scope, supervise, set_step_status\n\n\n# using the step decorator\n@step("2")\ndef step_2(name: str) -> bool:\n    print(f\'Hello {name}\')\n    return True  # some condition\n\ndef main() -> None:\n    # using the step_scope context manager\n    with step_scope(\'1\') as step_context:\n        try:\n            print("Getting credentials")\n            # ...\n        except Exception as e:\n            # set step status using method\n            step_context.set_status("warning")\n\n    if not step_2():\n        # set step status using function\n        set_step_status("2", "fail")\n\nif __name__ == \'__main__\':\n    with supervise():\n        main()\n```\n\n## Contributing\n\nContributions to **thoughtful** are welcome!\n\nTo get started, see the [contributing guide](CONTRIBUTING.md).\n\n---\n\n  Made with ❤️ by\n\n  [![Thoughtful](https://user-images.githubusercontent.com/1096881/141985289-317c2e72-3c2d-4e6b-800a-0def1a05f599.png)][url:ta]\n\n---\n\nThis project is open-source and licensed under the terms of the [Apache License 2.0][url:al].\n\n\n<!--  Link References -->\n\n[url:ta]: https://www.thoughtful.ai/\n[url:gh]: https://github.com/Thoughtful-Automation/supervisor\n[url:pypi]: https://pypi.org/project/thoughtful/\n[git:issues]: https://github.com/Thoughtful-Automation/supervisor/issues\n[url:readthedocs]: https://thoughtful-supervisor.readthedocs-hosted.com/en/latest/\n[url:al]: http://www.apache.org/licenses/LICENSE-2.0\n',
     'author': 'Thoughtful Automation',
     'author_email': 'engineering@thoughtfulautomation.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://thoughtfulautomation.com',
```

### Comparing `thoughtful-2.0.0rc1/PKG-INFO` & `thoughtful-2.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtful
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor
 Home-page: https://thoughtfulautomation.com
 License: Apache-2.0
 Keywords: rpa,robot-framework,robocorp,automation
 Author: Thoughtful Automation
 Author-email: engineering@thoughtfulautomation.com
 Requires-Python: >=3.8,<3.12
```

