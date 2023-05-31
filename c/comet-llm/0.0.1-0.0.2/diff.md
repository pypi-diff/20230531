# Comparing `tmp/comet_llm-0.0.1.tar.gz` & `tmp/comet_llm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comet_llm-0.0.1.tar", last modified: Thu May 18 09:23:50 2023, max compression
+gzip compressed data, was "comet_llm-0.0.2.tar", last modified: Wed May 31 13:58:31 2023, max compression
```

## Comparing `comet_llm-0.0.1.tar` & `comet_llm-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:23:50.727088 comet_llm-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-18 09:23:50.727088 comet_llm-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 09:23:34.000000 comet_llm-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 09:23:50.727088 comet_llm-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-18 09:23:34.000000 comet_llm-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:23:50.723087 comet_llm-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:23:50.723087 comet_llm-0.0.1/src/comet_llm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-18 09:23:34.000000 comet_llm-0.0.1/src/comet_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-18 09:23:34.000000 comet_llm-0.0.1/src/comet_llm/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-18 09:23:34.000000 comet_llm-0.0.1/src/comet_llm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-18 09:23:34.000000 comet_llm-0.0.1/src/comet_llm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-18 09:23:34.000000 comet_llm-0.0.1/src/comet_llm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:23:50.727088 comet_llm-0.0.1/src/comet_llm/experiment_api/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-18 09:23:34.000000 comet_llm-0.0.1/src/comet_llm/experiment_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-18 09:23:34.000000 comet_llm-0.0.1/src/comet_llm/experiment_api/comet_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-18 09:23:34.000000 comet_llm-0.0.1/src/comet_llm/experiment_api/experiment_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-18 09:23:34.000000 comet_llm-0.0.1/src/comet_llm/experiment_api/request_exception_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 09:23:34.000000 comet_llm-0.0.1/src/comet_llm/experiment_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-18 09:23:34.000000 comet_llm-0.0.1/src/comet_llm/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:23:50.723087 comet_llm-0.0.1/src/comet_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-18 09:23:50.000000 comet_llm-0.0.1/src/comet_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-18 09:23:50.000000 comet_llm-0.0.1/src/comet_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:23:50.000000 comet_llm-0.0.1/src/comet_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:23:50.000000 comet_llm-0.0.1/src/comet_llm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-18 09:23:50.000000 comet_llm-0.0.1/src/comet_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 09:23:50.000000 comet_llm-0.0.1/src/comet_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:31.439604 comet_llm-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-31 13:58:31.439604 comet_llm-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 13:58:21.000000 comet_llm-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:58:31.439604 comet_llm-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-31 13:58:21.000000 comet_llm-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:31.435604 comet_llm-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:31.439604 comet_llm-0.0.2/src/comet_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:31.439604 comet_llm-0.0.2/src/comet_llm/experiment_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/experiment_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/experiment_api/comet_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/experiment_api/experiment_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/experiment_api/request_exception_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/experiment_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:31.439604 comet_llm-0.0.2/src/comet_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-31 13:58:31.000000 comet_llm-0.0.2/src/comet_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 13:58:31.000000 comet_llm-0.0.2/src/comet_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:58:31.000000 comet_llm-0.0.2/src/comet_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:58:31.000000 comet_llm-0.0.2/src/comet_llm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 13:58:31.000000 comet_llm-0.0.2/src/comet_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 13:58:31.000000 comet_llm-0.0.2/src/comet_llm.egg-info/top_level.txt
```

### Comparing `comet_llm-0.0.1/PKG-INFO` & `comet_llm-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_llm
-Version: 0.0.1
+Version: 0.0.2
 Summary: Comet logger for LLM
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Keywords: comet_llm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `comet_llm-0.0.1/setup.py` & `comet_llm-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,11 +50,11 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="comet_llm",
     name="comet_llm",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://www.comet.ml",
-    version="0.0.1",
+    version="0.0.2",
     zip_safe=False,
     license="Proprietary",
 )
```

### Comparing `comet_llm-0.0.1/src/comet_llm/__init__.py` & `comet_llm-0.0.2/src/comet_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.1/src/comet_llm/api.py` & `comet_llm-0.0.2/src/comet_llm/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,81 +10,75 @@
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 import io
 import json
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 import flatten_dict
 
 from . import convert, experiment_api, experiment_info
-from .types import JSONEncodable
 
