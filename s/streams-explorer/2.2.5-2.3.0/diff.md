# Comparing `tmp/streams_explorer-2.2.5.tar.gz` & `tmp/streams_explorer-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streams_explorer-2.2.5.tar", max compression
+gzip compressed data, was "streams_explorer-2.3.0.tar", max compression
```

## Comparing `streams_explorer-2.2.5.tar` & `streams_explorer-2.3.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0    12340 2023-02-20 11:22:05.830173 streams_explorer-2.2.5/README.md
--rw-r--r--   0        0        0     1631 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/pyproject.toml
--rw-r--r--   0        0        0      102 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/api/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/api/dependencies/__init__.py
--rw-r--r--   0        0        0      217 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/api/dependencies/dataflow_graph.py
--rw-r--r--   0        0        0     1080 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/api/dependencies/streams_explorer.py
--rw-r--r--   0        0        0        0 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/api/routes/__init__.py
--rw-r--r--   0        0        0      525 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/api/routes/api.py
--rw-r--r--   0        0        0     1785 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/api/routes/graph.py
--rw-r--r--   0        0        0      161 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/api/routes/kubernetes_health.py
--rw-r--r--   0        0        0      449 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/api/routes/metrics.py
--rw-r--r--   0        0        0     1501 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/api/routes/node.py
--rw-r--r--   0        0        0      471 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/api/routes/pipelines.py
--rw-r--r--   0        0        0      427 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/api/routes/update.py
--rw-r--r--   0        0        0      400 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/application.py
--rw-r--r--   0        0        0        0 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/__init__.py
--rw-r--r--   0        0        0     1129 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/client_manager.py
--rw-r--r--   0        0        0     3528 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/config.py
--rw-r--r--   0        0        0        0 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/extractor/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/extractor/default/__init__.py
--rw-r--r--   0        0        0     1087 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/extractor/default/elasticsearch_sink.py
--rw-r--r--   0        0        0     1149 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/extractor/default/generic.py
--rw-r--r--   0        0        0      987 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/extractor/default/jdbc_sink.py
--rw-r--r--   0        0        0     1070 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/extractor/default/redis_sink.py
--rw-r--r--   0        0        0      981 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/extractor/default/s3_sink.py
--rw-r--r--   0        0        0     1013 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/extractor/default/streams_bootstrap_producer.py
--rw-r--r--   0        0        0     2107 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/extractor/default/transformer.py
--rw-r--r--   0        0        0     1453 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/extractor/extractor.py
--rw-r--r--   0        0        0     3150 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/extractor/extractor_container.py
--rw-r--r--   0        0        0     7760 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/k8s_app.py
--rw-r--r--   0        0        0     4444 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/k8s_config_parser.py
--rw-r--r--   0        0        0     2041 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/node_info_extractor.py
--rw-r--r--   0        0        0        0 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/services/__init__.py
--rw-r--r--   0        0        0    14081 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/services/dataflow_graph.py
--rw-r--r--   0        0        0     2040 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/services/kafka_admin_client.py
--rw-r--r--   0        0        0     2901 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/services/kafkaconnect.py
--rw-r--r--   0        0        0     6768 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/services/kubernetes.py
--rw-r--r--   0        0        0     2817 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/services/linking_services.py
--rw-r--r--   0        0        0     6820 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/services/metric_providers.py
--rw-r--r--   0        0        0     1755 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/core/services/schemaregistry.py
--rw-r--r--   0        0        0      725 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/default.py
--rw-r--r--   0        0        0     4944 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/defaultlinker.py
--rw-r--r--   0        0        0     1217 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/extractors.py
--rw-r--r--   0        0        0      500 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/k8s_config_parser.py
--rw-r--r--   0        0        0      501 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/linker.py
--rw-r--r--   0        0        0      527 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/metric_provider.py
--rw-r--r--   0        0        0        0 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/models/__init__.py
--rw-r--r--   0        0        0     1149 2023-02-20 11:22:05.834173 streams_explorer-2.2.5/streams_explorer/models/graph.py
--rw-r--r--   0        0        0     1571 2023-02-20 11:22:05.838173 streams_explorer-2.2.5/streams_explorer/models/k8s.py
--rw-r--r--   0        0        0     3873 2023-02-20 11:22:05.838173 streams_explorer-2.2.5/streams_explorer/models/kafka_connector.py
--rw-r--r--   0        0        0      427 2023-02-20 11:22:05.838173 streams_explorer-2.2.5/streams_explorer/models/node_information.py
--rw-r--r--   0        0        0      204 2023-02-20 11:22:05.838173 streams_explorer-2.2.5/streams_explorer/models/node_types.py
--rw-r--r--   0        0        0       86 2023-02-20 11:22:05.838173 streams_explorer-2.2.5/streams_explorer/models/pipelines.py
--rw-r--r--   0        0        0      117 2023-02-20 11:22:05.838173 streams_explorer-2.2.5/streams_explorer/models/sink.py
--rw-r--r--   0        0        0      121 2023-02-20 11:22:05.838173 streams_explorer-2.2.5/streams_explorer/models/source.py
--rw-r--r--   0        0        0     1913 2023-02-20 11:22:05.838173 streams_explorer-2.2.5/streams_explorer/plugins.py
--rw-r--r--   0        0        0       82 2023-02-20 11:22:05.838173 streams_explorer-2.2.5/streams_explorer/py.typed
--rw-r--r--   0        0        0     9682 2023-02-20 11:22:05.838173 streams_explorer-2.2.5/streams_explorer/streams_explorer.py
--rw-r--r--   0        0        0    14001 1970-01-01 00:00:00.000000 streams_explorer-2.2.5/setup.py
--rw-r--r--   0        0        0    14026 1970-01-01 00:00:00.000000 streams_explorer-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0    12340 2023-05-31 12:03:07.423954 streams_explorer-2.3.0/README.md
+-rw-r--r--   0        0        0     1631 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/api/dependencies/__init__.py
+-rw-r--r--   0        0        0      217 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/api/dependencies/dataflow_graph.py
+-rw-r--r--   0        0        0     1080 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/api/dependencies/streams_explorer.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/api/routes/__init__.py
+-rw-r--r--   0        0        0      525 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/api/routes/api.py
+-rw-r--r--   0        0        0     1785 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/api/routes/graph.py
+-rw-r--r--   0        0        0      161 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/api/routes/kubernetes_health.py
+-rw-r--r--   0        0        0      449 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/api/routes/metrics.py
+-rw-r--r--   0        0        0     1501 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/api/routes/node.py
+-rw-r--r--   0        0        0      471 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/api/routes/pipelines.py
+-rw-r--r--   0        0        0      427 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/api/routes/update.py
+-rw-r--r--   0        0        0      400 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/application.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/client_manager.py
+-rw-r--r--   0        0        0     3528 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/config.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/extractor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/extractor/default/__init__.py
+-rw-r--r--   0        0        0     1087 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/extractor/default/elasticsearch_sink.py
+-rw-r--r--   0        0        0     1149 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/extractor/default/generic.py
+-rw-r--r--   0        0        0      987 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/extractor/default/jdbc_sink.py
+-rw-r--r--   0        0        0     1070 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/extractor/default/redis_sink.py
+-rw-r--r--   0        0        0      981 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/extractor/default/s3_sink.py
+-rw-r--r--   0        0        0     1013 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/extractor/default/streams_bootstrap_producer.py
+-rw-r--r--   0        0        0     2107 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/extractor/default/transformer.py
+-rw-r--r--   0        0        0     1453 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/extractor/extractor.py
+-rw-r--r--   0        0        0     3150 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/extractor/extractor_container.py
+-rw-r--r--   0        0        0     7760 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/k8s_app.py
+-rw-r--r--   0        0        0     4593 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/k8s_config_parser.py
+-rw-r--r--   0        0        0     2041 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/node_info_extractor.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/services/__init__.py
+-rw-r--r--   0        0        0    14172 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/services/dataflow_graph.py
+-rw-r--r--   0        0        0     2040 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/services/kafka_admin_client.py
+-rw-r--r--   0        0        0     2901 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/services/kafkaconnect.py
+-rw-r--r--   0        0        0     7912 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/services/kubernetes.py
+-rw-r--r--   0        0        0     2817 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/services/linking_services.py
+-rw-r--r--   0        0        0     6820 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/services/metric_providers.py
+-rw-r--r--   0        0        0     1755 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/core/services/schemaregistry.py
+-rw-r--r--   0        0        0      725 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/default.py
+-rw-r--r--   0        0        0     4944 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/defaultlinker.py
+-rw-r--r--   0        0        0     1217 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/extractors.py
+-rw-r--r--   0        0        0      500 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/k8s_config_parser.py
+-rw-r--r--   0        0        0      501 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/linker.py
+-rw-r--r--   0        0        0      527 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/metric_provider.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/models/__init__.py
+-rw-r--r--   0        0        0     1149 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/models/graph.py
+-rw-r--r--   0        0        0     1571 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/models/k8s.py
+-rw-r--r--   0        0        0     3873 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/models/kafka_connector.py
+-rw-r--r--   0        0        0      427 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/models/node_information.py
+-rw-r--r--   0        0        0      204 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/models/node_types.py
+-rw-r--r--   0        0        0       86 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/models/pipelines.py
+-rw-r--r--   0        0        0      117 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/models/sink.py
+-rw-r--r--   0        0        0      121 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/models/source.py
+-rw-r--r--   0        0        0     1913 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/plugins.py
+-rw-r--r--   0        0        0       82 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/py.typed
+-rw-r--r--   0        0        0     9405 2023-05-31 12:03:07.427954 streams_explorer-2.3.0/streams_explorer/streams_explorer.py
+-rw-r--r--   0        0        0    14001 1970-01-01 00:00:00.000000 streams_explorer-2.3.0/setup.py
+-rw-r--r--   0        0        0    14026 1970-01-01 00:00:00.000000 streams_explorer-2.3.0/PKG-INFO
```

### Comparing `streams_explorer-2.2.5/README.md` & `streams_explorer-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/pyproject.toml` & `streams_explorer-2.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streams-explorer"
-version = "2.2.5"
+version = "2.3.0"
 description = "Explore Data Pipelines in Apache Kafka."
 readme = "README.md"
 authors = ["bakdata"]
 repository = "https://github.com/bakdata/streams-explorer"
 license = "MIT"
 keywords = ["kafka", "kubernetes", "stream-processing", "monitoring", "pipelines"]
 classifiers = [
```

### Comparing `streams_explorer-2.2.5/streams_explorer/api/dependencies/streams_explorer.py` & `streams_explorer-2.3.0/streams_explorer/api/dependencies/streams_explorer.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/api/routes/api.py` & `streams_explorer-2.3.0/streams_explorer/api/routes/api.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/api/routes/graph.py` & `streams_explorer-2.3.0/streams_explorer/api/routes/graph.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/api/routes/node.py` & `streams_explorer-2.3.0/streams_explorer/api/routes/node.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/client_manager.py` & `streams_explorer-2.3.0/streams_explorer/core/client_manager.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/config.py` & `streams_explorer-2.3.0/streams_explorer/core/config.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/extractor/default/elasticsearch_sink.py` & `streams_explorer-2.3.0/streams_explorer/core/extractor/default/elasticsearch_sink.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/extractor/default/generic.py` & `streams_explorer-2.3.0/streams_explorer/core/extractor/default/generic.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/extractor/default/jdbc_sink.py` & `streams_explorer-2.3.0/streams_explorer/core/extractor/default/jdbc_sink.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/extractor/default/redis_sink.py` & `streams_explorer-2.3.0/streams_explorer/core/extractor/default/redis_sink.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/extractor/default/s3_sink.py` & `streams_explorer-2.3.0/streams_explorer/core/extractor/default/s3_sink.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/extractor/default/streams_bootstrap_producer.py` & `streams_explorer-2.3.0/streams_explorer/core/extractor/default/streams_bootstrap_producer.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/extractor/default/transformer.py` & `streams_explorer-2.3.0/streams_explorer/core/extractor/default/transformer.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/extractor/extractor.py` & `streams_explorer-2.3.0/streams_explorer/core/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/extractor/extractor_container.py` & `streams_explorer-2.3.0/streams_explorer/core/extractor/extractor_container.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/k8s_app.py` & `streams_explorer-2.3.0/streams_explorer/core/k8s_app.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/k8s_config_parser.py` & `streams_explorer-2.3.0/streams_explorer/core/k8s_config_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,35 +18,37 @@
     def __init__(self, k8s_app: K8sApp) -> None:
         self.k8s_app = k8s_app
 
     @abstractmethod
     def parse(self) -> K8sConfig:
         ...
 
+    @staticmethod
+    def namespace(name: str, namespace: str | None = None) -> str:
+        return f"{namespace or 'default'}/{name}"
+
 
 class StreamsBootstrapConfigParser(K8sConfigParser):
     """Config parser for deployments configured through streams-bootstrap."""
 
     def __init__(self, k8s_app: K8sApp) -> None:
         super().__init__(k8s_app)
-        self._id = self.get_id()
-        self.config = K8sConfig(self._id, name=self.get_name())
+        self.set_id()
+        self.config = K8sConfig(self._id, self._name)
 
-    def get_id(self) -> str:
+    def set_id(self) -> None:
         name: str | None = None
         if self.k8s_app.metadata.labels:
             name = self.k8s_app.metadata.labels.get("app")
         if not name:
             name = self.k8s_app.metadata.name
         if not name:
             raise TypeError(f"Name is required for {self.k8s_app.class_name}")
-        return name
-
-    def get_name(self) -> str:
-        return self._id
+        self._id: str = self.namespace(name, self.k8s_app.metadata.namespace)
+        self._name: str = name
 
     def parse_config(self, name: str, value: str) -> None:
         match name:
             case "INPUT_TOPICS":
                 self.config.input_topics = self.parse_input_topics(value)
             case "OUTPUT_TOPIC":
                 self.config.output_topic = value
```

### Comparing `streams_explorer-2.2.5/streams_explorer/core/node_info_extractor.py` & `streams_explorer-2.3.0/streams_explorer/core/node_info_extractor.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/services/dataflow_graph.py` & `streams_explorer-2.3.0/streams_explorer/core/services/dataflow_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         self._add_streaming_app(self.graph, app)
         if pipeline:
             self._add_streaming_app(
                 self.pipelines.setdefault(pipeline, nx.DiGraph()), app
             )
 
     def _add_streaming_app(self, graph: nx.DiGraph, app: K8sApp) -> None:
+        if graph.has_node(app.id):
+            raise ValueError(f"Duplicate app {app.id}")
         graph.add_node(
             app.id,
             label=app.name,
             node_type=NodeTypesEnum.STREAMING_APP,
             **app.attributes,
         )
```

### Comparing `streams_explorer-2.2.5/streams_explorer/core/services/kafka_admin_client.py` & `streams_explorer-2.3.0/streams_explorer/core/services/kafka_admin_client.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/services/kafkaconnect.py` & `streams_explorer-2.3.0/streams_explorer/core/services/kafkaconnect.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/services/linking_services.py` & `streams_explorer-2.3.0/streams_explorer/core/services/linking_services.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/services/metric_providers.py` & `streams_explorer-2.3.0/streams_explorer/core/services/metric_providers.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/core/services/schemaregistry.py` & `streams_explorer-2.3.0/streams_explorer/core/services/schemaregistry.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/default.py` & `streams_explorer-2.3.0/streams_explorer/default.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/defaultlinker.py` & `streams_explorer-2.3.0/streams_explorer/defaultlinker.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/extractors.py` & `streams_explorer-2.3.0/streams_explorer/extractors.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/metric_provider.py` & `streams_explorer-2.3.0/streams_explorer/metric_provider.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/models/graph.py` & `streams_explorer-2.3.0/streams_explorer/models/graph.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/models/k8s.py` & `streams_explorer-2.3.0/streams_explorer/models/k8s.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/models/kafka_connector.py` & `streams_explorer-2.3.0/streams_explorer/models/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/plugins.py` & `streams_explorer-2.3.0/streams_explorer/plugins.py`

 * *Files identical despite different names*

### Comparing `streams_explorer-2.2.5/streams_explorer/streams_explorer.py` & `streams_explorer-2.3.0/streams_explorer/streams_explorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import re
-
 from cachetools.func import ttl_cache
 from fastapi import WebSocket
 from kubernetes_asyncio.client import V1beta1CronJob, V1Job
 from loguru import logger
 
 from streams_explorer.core.client_manager import ClientManager
 from streams_explorer.core.config import settings
@@ -21,15 +19,15 @@
     K8sEvent,
     Kubernetes,
 )
 from streams_explorer.core.services.linking_services import LinkingService
 from streams_explorer.core.services.metric_providers import MetricProvider
 from streams_explorer.extractors import extractor_container
 from streams_explorer.models.graph import Metric
