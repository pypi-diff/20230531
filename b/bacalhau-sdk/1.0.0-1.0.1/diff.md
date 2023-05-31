# Comparing `tmp/bacalhau_sdk-1.0.0.tar.gz` & `tmp/bacalhau_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacalhau_sdk-1.0.0.tar", max compression
+gzip compressed data, was "bacalhau_sdk-1.0.1.tar", max compression
```

## Comparing `bacalhau_sdk-1.0.0.tar` & `bacalhau_sdk-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10247 2023-05-09 13:53:51.586190 bacalhau_sdk-1.0.0/LICENSE
--rw-r--r--   0        0        0     7459 2023-05-09 13:53:51.586190 bacalhau_sdk-1.0.0/README.md
--rw-r--r--   0        0        0      133 2023-05-09 13:53:51.586190 bacalhau_sdk-1.0.0/bacalhau_sdk/__init__.py
--rw-r--r--   0        0        0     3020 2023-05-09 13:53:51.586190 bacalhau_sdk-1.0.0/bacalhau_sdk/api.py
--rw-r--r--   0        0        0     5375 2023-05-09 13:53:51.586190 bacalhau_sdk-1.0.0/bacalhau_sdk/config.py
--rw-r--r--   0        0        0     2744 2023-05-09 13:54:25.089993 bacalhau_sdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-09 13:53:51.586190 bacalhau_sdk-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     6721 2023-05-09 13:53:51.586190 bacalhau_sdk-1.0.0/tests/test_config.py
--rw-r--r--   0        0        0     9314 1970-01-01 00:00:00.000000 bacalhau_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10247 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/LICENSE
+-rw-r--r--   0        0        0     7401 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/README.md
+-rw-r--r--   0        0        0      133 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/bacalhau_sdk/__init__.py
+-rw-r--r--   0        0        0     3020 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/bacalhau_sdk/api.py
+-rw-r--r--   0        0        0     5375 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/bacalhau_sdk/config.py
+-rw-r--r--   0        0        0     2748 2023-05-31 18:48:20.930849 bacalhau_sdk-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     6458 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/tests/test_config.py
+-rw-r--r--   0        0        0     9266 1970-01-01 00:00:00.000000 bacalhau_sdk-1.0.1/PKG-INFO
```

### Comparing `bacalhau_sdk-1.0.0/LICENSE` & `bacalhau_sdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-1.0.0/README.md` & `bacalhau_sdk-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -56,26 +56,25 @@
 
 from bacalhau_sdk.api import submit
 from bacalhau_sdk.config import get_client_id
 from bacalhau_apiclient.models.storage_spec import StorageSpec
 from bacalhau_apiclient.models.spec import Spec
 from bacalhau_apiclient.models.job_spec_language import JobSpecLanguage
 from bacalhau_apiclient.models.job_spec_docker import JobSpecDocker
