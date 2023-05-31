# Comparing `tmp/kaskada-0.2.0.tar.gz` & `tmp/kaskada-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaskada-0.2.0.tar", max compression
+gzip compressed data, was "kaskada-0.4.0.tar", max compression
```

## Comparing `kaskada-0.2.0.tar` & `kaskada-0.4.0.tar`

### file list

```diff
@@ -1,65 +1,73 @@
--rw-r--r--   0        0        0     1646 2023-05-16 11:01:01.364553 kaskada-0.2.0/README.md
--rw-r--r--   0        0        0     3882 2023-05-16 11:01:01.364553 kaskada-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7371 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/fenlmagic/__init__.py
--rw-r--r--   0        0        0      401 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/fenlmagic/utils.py
--rw-r--r--   0        0        0       33 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/api/__init__.py
--rw-r--r--   0        0        0     1246 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/api/api_utils.py
--rw-r--r--   0        0        0     6381 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/api/release.py
--rw-r--r--   0        0        0    10056 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/api/session.py
--rw-r--r--   0        0        0     5838 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/client.py
--rw-r--r--   0        0        0     1500 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/formatters.css
--rw-r--r--   0        0        0      984 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/formatters.js
--rw-r--r--   0        0        0    26206 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/formatters.py
--rw-r--r--   0        0        0     7337 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/formatters_helpers.py
--rw-r--r--   0        0        0     9833 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/formatters_shared.py
--rw-r--r--   0        0        0     7626 2023-05-16 11:01:01.900555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/common_pb2.py
--rw-r--r--   0        0        0      159 2023-05-16 11:01:01.900555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
--rw-r--r--   0        0        0    12572 2023-05-16 11:01:01.936555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
--rw-r--r--   0        0        0    12538 2023-05-16 11:01:01.936555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
--rw-r--r--   0        0        0     4489 2023-05-16 11:01:01.968555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
--rw-r--r--   0        0        0     2938 2023-05-16 11:01:01.960555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
--rw-r--r--   0        0        0     4191 2023-05-16 11:01:01.992555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/destinations_pb2.py
--rw-r--r--   0        0        0      159 2023-05-16 11:01:02.004555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
--rw-r--r--   0        0        0     2668 2023-05-16 11:01:02.016555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
--rw-r--r--   0        0        0      159 2023-05-16 11:01:02.028555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
--rw-r--r--   0        0        0     3976 2023-05-16 11:01:02.048555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/file_service_pb2.py
--rw-r--r--   0        0        0     5054 2023-05-16 11:01:02.068555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
--rw-r--r--   0        0        0    10837 2023-05-16 11:01:02.080555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
--rw-r--r--   0        0        0     9283 2023-05-16 11:01:02.096555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     1897 2023-05-16 11:01:02.108555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/options_pb2.py
--rw-r--r--   0        0        0      159 2023-05-16 11:01:02.132555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
--rw-r--r--   0        0        0    13180 2023-05-16 11:01:02.132555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/plan_pb2.py
--rw-r--r--   0        0        0      159 2023-05-16 11:01:02.168556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
--rw-r--r--   0        0        0     3398 2023-05-16 11:01:02.168556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
--rw-r--r--   0        0        0     4894 2023-05-16 11:01:02.208556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
--rw-r--r--   0        0        0     2805 2023-05-16 11:01:02.192556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
--rw-r--r--   0        0        0      159 2023-05-16 11:01:02.240556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
--rw-r--r--   0        0        0    11773 2023-05-16 11:01:02.236556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/query_service_pb2.py
--rw-r--r--   0        0        0     6542 2023-05-16 11:01:02.272556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     4018 2023-05-16 11:01:02.272556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/schema_pb2.py
--rw-r--r--   0        0        0      159 2023-05-16 11:01:02.320556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-16 11:01:02.304556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/sources_pb2.py
--rw-r--r--   0        0        0      159 2023-05-16 11:01:02.336556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
--rw-r--r--   0        0        0     2729 2023-05-16 11:01:02.344556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/spec_pb2.py
--rw-r--r--   0        0        0      159 2023-05-16 11:01:02.392556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
--rw-r--r--   0        0        0    11249 2023-05-16 11:01:02.376556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/table_service_pb2.py
--rw-r--r--   0        0        0    10053 2023-05-16 11:01:02.404556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
--rw-r--r--   0        0        0     5157 2023-05-16 11:01:02.448556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
--rw-r--r--   0        0        0      159 2023-05-16 11:01:02.440556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
--rw-r--r--   0        0        0     8140 2023-05-16 11:01:02.476556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/view_service_pb2.py
--rw-r--r--   0        0        0     8153 2023-05-16 11:01:02.472556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
--rw-r--r--   0        0        0    16491 2023-05-16 11:01:02.508556 kaskada-0.2.0/src/kaskada/kaskada/v2alpha/query_service_pb2.py
--rw-r--r--   0        0        0     8377 2023-05-16 11:01:02.504557 kaskada-0.2.0/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     8622 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/materialization.py
--rw-r--r--   0        0        0     9272 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/query.py
--rw-r--r--   0        0        0     2564 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/slice_filters.py
--rw-r--r--   0        0        0    10126 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/table.py
--rw-r--r--   0        0        0     7131 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/utils.py
--rw-r--r--   0        0        0     4543 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/view.py
--rw-r--r--   0        0        0    29800 2023-05-16 11:01:01.364553 kaskada-0.2.0/vendor/validate/validate.proto
--rw-r--r--   0        0        0    13089 2023-05-16 11:01:01.364553 kaskada-0.2.0/vendor/validate/validate_pb2.py
--rw-r--r--   0        0        0    22952 2023-05-16 11:01:01.368553 kaskada-0.2.0/vendor/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-16 11:01:01.368553 kaskada-0.2.0/vendor/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 kaskada-0.2.0/setup.py
--rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 kaskada-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1646 2023-05-31 11:54:25.771904 kaskada-0.4.0/README.md
+-rw-r--r--   0        0        0     3917 2023-05-31 11:54:25.771904 kaskada-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7656 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/fenlmagic/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/fenlmagic/utils.py
+-rw-r--r--   0        0        0       33 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/api_utils.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/local_session/__init__.py
+-rw-r--r--   0        0        0     3573 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/local_session/local_service.py
+-rw-r--r--   0        0        0     3312 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/local_session/local_session_keep_alive.py
+-rw-r--r--   0        0        0     6381 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/release.py
+-rw-r--r--   0        0        0     1108 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/remote_session/__init__.py
+-rw-r--r--   0        0        0    11294 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/api/session.py
+-rw-r--r--   0        0        0    11972 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/client.py
+-rw-r--r--   0        0        0     1500 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/formatters.css
+-rw-r--r--   0        0        0      984 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/formatters.js
+-rw-r--r--   0        0        0    26206 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/formatters.py
+-rw-r--r--   0        0        0     7337 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/formatters_helpers.py
+-rw-r--r--   0        0        0    10325 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/formatters_shared.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/health/__init__.py
+-rw-r--r--   0        0        0     1886 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/health/health_check_client.py
+-rw-r--r--   0        0        0     4522 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/health/health_check_servicer.py
+-rw-r--r--   0        0        0     2326 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/health/health_check_watcher.py
+-rw-r--r--   0        0        0     7626 2023-05-31 11:54:26.287927 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/common_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-31 11:54:26.291927 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
+-rw-r--r--   0        0        0    12572 2023-05-31 11:54:26.319928 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
+-rw-r--r--   0        0        0    12538 2023-05-31 11:54:26.315928 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4489 2023-05-31 11:54:26.351930 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
+-rw-r--r--   0        0        0     2938 2023-05-31 11:54:26.367930 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4191 2023-05-31 11:54:26.375931 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/destinations_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-31 11:54:26.411932 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
+-rw-r--r--   0        0        0     2718 2023-05-31 11:54:26.411932 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-31 11:54:26.447934 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
+-rw-r--r--   0        0        0     3976 2023-05-31 11:54:26.447934 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/file_service_pb2.py
+-rw-r--r--   0        0        0     5054 2023-05-31 11:54:26.471935 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10837 2023-05-31 11:54:26.471935 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
+-rw-r--r--   0        0        0     9283 2023-05-31 11:54:26.495936 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1897 2023-05-31 11:54:26.503936 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/options_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-31 11:54:26.527938 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
+-rw-r--r--   0        0        0    13180 2023-05-31 11:54:26.531938 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/plan_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-31 11:54:26.555939 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
+-rw-r--r--   0        0        0     3398 2023-05-31 11:54:26.559939 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
+-rw-r--r--   0        0        0     4894 2023-05-31 11:54:26.579940 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2805 2023-05-31 11:54:26.587940 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-31 11:54:26.607941 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
+-rw-r--r--   0        0        0    11773 2023-05-31 11:54:26.619942 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     6542 2023-05-31 11:54:26.631942 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4018 2023-05-31 11:54:26.831951 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/schema_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-31 11:54:26.667944 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-31 11:54:26.703945 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/sources_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-31 11:54:26.731947 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
+-rw-r--r--   0        0        0     2729 2023-05-31 11:54:26.767948 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/spec_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-31 11:54:26.791949 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
+-rw-r--r--   0        0        0    11249 2023-05-31 11:54:26.819950 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/table_service_pb2.py
+-rw-r--r--   0        0        0    10053 2023-05-31 11:54:26.843952 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5157 2023-05-31 11:54:26.855952 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-31 11:54:26.871953 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
+-rw-r--r--   0        0        0     8140 2023-05-31 11:54:26.875953 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/view_service_pb2.py
+-rw-r--r--   0        0        0     8153 2023-05-31 11:54:26.891954 kaskada-0.4.0/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16491 2023-05-31 11:54:26.907954 kaskada-0.4.0/src/kaskada/kaskada/v2alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     8377 2023-05-31 11:54:26.923955 kaskada-0.4.0/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8622 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/materialization.py
+-rw-r--r--   0        0        0     9272 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/query.py
+-rw-r--r--   0        0        0     2564 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/slice_filters.py
+-rw-r--r--   0        0        0    10126 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/table.py
+-rw-r--r--   0        0        0     7131 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/utils.py
+-rw-r--r--   0        0        0     4543 2023-05-31 11:54:25.771904 kaskada-0.4.0/src/kaskada/view.py
+-rw-r--r--   0        0        0    29800 2023-05-31 11:54:25.775904 kaskada-0.4.0/vendor/validate/validate.proto
+-rw-r--r--   0        0        0    13089 2023-05-31 11:54:25.775904 kaskada-0.4.0/vendor/validate/validate_pb2.py
+-rw-r--r--   0        0        0    22952 2023-05-31 11:54:25.775904 kaskada-0.4.0/vendor/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:54:25.775904 kaskada-0.4.0/vendor/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 kaskada-0.4.0/setup.py
+-rw-r--r--   0        0        0     2742 1970-01-01 00:00:00.000000 kaskada-0.4.0/PKG-INFO
```

### Comparing `kaskada-0.2.0/README.md` & `kaskada-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/pyproject.toml` & `kaskada-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [tool.poetry]
 name = "kaskada"
