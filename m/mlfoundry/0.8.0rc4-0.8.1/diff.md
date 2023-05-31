# Comparing `tmp/mlfoundry-0.8.0rc4.tar.gz` & `tmp/mlfoundry-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfoundry-0.8.0rc4.tar", max compression
+gzip compressed data, was "mlfoundry-0.8.1.tar", max compression
```

## Comparing `mlfoundry-0.8.0rc4.tar` & `mlfoundry-0.8.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0     3158 2023-05-18 17:21:09.244919 mlfoundry-0.8.0rc4/README.md
--rw-r--r--   0        0        0      991 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/__main__.py
--rw-r--r--   0        0        0     3713 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/amplitude.py
--rw-r--r--   0        0        0        0 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/artifact/__init__.py
--rw-r--r--   0        0        0     7069 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/artifact/truefoundry_artifact_repo.py
--rw-r--r--   0        0        0        0 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/background/__init__.py
--rw-r--r--   0        0        0      287 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/background/events.py
--rw-r--r--   0        0        0     3032 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/background/interface.py
--rw-r--r--   0        0        0     4016 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/background/sender.py
--rw-r--r--   0        0        0     8756 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/background/system_metrics.py
--rw-r--r--   0        0        0     4028 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/background/utils.py
--rw-r--r--   0        0        0        0 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/cli/__init__.py
--rw-r--r--   0        0        0      918 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/cli/cli_interface.py
--rw-r--r--   0        0        0      100 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0      731 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/cli/commands/download.py
--rw-r--r--   0        0        0      739 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/cli/commands/login.py
--rw-r--r--   0        0        0     2724 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/constants.py
--rw-r--r--   0        0        0      103 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/dataset/__init__.py
--rw-r--r--   0        0        0     7854 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/dataset/dataset.py
--rw-r--r--   0        0        0     2255 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/dataset/schema.py
--rw-r--r--   0        0        0    13138 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/dataset/serde.py
--rw-r--r--   0        0        0     2028 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/dataset/serde_utils.py
--rw-r--r--   0        0        0     2078 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/dataset/stats.py
--rw-r--r--   0        0        0     1903 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/dataset/types.py
--rw-r--r--   0        0        0     2588 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/dataset/validation.py
--rw-r--r--   0        0        0       69 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/dataset/whylogs_types/__init__.py
--rw-r--r--   0        0        0     4025 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/dataset/whylogs_types/summary.py
--rw-r--r--   0        0        0     1392 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/enums.py
--rw-r--r--   0        0        0      325 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/env_vars.py
--rw-r--r--   0        0        0      365 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/exceptions.py
--rw-r--r--   0        0        0     2037 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/__init__.py
--rw-r--r--   0        0        0      301 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/base_registry.py
--rw-r--r--   0        0        0      718 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/fastai_registry.py
--rw-r--r--   0        0        0      892 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/gluon_registry.py
--rw-r--r--   0        0        0      700 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/h2o_registry.py
--rw-r--r--   0        0        0      712 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/keras_registry.py
--rw-r--r--   0        0        0      730 2023-05-18 17:21:09.264921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/lightgbm_registry.py
--rw-r--r--   0        0        0      706 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/onnx_registry.py
--rw-r--r--   0        0        0      775 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/paddle_registry.py
--rw-r--r--   0        0        0      744 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/pytorch_registry.py
--rw-r--r--   0        0        0      724 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/sklearn_registry.py
--rw-r--r--   0        0        0      712 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/spacy_registry.py
--rw-r--r--   0        0        0      748 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/statsmodel_registry.py
--rw-r--r--   0        0        0     3077 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/tensorflow_registry.py
--rw-r--r--   0        0        0      774 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/transformers_registry.py
--rw-r--r--   0        0        0      724 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/frameworks/xgboost_registry.py
--rw-r--r--   0        0        0     2349 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/git_info.py
--rw-r--r--   0        0        0        0 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/integrations/__init__.py
--rw-r--r--   0        0        0    15399 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/integrations/lightning.py
--rw-r--r--   0        0        0    22386 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/integrations/transformers.py
--rw-r--r--   0        0        0     1785 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/internal_namespace.py
--rw-r--r--   0        0        0      571 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/__init__.py
--rw-r--r--   0        0        0     7978 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/artifacts/artifact.py
--rw-r--r--   0        0        0     1019 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/artifacts/constants.py
--rw-r--r--   0        0        0     3068 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/artifacts/general_artifact.py
--rw-r--r--   0        0        0    15204 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/artifacts/model.py
--rw-r--r--   0        0        0     5983 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/artifacts/utils.py
--rw-r--r--   0        0        0     1281 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/dataset_artifact.py
--rw-r--r--   0        0        0      222 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/dataset_schema.py
--rw-r--r--   0        0        0      318 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/dataset_stats.py
--rw-r--r--   0        0        0       50 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/image/__init__.py
--rw-r--r--   0        0        0      255 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/image/constants.py
--rw-r--r--   0        0        0    11446 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/image/image.py
--rw-r--r--   0        0        0     2767 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/image/image_normalizer.py
--rw-r--r--   0        0        0     1566 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/image/types.py
--rw-r--r--   0        0        0      271 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/model_artifact.py
--rw-r--r--   0        0        0     7125 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/plot.py
--rw-r--r--   0        0        0     2486 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/pydantic_base.py
--rw-r--r--   0        0        0     1332 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/log_types/utils.py
--rw-r--r--   0        0        0      453 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/logger.py
--rw-r--r--   0        0        0     9286 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/login.py
--rw-r--r--   0        0        0        0 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/__init__.py
--rw-r--r--   0        0        0     1065 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v1/__init__.py
--rw-r--r--   0        0        0     2080 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v1/base_metrics.py
--rw-r--r--   0        0        0     6852 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v1/binary_classification_metrics.py
--rw-r--r--   0        0        0     6736 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v1/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     4419 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v1/regression_metrics.py
--rw-r--r--   0        0        0     3976 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v1/timeseries_metrics.py
--rw-r--r--   0        0        0     1026 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/__init__.py
--rw-r--r--   0        0        0     1898 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/base_metrics.py
--rw-r--r--   0        0        0      566 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/custom_metric_types.py
--rw-r--r--   0        0        0     6192 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     2718 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/regression_metrics.py
--rw-r--r--   0        0        0     2251 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/timeseries_metrics.py
--rw-r--r--   0        0        0      295 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/utils.py
--rw-r--r--   0        0        0    42544 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/mlfoundry_api.py
--rw-r--r--   0        0        0    46176 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/mlfoundry_run.py
--rw-r--r--   0        0        0        0 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/monitoring/__init__.py
--rw-r--r--   0        0        0     1994 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/monitoring/entities.py
--rw-r--r--   0        0        0       63 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/monitoring/store/__init__.py
--rw-r--r--   0        0        0     6630 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/monitoring/store/client.py
--rw-r--r--   0        0        0      169 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/monitoring/store/constants.py
--rw-r--r--   0        0        0      336 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/monitoring/store/repositories/__init__.py
--rw-r--r--   0        0        0     1351 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/monitoring/store/repositories/dto.py
--rw-r--r--   0        0        0     6529 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
--rw-r--r--   0        0        0     2178 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/monitoring/store/worker.py
--rw-r--r--   0        0        0     4304 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/run_utils.py
--rw-r--r--   0        0        0      492 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/schema.py
--rw-r--r--   0        0        0    10031 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/session.py
--rw-r--r--   0        0        0        0 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/tracking/__init__.py
--rw-r--r--   0        0        0     2766 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/tracking/auth_service.py
--rw-r--r--   0        0        0     2629 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/tracking/entities.py
--rw-r--r--   0        0        0     1175 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/tracking/servicefoundry_service.py
--rw-r--r--   0        0        0     4308 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/tracking/truefoundry_rest_store.py
--rw-r--r--   0        0        0        0 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 17:21:09.268921 mlfoundry-0.8.0rc4/mlfoundry/vendor/pynvml/__init__.py
--rw-r--r--   0        0        0    56147 2023-05-18 17:21:09.272921 mlfoundry-0.8.0rc4/mlfoundry/vendor/pynvml/pynvml.py
--rw-r--r--   0        0        0      253 2023-05-18 17:21:09.272921 mlfoundry-0.8.0rc4/mlfoundry/version.py
--rw-r--r--   0        0        0        0 2023-05-18 17:21:09.272921 mlfoundry-0.8.0rc4/mlfoundry/webapp/__init__.py
--rw-r--r--   0        0        0       38 2023-05-18 17:21:09.272921 mlfoundry-0.8.0rc4/mlfoundry/webapp/inputs.py
--rw-r--r--   0        0        0       39 2023-05-18 17:21:09.272921 mlfoundry-0.8.0rc4/mlfoundry/webapp/outputs.py
--rw-r--r--   0        0        0     3554 2023-05-18 17:21:23.177869 mlfoundry-0.8.0rc4/pyproject.toml
--rw-r--r--   0        0        0     4931 1970-01-01 00:00:00.000000 mlfoundry-0.8.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     3158 2023-05-31 16:00:16.854792 mlfoundry-0.8.1/README.md
+-rw-r--r--   0        0        0      991 2023-05-31 16:00:16.866792 mlfoundry-0.8.1/mlfoundry/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-31 16:00:16.866792 mlfoundry-0.8.1/mlfoundry/__main__.py
+-rw-r--r--   0        0        0     3713 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/amplitude.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/artifact/__init__.py
+-rw-r--r--   0        0        0     7069 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/artifact/truefoundry_artifact_repo.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/background/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/background/events.py
+-rw-r--r--   0        0        0     3032 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/background/interface.py
+-rw-r--r--   0        0        0     4016 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/background/sender.py
+-rw-r--r--   0        0        0     8756 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/background/system_metrics.py
+-rw-r--r--   0        0        0     4028 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/background/utils.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/cli/__init__.py
+-rw-r--r--   0        0        0      918 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/cli/cli_interface.py
+-rw-r--r--   0        0        0      100 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0      731 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/cli/commands/download.py
+-rw-r--r--   0        0        0      739 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/cli/commands/login.py
+-rw-r--r--   0        0        0     2724 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/constants.py
+-rw-r--r--   0        0        0      103 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/__init__.py
+-rw-r--r--   0        0        0     7854 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/dataset.py
+-rw-r--r--   0        0        0     2255 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/schema.py
+-rw-r--r--   0        0        0    13138 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/serde.py
+-rw-r--r--   0        0        0     2028 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/serde_utils.py
+-rw-r--r--   0        0        0     2078 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/stats.py
+-rw-r--r--   0        0        0     1903 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/types.py
+-rw-r--r--   0        0        0     2588 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/validation.py
+-rw-r--r--   0        0        0       69 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/whylogs_types/__init__.py
+-rw-r--r--   0        0        0     4025 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/whylogs_types/summary.py
+-rw-r--r--   0        0        0     1392 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/enums.py
+-rw-r--r--   0        0        0      325 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/env_vars.py
+-rw-r--r--   0        0        0      365 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/exceptions.py
+-rw-r--r--   0        0        0     2037 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/base_registry.py
+-rw-r--r--   0        0        0      718 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/fastai_registry.py
+-rw-r--r--   0        0        0      892 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/gluon_registry.py
+-rw-r--r--   0        0        0      700 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/h2o_registry.py
+-rw-r--r--   0        0        0      712 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/keras_registry.py
+-rw-r--r--   0        0        0      730 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/lightgbm_registry.py
+-rw-r--r--   0        0        0      706 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/onnx_registry.py
+-rw-r--r--   0        0        0      775 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/paddle_registry.py
+-rw-r--r--   0        0        0      744 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/pytorch_registry.py
+-rw-r--r--   0        0        0      724 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/sklearn_registry.py
+-rw-r--r--   0        0        0      712 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/spacy_registry.py
+-rw-r--r--   0        0        0      748 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/statsmodel_registry.py
+-rw-r--r--   0        0        0     3077 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/tensorflow_registry.py
+-rw-r--r--   0        0        0      774 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/transformers_registry.py
+-rw-r--r--   0        0        0      724 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/xgboost_registry.py
+-rw-r--r--   0        0        0     2349 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/git_info.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/integrations/__init__.py
+-rw-r--r--   0        0        0    15423 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/integrations/lightning.py
+-rw-r--r--   0        0        0    22410 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/integrations/transformers.py
+-rw-r--r--   0        0        0     1785 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/internal_namespace.py
+-rw-r--r--   0        0        0      571 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/__init__.py
+-rw-r--r--   0        0        0     7978 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/artifacts/artifact.py
+-rw-r--r--   0        0        0     1019 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/artifacts/constants.py
+-rw-r--r--   0        0        0     3072 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/artifacts/general_artifact.py
+-rw-r--r--   0        0        0    15275 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/artifacts/model.py
+-rw-r--r--   0        0        0     5983 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/artifacts/utils.py
+-rw-r--r--   0        0        0     1281 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/dataset_artifact.py
+-rw-r--r--   0        0        0      222 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/dataset_schema.py
+-rw-r--r--   0        0        0      318 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/dataset_stats.py
+-rw-r--r--   0        0        0       50 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/image/__init__.py
+-rw-r--r--   0        0        0      255 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/image/constants.py
+-rw-r--r--   0        0        0    11446 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/image/image.py
+-rw-r--r--   0        0        0     2767 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/image/image_normalizer.py
+-rw-r--r--   0        0        0     1566 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/image/types.py
+-rw-r--r--   0        0        0      271 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/model_artifact.py
+-rw-r--r--   0        0        0     7125 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/plot.py
+-rw-r--r--   0        0        0     2486 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/pydantic_base.py
+-rw-r--r--   0        0        0     1332 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/utils.py
+-rw-r--r--   0        0        0      453 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/logger.py
+-rw-r--r--   0        0        0     9286 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/login.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/__init__.py
+-rw-r--r--   0        0        0     1065 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v1/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v1/base_metrics.py
+-rw-r--r--   0        0        0     6852 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v1/binary_classification_metrics.py
+-rw-r--r--   0        0        0     6736 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v1/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     4419 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v1/regression_metrics.py
+-rw-r--r--   0        0        0     3976 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v1/timeseries_metrics.py
+-rw-r--r--   0        0        0     1026 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/__init__.py
+-rw-r--r--   0        0        0     1898 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/base_metrics.py
+-rw-r--r--   0        0        0      566 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/custom_metric_types.py
+-rw-r--r--   0        0        0     6192 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     2718 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/regression_metrics.py
+-rw-r--r--   0        0        0     2251 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/timeseries_metrics.py
+-rw-r--r--   0        0        0      295 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/utils.py
+-rw-r--r--   0        0        0    44772 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/mlfoundry_api.py
+-rw-r--r--   0        0        0    46176 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/mlfoundry_run.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/__init__.py
+-rw-r--r--   0        0        0     1994 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/entities.py
+-rw-r--r--   0        0        0       63 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/__init__.py
+-rw-r--r--   0        0        0     6630 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/client.py
+-rw-r--r--   0        0        0      169 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/constants.py
+-rw-r--r--   0        0        0      336 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/repositories/__init__.py
+-rw-r--r--   0        0        0     1351 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/repositories/dto.py
+-rw-r--r--   0        0        0     6529 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
+-rw-r--r--   0        0        0     2178 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/worker.py
+-rw-r--r--   0        0        0     4304 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/run_utils.py
+-rw-r--r--   0        0        0      492 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/schema.py
+-rw-r--r--   0        0        0    10031 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/session.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/tracking/__init__.py
+-rw-r--r--   0        0        0     2766 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/tracking/auth_service.py
+-rw-r--r--   0        0        0     2629 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/tracking/entities.py
+-rw-r--r--   0        0        0     1175 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/tracking/servicefoundry_service.py
+-rw-r--r--   0        0        0     4308 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/tracking/truefoundry_rest_store.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/vendor/pynvml/__init__.py
+-rw-r--r--   0        0        0    56147 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/vendor/pynvml/pynvml.py
+-rw-r--r--   0        0        0      253 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/version.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/webapp/__init__.py
+-rw-r--r--   0        0        0       38 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/webapp/inputs.py
+-rw-r--r--   0        0        0       39 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/webapp/outputs.py
+-rw-r--r--   0        0        0     3548 2023-05-31 16:00:27.847129 mlfoundry-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4925 1970-01-01 00:00:00.000000 mlfoundry-0.8.1/PKG-INFO
```

### Comparing `mlfoundry-0.8.0rc4/README.md` & `mlfoundry-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/__init__.py` & `mlfoundry-0.8.1/mlfoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/__main__.py` & `mlfoundry-0.8.1/mlfoundry/__main__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/amplitude.py` & `mlfoundry-0.8.1/mlfoundry/amplitude.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/artifact/truefoundry_artifact_repo.py` & `mlfoundry-0.8.1/mlfoundry/artifact/truefoundry_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/background/interface.py` & `mlfoundry-0.8.1/mlfoundry/background/interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/background/sender.py` & `mlfoundry-0.8.1/mlfoundry/background/sender.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/background/system_metrics.py` & `mlfoundry-0.8.1/mlfoundry/background/system_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/background/utils.py` & `mlfoundry-0.8.1/mlfoundry/background/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/cli/cli_interface.py` & `mlfoundry-0.8.1/mlfoundry/cli/cli_interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/cli/commands/download.py` & `mlfoundry-0.8.1/mlfoundry/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/cli/commands/login.py` & `mlfoundry-0.8.1/mlfoundry/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/constants.py` & `mlfoundry-0.8.1/mlfoundry/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/dataset/dataset.py` & `mlfoundry-0.8.1/mlfoundry/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/dataset/schema.py` & `mlfoundry-0.8.1/mlfoundry/dataset/schema.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/dataset/serde.py` & `mlfoundry-0.8.1/mlfoundry/dataset/serde.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/dataset/serde_utils.py` & `mlfoundry-0.8.1/mlfoundry/dataset/serde_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/dataset/stats.py` & `mlfoundry-0.8.1/mlfoundry/dataset/stats.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/dataset/types.py` & `mlfoundry-0.8.1/mlfoundry/dataset/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/dataset/validation.py` & `mlfoundry-0.8.1/mlfoundry/dataset/validation.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/dataset/whylogs_types/summary.py` & `mlfoundry-0.8.1/mlfoundry/dataset/whylogs_types/summary.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/enums.py` & `mlfoundry-0.8.1/mlfoundry/enums.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/__init__.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/fastai_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/fastai_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/gluon_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/gluon_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/h2o_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/h2o_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/keras_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/keras_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/lightgbm_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/lightgbm_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/onnx_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/onnx_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/paddle_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/paddle_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/pytorch_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/pytorch_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/sklearn_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/sklearn_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/spacy_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/spacy_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/statsmodel_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/statsmodel_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/tensorflow_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/tensorflow_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/transformers_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/transformers_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/frameworks/xgboost_registry.py` & `mlfoundry-0.8.1/mlfoundry/frameworks/xgboost_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/git_info.py` & `mlfoundry-0.8.1/mlfoundry/git_info.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/integrations/lightning.py` & `mlfoundry-0.8.1/mlfoundry/integrations/lightning.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     _convert_params,
     _sanitize_callable_params,
 )
 
 import mlfoundry
 from mlfoundry.enums import EnumMissingMixin
 from mlfoundry.logger import logger
