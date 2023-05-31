# Comparing `tmp/summa_embed-0.15.0.tar.gz` & `tmp/summa_embed-0.15.4.tar.gz`

## Comparing `summa_embed-0.15.0.tar` & `summa_embed-0.15.4.tar`

### file list

```diff
@@ -1,86 +1,106 @@
--rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 summa_embed-0.15.0/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20       92 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7087 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5015 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20     1021 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/driver.rs
--rw-r--r--   0      501       20    13794 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    24562 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13833 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    14335 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5038 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     4711 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      163 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20    14304 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1589 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    53916 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     2216 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11168 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7439 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     3093 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8014 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5490 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      450 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 summa_embed-0.15.0/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2262 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10377 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7125 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2353 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      424 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 summa_embed-0.15.0/Cargo.toml
--rw-r--r--   0      501       20      685 2023-05-27 21:56:58.000000 summa_embed-0.15.0/.gitignore
--rw-r--r--   0      501       20      373 2023-05-27 21:56:58.000000 summa_embed-0.15.0/pyproject.toml
--rw-r--r--   0      501       20     4324 2023-05-27 21:56:58.000000 summa_embed-0.15.0/src/lib.rs
--rw-r--r--   0      501       20   100911 2023-05-27 21:57:10.000000 summa_embed-0.15.0/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.15.0/PKG-INFO
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.15.4/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2262 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10419 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7125 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2353 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      424 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 summa_embed-0.15.4/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20       92 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7087 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5015 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20     1021 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/driver.rs
+-rw-r--r--   0      501       20    13794 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    24562 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13833 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    14335 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5038 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     4711 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      163 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20    15871 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1595 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    56532 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     2216 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11274 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7439 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     3093 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8014 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5490 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      450 2023-05-31 08:41:21.000000 summa_embed-0.15.4/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 summa_embed-0.15.4/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-05-31 08:41:21.000000 summa_embed-0.15.4/.gitignore
+-rwxr-xr-x   0      501       20      347 2023-05-31 08:41:21.000000 summa_embed-0.15.4/build.sh
+-rw-r--r--   0      501       20      515 2023-05-31 08:41:21.000000 summa_embed-0.15.4/pyproject.toml
+-rw-r--r--   0      501       20       14 2023-05-31 08:41:21.000000 summa_embed-0.15.4/requirements.txt
+-rw-r--r--   0      501       20     4333 2023-05-31 08:41:21.000000 summa_embed-0.15.4/src/lib.rs
+-rw-r--r--   0      501       20     1050 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/__init__.py
+-rw-r--r--   0      501       20        0 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/__init__.py
+-rw-r--r--   0      501       20     3123 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/consumer_service_pb2.py
+-rw-r--r--   0      501       20     3080 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/consumer_service_pb2.pyi
+-rw-r--r--   0      501       20     1335 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/dag_pb_pb2.py
+-rw-r--r--   0      501       20     1042 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/dag_pb_pb2.pyi
+-rw-r--r--   0      501       20    16230 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/index_service_pb2.py
+-rw-r--r--   0      501       20    19481 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/index_service_pb2.pyi
+-rw-r--r--   0      501       20    21461 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/query_pb2.py
+-rw-r--r--   0      501       20    29337 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/query_pb2.pyi
+-rw-r--r--   0      501       20     2213 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/reflection_service_pb2.py
+-rw-r--r--   0      501       20     1923 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/reflection_service_pb2.pyi
+-rw-r--r--   0      501       20     2012 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/search_service_pb2.py
+-rw-r--r--   0      501       20     1830 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/search_service_pb2.pyi
+-rw-r--r--   0      501       20     1741 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/unixfs_pb2.py
+-rw-r--r--   0      501       20     1598 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/unixfs_pb2.pyi
+-rw-r--r--   0      501       20     1040 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/utils_pb2.py
+-rw-r--r--   0      501       20      454 2023-05-31 08:41:21.000000 summa_embed-0.15.4/summa_embed/proto/utils_pb2.pyi
+-rw-r--r--   0      501       20   102226 2023-05-31 08:43:47.000000 summa_embed-0.15.4/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.15.4/PKG-INFO
```

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.15.4/local_dependencies/summa-core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.15.0"
+version = "0.15.5"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
@@ -29,15 +29,15 @@
 futures = "0.3"
 hyper = { version = "0.14", default_features = false, features = ["client", "http1", "http2", "tcp"] , optional = true }
 hyper-tls = { version = "0.5.0", features = ["vendored"] , optional = true }
 instant = { version = "0.1", default_features = false, features = [ "inaccurate", "wasm-bindgen" ] }
 itertools = "0.10"
 lru = "0.10.0"
 oneshot = "0.1"
-opentelemetry = { version = "0.18", features = ["rt-tokio"], optional = true }
+opentelemetry = { version = "0.19", features = ["metrics", "rt-tokio"], optional = true }
 parking_lot = { version = "0.12", features = ["send_guard"] }
 pest = "2.5"
 pest_derive = "2.5"
 prost = "0.11"
 rand = { version = "0.8", features = ["small_rng"] }
 rayon = "1.6.1"
 safe-regex = "0.2.5"
