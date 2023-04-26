# Comparing `tmp/opendal-0.33.0.tar.gz` & `tmp/opendal-0.33.1.tar.gz`

## Comparing `opendal-0.33.0.tar` & `opendal-0.33.1.tar`

### file list

```diff
@@ -1,252 +1,253 @@
--rw-r--r--   0        0        0     5737 1970-01-01 00:00:00.000000 opendal-0.33.0/local_dependencies/opendal/Cargo.toml
--rw-r--r--   0     1001      123    64485 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/CHANGELOG.md
--rw-r--r--   0     1001      123     1256 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/CONTRIBUTING.md
--rw-r--r--   0     1001      123     6635 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/README.md
--rw-r--r--   0     1001      123      378 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/benches/README.md
--rw-r--r--   0     1001      123      672 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/benches/ops/README.md
--rw-r--r--   0     1001      123      979 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/benches/ops/main.rs
--rw-r--r--   0     1001      123     5574 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/benches/ops/read.rs
--rw-r--r--   0     1001      123     2438 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/benches/ops/utils.rs
--rw-r--r--   0     1001      123     2163 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/benches/ops/write.rs
--rw-r--r--   0     1001      123     1832 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/examples/object.rs
--rw-r--r--   0     1001      123     1290 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
--rw-r--r--   0     1001      123     7682 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
--rw-r--r--   0     1001      123     5241 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/concepts.rs
--rw-r--r--   0     1001      123      982 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/features.md
--rw-r--r--   0     1001      123    10880 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/internals/accessor.rs
--rw-r--r--   0     1001      123     1765 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/internals/layer.rs
--rw-r--r--   0     1001      123     3409 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/internals/mod.rs
--rw-r--r--   0     1001      123     1458 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/mod.rs
--rw-r--r--   0     1001      123     3436 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
--rw-r--r--   0     1001      123     5329 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
--rw-r--r--   0     1001      123     4885 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
--rw-r--r--   0     1001      123     5428 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
--rw-r--r--   0     1001      123     3341 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
--rw-r--r--   0     1001      123     4425 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
--rw-r--r--   0     1001      123     2902 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
--rw-r--r--   0     1001      123    12349 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
--rw-r--r--   0     1001      123     2538 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
--rw-r--r--   0     1001      123     2347 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
--rw-r--r--   0     1001      123     2805 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
--rw-r--r--   0     1001      123     1803 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
--rw-r--r--   0     1001      123     4733 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
--rw-r--r--   0     1001      123     2184 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
--rw-r--r--   0     1001      123     5771 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
--rw-r--r--   0     1001      123     8563 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
--rw-r--r--   0     1001      123     3113 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
--rw-r--r--   0     1001      123     4321 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
--rw-r--r--   0     1001      123     1881 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
--rw-r--r--   0     1001      123     2926 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
--rw-r--r--   0     1001      123     2246 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
--rw-r--r--   0     1001      123     6523 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
--rw-r--r--   0     1001      123     4792 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
--rw-r--r--   0     1001      123    10091 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
--rw-r--r--   0     1001      123     2508 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
--rw-r--r--   0     1001      123     2670 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
--rw-r--r--   0     1001      123     8059 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
--rw-r--r--   0     1001      123     2472 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
--rw-r--r--   0     1001      123     4452 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
--rw-r--r--   0     1001      123     2534 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
--rw-r--r--   0     1001      123     3693 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
--rw-r--r--   0     1001      123     3255 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
--rw-r--r--   0     1001      123     4133 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
--rw-r--r--   0     1001      123     4408 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
--rw-r--r--   0     1001      123     4230 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
--rw-r--r--   0     1001      123     4392 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
--rw-r--r--   0     1001      123    23435 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/docs/upgrade.md
--rw-r--r--   0     1001      123     6746 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/chaos.rs
--rw-r--r--   0     1001      123    19723 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/complete.rs
--rw-r--r--   0     1001      123     9888 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
--rw-r--r--   0     1001      123    17355 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/error_context.rs
--rw-r--r--   0     1001      123    13556 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/immutable_index.rs
--rw-r--r--   0     1001      123    50969 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/logging.rs
--rw-r--r--   0     1001      123    13497 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/madsim.rs
--rw-r--r--   0     1001      123    31779 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/metrics.rs
--rw-r--r--   0     1001      123    12877 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/minitrace.rs
--rw-r--r--   0     1001      123     2205 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/mod.rs
--rw-r--r--   0     1001      123    13882 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/oteltrace.rs
--rw-r--r--   0     1001      123    24230 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/prometheus.rs
--rw-r--r--   0     1001      123    37745 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/retry.rs
--rw-r--r--   0     1001      123    12402 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/tracing.rs
--rw-r--r--   0     1001      123     3844 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/layers/type_eraser.rs
--rw-r--r--   0     1001      123     3001 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/lib.rs
--rw-r--r--   0     1001      123    18458 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/accessor.rs
--rw-r--r--   0     1001      123     5049 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
--rw-r--r--   0     1001      123     9348 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
--rw-r--r--   0     1001      123     1181 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
--rw-r--r--   0     1001      123     1548 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/mod.rs
--rw-r--r--   0     1001      123     1934 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/chrono_util.rs
--rw-r--r--   0     1001      123     6512 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/body.rs
--rw-r--r--   0     1001      123    10135 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
--rw-r--r--   0     1001      123    10534 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
--rw-r--r--   0     1001      123     5578 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/client.rs
--rw-r--r--   0     1001      123     3394 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/error.rs
--rw-r--r--   0     1001      123    10427 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/header.rs
--rw-r--r--   0     1001      123     2025 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/uri.rs
--rw-r--r--   0     1001      123    11983 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/layer.rs
--rw-r--r--   0     1001      123     1950 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/mod.rs
--rw-r--r--   0     1001      123     8881 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/cursor.rs
--rw-r--r--   0     1001      123     2512 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/entry.rs
--rw-r--r--   0     1001      123     3666 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
--rw-r--r--   0     1001      123     1006 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
--rw-r--r--   0     1001      123    15397 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
--rw-r--r--   0     1001      123     4148 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
--rw-r--r--   0     1001      123     1686 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
--rw-r--r--   0     1001      123     4577 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs
--rw-r--r--   0     1001      123     2001 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/mod.rs
--rw-r--r--   0     1001      123     3509 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/page.rs
--rw-r--r--   0     1001      123    10680 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/read.rs
--rw-r--r--   0     1001      123     9182 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
--rw-r--r--   0     1001      123     6861 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
--rw-r--r--   0     1001      123     5198 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/oio/write.rs
--rw-r--r--   0     1001      123     4081 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/operation.rs
--rw-r--r--   0     1001      123    11671 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/path.rs
--rw-r--r--   0     1001      123     6387 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/rps.rs
--rw-r--r--   0     1001      123     1396 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/serde_util.rs
--rw-r--r--   0     1001      123     1077 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/raw/version.rs
--rw-r--r--   0     1001      123    27973 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/backend.rs
--rw-r--r--   0     1001      123    10124 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/batch.rs
--rw-r--r--   0     1001      123    10574 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/core.rs
--rw-r--r--   0     1001      123     5821 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/error.rs
--rw-r--r--   0     1001      123      913 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/mod.rs
--rw-r--r--   0     1001      123    14196 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/pager.rs
--rw-r--r--   0     1001      123     2079 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azblob/writer.rs
--rw-r--r--   0     1001      123    16278 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/backend.rs
--rw-r--r--   0     1001      123     9557 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/core.rs
--rw-r--r--   0     1001      123     3520 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/error.rs
--rw-r--r--   0     1001      123      900 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/mod.rs
--rw-r--r--   0     1001      123     5647 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/pager.rs
--rw-r--r--   0     1001      123     2736 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/writer.rs
--rw-r--r--   0     1001      123     4046 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/dashmap/backend.rs
--rw-r--r--   0     1001      123      859 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/dashmap/mod.rs
--rw-r--r--   0     1001      123    23295 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/fs/backend.rs
--rw-r--r--   0     1001      123     1424 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/fs/error.rs
--rw-r--r--   0     1001      123      884 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/fs/mod.rs
--rw-r--r--   0     1001      123     4430 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/fs/pager.rs
--rw-r--r--   0     1001      123     3092 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/fs/writer.rs
--rw-r--r--   0     1001      123    16606 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ftp/backend.rs
--rw-r--r--   0     1001      123     1808 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ftp/err.rs
--rw-r--r--   0     1001      123      894 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ftp/mod.rs
--rw-r--r--   0     1001      123     2504 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ftp/pager.rs
--rw-r--r--   0     1001      123     4206 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ftp/util.rs
--rw-r--r--   0     1001      123     1900 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ftp/writer.rs
--rw-r--r--   0     1001      123    17782 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/backend.rs
--rw-r--r--   0     1001      123    11557 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/core.rs
--rw-r--r--   0     1001      123     3463 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/error.rs
--rw-r--r--   0     1001      123      905 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/mod.rs
--rw-r--r--   0     1001      123    10014 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/pager.rs
--rw-r--r--   0     1001      123     2820 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/uri.rs
--rw-r--r--   0     1001      123     6187 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/gcs/writer.rs
--rw-r--r--   0     1001      123    20642 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ghac/backend.rs
--rw-r--r--   0     1001      123     1908 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ghac/error.rs
--rw-r--r--   0     1001      123      877 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ghac/mod.rs
--rw-r--r--   0     1001      123     2375 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ghac/writer.rs
--rw-r--r--   0     1001      123    15656 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/backend.rs
--rw-r--r--   0     1001      123     1497 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/error.rs
--rw-r--r--   0     1001      123      888 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/mod.rs
--rw-r--r--   0     1001      123     3315 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/pager.rs
--rw-r--r--   0     1001      123     2549 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/writer.rs
--rw-r--r--   0     1001      123    15962 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/http/backend.rs
--rw-r--r--   0     1001      123     1826 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/http/error.rs
--rw-r--r--   0     1001      123      265 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
--rw-r--r--   0     1001      123      865 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/http/mod.rs
--rw-r--r--   0     1001      123    16861 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/backend.rs
--rw-r--r--   0     1001      123     1871 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/error.rs
--rw-r--r--   0     1001      123     8200 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
--rw-r--r--   0     1001      123      875 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/mod.rs
--rw-r--r--   0     1001      123     8716 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
--rw-r--r--   0     1001      123     3946 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
--rw-r--r--   0     1001      123     2790 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/error.rs
--rw-r--r--   0     1001      123      903 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
--rw-r--r--   0     1001      123     3819 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
--rw-r--r--   0     1001      123     1834 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
--rw-r--r--   0     1001      123     1074 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
--rw-r--r--   0     1001      123     4713 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/memcached/ascii.rs
--rw-r--r--   0     1001      123    10057 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/memcached/backend.rs
--rw-r--r--   0     1001      123      875 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/memcached/mod.rs
--rw-r--r--   0     1001      123     4336 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/memory/backend.rs
--rw-r--r--   0     1001      123      857 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/memory/mod.rs
--rw-r--r--   0     1001      123     3459 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/mod.rs
--rw-r--r--   0     1001      123     7999 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/moka/backend.rs
--rw-r--r--   0     1001      123      853 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/moka/mod.rs
--rw-r--r--   0     1001      123    13534 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/obs/backend.rs
--rw-r--r--   0     1001      123     7081 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/obs/core.rs
--rw-r--r--   0     1001      123     3443 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/obs/error.rs
--rw-r--r--   0     1001      123      896 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/obs/mod.rs
--rw-r--r--   0     1001      123     6027 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/obs/pager.rs
--rw-r--r--   0     1001      123     2057 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/obs/writer.rs
--rw-r--r--   0     1001      123    18746 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/oss/backend.rs
--rw-r--r--   0     1001      123    22799 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/oss/core.rs
--rw-r--r--   0     1001      123     3358 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/oss/error.rs
--rw-r--r--   0     1001      123      896 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/oss/mod.rs
--rw-r--r--   0     1001      123     7006 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/oss/pager.rs
--rw-r--r--   0     1001      123     6946 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/oss/writer.rs
--rw-r--r--   0     1001      123    10637 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/redis/backend.rs
--rw-r--r--   0     1001      123      855 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/redis/mod.rs
--rw-r--r--   0     1001      123     5664 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
--rw-r--r--   0     1001      123      859 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
--rw-r--r--   0     1001      123    39157 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/backend.rs
--rw-r--r--   0     1001      123     3395 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/compatible_services.md
--rw-r--r--   0     1001      123    28151 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/core.rs
--rw-r--r--   0     1001      123     3685 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/error.rs
--rw-r--r--   0     1001      123      894 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/mod.rs
--rw-r--r--   0     1001      123     7040 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/pager.rs
--rw-r--r--   0     1001      123     7529 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/s3/writer.rs
--rw-r--r--   0     1001      123     5518 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/sled/backend.rs
--rw-r--r--   0     1001      123      854 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/sled/mod.rs
--rw-r--r--   0     1001      123    38885 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/backend.rs
--rw-r--r--   0     1001      123    29663 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/core.rs
--rw-r--r--   0     1001      123     3712 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/error.rs
--rw-r--r--   0     1001      123      902 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/mod.rs
--rw-r--r--   0     1001      123     7061 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/pager.rs
--rw-r--r--   0     1001      123     2666 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/writer.rs
--rw-r--r--   0     1001      123    20511 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/backend.rs
--rw-r--r--   0     1001      123     1743 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/error.rs
--rw-r--r--   0     1001      123      130 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
--rw-r--r--   0     1001      123      626 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
--rw-r--r--   0     1001      123      531 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
--rw-r--r--   0     1001      123    16965 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/list_response.rs
--rw-r--r--   0     1001      123      911 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/mod.rs
--rw-r--r--   0     1001      123     2560 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/pager.rs
--rw-r--r--   0     1001      123     2066 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webdav/writer.rs
--rw-r--r--   0     1001      123    19374 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
--rw-r--r--   0     1001      123     4085 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/error.rs
--rw-r--r--   0     1001      123     4679 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/message.rs
--rw-r--r--   0     1001      123      907 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
--rw-r--r--   0     1001      123     2452 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
--rw-r--r--   0     1001      123     2076 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
--rw-r--r--   0     1001      123     2333 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/builder.rs
--rw-r--r--   0     1001      123     6381 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/capability.rs
--rw-r--r--   0     1001      123     2494 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/entry.rs
--rw-r--r--   0     1001      123    11590 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/error.rs
--rw-r--r--   0     1001      123     6197 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/list.rs
--rw-r--r--   0     1001      123    15166 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/metadata.rs
--rw-r--r--   0     1001      123     1511 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/mod.rs
--rw-r--r--   0     1001      123     1747 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/mode.rs
--rw-r--r--   0     1001      123    24145 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
--rw-r--r--   0     1001      123     8731 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/operator/builder.rs
--rw-r--r--   0     1001      123     3067 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/operator/metadata.rs
--rw-r--r--   0     1001      123     1098 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/operator/mod.rs
--rw-r--r--   0     1001      123    42195 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/operator/operator.rs
--rw-r--r--   0     1001      123    10788 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/ops.rs
--rw-r--r--   0     1001      123     9569 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/reader.rs
--rw-r--r--   0     1001      123     5852 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/scheme.rs
--rw-r--r--   0     1001      123    10180 2023-04-23 05:13:34.000000 opendal-0.33.0/local_dependencies/opendal/src/types/writer.rs
--rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.33.0/Cargo.toml
--rw-r--r--   0     1001      123      709 2023-04-23 05:13:34.000000 opendal-0.33.0/.gitignore
--rw-r--r--   0     1001      123      982 2023-04-23 05:13:34.000000 opendal-0.33.0/README.md
--rw-r--r--   0     1001      123      765 2023-04-23 05:13:34.000000 opendal-0.33.0/benchmark/README.md
--rw-r--r--   0     1001      123     2426 2023-04-23 05:13:34.000000 opendal-0.33.0/benchmark/async_opendal_benchmark.py
--rw-r--r--   0     1001      123     2955 2023-04-23 05:13:34.000000 opendal-0.33.0/benchmark/async_origin_s3_benchmark_with_gevent.py
--rw-r--r--   0     1001      123      917 2023-04-23 05:13:34.000000 opendal-0.33.0/examples/object.ipynb
--rw-r--r--   0     1001      123     1665 2023-04-23 05:13:34.000000 opendal-0.33.0/pyproject.toml
--rw-r--r--   0     1001      123      866 2023-04-23 05:13:34.000000 opendal-0.33.0/python/opendal/__init__.py
--rw-r--r--   0     1001      123     2917 2023-04-23 05:13:34.000000 opendal-0.33.0/python/opendal/__init__.pyi
--rw-r--r--   0     1001      123    11963 2023-04-23 05:13:34.000000 opendal-0.33.0/src/asyncio.rs
--rw-r--r--   0     1001      123     3311 2023-04-23 05:13:34.000000 opendal-0.33.0/src/layers.rs
--rw-r--r--   0     1001      123    13929 2023-04-23 05:13:34.000000 opendal-0.33.0/src/lib.rs
--rw-r--r--   0     1001      123     1604 2023-04-23 05:13:34.000000 opendal-0.33.0/tests/binding.feature
--rw-r--r--   0     1001      123     2942 2023-04-23 05:13:34.000000 opendal-0.33.0/tests/steps/binding.py
--rw-r--r--   0     1001      123   117424 2023-04-23 05:13:34.000000 opendal-0.33.0/Cargo.lock
--rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 opendal-0.33.0/PKG-INFO
+-rw-r--r--   0        0        0     5737 1970-01-01 00:00:00.000000 opendal-0.33.1/local_dependencies/opendal/Cargo.toml
+-rw-r--r--   0     1001      123    65426 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/CHANGELOG.md
+-rw-r--r--   0     1001      123     1256 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     6635 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/README.md
+-rw-r--r--   0     1001      123      378 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/benches/README.md
+-rw-r--r--   0     1001      123      672 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/benches/ops/README.md
+-rw-r--r--   0     1001      123      979 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/benches/ops/main.rs
+-rw-r--r--   0     1001      123     5574 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/benches/ops/read.rs
+-rw-r--r--   0     1001      123     2438 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/benches/ops/utils.rs
+-rw-r--r--   0     1001      123     2163 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/benches/ops/write.rs
+-rw-r--r--   0     1001      123     1832 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/examples/object.rs
+-rw-r--r--   0     1001      123     1290 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/comparisons/mod.rs
+-rw-r--r--   0     1001      123     7682 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
+-rw-r--r--   0     1001      123     6142 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/concepts.rs
+-rw-r--r--   0     1001      123      982 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/features.md
+-rw-r--r--   0     1001      123    10879 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/internals/accessor.rs
+-rw-r--r--   0     1001      123     1765 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/internals/layer.rs
+-rw-r--r--   0     1001      123     3409 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/internals/mod.rs
+-rw-r--r--   0     1001      123     1458 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3436 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md
+-rw-r--r--   0     1001      123     5329 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
+-rw-r--r--   0     1001      123     4885 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
+-rw-r--r--   0     1001      123     5428 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
+-rw-r--r--   0     1001      123     3341 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
+-rw-r--r--   0     1001      123     4425 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
+-rw-r--r--   0     1001      123     2902 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
+-rw-r--r--   0     1001      123    12349 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
+-rw-r--r--   0     1001      123     2538 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
+-rw-r--r--   0     1001      123     2347 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
+-rw-r--r--   0     1001      123     2805 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
+-rw-r--r--   0     1001      123     1803 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
+-rw-r--r--   0     1001      123     4733 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
+-rw-r--r--   0     1001      123     2184 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
+-rw-r--r--   0     1001      123     5771 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
+-rw-r--r--   0     1001      123     8563 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
+-rw-r--r--   0     1001      123     3113 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
+-rw-r--r--   0     1001      123     4321 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
+-rw-r--r--   0     1001      123     1881 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
+-rw-r--r--   0     1001      123     2926 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
+-rw-r--r--   0     1001      123     2246 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
+-rw-r--r--   0     1001      123     6523 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
+-rw-r--r--   0     1001      123     4792 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
+-rw-r--r--   0     1001      123    10091 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
+-rw-r--r--   0     1001      123     2508 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
+-rw-r--r--   0     1001      123     2670 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
+-rw-r--r--   0     1001      123     8059 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
+-rw-r--r--   0     1001      123     2472 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
+-rw-r--r--   0     1001      123     4452 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
+-rw-r--r--   0     1001      123     2534 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
+-rw-r--r--   0     1001      123     3693 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
+-rw-r--r--   0     1001      123     3255 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
+-rw-r--r--   0     1001      123     4133 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
+-rw-r--r--   0     1001      123     4408 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
+-rw-r--r--   0     1001      123     4230 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
+-rw-r--r--   0     1001      123     3172 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
+-rw-r--r--   0     1001      123     4478 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/mod.rs
+-rw-r--r--   0     1001      123    23435 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/docs/upgrade.md
+-rw-r--r--   0     1001      123     6746 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/chaos.rs
+-rw-r--r--   0     1001      123    20940 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/complete.rs
+-rw-r--r--   0     1001      123     9888 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/concurrent_limit.rs
+-rw-r--r--   0     1001      123    17355 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/error_context.rs
+-rw-r--r--   0     1001      123    13556 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/immutable_index.rs
+-rw-r--r--   0     1001      123    51478 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/logging.rs
+-rw-r--r--   0     1001      123    13497 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/madsim.rs
+-rw-r--r--   0     1001      123    31779 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/metrics.rs
+-rw-r--r--   0     1001      123    12877 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/minitrace.rs
+-rw-r--r--   0     1001      123     2205 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/mod.rs
+-rw-r--r--   0     1001      123    13882 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/oteltrace.rs
+-rw-r--r--   0     1001      123    24230 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/prometheus.rs
+-rw-r--r--   0     1001      123    37745 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/retry.rs
+-rw-r--r--   0     1001      123    12402 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/tracing.rs
+-rw-r--r--   0     1001      123     3844 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/layers/type_eraser.rs
+-rw-r--r--   0     1001      123     3001 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/lib.rs
+-rw-r--r--   0     1001      123    19037 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/accessor.rs
+-rw-r--r--   0     1001      123     5049 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs
+-rw-r--r--   0     1001      123     9830 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
+-rw-r--r--   0     1001      123     1181 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
+-rw-r--r--   0     1001      123     1548 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/mod.rs
+-rw-r--r--   0     1001      123     1934 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/chrono_util.rs
+-rw-r--r--   0     1001      123     6512 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/body.rs
+-rw-r--r--   0     1001      123    10135 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
+-rw-r--r--   0     1001      123    10534 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
+-rw-r--r--   0     1001      123     5578 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/client.rs
+-rw-r--r--   0     1001      123     3394 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/error.rs
+-rw-r--r--   0     1001      123    10427 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/header.rs
+-rw-r--r--   0     1001      123     2025 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/uri.rs
+-rw-r--r--   0     1001      123    11983 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/layer.rs
+-rw-r--r--   0     1001      123     1950 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/mod.rs
+-rw-r--r--   0     1001      123     8881 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/cursor.rs
+-rw-r--r--   0     1001      123     2512 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/entry.rs
+-rw-r--r--   0     1001      123     3666 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1006 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
+-rw-r--r--   0     1001      123    15397 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
+-rw-r--r--   0     1001      123     4148 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1686 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
+-rw-r--r--   0     1001      123     4577 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs
+-rw-r--r--   0     1001      123     2001 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/mod.rs
+-rw-r--r--   0     1001      123     3509 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/page.rs
+-rw-r--r--   0     1001      123    10680 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/read.rs
+-rw-r--r--   0     1001      123     9182 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
+-rw-r--r--   0     1001      123     6861 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
+-rw-r--r--   0     1001      123     5198 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/oio/write.rs
+-rw-r--r--   0     1001      123     4081 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/operation.rs
+-rw-r--r--   0     1001      123    11671 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/path.rs
+-rw-r--r--   0     1001      123     6387 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/rps.rs
+-rw-r--r--   0     1001      123     1396 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/serde_util.rs
+-rw-r--r--   0     1001      123     1077 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/raw/version.rs
+-rw-r--r--   0     1001      123    27973 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/backend.rs
+-rw-r--r--   0     1001      123    10124 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/batch.rs
+-rw-r--r--   0     1001      123    10574 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/core.rs
+-rw-r--r--   0     1001      123     5820 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/error.rs
+-rw-r--r--   0     1001      123      913 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/mod.rs
+-rw-r--r--   0     1001      123    14196 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/pager.rs
+-rw-r--r--   0     1001      123     2079 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azblob/writer.rs
+-rw-r--r--   0     1001      123    16278 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/backend.rs
+-rw-r--r--   0     1001      123     9557 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/core.rs
+-rw-r--r--   0     1001      123     3519 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/error.rs
+-rw-r--r--   0     1001      123      900 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/mod.rs
+-rw-r--r--   0     1001      123     5647 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/pager.rs
+-rw-r--r--   0     1001      123     2736 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/writer.rs
+-rw-r--r--   0     1001      123     4046 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/dashmap/backend.rs
+-rw-r--r--   0     1001      123      859 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/dashmap/mod.rs
+-rw-r--r--   0     1001      123    23347 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/fs/backend.rs
+-rw-r--r--   0     1001      123     1424 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/fs/error.rs
+-rw-r--r--   0     1001      123      884 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/fs/mod.rs
+-rw-r--r--   0     1001      123     4430 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/fs/pager.rs
+-rw-r--r--   0     1001      123     3092 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/fs/writer.rs
+-rw-r--r--   0     1001      123    16606 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ftp/backend.rs
+-rw-r--r--   0     1001      123     1808 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ftp/err.rs
+-rw-r--r--   0     1001      123      894 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ftp/mod.rs
+-rw-r--r--   0     1001      123     2504 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ftp/pager.rs
+-rw-r--r--   0     1001      123     4206 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ftp/util.rs
+-rw-r--r--   0     1001      123     1900 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ftp/writer.rs
+-rw-r--r--   0     1001      123    17843 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/backend.rs
+-rw-r--r--   0     1001      123    11763 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/core.rs
+-rw-r--r--   0     1001      123     3462 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/error.rs
+-rw-r--r--   0     1001      123      905 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/mod.rs
+-rw-r--r--   0     1001      123    10014 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/pager.rs
+-rw-r--r--   0     1001      123     2820 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/uri.rs
+-rw-r--r--   0     1001      123     6224 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/gcs/writer.rs
+-rw-r--r--   0     1001      123    20642 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ghac/backend.rs
+-rw-r--r--   0     1001      123     1908 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ghac/error.rs
+-rw-r--r--   0     1001      123      877 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ghac/mod.rs
+-rw-r--r--   0     1001      123     2375 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ghac/writer.rs
+-rw-r--r--   0     1001      123    15656 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/backend.rs
+-rw-r--r--   0     1001      123     1497 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/error.rs
+-rw-r--r--   0     1001      123      888 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/mod.rs
+-rw-r--r--   0     1001      123     3315 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/pager.rs
+-rw-r--r--   0     1001      123     2461 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/writer.rs
+-rw-r--r--   0     1001      123    15962 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/http/backend.rs
+-rw-r--r--   0     1001      123     1825 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/http/error.rs
+-rw-r--r--   0     1001      123      265 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      865 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/http/mod.rs
+-rw-r--r--   0     1001      123    16861 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/backend.rs
+-rw-r--r--   0     1001      123     1871 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/error.rs
+-rw-r--r--   0     1001      123     8200 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/ipld.rs
+-rw-r--r--   0     1001      123      875 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/mod.rs
+-rw-r--r--   0     1001      123     8716 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/backend.rs
+-rw-r--r--   0     1001      123     3946 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/builder.rs
+-rw-r--r--   0     1001      123     2790 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/error.rs
+-rw-r--r--   0     1001      123      903 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/mod.rs
+-rw-r--r--   0     1001      123     3819 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/pager.rs
+-rw-r--r--   0     1001      123     1834 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/writer.rs
+-rw-r--r--   0     1001      123     1074 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
+-rw-r--r--   0     1001      123     4713 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/memcached/ascii.rs
+-rw-r--r--   0     1001      123    10057 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/memcached/backend.rs
+-rw-r--r--   0     1001      123      875 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/memcached/mod.rs
+-rw-r--r--   0     1001      123     4337 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/memory/backend.rs
+-rw-r--r--   0     1001      123      857 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/memory/mod.rs
+-rw-r--r--   0     1001      123     3459 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/mod.rs
+-rw-r--r--   0     1001      123     7999 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/moka/backend.rs
+-rw-r--r--   0     1001      123      853 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/moka/mod.rs
+-rw-r--r--   0     1001      123    13617 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/obs/backend.rs
+-rw-r--r--   0     1001      123     7436 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/obs/core.rs
+-rw-r--r--   0     1001      123     3442 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/obs/error.rs
+-rw-r--r--   0     1001      123      896 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/obs/mod.rs
+-rw-r--r--   0     1001      123     6027 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/obs/pager.rs
+-rw-r--r--   0     1001      123     2057 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/obs/writer.rs
+-rw-r--r--   0     1001      123    21480 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/oss/backend.rs
+-rw-r--r--   0     1001      123    24192 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/oss/core.rs
+-rw-r--r--   0     1001      123     3357 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/oss/error.rs
+-rw-r--r--   0     1001      123      896 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/oss/mod.rs
+-rw-r--r--   0     1001      123     7006 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/oss/pager.rs
+-rw-r--r--   0     1001      123     6946 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/oss/writer.rs
+-rw-r--r--   0     1001      123    10637 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/redis/backend.rs
+-rw-r--r--   0     1001      123      855 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/redis/mod.rs
+-rw-r--r--   0     1001      123     5664 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/rocksdb/backend.rs
+-rw-r--r--   0     1001      123      859 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/rocksdb/mod.rs
+-rw-r--r--   0     1001      123    39561 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/backend.rs
+-rw-r--r--   0     1001      123     3395 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/compatible_services.md
+-rw-r--r--   0     1001      123    28456 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/core.rs
+-rw-r--r--   0     1001      123     3734 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/error.rs
+-rw-r--r--   0     1001      123      894 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/mod.rs
+-rw-r--r--   0     1001      123     7324 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/pager.rs
+-rw-r--r--   0     1001      123     7529 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/s3/writer.rs
+-rw-r--r--   0     1001      123     5518 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/sled/backend.rs
+-rw-r--r--   0     1001      123      854 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/sled/mod.rs
+-rw-r--r--   0     1001      123    38885 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/backend.rs
+-rw-r--r--   0     1001      123    29663 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/core.rs
+-rw-r--r--   0     1001      123     3711 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/error.rs
+-rw-r--r--   0     1001      123      902 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/mod.rs
+-rw-r--r--   0     1001      123     7061 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/pager.rs
+-rw-r--r--   0     1001      123     2666 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/writer.rs
+-rw-r--r--   0     1001      123    20511 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/backend.rs
+-rw-r--r--   0     1001      123     1743 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/error.rs
+-rw-r--r--   0     1001      123      130 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
+-rw-r--r--   0     1001      123      626 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
+-rw-r--r--   0     1001      123      531 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
+-rw-r--r--   0     1001      123    16965 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/list_response.rs
+-rw-r--r--   0     1001      123      911 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/mod.rs
+-rw-r--r--   0     1001      123     2560 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/pager.rs
+-rw-r--r--   0     1001      123     2066 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webdav/writer.rs
+-rw-r--r--   0     1001      123    19374 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/backend.rs
+-rw-r--r--   0     1001      123     4085 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/error.rs
+-rw-r--r--   0     1001      123     4679 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/message.rs
+-rw-r--r--   0     1001      123      907 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/mod.rs
+-rw-r--r--   0     1001      123     2452 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/pager.rs
+-rw-r--r--   0     1001      123     2076 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/writer.rs
+-rw-r--r--   0     1001      123     3368 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/builder.rs
+-rw-r--r--   0     1001      123     6381 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/capability.rs
+-rw-r--r--   0     1001      123     2494 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/entry.rs
+-rw-r--r--   0     1001      123    12002 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/error.rs
+-rw-r--r--   0     1001      123     6197 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/list.rs
+-rw-r--r--   0     1001      123    15166 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/metadata.rs
+-rw-r--r--   0     1001      123     1511 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/mod.rs
+-rw-r--r--   0     1001      123     1747 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/mode.rs
+-rw-r--r--   0     1001      123    24145 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs
+-rw-r--r--   0     1001      123     8731 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/operator/builder.rs
+-rw-r--r--   0     1001      123     3067 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/operator/metadata.rs
+-rw-r--r--   0     1001      123     1098 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/operator/mod.rs
+-rw-r--r--   0     1001      123    42718 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/operator/operator.rs
+-rw-r--r--   0     1001      123    10788 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/ops.rs
+-rw-r--r--   0     1001      123     9569 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/reader.rs
+-rw-r--r--   0     1001      123     5852 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/scheme.rs
+-rw-r--r--   0     1001      123    10696 2023-04-25 15:52:38.000000 opendal-0.33.1/local_dependencies/opendal/src/types/writer.rs
+-rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.33.1/Cargo.toml
+-rw-r--r--   0     1001      123      709 2023-04-25 15:52:38.000000 opendal-0.33.1/.gitignore
+-rw-r--r--   0     1001      123      982 2023-04-25 15:52:38.000000 opendal-0.33.1/README.md
+-rw-r--r--   0     1001      123      765 2023-04-25 15:52:38.000000 opendal-0.33.1/benchmark/README.md
+-rw-r--r--   0     1001      123     2426 2023-04-25 15:52:38.000000 opendal-0.33.1/benchmark/async_opendal_benchmark.py
+-rw-r--r--   0     1001      123     2955 2023-04-25 15:52:38.000000 opendal-0.33.1/benchmark/async_origin_s3_benchmark_with_gevent.py
+-rw-r--r--   0     1001      123      917 2023-04-25 15:52:38.000000 opendal-0.33.1/examples/object.ipynb
+-rw-r--r--   0     1001      123     1665 2023-04-25 15:52:38.000000 opendal-0.33.1/pyproject.toml
+-rw-r--r--   0     1001      123      866 2023-04-25 15:52:38.000000 opendal-0.33.1/python/opendal/__init__.py
+-rw-r--r--   0     1001      123     2917 2023-04-25 15:52:38.000000 opendal-0.33.1/python/opendal/__init__.pyi
+-rw-r--r--   0     1001      123    11963 2023-04-25 15:52:38.000000 opendal-0.33.1/src/asyncio.rs
+-rw-r--r--   0     1001      123     3311 2023-04-25 15:52:38.000000 opendal-0.33.1/src/layers.rs
+-rw-r--r--   0     1001      123    13929 2023-04-25 15:52:38.000000 opendal-0.33.1/src/lib.rs
+-rw-r--r--   0     1001      123     1604 2023-04-25 15:52:38.000000 opendal-0.33.1/tests/binding.feature
+-rw-r--r--   0     1001      123     2942 2023-04-25 15:52:38.000000 opendal-0.33.1/tests/steps/binding.py
+-rw-r--r--   0     1001      123   117424 2023-04-25 15:52:38.000000 opendal-0.33.1/Cargo.lock
+-rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 opendal-0.33.1/PKG-INFO
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/Cargo.toml` & `opendal-0.33.1/local_dependencies/opendal/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.64"
-version= "0.33.0"
+version= "0.33.1"
 
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
 default = [
   "rustls",
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/CHANGELOG.md` & `opendal-0.33.1/local_dependencies/opendal/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,41 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
+## [v0.33.1] - 2023-04-25
+
+### Added
+
+- feat: Add behavior test for read_with_if_match & stat_with_if_match (#2088)
+- feat(tests): Add fuzz test for writer without content length (#2100)
+- feat: add if_none_match support for obs (#2103)
+- feat(services/oss): Add server side encryption support for oss (#2092)
+- feat(core): update errorKind `PreconditionFailed` to `ConditionNotMatch` (#2104)
+- feat(services/s3): Add `start-after` support for list (#2096)
+- feat: gcs support cache control (#2116)
+
+### Fixed
+
+- fix(services/gcs): set `content length=0` for gcs initiate_resumable_upload (#2110)
+- fix(bindings/nodejs): Fix index.d.ts not updated (#2117)
+
+### Docs
+
+- chore: improve LoggingLayer docs and pub use log::Level (#2089)
+- docs(refactor): Add more detailed description of operator, accessor, and builder (#2094)
+
+### CI
+
+- chore(bindings/nodejs): update `package.json` repository info (#2078)
+- ci: Bring hdfs test back (#2114)
+
 ## [v0.33.0] - 2023-04-23
 
 ### Added
 
 - feat: Add OpenTelemetry Trace Layer (#2001)
 - feat: add if_none_match support for azblob (#2035)
 - feat: add if_none_match/if_match for gcs (#2039)
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/CONTRIBUTING.md` & `opendal-0.33.1/local_dependencies/opendal/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/README.md` & `opendal-0.33.1/local_dependencies/opendal/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/benches/ops/README.md` & `opendal-0.33.1/local_dependencies/opendal/benches/ops/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/benches/ops/main.rs` & `opendal-0.33.1/local_dependencies/opendal/benches/ops/main.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/benches/ops/read.rs` & `opendal-0.33.1/local_dependencies/opendal/benches/ops/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/benches/ops/utils.rs` & `opendal-0.33.1/local_dependencies/opendal/benches/ops/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/benches/ops/write.rs` & `opendal-0.33.1/local_dependencies/opendal/benches/ops/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/examples/object.rs` & `opendal-0.33.1/local_dependencies/opendal/examples/object.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/comparisons/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/docs/comparisons/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/concepts.rs` & `opendal-0.33.1/local_dependencies/opendal/src/docs/concepts.rs`

 * *Files 7% similar despite different names*

