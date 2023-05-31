# Comparing `tmp/summa_embed-0.15.7.tar.gz` & `tmp/summa_embed-0.15.8.tar.gz`

## Comparing `summa_embed-0.15.7.tar` & `summa_embed-0.15.8.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.15.7/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2262 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10419 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7125 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2353 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      424 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 summa_embed-0.15.7/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20       92 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7087 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5015 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20     1021 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/driver.rs
--rw-r--r--   0      501       20    13794 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    24648 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13833 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    14335 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5038 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     4711 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      163 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20    16401 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1595 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    56532 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     2216 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11274 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7439 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     3093 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8014 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5490 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      450 2023-05-31 11:10:15.000000 summa_embed-0.15.7/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 summa_embed-0.15.7/Cargo.toml
--rw-r--r--   0      501       20      685 2023-05-31 11:10:15.000000 summa_embed-0.15.7/.gitignore
--rwxr-xr-x   0      501       20      347 2023-05-31 11:10:15.000000 summa_embed-0.15.7/build.sh
--rw-r--r--   0      501       20      515 2023-05-31 11:10:15.000000 summa_embed-0.15.7/pyproject.toml
--rw-r--r--   0      501       20       14 2023-05-31 11:10:15.000000 summa_embed-0.15.7/requirements.txt
--rw-r--r--   0      501       20     4398 2023-05-31 11:10:15.000000 summa_embed-0.15.7/src/lib.rs
--rw-r--r--   0      501       20     1050 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/__init__.py
--rw-r--r--   0      501       20        0 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/__init__.py
--rw-r--r--   0      501       20     3124 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/consumer_service_pb2.py
--rw-r--r--   0      501       20     3153 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/consumer_service_pb2.pyi
--rw-r--r--   0      501       20     1336 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/dag_pb_pb2.py
--rw-r--r--   0      501       20     1115 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/dag_pb_pb2.pyi
--rw-r--r--   0      501       20    16689 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/index_service_pb2.py
--rw-r--r--   0      501       20    20021 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/index_service_pb2.pyi
--rw-r--r--   0      501       20    21461 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/query_pb2.py
--rw-r--r--   0      501       20    29410 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/query_pb2.pyi
--rw-r--r--   0      501       20     2214 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/reflection_service_pb2.py
--rw-r--r--   0      501       20     1996 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/reflection_service_pb2.pyi
--rw-r--r--   0      501       20     2012 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/search_service_pb2.py
--rw-r--r--   0      501       20     1903 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/search_service_pb2.pyi
--rw-r--r--   0      501       20     1742 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/unixfs_pb2.py
--rw-r--r--   0      501       20     1653 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/unixfs_pb2.pyi
--rw-r--r--   0      501       20     1041 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/utils_pb2.py
--rw-r--r--   0      501       20      455 2023-05-31 11:10:15.000000 summa_embed-0.15.7/summa_embed/proto/utils_pb2.pyi
--rw-r--r--   0      501       20   102226 2023-05-31 11:10:27.000000 summa_embed-0.15.7/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.15.7/PKG-INFO
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2262 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10419 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7125 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2353 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      424 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20       92 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7087 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5015 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20     1021 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/driver.rs
+-rw-r--r--   0      501       20    13794 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    24648 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13833 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    14335 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5038 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     4711 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      163 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20    16401 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1595 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    57848 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     2216 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11274 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7439 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     3093 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8014 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5490 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      450 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 summa_embed-0.15.8/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-05-31 18:46:00.000000 summa_embed-0.15.8/.gitignore
+-rwxr-xr-x   0      501       20      347 2023-05-31 18:46:00.000000 summa_embed-0.15.8/build.sh
+-rw-r--r--   0      501       20      515 2023-05-31 18:46:00.000000 summa_embed-0.15.8/pyproject.toml
+-rw-r--r--   0      501       20       14 2023-05-31 18:46:00.000000 summa_embed-0.15.8/requirements.txt
+-rw-r--r--   0      501       20     4398 2023-05-31 18:46:00.000000 summa_embed-0.15.8/src/lib.rs
+-rw-r--r--   0      501       20     1050 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/__init__.py
+-rw-r--r--   0      501       20        0 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/__init__.py
+-rw-r--r--   0      501       20     3124 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/consumer_service_pb2.py
+-rw-r--r--   0      501       20     3153 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/consumer_service_pb2.pyi
+-rw-r--r--   0      501       20     1336 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/dag_pb_pb2.py
+-rw-r--r--   0      501       20     1115 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/dag_pb_pb2.pyi
+-rw-r--r--   0      501       20    16689 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/index_service_pb2.py
+-rw-r--r--   0      501       20    20021 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/index_service_pb2.pyi
+-rw-r--r--   0      501       20    21461 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/query_pb2.py
+-rw-r--r--   0      501       20    29410 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/query_pb2.pyi
+-rw-r--r--   0      501       20     2214 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/reflection_service_pb2.py
+-rw-r--r--   0      501       20     1996 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/reflection_service_pb2.pyi
+-rw-r--r--   0      501       20     2012 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/search_service_pb2.py
+-rw-r--r--   0      501       20     1903 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/search_service_pb2.pyi
+-rw-r--r--   0      501       20     1742 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/unixfs_pb2.py
+-rw-r--r--   0      501       20     1653 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/unixfs_pb2.pyi
+-rw-r--r--   0      501       20     1041 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/utils_pb2.py
+-rw-r--r--   0      501       20      455 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/utils_pb2.pyi
+-rw-r--r--   0      501       20   102226 2023-05-31 18:48:32.000000 summa_embed-0.15.8/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.15.8/PKG-INFO
```

### Comparing `summa_embed-0.15.7/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.15.8/local_dependencies/summa-proto/Cargo.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.15.8/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-proto/build.rs` & `summa_embed-0.15.8/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.15.8/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.15.8/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.15.8/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.15.8/local_dependencies/summa-proto/proto/query.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.15.8/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.15.8/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.15.8/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.15.8/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.15.8/local_dependencies/summa-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.15.7"
+version = "0.15.8"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
```

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/LICENSE` & `summa_embed-0.15.8/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/driver.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/driver.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files 5% similar despite different names*

```diff
@@ -286,16 +286,20 @@
             }
         })
     }
 
     fn parse_range(&self, pre_term: Pair<Rule>, field: &Field) -> Result<RangeQuery, QueryParserError> {
         let mut range_pairs = pre_term.into_inner();
         let field_entry = self.schema.get_field_entry(*field);
+        if !field_entry.field_type().is_indexed() && !field_entry.field_type().is_fast() {
+            return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
+        }
         let left = self.parse_boundary_word(*field, range_pairs.next().expect("grammar failure"))?;
         let right = self.parse_boundary_word(*field, range_pairs.next().expect("grammar failure"))?;
+
         Ok(RangeQuery::new_term_bounds(
             field_entry.name().to_string(),
             field_entry.field_type().value_type(),
             &left,
             &right,
         ))
     }