-from mlfoundry.mlfoundry_api import resolve_ml_repo_name
+from mlfoundry.mlfoundry_api import _resolve_ml_repo_name
 from mlfoundry.mlfoundry_run import MlFoundryRun
 
 LIGHTNING_ARTIFACTS_PATH = "lightning/"
 LIGHTNING_MODELS_PATH = os.path.join(LIGHTNING_ARTIFACTS_PATH, "models")
 
 
 class LogModelStrategy(EnumMissingMixin, enum.Enum):
@@ -157,15 +157,17 @@
             prefix (str, optional): This prefix will be added in front of all metric_name logged.
 
         """
         super().__init__(agg_key_funcs=agg_key_funcs, agg_default_func=agg_default_func)
 
         log_model_strategy = LogModelStrategy(log_model_strategy)
 
-        self._ml_repo = resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
+        self._ml_repo = _resolve_ml_repo_name(
+            ml_repo=ml_repo, project_name=project_name
+        )
         self._run_name = run_name
         self._log_model_strategy = log_model_strategy
         self._flatten_params = flatten_params
         self._auto_end_run = True
         self._prefix = prefix
 
         self._run: Optional[MlFoundryRun] = None
```

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/integrations/transformers.py` & `mlfoundry-0.8.1/mlfoundry/integrations/transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from transformers.integrations import rewrite_logs
 from transformers.trainer_callback import TrainerCallback
 from transformers.utils import flatten_dict
 
 import mlfoundry
 from mlfoundry.enums import EnumMissingMixin
 from mlfoundry.logger import logger
-from mlfoundry.mlfoundry_api import resolve_ml_repo_name
+from mlfoundry.mlfoundry_api import _resolve_ml_repo_name
 from mlfoundry.mlfoundry_run import MlFoundryRun
 
 __all__ = ["HF_MODEL_PATH", "MlFoundryTrainerCallback", "LogModelStrategy"]
 
 
 HF_ARTIFACTS_PATH = "hf/"
 HF_MODELS_PATH = os.path.join(HF_ARTIFACTS_PATH, "models")
@@ -151,15 +151,17 @@
                 f"`log_model` argument has been deprecated, please use the `log_model_strategy` argument instead. "
                 f"E.g. log_model_strategy={_option}",
                 FutureWarning,
             )
             if kwargs["log_model"] and log_model_strategy == LogModelStrategy.NO:
                 log_model_strategy = LogModelStrategy.BEST_PLUS_LATEST
 
-        self._ml_repo = resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
+        self._ml_repo = _resolve_ml_repo_name(
+            ml_repo=ml_repo, project_name=project_name
+        )
         self._run_name = run_name
         self._run: Optional[MlFoundryRun] = None
         self._auto_end_run = True
 
         self._flatten_params = flatten_params
         self._log_model_strategy = log_model_strategy
         self._MAX_PARAM_VAL_LENGTH = 250
```

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/internal_namespace.py` & `mlfoundry-0.8.1/mlfoundry/internal_namespace.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/__init__.py` & `mlfoundry-0.8.1/mlfoundry/log_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/artifacts/artifact.py` & `mlfoundry-0.8.1/mlfoundry/log_types/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/artifacts/constants.py` & `mlfoundry-0.8.1/mlfoundry/log_types/artifacts/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/artifacts/general_artifact.py` & `mlfoundry-0.8.1/mlfoundry/log_types/artifacts/general_artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     metadata: Optional[Dict[str, Any]] = None,
     step: int = 0,
 ) -> ArtifactVersion:
 
     for i, artifact_path in enumerate(artifact_paths):
         if isinstance(artifact_path, ArtifactPath):
             continue
-        elif isinstance(artifact_path, collections.Sequence) and (
+        elif isinstance(artifact_path, collections.abc.Sequence) and (
             0 < len(artifact_path) <= 2
         ):
             artifact_paths[i] = ArtifactPath(*artifact_path)
         else:
             raise ValueError(
                 "`artifact_path` should be an instance of `mlfoundry.ArtifactPath` or a tuple of (src, dest) path strings"
             )
```

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/artifacts/model.py` & `mlfoundry-0.8.1/mlfoundry/log_types/artifacts/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,26 +392,31 @@
         artifact_size=model_size,
         step=step if run else None,
     )
     model_version = mlflow_client.create_model_version(
         artifact_version_id=version_id,
         description=description,
         artifact_metadata=metadata,
+        internal_metadata=internal_metadata.dict(),
         data_path=INTERNAL_METADATA_PATH,
         step=step if run else None,
     )
+
     # update model schema at end
-    if model_schema is not None:
-        try:
-            model_version = mlflow_client.update_model_version(
-                version_id=version_id,
-                model_schema=model_schema,
-                model_framework=framework.value,
-            )
+    update_args = {
+        "version_id": version_id,
+        "model_framework": framework.value,
+    }
+    if model_schema:
+        update_args["model_schema"] = model_schema
+
+    try:
+        model_version = mlflow_client.update_model_version(**update_args)
+        if model_schema:
             model_version = mlflow_client.add_custom_metrics_to_model_version(
                 version_id=version_id, custom_metrics=custom_metrics
             )
-        except Exception:
-            # TODO (chiragjn): what is the best exception to catch here?
-            logger.error(MODEL_SCHEMA_UPDATE_FAILURE_HELP.format(fqn=model_version.fqn))
+    except Exception:
+        # TODO (chiragjn): what is the best exception to catch here?
+        logger.error(MODEL_SCHEMA_UPDATE_FAILURE_HELP.format(fqn=model_version.fqn))
 
     return ModelVersion.from_fqn(fqn=model_version.fqn)
```

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/artifacts/utils.py` & `mlfoundry-0.8.1/mlfoundry/log_types/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/dataset_artifact.py` & `mlfoundry-0.8.1/mlfoundry/log_types/dataset_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/image/image.py` & `mlfoundry-0.8.1/mlfoundry/log_types/image/image.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/image/image_normalizer.py` & `mlfoundry-0.8.1/mlfoundry/log_types/image/image_normalizer.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/image/types.py` & `mlfoundry-0.8.1/mlfoundry/log_types/image/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/plot.py` & `mlfoundry-0.8.1/mlfoundry/log_types/plot.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/pydantic_base.py` & `mlfoundry-0.8.1/mlfoundry/log_types/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/log_types/utils.py` & `mlfoundry-0.8.1/mlfoundry/log_types/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/login.py` & `mlfoundry-0.8.1/mlfoundry/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/metrics/v1/__init__.py` & `mlfoundry-0.8.1/mlfoundry/metrics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/metrics/v1/base_metrics.py` & `mlfoundry-0.8.1/mlfoundry/metrics/v1/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/metrics/v1/binary_classification_metrics.py` & `mlfoundry-0.8.1/mlfoundry/metrics/v1/binary_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/metrics/v1/multiclass_classification_metrics.py` & `mlfoundry-0.8.1/mlfoundry/metrics/v1/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/metrics/v1/regression_metrics.py` & `mlfoundry-0.8.1/mlfoundry/metrics/v1/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/metrics/v1/timeseries_metrics.py` & `mlfoundry-0.8.1/mlfoundry/metrics/v1/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/__init__.py` & `mlfoundry-0.8.1/mlfoundry/metrics/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/base_metrics.py` & `mlfoundry-0.8.1/mlfoundry/metrics/v2/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/custom_metric_types.py` & `mlfoundry-0.8.1/mlfoundry/metrics/v2/custom_metric_types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/multiclass_classification_metrics.py` & `mlfoundry-0.8.1/mlfoundry/metrics/v2/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/regression_metrics.py` & `mlfoundry-0.8.1/mlfoundry/metrics/v2/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/metrics/v2/timeseries_metrics.py` & `mlfoundry-0.8.1/mlfoundry/metrics/v2/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/mlfoundry_api.py` & `mlfoundry-0.8.1/mlfoundry/mlfoundry_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,22 @@
     Tuple,
     Union,
 )
 
 import coolname
 import mlflow
 import pandas as pd
-from mlflow.entities import CustomMetric, Experiment, ModelSchema
+from mlflow.entities import (
+    Artifact,
+    ArtifactType,
+    CustomMetric,
+    Experiment,
+    Model,
+    ModelSchema,
+)
 from mlflow.store.tracking import SEARCH_MAX_RESULTS_DEFAULT
 from mlflow.tracking import MlflowClient
 
 from mlfoundry import amplitude, constants, env_vars
 from mlfoundry.enums import ModelFramework, ViewType
 from mlfoundry.env_vars import TRACKING_HOST_GLOBAL
 from mlfoundry.exceptions import MlflowException, MlFoundryException
@@ -93,15 +100,15 @@
         user_id = session.user_info.user_id
 
     amplitude.init(user_id=user_id, disable_analytics=disable_analytics)
     amplitude.track(amplitude.Event.GET_CLIENT)
     return MlFoundry(session=session)
 
 
-def resolve_ml_repo_name(
+def _resolve_ml_repo_name(
     ml_repo: Optional[str] = None,
     project_name: Optional[str] = None,
 ) -> str:
     if project_name and ml_repo:
         raise MlFoundryException(
             f"Only one of `ml_repo` or `project_name` should be passed"
         )
@@ -183,15 +190,15 @@
 
         return ml_repos_names
 
     def create_ml_repo(
         self,
         ml_repo: Optional[str] = None,
         storage_integration_fqn: Optional[str] = None,
-    ) -> Experiment:
+    ):
         existing_ml_repo = self.mlflow_client.get_experiment_by_name(name=ml_repo)
         if not existing_ml_repo:  # ml_repo does not exist
             return self.mlflow_client.get_experiment(
                 experiment_id=self.mlflow_client.create_experiment(
                     name=ml_repo, storage_integration_fqn=storage_integration_fqn
                 )
             )
@@ -298,15 +305,15 @@
 
         if not run_name:
             run_name = coolname.generate_slug(2)
             logger.info(
                 f"No run_name given. Using a randomly generated name {run_name}."
                 " You can pass your own using the `run_name` argument"
             )
-        ml_repo = resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
+        ml_repo = _resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
 
         ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
 
         if tags is not None:
             NAMESPACE.validate_namespace_not_used(tags.keys())
         else:
             tags = {}
@@ -377,15 +384,15 @@
         The user must have `READ` access to the project.
         Args:
             ml_repo (str): Name of the project.
         Returns:
             pd.DataFrame: dataframe with two columns- run_id and run_name
         """
         amplitude.track(amplitude.Event.GET_ALL_RUNS)