```diff
@@ -13,59 +13,70 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 //! The core concepts of OpenDAL's public API.
 //!
-//! OpenDAL provides a unified abstraction for all storage services.
+//! OpenDAL provides a unified abstraction that helps developers access all storage services.
 //!
 //! There are two core concepts in OpenDAL:
 //!
-//! - [`Builder`]: Build an instance of underlying services.
-//! - [`Operator`]: A bridge between underlying implementation detail and unified abstraction.
+//! - [`Builder`]: Builder accepts a series of parameters to set up an instance of underlying services.
+//! You can adjust the behaviour of underlying services with these parameters.
+//! - [`Operator`]: Developer can access underlying storage services with manipulating one Operator.
+//! The Operator is a delegate for underlying implementation detail, and provides one unified access interface,
+//! including `read`, `write`, `list` and so on.
 //!
 //! If you are interested in internal implementation details, please have a look at [`internals`][super::internals].
 //!
 //! # Builder
 //!
 //! Let's start with [`Builder`].
 //!
-//! A `Builder` is a trait that is implemented by the underlying services. We can use a `Builder` to configure and create a service. Builder is the only public API provided by services, and the detailed implementation is hidden.
+//! A `Builder` is a trait that is implemented by the underlying services. We can use a `Builder` to configure and create a service.
+//! Developer can only create one service via Builder, in other words, Builder is the only public API provided by services.
+//! And other detailed implementation will be hidden.
 //!
 //! ```text
 //! ┌───────────┐                 ┌───────────┐
 //! │           │     build()     │           │
 //! │  Builder  ├────────────────►│  Service  │
 //! │           │                 │           │
 //! └───────────┘                 └───────────┘
 //! ```
 //!
 //! All [`Builder`] provided by OpenDAL is under [`services`][crate::services], we can refer to them like `opendal::services::S3`.
