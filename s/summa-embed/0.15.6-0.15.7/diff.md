# Comparing `tmp/summa_embed-0.15.6.tar.gz` & `tmp/summa_embed-0.15.7.tar.gz`

## Comparing `summa_embed-0.15.6.tar` & `summa_embed-0.15.7.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.15.6/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2262 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10419 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7125 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2353 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      424 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-05-31 10:09:35.000000 summa_embed-0.15.6/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 summa_embed-0.15.6/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20       92 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7087 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5015 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20     1021 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/driver.rs
--rw-r--r--   0      501       20    13794 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    24562 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13833 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    14335 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5038 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     4711 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      163 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20    15871 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1595 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    56532 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     2216 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11274 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7439 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     3093 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8014 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5490 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      450 2023-05-31 10:09:34.000000 summa_embed-0.15.6/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 summa_embed-0.15.6/Cargo.toml
--rw-r--r--   0      501       20      685 2023-05-31 10:09:34.000000 summa_embed-0.15.6/.gitignore
--rwxr-xr-x   0      501       20      347 2023-05-31 10:09:34.000000 summa_embed-0.15.6/build.sh
--rw-r--r--   0      501       20      515 2023-05-31 10:09:35.000000 summa_embed-0.15.6/pyproject.toml
--rw-r--r--   0      501       20       14 2023-05-31 10:09:35.000000 summa_embed-0.15.6/requirements.txt
--rw-r--r--   0      501       20     4331 2023-05-31 10:09:35.000000 summa_embed-0.15.6/src/lib.rs
--rw-r--r--   0      501       20     1050 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/__init__.py
--rw-r--r--   0      501       20        0 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/__init__.py
--rw-r--r--   0      501       20     3124 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/consumer_service_pb2.py
--rw-r--r--   0      501       20     3153 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/consumer_service_pb2.pyi
--rw-r--r--   0      501       20     1336 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/dag_pb_pb2.py
--rw-r--r--   0      501       20     1115 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/dag_pb_pb2.pyi
--rw-r--r--   0      501       20    16689 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/index_service_pb2.py
--rw-r--r--   0      501       20    20021 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/index_service_pb2.pyi
--rw-r--r--   0      501       20    21461 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/query_pb2.py
--rw-r--r--   0      501       20    29410 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/query_pb2.pyi
--rw-r--r--   0      501       20     2214 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/reflection_service_pb2.py
--rw-r--r--   0      501       20     1996 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/reflection_service_pb2.pyi
--rw-r--r--   0      501       20     2012 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/search_service_pb2.py
--rw-r--r--   0      501       20     1903 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/search_service_pb2.pyi
--rw-r--r--   0      501       20     1742 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/unixfs_pb2.py
--rw-r--r--   0      501       20     1653 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/unixfs_pb2.pyi
--rw-r--r--   0      501       20     1041 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/utils_pb2.py
--rw-r--r--   0      501       20      455 2023-05-31 10:09:35.000000 summa_embed-0.15.6/summa_embed/proto/utils_pb2.pyi
--rw-r--r--   0      501       20   102226 2023-05-31 10:09:55.000000 summa_embed-0.15.6/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.15.6/PKG-INFO
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.15.7/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2262 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10419 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7125 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2353 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      424 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 summa_embed-0.15.7/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20       92 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7087 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5015 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20     1021 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/driver.rs
+-rw-r--r--   0      501       20    13794 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    24648 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13833 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    14335 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5038 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     4711 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      163 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20    16401 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1595 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    56532 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     2216 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11274 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7439 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     3093 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8014 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5490 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      450 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 summa_embed-0.15.7/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-05-31 11:10:15.000000 summa_embed-0.15.7/.gitignore
+-rwxr-xr-x   0      501       20      347 2023-05-31 11:10:15.000000 summa_embed-0.15.7/build.sh
+-rw-r--r--   0      501       20      515 2023-05-31 11:10:15.000000 summa_embed-0.15.7/pyproject.toml
+-rw-r--r--   0      501       20       14 2023-05-31 11:10:15.000000 summa_embed-0.15.7/requirements.txt
+-rw-r--r--   0      501       20     4398 2023-05-31 11:10:15.000000 summa_embed-0.15.7/src/lib.rs
+-rw-r--r--   0      501       20     1050 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/__init__.py
+-rw-r--r--   0      501       20        0 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/__init__.py
+-rw-r--r--   0      501       20     3124 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/consumer_service_pb2.py
+-rw-r--r--   0      501       20     3153 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/consumer_service_pb2.pyi
+-rw-r--r--   0      501       20     1336 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/dag_pb_pb2.py
+-rw-r--r--   0      501       20     1115 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/dag_pb_pb2.pyi
+-rw-r--r--   0      501       20    16689 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/index_service_pb2.py
+-rw-r--r--   0      501       20    20021 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/index_service_pb2.pyi
+-rw-r--r--   0      501       20    21461 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/query_pb2.py
+-rw-r--r--   0      501       20    29410 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/query_pb2.pyi
+-rw-r--r--   0      501       20     2214 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/reflection_service_pb2.py
+-rw-r--r--   0      501       20     1996 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/reflection_service_pb2.pyi
+-rw-r--r--   0      501       20     2012 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/search_service_pb2.py
+-rw-r--r--   0      501       20     1903 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/search_service_pb2.pyi
+-rw-r--r--   0      501       20     1742 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/unixfs_pb2.py
+-rw-r--r--   0      501       20     1653 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/unixfs_pb2.pyi
+-rw-r--r--   0      501       20     1041 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/utils_pb2.py
+-rw-r--r--   0      501       20      455 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/utils_pb2.pyi
+-rw-r--r--   0      501       20   102226 2023-05-31 11:10:27.000000 summa_embed-0.15.7/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.15.7/PKG-INFO
```

### Comparing `summa_embed-0.15.6/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.15.7/local_dependencies/summa-proto/Cargo.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.15.7/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-proto/build.rs` & `summa_embed-0.15.7/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.15.7/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.15.7/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.15.7/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.15.7/local_dependencies/summa-proto/proto/query.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.15.7/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.15.7/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.15.7/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.15.7/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.15.7/local_dependencies/summa-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.15.6"
+version = "0.15.7"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
```

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/LICENSE` & `summa_embed-0.15.7/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/driver.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/driver.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use std::collections::HashSet;
+use std::collections::{HashMap, HashSet};
 use std::fmt::Debug;
 use std::hash::{Hash, Hasher};
 use std::path::Path;
 use std::sync::Arc;
 
 use futures::future::{join_all, try_join_all};
 #[cfg(feature = "metrics")]
@@ -156,14 +156,15 @@
     /// Sets up `IndexHolder`
     pub fn create_holder(
         core_config: &crate::configs::core::Config,
         mut index: Index,
         index_name: Option<&str>,
         index_engine_config: Arc<dyn ConfigProxy<proto::IndexEngineConfig>>,
         merge_policy: Option<proto::MergePolicy>,
+        field_aliases: HashMap<String, String>,
         read_only: bool,
         driver: Driver,
     ) -> SummaResult<IndexHolder> {
         register_default_tokenizers(&index);
 
         index.settings_mut().docstore_compress_dedicated_thread = core_config.dedicated_compression_thread;
         index.set_segment_attributes_merger(Arc::new(SegmentAttributesMergerImpl::<SummaSegmentAttributes>::new()));
@@ -192,14 +193,15 @@
                 .expect("no index name")
         });
 
         let query_parser = ProtoQueryParser::for_index(
             &index_name,
             &index,
             cached_index_attributes.as_ref().map(|a| a.default_fields.clone()).unwrap_or_else(Vec::new),
+            field_aliases,
         )?;
         let index_reader = index
             .reader_builder()
             .doc_store_cache_num_blocks(core_config.doc_store_cache_num_blocks)
             .reload_policy(ReloadPolicy::OnCommit)
             .try_into()?;
         index_reader.reload()?;
```

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use std::collections::HashMap;
 use std::ops::Bound;
 use std::ops::Bound::Unbounded;
 use std::str::FromStr;
 
 use base64::Engine;
 #[cfg(feature = "metrics")]
 use opentelemetry::metrics::Counter;