-version = "0.2.0"
+version = "0.4.0"
 description = "A client library for the Kaskada time travel machine learning service"
 authors = ["Kaskada <maintainers@kaskada.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "kaskada", from = "src" },
     { include = "validate", from = "vendor" },
     { include = "fenlmagic", from = "src" },
 ]
 include = ["**/src/kaskada/kaskada/**/*.py"]
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python = "^3.8.2"
 certifi = "^2022.12.7"
 domonic = "^0.9.11"
 googleapis-common-protos = "^1.58.0"
 html5lib = "^1.1"
 pyarrow = "^10.0.1"
 requests = "^2.28.2"
 grpcio-status = "^1.51.1"
 grpcio = "^1.51.1"
 tqdm = "^4.64.1"
 pygithub = "^1.57"
 pandas = "~1.3"
 ipython = "7.34.0"
+grpcio-health-checking = "^1.54.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 pylint = "^2.15.10"
 pytest = "^7.2.0"
@@ -140,15 +141,15 @@
 
 
 module = ["kaskada.kaskada.*"]
 ignore_errors = true
 ignore_missing_imports = true
 
 [tool.pylint.format]
-max-line-length = "120"
+max-line-length = "200"
 fail-under = "5"
 
 [tool.pylint.MASTER]
 ignore-paths = 'src/ksakada/kaskada'
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `kaskada-0.2.0/src/fenlmagic/__init__.py` & `kaskada-0.4.0/src/fenlmagic/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -176,18 +176,25 @@
             return query_result
         except Exception as e:
             raise UsageError(e)
 
 
 def load_ipython_extension(ipython):
     if client.KASKADA_DEFAULT_CLIENT is None:
-        client_id = os.getenv("KASKADA_CLIENT_ID", None)
-        client.init(client_id=client_id)
+        logger.warn(
+            "No client was initialized. Initializing default client to connect to localhost:50051."
+        )
+        default_client = client.Client(
+            client_id=os.getenv("KASKADA_CLIENT_ID", None),
+            endpoint=client.KASKADA_DEFAULT_ENDPOINT,
+            is_secure=client.KASKADA_IS_SECURE,
+        )
+        client.set_default_client(default_client)
 
-    magics = FenlMagics(ipython, client.KASKADA_DEFAULT_CLIENT)
+    magics = FenlMagics(ipython, client.get_client())
     ipython.register_magics(magics)
 
 
 def clean_arg(arg: str) -> str:
     """
     Strips quotes and double-quotes from passed arguments
```