+//! By right the builder will be named like `OneServiceBuilder`, but usually we will export it to public with renaming it as one
+//! general name. For example, we will rename `S3Builder` to `S3` and developer will use `S3` finally.
 //!
 //! For example:
 //!
 //! ```no_run
 //! use opendal::services::S3;
 //!
 //! let mut builder = S3::default();
 //! builder.bucket("example");
 //! builder.root("/path/to/file");
 //! ```
 //!
 //! # Operator
-//!
-//! The [`Operator`] is a bridge between the underlying implementation details and the unified abstraction. OpenDAL will erase all generic types and higher abstraction around it.
+//! The [`Operator`] is a delegate for Service, the underlying implementation detail that implements [`Accessor`][crate::raw::Accessor],
+//! and it also provides one unified access interface.
+//! It will hold one reference of Service with its all generic types erased by OpenDAL,
+//! which is the reason why we say the Operator is the delegate of one Service.
 //!
 //! ```text
-//! ┌───────────┐           ┌───────────┐              ┌─────────────────┐
-//! │           │  build()  │           │  type erase  │                 │
-//! │  Builder  ├──────────►│  Service  ├─────────────►│     Operator    │
-//! │           │           │           │              │                 │
-//! └───────────┘           └───────────┘              └─────────────────┘
+//!                   ┌────────────────────┐
+//!                   │      Operator      │
+//!                   │         │delegate  │
+//! ┌─────────┐ build │         ▼          │ rely on ┌─────────────────────┐
+//! │ Builder ├───────┼──►┌────────────┐   │◄────────┤ business logic code │
+//! └─────────┘       │   │  Service   │   │         └─────────────────────┘
+//!                   └───┴────────────┴───┘
 //! ```
 //!
 //! `Operator` can be built from `Builder`:
 //!
 //! ```no_run
 //! # use opendal::Result;
 //! use opendal::services::S3;
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/features.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/features.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/internals/accessor.rs` & `opendal-0.33.1/local_dependencies/opendal/src/docs/internals/accessor.rs`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 //! This tutorial implements a `duck` storage service that sends API
 //! requests to a super-powered duck. Gagaga!
 //!
 //! ## Scheme
 //!
 //! First of all, let's pick a good [`Scheme`] for our duck service. The
 //! scheme should be unique and easy to understand. Normally we should
-//! use it's formal name.
+//! use its formal name.
 //!
 //! For example, we will use `s3` for AWS S3 Compatible Storage Service
 //! instead of `aws` or `awss3`. This is because there are many storage
 //! vendors that provide s3-like RESTful APIs, and our s3 service is
 //! implemented to support all of them, not just AWS S3.
 //!
 //! Obviously, we can use `duck` as scheme, let's add a new variant in [`Scheme`], and implement all reqired functions like `Scheme::from_str` and `Scheme::into_static`:
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/internals/layer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/docs/internals/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/internals/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/docs/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/docs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/rfcs/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/docs/rfcs/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -129,7 +129,10 @@
 pub mod rfc_1420_object_writer {}
 
 #[doc = include_str!("1477_remove_object_concept.md")]
 pub mod rfc_1477_remove_object_concept {}
 
 #[doc = include_str!("1735_operation_extension.md")]
 pub mod rfc_1735_operation_extension {}
+
+#[doc = include_str!("2083_writer_sink_api.md")]
+pub mod rfc_2083_writer_sink_api {}
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/docs/upgrade.md` & `opendal-0.33.1/local_dependencies/opendal/src/docs/upgrade.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/chaos.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/chaos.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/complete.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/complete.rs`

 * *Files 2% similar despite different names*

