# Comparing `tmp/gen3utils-0.9.2.tar.gz` & `tmp/gen3utils-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3utils-0.9.2.tar", max compression
+gzip compressed data, was "gen3utils-0.9.3.tar", max compression
```

## Comparing `gen3utils-0.9.2.tar` & `gen3utils-0.9.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2023-03-16 22:45:09.469257 gen3utils-0.9.2/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-03-16 22:45:09.473255 gen3utils-0.9.2/LICENSE
--rw-r--r--   0        0        0      558 2023-03-16 22:45:09.473255 gen3utils-0.9.2/NOTICE
--rw-r--r--   0        0        0     2128 2023-03-16 22:45:09.473255 gen3utils-0.9.2/README.md
--rw-r--r--   0        0        0        0 2023-03-16 22:45:09.473255 gen3utils-0.9.2/gen3utils/__init__.py
--rw-r--r--   0        0        0      604 2023-03-16 22:45:09.473255 gen3utils-0.9.2/gen3utils/assertion.py
--rw-r--r--   0        0        0        0 2023-03-16 22:45:09.473255 gen3utils-0.9.2/gen3utils/deployment_changes/__init__.py
--rw-r--r--   0        0        0    15561 2023-03-16 22:45:09.473255 gen3utils-0.9.2/gen3utils/deployment_changes/generate_comment.py
--rw-r--r--   0        0        0     1247 2023-03-16 22:45:09.473255 gen3utils-0.9.2/gen3utils/errors.py
--rw-r--r--   0        0        0        0 2023-03-16 22:45:09.473255 gen3utils-0.9.2/gen3utils/etl/__init__.py
--rw-r--r--   0        0        0      307 2023-03-16 22:45:09.473255 gen3utils-0.9.2/gen3utils/etl/dd_utils.py
--rw-r--r--   0        0        0    15983 2023-03-16 22:45:09.473255 gen3utils-0.9.2/gen3utils/etl/etl_validator.py
--rw-r--r--   0        0        0        0 2023-03-16 22:45:09.473255 gen3utils-0.9.2/gen3utils/gitops/__init__.py
--rw-r--r--   0        0        0    15569 2023-03-16 22:45:09.473255 gen3utils-0.9.2/gen3utils/gitops/gitops_validator.py
--rw-r--r--   0        0        0     6361 2023-03-16 22:45:09.473255 gen3utils-0.9.2/gen3utils/main.py
--rw-r--r--   0        0        0        0 2023-03-16 22:45:09.473255 gen3utils-0.9.2/gen3utils/manifest/__init__.py
--rw-r--r--   0        0        0    13738 2023-03-16 22:45:09.477253 gen3utils-0.9.2/gen3utils/manifest/manifest_validator.py
--rw-r--r--   0        0        0     2030 2023-03-16 22:45:09.477253 gen3utils-0.9.2/gen3utils/manifest/validation_config.yaml
--rw-r--r--   0        0        0     5037 2023-03-16 22:45:09.477253 gen3utils-0.9.2/gen3utils/s3log/s3log.py
--rw-r--r--   0        0        0     2356 2023-03-16 22:45:09.477253 gen3utils-0.9.2/gen3utils/s3log/s3log_worker.py
--rw-r--r--   0        0        0     1211 2023-03-16 22:45:09.477253 gen3utils-0.9.2/gen3utils/utils.py
--rw-r--r--   0        0        0     1263 2023-03-16 22:45:09.481251 gen3utils-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     3148 1970-01-01 00:00:00.000000 gen3utils-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-31 16:19:06.913035 gen3utils-0.9.3/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-05-31 16:19:06.913035 gen3utils-0.9.3/LICENSE
+-rw-r--r--   0        0        0      558 2023-05-31 16:19:06.913035 gen3utils-0.9.3/NOTICE
+-rw-r--r--   0        0        0     2128 2023-05-31 16:19:06.913035 gen3utils-0.9.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/__init__.py
+-rw-r--r--   0        0        0      604 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/assertion.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/deployment_changes/__init__.py
+-rw-r--r--   0        0        0    15561 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/deployment_changes/generate_comment.py
+-rw-r--r--   0        0        0     1247 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/errors.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/etl/__init__.py
+-rw-r--r--   0        0        0      307 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/etl/dd_utils.py
+-rw-r--r--   0        0        0    15983 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/etl/etl_validator.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/gitops/__init__.py
+-rw-r--r--   0        0        0    15569 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/gitops/gitops_validator.py
+-rw-r--r--   0        0        0     6657 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/main.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/manifest/__init__.py
+-rw-r--r--   0        0        0    13738 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/manifest/manifest_validator.py
+-rw-r--r--   0        0        0     2030 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/manifest/validation_config.yaml
+-rw-r--r--   0        0        0     5037 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/s3log/s3log.py
+-rw-r--r--   0        0        0     2356 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/s3log/s3log_worker.py
+-rw-r--r--   0        0        0     1211 2023-05-31 16:19:06.913035 gen3utils-0.9.3/gen3utils/utils.py
+-rw-r--r--   0        0        0     1263 2023-05-31 16:19:06.917033 gen3utils-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     3148 1970-01-01 00:00:00.000000 gen3utils-0.9.3/PKG-INFO
```

### Comparing `gen3utils-0.9.2/LICENSE` & `gen3utils-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/NOTICE` & `gen3utils-0.9.3/NOTICE`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/README.md` & `gen3utils-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/gen3utils/assertion.py` & `gen3utils-0.9.3/gen3utils/assertion.py`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/gen3utils/deployment_changes/generate_comment.py` & `gen3utils-0.9.3/gen3utils/deployment_changes/generate_comment.py`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/gen3utils/errors.py` & `gen3utils-0.9.3/gen3utils/errors.py`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/gen3utils/etl/etl_validator.py` & `gen3utils-0.9.3/gen3utils/etl/etl_validator.py`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/gen3utils/gitops/gitops_validator.py` & `gen3utils-0.9.3/gen3utils/gitops/gitops_validator.py`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/gen3utils/main.py` & `gen3utils-0.9.3/gen3utils/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,23 +55,30 @@
     if recorded_errors:
         for err in recorded_errors:
             logger.error("  - {}".format(err))
         if repository and pull_request_number:
             if not "GITHUB_TOKEN" in os.environ:
                 logger.warning("Missing GITHUB_TOKEN: not commenting on pull request.")
             else:
