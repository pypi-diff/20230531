# Comparing `tmp/checkmk_dev_tools-0.1.4.tar.gz` & `tmp/checkmk_dev_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkmk_dev_tools-0.1.4.tar", max compression
+gzip compressed data, was "checkmk_dev_tools-0.1.5.tar", max compression
```

## Comparing `checkmk_dev_tools-0.1.4.tar` & `checkmk_dev_tools-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1056 2023-05-17 11:57:16.555506 checkmk_dev_tools-0.1.4/README.rst
--rw-r--r--   0        0        0        0 2023-05-10 11:17:07.102380 checkmk_dev_tools-0.1.4/cmk_dev/__init__.py
--rwxr-xr-x   0        0        0    11148 2023-05-22 12:22:21.988260 checkmk_dev_tools-0.1.4/cmk_dev/ci_artifacts.py
--rwxr-xr-x   0        0        0     2184 2023-05-10 11:28:30.476996 checkmk_dev_tools-0.1.4/cmk_dev/cli.py
--rwxr-xr-x   0        0        0     2249 2023-05-10 11:18:34.886818 checkmk_dev_tools-0.1.4/cmk_dev/listen_std.py
--rw-r--r--   0        0        0     1919 2023-05-22 12:55:27.493637 checkmk_dev_tools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 checkmk_dev_tools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-31 14:32:38.730307 checkmk_dev_tools-0.1.5/README.rst
+-rw-r--r--   0        0        0        0 2023-05-10 11:17:07.102380 checkmk_dev_tools-0.1.5/cmk_dev/__init__.py
+-rwxr-xr-x   0        0        0    12759 2023-05-31 14:32:31.574262 checkmk_dev_tools-0.1.5/cmk_dev/ci_artifacts.py
+-rwxr-xr-x   0        0        0     2184 2023-05-10 11:28:30.476996 checkmk_dev_tools-0.1.5/cmk_dev/cli.py
+-rwxr-xr-x   0        0        0     2249 2023-05-10 11:18:34.886818 checkmk_dev_tools-0.1.5/cmk_dev/listen_std.py
+-rw-r--r--   0        0        0     1919 2023-05-31 14:33:16.562542 checkmk_dev_tools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 checkmk_dev_tools-0.1.5/PKG-INFO
```

### Comparing `checkmk_dev_tools-0.1.4/README.rst` & `checkmk_dev_tools-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.4/cmk_dev/ci_artifacts.py` & `checkmk_dev_tools-0.1.5/cmk_dev/ci_artifacts.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,19 @@
 from collections.abc import Mapping
 from configparser import ConfigParser
 from contextlib import contextmanager, suppress
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 
+import yaml
 from jenkins import Jenkins, JenkinsException
 