```diff
@@ -505,29 +505,41 @@
             NeedFlat(p) => p.next(),
             NeedHierarchy(p) => p.next(),
         }
     }
 }
 
 pub struct CompleteWriter<W> {
-    inner: W,
+    inner: Option<W>,
     size: Option<u64>,
     written: u64,
 }
 
 impl<W> CompleteWriter<W> {
     pub fn new(inner: W, size: Option<u64>) -> CompleteWriter<W> {
         CompleteWriter {
-            inner,
+            inner: Some(inner),
             size,
             written: 0,
         }
     }
 }
 
+/// Check if the writer has been closed or aborted while debug_assertions
+/// enabled. This code will never be executed in release mode.
+#[cfg(debug_assertions)]
+impl<W> Drop for CompleteWriter<W> {
+    fn drop(&mut self) {
+        if self.inner.is_some() {
+            // Do we need to panic here?
+            log::warn!("writer has not been closed or aborted, must be a bug")
+        }
+    }
+}
+
 #[async_trait]
 impl<W> oio::Write for CompleteWriter<W>
 where
     W: oio::Write,
 {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let n = bs.len();
@@ -540,21 +552,31 @@
                         "writer got too much data, expect: {size}, actual: {}",
                         self.written + n as u64
                     ),
                 ));
             }
         }
 
-        self.inner.write(bs).await?;
+        let w = self.inner.as_mut().ok_or_else(|| {
+            Error::new(ErrorKind::Unexpected, "writer has been closed or aborted")
+        })?;
+        w.write(bs).await?;
         self.written += n as u64;
         Ok(())
     }
 
     async fn abort(&mut self) -> Result<()> {
-        self.inner.abort().await
+        let w = self.inner.as_mut().ok_or_else(|| {
+            Error::new(ErrorKind::Unexpected, "writer has been closed or aborted")
+        })?;
+
+        w.abort().await?;
+        self.inner = None;
+
+        Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         if let Some(size) = self.size {
             if self.written < size {
                 return Err(Error::new(
                     ErrorKind::ContentIncomplete,
@@ -562,15 +584,21 @@
                         "writer got too less data, expect: {size}, actual: {}",
                         self.written
                     ),
                 ));
             }
         }
 
-        self.inner.close().await?;
+        let w = self.inner.as_mut().ok_or_else(|| {
+            Error::new(ErrorKind::Unexpected, "writer has been closed or aborted")
+        })?;
+
+        w.close().await?;
+        self.inner = None;
+
         Ok(())
     }
 }
 
 impl<W> oio::BlockingWrite for CompleteWriter<W>
 where
     W: oio::BlockingWrite,
@@ -586,15 +614,19 @@
                         "writer got too much data, expect: {size}, actual: {}",
                         self.written + n as u64
                     ),
                 ));
             }
         }
 
-        self.inner.write(bs)?;
+        let w = self.inner.as_mut().ok_or_else(|| {
+            Error::new(ErrorKind::Unexpected, "writer has been closed or aborted")
+        })?;
+
+        w.write(bs)?;
         self.written += n as u64;
         Ok(())
     }
 
     fn close(&mut self) -> Result<()> {
         if let Some(size) = self.size {
             if self.written < size {
@@ -604,11 +636,16 @@
                         "writer got too less data, expect: {size}, actual: {}",
                         self.written
                     ),
                 ));
             }
         }
 
-        self.inner.close()?;
+        let w = self.inner.as_mut().ok_or_else(|| {
+            Error::new(ErrorKind::Unexpected, "writer has been closed or aborted")
+        })?;
+
+        w.close()?;
+        self.inner = None;
         Ok(())
     }
 }
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/concurrent_limit.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/concurrent_limit.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/error_context.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/error_context.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/immutable_index.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/immutable_index.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/logging.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/logging.rs`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 ///
 /// - OpenDAL will log in structural way.
 /// - Every operation will start with a `started` log entry.
 /// - Every operation will finish with the following status:
 ///   - `finished`: the operation is successful.
 ///   - `errored`: the operation returns an expected error like `NotFound`.
 ///   - `failed`: the operation returns an unexpected error.
