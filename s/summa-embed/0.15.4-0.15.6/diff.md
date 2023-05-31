# Comparing `tmp/summa_embed-0.15.4.tar.gz` & `tmp/summa_embed-0.15.6.tar.gz`

## Comparing `summa_embed-0.15.4.tar` & `summa_embed-0.15.6.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.15.4/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2262 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10419 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7125 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2353 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      424 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 summa_embed-0.15.4/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20       92 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7087 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5015 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20     1021 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/driver.rs
--rw-r--r--   0      501       20    13794 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    24562 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13833 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    14335 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5038 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     4711 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      163 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20    15871 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1595 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    56532 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     2216 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11274 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7439 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     3093 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8014 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5490 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      450 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 summa_embed-0.15.4/Cargo.toml
--rw-r--r--   0      501       20      685 2023-05-31 08:41:21.000000 summa_embed-0.15.4/.gitignore
--rwxr-xr-x   0      501       20      347 2023-05-31 08:41:21.000000 summa_embed-0.15.4/build.sh
--rw-r--r--   0      501       20      515 2023-05-31 08:41:21.000000 summa_embed-0.15.4/pyproject.toml
--rw-r--r--   0      501       20       14 2023-05-31 08:41:21.000000 summa_embed-0.15.4/requirements.txt
--rw-r--r--   0      501       20     4333 2023-05-31 08:41:21.000000 summa_embed-0.15.4/src/lib.rs
--rw-r--r--   0      501       20     1050 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/__init__.py
--rw-r--r--   0      501       20        0 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/__init__.py
--rw-r--r--   0      501       20     3123 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/consumer_service_pb2.py
--rw-r--r--   0      501       20     3080 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/consumer_service_pb2.pyi
--rw-r--r--   0      501       20     1335 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/dag_pb_pb2.py
--rw-r--r--   0      501       20     1042 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/dag_pb_pb2.pyi
--rw-r--r--   0      501       20    16230 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/index_service_pb2.py
--rw-r--r--   0      501       20    19481 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/index_service_pb2.pyi
--rw-r--r--   0      501       20    21461 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/query_pb2.py
--rw-r--r--   0      501       20    29337 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/query_pb2.pyi
--rw-r--r--   0      501       20     2213 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/reflection_service_pb2.py
--rw-r--r--   0      501       20     1923 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/reflection_service_pb2.pyi
--rw-r--r--   0      501       20     2012 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/search_service_pb2.py
--rw-r--r--   0      501       20     1830 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/search_service_pb2.pyi
--rw-r--r--   0      501       20     1741 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/unixfs_pb2.py
--rw-r--r--   0      501       20     1598 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/unixfs_pb2.pyi
--rw-r--r--   0      501       20     1040 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/utils_pb2.py
--rw-r--r--   0      501       20      454 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/utils_pb2.pyi
--rw-r--r--   0      501       20   102226 2023-05-31 08:43:47.000000 summa_embed-0.15.4/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.15.4/PKG-INFO
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.15.6/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2262 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10419 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7125 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2353 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      424 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 summa_embed-0.15.6/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20       92 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7087 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5015 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20     1021 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/driver.rs
+-rw-r--r--   0      501       20    13794 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    24562 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13833 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    14335 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5038 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     4711 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      163 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20    15871 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1595 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    56532 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     2216 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11274 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7439 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     3093 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8014 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5490 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      450 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 summa_embed-0.15.6/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-05-31 10:09:34.000000 summa_embed-0.15.6/.gitignore
+-rwxr-xr-x   0      501       20      347 2023-05-31 10:09:34.000000 summa_embed-0.15.6/build.sh
+-rw-r--r--   0      501       20      515 2023-05-31 10:09:35.000000 summa_embed-0.15.6/pyproject.toml
+-rw-r--r--   0      501       20       14 2023-05-31 10:09:35.000000 summa_embed-0.15.6/requirements.txt
+-rw-r--r--   0      501       20     4331 2023-05-31 10:09:35.000000 summa_embed-0.15.6/src/lib.rs
+-rw-r--r--   0      501       20     1050 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/__init__.py
+-rw-r--r--   0      501       20        0 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/__init__.py
+-rw-r--r--   0      501       20     3124 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/consumer_service_pb2.py
+-rw-r--r--   0      501       20     3153 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/consumer_service_pb2.pyi
+-rw-r--r--   0      501       20     1336 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/dag_pb_pb2.py
+-rw-r--r--   0      501       20     1115 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/dag_pb_pb2.pyi
+-rw-r--r--   0      501       20    16689 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/index_service_pb2.py
+-rw-r--r--   0      501       20    20021 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/index_service_pb2.pyi
+-rw-r--r--   0      501       20    21461 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/query_pb2.py
+-rw-r--r--   0      501       20    29410 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/query_pb2.pyi
+-rw-r--r--   0      501       20     2214 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/reflection_service_pb2.py
+-rw-r--r--   0      501       20     1996 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/reflection_service_pb2.pyi
+-rw-r--r--   0      501       20     2012 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/search_service_pb2.py
+-rw-r--r--   0      501       20     1903 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/search_service_pb2.pyi
+-rw-r--r--   0      501       20     1742 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/unixfs_pb2.py
+-rw-r--r--   0      501       20     1653 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/unixfs_pb2.pyi
+-rw-r--r--   0      501       20     1041 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/utils_pb2.py
+-rw-r--r--   0      501       20      455 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/utils_pb2.pyi
+-rw-r--r--   0      501       20   102226 2023-05-31 10:09:55.000000 summa_embed-0.15.6/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.15.6/PKG-INFO
```

### Comparing `summa_embed-0.15.4/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.15.6/local_dependencies/summa-proto/Cargo.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.15.6/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-proto/build.rs` & `summa_embed-0.15.6/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.15.6/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.15.6/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.15.6/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.15.6/local_dependencies/summa-proto/proto/query.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.15.6/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.15.6/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.15.6/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.15.6/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.15.6/local_dependencies/summa-core/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.15.5"
+version = "0.15.6"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
```

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/LICENSE` & `summa_embed-0.15.6/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/driver.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/driver.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.15.6/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/Cargo.toml` & `summa_embed-0.15.6/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "summa-embed-py"
-version = "0.15.4"
+version = "0.15.6"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
 
 [dependencies]
 futures = "0.3"
 prost = "0.11"
 pyo3 = { version = "0.18", features = ["serde"] }
 pyo3-asyncio = { version =  "0.18", features = ["attributes", "tokio-runtime"] }
 pythonize = "0.18"
 serde_json = "1.0"
-summa-core = { version = "0.15.5", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.15.6", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.15.4/.gitignore` & `summa_embed-0.15.6/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/pyproject.toml` & `summa_embed-0.15.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.4/src/lib.rs` & `summa_embed-0.15.6/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use std::sync::Arc;
 
 use futures::future::join_all;
 use prost::Message;
 use pyo3::exceptions::PyOSError;
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
-use pythonize::{pythonize};
+use pythonize::pythonize;
 use summa_core::components::{Driver, IndexHolder};
 use summa_core::configs::{ConfigProxy, DirectProxy};
 use summa_core::directories::DefaultExternalRequestGenerator;
 use summa_core::hyper_external_request::HyperExternalRequest;
 use summa_proto::proto;
 use tantivy::IndexBuilder;
```

### Comparing `summa_embed-0.15.4/summa_embed/__init__.py` & `summa_embed-0.15.6/summa_embed/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Optional, Dict
+from typing import Dict, Optional
 
 from izihawa_utils.pb_to_json import ParseDict
 
-from .summa_embed_bin import IndexRegistry
 from .proto import search_service_pb2 as search_service_pb