-        ml_repo = resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
+        ml_repo = _resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
         ml_repo_obj = self.mlflow_client.get_experiment_by_name(ml_repo)
         if ml_repo_obj is None:
             return pd.DataFrame(
                 columns=[constants.RUN_ID_COL_NAME, constants.RUN_NAME_COL_NAME]
             )
 
         ml_repo_id = ml_repo_obj.experiment_id
@@ -480,15 +487,15 @@
             )
 
             ```
 
         Returns:
             Genarator[MlFoundryRun, None, None]: MLFoundryRuns matching the search query.
         """
-        ml_repo = resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
+        ml_repo = _resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
         try:
             run_view_type = ViewType.from_string(run_view_type.lower())
         except Exception as e:
             raise MlFoundryException(e) from e
 
         try:
             ml_repo_obj = self.mlflow_client.get_experiment_by_name(ml_repo)
@@ -547,15 +554,23 @@
             print(download_info)
             ```
         """
         # TODO (chiragjn): This API is called get_model and it returns ModelVersion
         #   This will cause confusion later when we have to eventually introduce APIs to get the parent Model class
         return ModelVersion.from_fqn(fqn)
 
-    def list_model_versions(self, model_fqn: str) -> Iterator[ModelVersion]:
+    def list_model_versions(self, ml_repo: str, name: str) -> Iterator[ModelVersion]:
+        ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
+        models = self.mlflow_client.list_models(ml_repo_id=ml_repo_id, name=name)
+        if not models or len(models) == 0:
+            err_msg = f"Model Does Not Exist for ml_repo={ml_repo}, name={name}"
+            raise MlFoundryException(err_msg)
+        return self._list_model_versions_by_id(model=models[0])
+
+    def list_model_versions_by_fqn(self, model_fqn: str) -> Iterator[ModelVersion]:
         """
         List versions for a given model
 
         Args:
             model_fqn: FQN of the Model to list versions for.
                 A model_fqn looks like `model:{org}/{user}/{project}/{artifact_name}`
                 or `model:{user}/{project}/{artifact_name}`