+/// - The default log level while expected error happened is `Warn`.
+/// - The default log level while unexpected failure happened is `Error`.
 ///
 /// # Todo
 ///
 /// We should migrate to log's kv api after it's ready.
 ///
 /// Tracking issue: <https://github.com/rust-lang/log/issues/328>
 ///
@@ -748,15 +750,15 @@
         );
 
         self.inner
             .blocking_write(path, args)
             .map(|(rp, w)| {
                 debug!(
                     target: LOGGING_TARGET,
-                    "service={} operation={} path={} -> written",
+                    "service={} operation={} path={} -> start writing",
                     self.scheme,
                     Operation::BlockingWrite,
                     path,
                 );
                 let w = LoggingWriter::new(
                     self.scheme,
                     Operation::BlockingWrite,
@@ -1334,27 +1336,14 @@
             written: 0,
             inner: writer,
             failure_level,
         }
     }
 }
 
-impl<W> Drop for LoggingWriter<W> {
-    fn drop(&mut self) {
-        debug!(
-            target: LOGGING_TARGET,
-            "service={} operation={} path={} written={} -> data written finished",
-            self.scheme,
-            self.op,
-            self.path,
-            self.written
-        );
-    }
-}
-
 #[async_trait]
 impl<W: oio::Write> oio::Write for LoggingWriter<W> {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let size = bs.len();
         match self.inner.write(bs).await {
             Ok(_) => {
                 self.written += size as u64;
@@ -1414,15 +1403,25 @@
                 Err(err)
             }
         }
     }
 
     async fn close(&mut self) -> Result<()> {
         match self.inner.close().await {
-            Ok(_) => Ok(()),
+            Ok(_) => {
+                debug!(
+                    target: LOGGING_TARGET,
+                    "service={} operation={} path={} written={} -> data written finished",
+                    self.scheme,
+                    self.op,
+                    self.path,
+                    self.written
+                );
+                Ok(())
+            }
             Err(err) => {
                 if let Some(lvl) = self.failure_level {
                     log!(
                         target: LOGGING_TARGET,
                         lvl,
                         "service={} operation={} path={} written={} -> data close failed: {err:?}",
                         self.scheme,
@@ -1469,15 +1468,25 @@
                 Err(err)
             }
         }
     }
 
     fn close(&mut self) -> Result<()> {
         match self.inner.close() {
-            Ok(_) => Ok(()),
+            Ok(_) => {
+                debug!(
+                    target: LOGGING_TARGET,
+                    "service={} operation={} path={} written={} -> data written finished",
+                    self.scheme,
+                    self.op,
+                    self.path,
+                    self.written
+                );
+                Ok(())
+            }
             Err(err) => {
                 if let Some(lvl) = self.failure_level {
                     log!(
                         target: LOGGING_TARGET,
                         lvl,
                         "service={} operation={} path={} written={} -> data close failed: {err:?}",
                         self.scheme,
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/madsim.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/madsim.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/metrics.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/metrics.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/minitrace.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/minitrace.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/oteltrace.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/oteltrace.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/prometheus.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/prometheus.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/retry.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/retry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/tracing.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/tracing.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/layers/type_eraser.rs` & `opendal-0.33.1/local_dependencies/opendal/src/layers/type_eraser.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/lib.rs` & `opendal-0.33.1/local_dependencies/opendal/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/accessor.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/accessor.rs`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,24 @@
 
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Underlying trait of all backends for implementors.
 ///
+/// The actual data access of storage service happens in Accessor layer.
+/// Every storage supported by OpenDAL must implement [`Accessor`] but not all
+/// methods of [`Accessor`] will be implemented according to how the storage service is.
+///
+/// For example, user can not modify the content from one HTTP file server directly.
+/// So [`Http`][crate::services::Http] implements and provides only read related actions.
+///
+/// [`Accessor`] gives default implementation for all methods which will raise [`ErrorKind::Unsupported`] error.
+/// And what action this [`Accessor`] supports will be pointed out in [`AccessorInfo`].
+///
 /// # Note
 ///
 /// Visit [`internals`][crate::docs::internals] for more tutorials.
 ///
 /// # Operations
 ///
 /// - Path in args will all be normalized into the same style, services
@@ -69,15 +79,14 @@
     /// This function is required to be implemented.
     ///
     /// By returning AccessorInfo, underlying services can declare
     /// some useful information about it self.
     ///
     /// - scheme: declare the scheme of backend.
     /// - capabilities: declare the capabilities of current backend.
-    /// - hints: declare the hints of current backend
     fn info(&self) -> AccessorInfo;
 
     /// Invoke the `create` operation on the specified path
     ///
     /// Require [`Capability::create_dir`]
     ///
     /// # Behavior
@@ -483,15 +492,15 @@
     }
 
     fn blocking_scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::BlockingPager)> {
         self.as_ref().blocking_scan(path, args)
     }
 }
 
-/// FusedAccessor is the type erased accessor with `Box<dyn Read>`.
+/// FusedAccessor is the type erased accessor with `Arc<dyn Accessor>`.
 pub type FusedAccessor = Arc<
     dyn Accessor<
         Reader = oio::Reader,
         BlockingReader = oio::BlockingReader,
         Writer = oio::Writer,
         BlockingWriter = oio::BlockingWriter,
         Pager = oio::Pager,
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,21 @@
 use bytes::Bytes;
 
 use super::Adapter;
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
-/// Backend of kv service.
+/// Backend of kv service. If the storage service is one k-v-like service, it should implement this kv [`Backend`] by right.
+///
+/// `Backend` implements one general logic on how to read, write, scan the data from one kv store efficiently.
+/// And the [`Adapter`] held by `Backend` will handle how to communicate with one k-v-like service really and provides
+/// a series of basic operation for this service.
+///
+/// OpenDAL developer can implement one new k-v store backend easily with help of this Backend.
 #[derive(Debug, Clone)]
 pub struct Backend<S: Adapter> {
     kv: Arc<S>,
     root: String,
 }
 
 impl<S> Backend<S>
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/adapters/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/adapters/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/chrono_util.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/chrono_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/body.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/body.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/client.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/client.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/header.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/header.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/http_util/uri.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/http_util/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/layer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/cursor.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/cursor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/entry.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/page.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/page.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/read.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/oio/write.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/oio/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/operation.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/operation.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/path.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/path.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/rps.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/rps.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/serde_util.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/serde_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/raw/version.rs` & `opendal-0.33.1/local_dependencies/opendal/src/raw/version.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/batch.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/batch.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/core.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/error.rs`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azblob/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azblob/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/core.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/error.rs`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/azdfs/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/azdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/dashmap/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/dashmap/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/dashmap/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/dashmap/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/fs/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/fs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -300,14 +300,15 @@
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Fs)
             .set_root(&self.root.to_string_lossy())
             .set_capability(Capability {
                 read: true,
                 read_can_seek: true,
                 write: true,
+                write_without_content_length: true,
                 create_dir: true,
                 list: true,
                 copy: true,
                 rename: true,
                 blocking: true,
                 ..Default::default()
             });
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/fs/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/fs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/fs/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/fs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/fs/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/fs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/fs/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/fs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ftp/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ftp/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ftp/err.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ftp/err.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ftp/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ftp/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ftp/util.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ftp/util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ftp/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ftp/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -373,26 +373,27 @@
         am.set_scheme(Scheme::Gcs)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
             .set_capability(Capability {
                 read: true,
                 read_can_next: true,
                 write: true,
+                write_without_content_length: true,
                 list: true,
                 scan: true,
                 copy: true,
                 ..Default::default()
             });
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
-        let mut req = self
-            .core
-            .gcs_insert_object_request(path, Some(0), None, AsyncBody::Empty)?;
+        let mut req =
+            self.core
+                .gcs_insert_object_request(path, Some(0), None, None, AsyncBody::Empty)?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         if resp.status().is_success() {
             resp.into_body().consume().await?;
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/core.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/core.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 use std::fmt::Formatter;
 use std::fmt::Write;
 
 use backon::ExponentialBuilder;
 use backon::Retryable;
 use bytes::Bytes;
 use bytes::BytesMut;
+use http::header::CACHE_CONTROL;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_RANGE;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
@@ -146,14 +147,15 @@
     }
 
     pub fn gcs_insert_object_request(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
+        cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let mut url = format!(
             "{}/upload/storage/v1/b/{}/o?uploadType={}&name={}",
             self.endpoint,
@@ -168,16 +170,18 @@
 
         if let Some(acl) = &self.predefined_acl {
             write!(&mut url, "&predefinedAcl={}", acl).unwrap();
         }
 
         let mut req = Request::post(&url);
 
-        if let Some(size) = size {
-            req = req.header(CONTENT_LENGTH, size)
+        req = req.header(CONTENT_LENGTH, size.unwrap_or_default());
+
+        if let Some(cache_control) = cache_control {
+            req = req.header(CACHE_CONTROL, cache_control)
         }
 
         if let Some(storage_class) = &self.default_storage_class {
             req = req.header(CONTENT_TYPE, "multipart/related; boundary=my-boundary");
 
             let mut req_body = BytesMut::with_capacity(100);
             write!(
@@ -321,17 +325,20 @@
         path: &str,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let url = format!(
             "{}/upload/storage/v1/b/{}/o?uploadType=resumable&name={}",
             self.endpoint, self.bucket, p
         );
+
         let mut req = Request::post(&url)
+            .header(CONTENT_LENGTH, 0)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
+
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
     pub fn gcs_upload_in_resumable_upload(
         &self,
         location: &str,
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/uri.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/gcs/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/gcs/writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     }
 
     async fn write_oneshot(&self, bs: Bytes) -> Result<()> {
         let mut req = self.core.gcs_insert_object_request(
             &percent_encode_path(&self.path),
             Some(bs.len()),
             self.op.content_type(),
+            self.op.cache_control(),
             AsyncBody::Bytes(bs),
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ghac/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ghac/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ghac/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ghac/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ghac/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ghac/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ghac/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ghac/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/hdfs/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/hdfs/writer.rs`

 * *Files 10% similar despite different names*

```diff
@@ -11,51 +11,51 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::io::Seek;
-use std::io::SeekFrom;
 use std::io::Write;
 
 use async_trait::async_trait;
 use bytes::Bytes;
-use futures::AsyncSeekExt;
 use futures::AsyncWriteExt;
 
 use super::error::parse_io_error;
 use crate::raw::*;
 use crate::*;
 
 pub struct HdfsWriter<F> {
     f: F,
-    pos: u64,
+    /// The position of current written bytes in the buffer.
+    ///
+    /// We will maintain the posstion in pos to make sure the buffer is written correctly.
+    pos: usize,
 }
 
 impl<F> HdfsWriter<F> {
     pub fn new(f: F) -> Self {
         Self { f, pos: 0 }
     }
 }
 
 #[async_trait]
 impl oio::Write for HdfsWriter<hdrs::AsyncFile> {
-    /// # Notes
-    ///
-    /// File could be partial written, so we will seek to start to make sure
-    /// we write the same content.
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        self.f
-            .seek(SeekFrom::Start(self.pos))
-            .await
-            .map_err(parse_io_error)?;
-        self.f.write_all(&bs).await.map_err(parse_io_error)?;
-        self.pos += bs.len() as u64;
+        while self.pos < bs.len() {
+            let n = self
+                .f
+                .write(&bs[self.pos..])
+                .await
+                .map_err(parse_io_error)?;
+            self.pos += n;
+        }
+        // Reset pos to 0 for next write.
+        self.pos = 0;
 
         Ok(())
     }
 
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
@@ -67,24 +67,21 @@
         self.f.close().await.map_err(parse_io_error)?;
 
         Ok(())
     }
 }
 
 impl oio::BlockingWrite for HdfsWriter<hdrs::File> {
-    /// # Notes
-    ///
-    /// File could be partial written, so we will seek to start to make sure
-    /// we write the same content.
     fn write(&mut self, bs: Bytes) -> Result<()> {
-        self.f
-            .seek(SeekFrom::Start(self.pos))
-            .map_err(parse_io_error)?;
-        self.f.write_all(&bs).map_err(parse_io_error)?;
-        self.pos += bs.len() as u64;
+        while self.pos < bs.len() {
+            let n = self.f.write(&bs[self.pos..]).map_err(parse_io_error)?;
+            self.pos += n;
+        }
+        // Reset pos to 0 for next write.
+        self.pos = 0;
 
         Ok(())
     }
 
     fn close(&mut self) -> Result<()> {
         self.f.flush().map_err(parse_io_error)?;
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/http/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/http/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/http/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/http/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/http/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/ipld.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/ipld.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ipfs/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ipfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/builder.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/ipmfs/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/ipmfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt` & `opendal-0.33.1/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/memcached/ascii.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/memcached/ascii.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/memcached/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/memcached/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/memcached/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/memcached/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/memory/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/memory/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 /// - [x] blocking
 #[derive(Default)]
 pub struct MemoryBuilder {
     root: Option<String>,
 }
 
 impl MemoryBuilder {
-    /// Set the root for dashmap.
+    /// Set the root for BTreeMap.
     pub fn root(&mut self, path: &str) -> &mut Self {
         self.root = Some(path.into());
         self
     }
 }
 
 impl Builder for MemoryBuilder {
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/memory/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/memory/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/moka/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/moka/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/moka/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/obs/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/obs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -337,15 +337,15 @@
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let resp = self
             .core
-            .obs_get_object(path, args.range(), args.if_match())
+            .obs_get_object(path, args.range(), args.if_match(), args.if_none_match())
             .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
@@ -385,15 +385,18 @@
 
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self.core.obs_get_head_object(path, args.if_match()).await?;
+        let resp = self
+            .core
+            .obs_get_head_object(path, args.if_match(), args.if_none_match())
+            .await?;
 
         let status = resp.status();
 
         // The response is very similar to azblob.
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             StatusCode::NOT_FOUND if path.ends_with('/') => {
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/obs/core.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/obs/core.rs`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 use std::fmt::Debug;
 use std::fmt::Formatter;
 
 use http::header::CACHE_CONTROL;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
+use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
 use reqsign::HuaweicloudObsCredential;
 use reqsign::HuaweicloudObsCredentialLoader;
 use reqsign::HuaweicloudObsSigner;
 
 use crate::raw::*;
@@ -84,14 +85,15 @@
 
 impl ObsCore {
     pub async fn obs_get_object(
         &self,
         path: &str,
         range: BytesRange,
         if_match: Option<&str>,
+        if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::get(&url);
 
@@ -99,14 +101,18 @@
             req = req.header(IF_MATCH, if_match);
         }
 
         if !range.is_full() {
             req = req.header(http::header::RANGE, range.to_header())
         }
 
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+
         let mut req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
@@ -142,28 +148,33 @@
         Ok(req)
     }
 
     pub async fn obs_get_head_object(
         &self,
         path: &str,
         if_match: Option<&str>,
+        if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         // The header 'Origin' is optional for API calling, the doc has mistake, confirmed with customer service of huaweicloud.
         // https://support.huaweicloud.com/intl/en-us/api-obs/obs_04_0084.html
 
         let mut req = Request::head(&url);
 
         if let Some(if_match) = if_match {
             req = req.header(IF_MATCH, if_match);
         }
 
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+
         let mut req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/obs/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/obs/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         // OBS could return `520 Origin Error` errors which should be retried.
         v if v.as_u16() == 520 => (ErrorKind::Unexpected, true),
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/obs/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/obs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/obs/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/obs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/obs/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/obs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/oss/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/oss/backend.rs`

 * *Files 13% similar despite different names*

```diff
@@ -110,14 +110,18 @@
 pub struct OssBuilder {
     root: Option<String>,
 
     endpoint: Option<String>,
     presign_endpoint: Option<String>,
     bucket: String,
 
+    // sse options
+    server_side_encryption: Option<String>,
+    server_side_encryption_key_id: Option<String>,
+
     // authenticate options
     access_key_id: Option<String>,
     access_key_secret: Option<String>,
 
     http_client: Option<HttpClient>,
 }
 
@@ -249,14 +253,49 @@
             None => {
                 return Err(Error::new(ErrorKind::ConfigInvalid, "endpoint is empty")
                     .with_context("service", Scheme::Oss));
             }
         };
         Ok((endpoint, host))
     }
+
+    /// Set server_side_encryption for this backend.
+    ///
+    /// Available values: `AES256`, `KMS`.
+    ///
+    /// Reference: <https://www.alibabacloud.com/help/en/object-storage-service/latest/server-side-encryption-5>
+    /// Brief explanation:
+    /// There are two server-side encryption methods available:
+    /// SSE-AES256:
+    ///     1. Configure the bucket encryption mode as OSS-managed and specify the encryption algorithm as AES256.
+    ///     2. Include the `x-oss-server-side-encryption` parameter in the request and set its value to AES256.
+    /// SSE-KMS:
+    ///     1. To use this service, you need to first enable KMS.
+    ///     2. Configure the bucket encryption mode as KMS, and specify the specific CMK ID for BYOK (Bring Your Own Key)
+    ///        or not specify the specific CMK ID for OSS-managed KMS key.
+    ///     3. Include the `x-oss-server-side-encryption` parameter in the request and set its value to KMS.
+    ///     4. If a specific CMK ID is specified, include the `x-oss-server-side-encryption-key-id` parameter in the request, and set its value to the specified CMK ID.
+    pub fn server_side_encryption(&mut self, v: &str) -> &mut Self {
+        if !v.is_empty() {
+            self.server_side_encryption = Some(v.to_string())
+        }
+        self
+    }
+
+    /// Set server_side_encryption_key_id for this backend.
+    ///
+    /// # Notes
+    ///
+    /// This option only takes effect when server_side_encryption equals to KMS.
+    pub fn server_side_encryption_key_id(&mut self, v: &str) -> &mut Self {
+        if !v.is_empty() {
+            self.server_side_encryption_key_id = Some(v.to_string())
+        }
+        self
+    }
 }
 
 impl Builder for OssBuilder {
     const SCHEME: Scheme = Scheme::Oss;
     type Accessor = OssBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
@@ -266,15 +305,18 @@
         map.get("bucket").map(|v| builder.bucket(v));
         map.get("endpoint").map(|v| builder.endpoint(v));
         map.get("presign_endpoint")
             .map(|v| builder.presign_endpoint(v));
         map.get("access_key_id").map(|v| builder.access_key_id(v));
         map.get("access_key_secret")
             .map(|v| builder.access_key_secret(v));
-
+        map.get("server_side_encryption")
+            .map(|v| builder.server_side_encryption(v));
+        map.get("server_side_encryption_key_id")
+            .map(|v| builder.server_side_encryption_key_id(v));
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         debug!("backend build started: {:?}", &self);
 
         let root = normalize_root(&self.root.clone().unwrap_or_default());
@@ -306,14 +348,30 @@
         let presign_endpoint = if self.presign_endpoint.is_some() {
             self.parse_endpoint(&self.presign_endpoint, bucket)?.0
         } else {
             endpoint.clone()
         };
         debug!("backend use presign_endpoint: {}", &presign_endpoint);
 
+        let server_side_encryption = match &self.server_side_encryption {
+            None => None,
+            Some(v) => Some(
+                build_header_value(v)
+                    .map_err(|err| err.with_context("key", "server_side_encryption"))?,
+            ),
+        };
+
+        let server_side_encryption_key_id = match &self.server_side_encryption_key_id {
+            None => None,
+            Some(v) => Some(
+                build_header_value(v)
+                    .map_err(|err| err.with_context("key", "server_side_encryption_key_id"))?,
+            ),
+        };
+
         let mut cfg = AliyunConfig::default();
         // Load cfg from env first.
         cfg = cfg.from_env();
 
         if let Some(v) = self.access_key_id.take() {
             cfg.access_key_id = Some(v);
         }
@@ -334,14 +392,16 @@
                 bucket: bucket.to_owned(),
                 endpoint,
                 host,
                 presign_endpoint,
                 signer,
                 loader,
                 client,
+                server_side_encryption,
+                server_side_encryption_key_id,
             }),
         })
     }
 }
 
 #[derive(Debug, Clone)]
 /// Aliyun Object Storage Service backend