-ASSET_FORMAT_VERSION = 1
+ASSET_FORMAT_VERSION = 3
 
 
 def log_prompt(
-    prompt: JSONEncodable,
-    outputs: JSONEncodable,
+    prompt: str,
+    output: str,
     workspace: Optional[str] = None,
     project: Optional[str] = None,
     api_key: Optional[str] = None,
-    prompt_template: Optional[JSONEncodable] = None,
-    prompt_template_variables: Optional[Dict[str, JSONEncodable]] = None,
-    metadata: Optional[Dict[str, JSONEncodable]] = None,
+    prompt_template: Optional[str] = None,
+    prompt_template_variables: Optional[
+        Dict[str, Union[str, bool, float, None]]
+    ] = None,
+    metadata: Optional[Dict[str, str]] = None,
     start_timestamp: Optional[float] = None,
     end_timestamp: Optional[float] = None,
     duration: Optional[float] = None,
 ) -> None:
     """
-    Returns a Comet API Key Secret that can be used instead of a clear-text API Key when creating an
-    Experiment or API object. The Comet API Key Secret is a string that represents the location of
-    the secret in the GCP Secret Manager without containing the API Key. This means
-    `get_api_key_from_secret_manager` doesn't need permission or access to GCP Secret Manager.
+    Logs a single prompt and output to Comet platform.
 
     Args:
-        prompt: JSONEncodable (required) input prompt to LLM.
-        outputs: JSONEncodable (required), outputs from LLM.
+        prompt: str (required) input prompt to LLM.
+        output: str (required), output from LLM.
         workspace: str (optional) comet workspace to use for logging.
         project: str (optional) project name to create in comet workspace.
         api_key: str (optional) comet API key.
-        prompt_template: JSONEncodable (optional) user-defined template used for creating a prompt.
-        prompt_template_variables: Dict[str, JSONEncodable] (optional) dictionary with data used
+        prompt_template: str (optional) user-defined template used for creating a prompt.
+        prompt_template_variables: Dict[str, str] (optional) dictionary with data used
             in prompt_template to build a prompt.
-        metadata: Dict[str, JSONEncodable] (optional) user-defined dictionary with additional
-            metadata to the call.
+        metadata: Dict[str, Union[str, bool, float, None]] (optional) user-defined
+            dictionary with additional metadata to the call.
         start_timestamp: float (optional) start timestamp of prompt call
         end_timestamp: float (optional) end timestamp of prompt call
         duration: float (optional) duration of prompt call
+
     Example:
 
     ```python
     log_prompt(
         prompt="Answer the question and if the question can't be answered, say \"I don't know\"\n\n---\n\nQuestion: What is your name?\nAnswer:",
         metadata={
-            "prompt": {
-                "model": "text-davinci-003",
-                "provider": "openai",
-                "temperature": 0.95,
-                "presence_penalty": -1,
-            },
-            "output": {
-                "id": "cmpl-76ehKGbEMC0BIwTPH0m1W4YoY3oPV",
-                "object": "text-completion",
-                "index": 0,
-                "logprobs": None,
-                "finish_reason": "stop",
-                "usage": {"prompt_tokens": 34, "completion_tokens": 7, "total_tokens": 41},
-            },
+            "input.type": "completions",
+            "input.model": "text-davinci-003",
+            "input.provider": "openai",
+            "output.index": 0,
+            "output.logprobs": None,
+            "output.finish_reason": "length",
+            "usage.prompt_tokens": 5,
+            "usage.completion_tokens": 7,
+            "usage.total_tokens": 12,
         },
         prompt_template="Answer the question and if the question can't be answered, say \"I don't know\"\n\n---\n\nQuestion: {{question}}?\nAnswer:",
         prompt_template_variables={"question": "What is your name?"},
-        outputs=" My name is [your name].",
+        output=" My name is [your name].",
         duration=16.598,
     )
 
     ```
 
     Returns: None.
     """