+# pylint: disable=too-many-instance-attributes
+
 
 def parse_args() -> Args:
     """Cool git like multi command argument parser"""
     parser = ArgumentParser("Provide CI artifacts locally")
     parser.add_argument(
         "--log-level",
         "-l",
@@ -52,14 +55,15 @@
             " ~/.config/jenkins_jobs/jenkins_jobs.ini is being used."
         ),
     )
     parser_fetch.add_argument("-p", "--params", type=split_params, action="append")
     parser_fetch.add_argument(
         "-t",
         "--time-constraints",
+        type=str,
         default="today",
     )
     parser_fetch.add_argument(
         "-o",
         "--out-dir",
         default="out",
         type=Path,
@@ -78,14 +82,15 @@
     return logging.getLogger("ci-artifacts")
 
 
 @dataclass
 class Build:
     """Models a Jenkins job build"""
 
+    number: int
     timestamp: datetime
     result: str
     building: str
     artifacts: list[str]
     parameters: str
     in_progress: bool
 
@@ -93,14 +98,15 @@
         def params_from(build_info):
             """Return job parameters of provided @build_info as dict"""
             for action in build_info["actions"]:
                 if action.get("_class") == "hudson.model.ParametersAction":
                     return {p["name"]: p["value"] for p in action["parameters"]}
             return {}
 
+        self.number = raw_build_info["number"]
         self.timestamp = datetime.fromtimestamp(raw_build_info["timestamp"] // 1000)
         self.result = raw_build_info["result"]
         self.building = raw_build_info["building"]
         self.artifacts = [a["relativePath"] for a in raw_build_info["artifacts"]]
         self.parameters = params_from(raw_build_info)
         self.url = raw_build_info["url"]
         self.in_progress = raw_build_info["inProgress"]
@@ -130,17 +136,17 @@
 
     def __init__(self, raw_job_info):
         self.name = raw_job_info["name"]
         self.fullname = raw_job_info["fullName"]
         self.jobs = [j["name"] for j in raw_job_info["jobs"]]
 
 
-def extract_credentials(credentials: Mapping[str, str]) -> Mapping[str, str]:
+def extract_credentials(credentials: None | Mapping[str, str]) -> Mapping[str, str]:
     """Turns the information provided via --credentials into actual values"""
-    if (
+    if credentials and (
         any(key in credentials for key in ("url", "url_env"))
         and any(key in credentials for key in ("username", "username_env"))
         and any(key in credentials for key in ("password", "password_env"))
     ):
         return {
             "url": credentials.get("url") or os.environ[credentials.get("url_env")],
             "username": credentials.get("username") or os.environ[credentials.get("username_env")],
@@ -183,20 +189,22 @@
             print(f"Don't know class type {class_name}", file=sys.stderr)
             raise SystemExit(-1)
 
 
 def meets_constraints(build, params, time_constraints):
     """Checks if a set of requirements are met for a given build"""
     if build.parameters != params:
-        print(f"don't match: {build.parameters} != {params}")
+        logger().debug("don't match: %s != %s", build.parameters, params)
         return False
 
     if time_constraints == "today":
         if build.timestamp.date() != datetime.now().date():
-            print(f"Time constraints not met: {build.timestamp.date()} != {datetime.now().date()}")
+            logger().debug(
+                "time constraints not met: %s != %s", build.timestamp.date(), datetime.now().date()
+            )
             return False
     else:
         raise RuntimeError(f"Don't understand {time_constraints}")
 
     return True
 
 
@@ -248,53 +256,84 @@
             logger().debug("Download: %s", fp_filename)
             reply.raise_for_status()
             with open(artifact_filename, "wb") as out_file:
                 for chunk in reply.iter_content(chunk_size=1 << 16):
                     out_file.write(chunk)
 
 
+def find_matching_build(job: Job, params: Mapping[str, str | int], time_constraints: str) -> Build:
+    """Goes through a job's build items and returns the first one to match certain criteria or None
+    if none is found"""
+    for build_id, build in job.builds.items():
+        if meets_constraints(build, params, time_constraints):
+            print(
+                f"Found matching build: {build_id}"
+                f" {build.timestamp} {build.result} {build.parameters}"
+            )
+            for key, value in build.__dict__.items():
+                print(f"  {key}: {value}")
+            return build
+    return None
+
+
+def create_new(client, job_full_path, params: Mapping[str, str | int]) -> Build:
+    """Starts a job specified by @job_full_path using @params and returns its build info object"""
+    queue_id = client.build_job(job_full_path, params)
+    while True:
+        queue_item = client.get_queue_item(queue_id)
+        print(yaml.dump(queue_item))
+        if executable := queue_item.get("executable"):
+            print(yaml.dump(executable))
+            return Build(client.get_build_info(job_full_path, executable["number"]))
+        time.sleep(1)
+
+
 def fn_fetch(args: Args) -> None:
     """Entry point for fetching artifacts"""
     params = {k: v for p in (args.params or []) for k, v in p.items()}
     logger().debug("Parsed params: %s", params)
+    fetch_job_artifacts(args.job, params, args.time_constraints, args.credentials, args.out_dir)
 
-    with jenkins_client(**extract_credentials(args.credentials)) as client:
-        if not (job_info := client.get_job_info(args.job))["_class"].endswith("WorkflowJob"):
-            logger().error("'%s' is not a WorkflowJob", args.job)
+
+def fetch_job_artifacts(job_full_path, params, time_constraints, credentials, out_dir) -> None:
+    """Returns artifacts of Jenkins job specified by @job_full_path matching @params and
+    @time_constraints. If none of the existing builds match the conditions a new build will be
+    issued. If the existing build has not finished yet it will be waited for."""
+    with jenkins_client(**extract_credentials(credentials)) as client:
+        if not (job_info := client.get_job_info(job_full_path))["_class"].endswith("WorkflowJob"):
+            logger().error("'%s' is not a WorkflowJob", job_full_path)
             raise SystemExit(-1)
         job = Job(
-            job_info, (client.get_build_info(args.job, b["number"]) for b in job_info["builds"])
+            job_info,
+            (client.get_build_info(job_full_path, b["number"]) for b in job_info["builds"]),
         )
-        for build_id, build in job.builds.items():
-            if meets_constraints(build, params, args.time_constraints):
-                print(
-                    f"Found matching build: {build_id}"
-                    f" {build.timestamp} {build.result} {build.parameters}"
-                )
-                for key, value in build.__dict__.items():
-                    print(f"  {key}: {value}")
-                if build.in_progress or build.building:
-                    print(f"Waiting for job #{build_id} to finish..")
-                    while True:
-                        build = Build(client.get_build_info(args.job, build_id))
-                        if build.in_progress or build.building:
-                            logger().debug(
-                                "build.in_progress=%s build.building=%s",
-                                build.in_progress,
-                                build.building,
-                            )
-                            time.sleep(2)
-                            continue
-                        break
-                if not build.artifacts:
-                    raise RuntimeError("Job has no artifacts!")
 
-                download_artifacts(client, build.url, args.out_dir)
+        build_candidate = find_matching_build(job, params, time_constraints) or create_new(
+            client, job_full_path, params
+        )
+
+        if build_candidate.in_progress or build_candidate.building:
+            print(f"Waiting for job #{build_candidate.number} to finish..")
+            while True:
+                build_candidate = Build(
+                    client.get_build_info(job_full_path, build_candidate.number)
+                )
+                if build_candidate.in_progress or build_candidate.building:
+                    logger().debug(
+                        "build.in_progress=%s build.building=%s",
+                        build_candidate.in_progress,
+                        build_candidate.building,
+                    )
+                    time.sleep(2)
+                    continue
                 break
-            print("===")
+            if not build_candidate.artifacts:
+                raise RuntimeError("Job has no artifacts!")
+
+        download_artifacts(client, build_candidate.url, out_dir)
 
 
 def main() -> None:
     """Entry point for everything else"""
     try:
         args = parse_args()
         logging.basicConfig(
```

### Comparing `checkmk_dev_tools-0.1.4/cmk_dev/cli.py` & `checkmk_dev_tools-0.1.5/cmk_dev/cli.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.4/cmk_dev/listen_std.py` & `checkmk_dev_tools-0.1.5/cmk_dev/listen_std.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.4/pyproject.toml` & `checkmk_dev_tools-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkmk-dev-tools"
-version = "0.1.4"
+version = "0.1.5"
 description = "Checkmk DevOps tools"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/tribe29/checkmk"
 readme = "README.rst"
 packages = [
   {include = "cmk_dev/**/*.py"}
 ]
```

### Comparing `checkmk_dev_tools-0.1.4/PKG-INFO` & `checkmk_dev_tools-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkmk-dev-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Checkmk DevOps tools
 Home-page: https://github.com/tribe29/checkmk
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

