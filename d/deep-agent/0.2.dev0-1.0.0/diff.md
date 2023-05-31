# Comparing `tmp/deep_agent-0.2.dev0.tar.gz` & `tmp/deep_agent-1.0.0.tar.gz`

## Comparing `deep_agent-0.2.dev0.tar` & `deep_agent-1.0.0.tar`

### file list

```diff
@@ -1,4 +1,39 @@
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 deep_agent-0.2.dev0/.gitignore
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 deep_agent-0.2.dev0/pyproject.toml
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 deep_agent-0.2.dev0/../../README.md
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 deep_agent-0.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/__init__.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/utils.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/version.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/__init__.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/deep.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/types.py
+-rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/attributes/__init__.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/auth/__init__.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/plugin/__init__.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/plugin/otel.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/plugin/python.py
+-rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/resource/__init__.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/tracepoint/__init__.py
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/tracepoint/eventsnapshot.py
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/api/tracepoint/tracepoint_config.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/config/__init__.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/config/config_service.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/config/tracepoint_config.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/grpc/__init__.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/grpc/grpc_service.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/logging/__init__.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/logging/logging.conf
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/poll/__init__.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/poll/poll.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/__init__.py
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/frame_collector.py
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/frame_config.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/frame_processor.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/trigger_handler.py
+-rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/variable_processor.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/processor/bfs/__init__.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/push/__init__.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/push/push_service.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 deep_agent-1.0.0/src/deep/task/__init__.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 deep_agent-1.0.0/.gitignore
+-rw-r--r--   0        0        0    34522 2020-02-02 00:00:00.000000 deep_agent-1.0.0/LICENSE
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 deep_agent-1.0.0/README.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 deep_agent-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 deep_agent-1.0.0/PKG-INFO
```

### Comparing `deep_agent-0.2.dev0/pyproject.toml` & `deep_agent-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deep-agent"
-description = "DEEP Python Protobuf"
-readme = "../../README.md"
-license = "Apache-2.0"
+description = "DEEP Python Agent"
+readme = "README.md"
+license = "AGPL-3.0-only"
 requires-python = ">3.7"
 authors = [
+    { name = "Intergral GmbH", email = "support@intergral.com" },
     { name = "Ben Donnelly", email = "b.w.donnelly1@gmail.com" }
 ]
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
-    "License :: OSI Approved :: Apache Software License",
+    "License :: OSI Approved :: GNU Affero General Public License v3",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
-dependencies = []
-version = "0.2-dev"
+dependencies = [
+    "grpcio>=1.51.3",
+    "deep-proto>=1.0.0",
+    "protobuf>=3.20.3"
+]
+dynamic = [
+    "version"
+]
 
 [tool.hatch.build.targets.sdist]
 include = [
-    "src/deep",
+    "/src",
+    "/tests",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/deep"]
+
+
+[tool.hatch.version]
+path = "src/deep/version.py"
```

### Comparing `deep_agent-0.2.dev0/PKG-INFO` & `deep_agent-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,58 @@
 Metadata-Version: 2.1
 Name: deep-agent
-Version: 0.2.dev0
-Summary: DEEP Python Protobuf
-Author-email: Ben Donnelly <b.w.donnelly1@gmail.com>
-License-Expression: Apache-2.0
-Classifier: Development Status :: 1 - Planning
+Version: 1.0.0
+Summary: DEEP Python Agent
+Author-email: Intergral GmbH <support@intergral.com>, Ben Donnelly <b.w.donnelly1@gmail.com>
+License-Expression: AGPL-3.0-only
+License-File: LICENSE
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >3.7
+Requires-Dist: deep-proto>=1.0.0
+Requires-Dist: grpcio>=1.51.3
+Requires-Dist: protobuf>=3.20.3
 Description-Content-Type: text/markdown
 
-# Language Independent Interface Types For DEEP
+[![Tests](https://github.com/intergral/deep-python-client/actions/workflows/on_push.yaml/badge.svg)](https://github.com/intergral/deep-python-client/actions/workflows/on_push.yaml)
+[![PyPI](https://img.shields.io/pypi/v/deep-agent)](https://pypi.org/project/deep-agent/)
 
-The proto files can be consumed as GIT submodules or copied and built directly in the consumer project.
+# DEEP Python Client
 
-The compiled files are published to central repositories (Maven, ...).
+DEEP is an open source dynamic insight engine based on the Grafana stack. The idea is to allow dynamic collection of
+Traces, Metrics, Logs and Snapshots via the Grafana UI.
 
-See [contribution guidelines](CONTRIBUTING.md) if you would like to make any changes.
+## Usage
 
-## Generate gRPC Client Libraries
+To use DEEP simple import the package and start the agent at the earliest point in the code.
 
-To generate the raw gRPC client libraries, use `make gen-${LANGUAGE}`. Currently supported languages are:
+```bash
+pip install deep-agent
+```
 
-* python
+```python
+import deep
+
+deep.start()
+```
+
+## Examples
+
+There are a couple of examples [available here](./examples/README.md).
+
+## Documentation
+
+For further documentation on the usage of deep-agent view the [docs](https://intergral.github.io/deep-python-client/).
+
+
+## Licensing
+
+For licensing info please see [LICENSING.md](./LICENSING.md)
```