@@ -100,67 +94,45 @@
         api_key_not_found_message=LOG_PROMPT_API_KEY_NOT_FOUND_MESSAGE,
     )
     experiment_api_ = experiment_api.ExperimentAPI(
         api_key=info.api_key, workspace=info.workspace, project_name=info.project_name
     )
 
     call_data = convert.call_data_to_dict(
-        id=0,
         prompt=prompt,
-        outputs=outputs,
+        outputs=output,
         metadata=metadata,
         prompt_template=prompt_template,
         prompt_template_variables=prompt_template_variables,
         start_timestamp=start_timestamp,
         end_timestamp=end_timestamp,
         duration=duration,
     )
 
     asset_data = {
-        "_version": ASSET_FORMAT_VERSION,
+        "version": ASSET_FORMAT_VERSION,
         "chain_nodes": [call_data],
-        "chain_edges": [],
-        "chain_context": {"parent_context_id": {}},
         "chain_inputs": {
             "final_prompt": prompt,
             "prompt_template": prompt_template,
             "prompt_template_variables": prompt_template_variables,
         },
-        "chain_outputs": {"output": outputs},
+        "chain_outputs": {"output": output},
+        "category": "single_prompt",
         "metadata": {},
         "start_timestamp": start_timestamp,
         "end_timestamp": end_timestamp,
-        "duration": duration,
+        "chain_duration": duration,
     }
 
     experiment_api_.log_asset_with_io(
-        name="comet_llm_data.json", file=io.StringIO(json.dumps(asset_data))
+        name="comet_llm_data.json",
+        file=io.StringIO(json.dumps(asset_data)),
+        asset_type="llm_data",
     )
 
-    parameters = _prepare_parameters(metadata, start_timestamp, end_timestamp, duration)
-    for name, value in parameters.items():
-        experiment_api_.log_parameter(name, value)
-
-
-def _prepare_parameters(
-    metadata: Optional[Dict[str, Any]],
-    start_timestamp: Optional[float],
-    end_timestamp: Optional[float],
-    duration: Optional[float],
-) -> Dict[str, Any]:
-
-    timestamp_parameters = {
-        "start_timestamp": start_timestamp,
-        "end_timestamp": end_timestamp,
-        "duration": duration,
-    }
-    metadata_parameters = (
-        flatten_dict.flatten(metadata, reducer="dot") if metadata is not None else {}
+    parameters = convert.chain_metadata_to_flat_dict(
+        metadata, start_timestamp, end_timestamp, duration
     )
 
-    result = {
-        key: value
-        for key, value in {**timestamp_parameters, **metadata_parameters}.items()
-        if value is not None
-    }
-
-    return result
+    for name, value in parameters.items():
+        experiment_api_.log_parameter(name, value)
```

### Comparing `comet_llm-0.0.1/src/comet_llm/config.py` & `comet_llm-0.0.2/src/comet_llm/config.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.1/src/comet_llm/convert.py` & `comet_llm-0.0.2/src/comet_llm/convert.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,41 +10,63 @@
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 from typing import Any, Dict, Optional
 
-from .types import JSONEncodable
+import flatten_dict
 
-CALL_DICT_VERSION = 1
+from .types import JSONEncodable
 
 
 def call_data_to_dict(
     prompt: JSONEncodable,
     outputs: JSONEncodable,
-    id: int,
     metadata: Optional[Dict[str, Any]] = None,
     prompt_template: Optional[JSONEncodable] = None,
     prompt_template_variables: Optional[JSONEncodable] = None,
     start_timestamp: Optional[float] = None,
     end_timestamp: Optional[float] = None,
     duration: Optional[float] = None,
 ) -> Dict[str, Any]:
-
-    result = {
-        "_id": id,
-        "_type": "llm_call",
+    return {
+        "id": 1,
+        "category": "llm-call",
+        "name": "llm-call-1",
         "inputs": {
             "final_prompt": prompt,
             "prompt_template": prompt_template,
             "prompt_template_variables": prompt_template_variables,
         },
-        "outputs": outputs,
+        "outputs": {"output": outputs},
         "duration": duration,
         "start_timestamp": start_timestamp,
         "end_timestamp": end_timestamp,
-        "context": [],
+        "parent_ids": [],
         "metadata": metadata,
     }
 
+
+def chain_metadata_to_flat_dict(
+    metadata: Optional[Dict[str, Any]],
+    start_timestamp: Optional[float],
+    end_timestamp: Optional[float],
+    duration: Optional[float],
+) -> Dict[str, Any]:
+
+    timestamp_parameters = {
+        "start_timestamp": start_timestamp,
+        "end_timestamp": end_timestamp,
+        "chain_duration": duration,
+    }
+    metadata_parameters = (
+        flatten_dict.flatten(metadata, reducer="dot") if metadata is not None else {}
+    )
+
+    result = {
+        key: value
+        for key, value in {**timestamp_parameters, **metadata_parameters}.items()
+        if value is not None
+    }
+
     return result
```

### Comparing `comet_llm-0.0.1/src/comet_llm/exceptions.py` & `comet_llm-0.0.2/src/comet_llm/exceptions.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.1/src/comet_llm/experiment_api/__init__.py` & `comet_llm-0.0.2/src/comet_llm/experiment_api/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.1/src/comet_llm/experiment_api/comet_api_client.py` & `comet_llm-0.0.2/src/comet_llm/experiment_api/comet_api_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,23 +28,23 @@
 
 class CometAPIClient:
     def __init__(self, api_key: str, comet_url: str):
         self._headers = {"Authorization": api_key}
         self._comet_url = comet_url
 
     def create_experiment(
-        self, workspace: Optional[str], project: Optional[str]
+        self,
+        type_: str,
+        workspace: Optional[str],
+        project: Optional[str],
     ) -> ResponseContent:
         return self._request(
             "POST",
             "/api/rest/v2/write/experiment/create",
-            json={
-                "workspaceName": workspace,
-                "projectName": project,
-            },
+            json={"workspaceName": workspace, "projectName": project, "type": type_},
         )
 
     def log_experiment_parameter(
         self, experiment_key: str, name: str, value: JSONEncodable
     ) -> ResponseContent:
         return self._request(
             "POST",
@@ -53,22 +53,31 @@
                 "experimentKey": experiment_key,
                 "parameterName": name,
                 "parameterValue": value,
             },
         )
 
     def log_experiment_asset_with_io(
-        self, experiment_key: str, name: str, file: IO
+        self,
+        experiment_key: str,
+        name: str,
+        file: IO,
+        asset_type: str,
+        extension: Optional[str] = None,
     ) -> ResponseContent:
+        extension = name.split(".")[-1] if extension is None else extension
+
         return self._request(
             "POST",
             "/api/rest/v2/write/experiment/upload-asset",
             params={
                 "experimentKey": experiment_key,
                 "fileName": name,
+                "extension": extension,
+                "type": asset_type,
             },
             files={"file": file},
         )
 
     @request_exception_wrapper.wrap
     def _request(self, method: str, path: str, *args, **kwargs) -> ResponseContent:  # type: ignore
         url = urllib.parse.urljoin(self._comet_url, path)
```

### Comparing `comet_llm-0.0.1/src/comet_llm/experiment_api/experiment_api.py` & `comet_llm-0.0.2/src/comet_llm/experiment_api/experiment_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     ):
         self._client = comet_api_client.get(api_key)
         self._initialize_experiment(workspace, project_name)
 
     def _initialize_experiment(
         self, workspace: Optional[str] = None, project_name: Optional[str] = None
     ) -> None:
-        response = self._client.create_experiment(workspace, project_name)
+        response = self._client.create_experiment("LLM", workspace, project_name)
         self._experiment_key = response["experimentKey"]
 
-    def log_asset_with_io(self, name: str, file: IO) -> None:
+    def log_asset_with_io(self, name: str, file: IO, asset_type: str) -> None:
         self._client.log_experiment_asset_with_io(
-            self._experiment_key, name=name, file=file
+            self._experiment_key, name=name, file=file, asset_type=asset_type
         )
 
     def log_parameter(self, name: str, value: Any) -> None:
         self._client.log_experiment_parameter(
             self._experiment_key, name=name, value=value
         )
```

### Comparing `comet_llm-0.0.1/src/comet_llm/experiment_api/request_exception_wrapper.py` & `comet_llm-0.0.2/src/comet_llm/experiment_api/request_exception_wrapper.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.1/src/comet_llm/experiment_info.py` & `comet_llm-0.0.2/src/comet_llm/experiment_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # *******************************************************
 
 import dataclasses
 from typing import Optional
 
 from . import config, exceptions
 
+DEFAULT_PROJECT_NAME = "llm-general"
+
 
 @dataclasses.dataclass
 class ExperimentInfo:
     api_key: str
     workspace: Optional[str]
     project_name: Optional[str]
 
@@ -34,8 +36,10 @@
     api_key = api_key if api_key else config.api_key()
     if api_key is None:
         raise exceptions.CometLLMException(api_key_not_found_message)
 
     workspace = workspace if workspace else config.workspace()
     project_name = project_name if project_name else config.project_name()
 
+    project_name = project_name if project_name else DEFAULT_PROJECT_NAME
+
     return ExperimentInfo(api_key, workspace, project_name)
```

### Comparing `comet_llm-0.0.1/src/comet_llm/types.py` & `comet_llm-0.0.2/src/comet_llm/types.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.1/src/comet_llm.egg-info/PKG-INFO` & `comet_llm-0.0.2/src/comet_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet-llm
-Version: 0.0.1
+Version: 0.0.2
 Summary: Comet logger for LLM
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Keywords: comet_llm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `comet_llm-0.0.1/src/comet_llm.egg-info/SOURCES.txt` & `comet_llm-0.0.2/src/comet_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