@@ -363,14 +423,15 @@
         am.set_scheme(Scheme::Oss)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
             .set_capability(Capability {
                 read: true,
                 read_can_next: true,
                 write: true,
+                write_without_content_length: true,
                 list: true,
                 scan: true,
                 copy: true,
                 presign: true,
                 batch: true,
                 batch_max_operations: Some(1000),
                 ..Default::default()
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/oss/core.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/oss/core.rs`

 * *Files 4% similar despite different names*

```diff
@@ -23,40 +23,49 @@
 use http::header::CACHE_CONTROL;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
 use http::header::RANGE;
+use http::HeaderName;
+use http::HeaderValue;
 use http::Request;
 use http::Response;
 use reqsign::AliyunCredential;
 use reqsign::AliyunLoader;
 use reqsign::AliyunOssSigner;
 use serde::Deserialize;
 use serde::Serialize;
 
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 mod constants {
+    pub const X_OSS_SERVER_SIDE_ENCRYPTION: &str = "x-oss-server-side-encryption";
+
+    pub const X_OSS_SERVER_SIDE_ENCRYPTION_KEY_ID: &str = "x-oss-server-side-encryption-key-id";
+
     pub const RESPONSE_CONTENT_DISPOSITION: &str = "response-content-disposition";
 }
 
 pub struct OssCore {
     pub root: String,
     pub bucket: String,
     /// buffered host string
     ///
     /// format: <bucket-name>.<endpoint-domain-name>
     pub host: String,
     pub endpoint: String,
     pub presign_endpoint: String,
 
+    pub server_side_encryption: Option<HeaderValue>,
+    pub server_side_encryption_key_id: Option<HeaderValue>,
+
     pub client: HttpClient,
     pub loader: AliyunLoader,
     pub signer: AliyunOssSigner,
 }
 
 impl Debug for OssCore {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
@@ -106,14 +115,39 @@
             .map_err(new_request_sign_error)
     }
 
     #[inline]
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
         self.client.send(req).await
     }
+
+    /// Set sse headers
+    /// # Note
+    /// According to the OSS documentation, only PutObject, CopyObject, and InitiateMultipartUpload may require to be set.
+    pub fn insert_sse_headers(&self, mut req: http::request::Builder) -> http::request::Builder {
+        if let Some(v) = &self.server_side_encryption {
+            let mut v = v.clone();
+            v.set_sensitive(true);
+
+            req = req.header(
+                HeaderName::from_static(constants::X_OSS_SERVER_SIDE_ENCRYPTION),
+                v,
+            )
+        }
+        if let Some(v) = &self.server_side_encryption_key_id {
+            let mut v = v.clone();
+            v.set_sensitive(true);
+
+            req = req.header(
+                HeaderName::from_static(constants::X_OSS_SERVER_SIDE_ENCRYPTION_KEY_ID),
+                v,
+            )
+        }
+        req
+    }
 }
 
 impl OssCore {
     #[allow(clippy::too_many_arguments)]
     pub fn oss_put_object_request(
         &self,
         path: &str,
@@ -140,14 +174,17 @@
             req = req.header(CONTENT_DISPOSITION, pos);
         }
 
         if let Some(cache_control) = cache_control {
             req = req.header(CACHE_CONTROL, cache_control)
         }
 
+        // set sse headers
+        req = self.insert_sse_headers(req);
+
         let req = req.body(body).map_err(new_request_build_error)?;
         Ok(req)
     }
 
     pub fn oss_get_object_request(
         &self,
         path: &str,
@@ -329,16 +366,21 @@
         let url = format!(
             "{}/{}",
             self.get_endpoint(false),
             percent_encode_path(&target)
         );
         let source = format!("/{}/{}", self.bucket, percent_encode_path(&source));
 
-        let mut req = Request::put(&url)
-            .header("x-oss-copy-source", source)
+        let mut req = Request::put(&url);
+
+        req = self.insert_sse_headers(req);
+
+        req = req.header("x-oss-copy-source", source);
+
+        let mut req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
@@ -434,15 +476,15 @@
         }
         if let Some(disposition) = content_disposition {
             req = req.header(CONTENT_DISPOSITION, disposition);
         }
         if let Some(cache_control) = cache_control {
             req = req.header(CACHE_CONTROL, cache_control);
         }