@@ -576,20 +591,32 @@
             client = mlfoundry.get_client()
             model_fqn = "model:org/user/my-project/my-model"
             for mv in client.list_model_versions(model_fqn=model_fqn):
                 print(mv.name, mv.version, mv.description)
             ```
         """
         model = self.mlflow_client.get_model_by_fqn(fqn=model_fqn)
-        max_results = 10
-        page_token = None
-        done = False
+        return self._list_model_versions_by_id(model=model)
+
+    def _list_model_versions_by_id(
+        self, model_id: str = None, model: Model = None
+    ) -> Iterator[ModelVersion]:
+        if model and not model_id:
+            model_id = model.id
+        elif not model and model_id:
+            model = self.mlflow_client.get_model_by_id(model_id=model_id)
+        else:
+            raise MlFoundryException(
+                "Exactly one of model_id or model should be passed"
+            )
+
+        max_results, page_token, done = 10, None, False
         while not done:
             model_versions = self.mlflow_client.list_model_versions(
-                model_id=model.id, max_results=max_results, page_token=page_token
+                model_id=model_id, max_results=max_results, page_token=page_token
             )
             page_token = model_versions.token
             for model_version in model_versions:
                 yield ModelVersion(model_version=model_version, model=model)
             if not model_versions or not page_token:
                 done = True
 
@@ -615,15 +642,32 @@
             print(download_info)
             ```
         """
         # TODO (chiragjn): This API is called get_artifact and it returns ArtifactVersion
         #   This will cause confusion later when we have to eventually introduce APIs to get the parent Artifact class
         return ArtifactVersion.from_fqn(fqn)
 
-    def list_artifact_versions(self, artifact_fqn: str) -> Iterator[ArtifactVersion]:
+    def list_artifact_versions(
+        self,
+        ml_repo: str,
+        name: str,
+        artifact_type: Optional[ArtifactType] = ArtifactType.ARTIFACT,
+    ) -> Iterator[ArtifactVersion]:
+        ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
+        artifacts = self.mlflow_client.list_artifacts_(
+            ml_repo_id=ml_repo_id, name=name, artifact_type=artifact_type
+        )
+        if not artifacts or len(artifacts) == 0:
+            err_msg = f"Artifact Does Not Exist for ml_repo={ml_repo}, name={name}, type={artifact_type}"
+            raise MlFoundryException(err_msg)
+        return self._list_artifact_versions_by_id(artifact=artifacts[0])
+
+    def list_artifact_versions_by_fqn(
+        self, artifact_fqn: str
+    ) -> Iterator[ArtifactVersion]:
         """
         List versions for a given artifact
 
         Args:
             artifact_fqn: FQN of the Artifact to list versions for.
                 An artifact_fqn looks like `{artifact_type}:{org}/{user}/{project}/{artifact_name}`
                 or `{artifact_type}:{user}/{project}/{artifact_name}`