@@ -31,14 +32,15 @@
     cached_schema: Schema,
     // Counters
     #[cfg(feature = "metrics")]
     query_counter: Counter<u64>,
     #[cfg(feature = "metrics")]
     subquery_counter: Counter<u64>,
     index_default_fields: Vec<String>,
+    field_aliases: HashMap<String, String>,
 }
 
 pub enum MatchQueryDefaultMode {
     Boolean,
     DisjuctionMax { tie_breaker: Score },
 }
 
@@ -101,15 +103,20 @@
                 Bound::Excluded(casted_value)
             }
         }
     })
 }
 
 impl ProtoQueryParser {
-    pub fn for_index(index_name: &str, index: &Index, index_default_fields: Vec<String>) -> SummaResult<ProtoQueryParser> {
+    pub fn for_index(
+        index_name: &str,
+        index: &Index,
+        index_default_fields: Vec<String>,
+        field_aliases: HashMap<String, String>,
+    ) -> SummaResult<ProtoQueryParser> {
         #[cfg(feature = "metrics")]
         let query_counter = global::meter("summa").u64_counter("query_counter").with_description("Queries counter").init();
         #[cfg(feature = "metrics")]
         let subquery_counter = global::meter("summa")
             .u64_counter("subquery_counter")
             .with_description("Sub-queries counter")
             .init();
@@ -119,20 +126,25 @@
             index_name: index_name.to_string(),
             cached_schema: index.schema(),
             #[cfg(feature = "metrics")]
             query_counter,
             #[cfg(feature = "metrics")]
             subquery_counter,
             index_default_fields,
+            field_aliases,
         })
     }
 