```

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/LICENSE` & `summa_embed-0.15.4/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/driver.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/driver.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #[cfg(feature = "metrics")]
 use opentelemetry::metrics::Counter;
 #[cfg(feature = "metrics")]
 use opentelemetry::Context;
 #[cfg(feature = "metrics")]
 use opentelemetry::{global, KeyValue};
 use summa_proto::proto;
+use tantivy::json_utils::{convert_to_fast_value_and_get_term, JsonTermWriter};
 use tantivy::query::{
     AllQuery, BooleanQuery, BoostQuery, DisjunctionMaxQuery, EmptyQuery, MoreLikeThisQuery, Occur, PhraseQuery, Query, RangeQuery, RegexQuery, TermQuery,
 };
 use tantivy::schema::{Field, FieldEntry, FieldType, IndexRecordOption, Schema};
 use tantivy::{DateTime, Index, Score, Term};
 use tracing::{info, warn};
 
@@ -48,17 +49,25 @@
             Some(proto::match_query::DefaultMode::DisjuctionMaxMode(proto::MatchQueryDisjuctionMaxMode { tie_breaker })) => {
                 MatchQueryDefaultMode::DisjuctionMax { tie_breaker }
             }
         }
     }
 }
 
-fn cast_value_to_term(field: Field, field_type: &FieldType, value: &str) -> SummaResult<Term> {
+fn cast_value_to_term(field: Field, full_path: &str, field_type: &FieldType, value: &str) -> SummaResult<Term> {
     Ok(match field_type {
         FieldType::Str(_) => Term::from_field_text(field, value),
+        FieldType::JsonObject(json_options) => {
+            let mut term = Term::with_capacity(128);
+            let mut json_term_writer = JsonTermWriter::from_field_and_json_path(field, full_path, json_options.is_expand_dots_enabled(), &mut term);
+            convert_to_fast_value_and_get_term(&mut json_term_writer, value).unwrap_or_else(|| {
+                json_term_writer.set_str(value.trim_matches(|c| c == '\'' || c == '\"'));
+                json_term_writer.term().clone()
+            })
+        }
         FieldType::I64(_) => Term::from_field_i64(
             field,
             i64::from_str(value).map_err(|_e| Error::InvalidSyntax(format!("cannot parse {value} as i64")))?,
         ),
         FieldType::U64(_) => Term::from_field_u64(
             field,
             u64::from_str(value).map_err(|_e| Error::InvalidSyntax(format!("cannot parse {value} as u64")))?,
@@ -77,19 +86,19 @@
             field,
             DateTime::from_timestamp_secs(i64::from_str(value).map_err(|_e| Error::InvalidSyntax(format!("cannot parse {value} as date")))?),
         ),
         _ => return Err(Error::InvalidSyntax("invalid range type".to_owned())),
     })
 }
 
-fn cast_value_to_bound_term(field: Field, field_type: &FieldType, value: &str, including: bool) -> SummaResult<Bound<Term>> {
+fn cast_value_to_bound_term(field: Field, full_path: &str, field_type: &FieldType, value: &str, including: bool) -> SummaResult<Bound<Term>> {
     Ok(match value {
         "*" => Unbounded,
         value => {
-            let casted_value = cast_value_to_term(field, field_type, value)?;
+            let casted_value = cast_value_to_term(field, full_path, field_type, value)?;
             if including {
                 Bound::Included(casted_value)
             } else {
                 Bound::Excluded(casted_value)
             }
         }
     })
@@ -114,18 +123,22 @@
             #[cfg(feature = "metrics")]
             subquery_counter,
             index_default_fields,
         })
     }
 
     #[inline]
-    pub(crate) fn field_and_field_entry(&self, field_name: &str) -> SummaResult<(Field, &FieldEntry)> {
-        let field = self.cached_schema.get_field(field_name)?;
-        let field_entry = self.cached_schema.get_field_entry(field);
-        Ok((field, field_entry))
+    pub(crate) fn field_and_field_entry<'a>(&'a self, field_name: &'a str) -> SummaResult<(Field, &str, &FieldEntry)> {
+        match self.cached_schema.find_field(field_name) {
+            Some((field, full_path)) => {
+                let field_entry = self.cached_schema.get_field_entry(field);
+                Ok((field, full_path, field_entry))
+            }
+            None => Err(ValidationError::MissingField(field_name.to_string()).into()),
+        }
     }
 
     fn parse_subquery(&self, query: proto::query::Query) -> SummaResult<Box<dyn Query>> {
         #[cfg(feature = "metrics")]
         self.subquery_counter.add(
             &Context::current(),
             1,
@@ -191,57 +204,57 @@
                         Ok(parsed_query)
                     }
                     Err(QueryParserError::FieldDoesNotExist(field)) => Err(ValidationError::MissingField(field).into()),
                     Err(e) => Err(Error::InvalidQuerySyntax(Box::new(e), match_query_proto.value.to_owned())),
                 }?
             }
             proto::query::Query::Range(range_query_proto) => {
-                let (field, field_entry) = self.field_and_field_entry(&range_query_proto.field)?;
+                let (field, full_path, field_entry) = self.field_and_field_entry(&range_query_proto.field)?;
                 let value = range_query_proto.value.as_ref().ok_or(ValidationError::MissingRange)?;
-                let left = cast_value_to_bound_term(field, field_entry.field_type(), &value.left, value.including_left)?;
-                let right = cast_value_to_bound_term(field, field_entry.field_type(), &value.right, value.including_right)?;
+                let left = cast_value_to_bound_term(field, full_path, field_entry.field_type(), &value.left, value.including_left)?;
+                let right = cast_value_to_bound_term(field, full_path, field_entry.field_type(), &value.right, value.including_right)?;
                 Box::new(RangeQuery::new_term_bounds(
                     range_query_proto.field.clone(),
                     field_entry.field_type().value_type(),
                     &left,
                     &right,
                 ))
             }
             proto::query::Query::Boost(boost_query_proto) => Box::new(BoostQuery::new(
                 self.parse_subquery(boost_query_proto.query.and_then(|query| query.query).ok_or(Error::EmptyQuery)?)?,
                 f32::from_str(&boost_query_proto.score).map_err(|_e| Error::InvalidSyntax(format!("cannot parse {} as f32", boost_query_proto.score)))?,
             )),
             proto::query::Query::Regex(regex_query_proto) => {
-                let (field, _) = self.field_and_field_entry(&regex_query_proto.field)?;
+                let (field, _, _) = self.field_and_field_entry(&regex_query_proto.field)?;
                 Box::new(RegexQuery::from_pattern(&regex_query_proto.value, field)?)
             }
             proto::query::Query::Phrase(phrase_query_proto) => {
-                let (field, field_entry) = self.field_and_field_entry(&phrase_query_proto.field)?;
+                let (field, full_path, field_entry) = self.field_and_field_entry(&phrase_query_proto.field)?;
                 let tokenizer = self.index.tokenizer_for_field(field)?;
 
                 let mut token_stream = tokenizer.token_stream(&phrase_query_proto.value);
                 let mut terms: Vec<(usize, Term)> = vec![];
                 while let Some(token) = token_stream.next() {
-                    terms.push((token.position, cast_value_to_term(field, field_entry.field_type(), &token.text)?))
+                    terms.push((token.position, cast_value_to_term(field, full_path, field_entry.field_type(), &token.text)?))
                 }
                 if terms.is_empty() {
                     Box::new(EmptyQuery)
                 } else if terms.len() == 1 {
                     Box::new(TermQuery::new(
                         terms[0].1.clone(),
                         field_entry.field_type().index_record_option().unwrap_or(IndexRecordOption::Basic),
                     ))
                 } else {
                     Box::new(PhraseQuery::new_with_offset_and_slop(terms, phrase_query_proto.slop))
                 }
             }
             proto::query::Query::Term(term_query_proto) => {
-                let (field, field_entry) = self.field_and_field_entry(&term_query_proto.field)?;
+                let (field, full_path, field_entry) = self.field_and_field_entry(&term_query_proto.field)?;
                 Box::new(TermQuery::new(
-                    cast_value_to_term(field, field_entry.field_type(), &term_query_proto.value)?,
+                    cast_value_to_term(field, full_path, field_entry.field_type(), &term_query_proto.value)?,
                     field_entry.field_type().index_record_option().unwrap_or(IndexRecordOption::Basic),
                 ))
             }
             proto::query::Query::MoreLikeThis(more_like_this_query_proto) => {
                 let document = self
                     .cached_schema
                     .parse_document(&more_like_this_query_proto.document)
@@ -274,16 +287,27 @@
                     query_builder =
                         query_builder.with_boost_factor(f32::from_str(boost).map_err(|_e| Error::InvalidSyntax(format!("cannot parse {boost} as f32")))?);
                 }
                 query_builder = query_builder.with_stop_words(more_like_this_query_proto.stop_words);
                 Box::new(query_builder.with_document_fields(field_values))
             }
             proto::query::Query::Exists(exists_query_proto) => {
-                let (field, _) = self.field_and_field_entry(&exists_query_proto.field)?;
-                Box::new(ExistsQuery::new(field))
+                let (field, full_path, field_entry) = self.field_and_field_entry(&exists_query_proto.field)?;
+                if !field_entry.field_type().is_indexed() {
+                    let fni = QueryParserError::FieldNotIndexed(field_entry.name().to_string());
+                    return Err(Error::InvalidQuerySyntax(Box::new(fni), exists_query_proto.field.to_string()));
+                }
+                if full_path == "" {
+                    Box::new(ExistsQuery::new(field))
+                } else {
+                    Box::new(TermQuery::new(
+                        cast_value_to_term(field, full_path, field_entry.field_type(), "")?,
+                        field_entry.field_type().index_record_option().unwrap_or(IndexRecordOption::Basic),
+                    ))
+                }
             }
         })
     }
 
     pub fn parse_query(&self, query: proto::query::Query) -> SummaResult<Box<dyn Query>> {
         #[cfg(feature = "metrics")]
         self.query_counter.add(
```

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 doi = @{ "10." ~ ASCII_DIGIT{4,9} ~ WHITE_SPACE? ~ "/" ~ WHITE_SPACE? ~ (!WHITE_SPACE ~ ANY)+ }
 wrapped_doi = _{ ("http" ~ "s"? ~ "://")? ~ "doi.org/"? ~ doi }
 
 slop = @{ DECIMAL_NUMBER+ }
 boost = { (DECIMAL_NUMBER | ".")+ }
 range = ${ "[" ~ WHITE_SPACE* ~ boundary_word ~ WHITE_SPACE+ ~ ^"to" ~ WHITE_SPACE+ ~ boundary_word ~ WHITE_SPACE* ~ "]" }
 