-
+        req = self.insert_sse_headers(req);
         let mut req = req.body(body).map_err(new_request_build_error)?;
         self.sign(&mut req).await?;
         Ok(req)
     }
 
     /// Creates a request to upload a part
     pub async fn oss_upload_part_request(
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/oss/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/oss/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/oss/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/oss/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/oss/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/oss/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/oss/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/oss/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/redis/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/redis/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/redis/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/rocksdb/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/rocksdb/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/rocksdb/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/rocksdb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/s3/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/s3/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,16 @@
     m.insert(
         "https://s3.amazonaws.com",
         "https://s3.{region}.amazonaws.com",
     );
     m
 });
 
-/// Aws S3 and compatible services (including minio, digitalocean space and so on) support
+/// Aws S3 and compatible services (including minio, digitalocean space, Tencent Cloud Object Storage(COS) and so on) support.
+/// For more information about s3-compatible services, refer to [Compatible Services](#compatible-services).
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
@@ -919,15 +920,20 @@
                 read: true,
                 read_can_next: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
                 read_with_override_content_disposition: true,
 
                 write: true,
+                write_without_content_length: true,
+
                 list: true,
+                list_with_limit: true,
+                list_with_start_after: true,
+
                 scan: true,
                 copy: true,
                 presign: true,
                 batch: true,
                 batch_max_operations: Some(1000),
 
                 ..Default::default()