-from streams_explorer.models.k8s import K8sDeploymentUpdateType, K8sReason
+from streams_explorer.models.k8s import K8sDeploymentUpdateType
 from streams_explorer.models.kafka_connector import KafkaConnector
 from streams_explorer.models.node_information import (
     NodeInfoListItem,
     NodeInformation,
     NodeInfoType,
 )
 
@@ -171,34 +169,28 @@
     ) -> None:
         match type:
             case K8sDeploymentUpdateType.ADDED | K8sDeploymentUpdateType.MODIFIED:
                 await self.__add_app(app)
             case K8sDeploymentUpdateType.DELETED:
                 self.__remove_app(app)
 
-    async def handle_event(self, raw_event: K8sEvent) -> None:
-        event = raw_event["object"]
-
-        # extract deployment name from pod
-        if not event.reason or not event.regarding or not event.regarding.field_path:
+    async def handle_event(self, event: K8sEvent) -> None:
+        logger.trace(event)
+        if not event.is_valid:
             return
-        name = re.findall(r"{(.+?)}", event.regarding.field_path)[0]
-
-        logger.info(
-            "{} {} {} ({})",
-            event.regarding.namespace,
-            name,
-            event.reason,
+        logger.debug(
+            "{} {} ({})",
+            event.id,
+            event.object.reason,
             event.type,
         )
-        logger.debug(event)
 
         # map event to application
-        if app := self.applications.get(name):
-            app.state = K8sReason.from_str(event.reason)
+        if app := self.applications.get(event.id):
+            app.state = event.reason
             # app.note = event["note"] # TODO
             await self._update_clients_delta(app)
 
     def update_connectors(self) -> None:
         extractor_container.reset_connectors()
         logger.info("Retrieve Kafka connectors")
         self.kafka_connectors = KafkaConnect.connectors()
```

### Comparing `streams_explorer-2.2.5/setup.py` & `streams_explorer-2.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'uvicorn[standard]>=0.20.0,<0.21.0']
 
 entry_points = \
 {'console_scripts': ['start = main:start']}
 
 setup_kwargs = {
     'name': 'streams-explorer',
-    'version': '2.2.5',
+    'version': '2.3.0',
     'description': 'Explore Data Pipelines in Apache Kafka.',
     'long_description': '# Streams Explorer\n\n> Explore Apache Kafka data pipelines in Kubernetes.\n\n![streams-explorer](https://github.com/bakdata/streams-explorer/blob/main/screens/overview.png?raw=true)\n\n> **Note**\n> We are participating in the annual Hacktoberfest. If you\'re looking to contribute, please see our [open issues](https://github.com/bakdata/streams-explorer/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc+label%3Ahacktoberfest) and use the [standalone installation](#standalone) for development.\n\n## Contents\n\n- [Streams Explorer](#streams-explorer)\n  - [Features](#features)\n  - [Overview](#overview)\n  - [Installation](#installation)\n    - [Docker Compose](#docker-compose)\n    - [Deploying to Kubernetes cluster](#deploying-to-kubernetes-cluster)\n    - [Standalone](#standalone)\n      - [Backend](#backend)\n      - [Frontend](#frontend)\n  - [Configuration](#configuration)\n    - [Kafka](#kafka)\n    - [Kafka Connect](#kafka-connect)\n    - [Kubernetes](#kubernetes)\n    - [Schema Registry / Karapace](#schema-registry--karapace)\n    - [Prometheus](#prometheus)\n    - [AKHQ](#akhq)\n    - [Redpanda Console](#redpanda-console)\n    - [Grafana](#grafana)\n    - [Kibana](#kibana)\n    - [Elasticsearch](#elasticsearch)\n    - [Plugins](#plugins)\n  - [Demo pipeline](#demo-pipeline)\n  - [Plugin customization](#plugin-customization)\n\n## Features\n\n- Visualization of streaming applications, topics, and connectors\n- Monitor all or individual pipelines from multiple namespaces\n- Inspection of Avro schema from schema registry\n- Integration with [streams-bootstrap](https://github.com/bakdata/streams-bootstrap) and [faust-bootstrap](https://github.com/bakdata/faust-bootstrap), or custom streaming app config parsing from Kubernetes deployments using plugins\n- Real-time metrics from Prometheus (consumer lag & read rate, replicas, topic size, messages in & out per second, connector tasks)\n- Linking to external services for logging and analysis, such as Kibana, Grafana, Loki, AKHQ, Redpanda Console, and Elasticsearch\n- Customizable through Python plugins\n\n## Overview\n\nVisit our introduction [blogpost](https://medium.com/bakdata/exploring-data-pipelines-in-apache-kafka-with-streams-explorer-8337dd11fdad) for a complete overview and demo of Streams Explorer.\n\n## Installation\n\n> **Prerequisites**\n> Access to a Kubernetes cluster, where streaming apps and services are deployed.\n\n### Docker Compose\n\n1. Forward the ports to Prometheus. (Kafka Connect, Schema Registry, and other integrations are optional)\n2. Start the container\n\n```sh\ndocker compose up\n```\n\nOnce the container is started visit <http://localhost:8080>\n\n### Deploying to Kubernetes cluster\n\n1. Add the Helm chart repository\n\n```sh\nhelm repo add streams-explorer https://bakdata.github.io/streams-explorer\n```\n\n2. Install\n\n```sh\nhelm upgrade --install --values helm-chart/values.yaml streams-explorer streams-explorer/streams-explorer\n```\n\n### Standalone\n\n#### Backend\n\n1. Install dependencies using [Poetry](https://python-poetry.org)\n\n```sh\npoetry install\n```\n\n2. Forward the ports to Prometheus. (Kafka Connect, Schema Registry, and other integrations are optional)\n3. Configure the backend in [settings.yaml](backend/settings.yaml).\n4. Start the backend server\n\n```sh\npoetry run start\n```\n\n#### Frontend\n\n1. Install dependencies\n\n```sh\nnpm ci\n```\n\n2. Start the frontend server\n\n```sh\nnpm run build && npm run prod\n```\n\nVisit <http://localhost:3000>\n\n## Configuration\n\nDepending on your type of installation set the configuration for the backend server in this file:\n\n- **Docker Compose**: [docker-compose.yaml](docker-compose.yaml)\n- **Kubernetes**: [helm-chart/values.yaml](helm-chart/values.yaml)\n- **standalone**: [backend/settings.yaml](backend/settings.yaml)\n\nIn the [helm-chart/values.yaml](helm-chart/values.yaml) configuration is done either through the `config` section using double underscore notation, e.g. `K8S__consumer_group_annotation: consumerGroup` or the content of [backend/settings.yaml](backend/settings.yaml) can be pasted under the `settings` section. Alternatively all configuration options can be written as environment variables using double underscore notation and the prefix `SE`, e.g. `SE_K8S__deployment__cluster=false`.\n\nThe following configuration options are available:\n\n#### General\n\n- `graph.update_interval` Render the graph every x seconds (int, **required**, default: `30`)\n- `graph.layout_arguments` Arguments passed to graphviz layout (string, **required**, default: `-Grankdir=LR -Gnodesep=0.8 -Gpad=10`)\n- `graph.pipeline_distance` Increase/decrease vertical space between pipeline graphs by X pixels (int, **required**, default: `500`)\n- `graph.resolve.input_pattern_topics.all` If true topics that match (extra) input pattern(s) are connected to the streaming app in the graph containing all pipelines (bool, **required**, default: `false`)\n- `graph.resolve.input_pattern_topics.pipelines` If true topics that match (extra) input pattern(s) are connected to the streaming app in pipeline graphs (bool, **required**, default: `false`)\n\n#### Kafka\n\n- `kafka.enable` Enable Kafka (bool, default: `false`)\n- `kafka.config` librdkafka configuration properties ([reference](https://github.com/edenhill/librdkafka/blob/master/CONFIGURATION.md)) (dict, default: `{"bootstrap.servers": "localhost:9092"}`)\n- `kafka.displayed_information` Configuration options of Kafka topics displayed in the frontend (list of dict)\n- `kafka.topic_names_cache.ttl` Cache for retrieving all topic names (used when input topic patterns are resolved) (int, default: `3600`)\n\n#### Kafka Connect\n\n- `kafkaconnect.url` URL of Kafka Connect server (string, default: None)\n- `kafkaconnect.update_interval` Fetch connectors every x seconds (int, default: `300`)\n- `kafkaconnect.displayed_information` Configuration options of Kafka connectors displayed in the frontend (list of dict)\n\n#### Kubernetes\n\n- `k8s.deployment.cluster` Whether streams-explorer is deployed to Kubernetes cluster (bool, **required**, default: `false`)\n- `k8s.deployment.context` Name of cluster (string, optional if running in cluster, default: `kubernetes-cluster`)\n- `k8s.deployment.namespaces` Kubernetes namespaces (list of string, **required**, default: `[\'kubernetes-namespace\']`)\n- `k8s.containers.ignore` Name of containers that should be ignored/hidden (list of string, default: `[\'prometheus-jmx-exporter\']`)\n- `k8s.displayed_information` Details of pod that should be displayed (list of dict, default: `[{\'name\': \'Labels\', \'key\': \'metadata.labels\'}]`)\n- `k8s.labels` Labels used to set attributes of nodes (list of string, **required**, default: `[\'pipeline\']`)\n- `k8s.pipeline.label` Attribute of nodes the pipeline name should be extracted from (string, **required**, default: `pipeline`)\n- `k8s.consumer_group_annotation` Annotation the consumer group name should be extracted from (string, **required**, default: `consumerGroup`)\n\n#### Schema Registry / Karapace\n\n- `schemaregistry.url` URL of Confluent Schema Registry or Karapace (string, default: None)\n\n#### Prometheus\n\n- `prometheus.url` URL of Prometheus (string, **required**, default: `http://localhost:9090`)\n\nThe following exporters are required to collect Kafka metrics for Prometheus:\n\n- [Kafka Exporter](https://github.com/danielqsj/kafka_exporter)\n- [Kafka Lag Exporter](https://github.com/lightbend/kafka-lag-exporter)\n- [Kafka Connect Exporter](https://github.com/wakeful/kafka_connect_exporter)\n\n#### AKHQ\n\n- `akhq.enable` Enable AKHQ (bool, default: `false`)\n- `akhq.url` URL of AKHQ (string, default: `http://localhost:8080`)\n- `akhq.cluster` Name of cluster (string, default: `kubernetes-cluster`)\n- `akhq.connect` Name of connect (string, default: None)\n\n#### Redpanda Console\n\nRedpanda Console can be used instead of AKHQ. (mutually exclusive)\n\n- `redpanda_console.enable` Enable Redpanda Console (bool, default: `false`)\n- `redpanda_console.url` URL of Redpanda Console (string, default: `http://localhost:8080`)\n\n#### Grafana\n\n- `grafana.enable` Enable Grafana (bool, default: `false`)\n- `grafana.url` URL of Grafana (string, default: `http://localhost:3000`)\n- `grafana.dashboards.topics` Path to topics dashboard (string), sample dashboards for topics and consumer groups are included in the [`./grafana`](https://github.com/bakdata/streams-explorer/tree/main/grafana) subfolder\n- `grafana.dashboards.consumergroups` Path to consumer groups dashboard (string)\n\n#### Kibana\n\n- `kibanalogs.enable` Enable Kibana logs (bool, default: `false`)\n- `kibanalogs.url` URL of Kibana logs (string, default: `http://localhost:5601`)\n\n#### Loki\n\nLoki can be used instead of Kibana. (mutually exclusive)\n\n- `loki.enable` Enable Loki logs (bool, default: `false`)\n- `loki.url` URL of Loki logs (string, default: `http://localhost:3000`)\n\n#### Elasticsearch\n\nfor Kafka Connect Elasticsearch connector\n\n- `esindex.url` URL of Elasticsearch index (string, default: `http://localhost:5601/app/kibana#/dev_tools/console`)\n\n#### Plugins\n\n- `plugins.path` Path to folder containing plugins relative to backend (string, **required**, default: `./plugins`)\n- `plugins.extractors.default` Whether to load default extractors (bool, **required**, default: `true`)\n\n## Demo pipeline\n\n![demo-pipeline](https://github.com/bakdata/streams-explorer/blob/main/screens/demo-pipeline.png?raw=true)\n\n[ATM Fraud detection with streams-bootstrap](https://github.com/bakdata/streams-explorer/blob/main/demo-atm-fraud/README.md)\n\n## Plugin customization\n\nIt is possible to create your own config parser, linker, metric provider, and extractors in Python by implementing the `K8sConfigParser`, `LinkingService`, `MetricProvider`, or `Extractor` classes. This way you can customize it to your specific setup and services. As an example we provide the [`DefaultLinker`](https://github.com/bakdata/streams-explorer/blob/main/backend/streams_explorer/defaultlinker.py) as `LinkingService`. The default [`MetricProvider`](https://github.com/bakdata/streams-explorer/blob/main/backend/streams_explorer/core/services/metric_providers.py) supports Prometheus. Furthermore the following default `Extractor` plugins are included:\n\n- [`ElasticsearchSink`](https://github.com/bakdata/streams-explorer/blob/main/backend/streams_explorer/core/extractor/default/elasticsearch_sink.py)\n- [`JdbcSink`](https://github.com/bakdata/streams-explorer/blob/main/backend/streams_explorer/core/extractor/default/jdbc_sink.py)\n- [`S3Sink`](https://github.com/bakdata/streams-explorer/blob/main/backend/streams_explorer/core/extractor/default/s3_sink.py)\n- [`GenericSink`/`GenericSource`](https://github.com/bakdata/streams-explorer/blob/main/backend/streams_explorer/core/extractor/default/generic.py)\n\nIf your streaming application deployments are configured through environment variables, following the schema of [streams-bootstrap](https://github.com/bakdata/streams-bootstrap) or [faust-bootstrap](https://github.com/bakdata/faust-bootstrap), the Streams Explorer works out-of-the-box with the default deployment parser.\nFor streams-bootstrap deployments configured through CLI arguments a separate parser can be loaded by creating a Python file (e.g. `config_parser.py`) in the plugins folder with the following import statement:\n\n```python\nfrom streams_explorer.core.k8s_config_parser import StreamsBootstrapArgsParser\n```\n\nFor other setups a custom config parser plugin can be created by inheriting from the [`K8sConfigParser`](https://github.com/bakdata/streams-explorer/blob/main/backend/streams_explorer/core/k8s_config_parser.py) class and implementing the `parse` method. In this example we\'re retrieving the streaming app configurations from an external REST API. In order for a deployment to be indentified as streaming app, input and output topics are required.\n\n```python\nimport httpx\n\nfrom streams_explorer.core.k8s_config_parser import K8sConfigParser\nfrom streams_explorer.models.k8s import K8sConfig\n\n\nclass CustomConfigParser(K8sConfigParser):\n    def get_name(self) -> str:\n        name = self.k8s_app.metadata.name\n        if not name:\n            raise TypeError(f"Name is required for {self.k8s_app.class_name}")\n        return name\n\n    def parse(self) -> K8sConfig:\n        """Retrieve app config from REST endpoint."""\n        name = self.get_name()\n        data = httpx.get(f"url/config/{name}").json()\n        return K8sConfig(**data)\n```\n',
     'author': 'bakdata',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bakdata/streams-explorer',
```

### Comparing `streams_explorer-2.2.5/PKG-INFO` & `streams_explorer-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streams-explorer
-Version: 2.2.5
+Version: 2.3.0
 Summary: Explore Data Pipelines in Apache Kafka.
 Home-page: https://github.com/bakdata/streams-explorer
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,monitoring,pipelines
 Author: bakdata
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