-field_name = @{ ASCII_ALPHA ~ (ASCII_ALPHANUMERIC | "_")* }
+field_name = @{ ASCII_ALPHA ~ (ASCII_ALPHANUMERIC | "_" | ".")* }
 word = @{ wrapped_doi | ((LETTER | NUMBER) ~ (LETTER | NUMBER | "_" | "+" | "#" | "-" | "–")*) }
 
 boundary_word = _{ star | word }
 phrase_internals = { (!quote ~ ANY)* }
 phrase = ${ quote ~ phrase_internals? ~ (quote | EOI) ~ ("~" ~ slop)? }
 regex_internals = ${ (!PEEK ~ ANY)* }
 regex = ${ PUSH("/"+) ~ regex_internals ~ POP }
```

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 use std::str::FromStr;
 
 use pest::iterators::{Pair, Pairs};
 use pest::Parser;
 use pest_derive::Parser;
 use safe_regex::{regex, Matcher3};
 use summa_proto::proto;
+use tantivy::json_utils::{convert_to_fast_value_and_get_term, JsonTermWriter};
 use tantivy::query::{BooleanQuery, BoostQuery, DisjunctionMaxQuery, EmptyQuery, PhraseQuery, Query, QueryClone, RangeQuery, RegexQuery, TermQuery};
 use tantivy::schema::{FacetParseError, Field, FieldEntry, FieldType, IndexRecordOption, Schema, TextFieldIndexing, Type};
 use tantivy::tokenizer::{TextAnalyzer, TokenizerManager};
 use tantivy::{Index, Term};
 use tantivy_common::HasLen;
 use tantivy_query_grammar::Occur;
 
@@ -32,14 +33,15 @@
 
 pub struct QueryParser {
     schema: Schema,
     default_fields: Vec<Field>,
     tokenizer_manager: TokenizerManager,
     missing_field_policy: MissingFieldPolicy,
     limit: usize,
+    field_aliases: HashMap<String, String>,
     field_boosts: Option<HashMap<String, f32>>,
     default_mode: MatchQueryDefaultMode,
     exact_matches_promoter: Option<proto::ExactMatchesPromoter>,
 }
 
 /// Possible error that may happen when parsing a query.
 #[derive(thiserror::Error, Debug, PartialEq)]
@@ -76,14 +78,20 @@
     /// field specified is forbbidden.
     #[error("No default field declared and no field specified in query")]
     NoDefaultFieldDeclared,
     /// The field searched for is not declared
     /// as indexed in the schema.
     #[error("field_not_indexed_error: {0}")]
     FieldNotIndexed(String),
+    /// The field is declated as JSON but the query does not contain object path
+    #[error("json_field_without_path_error: {0}")]
+    JsonFieldWithoutPath(String),
+    /// The field is not declated as JSON but the query does contain object path
+    #[error("non_json_field_with_path_error: {0}")]
+    NonJsonFieldWithPath(String),
     /// A phrase query was requested for a field that does not
     /// have any positions indexed.
     #[error("field_does_not_have_positions_indexed_error: {0}")]
     FieldDoesNotHavePositionsIndexed(String),
     /// The tokenizer for the given field is unknown
     /// The two argument strings are the name of the field, the name of the tokenizer
     #[error("unknown_tokenizer_error: '{tokenizer:?}' for the field '{field:?}'")]
@@ -187,24 +195,29 @@
         let default_fields = validators::parse_fields(&schema, &default_fields)?;
         Ok(QueryParser {
             schema,
             default_fields,
             tokenizer_manager: tokenizer_manager.clone(),
             missing_field_policy: MissingFieldPolicy::Remove,
             limit: 16,
+            field_aliases: HashMap::new(),
             field_boosts: None,
             default_mode: MatchQueryDefaultMode::Boolean,
             exact_matches_promoter: None,
         })
     }
 
     pub fn for_index(index: &Index, default_fields: Vec<String>) -> SummaResult<QueryParser> {
         QueryParser::new(index.schema(), default_fields, index.tokenizers())
     }
 
+    pub fn set_field_aliases(&mut self, field_aliases: HashMap<String, String>) {
+        self.field_aliases = field_aliases;
+    }
+
     pub fn set_field_boosts(&mut self, field_boosts: HashMap<String, f32>) {
         self.field_boosts = Some(field_boosts);
     }
 
     pub fn set_default_mode(&mut self, default_mode: MatchQueryDefaultMode) {
         self.default_mode = default_mode;
     }
@@ -213,14 +226,18 @@
         self.missing_field_policy = missing_field_policy;
     }
 
     pub fn set_exact_match_promoter(&mut self, exact_matches_promoter: proto::ExactMatchesPromoter) {
         self.exact_matches_promoter = Some(exact_matches_promoter);
     }
 
+    pub fn resolve_field_name<'a>(&'a self, field_name: &'a str) -> &str {
+        self.field_aliases.get(field_name).map(|s| s.as_str()).unwrap_or(field_name)
+    }
+
     fn get_text_analyzer(&self, field_entry: &FieldEntry, option: &TextFieldIndexing) -> Result<TextAnalyzer, QueryParserError> {
         self.tokenizer_manager
             .get(option.tokenizer())
             .ok_or_else(|| QueryParserError::UnknownTokenizer {
                 field: field_entry.name().to_string(),
                 tokenizer: option.tokenizer().to_string(),
             })
@@ -229,15 +246,15 @@
     fn default_fields_term(&self, term: Pair<Rule>, boost: Option<f32>) -> Result<Box<dyn Query>, QueryParserError> {
         let term = term.into_inner().next().expect("grammar failure");
         let occur = self.parse_occur(&term);
         let pre_term = term.into_inner().next().expect("grammar failure");
         let default_field_queries = self
             .default_fields
             .iter()
-            .map(|field| self.parse_pre_term(field, pre_term.clone(), boost))
+            .map(|field| self.parse_pre_term(field, "", pre_term.clone(), boost))
             .collect::<Result<Vec<_>, _>>()?;
 
         Ok(match occur {
             Occur::Should => {
                 let default_field_queries = default_field_queries.into_iter().flatten();
                 match self.default_mode {
                     MatchQueryDefaultMode::Boolean => Box::new(BooleanQuery::new(default_field_queries.map(|q| (occur, q)).collect())) as Box<dyn Query>,
@@ -291,22 +308,34 @@
         token_stream.process(&mut |token| {
             let term = Term::from_field_text(field, &token.text);
             terms.push((token.position, term));
         });
         Ok(terms)
     }
 
-    fn parse_pre_term(&self, field: &Field, pre_term: Pair<Rule>, boost: Option<f32>) -> Result<Vec<Box<dyn Query>>, QueryParserError> {
+    fn parse_pre_term(&self, field: &Field, full_path: &str, pre_term: Pair<Rule>, boost: Option<f32>) -> Result<Vec<Box<dyn Query>>, QueryParserError> {
         let field_entry = self.schema.get_field_entry(*field);
         let field_type = field_entry.field_type();
 
         if !field_type.is_indexed() {
             return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
         }
 
+        if field_type.value_type() == Type::Json && full_path.is_empty() {
+            return Err(QueryParserError::JsonFieldWithoutPath(field_entry.name().to_string()));
+        }
+
+        if field_type.value_type() != Type::Json && !full_path.is_empty() {
+            return Err(QueryParserError::NonJsonFieldWithPath(format!(
+                "{}.{}",
+                field_entry.name().to_string(),
+                full_path
+            )));
+        }
+
         let boost = multiply_boosts(self.field_boosts.as_ref().and_then(|boosts| boosts.get(field_entry.name()).cloned()), boost);
 
         if matches!(pre_term.as_rule(), Rule::range) {
             return Ok(vec![boost_query(Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>, boost)]);
         }
 
         return match *field_type {
@@ -342,25 +371,46 @@
                 Rule::phrase | Rule::word => {
                     let val: bool = bool::from_str(pre_term.as_str())?;
                     let query = Box::new(TermQuery::new(Term::from_field_bool(*field, val), IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                     Ok(vec![boost_query(query, boost)])
                 }
                 _ => unreachable!(),
             },
-            FieldType::Str(ref str_options) => {
-                let option = str_options.get_indexing_options().expect("unreachable");
+            FieldType::Str(_) | FieldType::JsonObject(_) => {
+                let indexing = if let FieldType::Str(ref text_options) = field_type {
+                    text_options.get_indexing_options().expect("unreachable")
+                } else if let FieldType::JsonObject(ref json_options) = field_type {
+                    json_options.get_text_indexing_options().expect("unreachable")
+                } else {
+                    unreachable!()
+                };
+
                 match pre_term.as_rule() {
                     Rule::word | Rule::field_name => {
-                        let mut token_stream = self.get_text_analyzer(field_entry, option)?.token_stream(pre_term.as_str());
+                        let mut token_stream = self.get_text_analyzer(field_entry, indexing)?.token_stream(pre_term.as_str());
                         let mut queries = Vec::new();
 
                         token_stream.process(&mut |token| {
-                            let query = Box::new(TermQuery::new(Term::from_field_text(*field, &token.text), IndexRecordOption::WithFreqs)) as Box<dyn Query>;
+                            let term = match field_type {
+                                FieldType::Str(_) => Term::from_field_text(*field, &token.text),
+                                FieldType::JsonObject(ref json_options) => {
+                                    let mut term = Term::with_capacity(128);
+                                    let mut json_term_writer =
+                                        JsonTermWriter::from_field_and_json_path(*field, full_path, json_options.is_expand_dots_enabled(), &mut term);
+                                    convert_to_fast_value_and_get_term(&mut json_term_writer, &token.text).unwrap_or_else(|| {
+                                        json_term_writer.set_str(&token.text);
+                                        json_term_writer.term().clone()
+                                    })
+                                }
+                                _ => unreachable!(),
+                            };
+                            let query = Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                             queries.push(boost_query(query, boost));
                         });
+
                         Ok(queries)
                     }
                     Rule::phrase => {
                         let mut phrase_pairs = pre_term.into_inner();
                         let words = match phrase_pairs.next() {
                             None => return Ok(vec![]),
                             Some(words) => words,
@@ -368,25 +418,25 @@
                         let slop = phrase_pairs
                             .next()
                             .map(|v| match v.as_str() {
                                 "" => 0,
                                 _ => u32::from_str(v.as_str()).expect("cannot parse"),
                             })
                             .unwrap_or(0);
-                        let terms = self.parse_words(*field, option, words.as_str())?;
+                        let terms = self.parse_words(*field, indexing, words.as_str())?;
                         if terms.len() <= 1 {
                             return Ok(terms
                                 .into_iter()
                                 .map(|(_, term)| {
                                     let query = Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                                     boost_query(query, boost)
                                 })
                                 .collect());
                         }
-                        if !option.index_option().has_positions() {
+                        if !indexing.index_option().has_positions() {
                             return Err(QueryParserError::FieldDoesNotHavePositionsIndexed(field_entry.name().to_string()));
                         }
                         let query = Box::new(PhraseQuery::new_with_offset_and_slop(terms, slop)) as Box<dyn Query>;
                         return Ok(vec![boost_query(query, boost)]);
                     }
                     Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                     Rule::regex => {
@@ -408,20 +458,23 @@
             Rule::positive_term => Occur::Must,
             Rule::negative_term => Occur::MustNot,
             Rule::default_term => Occur::Should,
             _ => unreachable!(),
         }
     }
 
-    fn parse_term(&self, term: Pair<Rule>, field: &Field, boost: Option<f32>) -> Result<Box<dyn Query>, QueryParserError> {
+    fn parse_term(&self, term: Pair<Rule>, field: &Field, full_path: &str, boost: Option<f32>) -> Result<Box<dyn Query>, QueryParserError> {
         let term = term.into_inner().next().expect("grammar_failure");
         let occur = self.parse_occur(&term);
         let pre_term = term.into_inner().next().expect("grammar failure");
         Ok(Box::new(BooleanQuery::new(
-            self.parse_pre_term(field, pre_term, boost)?.into_iter().map(|q| (occur, q)).collect(),
+            self.parse_pre_term(field, full_path, pre_term, boost)?
+                .into_iter()
+                .map(|q| (occur, q))
+                .collect(),
         )))
     }
 
     fn compute_boundary_term(&self, field: Field, phrase: &str) -> Result<Term, QueryParserError> {
         let field_entry = self.schema.get_field_entry(field);
         let field_type = field_entry.field_type();
         let field_supports_ff_range_queries = field_type.is_fast() && is_type_valid_for_fastfield_range_query(field_type.value_type());
@@ -574,18 +627,18 @@
             Rule::search_group => {
                 let mut search_group = isbn_doi_or_search_group_or_term.into_inner();
                 let field_name = search_group.next().expect("grammar failure");
                 let grouping_or_term = search_group.next().expect("grammar failure");
                 match grouping_or_term.as_rule() {
                     Rule::grouping => {
                         let mut intermediate_results = vec![];
-                        match self.schema.get_field(field_name.as_str()) {
+                        match self.schema.get_field(self.resolve_field_name(field_name.as_str())) {
                             Ok(field) => {
                                 for term in grouping_or_term.into_inner() {
-                                    intermediate_results.push(self.parse_term(term, &field, statement_boost)?);
+                                    intermediate_results.push(self.parse_term(term, &field, "", statement_boost)?);
                                 }
                             }
                             Err(tantivy::TantivyError::FieldNotFound(_)) => match self.missing_field_policy {
                                 MissingFieldPolicy::AsUsualTerms => {
                                     intermediate_results.push(self.default_fields_term(field_name, statement_boost)?);
                                     for term in grouping_or_term.into_inner() {
                                         intermediate_results.push(self.default_fields_term(term, statement_boost)?)
@@ -594,25 +647,24 @@
                                 MissingFieldPolicy::Remove => return Ok(Box::new(EmptyQuery {})),
                                 MissingFieldPolicy::Fail => return Err(QueryParserError::FieldDoesNotExist(field_name.as_str().to_string())),
                             },
                             _ => unreachable!(),
                         }
                         Ok(Box::new(BooleanQuery::new(intermediate_results.into_iter().map(|q| (Occur::Should, q)).collect())) as Box<dyn Query>)
                     }
-                    Rule::term => match self.schema.get_field(field_name.as_str()) {
-                        Ok(field) => self.parse_term(grouping_or_term, &field, statement_boost),
-                        Err(tantivy::TantivyError::FieldNotFound(_)) => match self.missing_field_policy {
+                    Rule::term => match self.schema.find_field(self.resolve_field_name(field_name.as_str())) {
+                        Some((field, full_path)) => self.parse_term(grouping_or_term, &field, full_path, statement_boost),
+                        None => match self.missing_field_policy {
                             MissingFieldPolicy::AsUsualTerms => Ok(Box::new(BooleanQuery::new(vec![
                                 (Occur::Should, self.default_fields_term(field_name, statement_boost)?),
                                 (Occur::Should, self.default_fields_term(grouping_or_term, statement_boost)?),
                             ])) as Box<dyn Query>),
                             MissingFieldPolicy::Remove => Ok(Box::new(EmptyQuery {}) as Box<dyn Query>),
                             MissingFieldPolicy::Fail => Err(QueryParserError::FieldDoesNotExist(field_name.as_str().to_string())),
                         },
-                        _ => unreachable!(),
                     },
                     _ => unreachable!(),
                 }
             }
             Rule::doi => self.parse_doi(isbn_doi_or_search_group_or_term.as_str()),
             Rule::isbn => self.parse_isbn(isbn_doi_or_search_group_or_term.as_str()),
             Rule::term => self.default_fields_term(isbn_doi_or_search_group_or_term, statement_boost),
```

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 use std::net::IpAddr;
 use std::str::{from_utf8, FromStr};
 
 use base64::Engine;
