# Comparing `tmp/permutate-0.0.1.tar.gz` & `tmp/permutate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permutate-0.0.1.tar", max compression
+gzip compressed data, was "permutate-0.0.2.tar", max compression
```

## Comparing `permutate-0.0.1.tar` & `permutate-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     3488 2023-05-25 19:24:36.085184 permutate-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-25 13:34:42.177953 permutate-0.0.1/permutate/__init__.py
--rw-r--r--   0        0        0     1357 2023-05-25 15:11:34.401302 permutate-0.0.1/permutate/job_request_schema.py
--rw-r--r--   0        0        0     4369 2023-05-25 18:39:22.672787 permutate-0.0.1/permutate/job_response_schema.py
--rw-r--r--   0        0        0     1019 2023-05-25 18:39:22.677544 permutate-0.0.1/permutate/logger.py
--rw-r--r--   0        0        0     7928 2023-05-25 18:53:30.758320 permutate-0.0.1/permutate/main.py
--rw-r--r--   0        0        0      559 2023-05-25 17:31:15.484872 permutate-0.0.1/permutate/singleton.py
--rw-r--r--   0        0        0      424 2023-05-25 14:14:19.775886 permutate-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4151 1970-01-01 00:00:00.000000 permutate-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3488 2023-05-25 19:24:36.085184 permutate-0.0.2/README.md
+-rw-r--r--   0        0        0      109 2023-05-31 04:30:07.057254 permutate-0.0.2/permutate/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-31 03:53:49.018228 permutate-0.0.2/permutate/__main__.py
+-rw-r--r--   0        0        0     2135 2023-05-30 20:40:58.184224 permutate-0.0.2/permutate/job_request_schema.py
+-rw-r--r--   0        0        0     9361 2023-05-31 04:48:07.058385 permutate-0.0.2/permutate/job_response_schema.py
+-rw-r--r--   0        0        0     1138 2023-05-31 04:36:41.664733 permutate-0.0.2/permutate/logger.py
+-rw-r--r--   0        0        0      668 2023-05-31 05:04:41.759961 permutate-0.0.2/permutate/main.py
+-rw-r--r--   0        0        0     7107 2023-05-31 04:56:20.655804 permutate-0.0.2/permutate/runner.py
+-rw-r--r--   0        0        0      559 2023-05-25 17:31:15.484872 permutate-0.0.2/permutate/singleton.py
+-rw-r--r--   0        0        0      271 2023-05-31 04:39:10.442019 permutate-0.0.2/permutate/test.py
+-rw-r--r--   0        0        0      523 2023-05-31 05:12:08.983755 permutate-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 permutate-0.0.2/PKG-INFO
```

### Comparing `permutate-0.0.1/README.md` & `permutate-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `permutate-0.0.1/permutate/main.py` & `permutate-0.0.2/permutate/runner.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,176 +1,150 @@
 import json
 import requests
 import webbrowser
 from tqdm import tqdm
 from .logger import logger
 from datetime import datetime
-from prettytable import PrettyTable
 from .job_request_schema import JobRequest
 from .job_response_schema import JobResponse, JobSummary, JobDetail
 
-pbar = tqdm(total=100)
-progress_counter = 25
 
+class Runner:
 
-def permutate(file_path: str, save_to_html=True, save_to_csv=True):
-    logger.info("Starting permutate")
-    with open(file_path) as f:
-        yaml_file = f.read()
-    request = JobRequest.parse_raw(yaml_file)
-
-    batch_job_started_on = datetime.now()
-    all_details = []
-    all_summaries = []
-    for permutation in request.permutations:
-        permutation_details = single_permutation(request, permutation)
-        permutation_summary = JobSummary.build_from_details(permutation_details, permutation.name, 0)
-        all_details.extend(permutation_details)
-        all_summaries.append(permutation_summary)
-
-    response = JobResponse(
-        started_on=batch_job_started_on,
-        completed_on=datetime.now(),
-        permutations=request.permutations,
-        summaries=all_summaries,
-        details=all_details
-    )
-    pbar.close()
-    response.save_to_csv(break_down_by_environment=False) if save_to_csv else None
-    if save_to_html:
-        build_pretty_table(response)
-        webbrowser.open("file:///Users/shrikant/Workspace/PythonWorkspace/permutate/workspace/job_result.html")
-
-
-def build_pretty_table(response: JobResponse):
-    table = PrettyTable()
-    table = PrettyTable()
-    table.format = True
-    table.header = False
-    table.padding_width = 1
-    table.preserve_internal_border = True
-    table.border = True
-    table.add_row(["Tool", "Pipeline", "LLM", "Model", "Completed?", "Language",
-                   "Match Score", "Plugin Detected", "Operation Found", "Parameters Mapped",
-                   "Parameter Mapped Percentage", "Response Time(in seconds)", "LLM Tokens Used", "LLM API Cost"])
-    for detail in response.details:
-        permutation = response.get_permutation_by_name(detail.permutation_name)
-        table.add_row([permutation.tool_selector.get("provider"), permutation.tool_selector.get("pipeline_name"),
-                       permutation.llm.get("provider"), permutation.llm.get("model_name"), detail.is_run_completed,
-                       detail.language, detail.match_score, detail.is_plugin_detected, detail.is_plugin_operation_found,
-                       detail.is_plugin_parameter_mapped, detail.parameter_mapped_percentage, detail.response_time_sec,
-                       detail.total_llm_tokens_used, detail.llm_api_cost])
-
-    # build and save html
-    html_table = table.get_html_string(attributes={"id": "my_table", "class": "red_table"})
-    row_index = 1
-    css_styling = "background-color: yellow; color: blue;"
-    enhanced_row = f'<tr style="{css_styling}">' + html_table.split('\n')[row_index] + "</tr>"
-    styled_table_str = '\n'.join([html_table.split('\n')[i] if i != 2 else enhanced_row
-                                  for i in range(len(html_table.split('\n')))])
-    styled_html_table = f"""
-    <style>
-        table {{ border-collapse: collapse; margin: 1em 0; }}
-        th, td {{ padding: 8px; border: 1px solid black; }}
-        thead {{ background-color: lightgray; }}
-        /* Add more CSS styles as needed */
-    </style>
-    {styled_table_str}
-    """
-    with open("workspace/job_result.html", "w") as f:
-        f.write(styled_html_table)
-
-
-def single_permutation(request, permutation):
-    permutation_details = []
-    permutation_summary = f"{permutation.llm.get('provider')}[{permutation.llm.get('model_name')}] - {permutation.tool_selector.get('provider')}[{permutation.tool_selector.get('pipeline_name')}]"
-    for test_case in request.test_cases:
-        pbar.update(progress_counter)
-        plugin_group = request.get_plugin_group_from_permutation(permutation)
-        detail = run_single_permutation_test_case(
-            test_case,
-            request.config,
-            permutation,
-            plugin_group,
-            permutation_summary
+    def __init__(self, show_progress_bar: bool = True):
+        self.show_progress_bar = show_progress_bar
+        if self.show_progress_bar:
+            self.pbar = tqdm(total=100)
+            self.progress_counter = None
+
+    def start(self, file_path: str, save_to_html=True, save_to_csv=True):
+        logger.info("Starting permutate")
+        with open(file_path) as f:
+            yaml_file = f.read()
+        request = JobRequest.parse_raw(yaml_file)
+        self.progress_counter = 100 / (len(request.permutations) * len(request.test_cases))
+        batch_job_started_on = datetime.now()
+        all_details = []
+        for permutation in request.permutations:
+            permutation_details = self.single_permutation(request, permutation)
+            all_details.extend(permutation_details)
+
+        summary = JobSummary.build_from_details(all_details)
+        response = JobResponse(
+            started_on=batch_job_started_on,
+            completed_on=datetime.now(),
+            test_plugin=request.test_plugin,
+            permutations=request.permutations,
+            summary=summary,
+            details=all_details
         )
-        permutation_details.append(detail)
-        break
-    return permutation_details
-
-
-def run_single_permutation_test_case(test_case, config, permutation, plugin_group, permutation_summary):
-    if permutation.tool_selector.get("provider") == "Imprompt":
-        url = config.imprompt_tool_selector
-    elif permutation.tool_selector.get("provider") == "Langchain":
-        url = config.langchain_tool_selector
-    payload = json.dumps({
-        "messages": [{
-            "content": test_case.prompt,
-            "message_type": "HumanMessage"
-        }],
-        "plugins": plugin_group.dict().get("plugins"),
-        "config": config.dict(),
-        "tool_selector_config": permutation.tool_selector,
-        "llm": permutation.llm
-    })
-    headers = {'Content-Type': 'application/json'}
-    response = requests.request("POST", url, headers=headers, data=payload)
-    if response.status_code == 200:
-        response_json = response.json()
-        is_plugin_detected = False
-        is_plugin_operation_found = False
-        is_plugin_parameter_mapped = False
-        parameter_mapped_percentage = 0
-        for detected_plugin_operation in response_json.get("detected_plugin_operations"):
-            if detected_plugin_operation.get("plugin").get("name_for_model") == test_case.expected_plugin_used or \
-                    detected_plugin_operation.get("plugin").get("name_for_human") == test_case.expected_plugin_used:
-                is_plugin_detected = True
-                if detected_plugin_operation.get("plugin").get("api_called") == test_case.expected_api_used:
-                    is_plugin_operation_found = True
-                extracted_params = detected_plugin_operation.get("mapped_operation_parameters")
-                if extracted_params:
-                    expected_params = test_case.expected_parameters
-                    common_pairs = {k: extracted_params[k] for k in extracted_params if
-                                    k in expected_params and extracted_params[k] == expected_params[k]}
-                    if len(common_pairs) == len(expected_params):
-                        parameter_mapped_percentage = 100
-                        is_plugin_parameter_mapped = True
-                    else:
-                        parameter_mapped_percentage = len(common_pairs) / len(expected_params) * 100
-                break
-        detail = JobDetail(
-            permutation_name=permutation.name,
-            permutation_summary=permutation_summary,
-            test_case_name=test_case.name,
-            is_run_completed=True,
-            language="English",
-            prompt=test_case.prompt,
-            final_output=response_json.get("final_text_response"),
-            match_score="0.0",
-            is_plugin_detected=is_plugin_detected,
-            is_plugin_operation_found=is_plugin_operation_found,
-            is_plugin_parameter_mapped=is_plugin_parameter_mapped,
-            parameter_mapped_percentage=parameter_mapped_percentage,
-            response_time_sec=response_json.get("response_time"),
-            total_llm_tokens_used=response_json.get("tokens_used"),
-            llm_api_cost=response_json.get("llm_api_cost")
-        )
-    else:
-        detail = JobDetail(
-            permutation_name=permutation.name,
-            permutation_summary=permutation_summary,
-            test_case_name=test_case.name,
-            is_run_completed=False,
-            language="English",
-            prompt=test_case.prompt,
-            final_output=f"FAILED",
-            match_score="0.0",
-            is_plugin_detected=False,
-            is_plugin_operation_found=False,
-            is_plugin_parameter_mapped=False,
-            parameter_mapped_percentage=0,
-            response_time_sec=0,
-            total_llm_tokens_used=0,
-            llm_api_cost=0
-        )
-    return detail
+        if self.show_progress_bar:
+            self.pbar.close()
+        response.save_to_csv(break_down_by_environment=False) if save_to_csv else None
+        if save_to_html:
+            url = response.build_html_table()
+            webbrowser.open(url)
+
+    def single_permutation(self, request, permutation):
+        permutation_details = []
+        permutation_summary = f"{permutation.llm.get('provider')}[{permutation.llm.get('model_name')}] - {permutation.tool_selector.get('provider')}[{permutation.tool_selector.get('pipeline_name')}]"
+        for test_case in request.test_cases:
+            if self.show_progress_bar:
+                self.pbar.update(self.progress_counter)
+            plugin_group = request.get_plugin_group_from_permutation(permutation)
+            detail = self.run_single_permutation_test_case(
+                test_case,
+                request.config,
+                permutation,
+                plugin_group,
+                permutation_summary
+            )
+            permutation_details.append(detail)
+        return permutation_details
+
+    @staticmethod
+    def run_single_permutation_test_case(test_case, config, permutation, plugin_group, permutation_summary):
+        if permutation.tool_selector.get("provider") == "Imprompt":
+            url = config.imprompt_tool_selector
+        elif permutation.tool_selector.get("provider") == "Langchain":
+            url = config.langchain_tool_selector
+        else:
+            raise Exception("Tool selector provider not supported")
+        payload = json.dumps({
+            "messages": [{
+                "content": test_case.prompt,
+                "message_type": "HumanMessage"
+            }],
+            "plugins": plugin_group.dict().get("plugins"),
+            "config": config.dict(),
+            "tool_selector_config": permutation.tool_selector,
+            "llm": permutation.llm
+        })
+        headers = {'Content-Type': 'application/json'}
+        response = requests.request("POST", url, headers=headers, data=payload)
+        if response.status_code == 200:
+            response_json = response.json()
+            is_plugin_detected = False
+            is_plugin_operation_found = False
+            is_plugin_parameter_mapped = False
+            parameter_mapped_percentage = 0
+            plugin_operation = None
+            plugin_name = None
+            plugin_parameters_mapped = None
+            for detected_plugin_operation in response_json.get("detected_plugin_operations"):
+                if detected_plugin_operation.get("plugin").get("name_for_model") == test_case.expected_plugin_used or \
+                        detected_plugin_operation.get("plugin").get("name_for_human") == test_case.expected_plugin_used:
+                    is_plugin_detected = True
+                    plugin_name = detected_plugin_operation.get("plugin").get("name_for_human")
+                    if detected_plugin_operation.get("plugin").get("api_called") == test_case.expected_api_used:
+                        is_plugin_operation_found = True
+                    plugin_operation = detected_plugin_operation.get("plugin").get("api_called")
+                    plugin_parameters_mapped = detected_plugin_operation.get("mapped_operation_parameters")
+                    if plugin_parameters_mapped:
+                        expected_params = test_case.expected_parameters
+                        common_pairs = {k: plugin_parameters_mapped[k] for k in plugin_parameters_mapped if
+                                        k in expected_params and plugin_parameters_mapped[k] == expected_params[k]}
+                        if len(common_pairs) == len(expected_params):
+                            parameter_mapped_percentage = 100
+                            is_plugin_parameter_mapped = True
+                        else:
+                            parameter_mapped_percentage = len(common_pairs) / len(expected_params) * 100
+
+            detail = JobDetail(
+                permutation_name=permutation.name,
+                permutation_summary=permutation_summary,
+                test_case_name=test_case.name,
+                is_run_completed=True,
+                language="English",
+                prompt=test_case.prompt,
+                final_output=response_json.get("final_text_response"),
+                match_score="0.0",
+                is_plugin_detected=is_plugin_detected,
+                is_plugin_operation_found=is_plugin_operation_found,
+                is_plugin_parameter_mapped=is_plugin_parameter_mapped,
+                parameter_mapped_percentage=parameter_mapped_percentage,
+                plugin_name=plugin_name,
+                plugin_operation=plugin_operation,
+                plugin_parameters_mapped=plugin_parameters_mapped,
+                response_time_sec=response_json.get("response_time"),
+                total_llm_tokens_used=response_json.get("tokens_used"),
+                llm_api_cost=response_json.get("llm_api_cost")
+            )
+        else:
+            detail = JobDetail(
+                permutation_name=permutation.name,
+                permutation_summary=permutation_summary,
+                test_case_name=test_case.name,
+                is_run_completed=False,
+                language="English",
+                prompt=test_case.prompt,
+                final_output=f"FAILED",
+                match_score="0.0",
+                is_plugin_detected=False,
+                is_plugin_operation_found=False,
+                is_plugin_parameter_mapped=False,
+                parameter_mapped_percentage=0,
+                response_time_sec=0,
+                total_llm_tokens_used=0,
+                llm_api_cost=0
+            )
+        return detail
```

### Comparing `permutate-0.0.1/permutate/singleton.py` & `permutate-0.0.2/permutate/singleton.py`

 * *Files identical despite different names*

### Comparing `permutate-0.0.1/PKG-INFO` & `permutate-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: permutate
-Version: 0.0.1
+Version: 0.0.2
 Summary: Testing framework for LLM Plugins
 Author: shrikant
 Author-email: shrikant.pm14@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: prettytable (>=3.7.0,<4.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pydantic-yaml (>=0.11.2,<0.12.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (==2.29.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Permutate
 ![Alt text](docs/logo.png?raw=true "Title")
 #### Permutate is an automated testing framework for LLM Plugins. 
 
 ##### ChatGPT Ignited LLM Plugins
```