### Comparing `kaskada-0.2.0/src/kaskada/api/release.py` & `kaskada-0.4.0/src/kaskada/api/release.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/api/session.py` & `kaskada-0.4.0/src/kaskada/api/session.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,122 @@
 import logging
 import os
-import sys
 import time
 from abc import ABC
 from datetime import datetime
 from pathlib import Path
-from subprocess import Popen
 from typing import Any, Dict, Optional, Tuple
 
 import kaskada.client
-from kaskada.api import api_utils, release
+from kaskada.api import release
+from kaskada.api.local_session.local_service import KaskadaLocalService
+from kaskada.api.local_session.local_session_keep_alive import LocalSessionKeepAlive
 
-logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
+KASKADA_PATH_ENV = "KASKADA_PATH"
+KASKADA_PATH_DEFAULT = "~/.cache/kaskada"
+KASKADA_LOG_PATH_DEFAULT = "logs"
+KASKADA_LOG_PATH_ENV = "KASKADA_LOG_PATH"
+KASKADA_BIN_PATH_DEFAULT = "bin"
+KASKADA_BIN_PATH_ENV = "KASKADA_BIN_PATH"
+
+KASKADA_MANAGER_BIN_NAME_DEFAULT = "kaskada-manager"
+KASKADA_ENGINE_BIN_NAME_DEFAULT = "kaskada-engine"
+
+KASKADA_DISABLE_DOWNLOAD_ENV = "KASKADA_DISABLE_DOWNLOAD"
+
+
 class Session:
     def __init__(
         self,
         endpoint: str,
         is_secure: bool,
         client_id: Optional[str] = None,
-        manager_process: Optional[Popen] = None,
-        engine_process: Optional[Popen] = None,
+        client_factory: Optional[kaskada.client.ClientFactory] = None,
     ) -> None:
         self._endpoint = endpoint
         self._is_secure = is_secure
         self._client_id = client_id