-from bacalhau_apiclient.models.job_sharding_config import JobShardingConfig
-from bacalhau_apiclient.models.job_execution_plan import JobExecutionPlan
+from bacalhau_apiclient.models.publisher_spec import PublisherSpec
 from bacalhau_apiclient.models.deal import Deal
 
 
 data = dict(
     APIVersion='V1beta1',
     ClientID=get_client_id(),
     Spec=Spec(
         engine="Docker",
         verifier="Noop",
-        publisher="Estuary",
+        publisher_spec=PublisherSpec(type="Estuary"),
         docker=JobSpecDocker(
             image="ubuntu",
             entrypoint=["echo", "Hello World!"],
         ),
         language=JobSpecLanguage(job_context=None),
         wasm=None,
         resources=None,
```

### Comparing `bacalhau_sdk-1.0.0/bacalhau_sdk/api.py` & `bacalhau_sdk-1.0.1/bacalhau_sdk/api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-1.0.0/bacalhau_sdk/config.py` & `bacalhau_sdk-1.0.1/bacalhau_sdk/config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-1.0.0/pyproject.toml` & `bacalhau_sdk-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "bacalhau-sdk"
-version = "1.0.0"
+version = "1.0.1"
 homepage = "https://github.com/bacalhau-project/bacalhau/"
 repository = "https://github.com/bacalhau-project/bacalhau/"
 documentation = "https://docs.bacalhau.org/"
 keywords = ["bacalhau", "Filecoin", "IPFS", "cod", "compute over data", "verifiable computation"]
 description = "Compute over Data framework for public, transparent, and optionally verifiable computation using IPFS & Filecoin."
 authors = ["Enrico Rotundo <team@bacalhau.org>"]
 readme = "README.md"
@@ -38,15 +38,15 @@
 pre-commit = {version = "^2.12.0", optional = true}
 toml = {version = "^0.10.2", optional = true}
 pem = "^21.2.0"
 pycryptodome = "^3.16.0"
 cryptography = "^39.0.1"
 six = "^1.16.0"
 types-six = "^1.16.21.4"
-bacalhau-apiclient = "*"
+bacalhau-apiclient = "1.0.0"
 
 [tool.poetry.extras]
 
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.2.6"
 pre-commit = "^2.21.0"
```

### Comparing `bacalhau_sdk-1.0.0/tests/test_config.py` & `bacalhau_sdk-1.0.1/tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,18 +114,17 @@
 def test_sign_for_client():
     """Test sign_for_client()."""
     import base64
     import json
 
     from bacalhau_apiclient.api import job_api
     from bacalhau_apiclient.models.deal import Deal
-    from bacalhau_apiclient.models.job_execution_plan import JobExecutionPlan
-    from bacalhau_apiclient.models.job_sharding_config import JobShardingConfig
     from bacalhau_apiclient.models.job_spec_docker import JobSpecDocker
     from bacalhau_apiclient.models.job_spec_language import JobSpecLanguage
+    from bacalhau_apiclient.models.publisher_spec import PublisherSpec
     from bacalhau_apiclient.models.spec import Spec
     from bacalhau_apiclient.models.storage_spec import StorageSpec
     from Crypto.Hash import SHA256
     from Crypto.Signature import pkcs1_15
 
     from bacalhau_sdk.config import get_client_id, get_user_id_key, init_config, sign_for_client
 
@@ -133,15 +132,15 @@
 
     test_payload = dict(
         api_version="V1beta1",
         client_id=get_client_id(),
         spec=Spec(
             engine="Docker",
             verifier="Noop",
-            publisher="Estuary",
+            publisher=PublisherSpec(type="Estuary"),
             docker=JobSpecDocker(
                 image="ubuntu",
                 entrypoint=["date"],
             ),
             language=JobSpecLanguage(job_context=None),
             wasm=None,
             resources=None,
@@ -149,19 +148,14 @@
             outputs=[
                 StorageSpec(
                     storage_source="IPFS",
                     name="outputs",
                     path="/outputs",
                 )
             ],
-            sharding=JobShardingConfig(
-                batch_size=1,
-                glob_pattern_base_path="/inputs",
-            ),
-            execution_plan=JobExecutionPlan(shards_total=0),
             deal=Deal(concurrency=1, confidence=0, min_bids=0),
             do_not_track=False,
         ),
     )
 
     client = job_api.ApiClient()
     sanitized_data = client.sanitize_for_serialization(test_payload)
```

### Comparing `bacalhau_sdk-1.0.0/PKG-INFO` & `bacalhau_sdk-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacalhau-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Compute over Data framework for public, transparent, and optionally verifiable computation using IPFS & Filecoin.
 Home-page: https://github.com/bacalhau-project/bacalhau/
 License: Apache-2.0
 Keywords: bacalhau,Filecoin,IPFS,cod,compute over data,verifiable computation
 Author: Enrico Rotundo
 Author-email: team@bacalhau.org
 Requires-Python: >=3.8.1,<3.12
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: bacalhau-apiclient
+Requires-Dist: bacalhau-apiclient (==1.0.0)
 Requires-Dist: black (>=22.12.0,<23.0.0)
 Requires-Dist: cryptography (>=39.0.1,<40.0.0)
 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: isort (>=5.8.0,<6.0.0)
 Requires-Dist: mypy (>=0.991,<0.992)
 Requires-Dist: pem (>=21.2.0,<22.0.0)
 Requires-Dist: pip (>=22.3.1,<23.0.0)
@@ -98,26 +98,25 @@
 
 from bacalhau_sdk.api import submit
 from bacalhau_sdk.config import get_client_id
 from bacalhau_apiclient.models.storage_spec import StorageSpec
 from bacalhau_apiclient.models.spec import Spec
 from bacalhau_apiclient.models.job_spec_language import JobSpecLanguage
 from bacalhau_apiclient.models.job_spec_docker import JobSpecDocker
-from bacalhau_apiclient.models.job_sharding_config import JobShardingConfig
-from bacalhau_apiclient.models.job_execution_plan import JobExecutionPlan
+from bacalhau_apiclient.models.publisher_spec import PublisherSpec
 from bacalhau_apiclient.models.deal import Deal
 
 
 data = dict(
     APIVersion='V1beta1',
     ClientID=get_client_id(),
     Spec=Spec(
         engine="Docker",
         verifier="Noop",
-        publisher="Estuary",
+        publisher_spec=PublisherSpec(type="Estuary"),
         docker=JobSpecDocker(
             image="ubuntu",
             entrypoint=["echo", "Hello World!"],
         ),
         language=JobSpecLanguage(job_context=None),
         wasm=None,
         resources=None,
```