@@ -1035,22 +1041,28 @@
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         Ok((
             RpList::default(),
-            S3Pager::new(self.core.clone(), path, "/", args.limit()),
+            S3Pager::new(
+                self.core.clone(),
+                path,
+                "/",
+                args.limit(),
+                args.start_after(),
+            ),
         ))
     }
 
     async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
         Ok((
             RpScan::default(),
-            S3Pager::new(self.core.clone(), path, "", args.limit()),
+            S3Pager::new(self.core.clone(), path, "", args.limit(), None),
         ))
     }
 
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
             PresignOperation::Stat(v) => {
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/s3/compatible_services.md` & `opendal-0.33.1/local_dependencies/opendal/src/services/s3/compatible_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/s3/core.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/s3/core.rs`

 * *Files 2% similar despite different names*

```diff
@@ -450,28 +450,34 @@
     /// on this.
     pub async fn s3_list_objects(
         &self,
         path: &str,
         continuation_token: &str,
         delimiter: &str,
         limit: Option<usize>,
+        start_after: Option<String>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let mut url = format!("{}?list-type=2", self.endpoint);
         if !p.is_empty() {
             write!(url, "&prefix={}", percent_encode_path(&p))
                 .expect("write into string must succeed");
         }
         if !delimiter.is_empty() {
             write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
         }
         if let Some(limit) = limit {
             write!(url, "&max-keys={limit}").expect("write into string must succeed");
         }
+        if let Some(start_after) = start_after {
+            let start_after = build_abs_path(&self.root, &start_after);
+            write!(url, "&start-after={}", percent_encode_path(&start_after))
+                .expect("write into string must succeed");
+        }
         if !continuation_token.is_empty() {
             // AWS S3 could return continuation-token that contains `=`
             // which could lead `reqsign` parse query wrongly.
             // URL encode continuation-token before starting signing so that
             // our signer will not be confused.
             write!(
                 url,
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/s3/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/s3/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,17 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (mut kind, mut retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
+        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
+            (ErrorKind::ConditionNotMatch, false)
+        }
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/s3/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/s3/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/s3/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/pager.rs`

 * *Files 2% similar despite different names*

```diff
@@ -18,57 +18,57 @@
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Buf;
 use quick_xml::de;
 use serde::Deserialize;
 
-use super::core::S3Core;
+use super::core::WasabiCore;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::EntryMode;
 use crate::Metadata;
 use crate::Result;
 
-pub struct S3Pager {
-    core: Arc<S3Core>,
+pub struct WasabiPager {
+    core: Arc<WasabiCore>,
 
     path: String,
     delimiter: String,
     limit: Option<usize>,
 
     token: String,
     done: bool,
 }
 
-impl S3Pager {
-    pub fn new(core: Arc<S3Core>, path: &str, delimiter: &str, limit: Option<usize>) -> Self {
+impl WasabiPager {
+    pub fn new(core: Arc<WasabiCore>, path: &str, delimiter: &str, limit: Option<usize>) -> Self {
         Self {
             core,
 
             path: path.to_string(),
             delimiter: delimiter.to_string(),
             limit,
 
             token: "".to_string(),
             done: false,
         }
     }
 }
 
 #[async_trait]
-impl oio::Page for S3Pager {
+impl oio::Page for WasabiPager {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         if self.done {
             return Ok(None);
         }
 
         let resp = self
             .core
-            .s3_list_objects(&self.path, &self.token, &self.delimiter, self.limit)
+            .list_objects(&self.path, &self.token, &self.delimiter, self.limit)
             .await?;
 
         if resp.status() != http::StatusCode::OK {
             return Err(parse_error(resp).await?);
         }
 
         let bs = resp.into_body().bytes().await?;
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/s3/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/s3/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/sled/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/sled/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/sled/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/sled/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/core.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (mut kind, mut retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/s3/pager.rs`

 * *Files 4% similar despite different names*

```diff
@@ -18,57 +18,71 @@
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Buf;
 use quick_xml::de;
 use serde::Deserialize;
 
-use super::core::WasabiCore;
+use super::core::S3Core;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::EntryMode;
 use crate::Metadata;
 use crate::Result;
 
-pub struct WasabiPager {
-    core: Arc<WasabiCore>,
+pub struct S3Pager {
+    core: Arc<S3Core>,
 
     path: String,
     delimiter: String,
     limit: Option<usize>,
+    start_after: Option<String>,
 
     token: String,
     done: bool,
 }
 
-impl WasabiPager {
-    pub fn new(core: Arc<WasabiCore>, path: &str, delimiter: &str, limit: Option<usize>) -> Self {
+impl S3Pager {
+    pub fn new(
+        core: Arc<S3Core>,
+        path: &str,
+        delimiter: &str,
+        limit: Option<usize>,
+        start_after: Option<&str>,
+    ) -> Self {
         Self {
             core,
 
             path: path.to_string(),
             delimiter: delimiter.to_string(),
             limit,
+            start_after: start_after.map(String::from),
 
             token: "".to_string(),
             done: false,
         }
     }
 }
 
 #[async_trait]
-impl oio::Page for WasabiPager {
+impl oio::Page for S3Pager {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         if self.done {
             return Ok(None);
         }
 
         let resp = self
             .core
-            .list_objects(&self.path, &self.token, &self.delimiter, self.limit)
+            .s3_list_objects(
+                &self.path,
+                &self.token,
+                &self.delimiter,
+                self.limit,
+                self.start_after.clone(),
+            )
             .await?;
 
         if resp.status() != http::StatusCode::OK {
             return Err(parse_error(resp).await?);
         }
 
         let bs = resp.into_body().bytes().await?;
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/wasabi/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/wasabi/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/http/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf` & `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf` & `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/list_response.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/list_response.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webdav/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/webdav/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/backend.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/message.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/message.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/pager.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/services/webhdfs/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/services/webhdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/capability.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/capability.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/entry.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/error.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/error.rs`

 * *Files 3% similar despite different names*

```diff
@@ -66,19 +66,25 @@
     NotADirectory,
     /// The given path already exists thus we failed to the specified operation on it.
     AlreadyExists,
     /// Requests that sent to this path is over the limit, please slow down.
     RateLimited,
     /// The given file paths are same.
     IsSameFile,
-    /// The preconfition of this operation is not met.
+    /// The condition of this operation is not match.
     ///
-    /// For example, reading a file with If-Match header but the file's ETag
-    /// is not match.
-    PreconditionFailed,
+    /// The `condition` itself is context based.
+    ///
+    /// For example, in S3, the `condition` can be:
+    /// 1. writing a file with If-Match header but the file's ETag is not match (will get a 412 Precondition Failed).
+    /// 2. reading a file with If-None-Match header but the file's ETag is match (will get a 304 Not Modified).
+    ///
+    /// As OpenDAL cannot handle the `condition not match` error, it will always return this error to users.
+    /// So users could to handle this error by themselves.
+    ConditionNotMatch,
     /// The content is truncated.
     ///
     /// This error kind means there are more content to come but been truncated.
     ///
     /// For examples:
     ///
     /// - Users expected to read 1024 bytes, but service returned more bytes.
@@ -117,15 +123,15 @@
             ErrorKind::NotFound => "NotFound",
             ErrorKind::PermissionDenied => "PermissionDenied",
             ErrorKind::IsADirectory => "IsADirectory",
             ErrorKind::NotADirectory => "NotADirectory",
             ErrorKind::AlreadyExists => "AlreadyExists",
             ErrorKind::RateLimited => "RateLimited",
             ErrorKind::IsSameFile => "IsSameFile",
-            ErrorKind::PreconditionFailed => "PreconditionFailed",
+            ErrorKind::ConditionNotMatch => "ConditionNotMatch",
             ErrorKind::ContentTruncated => "ContentTruncated",
             ErrorKind::ContentIncomplete => "ContentIncomplete",
         }
     }
 }
 
 #[derive(Clone, Copy, Debug, PartialEq, Eq)]
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/list.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/list.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/metadata.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/mode.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/mode.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/operator/builder.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/operator/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/operator/metadata.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/operator/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/operator/mod.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/operator/operator.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/operator/operator.rs`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 
 use super::BlockingOperator;
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Operator is the entry for all public async APIs.
+/// Developer should manipulate the data from storage service through Operator only by right.
 ///
+/// We will usually do some general checks and data transformations in this layer,
+/// like normalizing path from input, checking whether the path refers to one file or one directory, and so on.
 /// Read [`concepts`][docs::concepts] for know more about [`Operator`].
 ///
 /// # Examples
 ///
 /// Read more backend init examples in [`services`]
 ///
 /// ```
@@ -57,16 +60,18 @@
 ///     let _: Operator = Operator::new(builder)?.finish();
 ///
 ///     Ok(())
 /// }
 /// ```
 #[derive(Clone, Debug)]
 pub struct Operator {
+    // accessor is what Operator delegates for
     accessor: FusedAccessor,
 
+    // limit is usually the maximum size of data that operator will handle in one operation
     limit: usize,
 }
 
 /// # Operator basic API.
 impl Operator {
     pub(super) fn inner(&self) -> &FusedAccessor {
         &self.accessor
@@ -81,15 +86,16 @@
         Self { accessor, limit }
     }
 
     pub(super) fn into_inner(self) -> FusedAccessor {
         self.accessor
     }
 
-    /// Get current operator's limit
+    /// Get current operator's limit.
+    /// Limit is usually the maximum size of data that operator will handle in one operation.
     pub fn limit(&self) -> usize {
         self.limit
     }
 
     /// Specify the batch limit.
     ///
     /// Default: 1000
```

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/ops.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/ops.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/reader.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/reader.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/scheme.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/scheme.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/local_dependencies/opendal/src/types/writer.rs` & `opendal-0.33.1/local_dependencies/opendal/src/types/writer.rs`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,19 @@
 use crate::*;
 
 /// Writer is designed to write data into given path in an asynchronous
 /// manner.
 ///
 /// ## Notes
 ///
+/// Please make sure either `close` or `abort` has been called before
+/// dropping the writer otherwise the data could be lost.
+///
+/// ## Notes
+///
 /// Writer can be used in two ways:
 ///
 /// - Sized: write data with a known size by specify the content length.
 /// - Unsized: write data with an unknown size, also known as streaming.
 ///
 /// All services will support `sized` writer and provide special optimization if
 /// the given data size is the same as the content length, allowing them to
@@ -77,27 +82,37 @@
             unreachable!(
                 "writer state invalid while write, expect Idle, actual {}",
                 self.state
             );
         }
     }
 
-    /// Abort inner writer.
+    /// Abort the writer and clean up all written data.
+    ///
+    /// ## Notes
+    ///
+    /// Abort should only be called when the writer is not closed or
+    /// aborted, otherwise an unexpected error could be returned.
     pub async fn abort(&mut self) -> Result<()> {
         if let State::Idle(Some(w)) = &mut self.state {
             w.abort().await
         } else {
             unreachable!(
                 "writer state invalid while abort, expect Idle, actual {}",
                 self.state
             );
         }
     }
 
-    /// Close the writer and make sure all data have been stored.
+    /// Close the writer and make sure all data have been committed.
+    ///
+    /// ## Notes
+    ///
+    /// Close should only be called when the writer is not closed or
+    /// aborted, otherwise an unexpected error could be returned.
     pub async fn close(&mut self) -> Result<()> {
         if let State::Idle(Some(w)) = &mut self.state {
             w.close().await
         } else {
             unreachable!(
                 "writer state invalid while close, expect Idle, actual {}",
                 self.state
```

### Comparing `opendal-0.33.0/Cargo.toml` & `opendal-0.33.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.64"
-version= "0.33.0"
+version= "0.33.1"
 
 [lib]
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 chrono = { version = "0.4.24", default-features = false, features = ["std"] }
```

### Comparing `opendal-0.33.0/.gitignore` & `opendal-0.33.1/.gitignore`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/README.md` & `opendal-0.33.1/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/benchmark/README.md` & `opendal-0.33.1/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/benchmark/async_opendal_benchmark.py` & `opendal-0.33.1/benchmark/async_opendal_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/benchmark/async_origin_s3_benchmark_with_gevent.py` & `opendal-0.33.1/benchmark/async_origin_s3_benchmark_with_gevent.py`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/examples/object.ipynb` & `opendal-0.33.1/examples/object.ipynb`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/pyproject.toml` & `opendal-0.33.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/python/opendal/__init__.py` & `opendal-0.33.1/python/opendal/__init__.py`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/python/opendal/__init__.pyi` & `opendal-0.33.1/python/opendal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/src/asyncio.rs` & `opendal-0.33.1/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/src/layers.rs` & `opendal-0.33.1/src/layers.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/src/lib.rs` & `opendal-0.33.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/tests/binding.feature` & `opendal-0.33.1/tests/binding.feature`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/tests/steps/binding.py` & `opendal-0.33.1/tests/steps/binding.py`

 * *Files identical despite different names*

### Comparing `opendal-0.33.0/Cargo.lock` & `opendal-0.33.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -2289,15 +2289,15 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "oay"
-version = "0.33.0"
+version = "0.33.1"
 dependencies = [
  "anyhow",
  "clap 4.1.11",
  "dirs",
  "env_logger",
  "futures",
  "log",
@@ -2326,27 +2326,27 @@
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "object_store_opendal"
-version = "0.33.0"
+version = "0.33.1"
 dependencies = [
  "async-trait",
  "bytes",
  "futures",
  "object_store",
  "opendal",
  "tokio",
 ]
 
 [[package]]
 name = "oli"
-version = "0.33.0"
+version = "0.33.1"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "clap 4.1.11",
  "dirs",
  "env_logger",
  "futures",
@@ -2369,15 +2369,15 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opendal"
-version = "0.33.0"
+version = "0.33.1"
 dependencies = [
  "anyhow",
  "async-compat",
  "async-tls",
  "async-trait",
  "backon",
  "base64 0.21.0",
@@ -2446,26 +2446,26 @@
 dependencies = [
  "jni",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-nodejs"
-version = "0.33.0"
+version = "0.33.1"
 dependencies = [
  "futures",
  "napi",
  "napi-build",
  "napi-derive",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-python"
-version = "0.33.0"
+version = "0.33.1"
 dependencies = [
  "chrono",
  "futures",
  "opendal",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
```

### Comparing `opendal-0.33.0/PKG-INFO` & `opendal-0.33.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: opendal
-Version: 0.33.0
+Version: 0.33.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pdoc; extra == 'docs'
+Requires-Dist: behave; extra == 'test'
 Requires-Dist: gevent; extra == 'benchmark'
 Requires-Dist: greenify; extra == 'benchmark'
 Requires-Dist: greenlet; extra == 'benchmark'
 Requires-Dist: boto3; extra == 'benchmark'
 Requires-Dist: pydantic; extra == 'benchmark'
 Requires-Dist: boto3-stubs[essential]; extra == 'benchmark'
-Requires-Dist: behave; extra == 'test'
 Provides-Extra: docs
-Provides-Extra: benchmark
 Provides-Extra: test
+Provides-Extra: benchmark
 Summary: OpenDAL Python Binding
 Home-Page: https://opendal.apache.org/
 Author: OpenDAL Contributors <dev@opendal.apache.org>
 Author-email: OpenDAL Contributors <dev@opendal.apache.org>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