-        self._client = self.connect()
-        self._manager_process = manager_process
-        self._engine_process = engine_process
-
-    def __del__(self):
-        if self._manager_process is not None:
-            logger.info(
-                "Stopping Kaskada Manager service"
-            ) if logger is not None else None
-            self._manager_process.kill()
-
-        if self._engine_process is not None:
-            logger.info(
-                "Stopping Kaskada Engine service"
-            ) if logger is not None else None
-            self._engine_process.kill()
-
-    def connect(self):
-        attempt = 0
-        is_valid_session = False
-        while attempt < 3 and not is_valid_session:
-            logger.debug(f"Attempting (try #{attempt}) to connect to {self._endpoint}")
-            if api_utils.check_socket(self._endpoint):
-                logger.info(f"Successfully connected to session.")
-                is_valid_session = True
-            attempt += 1
-            # Sleep with exponential backoff
-            time.sleep(1.5**attempt)
-        if is_valid_session == False:
-            raise ConnectionError(
-                "unable to connect to Manager or Engine after {} attempts".format(
-                    attempt
-                )
+        self.client: Optional[kaskada.client.Client] = None
+        if client_factory is None:
+            self.client_factory = kaskada.client.ClientFactory(
+                self._client_id, self._endpoint, self._is_secure
             )
-        return kaskada.client.init(self._client_id, self._endpoint, self._is_secure)
+        else:
+            self.client_factory = client_factory
+
+    def stop(self):
+        kaskada.client.reset()
+        global KASKADA_SESSION
+        KASKADA_SESSION = None
+
+    def connect(self, should_check_health: bool = True) -> kaskada.client.Client:
+        self.client = self.client_factory.get_client(
+            should_check_health=should_check_health
+        )
+        assert self.client is not None
+        kaskada.client.set_default_client(self.client)
+        return self.client
+
+
+class LocalSession(Session):
+    """An extension of a kaskada.api.Session that is executed locally. The local session is kept alive by using the LocalSessionKeepAlive."""
+
+    keep_alive_watcher: Optional[LocalSessionKeepAlive] = None
+
+    def __init__(
+        self,
+        endpoint: str,
+        is_secure: bool,
+        manager_service: KaskadaLocalService,
+        engine_service: KaskadaLocalService,
+        client_id: Optional[str] = None,
+        should_keep_alive: bool = True,
+    ):
+        """Instantiates a LocalSession.
+
+        Args:
+            endpoint (str): The endpoint of the manager service
+            is_secure (bool): True to use TLS or False to use an insecure connection
+            manager_service (KaskadaLocalService): The manager service resource
+            engine_service (KaskadaLocalService): The engine service resource
+            client_id (Optional[str], optional): A custom client ID. Defaults to None.
+        """
+        super().__init__(endpoint, is_secure, client_id)
+        self.manager_service = manager_service
+        self.engine_service = engine_service
+        self.should_keep_alive = should_keep_alive
+
+    def start(self):
+        """Starts the local session by calling start on all services and connect on the client."""
+        self.manager_service.start()
+        self.engine_service.start()
+        client = self.connect()
+        self.keep_alive_watcher = LocalSessionKeepAlive(
+            self.manager_service,
+            self.engine_service,
+            client,
+            should_check=self.should_keep_alive,
+        )
+        self.keep_alive_watcher.start()
+
+    def stop(self):
+        """Stops the local session by calling stop on all services and stops the keep alive watcher."""
+        self.keep_alive_watcher.stop()
+        self.keep_alive_watcher.join()
+        self.client.disconnect()
+        super().stop()
+        self.manager_service.stop()
+        self.engine_service.stop()
+        logger.info("Local session successfully stopped.")
+
+
+KASKADA_SESSION: Optional[LocalSession] = None
 
 
 class Builder(ABC):
     def __init__(
         self,
         endpoint: Optional[str] = None,
         is_secure: Optional[bool] = None,
@@ -88,52 +139,34 @@
         return self
 
     def client_id(self, client_id: str):
         self._client_id = client_id
         return self
 
 
-KASKADA_ENDPOINT_DEFAULT = "localhost:50051"
-KASKADA_IS_SECURE_DEFAULT = False
-
-
 class LocalBuilder(Builder):
-    KASKADA_PATH_ENV = "KASKADA_PATH"
-    KASKADA_PATH_DEFAULT = "~/.cache/kaskada"
-    KASKADA_LOG_PATH_DEFAULT = "logs"
-    KASKADA_LOG_PATH_ENV = "KASKADA_LOG_PATH"
-    KASKADA_BIN_PATH_DEFAULT = "bin"
-    KASKADA_BIN_PATH_ENV = "KASKADA_BIN_PATH"
 
-    KASKADA_MANAGER_BIN_NAME_DEFAULT = "kaskada-manager"
-    KASKADA_ENGINE_BIN_NAME_DEFAULT = "kaskada-engine"
-
-    KASKADA_DISABLE_DOWNLOAD_ENV = "KASKADA_DISABLE_DOWNLOAD"
+    manager_configs: Dict[str, Any]
+    engine_configs: Dict[str, Any]
 
     def __init__(
         self,
-        endpoint: str = KASKADA_ENDPOINT_DEFAULT,
-        is_secure: bool = KASKADA_IS_SECURE_DEFAULT,
+        endpoint: str = kaskada.client.KASKADA_DEFAULT_ENDPOINT,
+        is_secure: bool = kaskada.client.KASKADA_IS_SECURE,
     ) -> None:
         super().__init__()
-        self._path: str = os.getenv(
-            LocalBuilder.KASKADA_PATH_ENV, LocalBuilder.KASKADA_PATH_DEFAULT
-        )
-        self._bin_path: str = os.getenv(
-            LocalBuilder.KASKADA_BIN_PATH_ENV, LocalBuilder.KASKADA_BIN_PATH_DEFAULT
-        )
-        self._log_path: str = os.getenv(
-            LocalBuilder.KASKADA_LOG_PATH_ENV, LocalBuilder.KASKADA_LOG_PATH_DEFAULT
-        )
+        self.manager_configs = {"-no-color": "1"}
+        self._path: str = os.getenv(KASKADA_PATH_ENV, KASKADA_PATH_DEFAULT)
+        self._bin_path: str = os.getenv(KASKADA_BIN_PATH_ENV, KASKADA_BIN_PATH_DEFAULT)
+        self._log_path: str = os.getenv(KASKADA_LOG_PATH_ENV, KASKADA_LOG_PATH_DEFAULT)
         self.endpoint(endpoint, is_secure)
-        self._download = (
-            os.getenv(LocalBuilder.KASKADA_DISABLE_DOWNLOAD_ENV, "false") != "true"
-        )
-        self._manager_configs: Dict[str, Any] = {"-no-color": "1"}
-        self._engine_configs: Dict[str, Any] = {"--log-no-color": "1"}
+        self._download = os.getenv(KASKADA_DISABLE_DOWNLOAD_ENV, "false") != "true"
+        self.in_memory(False)
+        self.engine_configs: Dict[str, Any] = {"--log-no-color": "1"}
+        self.keep_alive(True)
 
     def path(self, path: str):
         self._path = path
         return self
 
     def log_path(self, path: str):
         self._log_path = path
@@ -143,34 +176,35 @@
         self._bin_path = path
         return self
 
     def download(self, download: bool):
         self._download = download
         return self
 
+    def keep_alive(self, keep_alive: bool):
+        self._keep_alive = keep_alive
+        return self
+
+    def in_memory(self, in_memory: bool):
+        self.manager_configs["-db-in-memory"] = "1" if in_memory else "0"
+        return self
+
+    def database_path(self, path: str):
+        self.manager_configs["-db-path"] = path
+        self.in_memory(False)
+        return self
+
     def manager_rest_port(self, port: int):
-        self._manager_configs["-rest-port"] = port
+        self.manager_configs["-rest-port"] = port
         return self
 
     def manager_grpc_port(self, port: int):
-        self._manager_configs["-grpc-port"] = port
+        self.manager_configs["-grpc-port"] = port
         return self
 
-    def __get_manager_configs_as_args(self):
-        configs = []
-        for key, value in self._manager_configs.items():
-            configs.append(f"{key}={value}")
-        return configs
-
-    def __get_engine_configs_as_args(self):
-        configs = []
-        for key, value in self._engine_configs.items():
-            configs.append(f"{key}={value}")
-        return configs
-
     def __get_log_path(self, file_name: str) -> Path:
         if self._path is None:
             raise ValueError("no path provided and KASKADA_PATH was not set")
         if self._log_path is None:
             raise ValueError("no log path provided and KASKADA_LOG_PATH was not set")
         log_path = Path("{}/{}".format(self._path, self._log_path)).expanduser()
         if self._name is not None:
@@ -190,91 +224,94 @@
             raise ValueError("no path provided and KASKADA_PATH was not set")
         if self._bin_path is None:
             raise ValueError("no bin path provided and KASKADA_BIN_PATH was not set")
         bin_path = Path("{}/{}".format(self._path, self._bin_path)).expanduser()
         bin_path.mkdir(parents=True, exist_ok=True)
         return bin_path
 
-    def __start(self):
+    def __get_local_services(self) -> Tuple[KaskadaLocalService, KaskadaLocalService]:
         manager_binary_path = (
-            self.__get_binary_path() / self.KASKADA_MANAGER_BIN_NAME_DEFAULT
+            self.__get_binary_path() / KASKADA_MANAGER_BIN_NAME_DEFAULT
         )
         manager_std_err, manager_std_out = self.__get_std_paths("manager")
-        engine_binary_path = (
-            self.__get_binary_path() / self.KASKADA_ENGINE_BIN_NAME_DEFAULT
-        )
+        engine_binary_path = self.__get_binary_path() / KASKADA_ENGINE_BIN_NAME_DEFAULT
         engine_std_err, engine_std_out = self.__get_std_paths("engine")
         engine_command = "serve"
-
-        manager_cmd = [str(manager_binary_path)] + self.__get_manager_configs_as_args()
-        logger.debug(f"Manager start command: {manager_cmd}")
-        engine_cmd = (
-            [str(engine_binary_path)]
-            + self.__get_engine_configs_as_args()
-            + [str(engine_command)]
-        )
-        logger.debug(f"Engine start command: {engine_cmd}")
-        logger.info("Initializing manager process")
-        logger.info(f"Logging manager STDOUT to {manager_std_out.absolute()}")
-        logger.info(f"Logging manager STDERR to {manager_std_err.absolute()}")
-        manager_process = api_utils.run_subprocess(
-            manager_cmd, manager_std_err, manager_std_out
-        )
-        logger.info("Initializing engine process")
-        logger.info(f"Logging engine STDOUT to {engine_std_out.absolute()}")
-        logger.info(f"Logging engine STDERR to {engine_std_err.absolute()}")
-        engine_process = api_utils.run_subprocess(
-            engine_cmd, engine_std_err, engine_std_out
+        manager_service = KaskadaLocalService(
+            "manager",
+            str(manager_binary_path),
+            "",
+            manager_std_err,
+            manager_std_out,
+            self.manager_configs,
+        )
+        engine_service = KaskadaLocalService(
+            "engine",
+            str(engine_binary_path),
+            engine_command,
+            engine_std_err,
+            engine_std_out,
+            self.engine_configs,
         )
-        return (manager_process, engine_process)
+        return (manager_service, engine_service)
 
     def __download_latest_release(self):
         """Downloads the latest release version to the binary path."""
         client = release.ReleaseClient()
         download_path = self.__get_binary_path()
         download_path.mkdir(parents=True, exist_ok=True)
         local_release = client.download_latest_release(
             download_path,
-            self.KASKADA_MANAGER_BIN_NAME_DEFAULT,
-            self.KASKADA_ENGINE_BIN_NAME_DEFAULT,
+            KASKADA_MANAGER_BIN_NAME_DEFAULT,
+            KASKADA_ENGINE_BIN_NAME_DEFAULT,
         )
         logger.debug(f"Download Path: {local_release._download_path}")
         logger.debug(f"Manager Path: {local_release._manager_path}")
         logger.debug(f"Engine Path: {local_release._engine_path}")
         # Update the binary path to the path downloaded and saved to by the latest release downloader.
         self.bin_path(
             local_release._download_path.absolute().relative_to(
                 Path(self._path).expanduser().absolute()
             )
         )
         os.chmod(local_release._manager_path, 0o755)
         os.chmod(local_release._engine_path, 0o755)
 
-    def build(self) -> Session:
+    def build(self) -> LocalSession:
         """Builds the local session. Starts by downloading the latest release and starting the local binaries.
 
         Returns:
-            Session: The local session object
+            LocalSession: The local session object
         """
-        if self._download:
-            self.__download_latest_release()
-        manager_process, engine_process = self.__start()
         if self._endpoint is None:
             raise ValueError("endpoint was not set")
         if self._is_secure is None:
             raise ValueError("is_secure was not set")
 
-        return Session(
+        global KASKADA_SESSION
+        if KASKADA_SESSION is not None and KASKADA_SESSION.client is not None:
+            logger.info("Detected an existing session.")
+            is_ready = KASKADA_SESSION.client.is_ready()
+            if is_ready:
+                logger.info(
+                    "Existing session is available and ready to accept requests. Reusing existing session."
+                )
+                return KASKADA_SESSION
+            else:
+                logger.warn(
+                    "Existing session is no longer available. Creating a new session."
+                )
+
+        if self._download:
+            self.__download_latest_release()
+
+        manager_process, engine_process = self.__get_local_services()
+        session = LocalSession(
             self._endpoint,
             self._is_secure,
+            manager_process,
+            engine_process,
             client_id=self._client_id,
-            manager_process=manager_process,
-            engine_process=engine_process,
         )
-
-
-class RemoteBuilder(Builder):
-    def __init__(self) -> None:
-        super().__init__()
-
-    def build(self):
-        return Session(self._endpoint, self._is_secure, client_id=self._client_id)
+        session.start()
+        KASKADA_SESSION = session
+        return session
```

### Comparing `kaskada-0.2.0/src/kaskada/formatters.css` & `kaskada-0.4.0/src/kaskada/formatters.css`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/formatters.js` & `kaskada-0.4.0/src/kaskada/formatters.js`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/formatters.py` & `kaskada-0.4.0/src/kaskada/formatters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/formatters_helpers.py` & `kaskada-0.4.0/src/kaskada/formatters_helpers.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/formatters_shared.py` & `kaskada-0.4.0/src/kaskada/formatters_shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # pylint: disable=no-member
 import operator
 import pprint
-from typing import Optional
 
-import pandas as pd
-from domonic.html import pre, table, td, th, tr
+from domonic.html import a, pre, table, td, th, tr
 from domonic.utils import Utils
 
+import kaskada.kaskada.v1alpha.fenl_diagnostics_pb2 as fenl_pb
 import kaskada.kaskada.v1alpha.pulsar_pb2 as pulsar_pb
 import kaskada.kaskada.v1alpha.table_service_pb2 as table_pb
 import kaskada.kaskada.v1alpha.view_service_pb2 as view_pb
 
 from .formatters_helpers import (
     appendChildren,
     appendHtmlObjTableRowIfAttrExists,
@@ -57,19 +56,33 @@
         )
         diagnostics, has_errors = get_fenl_diagnostics_html_and_has_errors(
             obj.fenl_diagnostics
         )
     return can_execute, has_errors, details, diagnostics
 
 
+def get_hyperlink(text: str, link: str) -> str:
+    return str(a(text, _href=link, _target="_blank"))
+
+
+def update_diagnostic_with_link(fenl_diag: fenl_pb.FenlDiagnostic) -> str:
+    formatted: str = fenl_diag.formatted
+    web_link: str = fenl_diag.web_link
+    code = fenl_diag.code
+    if len(web_link.strip()) > 0:
+        formatted = formatted.replace(code, get_hyperlink(code, web_link))
+    return formatted
+
+
 def get_fenl_diagnostics_html_and_has_errors(obj):
     diagnostics = table(_class="kda_table")
     for i in range(len(obj.fenl_diagnostics)):
         fenl_diag = obj.fenl_diagnostics[i]
-        diagnostics.appendChild(html_obj_table_row(i, fenl_diag.formatted))
+        rendered_diag = update_diagnostic_with_link(fenl_diag)
+        diagnostics.appendChild(html_obj_table_row(i, rendered_diag))
     return diagnostics, obj.num_errors > 0
 
 
 def get_generic_object_html_and_schema_df(obj):
     props = get_properties(obj)
     obj_type = type(obj).__name__.lower()
```

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/common_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/common_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/compute_service_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/compute_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/destinations_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/destinations_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x12\x17kaskada.kaskada.v1alpha\"\x84\x01\n\x0f\x46\x65nlDiagnostics\x12R\n\x10\x66\x65nl_diagnostics\x18\x01 \x03(\x0b\x32\'.kaskada.kaskada.v1alpha.FenlDiagnosticR\x0f\x66\x65nlDiagnostics\x12\x1d\n\nnum_errors\x18\x02 \x01(\x03R\tnumErrors\"\x9b\x01\n\x0e\x46\x65nlDiagnostic\x12=\n\x08severity\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.SeverityR\x08severity\x12\x12\n\x04\x63ode\x18\x02 \x01(\tR\x04\x63ode\x12\x18\n\x07message\x18\x03 \x01(\tR\x07message\x12\x1c\n\tformatted\x18\x04 \x01(\tR\tformatted*\x86\x01\n\x08Severity\x12\x18\n\x14SEVERITY_UNSPECIFIED\x10\x00\x12\x10\n\x0cSEVERITY_BUG\x10\x01\x12\x12\n\x0eSEVERITY_ERROR\x10\x02\x12\x14\n\x10SEVERITY_WARNING\x10\x03\x12\x11\n\rSEVERITY_NOTE\x10\x04\x12\x11\n\rSEVERITY_HELP\x10\x05\x42\x84\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x14\x46\x65nlDiagnosticsProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x12\x17kaskada.kaskada.v1alpha\"\x84\x01\n\x0f\x46\x65nlDiagnostics\x12R\n\x10\x66\x65nl_diagnostics\x18\x01 \x03(\x0b\x32\'.kaskada.kaskada.v1alpha.FenlDiagnosticR\x0f\x66\x65nlDiagnostics\x12\x1d\n\nnum_errors\x18\x02 \x01(\x03R\tnumErrors\"\xb6\x01\n\x0e\x46\x65nlDiagnostic\x12=\n\x08severity\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.SeverityR\x08severity\x12\x12\n\x04\x63ode\x18\x02 \x01(\tR\x04\x63ode\x12\x18\n\x07message\x18\x03 \x01(\tR\x07message\x12\x1c\n\tformatted\x18\x04 \x01(\tR\tformatted\x12\x19\n\x08web_link\x18\x05 \x01(\tR\x07webLink*\x86\x01\n\x08Severity\x12\x18\n\x14SEVERITY_UNSPECIFIED\x10\x00\x12\x10\n\x0cSEVERITY_BUG\x10\x01\x12\x12\n\x0eSEVERITY_ERROR\x10\x02\x12\x14\n\x10SEVERITY_WARNING\x10\x03\x12\x11\n\rSEVERITY_NOTE\x10\x04\x12\x11\n\rSEVERITY_HELP\x10\x05\x42\x84\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x14\x46\x65nlDiagnosticsProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.fenl_diagnostics_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\024FenlDiagnosticsProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _globals['_SEVERITY']._serialized_start=369
-  _globals['_SEVERITY']._serialized_end=503
+  _globals['_SEVERITY']._serialized_start=396
+  _globals['_SEVERITY']._serialized_end=530
   _globals['_FENLDIAGNOSTICS']._serialized_start=76
   _globals['_FENLDIAGNOSTICS']._serialized_end=208
   _globals['_FENLDIAGNOSTIC']._serialized_start=211
-  _globals['_FENLDIAGNOSTIC']._serialized_end=366
+  _globals['_FENLDIAGNOSTIC']._serialized_end=393
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/file_service_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/file_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/options_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/options_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/plan_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/plan_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/pulsar_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/pulsar_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/query_service_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/schema_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/sources_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/sources_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/spec_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/table_service_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/table_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/test_cases_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/test_cases_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/view_service_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/view_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py` & `kaskada-0.4.0/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v2alpha/query_service_pb2.py` & `kaskada-0.4.0/src/kaskada/kaskada/v2alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py` & `kaskada-0.4.0/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/materialization.py` & `kaskada-0.4.0/src/kaskada/materialization.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/query.py` & `kaskada-0.4.0/src/kaskada/query.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/slice_filters.py` & `kaskada-0.4.0/src/kaskada/slice_filters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/table.py` & `kaskada-0.4.0/src/kaskada/table.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/utils.py` & `kaskada-0.4.0/src/kaskada/utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/src/kaskada/view.py` & `kaskada-0.4.0/src/kaskada/view.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/vendor/validate/validate.proto` & `kaskada-0.4.0/vendor/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/vendor/validate/validate_pb2.py` & `kaskada-0.4.0/vendor/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/vendor/validate/validate_pb2.pyi` & `kaskada-0.4.0/vendor/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kaskada-0.2.0/setup.py` & `kaskada-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,47 +4,51 @@
 package_dir = \
 {'': 'src', 'fenlmagic': 'src/fenlmagic', 'validate': 'vendor/validate'}
 
 packages = \
 ['fenlmagic',
  'kaskada',
  'kaskada.api',
+ 'kaskada.api.local_session',
+ 'kaskada.api.remote_session',
+ 'kaskada.health',
  'kaskada.kaskada.v1alpha',
  'kaskada.kaskada.v2alpha',
  'validate']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['certifi>=2022.12.7,<2023.0.0',
  'domonic>=0.9.11,<0.10.0',
  'googleapis-common-protos>=1.58.0,<2.0.0',
+ 'grpcio-health-checking>=1.54.2,<2.0.0',
  'grpcio-status>=1.51.1,<2.0.0',
  'grpcio>=1.51.1,<2.0.0',
  'html5lib>=1.1,<2.0',
  'ipython==7.34.0',
  'pandas>=1.3,<1.4',
  'pyarrow>=10.0.1,<11.0.0',
  'pygithub>=1.57,<2.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'kaskada',
-    'version': '0.2.0',
+    'version': '0.4.0',
     'description': 'A client library for the Kaskada time travel machine learning service',
     'long_description': '# Kaskada SDK\n\n## Developer Instructions\nThe package uses Poetry to develop and build.\n\n1. Install Pyenv [Pyenv Documentation](https://github.com/pyenv/pyenv)\n1. Install Python 3.9.16: `$ pyenv install 3.9.16`\n1. Install Poetry [Poetry Documentation](https://python-poetry.org/docs/)\n1. Install dependences: `$ poetry install`\n\n### Run tasks\nThe package uses [`poethepoet`](https://github.com/nat-n/poethepoet) for running tasks\n\n#### Test Task\nTo run tests: `$ poetry run poe test` \n\n#### Check Style Task\nTo check the style: `$ poetry run poe style`\n\n#### Format Task\nTo auto-format (isort + black): `$ poetry run poe format`\n\n#### Check Static Type Task\nTo perform static type analysis (mypy): `$ poetry run poe types`\n\n#### Lint Task\nTo run the linter (pylint): `$ poetry run poe lint`\n\n#### Generate documentation \nWe use Sphinx and rely on autogeneration extensions within Sphinx to read docstrings and \ngenerate an HTML formatted version of the codes documentation. \n\n* `poetry run poe docs` : generates and builds the docs \n* `poetry run poe docs-generate` : generates the docs (.rst files)\n* `poetry run poe docs-build` : builds the HTML rendered version of the generated docs (from .rst to .html)\n\nThe generated HTML is located inside `docs/build`. Load `docs/build/index.html` in your browser to see the HTML rendered output. \n\n## Using the Client from Jupyter\n\n#### Install Jupyter\nTo install Jupyter: `$ pip install notebook`\n\n#### Build the Client\nTo build the client: `$ poetry build`\n\n#### Install the Client\nTo install the client: `$ pip install dist/*.whl`\n\n#### Open a Jupyter Notebook\nTo open a notebook: `$ jupyter notebook`\n',
     'author': 'Kaskada',
     'author_email': 'maintainers@kaskada.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7.2,<4.0.0',
+    'python_requires': '>=3.8.2,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `kaskada-0.2.0/PKG-INFO` & `kaskada-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kaskada
-Version: 0.2.0
+Version: 0.4.0
 Summary: A client library for the Kaskada time travel machine learning service
 License: Apache-2.0
 Author: Kaskada
 Author-email: maintainers@kaskada.io
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.8.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
 Requires-Dist: domonic (>=0.9.11,<0.10.0)
 Requires-Dist: googleapis-common-protos (>=1.58.0,<2.0.0)
 Requires-Dist: grpcio (>=1.51.1,<2.0.0)
+Requires-Dist: grpcio-health-checking (>=1.54.2,<2.0.0)
 Requires-Dist: grpcio-status (>=1.51.1,<2.0.0)
 Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: ipython (==7.34.0)
 Requires-Dist: pandas (>=1.3,<1.4)
 Requires-Dist: pyarrow (>=10.0.1,<11.0.0)
 Requires-Dist: pygithub (>=1.57,<2.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
```