+    pub fn resolve_field_name<'a>(&'a self, field_name: &'a str) -> &str {
+        self.field_aliases.get(field_name).map(|s| s.as_str()).unwrap_or(field_name)
+    }
+
     #[inline]
     pub(crate) fn field_and_field_entry<'a>(&'a self, field_name: &'a str) -> SummaResult<(Field, &str, &FieldEntry)> {
-        match self.cached_schema.find_field(field_name) {
+        match self.cached_schema.find_field(self.resolve_field_name(field_name)) {
             Some((field, full_path)) => {
                 let field_entry = self.cached_schema.get_field_entry(field);
                 Ok((field, full_path, field_entry))
             }
             None => Err(ValidationError::MissingField(field_name.to_string()).into()),
         }
     }
@@ -194,14 +206,18 @@
                     nested_query_parser.set_field_boosts(match_query_proto.field_boosts)
                 }
 
                 if let Some(exact_matches_promoter) = match_query_proto.exact_matches_promoter {
                     nested_query_parser.set_exact_match_promoter(exact_matches_promoter)
                 }
 
+                if !self.field_aliases.is_empty() {
+                    nested_query_parser.set_field_aliases(self.field_aliases.clone())
+                }
+
                 match nested_query_parser.parse_query(&match_query_proto.value) {
                     Ok(parsed_query) => {
                         info!(parsed_match_query = ?parsed_query);
                         Ok(parsed_query)
                     }
                     Err(QueryParserError::FieldDoesNotExist(field)) => Err(ValidationError::MissingField(field).into()),
                     Err(e) => Err(Error::InvalidQuerySyntax(Box::new(e), match_query_proto.value.to_owned())),
```

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.15.7/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/Cargo.toml` & `summa_embed-0.15.7/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "summa-embed-py"
-version = "0.15.6"
+version = "0.15.7"
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
-summa-core = { version = "0.15.6", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.15.7", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.15.6/.gitignore` & `summa_embed-0.15.7/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/pyproject.toml` & `summa_embed-0.15.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/src/lib.rs` & `summa_embed-0.15.7/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use std::collections::HashMap;
 use std::sync::Arc;
 
 use futures::future::join_all;
 use prost::Message;
 use pyo3::exceptions::PyOSError;
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
@@ -72,14 +73,15 @@
             let index_holder = tokio::task::spawn_blocking(move || {
                 IndexHolder::create_holder(
                     &core_config,
                     index,
                     index_name.as_deref(),
                     Arc::new(DirectProxy::new(index_engine_config)),
                     None,
+                    HashMap::new(),
                     true,
                     Driver::current_tokio(),
                 )
             })
             .await
             .unwrap()
             .unwrap();
```

### Comparing `summa_embed-0.15.6/summa_embed/__init__.py` & `summa_embed-0.15.7/summa_embed/__init__.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/consumer_service_pb2.py` & `summa_embed-0.15.7/summa_embed/proto/consumer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/consumer_service_pb2.pyi` & `summa_embed-0.15.7/summa_embed/proto/consumer_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/dag_pb_pb2.py` & `summa_embed-0.15.7/summa_embed/proto/dag_pb_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/dag_pb_pb2.pyi` & `summa_embed-0.15.7/summa_embed/proto/dag_pb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/index_service_pb2.py` & `summa_embed-0.15.7/summa_embed/proto/index_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/index_service_pb2.pyi` & `summa_embed-0.15.7/summa_embed/proto/index_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/query_pb2.py` & `summa_embed-0.15.7/summa_embed/proto/query_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/query_pb2.pyi` & `summa_embed-0.15.7/summa_embed/proto/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/reflection_service_pb2.py` & `summa_embed-0.15.7/summa_embed/proto/reflection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/reflection_service_pb2.pyi` & `summa_embed-0.15.7/summa_embed/proto/reflection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/search_service_pb2.py` & `summa_embed-0.15.7/summa_embed/proto/search_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/search_service_pb2.pyi` & `summa_embed-0.15.7/summa_embed/proto/search_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/unixfs_pb2.py` & `summa_embed-0.15.7/summa_embed/proto/unixfs_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/unixfs_pb2.pyi` & `summa_embed-0.15.7/summa_embed/proto/unixfs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/summa_embed/proto/utils_pb2.py` & `summa_embed-0.15.7/summa_embed/proto/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.6/Cargo.lock` & `summa_embed-0.15.7/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -2912,15 +2912,15 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "summa-core"
-version = "0.15.6"
+version = "0.15.7"
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
-version = "0.15.6"
+version = "0.15.7"
 dependencies = [
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
  "pythonize",
  "serde_json",
```