-use serde_json::Value as JsonValue;
+use serde_json::{json, Value as JsonValue};
 use tantivy::schema::{Facet, FieldType, IntoIpv6Addr, Schema, Value};
 use tantivy::tokenizer::PreTokenizedString;
 use tantivy::{DateTime, Document};
 use time::format_description::well_known::Rfc3339;
 use time::OffsetDateTime;
 
 use crate::errors::{Error, SummaResult, ValidationError};
 use crate::page_rank::quantize_page_rank;
+use crate::utils::current_time;
 
 /// Wrapper for carrying `tantivy::Document` from various sources
 pub enum SummaDocument<'a> {
     BoundJsonBytes((&'a Schema, &'a [u8])),
     UnboundJsonBytes(&'a [u8]),
     TantivyDocument(Document),
 }
@@ -43,24 +44,25 @@
     #[error("The provided string is not valid JSON")]
     InvalidJson(String),
     /// One of the value node could not be parsed.
     #[error("The field '{0:?}' could not be parsed: {1:?}")]
     ValueError(String, ValueParsingError),
 }
 
-pub fn process_dynamic_fields(schema: &Schema, document: &mut Document) {
-    if let Ok(page_rank_field) = schema.get_field("page_rank") {
-        if let Ok(quantized_page_rank_field) = schema.get_field("quantized_page_rank") {
-            if let Some(page_rank_value) = document.get_first(page_rank_field) {
-                if let Some(page_rank_value) = page_rank_value.as_f64() {
-                    document.add_u64(quantized_page_rank_field, quantize_page_rank(page_rank_value))
-                }
+pub fn process_dynamic_fields(schema: &Schema, json_object: &mut serde_json::Map<String, JsonValue>) {
+    if schema.get_field("page_rank").is_ok() && schema.get_field("quantized_page_rank").is_ok() {
+        if let Some(page_rank_value) = json_object.get_mut("page_rank") {
+            if let Some(v) = page_rank_value.as_f64() {
+                json_object.insert("quantized_page_rank".to_string(), json!(quantize_page_rank(v)));
             }
         }
     }
+    if schema.get_field("updated_at").is_ok() {
+        json_object.insert("updated_at".to_string(), json!(current_time()));
+    }
 }
 
 impl<'a> SummaDocument<'a> {
     pub fn bound_with(self, schema: &'a Schema) -> SummaDocument {
         match self {
             SummaDocument::UnboundJsonBytes(json_bytes) => SummaDocument::BoundJsonBytes((schema, json_bytes)),
             SummaDocument::BoundJsonBytes((_, json_bytes)) => SummaDocument::BoundJsonBytes((schema, json_bytes)),
@@ -183,17 +185,18 @@
                 expected: field_type.value_type().name(),
                 json: json.clone(),
             }),
         }
     }
 
     /// Build a document object from a json-object.
-    pub fn parse_document(&self, schema: &Schema, doc_json: &str) -> SummaResult<Document> {
-        let json_obj: serde_json::Map<String, JsonValue> =
+    pub fn parse_and_setup_document(&self, schema: &Schema, doc_json: &str) -> SummaResult<Document> {
+        let mut json_obj: serde_json::Map<String, JsonValue> =
             serde_json::from_str(doc_json).map_err(|_| DocumentParsingError::InvalidJson(doc_json.to_owned()))?;
+        process_dynamic_fields(schema, &mut json_obj);
         self.json_object_to_doc(schema, json_obj)
     }
 
     /// Build a document object from a json-object.
     pub fn json_object_to_doc(&self, schema: &Schema, json_obj: serde_json::Map<String, JsonValue>) -> SummaResult<Document> {
         let mut doc = Document::default();
         for (field_name, json_value) in json_obj {
@@ -225,16 +228,15 @@
 impl<'a> TryInto<Document> for SummaDocument<'a> {
     type Error = Error;
 
     fn try_into(self) -> SummaResult<Document> {
         match self {
             SummaDocument::BoundJsonBytes((schema, json_bytes)) => {
                 let text_document = from_utf8(json_bytes).map_err(ValidationError::Utf8)?;
-                let mut parsed_document = self.parse_document(schema, text_document)?;
-                process_dynamic_fields(schema, &mut parsed_document);
+                let parsed_document = self.parse_and_setup_document(schema, text_document)?;
                 Ok(parsed_document)
             }
             SummaDocument::UnboundJsonBytes(_) => Err(Error::UnboundDocument),
             SummaDocument::TantivyDocument(document) => Ok(document),
         }
     }
 }
```

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-use tantivy::aggregation::agg_req::Aggregation;
 use summa_proto::proto;
+use tantivy::aggregation::agg_req::Aggregation;
 use tantivy::aggregation::agg_result::{AggregationResult, BucketEntries, BucketEntry, BucketResult, MetricResult, RangeBucketEntry};
 use tantivy::aggregation::Key;
 
 use crate::errors::Error;
 use crate::proto_traits::Wrapper;
 
 impl TryFrom<Wrapper<proto::Aggregation>> for Aggregation {
```

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.15.4/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.15.4/local_dependencies/summa-proto/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 [features]
 default = ["grpc"]
 grpc = ["tonic", "tonic-build", "tonic-reflection"]
 
 [build-dependencies]
 prost-build = { version = "0.11.0" }
 protoc-bin-vendored = "3.0.0"
-tonic-build = { version = "0.8.0", default-features = false, features = ["prost", "transport"], optional = true }
+tonic-build = { version = "0.9", default-features = false, features = ["prost", "transport"], optional = true }
 
 [dependencies]
 prost = "0.11.0"
 prost-types = "0.11.0"
 serde = { version = "1.0", default_features = false, features = ["derive", "std"] }
-tonic = { version = "0.8.0", features = ["gzip"], optional = true }
-tonic-build = { version = "0.8.0", default-features = false, features = ["prost", "transport"], optional = true }
-tonic-reflection = { version = "0.6.0", optional = true }
+tonic = { version = "0.9", features = ["gzip"], optional = true }
+tonic-build = { version = "0.9", default-features = false, features = ["prost", "transport"], optional = true }
+tonic-reflection = { version = "0.9", optional = true }
```

### Comparing `summa_embed-0.15.0/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.15.4/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-proto/build.rs` & `summa_embed-0.15.4/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.15.4/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.15.4/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.15.4/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files 0% similar despite different names*

```diff
@@ -350,14 +350,15 @@
   oneof config {
     FileEngineConfig file = 1;
     MemoryEngineConfig memory = 2;
     RemoteEngineConfig remote = 3;
   }
   // Merge policy
   MergePolicy merge_policy = 10;
+  map<string, string> field_aliases = 11;
 }
 
 // Description containing `Index` metadata fields
 message IndexDescription {
   string index_name = 1;
   // All index aliases
   repeated string index_aliases = 2;
```

### Comparing `summa_embed-0.15.0/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.15.4/local_dependencies/summa-proto/proto/query.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.15.4/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.15.4/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.15.4/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.15.4/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/Cargo.toml` & `summa_embed-0.15.4/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [package]
 name = "summa-embed-py"
-version = "0.15.0"
+version = "0.15.4"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
 
 [dependencies]
 futures = "0.3"
+prost = "0.11"
 pyo3 = { version = "0.18", features = ["serde"] }
 pyo3-asyncio = { version =  "0.18", features = ["attributes", "tokio-runtime"] }
 pythonize = "0.18"
 serde_json = "1.0"
-summa-core = { version = "0.15.0", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.15.5", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.15.0/.gitignore` & `summa_embed-0.15.4/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.0/src/lib.rs` & `summa_embed-0.15.4/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 use std::sync::Arc;
 
 use futures::future::join_all;
+use prost::Message;
 use pyo3::exceptions::PyOSError;
 use pyo3::prelude::*;
-use pythonize::{depythonize, pythonize};
+use pyo3::types::PyBytes;
+use pythonize::{pythonize};
 use summa_core::components::{Driver, IndexHolder};
 use summa_core::configs::{ConfigProxy, DirectProxy};
 use summa_core::directories::DefaultExternalRequestGenerator;
 use summa_core::hyper_external_request::HyperExternalRequest;
 use summa_proto::proto;
-use summa_proto::proto::IndexEngineConfig;
 use tantivy::IndexBuilder;
 
 struct SummaPyError(String);
 
 impl From<summa_core::Error> for SummaPyError {
     fn from(value: summa_core::Error) -> Self {
         SummaPyError(format!("{:?}", value))
@@ -45,16 +46,16 @@
         let core_config = Arc::new(DirectProxy::new(core_config)) as Arc<dyn ConfigProxy<_>>;
         IndexRegistry {
             index_registry: summa_core::components::IndexRegistry::new(&core_config),
             core_config,
         }
     }
 
-    fn add<'a>(&'a self, py: Python<'a>, index_engine_config: PyObject, index_name: Option<String>) -> PyResult<&'a PyAny> {
-        let index_engine_config: IndexEngineConfig = depythonize(index_engine_config.as_ref(py)).unwrap();
+    fn add<'a>(&'a self, py: Python<'a>, index_engine_config: &PyBytes, index_name: Option<String>) -> PyResult<&'a PyAny> {
+        let index_engine_config = proto::IndexEngineConfig::decode(index_engine_config.as_bytes()).unwrap();
         let this = self.clone();
         pyo3_asyncio::tokio::future_into_py(py, async move {
             let index = match &index_engine_config.config {
                 Some(proto::index_engine_config::Config::Memory(memory_engine_config)) => {
                     let schema = serde_json::from_str(&memory_engine_config.schema).unwrap();
                     let index_builder = IndexBuilder::new().schema(schema);
                     IndexHolder::create_memory_index(index_builder).unwrap()
@@ -84,26 +85,26 @@
             .unwrap();
             let index_attributes = index_holder.index_attributes().cloned();
             this.index_registry.add(index_holder).await.unwrap();
             Ok(Python::with_gil(|py| pythonize(py, &index_attributes).unwrap()))
         })
     }
 
-    fn search<'a>(&'a self, py: Python<'a>, index_queries: PyObject) -> PyResult<&'a PyAny> {
-        let index_queries: Vec<proto::IndexQuery> = depythonize(index_queries.as_ref(py)).unwrap();
+    fn search<'a>(&'a self, py: Python<'a>, index_queries: &PyBytes) -> PyResult<&'a PyAny> {
+        let search_request = proto::SearchRequest::decode(index_queries.as_bytes()).unwrap();
         let this = self.clone();
         pyo3_asyncio::tokio::future_into_py(py, async move {
-            let futures = this.index_registry.search_futures(index_queries).unwrap();
+            let futures = this.index_registry.search_futures(search_request.index_queries).unwrap();
             let extraction_results = join_all(futures).await.into_iter().map(|r| r.expect("cannot receive")).collect::<Vec<_>>();
             let result = this.index_registry.finalize_extraction(extraction_results).await.unwrap();
             Ok(Python::with_gil(|py| pythonize(py, &result).unwrap()))
         })
     }
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
-#[pyo3(name = "summa_embed")]
-fn summa_embed(_py: Python, m: &PyModule) -> PyResult<()> {
+#[pyo3(name = "summa_embed_bin")]
+fn summa_embed_bin(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<IndexRegistry>()?;
     Ok(())
 }
```

### Comparing `summa_embed-0.15.0/Cargo.lock` & `summa_embed-0.15.4/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -713,15 +713,15 @@
 [[package]]
 name = "examples"
 version = "0.0.0"
 dependencies = [
  "serde_json",
  "summa-proto 0.26.0",
  "tokio",
- "tonic",
+ "tonic 0.9.2",
 ]
 
 [[package]]
 name = "fail"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe5e43d0f78a42ad591453aedb1d7ae631ce7ee445c7643691055a9ed8d3b01c"
@@ -835,17 +835,17 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "fs4"
-version = "0.6.4"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7f5b6908aecca5812a4569056285e58c666588c9573ee59765bf1d3692699e2"
+checksum = "7672706608ecb74ab2e055c68327ffc25ae4cac1e12349204fd5fb0f3487cce2"
 dependencies = [
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "fuchsia-cprng"
@@ -1467,20 +1467,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "loom"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff50ecb28bb86013e935fb6683ab1f6d3a20016f123c76fd4c27470076ac30f5"
 dependencies = [
@@ -1595,22 +1592,21 @@
 checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.6"
+version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
- "log",
  "wasi",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "multibase"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b3539ec3c1f04ac9748a260728e855f261b4977f5c3406612c884564f329404"
@@ -1747,32 +1743,32 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "oneshot"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc22d22931513428ea6cc089e942d38600e3d00976eef8c86de6b8a3aadec6eb"
 dependencies = [
  "loom",
 ]
 
 [[package]]
 name = "openssl"
-version = "0.10.52"
+version = "0.10.53"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01b8574602df80f7b85fdfc5392fa884a4e3b3f4f35402c070ab34c3d3f78d56"
+checksum = "12df40a956736488b7b44fe79fe12d4f245bb5b3f5a1f6095e499760015be392"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
@@ -1803,67 +1799,67 @@
 checksum = "924757a6a226bf60da5f7dd0311a34d2b52283dd82ddeb103208ddc66362f80c"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.87"
+version = "0.9.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e17f59264b2809d77ae94f0e1ebabc434773f370d6ca667bd223ea10e06cc7e"
+checksum = "c2ce0f250f34a308dcfdbb351f511359857d4ed2134ba715a4eadd46e1ffd617"
 dependencies = [
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "opentelemetry"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69d6c3d7288a106c0a363e4b0e8d308058d56902adefb16f4936f417ffef086e"
+checksum = "5f4b8347cc26099d3aeee044065ecc3ae11469796b4d65d065a23a584ed92a6f"
 dependencies = [
  "opentelemetry_api",
  "opentelemetry_sdk",
 ]
 
 [[package]]
 name = "opentelemetry-prometheus"
-version = "0.11.0"
+version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06c3d833835a53cf91331d2cfb27e9121f5a95261f31f08a1f79ab31688b8da8"
+checksum = "9a9f186f6293ebb693caddd0595e66b74a6068fa51048e26e0bf9c95478c639c"
 dependencies = [
  "opentelemetry",
  "prometheus",
  "protobuf",
 ]
 
 [[package]]
 name = "opentelemetry_api"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c24f96e21e7acc813c7a8394ee94978929db2bcc46cf6b5014fc612bf7760c22"
+checksum = "ed41783a5bf567688eb38372f2b7a8530f5a607a4b49d38dd7573236c23ca7e2"
 dependencies = [
  "fnv",
  "futures-channel",
  "futures-util",
  "indexmap",
- "js-sys",
  "once_cell",
  "pin-project-lite",
  "thiserror",
+ "urlencoding",
 ]
 
 [[package]]
 name = "opentelemetry_sdk"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ca41c4933371b61c2a2f214bf16931499af4ec90543604ec828f7a625c09113"
+checksum = "8b3a2a91fdbfdd4d212c0dcc2ab540de2c2bcbbd90be17de7a7daf8822d010c1"
 dependencies = [
  "async-trait",
  "crossbeam-channel",
  "dashmap",
  "fnv",
  "futures-channel",
  "futures-executor",
@@ -1892,15 +1888,15 @@
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "ownedbytes"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
@@ -2734,17 +2730,17 @@
 checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
-version = "0.4.5"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b4c031cd0d9014307d82b8abf653c0290fbdaeb4c02d00c63cf52f728628bf"
+checksum = "f3b143e2833c57ab9ad3ea280d21fd34e285a42837aeb0ee301f4f41890fa00e"
 dependencies = [
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
@@ -2916,15 +2912,15 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "summa-core"
-version = "0.15.0"
+version = "0.15.5"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bytes",
  "config",
  "derive_builder",
@@ -2962,17 +2958,18 @@
  "time",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.15.0"
+version = "0.15.4"
 dependencies = [
  "futures",
+ "prost",
  "pyo3",
  "pyo3-asyncio",
  "pythonize",
  "serde_json",
  "summa-core",
  "summa-proto 0.26.0",
  "tantivy",
@@ -2985,33 +2982,33 @@
 dependencies = [
  "prost",
  "prost-build",
  "prost-types",
  "protoc-bin-vendored",
  "serde",
  "tokio",
- "tonic",
- "tonic-build",
- "tonic-reflection",
+ "tonic 0.9.2",
+ "tonic-build 0.9.2",
+ "tonic-reflection 0.9.2",
 ]
 
 [[package]]
 name = "summa-proto"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11800e4c382bb5e8b6756e4fcaeb37a966e75f9c9796912e5066799587d81d00"
 dependencies = [
  "prost",
  "prost-build",
  "prost-types",
  "protoc-bin-vendored",
  "serde",
- "tonic",
- "tonic-build",
- "tonic-reflection",
+ "tonic 0.8.3",
+ "tonic-build 0.8.4",
+ "tonic-reflection 0.6.0",
 ]
 
 [[package]]
 name = "summa-server"
 version = "0.15.0"
 dependencies = [
  "anyhow",
@@ -3047,17 +3044,17 @@
  "tempdir",
  "thiserror",
  "tikv-jemallocator",
  "time",
  "tokio",
  "tokio-stream",
  "tokio-util",
- "tonic",
- "tonic-build",
- "tonic-reflection",
+ "tonic 0.9.2",
+ "tonic-build 0.9.2",
+ "tonic-reflection 0.9.2",
  "tonic-web",
  "tower",
  "tower-http",
  "tracing",
  "tracing-appender",
  "tracing-futures",
  "tracing-subscriber",
@@ -3134,15 +3131,15 @@
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f764005d11ee5f36500a149ace24e00e3da98b0158b3e2d53a7495660d3f4d60"
 
 [[package]]
 name = "tantivy"
 version = "0.19.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
 dependencies = [
  "aho-corasick",
  "arc-swap",
  "async-trait",
  "base64 0.21.2",
  "bitpacking",
  "byteorder",
@@ -3190,38 +3187,38 @@
  "winapi",
  "zstd",
 ]
 
 [[package]]
 name = "tantivy-bitpacker"
 version = "0.3.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
 dependencies = [
  "bitpacking",
 ]
 
 [[package]]
 name = "tantivy-columnar"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
 dependencies = [
  "fastdivide",
  "fnv",
  "itertools",
  "serde",
  "tantivy-bitpacker",
  "tantivy-common",
  "tantivy-sstable",
  "tantivy-stacker",
 ]
 
 [[package]]
 name = "tantivy-common"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
 dependencies = [
  "async-trait",
  "byteorder",
  "ownedbytes",
  "serde",
  "time",
 ]
@@ -3236,44 +3233,44 @@
  "regex-syntax 0.6.29",
  "utf8-ranges",
 ]
 
 [[package]]
 name = "tantivy-query-grammar"
 version = "0.19.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
 dependencies = [
  "combine",
  "once_cell",
  "regex",
 ]
 
 [[package]]
 name = "tantivy-sstable"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
 dependencies = [
  "izihawa-fst",
  "tantivy-common",
  "zstd",
 ]
 
 [[package]]
 name = "tantivy-stacker"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
 dependencies = [
  "murmurhash32",
  "tantivy-common",
 ]
 
 [[package]]
 name = "tantivy-tokenizer-api"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
@@ -3502,54 +3499,109 @@
  "tower-layer",
  "tower-service",
  "tracing",
  "tracing-futures",
 ]
 
 [[package]]
+name = "tonic"
+version = "0.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3082666a3a6433f7f511c7192923fa1fe07c69332d3c6a2e6bb040b569199d5a"
+dependencies = [
+ "async-trait",
+ "axum",
+ "base64 0.21.2",
+ "bytes",
+ "flate2",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "hyper",
+ "hyper-timeout",
+ "percent-encoding",
+ "pin-project",
+ "prost",
+ "tokio",
+ "tokio-stream",
+ "tower",
+ "tower-layer",
+ "tower-service",
+ "tracing",
+]
+
+[[package]]
 name = "tonic-build"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5bf5e9b9c0f7e0a7c027dcfaba7b2c60816c7049171f679d99ee2ff65d0de8c4"
 dependencies = [
  "prettyplease",
  "proc-macro2",
  "prost-build",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "tonic-build"
+version = "0.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a6fdaae4c2c638bb70fe42803a26fbd6fc6ac8c72f5c59f67ecc2a2dcabf4b07"
+dependencies = [
+ "prettyplease",
+ "proc-macro2",
+ "prost-build",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "tonic-reflection"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67494bad4dda4c9bffae901dfe14e2b2c0f760adb4706dc10beeb81799f7f7b2"
 dependencies = [
  "bytes",
  "prost",
  "prost-types",
  "tokio",
  "tokio-stream",
- "tonic",
+ "tonic 0.8.3",
+]
+
+[[package]]
+name = "tonic-reflection"
+version = "0.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0543d7092032041fbeac1f2c84304537553421a11a623c2301b12ef0264862c7"
+dependencies = [
+ "prost",
+ "prost-types",
+ "tokio",
+ "tokio-stream",
+ "tonic 0.9.2",
 ]
 
 [[package]]
 name = "tonic-web"
-version = "0.5.0"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9213351ad53b0dcf1c9cf7c372a47533446b1114928a9177bedc6c551e14b7cf"
+checksum = "21b00ec4842256d1fe0a46176e2ef5bc357664c66e7d91aff5a7d43d83a65f47"
 dependencies = [
- "base64 0.13.1",
+ "base64 0.21.2",
  "bytes",
  "futures-core",
  "http",
  "http-body",
  "hyper",
  "pin-project",
- "tonic",
+ "tonic 0.9.2",
  "tower-http",
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
@@ -3570,17 +3622,17 @@
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
 name = "tower-http"
-version = "0.3.5"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f873044bf02dd1e8239e9c1293ea39dad76dc594ec16185d0a1bf31d8dc8d858"
+checksum = "5d1d42a9b3f3ec46ba828e8d376aec14592ea199f70a06a548587ecd1c4ab658"
 dependencies = [
  "bitflags",
  "bytes",
  "futures-core",
  "futures-util",
  "http",
  "http-body",
@@ -3750,14 +3802,20 @@
 [[package]]
 name = "unsigned-varint"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d86a8dc7f45e4c1b0d30e43038c38f274e77af056aa5f74b93c2cf9eb3c1c836"
 
 [[package]]
+name = "urlencoding"
+version = "2.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e8db7427f936968176eaa7cdf81b7f98b980b18495ec28f1b5791ac3bfe3eea9"
+
+[[package]]
 name = "utf8-ranges"
 version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcfc827f90e53a02eaef5e535ee14266c1d569214c6aa70133a624d8a3164ba"
 
 [[package]]
 name = "utf8parse"
```