-                message_header = (
-                    "{}\n :x: etlMapping.yaml - gitops.json mismatch".format(hostname)
-                )
-                comment_on_pr(
-                    repository,
-                    pull_request_number,
-                    message_header,
-                    recorded_errors,
-                )
+                try:
+                    message_header = (
+                        "{}\n :x: etlMapping.yaml - gitops.json mismatch".format(
+                            hostname
+                        )
+                    )
+                    comment_on_pr(
+                        repository,
+                        pull_request_number,
+                        message_header,
+                        recorded_errors,
+                    )
+                except Exception as e:
+                    logger.warning(
+                        f"Unable to comment on pull request - continuing. Details: {e}"
+                    )
 
     if not ok:
         raise AssertionError(
             "Portal configuration validation failed. See errors in previous logs."
         )
     else:
         logger.info("  OK!")
```

### Comparing `gen3utils-0.9.2/gen3utils/manifest/manifest_validator.py` & `gen3utils-0.9.3/gen3utils/manifest/manifest_validator.py`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/gen3utils/manifest/validation_config.yaml` & `gen3utils-0.9.3/gen3utils/manifest/validation_config.yaml`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/gen3utils/s3log/s3log.py` & `gen3utils-0.9.3/gen3utils/s3log/s3log.py`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/gen3utils/s3log/s3log_worker.py` & `gen3utils-0.9.3/gen3utils/s3log/s3log_worker.py`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/gen3utils/utils.py` & `gen3utils-0.9.3/gen3utils/utils.py`

 * *Files identical despite different names*

### Comparing `gen3utils-0.9.2/pyproject.toml` & `gen3utils-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gen3utils"
-version = "0.9.2"
+version = "0.9.3"
 description = "Gen3 Library Template"
 authors = ["CTDS UChicago <cdis@uchicago.edu>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/uc-cdis/gen3utils"
 include = [
   "CHANGELOG.md",
```

### Comparing `gen3utils-0.9.2/PKG-INFO` & `gen3utils-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3utils
-Version: 0.9.2
+Version: 0.9.3
 Summary: Gen3 Library Template
 Home-page: https://github.com/uc-cdis/gen3utils
 License: Apache-2.0
 Author: CTDS UChicago
 Author-email: cdis@uchicago.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

