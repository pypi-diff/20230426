# Comparing `tmp/summa_embed-0.1.2.tar.gz` & `tmp/summa_embed-0.1.3.tar.gz`

## Comparing `summa_embed-0.1.2.tar` & `summa_embed-0.1.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 summa_embed-0.1.2/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2129 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20    10377 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7125 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20       96 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2183 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      424 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 summa_embed-0.1.2/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20       92 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7087 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5015 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20     1021 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/driver.rs
--rw-r--r--   0      501       20    13794 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    24562 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13833 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    14335 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5038 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     4711 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      163 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20    14304 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1589 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    53911 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     2216 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11168 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7439 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     3093 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8014 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5117 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2447 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     9854 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      450 2023-04-26 05:25:34.000000 summa_embed-0.1.2/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 summa_embed-0.1.2/Cargo.toml
--rw-r--r--   0      501       20     2809 2023-04-26 05:25:34.000000 summa_embed-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0      501       20      685 2023-04-26 05:25:34.000000 summa_embed-0.1.2/.gitignore
--rw-r--r--   0      501       20      373 2023-04-26 05:25:34.000000 summa_embed-0.1.2/pyproject.toml
--rw-r--r--   0      501       20     4321 2023-04-26 05:25:34.000000 summa_embed-0.1.2/src/lib.rs
--rw-r--r--   0      501       20    88981 2023-04-26 05:25:56.000000 summa_embed-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 summa_embed-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 summa_embed-0.1.3/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20       92 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7087 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5015 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20     1021 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/driver.rs
+-rw-r--r--   0      501       20    13794 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    24562 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13833 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    14335 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5038 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     4711 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      163 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20    14304 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1589 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    53911 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     2216 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11168 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7439 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     3093 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8014 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5117 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2447 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     9854 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      450 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 summa_embed-0.1.3/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2129 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20    10377 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7125 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20       96 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2183 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      424 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 summa_embed-0.1.3/Cargo.toml
+-rw-r--r--   0      501       20     2809 2023-04-26 12:21:44.000000 summa_embed-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      685 2023-04-26 12:21:44.000000 summa_embed-0.1.3/.gitignore
+-rw-r--r--   0      501       20      373 2023-04-26 12:21:44.000000 summa_embed-0.1.3/pyproject.toml
+-rw-r--r--   0      501       20     4324 2023-04-26 12:21:44.000000 summa_embed-0.1.3/src/lib.rs
+-rw-r--r--   0      501       20    88981 2023-04-26 12:22:14.000000 summa_embed-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 summa_embed-0.1.3/PKG-INFO
```

### Comparing `summa_embed-0.1.2/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.1.3/local_dependencies/summa-proto/Cargo.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.1.3/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-proto/build.rs` & `summa_embed-0.1.3/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.1.3/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.1.3/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.1.3/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.1.3/local_dependencies/summa-proto/proto/query.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.1.3/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.1.3/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.1.3/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.1.3/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.1.3/local_dependencies/summa-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/LICENSE` & `summa_embed-0.1.3/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/driver.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/driver.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.1.3/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/Cargo.toml` & `summa_embed-0.1.3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-embed-py"
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
```

### Comparing `summa_embed-0.1.2/.github/workflows/CI.yml` & `summa_embed-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/.gitignore` & `summa_embed-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.2/src/lib.rs` & `summa_embed-0.1.3/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -99,11 +99,11 @@
         })
     }
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 #[pyo3(name = "summa_embed")]
-fn summa_py(_py: Python, m: &PyModule) -> PyResult<()> {
+fn summa_embed(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<IndexRegistry>()?;
     Ok(())
 }
```

### Comparing `summa_embed-0.1.2/Cargo.lock` & `summa_embed-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2477,15 +2477,15 @@
  "time",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "futures",
  "pyo3",
  "pyo3-asyncio",
  "pythonize",
  "serde_json",
  "summa-core",
@@ -2914,17 +2914,17 @@
 dependencies = [
  "native-tls",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-stream"
-version = "0.1.13"
+version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "76cd2598a37719e3cd4c28af93f978506a97a2920ef4d96e4b12e38b8cbc8940"
+checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
```