+from .summa_embed_bin import IndexRegistry
 
 
 class SummaEmbed:
     def __init__(self):
         self.index_registry = IndexRegistry()
 
     def add(self, index_config, index_name: Optional[str] = None):
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/consumer_service_pb2.py` & `summa_embed-0.15.6/summa_embed/proto/consumer_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: consumer_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/consumer_service_pb2.pyi` & `summa_embed-0.15.6/summa_embed/proto/consumer_service_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-from google.protobuf.internal import containers as _containers
+from typing import ClassVar as _ClassVar
+from typing import Iterable as _Iterable
+from typing import Mapping as _Mapping
+from typing import Optional as _Optional
+from typing import Union as _Union
+
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from google.protobuf.internal import containers as _containers
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Consumer(_message.Message):
     __slots__ = ["consumer_name", "index_name"]
     CONSUMER_NAME_FIELD_NUMBER: _ClassVar[int]
     INDEX_NAME_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/dag_pb_pb2.py` & `summa_embed-0.15.6/summa_embed/proto/dag_pb_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: dag_pb.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/dag_pb_pb2.pyi` & `summa_embed-0.15.6/summa_embed/proto/dag_pb_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-from google.protobuf.internal import containers as _containers
+from typing import ClassVar as _ClassVar
+from typing import Iterable as _Iterable
+from typing import Mapping as _Mapping
+from typing import Optional as _Optional
+from typing import Union as _Union
+
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from google.protobuf.internal import containers as _containers
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class PBLink(_message.Message):
     __slots__ = ["hash", "name", "t_size"]
     HASH_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/index_service_pb2.py` & `summa_embed-0.15.6/summa_embed/proto/index_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: index_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import query_pb2 as query__pb2
 from . import utils_pb2 as utils__pb2
 
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13index_service.proto\x12\x0bsumma.proto\x1a\x0bquery.proto\x1a\x0butils.proto\"3\n\nPrimaryKey\x12\r\n\x03str\x18\x01 \x01(\tH\x00\x12\r\n\x03i64\x18\x02 \x01(\x03H\x00\x42\x07\n\x05value\"\x7f\n\x0bMergePolicy\x12*\n\x03log\x18\x0b \x01(\x0b\x32\x1b.summa.proto.LogMergePolicyH\x00\x12\x34\n\x08temporal\x18\x0c \x01(\x0b\x32 .summa.proto.TemporalMergePolicyH\x00\x42\x0e\n\x0cmerge_policy\"\x19\n\x17\x41ttachFileEngineRequest\"L\n\x19\x41ttachRemoteEngineRequest\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1f.summa.proto.RemoteEngineConfig\"\xd8\x01\n\x12\x41ttachIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x34\n\x04\x66ile\x18\x02 \x01(\x0b\x32$.summa.proto.AttachFileEngineRequestH\x00\x12\x38\n\x06remote\x18\x03 \x01(\x0b\x32&.summa.proto.AttachRemoteEngineRequestH\x00\x12.\n\x0cmerge_policy\x18\n \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x0e\n\x0cindex_engine\"C\n\x13\x41ttachIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"(\n\x12\x43ommitIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"+\n\x13\x43ommitIndexResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\"L\n\x14\x43opyDocumentsRequest\x12\x19\n\x11source_index_name\x18\x01 \x01(\t\x12\x19\n\x11target_index_name\x18\x02 \x01(\t\"G\n\x15\x43opyDocumentsResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x18\n\x10\x63opied_documents\x18\x02 \x01(\r\"\xff\x01\n\x10\x43opyIndexRequest\x12\x19\n\x11source_index_name\x18\x01 \x01(\t\x12\x19\n\x11target_index_name\x18\x02 \x01(\t\x12\x34\n\x04\x66ile\x18\x03 \x01(\x0b\x32$.summa.proto.CreateFileEngineRequestH\x00\x12\x38\n\x06memory\x18\x04 \x01(\x0b\x32&.summa.proto.CreateMemoryEngineRequestH\x00\x12.\n\x0cmerge_policy\x18\x06 \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x15\n\x13target_index_engine\"A\n\x11\x43opyIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"?\n\x0bSortByField\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12!\n\x05order\x18\x02 \x01(\x0e\x32\x12.summa.proto.Order\"\x19\n\x17\x43reateFileEngineRequest\"\x1b\n\x19\x43reateMemoryEngineRequest\"\xa0\x02\n\x0fIndexAttributes\x12\x12\n\ncreated_at\x18\x01 \x01(\x04\x12\x15\n\runique_fields\x18\x02 \x03(\t\x12\x16\n\x0e\x64\x65\x66\x61ult_fields\x18\x03 \x03(\t\x12\x14\n\x0cmulti_fields\x18\x04 \x03(\t\x12\x1f\n\x12\x64\x65\x66\x61ult_index_name\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x06 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x10\x64\x65\x66\x61ult_snippets\x18\x07 \x03(\t\x12\x38\n\x11\x63onflict_strategy\x18\x08 \x01(\x0e\x32\x1d.summa.proto.ConflictStrategyB\x15\n\x13_default_index_nameB\x0e\n\x0c_description\"\xbd\x03\n\x12\x43reateIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x34\n\x04\x66ile\x18\x07 \x01(\x0b\x32$.summa.proto.CreateFileEngineRequestH\x00\x12\x38\n\x06memory\x18\x08 \x01(\x0b\x32&.summa.proto.CreateMemoryEngineRequestH\x00\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12-\n\x0b\x63ompression\x18\x03 \x01(\x0e\x32\x18.summa.proto.Compression\x12\x16\n\tblocksize\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x34\n\rsort_by_field\x18\x05 \x01(\x0b\x32\x18.summa.proto.SortByFieldH\x02\x88\x01\x01\x12\x36\n\x10index_attributes\x18\x06 \x01(\x0b\x32\x1c.summa.proto.IndexAttributes\x12.\n\x0cmerge_policy\x18\x14 \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x0e\n\x0cindex_engineB\x0c\n\n_blocksizeB\x10\n\x0e_sort_by_field\"C\n\x13\x43reateIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"O\n\x16\x44\x65leteDocumentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12!\n\x05query\x18\x02 \x01(\x0b\x32\x12.summa.proto.Query\"4\n\x17\x44\x65leteDocumentsResponse\x12\x19\n\x11\x64\x65leted_documents\x18\x01 \x01(\x04\"(\n\x12\x44\x65leteIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"1\n\x13\x44\x65leteIndexResponse\x12\x1a\n\x12\x64\x65leted_index_name\x18\x01 \x01(\t\"\x1a\n\x18GetIndicesAliasesRequest\"\xa7\x01\n\x19GetIndicesAliasesResponse\x12S\n\x0findices_aliases\x18\x01 \x03(\x0b\x32:.summa.proto.GetIndicesAliasesResponse.IndicesAliasesEntry\x1a\x35\n\x13IndicesAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"%\n\x0fGetIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"@\n\x10GetIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"\x13\n\x11GetIndicesRequest\")\n\x12GetIndicesResponse\x12\x13\n\x0bindex_names\x18\x01 \x03(\t\"C\n\x1aIndexDocumentStreamRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x11\n\tdocuments\x18\x02 \x03(\x0c\"^\n\x1bIndexDocumentStreamResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x14\n\x0csuccess_docs\x18\x02 \x01(\x04\x12\x13\n\x0b\x66\x61iled_docs\x18\x03 \x01(\x04\"<\n\x14IndexDocumentRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocument\x18\x02 \x01(\x0c\"\x17\n\x15IndexDocumentResponse\"?\n\x14MergeSegmentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x13\n\x0bsegment_ids\x18\x02 \x03(\t\"?\n\x15MergeSegmentsResponse\x12\x17\n\nsegment_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_segment_id\"?\n\x14SetIndexAliasRequest\x12\x13\n\x0bindex_alias\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"G\n\x15SetIndexAliasResponse\x12\x1b\n\x0eold_index_name\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x11\n\x0f_old_index_name\"6\n\x10\x44ocumentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"%\n\x11\x44ocumentsResponse\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\"C\n\x12VacuumIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x19\n\x11\x65xcluded_segments\x18\x02 \x03(\t\"0\n\x13VacuumIndexResponse\x12\x19\n\x11\x66reed_space_bytes\x18\x01 \x01(\x04\"9\n\x12WarmupIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0f\n\x07is_full\x18\x02 \x01(\x08\"+\n\x13WarmupIndexResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\" \n\x10\x46ileEngineConfig\x12\x0c\n\x04path\x18\x01 \x01(\t\"$\n\x12MemoryEngineConfig\x12\x0e\n\x06schema\x18\x01 \x01(\t\"!\n\x0b\x43\x61\x63heConfig\x12\x12\n\ncache_size\x18\x01 \x01(\x04\"\x9a\x02\n\x12RemoteEngineConfig\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x14\n\x0curl_template\x18\x02 \x01(\t\x12N\n\x10headers_template\x18\x03 \x03(\x0b\x32\x34.summa.proto.RemoteEngineConfig.HeadersTemplateEntry\x12.\n\x0c\x63\x61\x63he_config\x18\x04 \x01(\x0b\x32\x18.summa.proto.CacheConfig\x12\x17\n\ntimeout_ms\x18\x05 \x01(\rH\x00\x88\x01\x01\x1a\x36\n\x14HeadersTemplateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\r\n\x0b_timeout_ms\"#\n\x0eLogMergePolicy\x12\x11\n\tis_frozen\x18\x01 \x01(\x08\"4\n\x13TemporalMergePolicy\x12\x1d\n\x15merge_older_then_secs\x18\x01 \x01(\x04\"\xe2\x01\n\x11IndexEngineConfig\x12-\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x1d.summa.proto.FileEngineConfigH\x00\x12\x31\n\x06memory\x18\x02 \x01(\x0b\x32\x1f.summa.proto.MemoryEngineConfigH\x00\x12\x31\n\x06remote\x18\x03 \x01(\x0b\x32\x1f.summa.proto.RemoteEngineConfigH\x00\x12.\n\x0cmerge_policy\x18\n \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x08\n\x06\x63onfig\"\xec\x01\n\x10IndexDescription\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x15\n\rindex_aliases\x18\x02 \x03(\t\x12\x34\n\x0cindex_engine\x18\x03 \x01(\x0b\x32\x1e.summa.proto.IndexEngineConfig\x12\x10\n\x08num_docs\x18\x04 \x01(\x04\x12-\n\x0b\x63ompression\x18\x05 \x01(\x0e\x32\x18.summa.proto.Compression\x12\x36\n\x10index_attributes\x18\x06 \x01(\x0b\x32\x1c.summa.proto.IndexAttributes\"*\n\x16IndexDocumentOperation\x12\x10\n\x08\x64ocument\x18\x01 \x01(\x0c\"\\\n\x0eIndexOperation\x12=\n\x0eindex_document\x18\x02 \x01(\x0b\x32#.summa.proto.IndexDocumentOperationH\x00\x42\x0b\n\toperation*R\n\x10\x43onflictStrategy\x12\x0e\n\nDO_NOTHING\x10\x00\x12\x14\n\x10OVERWRITE_ALWAYS\x10\x01\x12\r\n\tOVERWRITE\x10\x02\x12\t\n\x05MERGE\x10\x03*|\n\x0b\x43ompression\x12\x08\n\x04None\x10\x00\x12\n\n\x06\x42rotli\x10\x01\x12\x07\n\x03Lz4\x10\x02\x12\n\n\x06Snappy\x10\x03\x12\x08\n\x04Zstd\x10\x04\x12\t\n\x05Zstd7\x10\x05\x12\t\n\x05Zstd9\x10\x06\x12\n\n\x06Zstd14\x10\x07\x12\n\n\x06Zstd19\x10\x08\x12\n\n\x06Zstd22\x10\t2\xeb\x0b\n\x08IndexApi\x12S\n\x0c\x61ttach_index\x12\x1f.summa.proto.AttachIndexRequest\x1a .summa.proto.AttachIndexResponse\"\x00\x12S\n\x0c\x63ommit_index\x12\x1f.summa.proto.CommitIndexRequest\x1a .summa.proto.CommitIndexResponse\"\x00\x12Y\n\x0e\x63opy_documents\x12!.summa.proto.CopyDocumentsRequest\x1a\".summa.proto.CopyDocumentsResponse\"\x00\x12S\n\x0c\x63reate_index\x12\x1f.summa.proto.CreateIndexRequest\x1a .summa.proto.CreateIndexResponse\"\x00\x12M\n\ncopy_index\x12\x1d.summa.proto.CopyIndexRequest\x1a\x1e.summa.proto.CopyIndexResponse\"\x00\x12_\n\x10\x64\x65lete_documents\x12#.summa.proto.DeleteDocumentsRequest\x1a$.summa.proto.DeleteDocumentsResponse\"\x00\x12S\n\x0c\x64\x65lete_index\x12\x1f.summa.proto.DeleteIndexRequest\x1a .summa.proto.DeleteIndexResponse\"\x00\x12N\n\tdocuments\x12\x1d.summa.proto.DocumentsRequest\x1a\x1e.summa.proto.DocumentsResponse\"\x00\x30\x01\x12\x66\n\x13get_indices_aliases\x12%.summa.proto.GetIndicesAliasesRequest\x1a&.summa.proto.GetIndicesAliasesResponse\"\x00\x12J\n\tget_index\x12\x1c.summa.proto.GetIndexRequest\x1a\x1d.summa.proto.GetIndexResponse\"\x00\x12P\n\x0bget_indices\x12\x1e.summa.proto.GetIndicesRequest\x1a\x1f.summa.proto.GetIndicesResponse\"\x00\x12n\n\x15index_document_stream\x12\'.summa.proto.IndexDocumentStreamRequest\x1a(.summa.proto.IndexDocumentStreamResponse\"\x00(\x01\x12Y\n\x0eindex_document\x12!.summa.proto.IndexDocumentRequest\x1a\".summa.proto.IndexDocumentResponse\"\x00\x12Y\n\x0emerge_segments\x12!.summa.proto.MergeSegmentsRequest\x1a\".summa.proto.MergeSegmentsResponse\"\x00\x12Z\n\x0fset_index_alias\x12!.summa.proto.SetIndexAliasRequest\x1a\".summa.proto.SetIndexAliasResponse\"\x00\x12S\n\x0cvacuum_index\x12\x1f.summa.proto.VacuumIndexRequest\x1a .summa.proto.VacuumIndexResponse\"\x00\x12S\n\x0cwarmup_index\x12\x1f.summa.proto.WarmupIndexRequest\x1a .summa.proto.WarmupIndexResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13index_service.proto\x12\x0bsumma.proto\x1a\x0bquery.proto\x1a\x0butils.proto\"3\n\nPrimaryKey\x12\r\n\x03str\x18\x01 \x01(\tH\x00\x12\r\n\x03i64\x18\x02 \x01(\x03H\x00\x42\x07\n\x05value\"\x7f\n\x0bMergePolicy\x12*\n\x03log\x18\x0b \x01(\x0b\x32\x1b.summa.proto.LogMergePolicyH\x00\x12\x34\n\x08temporal\x18\x0c \x01(\x0b\x32 .summa.proto.TemporalMergePolicyH\x00\x42\x0e\n\x0cmerge_policy\"\x19\n\x17\x41ttachFileEngineRequest\"L\n\x19\x41ttachRemoteEngineRequest\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1f.summa.proto.RemoteEngineConfig\"\xd8\x01\n\x12\x41ttachIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x34\n\x04\x66ile\x18\x02 \x01(\x0b\x32$.summa.proto.AttachFileEngineRequestH\x00\x12\x38\n\x06remote\x18\x03 \x01(\x0b\x32&.summa.proto.AttachRemoteEngineRequestH\x00\x12.\n\x0cmerge_policy\x18\n \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x0e\n\x0cindex_engine\"C\n\x13\x41ttachIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"(\n\x12\x43ommitIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"+\n\x13\x43ommitIndexResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\"L\n\x14\x43opyDocumentsRequest\x12\x19\n\x11source_index_name\x18\x01 \x01(\t\x12\x19\n\x11target_index_name\x18\x02 \x01(\t\"G\n\x15\x43opyDocumentsResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x18\n\x10\x63opied_documents\x18\x02 \x01(\r\"\xff\x01\n\x10\x43opyIndexRequest\x12\x19\n\x11source_index_name\x18\x01 \x01(\t\x12\x19\n\x11target_index_name\x18\x02 \x01(\t\x12\x34\n\x04\x66ile\x18\x03 \x01(\x0b\x32$.summa.proto.CreateFileEngineRequestH\x00\x12\x38\n\x06memory\x18\x04 \x01(\x0b\x32&.summa.proto.CreateMemoryEngineRequestH\x00\x12.\n\x0cmerge_policy\x18\x06 \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x15\n\x13target_index_engine\"A\n\x11\x43opyIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"?\n\x0bSortByField\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12!\n\x05order\x18\x02 \x01(\x0e\x32\x12.summa.proto.Order\"\x19\n\x17\x43reateFileEngineRequest\"\x1b\n\x19\x43reateMemoryEngineRequest\"\xa0\x02\n\x0fIndexAttributes\x12\x12\n\ncreated_at\x18\x01 \x01(\x04\x12\x15\n\runique_fields\x18\x02 \x03(\t\x12\x16\n\x0e\x64\x65\x66\x61ult_fields\x18\x03 \x03(\t\x12\x14\n\x0cmulti_fields\x18\x04 \x03(\t\x12\x1f\n\x12\x64\x65\x66\x61ult_index_name\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x06 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x10\x64\x65\x66\x61ult_snippets\x18\x07 \x03(\t\x12\x38\n\x11\x63onflict_strategy\x18\x08 \x01(\x0e\x32\x1d.summa.proto.ConflictStrategyB\x15\n\x13_default_index_nameB\x0e\n\x0c_description\"\xbd\x03\n\x12\x43reateIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x34\n\x04\x66ile\x18\x07 \x01(\x0b\x32$.summa.proto.CreateFileEngineRequestH\x00\x12\x38\n\x06memory\x18\x08 \x01(\x0b\x32&.summa.proto.CreateMemoryEngineRequestH\x00\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12-\n\x0b\x63ompression\x18\x03 \x01(\x0e\x32\x18.summa.proto.Compression\x12\x16\n\tblocksize\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x34\n\rsort_by_field\x18\x05 \x01(\x0b\x32\x18.summa.proto.SortByFieldH\x02\x88\x01\x01\x12\x36\n\x10index_attributes\x18\x06 \x01(\x0b\x32\x1c.summa.proto.IndexAttributes\x12.\n\x0cmerge_policy\x18\x14 \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x0e\n\x0cindex_engineB\x0c\n\n_blocksizeB\x10\n\x0e_sort_by_field\"C\n\x13\x43reateIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"O\n\x16\x44\x65leteDocumentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12!\n\x05query\x18\x02 \x01(\x0b\x32\x12.summa.proto.Query\"4\n\x17\x44\x65leteDocumentsResponse\x12\x19\n\x11\x64\x65leted_documents\x18\x01 \x01(\x04\"(\n\x12\x44\x65leteIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"1\n\x13\x44\x65leteIndexResponse\x12\x1a\n\x12\x64\x65leted_index_name\x18\x01 \x01(\t\"\x1a\n\x18GetIndicesAliasesRequest\"\xa7\x01\n\x19GetIndicesAliasesResponse\x12S\n\x0findices_aliases\x18\x01 \x03(\x0b\x32:.summa.proto.GetIndicesAliasesResponse.IndicesAliasesEntry\x1a\x35\n\x13IndicesAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"%\n\x0fGetIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"@\n\x10GetIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"\x13\n\x11GetIndicesRequest\")\n\x12GetIndicesResponse\x12\x13\n\x0bindex_names\x18\x01 \x03(\t\"C\n\x1aIndexDocumentStreamRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x11\n\tdocuments\x18\x02 \x03(\x0c\"^\n\x1bIndexDocumentStreamResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x14\n\x0csuccess_docs\x18\x02 \x01(\x04\x12\x13\n\x0b\x66\x61iled_docs\x18\x03 \x01(\x04\"<\n\x14IndexDocumentRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocument\x18\x02 \x01(\x0c\"\x17\n\x15IndexDocumentResponse\"?\n\x14MergeSegmentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x13\n\x0bsegment_ids\x18\x02 \x03(\t\"?\n\x15MergeSegmentsResponse\x12\x17\n\nsegment_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_segment_id\"?\n\x14SetIndexAliasRequest\x12\x13\n\x0bindex_alias\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"G\n\x15SetIndexAliasResponse\x12\x1b\n\x0eold_index_name\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x11\n\x0f_old_index_name\"6\n\x10\x44ocumentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"%\n\x11\x44ocumentsResponse\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\"C\n\x12VacuumIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x19\n\x11\x65xcluded_segments\x18\x02 \x03(\t\"0\n\x13VacuumIndexResponse\x12\x19\n\x11\x66reed_space_bytes\x18\x01 \x01(\x04\"9\n\x12WarmupIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0f\n\x07is_full\x18\x02 \x01(\x08\"+\n\x13WarmupIndexResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\" \n\x10\x46ileEngineConfig\x12\x0c\n\x04path\x18\x01 \x01(\t\"$\n\x12MemoryEngineConfig\x12\x0e\n\x06schema\x18\x01 \x01(\t\"!\n\x0b\x43\x61\x63heConfig\x12\x12\n\ncache_size\x18\x01 \x01(\x04\"\x9a\x02\n\x12RemoteEngineConfig\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x14\n\x0curl_template\x18\x02 \x01(\t\x12N\n\x10headers_template\x18\x03 \x03(\x0b\x32\x34.summa.proto.RemoteEngineConfig.HeadersTemplateEntry\x12.\n\x0c\x63\x61\x63he_config\x18\x04 \x01(\x0b\x32\x18.summa.proto.CacheConfig\x12\x17\n\ntimeout_ms\x18\x05 \x01(\rH\x00\x88\x01\x01\x1a\x36\n\x14HeadersTemplateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\r\n\x0b_timeout_ms\"#\n\x0eLogMergePolicy\x12\x11\n\tis_frozen\x18\x01 \x01(\x08\"4\n\x13TemporalMergePolicy\x12\x1d\n\x15merge_older_then_secs\x18\x01 \x01(\x04\"\xe0\x02\n\x11IndexEngineConfig\x12-\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x1d.summa.proto.FileEngineConfigH\x00\x12\x31\n\x06memory\x18\x02 \x01(\x0b\x32\x1f.summa.proto.MemoryEngineConfigH\x00\x12\x31\n\x06remote\x18\x03 \x01(\x0b\x32\x1f.summa.proto.RemoteEngineConfigH\x00\x12.\n\x0cmerge_policy\x18\n \x01(\x0b\x32\x18.summa.proto.MergePolicy\x12G\n\rfield_aliases\x18\x0b \x03(\x0b\x32\x30.summa.proto.IndexEngineConfig.FieldAliasesEntry\x1a\x33\n\x11\x46ieldAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x08\n\x06\x63onfig\"\xec\x01\n\x10IndexDescription\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x15\n\rindex_aliases\x18\x02 \x03(\t\x12\x34\n\x0cindex_engine\x18\x03 \x01(\x0b\x32\x1e.summa.proto.IndexEngineConfig\x12\x10\n\x08num_docs\x18\x04 \x01(\x04\x12-\n\x0b\x63ompression\x18\x05 \x01(\x0e\x32\x18.summa.proto.Compression\x12\x36\n\x10index_attributes\x18\x06 \x01(\x0b\x32\x1c.summa.proto.IndexAttributes\"*\n\x16IndexDocumentOperation\x12\x10\n\x08\x64ocument\x18\x01 \x01(\x0c\"\\\n\x0eIndexOperation\x12=\n\x0eindex_document\x18\x02 \x01(\x0b\x32#.summa.proto.IndexDocumentOperationH\x00\x42\x0b\n\toperation*R\n\x10\x43onflictStrategy\x12\x0e\n\nDO_NOTHING\x10\x00\x12\x14\n\x10OVERWRITE_ALWAYS\x10\x01\x12\r\n\tOVERWRITE\x10\x02\x12\t\n\x05MERGE\x10\x03*|\n\x0b\x43ompression\x12\x08\n\x04None\x10\x00\x12\n\n\x06\x42rotli\x10\x01\x12\x07\n\x03Lz4\x10\x02\x12\n\n\x06Snappy\x10\x03\x12\x08\n\x04Zstd\x10\x04\x12\t\n\x05Zstd7\x10\x05\x12\t\n\x05Zstd9\x10\x06\x12\n\n\x06Zstd14\x10\x07\x12\n\n\x06Zstd19\x10\x08\x12\n\n\x06Zstd22\x10\t2\xeb\x0b\n\x08IndexApi\x12S\n\x0c\x61ttach_index\x12\x1f.summa.proto.AttachIndexRequest\x1a .summa.proto.AttachIndexResponse\"\x00\x12S\n\x0c\x63ommit_index\x12\x1f.summa.proto.CommitIndexRequest\x1a .summa.proto.CommitIndexResponse\"\x00\x12Y\n\x0e\x63opy_documents\x12!.summa.proto.CopyDocumentsRequest\x1a\".summa.proto.CopyDocumentsResponse\"\x00\x12S\n\x0c\x63reate_index\x12\x1f.summa.proto.CreateIndexRequest\x1a .summa.proto.CreateIndexResponse\"\x00\x12M\n\ncopy_index\x12\x1d.summa.proto.CopyIndexRequest\x1a\x1e.summa.proto.CopyIndexResponse\"\x00\x12_\n\x10\x64\x65lete_documents\x12#.summa.proto.DeleteDocumentsRequest\x1a$.summa.proto.DeleteDocumentsResponse\"\x00\x12S\n\x0c\x64\x65lete_index\x12\x1f.summa.proto.DeleteIndexRequest\x1a .summa.proto.DeleteIndexResponse\"\x00\x12N\n\tdocuments\x12\x1d.summa.proto.DocumentsRequest\x1a\x1e.summa.proto.DocumentsResponse\"\x00\x30\x01\x12\x66\n\x13get_indices_aliases\x12%.summa.proto.GetIndicesAliasesRequest\x1a&.summa.proto.GetIndicesAliasesResponse\"\x00\x12J\n\tget_index\x12\x1c.summa.proto.GetIndexRequest\x1a\x1d.summa.proto.GetIndexResponse\"\x00\x12P\n\x0bget_indices\x12\x1e.summa.proto.GetIndicesRequest\x1a\x1f.summa.proto.GetIndicesResponse\"\x00\x12n\n\x15index_document_stream\x12\'.summa.proto.IndexDocumentStreamRequest\x1a(.summa.proto.IndexDocumentStreamResponse\"\x00(\x01\x12Y\n\x0eindex_document\x12!.summa.proto.IndexDocumentRequest\x1a\".summa.proto.IndexDocumentResponse\"\x00\x12Y\n\x0emerge_segments\x12!.summa.proto.MergeSegmentsRequest\x1a\".summa.proto.MergeSegmentsResponse\"\x00\x12Z\n\x0fset_index_alias\x12!.summa.proto.SetIndexAliasRequest\x1a\".summa.proto.SetIndexAliasResponse\"\x00\x12S\n\x0cvacuum_index\x12\x1f.summa.proto.VacuumIndexRequest\x1a .summa.proto.VacuumIndexResponse\"\x00\x12S\n\x0cwarmup_index\x12\x1f.summa.proto.WarmupIndexRequest\x1a .summa.proto.WarmupIndexResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'index_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._options = None
   _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_options = b'8\001'
   _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._options = None
   _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_options = b'8\001'
-  _CONFLICTSTRATEGY._serialized_start=4651
-  _CONFLICTSTRATEGY._serialized_end=4733
-  _COMPRESSION._serialized_start=4735
-  _COMPRESSION._serialized_end=4859
+  _INDEXENGINECONFIG_FIELDALIASESENTRY._options = None
+  _INDEXENGINECONFIG_FIELDALIASESENTRY._serialized_options = b'8\001'
+  _CONFLICTSTRATEGY._serialized_start=4777
+  _CONFLICTSTRATEGY._serialized_end=4859
+  _COMPRESSION._serialized_start=4861
+  _COMPRESSION._serialized_end=4985
   _PRIMARYKEY._serialized_start=62
   _PRIMARYKEY._serialized_end=113
   _MERGEPOLICY._serialized_start=115
   _MERGEPOLICY._serialized_end=242
   _ATTACHFILEENGINEREQUEST._serialized_start=244
   _ATTACHFILEENGINEREQUEST._serialized_end=269
   _ATTACHREMOTEENGINEREQUEST._serialized_start=271
@@ -127,17 +129,19 @@
   _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_start=3883
   _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_end=3937
   _LOGMERGEPOLICY._serialized_start=3954
   _LOGMERGEPOLICY._serialized_end=3989
   _TEMPORALMERGEPOLICY._serialized_start=3991
   _TEMPORALMERGEPOLICY._serialized_end=4043
   _INDEXENGINECONFIG._serialized_start=4046
-  _INDEXENGINECONFIG._serialized_end=4272
-  _INDEXDESCRIPTION._serialized_start=4275
-  _INDEXDESCRIPTION._serialized_end=4511
-  _INDEXDOCUMENTOPERATION._serialized_start=4513
-  _INDEXDOCUMENTOPERATION._serialized_end=4555
-  _INDEXOPERATION._serialized_start=4557
-  _INDEXOPERATION._serialized_end=4649
-  _INDEXAPI._serialized_start=4862
-  _INDEXAPI._serialized_end=6377
+  _INDEXENGINECONFIG._serialized_end=4398
+  _INDEXENGINECONFIG_FIELDALIASESENTRY._serialized_start=4337
+  _INDEXENGINECONFIG_FIELDALIASESENTRY._serialized_end=4388
+  _INDEXDESCRIPTION._serialized_start=4401
+  _INDEXDESCRIPTION._serialized_end=4637
+  _INDEXDOCUMENTOPERATION._serialized_start=4639
+  _INDEXDOCUMENTOPERATION._serialized_end=4681
+  _INDEXOPERATION._serialized_start=4683
+  _INDEXOPERATION._serialized_end=4775
+  _INDEXAPI._serialized_start=4988
+  _INDEXAPI._serialized_end=6503
 # @@protoc_insertion_point(module_scope)
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/index_service_pb2.pyi` & `summa_embed-0.15.6/summa_embed/proto/index_service_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+from typing import ClassVar as _ClassVar
+from typing import Iterable as _Iterable
+from typing import Mapping as _Mapping
+from typing import Optional as _Optional
+from typing import Union as _Union
+
 import query_pb2 as _query_pb2
 import utils_pb2 as _utils_pb2
-from google.protobuf.internal import containers as _containers
-from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from google.protobuf.internal import containers as _containers
+from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 
 Brotli: Compression
 DESCRIPTOR: _descriptor.FileDescriptor
 DO_NOTHING: ConflictStrategy
 Lz4: Compression
 MERGE: ConflictStrategy
 None: Compression
@@ -294,24 +299,33 @@
     SUCCESS_DOCS_FIELD_NUMBER: _ClassVar[int]
     elapsed_secs: float
     failed_docs: int
     success_docs: int
     def __init__(self, elapsed_secs: _Optional[float] = ..., success_docs: _Optional[int] = ..., failed_docs: _Optional[int] = ...) -> None: ...
 
 class IndexEngineConfig(_message.Message):
-    __slots__ = ["file", "memory", "merge_policy", "remote"]
+    __slots__ = ["field_aliases", "file", "memory", "merge_policy", "remote"]
+    class FieldAliasesEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    FIELD_ALIASES_FIELD_NUMBER: _ClassVar[int]
     FILE_FIELD_NUMBER: _ClassVar[int]
     MEMORY_FIELD_NUMBER: _ClassVar[int]
     MERGE_POLICY_FIELD_NUMBER: _ClassVar[int]
     REMOTE_FIELD_NUMBER: _ClassVar[int]
+    field_aliases: _containers.ScalarMap[str, str]
     file: FileEngineConfig
     memory: MemoryEngineConfig
     merge_policy: MergePolicy
     remote: RemoteEngineConfig
-    def __init__(self, file: _Optional[_Union[FileEngineConfig, _Mapping]] = ..., memory: _Optional[_Union[MemoryEngineConfig, _Mapping]] = ..., remote: _Optional[_Union[RemoteEngineConfig, _Mapping]] = ..., merge_policy: _Optional[_Union[MergePolicy, _Mapping]] = ...) -> None: ...
+    def __init__(self, file: _Optional[_Union[FileEngineConfig, _Mapping]] = ..., memory: _Optional[_Union[MemoryEngineConfig, _Mapping]] = ..., remote: _Optional[_Union[RemoteEngineConfig, _Mapping]] = ..., merge_policy: _Optional[_Union[MergePolicy, _Mapping]] = ..., field_aliases: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
 class IndexOperation(_message.Message):
     __slots__ = ["index_document"]
     INDEX_DOCUMENT_FIELD_NUMBER: _ClassVar[int]
     index_document: IndexDocumentOperation
     def __init__(self, index_document: _Optional[_Union[IndexDocumentOperation, _Mapping]] = ...) -> None: ...
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/query_pb2.py` & `summa_embed-0.15.6/summa_embed/proto/query_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: query.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import utils_pb2 as utils__pb2
 
-
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bquery.proto\x12\x0bsumma.proto\x1a\x0butils.proto\"_\n\x0eSearchResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x37\n\x11\x63ollector_outputs\x18\x02 \x03(\x0b\x32\x1c.summa.proto.CollectorOutput\"\xad\x04\n\x05Query\x12,\n\x07\x62oolean\x18\x01 \x01(\x0b\x32\x19.summa.proto.BooleanQueryH\x00\x12(\n\x05match\x18\x02 \x01(\x0b\x32\x17.summa.proto.MatchQueryH\x00\x12(\n\x05regex\x18\x03 \x01(\x0b\x32\x17.summa.proto.RegexQueryH\x00\x12&\n\x04term\x18\x04 \x01(\x0b\x32\x16.summa.proto.TermQueryH\x00\x12*\n\x06phrase\x18\x05 \x01(\x0b\x32\x18.summa.proto.PhraseQueryH\x00\x12(\n\x05range\x18\x06 \x01(\x0b\x32\x17.summa.proto.RangeQueryH\x00\x12$\n\x03\x61ll\x18\x07 \x01(\x0b\x32\x15.summa.proto.AllQueryH\x00\x12\x38\n\x0emore_like_this\x18\x08 \x01(\x0b\x32\x1e.summa.proto.MoreLikeThisQueryH\x00\x12(\n\x05\x62oost\x18\t \x01(\x0b\x32\x17.summa.proto.BoostQueryH\x00\x12;\n\x0f\x64isjunction_max\x18\n \x01(\x0b\x32 .summa.proto.DisjunctionMaxQueryH\x00\x12(\n\x05\x65mpty\x18\x0b \x01(\x0b\x32\x17.summa.proto.EmptyQueryH\x00\x12*\n\x06\x65xists\x18\x0c \x01(\x0b\x32\x18.summa.proto.ExistsQueryH\x00\x42\x07\n\x05query\"\n\n\x08\x41llQuery\"\x0c\n\nEmptyQuery\">\n\nBoostQuery\x12!\n\x05query\x18\x01 \x01(\x0b\x32\x12.summa.proto.Query\x12\r\n\x05score\x18\x02 \x01(\t\"Q\n\x13\x44isjunctionMaxQuery\x12%\n\tdisjuncts\x18\x01 \x03(\x0b\x32\x12.summa.proto.Query\x12\x13\n\x0btie_breaker\x18\x02 \x01(\t\"\x91\x03\n\x11MoreLikeThisQuery\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12\x1e\n\x11min_doc_frequency\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x1e\n\x11max_doc_frequency\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x1f\n\x12min_term_frequency\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x1c\n\x0fmax_query_terms\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12\x1c\n\x0fmin_word_length\x18\x06 \x01(\x04H\x04\x88\x01\x01\x12\x1c\n\x0fmax_word_length\x18\x07 \x01(\x04H\x05\x88\x01\x01\x12\x12\n\x05\x62oost\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x12\n\nstop_words\x18\t \x03(\tB\x14\n\x12_min_doc_frequencyB\x14\n\x12_max_doc_frequencyB\x15\n\x13_min_term_frequencyB\x12\n\x10_max_query_termsB\x12\n\x10_min_word_lengthB\x12\n\x10_max_word_lengthB\x08\n\x06_boost\"9\n\x0bPhraseQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04slop\x18\x03 \x01(\r\">\n\nRangeQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.summa.proto.Range\"\x1d\n\x1bMatchQueryBooleanShouldMode\"2\n\x1bMatchQueryDisjuctionMaxMode\x12\x13\n\x0btie_breaker\x18\x01 \x01(\x02\"B\n\x14\x45xactMatchesPromoter\x12\x0c\n\x04slop\x18\x01 \x01(\r\x12\x12\n\x05\x62oost\x18\x02 \x01(\x02H\x00\x88\x01\x01\x42\x08\n\x06_boost\"\x8c\x03\n\nMatchQuery\x12\r\n\x05value\x18\x01 \x01(\t\x12\x16\n\x0e\x64\x65\x66\x61ult_fields\x18\x02 \x03(\t\x12G\n\x13\x62oolean_should_mode\x18\x03 \x01(\x0b\x32(.summa.proto.MatchQueryBooleanShouldModeH\x00\x12G\n\x13\x64isjuction_max_mode\x18\x04 \x01(\x0b\x32(.summa.proto.MatchQueryDisjuctionMaxModeH\x00\x12>\n\x0c\x66ield_boosts\x18\x05 \x03(\x0b\x32(.summa.proto.MatchQuery.FieldBoostsEntry\x12\x41\n\x16\x65xact_matches_promoter\x18\x06 \x01(\x0b\x32!.summa.proto.ExactMatchesPromoter\x1a\x32\n\x10\x46ieldBoostsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x42\x0e\n\x0c\x64\x65\x66\x61ult_mode\"W\n\x0f\x42ooleanSubquery\x12!\n\x05occur\x18\x01 \x01(\x0e\x32\x12.summa.proto.Occur\x12!\n\x05query\x18\x02 \x01(\x0b\x32\x12.summa.proto.Query\"@\n\x0c\x42ooleanQuery\x12\x30\n\nsubqueries\x18\x01 \x03(\x0b\x32\x1c.summa.proto.BooleanSubquery\"*\n\nRegexQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\")\n\tTermQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x1c\n\x0b\x45xistsQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"\x80\x01\n\x0b\x41ggregation\x12\x30\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x1e.summa.proto.BucketAggregationH\x00\x12\x30\n\x06metric\x18\x02 \x01(\x0b\x32\x1e.summa.proto.MetricAggregationH\x00\x42\r\n\x0b\x61ggregation\"\xd7\x02\n\x11\x42ucketAggregation\x12.\n\x05range\x18\x01 \x01(\x0b\x32\x1d.summa.proto.RangeAggregationH\x00\x12\x36\n\thistogram\x18\x02 \x01(\x0b\x32!.summa.proto.HistogramAggregationH\x00\x12.\n\x05terms\x18\x03 \x01(\x0b\x32\x1d.summa.proto.TermsAggregationH\x00\x12K\n\x0fsub_aggregation\x18\x04 \x03(\x0b\x32\x32.summa.proto.BucketAggregation.SubAggregationEntry\x1aO\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.summa.proto.Aggregation:\x02\x38\x01\x42\x0c\n\nbucket_agg\"U\n\x10RangeAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x32\n\x06ranges\x18\x02 \x03(\x0b\x32\".summa.proto.RangeAggregationRange\"e\n\x15RangeAggregationRange\x12\x11\n\x04\x66rom\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02to\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03key\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x07\n\x05_fromB\x05\n\x03_toB\x06\n\x04_key\"\x9d\x02\n\x14HistogramAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x10\n\x08interval\x18\x02 \x01(\x01\x12\x13\n\x06offset\x18\x03 \x01(\x01H\x00\x88\x01\x01\x12\x1a\n\rmin_doc_count\x18\x04 \x01(\x04H\x01\x88\x01\x01\x12\x36\n\x0bhard_bounds\x18\x05 \x01(\x0b\x32\x1c.summa.proto.HistogramBoundsH\x02\x88\x01\x01\x12:\n\x0f\x65xtended_bounds\x18\x06 \x01(\x0b\x32\x1c.summa.proto.HistogramBoundsH\x03\x88\x01\x01\x42\t\n\x07_offsetB\x10\n\x0e_min_doc_countB\x0e\n\x0c_hard_boundsB\x12\n\x10_extended_bounds\"+\n\x0fHistogramBounds\x12\x0b\n\x03min\x18\x01 \x01(\x01\x12\x0b\n\x03max\x18\x02 \x01(\x01\"\xbd\x02\n\x10TermsAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x11\n\x04size\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x17\n\nsplit_size\x18\x03 \x01(\rH\x01\x88\x01\x01\x12\x19\n\x0csegment_size\x18\x04 \x01(\rH\x02\x88\x01\x01\x12&\n\x19show_term_doc_count_error\x18\x05 \x01(\x08H\x03\x88\x01\x01\x12\x1a\n\rmin_doc_count\x18\x06 \x01(\x04H\x04\x88\x01\x01\x12,\n\x05order\x18\x07 \x01(\x0b\x32\x18.summa.proto.CustomOrderH\x05\x88\x01\x01\x42\x07\n\x05_sizeB\r\n\x0b_split_sizeB\x0f\n\r_segment_sizeB\x1c\n\x1a_show_term_doc_count_errorB\x10\n\x0e_min_doc_countB\x08\n\x06_order\"\xa3\x01\n\x0b\x43ustomOrder\x12!\n\x03key\x18\x01 \x01(\x0b\x32\x12.summa.proto.EmptyH\x00\x12#\n\x05\x63ount\x18\x02 \x01(\x0b\x32\x12.summa.proto.EmptyH\x00\x12\x19\n\x0fsub_aggregation\x18\x03 \x01(\tH\x00\x12!\n\x05order\x18\x04 \x01(\x0e\x32\x12.summa.proto.OrderB\x0e\n\x0corder_target\"\x8d\x01\n\x11MetricAggregation\x12\x32\n\x07\x61verage\x18\x01 \x01(\x0b\x32\x1f.summa.proto.AverageAggregationH\x00\x12.\n\x05stats\x18\x02 \x01(\x0b\x32\x1d.summa.proto.StatsAggregationH\x00\x42\x14\n\x12metric_aggregation\"#\n\x12\x41verageAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"!\n\x10StatsAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"\xdd\x01\n\x0b\x42ucketEntry\x12\x1d\n\x03key\x18\x01 \x01(\x0b\x32\x10.summa.proto.Key\x12\x11\n\tdoc_count\x18\x02 \x01(\x04\x12\x45\n\x0fsub_aggregation\x18\x03 \x03(\x0b\x32,.summa.proto.BucketEntry.SubAggregationEntry\x1aU\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\"*\n\x03Key\x12\r\n\x03str\x18\x01 \x01(\tH\x00\x12\r\n\x03\x66\x36\x34\x18\x02 \x01(\x01H\x00\x42\x05\n\x03key\"U\n\x05Range\x12\x0c\n\x04left\x18\x01 \x01(\t\x12\r\n\x05right\x18\x02 \x01(\t\x12\x16\n\x0eincluding_left\x18\x03 \x01(\x08\x12\x17\n\x0fincluding_right\x18\x04 \x01(\x08\"\x9b\x02\n\x10RangeBucketEntry\x12\x1d\n\x03key\x18\x01 \x01(\x0b\x32\x10.summa.proto.Key\x12\x11\n\tdoc_count\x18\x02 \x01(\x04\x12J\n\x0fsub_aggregation\x18\x03 \x03(\x0b\x32\x31.summa.proto.RangeBucketEntry.SubAggregationEntry\x12\x11\n\x04\x66rom\x18\x04 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02to\x18\x05 \x01(\x01H\x01\x88\x01\x01\x1aU\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\x42\x07\n\x05_fromB\x05\n\x03_to\":\n\x05Score\x12\x13\n\tf64_score\x18\x01 \x01(\x01H\x00\x12\x13\n\tu64_score\x18\x02 \x01(\x04H\x00\x42\x07\n\x05score\"%\n\tHighlight\x12\x0c\n\x04\x66rom\x18\x01 \x01(\r\x12\n\n\x02to\x18\x02 \x01(\r\"U\n\x07Snippet\x12\x10\n\x08\x66ragment\x18\x01 \x01(\x0c\x12*\n\nhighlights\x18\x02 \x03(\x0b\x32\x16.summa.proto.Highlight\x12\x0c\n\x04html\x18\x03 \x01(\t\"\xf0\x01\n\x0eScoredDocument\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12!\n\x05score\x18\x02 \x01(\x0b\x32\x12.summa.proto.Score\x12\x10\n\x08position\x18\x03 \x01(\r\x12;\n\x08snippets\x18\x04 \x03(\x0b\x32).summa.proto.ScoredDocument.SnippetsEntry\x12\x13\n\x0bindex_alias\x18\x05 \x01(\t\x1a\x45\n\rSnippetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.summa.proto.Snippet:\x02\x38\x01\";\n\x06Scorer\x12\x13\n\teval_expr\x18\x01 \x01(\tH\x00\x12\x12\n\x08order_by\x18\x02 \x01(\tH\x00\x42\x08\n\x06scorer\"\xa8\x02\n\tCollector\x12\x31\n\x08top_docs\x18\x01 \x01(\x0b\x32\x1d.summa.proto.TopDocsCollectorH\x00\x12\x45\n\x12reservoir_sampling\x18\x02 \x01(\x0b\x32\'.summa.proto.ReservoirSamplingCollectorH\x00\x12,\n\x05\x63ount\x18\x03 \x01(\x0b\x32\x1b.summa.proto.CountCollectorH\x00\x12,\n\x05\x66\x61\x63\x65t\x18\x04 \x01(\x0b\x32\x1b.summa.proto.FacetCollectorH\x00\x12\x38\n\x0b\x61ggregation\x18\x05 \x01(\x0b\x32!.summa.proto.AggregationCollectorH\x00\x42\x0b\n\tcollector\"\x89\x02\n\x0f\x43ollectorOutput\x12:\n\tdocuments\x18\x01 \x01(\x0b\x32%.summa.proto.DocumentsCollectorOutputH\x00\x12\x32\n\x05\x63ount\x18\x03 \x01(\x0b\x32!.summa.proto.CountCollectorOutputH\x00\x12\x32\n\x05\x66\x61\x63\x65t\x18\x04 \x01(\x0b\x32!.summa.proto.FacetCollectorOutputH\x00\x12>\n\x0b\x61ggregation\x18\x05 \x01(\x0b\x32\'.summa.proto.AggregationCollectorOutputH\x00\x42\x12\n\x10\x63ollector_output\"\x10\n\x0e\x43ountCollector\"%\n\x14\x43ountCollectorOutput\x12\r\n\x05\x63ount\x18\x01 \x01(\r\"/\n\x0e\x46\x61\x63\x65tCollector\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x0e\n\x06\x66\x61\x63\x65ts\x18\x02 \x03(\t\"\x94\x01\n\x14\x46\x61\x63\x65tCollectorOutput\x12H\n\x0c\x66\x61\x63\x65t_counts\x18\x01 \x03(\x0b\x32\x32.summa.proto.FacetCollectorOutput.FacetCountsEntry\x1a\x32\n\x10\x46\x61\x63\x65tCountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01\";\n\x1aReservoirSamplingCollector\x12\r\n\x05limit\x18\x01 \x01(\r\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"Z\n\x0eRandomDocument\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12!\n\x05score\x18\x02 \x01(\x0b\x32\x12.summa.proto.Score\x12\x13\n\x0bindex_alias\x18\x03 \x01(\t\"R\n ReservoirSamplingCollectorOutput\x12.\n\tdocuments\x18\x01 \x03(\x0b\x32\x1b.summa.proto.RandomDocument\"\x8a\x02\n\x10TopDocsCollector\x12\r\n\x05limit\x18\x01 \x01(\r\x12\x0e\n\x06offset\x18\x02 \x01(\r\x12(\n\x06scorer\x18\x03 \x01(\x0b\x32\x13.summa.proto.ScorerH\x00\x88\x01\x01\x12J\n\x0fsnippet_configs\x18\x04 \x03(\x0b\x32\x31.summa.proto.TopDocsCollector.SnippetConfigsEntry\x12\x0f\n\x07\x65xplain\x18\x05 \x01(\x08\x12\x0e\n\x06\x66ields\x18\x06 \x03(\t\x1a\x35\n\x13SnippetConfigsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\x42\t\n\x07_scorer\"c\n\x18\x44ocumentsCollectorOutput\x12\x35\n\x10scored_documents\x18\x01 \x03(\x0b\x32\x1b.summa.proto.ScoredDocument\x12\x10\n\x08has_next\x18\x02 \x01(\x08\"\xb0\x01\n\x14\x41ggregationCollector\x12I\n\x0c\x61ggregations\x18\x01 \x03(\x0b\x32\x33.summa.proto.AggregationCollector.AggregationsEntry\x1aM\n\x11\x41ggregationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.summa.proto.Aggregation:\x02\x38\x01\"\xd5\x01\n\x1a\x41ggregationCollectorOutput\x12\\\n\x13\x61ggregation_results\x18\x01 \x03(\x0b\x32?.summa.proto.AggregationCollectorOutput.AggregationResultsEntry\x1aY\n\x17\x41ggregationResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\"\x83\x01\n\x11\x41ggregationResult\x12+\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x19.summa.proto.BucketResultH\x00\x12+\n\x06metric\x18\x02 \x01(\x0b\x32\x19.summa.proto.MetricResultH\x00\x42\x14\n\x12\x61ggregation_result\"\xa8\x01\n\x0c\x42ucketResult\x12)\n\x05range\x18\x01 \x01(\x0b\x32\x18.summa.proto.RangeResultH\x00\x12\x31\n\thistogram\x18\x02 \x01(\x0b\x32\x1c.summa.proto.HistogramResultH\x00\x12)\n\x05terms\x18\x03 \x01(\x0b\x32\x18.summa.proto.TermsResultH\x00\x42\x0f\n\rbucket_result\"=\n\x0bRangeResult\x12.\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x1d.summa.proto.RangeBucketEntry\"<\n\x0fHistogramResult\x12)\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x18.summa.proto.BucketEntry\"\x9f\x01\n\x0bTermsResult\x12)\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x18.summa.proto.BucketEntry\x12\x1b\n\x13sum_other_doc_count\x18\x02 \x01(\x04\x12(\n\x1b\x64oc_count_error_upper_bound\x18\x03 \x01(\x04H\x00\x88\x01\x01\x42\x1e\n\x1c_doc_count_error_upper_bound\"\x84\x01\n\x0cMetricResult\x12\x38\n\rsingle_metric\x18\x01 \x01(\x0b\x32\x1f.summa.proto.SingleMetricResultH\x00\x12)\n\x05stats\x18\x02 \x01(\x0b\x32\x18.summa.proto.StatsResultH\x00\x42\x0f\n\rmetric_result\"2\n\x12SingleMetricResult\x12\x12\n\x05value\x18\x01 \x01(\x01H\x00\x88\x01\x01\x42\x08\n\x06_value\"w\n\x0bStatsResult\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\x12\x0b\n\x03sum\x18\x02 \x01(\x01\x12\x10\n\x03min\x18\x03 \x01(\x01H\x00\x88\x01\x01\x12\x10\n\x03max\x18\x04 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03\x61vg\x18\x05 \x01(\x01H\x02\x88\x01\x01\x42\x06\n\x04_minB\x06\n\x04_maxB\x06\n\x04_avg*+\n\x05Occur\x12\n\n\x06should\x10\x00\x12\x08\n\x04must\x10\x01\x12\x0c\n\x08must_not\x10\x02\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'query_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/query_pb2.pyi` & `summa_embed-0.15.6/summa_embed/proto/query_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+from typing import ClassVar as _ClassVar
+from typing import Iterable as _Iterable
+from typing import Mapping as _Mapping
+from typing import Optional as _Optional
+from typing import Union as _Union
+
 import utils_pb2 as _utils_pb2
-from google.protobuf.internal import containers as _containers
-from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from google.protobuf.internal import containers as _containers
+from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 
 DESCRIPTOR: _descriptor.FileDescriptor
 must: Occur
 must_not: Occur
 should: Occur
 
 class Aggregation(_message.Message):
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/reflection_service_pb2.py` & `summa_embed-0.15.6/summa_embed/proto/reflection_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: reflection_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/reflection_service_pb2.pyi` & `summa_embed-0.15.6/summa_embed/proto/reflection_service_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-from google.protobuf.internal import containers as _containers
+from typing import ClassVar as _ClassVar
+from typing import Iterable as _Iterable
+from typing import Mapping as _Mapping
+from typing import Optional as _Optional
+from typing import Union as _Union
+
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from google.protobuf.internal import containers as _containers
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class GetTopTermsRequest(_message.Message):
     __slots__ = ["field_name", "index_name", "top_k"]
     FIELD_NAME_FIELD_NUMBER: _ClassVar[int]
     INDEX_NAME_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/search_service_pb2.py` & `summa_embed-0.15.6/summa_embed/proto/search_service_pb2.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: search_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import query_pb2 as query__pb2
 
-
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14search_service.proto\x12\x0bsumma.proto\x1a\x0bquery.proto\"\xa0\x01\n\rSearchRequest\x12.\n\rindex_queries\x18\x01 \x03(\x0b\x32\x17.summa.proto.IndexQuery\x12\x32\n\x04tags\x18\x02 \x03(\x0b\x32$.summa.proto.SearchRequest.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xbe\x01\n\nIndexQuery\x12\x13\n\x0bindex_alias\x18\x01 \x01(\t\x12!\n\x05query\x18\x02 \x01(\x0b\x32\x12.summa.proto.Query\x12*\n\ncollectors\x18\x03 \x03(\x0b\x32\x16.summa.proto.Collector\x12*\n\x1dis_fieldnorms_scoring_enabled\x18\x04 \x01(\x08H\x00\x88\x01\x01\x42 \n\x1e_is_fieldnorms_scoring_enabled2P\n\tSearchApi\x12\x43\n\x06search\x12\x1a.summa.proto.SearchRequest\x1a\x1b.summa.proto.SearchResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'search_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/search_service_pb2.pyi` & `summa_embed-0.15.6/summa_embed/proto/search_service_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+from typing import ClassVar as _ClassVar
+from typing import Iterable as _Iterable
+from typing import Mapping as _Mapping
+from typing import Optional as _Optional
+from typing import Union as _Union
+
 import query_pb2 as _query_pb2
-from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from google.protobuf.internal import containers as _containers
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class IndexQuery(_message.Message):
     __slots__ = ["collectors", "index_alias", "is_fieldnorms_scoring_enabled", "query"]
     COLLECTORS_FIELD_NUMBER: _ClassVar[int]
     INDEX_ALIAS_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/unixfs_pb2.py` & `summa_embed-0.15.6/summa_embed/proto/unixfs_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: unixfs.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/unixfs_pb2.pyi` & `summa_embed-0.15.6/summa_embed/proto/unixfs_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from google.protobuf.internal import containers as _containers
-from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
+from typing import ClassVar as _ClassVar
+from typing import Iterable as _Iterable
+from typing import Optional as _Optional
+from typing import Union as _Union
+
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Optional as _Optional, Union as _Union
+from google.protobuf.internal import containers as _containers
+from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Data(_message.Message):
     __slots__ = ["blocksizes", "data", "fanout", "filesize", "hashType", "type"]
     class DataType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
```

### Comparing `summa_embed-0.15.4/summa_embed/proto/utils_pb2.py` & `summa_embed-0.15.6/summa_embed/proto/utils_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: utils.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `summa_embed-0.15.4/Cargo.lock` & `summa_embed-0.15.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2912,15 +2912,15 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "summa-core"
-version = "0.15.5"
+version = "0.15.6"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bytes",
  "config",
  "derive_builder",
@@ -2958,15 +2958,15 @@
  "time",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.15.4"
+version = "0.15.6"
 dependencies = [
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
  "pythonize",
  "serde_json",
```