@@ -312,18 +316,14 @@
         Ok(terms)
     }
 
     fn parse_pre_term(&self, field: &Field, full_path: &str, pre_term: Pair<Rule>, boost: Option<f32>) -> Result<Vec<Box<dyn Query>>, QueryParserError> {
         let field_entry = self.schema.get_field_entry(*field);
         let field_type = field_entry.field_type();
 
-        if !field_type.is_indexed() {
-            return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
-        }
-
         if field_type.value_type() == Type::Json && full_path.is_empty() {
             return Err(QueryParserError::JsonFieldWithoutPath(field_entry.name().to_string()));
         }
 
         if field_type.value_type() != Type::Json && !full_path.is_empty() {
             return Err(QueryParserError::NonJsonFieldWithPath(format!(
                 "{}.{}",
@@ -338,41 +338,53 @@
             return Ok(vec![boost_query(Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>, boost)]);
         }
 
         return match *field_type {
             FieldType::U64(_) => match pre_term.as_rule() {
                 Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                 Rule::phrase | Rule::word => {
+                    if !field_type.is_indexed() {
+                        return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
+                    }
                     let val: u64 = u64::from_str(pre_term.as_str())?;
                     let query = Box::new(TermQuery::new(Term::from_field_u64(*field, val), IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                     Ok(vec![boost_query(query, boost)])
                 }
                 _ => unreachable!(),
             },
             FieldType::I64(_) => match pre_term.as_rule() {
                 Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                 Rule::phrase | Rule::word => {
+                    if !field_type.is_indexed() {
+                        return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
+                    }
                     let val: i64 = i64::from_str(pre_term.as_str())?;
                     let query = Box::new(TermQuery::new(Term::from_field_i64(*field, val), IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                     Ok(vec![boost_query(query, boost)])
                 }
                 _ => unreachable!(),
             },
             FieldType::F64(_) => match pre_term.as_rule() {
                 Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                 Rule::phrase | Rule::word => {
+                    if !field_type.is_indexed() {
+                        return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
+                    }
                     let val: f64 = f64::from_str(pre_term.as_str())?;
                     let query = Box::new(TermQuery::new(Term::from_field_f64(*field, val), IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                     Ok(vec![boost_query(query, boost)])
                 }
                 _ => unreachable!(),
             },
             FieldType::Bool(_) => match pre_term.as_rule() {
                 Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                 Rule::phrase | Rule::word => {
+                    if !field_type.is_indexed() {
+                        return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
+                    }
                     let val: bool = bool::from_str(pre_term.as_str())?;
                     let query = Box::new(TermQuery::new(Term::from_field_bool(*field, val), IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                     Ok(vec![boost_query(query, boost)])
                 }
                 _ => unreachable!(),
             },
             FieldType::Str(_) | FieldType::JsonObject(_) => {
@@ -382,14 +394,18 @@
                     json_options.get_text_indexing_options().expect("unreachable")
                 } else {
                     unreachable!()
                 };
 
                 match pre_term.as_rule() {
                     Rule::word | Rule::field_name => {
+                        if !field_type.is_indexed() {
+                            return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
+                        }
+
                         let mut token_stream = self.get_text_analyzer(field_entry, indexing)?.token_stream(pre_term.as_str());
                         let mut queries = Vec::new();
 
                         token_stream.process(&mut |token| {
                             let term = match field_type {
                                 FieldType::Str(_) => Term::from_field_text(*field, &token.text),
                                 FieldType::JsonObject(ref json_options) => {
@@ -406,14 +422,18 @@
                             let query = Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                             queries.push(boost_query(query, boost));
                         });
 
                         Ok(queries)
                     }
                     Rule::phrase => {
+                        if !field_type.is_indexed() {
+                            return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
+                        }
+
                         let mut phrase_pairs = pre_term.into_inner();
                         let words = match phrase_pairs.next() {
                             None => return Ok(vec![]),
                             Some(words) => words,
                         };
                         let slop = phrase_pairs
                             .next()
@@ -436,14 +456,17 @@
                             return Err(QueryParserError::FieldDoesNotHavePositionsIndexed(field_entry.name().to_string()));
                         }
                         let query = Box::new(PhraseQuery::new_with_offset_and_slop(terms, slop)) as Box<dyn Query>;
                         return Ok(vec![boost_query(query, boost)]);
                     }
                     Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                     Rule::regex => {
+                        if !field_type.is_indexed() {
+                            return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
+                        }
                         let query = Box::new(
                             RegexQuery::from_pattern(pre_term.clone().into_inner().next().expect("grammar failure").as_str(), *field)
                                 .map_err(|_| QueryParserError::Syntax(pre_term.as_str().to_string()))?,
                         ) as Box<dyn Query>;
                         return Ok(vec![boost_query(query, boost)]);
                     }
                     _ => unreachable!(),
```

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.15.8/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/Cargo.toml` & `summa_embed-0.15.8/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "summa-embed-py"
-version = "0.15.7"
+version = "0.15.8"
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
-summa-core = { version = "0.15.7", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.15.8", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.15.7/.gitignore` & `summa_embed-0.15.8/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/pyproject.toml` & `summa_embed-0.15.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/src/lib.rs` & `summa_embed-0.15.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/__init__.py` & `summa_embed-0.15.8/summa_embed/__init__.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/consumer_service_pb2.py` & `summa_embed-0.15.8/summa_embed/proto/consumer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/consumer_service_pb2.pyi` & `summa_embed-0.15.8/summa_embed/proto/consumer_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/dag_pb_pb2.py` & `summa_embed-0.15.8/summa_embed/proto/dag_pb_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/dag_pb_pb2.pyi` & `summa_embed-0.15.8/summa_embed/proto/dag_pb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/index_service_pb2.py` & `summa_embed-0.15.8/summa_embed/proto/index_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/index_service_pb2.pyi` & `summa_embed-0.15.8/summa_embed/proto/index_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/query_pb2.py` & `summa_embed-0.15.8/summa_embed/proto/query_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/query_pb2.pyi` & `summa_embed-0.15.8/summa_embed/proto/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/reflection_service_pb2.py` & `summa_embed-0.15.8/summa_embed/proto/reflection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/reflection_service_pb2.pyi` & `summa_embed-0.15.8/summa_embed/proto/reflection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/search_service_pb2.py` & `summa_embed-0.15.8/summa_embed/proto/search_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/search_service_pb2.pyi` & `summa_embed-0.15.8/summa_embed/proto/search_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/unixfs_pb2.py` & `summa_embed-0.15.8/summa_embed/proto/unixfs_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/unixfs_pb2.pyi` & `summa_embed-0.15.8/summa_embed/proto/unixfs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/summa_embed/proto/utils_pb2.py` & `summa_embed-0.15.8/summa_embed/proto/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.7/Cargo.lock` & `summa_embed-0.15.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1790,17 +1790,17 @@
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "111.25.3+1.1.1t"
+version = "111.26.0+1.1.1u"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "924757a6a226bf60da5f7dd0311a34d2b52283dd82ddeb103208ddc66362f80c"
+checksum = "efc62c9f12b22b8f5208c23a7200a442b2e5999f8bdf80233852122b5a4f6f37"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
 version = "0.9.88"
@@ -2912,15 +2912,15 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "summa-core"
-version = "0.15.7"
+version = "0.15.8"
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
-version = "0.15.7"
+version = "0.15.8"
 dependencies = [
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
  "pythonize",
  "serde_json",
```