@@ -648,20 +692,32 @@
             client = mlfoundry.get_client()
             artifact_fqn = "artifact:org/user/my-project/my-artifact"
             for av in client.list_artifact_versions(artifact_fqn=artifact_fqn):
                 print(av.name, av.version, av.description)
             ```
         """
         artifact = self.mlflow_client.get_artifact_by_fqn(fqn=artifact_fqn)
-        max_results = 10
-        page_token = None
-        done = False
+        return self._list_artifact_versions_by_id(artifact=artifact)
+
+    def _list_artifact_versions_by_id(
+        self, artifact_id: str = None, artifact: Artifact = None
+    ) -> Iterator[ArtifactVersion]:
+        if artifact and not artifact_id:
+            artifact_id = artifact.id
+        elif not artifact and artifact_id:
+            artifact = self.mlflow_client.get_artifact_by_id(artifact_id=artifact_id)
+        else:
+            raise MlFoundryException(
+                "Exactly one of artifact_id or artifact should be passed"
+            )
+
+        max_results, page_token, done = 10, None, False
         while not done:
             artifact_versions = self.mlflow_client.list_artifact_versions(
-                artifact_id=artifact.id, max_results=max_results, page_token=page_token
+                artifact_id=artifact_id, max_results=max_results, page_token=page_token
             )
             page_token = artifact_versions.token
             for artifact_version in artifact_versions:
                 yield ArtifactVersion(
                     artifact_version=artifact_version, artifact=artifact
                 )
             if not artifact_versions or not page_token:
```

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/mlfoundry_run.py` & `mlfoundry-0.8.1/mlfoundry/mlfoundry_run.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/monitoring/entities.py` & `mlfoundry-0.8.1/mlfoundry/monitoring/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/monitoring/store/client.py` & `mlfoundry-0.8.1/mlfoundry/monitoring/store/client.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/monitoring/store/repositories/dto.py` & `mlfoundry-0.8.1/mlfoundry/monitoring/store/repositories/dto.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py` & `mlfoundry-0.8.1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/monitoring/store/worker.py` & `mlfoundry-0.8.1/mlfoundry/monitoring/store/worker.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/run_utils.py` & `mlfoundry-0.8.1/mlfoundry/run_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/session.py` & `mlfoundry-0.8.1/mlfoundry/session.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/tracking/auth_service.py` & `mlfoundry-0.8.1/mlfoundry/tracking/auth_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/tracking/entities.py` & `mlfoundry-0.8.1/mlfoundry/tracking/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/tracking/servicefoundry_service.py` & `mlfoundry-0.8.1/mlfoundry/tracking/servicefoundry_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/tracking/truefoundry_rest_store.py` & `mlfoundry-0.8.1/mlfoundry/tracking/truefoundry_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/mlfoundry/vendor/pynvml/pynvml.py` & `mlfoundry-0.8.1/mlfoundry/vendor/pynvml/pynvml.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.0rc4/pyproject.toml` & `mlfoundry-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlfoundry"
-version = "0.8.0rc4" # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.8.1" # do not change, auto-generated by poetry-dynamic-versioning
 description = "Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/truefoundry/mlfoundry"
 repository = "https://github.com/truefoundry/mlfoundry"
 readme = "README.md"
 packages = [
     { include = "mlfoundry" },
@@ -31,15 +31,15 @@
 pydantic = ">=1.8.2,<2.0.0"
 scikit-learn = ">=0.24.2,<2.0.0"
 scipy = [
     # This is split into two because poetry will select a version which has no wheel on python >= 3.10 :/
     { version = ">=1.5.4,<2.0.0", python = "<3.10" },
     { version = ">=1.8.0,<2.0.0", python = ">=3.10" },
 ]
-tfy-mlflow-client = "0.0.29rc3"
+tfy-mlflow-client = "0.0.31"
 # Check and try to eliminate libs below this comment
 boto3 = ">=1.14.1,<2.0.0"
 fastparquet = ">=0.8.0,<=2022.12.0"
 importlib-metadata = ">=4.11.3,<5.0.0"
 packaging = ">=20.0,<24.0"
 pyarrow = ">=5.0.0,<11.0.0"
 whylogs = [
```

### Comparing `mlfoundry-0.8.0rc4/PKG-INFO` & `mlfoundry-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfoundry
-Version: 0.8.0rc4
+Version: 0.8.1
 Summary: Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library
 Home-page: https://github.com/truefoundry/mlfoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -27,15 +27,15 @@
 Requires-Dist: protobuf (>=3.19.0,<3.21.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: pyarrow (>=5.0.0,<11.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: scikit-learn (>=0.24.2,<2.0.0)
 Requires-Dist: scipy (>=1.5.4,<2.0.0) ; python_version < "3.10"
 Requires-Dist: scipy (>=1.8.0,<2.0.0) ; python_version >= "3.10"
-Requires-Dist: tfy-mlflow-client (==0.0.29rc3)
+Requires-Dist: tfy-mlflow-client (==0.0.31)
 Requires-Dist: whylogs (>=0.6.15,<1.0.0) ; python_version < "3.10"
 Requires-Dist: whylogs (>=1.0.0,<2.0.0) ; python_version >= "3.10"
 Project-URL: Repository, https://github.com/truefoundry/mlfoundry
 Description-Content-Type: text/markdown
 
 # MlFoundry
```

