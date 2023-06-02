# Comparing `tmp/opendal-0.35.0.tar.gz` & `tmp/opendal-0.36.1.tar.gz`

## Comparing `opendal-0.35.0.tar` & `opendal-0.36.1.tar`

### file list

```diff
@@ -1,298 +1,319 @@
--rw-r--r--   0        0        0     6232 1970-01-01 00:00:00.000000 opendal-0.35.0/local_dependencies/opendal/Cargo.toml
--rw-r--r--   0     1001      123    72241 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/CHANGELOG.md
--rw-r--r--   0     1001      123     1114 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/CONTRIBUTING.md
--rw-r--r--   0     1001      123     6804 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/README.md
--rw-r--r--   0     1001      123      378 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/benches/README.md
--rw-r--r--   0     1001      123      672 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/benches/ops/README.md
--rw-r--r--   0     1001      123      979 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/benches/ops/main.rs
--rw-r--r--   0     1001      123     5574 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/benches/ops/read.rs
--rw-r--r--   0     1001      123     2792 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/benches/ops/utils.rs
--rw-r--r--   0     1001      123     2163 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/benches/ops/write.rs
--rw-r--r--   0     1001      123     1823 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/examples/object.rs
--rw-r--r--   0     1001      123     1290 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
--rw-r--r--   0     1001      123     7682 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
--rw-r--r--   0     1001      123     6142 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/concepts.rs
--rw-r--r--   0     1001      123      982 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/features.md
--rw-r--r--   0     1001      123    10879 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/internals/accessor.rs
--rw-r--r--   0     1001      123     1765 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/internals/layer.rs
--rw-r--r--   0     1001      123     3409 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/internals/mod.rs
--rw-r--r--   0     1001      123     1458 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/mod.rs
--rw-r--r--   0     1001      123     3436 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
--rw-r--r--   0     1001      123     5329 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
--rw-r--r--   0     1001      123     4885 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
--rw-r--r--   0     1001      123     5428 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
--rw-r--r--   0     1001      123     3341 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
--rw-r--r--   0     1001      123     4425 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
--rw-r--r--   0     1001      123     2902 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
--rw-r--r--   0     1001      123    12349 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
--rw-r--r--   0     1001      123     2538 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
--rw-r--r--   0     1001      123     2347 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
--rw-r--r--   0     1001      123     2805 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
--rw-r--r--   0     1001      123     1803 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
--rw-r--r--   0     1001      123     4733 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
--rw-r--r--   0     1001      123     2184 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
--rw-r--r--   0     1001      123     5771 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
--rw-r--r--   0     1001      123     8563 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
--rw-r--r--   0     1001      123     3113 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
--rw-r--r--   0     1001      123     4321 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
--rw-r--r--   0     1001      123     1881 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
--rw-r--r--   0     1001      123     2926 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
--rw-r--r--   0     1001      123     2246 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
--rw-r--r--   0     1001      123     6523 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
--rw-r--r--   0     1001      123     4792 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
--rw-r--r--   0     1001      123    10091 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
--rw-r--r--   0     1001      123     2508 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
--rw-r--r--   0     1001      123     2670 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
--rw-r--r--   0     1001      123     8059 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
--rw-r--r--   0     1001      123     2472 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
--rw-r--r--   0     1001      123     4452 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
--rw-r--r--   0     1001      123     2534 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
--rw-r--r--   0     1001      123     3693 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
--rw-r--r--   0     1001      123     3255 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
--rw-r--r--   0     1001      123     4133 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
--rw-r--r--   0     1001      123     4408 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
--rw-r--r--   0     1001      123     4230 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
--rw-r--r--   0     1001      123     3172 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
--rw-r--r--   0     1001      123     2687 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md
--rw-r--r--   0     1001      123     4554 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
--rw-r--r--   0     1001      123    24636 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/upgrade.md
--rw-r--r--   0     1001      123     6641 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/chaos.rs
--rw-r--r--   0     1001      123    22169 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/complete.rs
--rw-r--r--   0     1001      123     9848 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
--rw-r--r--   0     1001      123    17440 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/error_context.rs
--rw-r--r--   0     1001      123    14233 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/immutable_index.rs
--rw-r--r--   0     1001      123    52926 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/logging.rs
--rw-r--r--   0     1001      123    13301 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/madsim.rs
--rw-r--r--   0     1001      123    29707 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/metrics.rs
--rw-r--r--   0     1001      123    12389 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/minitrace.rs
--rw-r--r--   0     1001      123     2205 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/mod.rs
--rw-r--r--   0     1001      123    13121 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/oteltrace.rs
--rw-r--r--   0     1001      123    23065 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/prometheus.rs
--rw-r--r--   0     1001      123    38385 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/retry.rs
--rw-r--r--   0     1001      123    11997 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/tracing.rs
--rw-r--r--   0     1001      123     3663 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/type_eraser.rs
--rw-r--r--   0     1001      123     3570 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/lib.rs
--rw-r--r--   0     1001      123    18884 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/accessor.rs
--rw-r--r--   0     1001      123     5049 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
--rw-r--r--   0     1001      123    10382 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
--rw-r--r--   0     1001      123     1020 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
--rw-r--r--   0     1001      123     1566 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/mod.rs
--rw-r--r--   0     1001      123     5407 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs
--rw-r--r--   0     1001      123    10368 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs
--rw-r--r--   0     1001      123     1067 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs
--rw-r--r--   0     1001      123     1934 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/chrono_util.rs
--rw-r--r--   0     1001      123     5973 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/body.rs
--rw-r--r--   0     1001      123    10135 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
--rw-r--r--   0     1001      123    10534 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
--rw-r--r--   0     1001      123     5424 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/client.rs
--rw-r--r--   0     1001      123     3415 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/error.rs
--rw-r--r--   0     1001      123    11165 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/header.rs
--rw-r--r--   0     1001      123     2159 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/mod.rs
--rw-r--r--   0     1001      123    21679 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/multipart.rs
--rw-r--r--   0     1001      123     2962 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/uri.rs
--rw-r--r--   0     1001      123    11756 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/layer.rs
--rw-r--r--   0     1001      123     1950 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/mod.rs
--rw-r--r--   0     1001      123     3018 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/append.rs
--rw-r--r--   0     1001      123     9434 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/cursor.rs
--rw-r--r--   0     1001      123     2512 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/entry.rs
--rw-r--r--   0     1001      123     3666 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
--rw-r--r--   0     1001      123     1006 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
--rw-r--r--   0     1001      123    15427 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
--rw-r--r--   0     1001      123     4150 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
--rw-r--r--   0     1001      123     1686 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
--rw-r--r--   0     1001      123     4579 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs
--rw-r--r--   0     1001      123     2097 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/mod.rs
--rw-r--r--   0     1001      123     3516 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/page.rs
--rw-r--r--   0     1001      123    10670 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/read.rs
--rw-r--r--   0     1001      123     9177 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
--rw-r--r--   0     1001      123     6894 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
--rw-r--r--   0     1001      123     5206 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/write.rs
--rw-r--r--   0     1001      123     3953 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/operation.rs
--rw-r--r--   0     1001      123    11671 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/path.rs
--rw-r--r--   0     1001      123     6507 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/rps.rs
--rw-r--r--   0     1001      123     1396 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/serde_util.rs
--rw-r--r--   0     1001      123     1077 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/version.rs
--rw-r--r--   0     1001      123    26673 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/backend.rs
--rw-r--r--   0     1001      123     5544 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/batch.rs
--rw-r--r--   0     1001      123    11380 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/core.rs
--rw-r--r--   0     1001      123     2286 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/docs.md
--rw-r--r--   0     1001      123     5870 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/error.rs
--rw-r--r--   0     1001      123      913 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/mod.rs
--rw-r--r--   0     1001      123    14196 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/pager.rs
--rw-r--r--   0     1001      123     2079 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/writer.rs
--rw-r--r--   0     1001      123    16596 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/backend.rs
--rw-r--r--   0     1001      123     9557 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/core.rs
--rw-r--r--   0     1001      123     3519 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/error.rs
--rw-r--r--   0     1001      123      900 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/mod.rs
--rw-r--r--   0     1001      123     5647 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/pager.rs
--rw-r--r--   0     1001      123     2736 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/writer.rs
--rw-r--r--   0     1001      123    14710 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/cos/backend.rs
--rw-r--r--   0     1001      123     8178 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/cos/core.rs
--rw-r--r--   0     1001      123     3492 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/cos/error.rs
--rw-r--r--   0     1001      123      896 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/cos/mod.rs
--rw-r--r--   0     1001      123     5963 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/cos/pager.rs
--rw-r--r--   0     1001      123     2057 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/cos/writer.rs
--rw-r--r--   0     1001      123     4186 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/dashmap/backend.rs
--rw-r--r--   0     1001      123      859 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/dashmap/mod.rs
--rw-r--r--   0     1001      123    23672 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/fs/backend.rs
--rw-r--r--   0     1001      123     1424 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/fs/error.rs
--rw-r--r--   0     1001      123      884 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/fs/mod.rs
--rw-r--r--   0     1001      123     4430 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/fs/pager.rs
--rw-r--r--   0     1001      123     3092 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/fs/writer.rs
--rw-r--r--   0     1001      123    16921 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ftp/backend.rs
--rw-r--r--   0     1001      123     1808 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ftp/err.rs
--rw-r--r--   0     1001      123      894 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ftp/mod.rs
--rw-r--r--   0     1001      123     2504 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ftp/pager.rs
--rw-r--r--   0     1001      123     4208 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ftp/util.rs
--rw-r--r--   0     1001      123     1900 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ftp/writer.rs
--rw-r--r--   0     1001      123    21339 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/backend.rs
--rw-r--r--   0     1001      123    16245 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/core.rs
--rw-r--r--   0     1001      123     3512 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/error.rs
--rw-r--r--   0     1001      123      905 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/mod.rs
--rw-r--r--   0     1001      123    10592 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/pager.rs
--rw-r--r--   0     1001      123     2820 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/uri.rs
--rw-r--r--   0     1001      123     6340 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/writer.rs
--rw-r--r--   0     1001      123     3648 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/backend.rs
--rw-r--r--   0     1001      123     4276 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/builder.rs
--rw-r--r--   0     1001      123     7046 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/core.rs
--rw-r--r--   0     1001      123     1743 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/error.rs
--rw-r--r--   0     1001      123      904 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/mod.rs
--rw-r--r--   0     1001      123     1981 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/writer.rs
--rw-r--r--   0     1001      123    20887 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ghac/backend.rs
--rw-r--r--   0     1001      123     1908 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ghac/error.rs
--rw-r--r--   0     1001      123      877 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ghac/mod.rs
--rw-r--r--   0     1001      123     2375 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ghac/writer.rs
--rw-r--r--   0     1001      123    16113 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/backend.rs
--rw-r--r--   0     1001      123     1497 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/error.rs
--rw-r--r--   0     1001      123      888 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/mod.rs
--rw-r--r--   0     1001      123     3315 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/pager.rs
--rw-r--r--   0     1001      123     2461 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/writer.rs
--rw-r--r--   0     1001      123    16387 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/http/backend.rs
--rw-r--r--   0     1001      123     1875 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/http/error.rs
--rw-r--r--   0     1001      123      265 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
--rw-r--r--   0     1001      123      865 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/http/mod.rs
--rw-r--r--   0     1001      123    17104 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/backend.rs
--rw-r--r--   0     1001      123     1871 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/error.rs
--rw-r--r--   0     1001      123     8200 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
--rw-r--r--   0     1001      123      875 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/mod.rs
--rw-r--r--   0     1001      123     9272 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
--rw-r--r--   0     1001      123     3946 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
--rw-r--r--   0     1001      123     2790 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/error.rs
--rw-r--r--   0     1001      123      903 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
--rw-r--r--   0     1001      123     3819 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
--rw-r--r--   0     1001      123     1753 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
--rw-r--r--   0     1001      123     5712 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/memcached/ascii.rs
--rw-r--r--   0     1001      123     9250 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/memcached/backend.rs
--rw-r--r--   0     1001      123      875 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/memcached/mod.rs
--rw-r--r--   0     1001      123     4434 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/memory/backend.rs
--rw-r--r--   0     1001      123      857 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/memory/mod.rs
--rw-r--r--   0     1001      123     4157 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/mod.rs
--rw-r--r--   0     1001      123     8174 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/moka/backend.rs
--rw-r--r--   0     1001      123      853 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/moka/mod.rs
--rw-r--r--   0     1001      123    15197 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/obs/backend.rs
--rw-r--r--   0     1001      123     8411 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/obs/core.rs
--rw-r--r--   0     1001      123     3492 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/obs/error.rs
--rw-r--r--   0     1001      123      896 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/obs/mod.rs
--rw-r--r--   0     1001      123     6027 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/obs/pager.rs
--rw-r--r--   0     1001      123     2057 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/obs/writer.rs
--rw-r--r--   0     1001      123    14620 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/backend.rs
--rw-r--r--   0     1001      123     4177 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/builder.rs
--rw-r--r--   0     1001      123     1743 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/error.rs
--rw-r--r--   0     1001      123     9228 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/graph_model.rs
--rw-r--r--   0     1001      123      926 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/mod.rs
--rw-r--r--   0     1001      123     4874 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/pager.rs
--rw-r--r--   0     1001      123     6253 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/writer.rs
--rw-r--r--   0     1001      123     4895 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/appender.rs
--rw-r--r--   0     1001      123    23406 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/backend.rs
--rw-r--r--   0     1001      123    25647 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/core.rs
--rw-r--r--   0     1001      123     3407 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/error.rs
--rw-r--r--   0     1001      123      910 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/mod.rs
--rw-r--r--   0     1001      123     7006 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/pager.rs
--rw-r--r--   0     1001      123     6676 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/writer.rs
--rw-r--r--   0     1001      123    10722 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/redis/backend.rs
--rw-r--r--   0     1001      123      855 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/redis/mod.rs
--rw-r--r--   0     1001      123     5749 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
--rw-r--r--   0     1001      123      859 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
--rw-r--r--   0     1001      123    42100 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/backend.rs
--rw-r--r--   0     1001      123     3395 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/compatible_services.md
--rw-r--r--   0     1001      123    28632 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/core.rs
--rw-r--r--   0     1001      123     4749 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/error.rs
--rw-r--r--   0     1001      123      894 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/mod.rs
--rw-r--r--   0     1001      123     7387 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/pager.rs
--rw-r--r--   0     1001      123     7259 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/writer.rs
--rw-r--r--   0     1001      123    16772 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sftp/backend.rs
--rw-r--r--   0     1001      123     2587 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sftp/error.rs
--rw-r--r--   0     1001      123      899 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sftp/mod.rs
--rw-r--r--   0     1001      123     2420 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sftp/pager.rs
--rw-r--r--   0     1001      123     3641 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sftp/utils.rs
--rw-r--r--   0     1001      123     1519 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sftp/writer.rs
--rw-r--r--   0     1001      123     5603 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sled/backend.rs
--rw-r--r--   0     1001      123      854 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sled/mod.rs
--rw-r--r--   0     1001      123     9798 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/supabase/backend.rs
--rw-r--r--   0     1001      123     8021 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/supabase/core.rs
--rw-r--r--   0     1001      123     2582 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/supabase/error.rs
--rw-r--r--   0     1001      123      894 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/supabase/mod.rs
--rw-r--r--   0     1001      123     2382 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/supabase/writer.rs
--rw-r--r--   0     1001      123     4936 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs
--rw-r--r--   0     1001      123     3636 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs
--rw-r--r--   0     1001      123     1743 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs
--rw-r--r--   0     1001      123      912 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs
--rw-r--r--   0     1001      123     2055 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs
--rw-r--r--   0     1001      123    39360 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/backend.rs
--rw-r--r--   0     1001      123    29776 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/core.rs
--rw-r--r--   0     1001      123     3761 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/error.rs
--rw-r--r--   0     1001      123      902 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/mod.rs
--rw-r--r--   0     1001      123     7061 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/pager.rs
--rw-r--r--   0     1001      123     2050 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/writer.rs
--rw-r--r--   0     1001      123    20987 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/backend.rs
--rw-r--r--   0     1001      123     1743 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/error.rs
--rw-r--r--   0     1001      123      130 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
--rw-r--r--   0     1001      123      626 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
--rw-r--r--   0     1001      123      531 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
--rw-r--r--   0     1001      123    16965 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/list_response.rs
--rw-r--r--   0     1001      123      911 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/mod.rs
--rw-r--r--   0     1001      123     2560 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/pager.rs
--rw-r--r--   0     1001      123     2066 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/writer.rs
--rw-r--r--   0     1001      123    19875 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
--rw-r--r--   0     1001      123     4085 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/error.rs
--rw-r--r--   0     1001      123     4679 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/message.rs
--rw-r--r--   0     1001      123      907 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
--rw-r--r--   0     1001      123     2452 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
--rw-r--r--   0     1001      123     2076 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
--rw-r--r--   0     1001      123     8622 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/appender.rs
--rw-r--r--   0     1001      123     2649 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/builder.rs
--rw-r--r--   0     1001      123     6870 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/capability.rs
--rw-r--r--   0     1001      123     2494 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/entry.rs
--rw-r--r--   0     1001      123    12002 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/error.rs
--rw-r--r--   0     1001      123     7417 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/list.rs
--rw-r--r--   0     1001      123    16557 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/metadata.rs
--rw-r--r--   0     1001      123     1554 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/mod.rs
--rw-r--r--   0     1001      123     1747 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/mode.rs
--rw-r--r--   0     1001      123    24284 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
--rw-r--r--   0     1001      123    13497 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/operator/builder.rs
--rw-r--r--   0     1001      123     3073 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/operator/metadata.rs
--rw-r--r--   0     1001      123     1098 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/operator/mod.rs
--rw-r--r--   0     1001      123    48177 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/operator/operator.rs
--rw-r--r--   0     1001      123    12114 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/ops.rs
--rw-r--r--   0     1001      123     9571 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/reader.rs
--rw-r--r--   0     1001      123     6741 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/scheme.rs
--rw-r--r--   0     1001      123    10795 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/writer.rs
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 opendal-0.35.0/Cargo.toml
--rw-r--r--   0     1001      123      709 2023-05-23 08:09:35.000000 opendal-0.35.0/.gitignore
--rw-r--r--   0     1001      123     2212 2023-05-23 08:09:35.000000 opendal-0.35.0/CONTRIBUTING.md
--rw-r--r--   0     1001      123      982 2023-05-23 08:09:35.000000 opendal-0.35.0/README.md
--rw-r--r--   0     1001      123      765 2023-05-23 08:09:35.000000 opendal-0.35.0/benchmark/README.md
--rw-r--r--   0     1001      123     2426 2023-05-23 08:09:35.000000 opendal-0.35.0/benchmark/async_opendal_benchmark.py
--rw-r--r--   0     1001      123     2955 2023-05-23 08:09:35.000000 opendal-0.35.0/benchmark/async_origin_s3_benchmark_with_gevent.py
--rw-r--r--   0     1001      123      917 2023-05-23 08:09:35.000000 opendal-0.35.0/examples/object.ipynb
--rw-r--r--   0     1001      123     1665 2023-05-23 08:09:35.000000 opendal-0.35.0/pyproject.toml
--rw-r--r--   0     1001      123      866 2023-05-23 08:09:35.000000 opendal-0.35.0/python/opendal/__init__.py
--rw-r--r--   0     1001      123     2917 2023-05-23 08:09:35.000000 opendal-0.35.0/python/opendal/__init__.pyi
--rw-r--r--   0     1001      123      405 2023-05-23 08:09:35.000000 opendal-0.35.0/python/opendal/layers.pyi
--rw-r--r--   0     1001      123    11963 2023-05-23 08:09:35.000000 opendal-0.35.0/src/asyncio.rs
--rw-r--r--   0     1001      123     3074 2023-05-23 08:09:35.000000 opendal-0.35.0/src/layers.rs
--rw-r--r--   0     1001      123    12218 2023-05-23 08:09:35.000000 opendal-0.35.0/src/lib.rs
--rw-r--r--   0     1001      123     1604 2023-05-23 08:09:35.000000 opendal-0.35.0/tests/binding.feature
--rw-r--r--   0     1001      123     2942 2023-05-23 08:09:35.000000 opendal-0.35.0/tests/steps/binding.py
--rw-r--r--   0     1001      123   131969 2023-05-23 08:09:35.000000 opendal-0.35.0/Cargo.lock
--rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 opendal-0.35.0/PKG-INFO
+-rw-r--r--   0        0        0     6291 1970-01-01 00:00:00.000000 opendal-0.36.1/local_dependencies/opendal/Cargo.toml
+-rw-r--r--   0     1001      123    78200 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/CHANGELOG.md
+-rw-r--r--   0     1001      123     1114 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     6804 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/README.md
+-rw-r--r--   0     1001      123      378 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/benches/README.md
+-rw-r--r--   0     1001      123      672 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/benches/ops/README.md
+-rw-r--r--   0     1001      123      979 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/benches/ops/main.rs
+-rw-r--r--   0     1001      123     5574 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/benches/ops/read.rs
+-rw-r--r--   0     1001      123     2792 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/benches/ops/utils.rs
+-rw-r--r--   0     1001      123     2163 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/benches/ops/write.rs
+-rw-r--r--   0     1001      123     1827 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/examples/object.rs
+-rw-r--r--   0     1001      123     1290 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/comparisons/mod.rs
+-rw-r--r--   0     1001      123     7682 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
+-rw-r--r--   0     1001      123     6142 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/concepts.rs
+-rw-r--r--   0     1001      123      982 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/features.md
+-rw-r--r--   0     1001      123    10879 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/internals/accessor.rs
+-rw-r--r--   0     1001      123     1765 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/internals/layer.rs
+-rw-r--r--   0     1001      123     3409 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/internals/mod.rs
+-rw-r--r--   0     1001      123     1458 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3436 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md
+-rw-r--r--   0     1001      123     5329 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
+-rw-r--r--   0     1001      123     4885 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
+-rw-r--r--   0     1001      123     5428 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
+-rw-r--r--   0     1001      123     3341 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
+-rw-r--r--   0     1001      123     4425 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
+-rw-r--r--   0     1001      123     2902 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
+-rw-r--r--   0     1001      123    12349 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
+-rw-r--r--   0     1001      123     2538 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
+-rw-r--r--   0     1001      123     2347 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
+-rw-r--r--   0     1001      123     2805 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
+-rw-r--r--   0     1001      123     1803 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
+-rw-r--r--   0     1001      123     4733 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
+-rw-r--r--   0     1001      123     2184 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
+-rw-r--r--   0     1001      123     5771 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
+-rw-r--r--   0     1001      123     8563 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
+-rw-r--r--   0     1001      123     3113 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
+-rw-r--r--   0     1001      123     4321 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
+-rw-r--r--   0     1001      123     1881 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
+-rw-r--r--   0     1001      123     2926 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
+-rw-r--r--   0     1001      123     2246 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
+-rw-r--r--   0     1001      123     6523 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
+-rw-r--r--   0     1001      123     4792 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
+-rw-r--r--   0     1001      123    10091 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
+-rw-r--r--   0     1001      123     2508 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
+-rw-r--r--   0     1001      123     2670 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
+-rw-r--r--   0     1001      123     8059 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
+-rw-r--r--   0     1001      123     2472 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
+-rw-r--r--   0     1001      123     4452 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
+-rw-r--r--   0     1001      123     2534 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
+-rw-r--r--   0     1001      123     3693 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
+-rw-r--r--   0     1001      123     3255 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
+-rw-r--r--   0     1001      123     4133 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
+-rw-r--r--   0     1001      123     4408 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
+-rw-r--r--   0     1001      123     4230 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
+-rw-r--r--   0     1001      123     3172 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
+-rw-r--r--   0     1001      123     2687 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md
+-rw-r--r--   0     1001      123     2576 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md
+-rw-r--r--   0     1001      123     4658 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/mod.rs
+-rw-r--r--   0     1001      123    25915 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/docs/upgrade.md
+-rw-r--r--   0     1001      123     6622 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/chaos.rs
+-rw-r--r--   0     1001      123    22150 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/complete.rs
+-rw-r--r--   0     1001      123     9829 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/concurrent_limit.rs
+-rw-r--r--   0     1001      123    17421 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/error_context.rs
+-rw-r--r--   0     1001      123    14214 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/immutable_index.rs
+-rw-r--r--   0     1001      123    52907 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/logging.rs
+-rw-r--r--   0     1001      123    13282 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/madsim.rs
+-rw-r--r--   0     1001      123    29688 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/metrics.rs
+-rw-r--r--   0     1001      123    12370 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/minitrace.rs
+-rw-r--r--   0     1001      123     2250 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/mod.rs
+-rw-r--r--   0     1001      123    13102 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/oteltrace.rs
+-rw-r--r--   0     1001      123    23050 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/prometheus.rs
+-rw-r--r--   0     1001      123    38366 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/retry.rs
+-rw-r--r--   0     1001      123    13680 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/timeout.rs
+-rw-r--r--   0     1001      123    11978 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/tracing.rs
+-rw-r--r--   0     1001      123     3644 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/layers/type_eraser.rs
+-rw-r--r--   0     1001      123     3570 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/lib.rs
+-rw-r--r--   0     1001      123    18865 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/accessor.rs
+-rw-r--r--   0     1001      123     5049 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs
+-rw-r--r--   0     1001      123    10363 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
+-rw-r--r--   0     1001      123     1020 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
+-rw-r--r--   0     1001      123     1566 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/mod.rs
+-rw-r--r--   0     1001      123     5407 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs
+-rw-r--r--   0     1001      123    10349 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs
+-rw-r--r--   0     1001      123     1067 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs
+-rw-r--r--   0     1001      123     1934 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/chrono_util.rs
+-rw-r--r--   0     1001      123     5973 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/body.rs
+-rw-r--r--   0     1001      123    10135 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
+-rw-r--r--   0     1001      123    10534 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
+-rw-r--r--   0     1001      123     5282 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/client.rs
+-rw-r--r--   0     1001      123     3415 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/error.rs
+-rw-r--r--   0     1001      123    11165 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/header.rs
+-rw-r--r--   0     1001      123     2159 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/mod.rs
+-rw-r--r--   0     1001      123    22541 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/multipart.rs
+-rw-r--r--   0     1001      123     2962 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/uri.rs
+-rw-r--r--   0     1001      123    11712 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/layer.rs
+-rw-r--r--   0     1001      123     1976 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/mod.rs
+-rw-r--r--   0     1001      123     3018 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/append.rs
+-rw-r--r--   0     1001      123     9434 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/cursor.rs
+-rw-r--r--   0     1001      123     2512 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/entry.rs
+-rw-r--r--   0     1001      123     3666 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1006 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
+-rw-r--r--   0     1001      123    15408 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
+-rw-r--r--   0     1001      123     4150 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1686 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
+-rw-r--r--   0     1001      123     4579 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs
+-rw-r--r--   0     1001      123     2097 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/mod.rs
+-rw-r--r--   0     1001      123     3516 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/page.rs
+-rw-r--r--   0     1001      123    10670 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/read.rs
+-rw-r--r--   0     1001      123     9158 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
+-rw-r--r--   0     1001      123     6894 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
+-rw-r--r--   0     1001      123     5206 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/oio/write.rs
+-rw-r--r--   0     1001      123     3953 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/operation.rs
+-rw-r--r--   0     1001      123    12115 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/ops.rs
+-rw-r--r--   0     1001      123    11671 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/path.rs
+-rw-r--r--   0     1001      123     6507 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/rps.rs
+-rw-r--r--   0     1001      123     1396 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/serde_util.rs
+-rw-r--r--   0     1001      123     1077 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/raw/version.rs
+-rw-r--r--   0     1001      123     4514 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azblob/appender.rs
+-rw-r--r--   0     1001      123    31443 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azblob/backend.rs
+-rw-r--r--   0     1001      123     5544 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azblob/batch.rs
+-rw-r--r--   0     1001      123    16950 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azblob/core.rs
+-rw-r--r--   0     1001      123     2304 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azblob/docs.md
+-rw-r--r--   0     1001      123     5870 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azblob/error.rs
+-rw-r--r--   0     1001      123      927 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azblob/mod.rs
+-rw-r--r--   0     1001      123    14196 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azblob/pager.rs
+-rw-r--r--   0     1001      123     2054 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azblob/writer.rs
+-rw-r--r--   0     1001      123    14348 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/backend.rs
+-rw-r--r--   0     1001      123    10123 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/core.rs
+-rw-r--r--   0     1001      123     1960 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/docs.md
+-rw-r--r--   0     1001      123     3519 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/error.rs
+-rw-r--r--   0     1001      123      900 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/mod.rs
+-rw-r--r--   0     1001      123     5647 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/pager.rs
+-rw-r--r--   0     1001      123     2711 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/writer.rs
+-rw-r--r--   0     1001      123     5727 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/cos/appender.rs
+-rw-r--r--   0     1001      123    13653 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/cos/backend.rs
+-rw-r--r--   0     1001      123     9184 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/cos/core.rs
+-rw-r--r--   0     1001      123     1314 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/cos/docs.md
+-rw-r--r--   0     1001      123     3492 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/cos/error.rs
+-rw-r--r--   0     1001      123      910 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/cos/mod.rs
+-rw-r--r--   0     1001      123     5963 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/cos/pager.rs
+-rw-r--r--   0     1001      123     2032 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/cos/writer.rs
+-rw-r--r--   0     1001      123     3972 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/dashmap/backend.rs
+-rw-r--r--   0     1001      123      186 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/dashmap/docs.md
+-rw-r--r--   0     1001      123      859 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/dashmap/mod.rs
+-rw-r--r--   0     1001      123     1409 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/fs/appender.rs
+-rw-r--r--   0     1001      123    23158 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/fs/backend.rs
+-rw-r--r--   0     1001      123      869 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/fs/docs.md
+-rw-r--r--   0     1001      123     1424 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/fs/error.rs
+-rw-r--r--   0     1001      123      898 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/fs/mod.rs
+-rw-r--r--   0     1001      123     4430 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/fs/pager.rs
+-rw-r--r--   0     1001      123     3092 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/fs/writer.rs
+-rw-r--r--   0     1001      123    15925 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ftp/backend.rs
+-rw-r--r--   0     1001      123      737 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ftp/docs.md
+-rw-r--r--   0     1001      123     1808 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ftp/err.rs
+-rw-r--r--   0     1001      123      894 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ftp/mod.rs
+-rw-r--r--   0     1001      123     2504 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ftp/pager.rs
+-rw-r--r--   0     1001      123     4208 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ftp/util.rs
+-rw-r--r--   0     1001      123     1900 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ftp/writer.rs
+-rw-r--r--   0     1001      123    21320 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gcs/backend.rs
+-rw-r--r--   0     1001      123    16245 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gcs/core.rs
+-rw-r--r--   0     1001      123     3512 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gcs/error.rs
+-rw-r--r--   0     1001      123      905 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gcs/mod.rs
+-rw-r--r--   0     1001      123    10592 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gcs/pager.rs
+-rw-r--r--   0     1001      123     2820 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gcs/uri.rs
+-rw-r--r--   0     1001      123     6315 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gcs/writer.rs
+-rw-r--r--   0     1001      123     3361 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gdrive/backend.rs
+-rw-r--r--   0     1001      123     4276 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gdrive/builder.rs
+-rw-r--r--   0     1001      123     7046 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gdrive/core.rs
+-rw-r--r--   0     1001      123     1743 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gdrive/error.rs
+-rw-r--r--   0     1001      123      904 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gdrive/mod.rs
+-rw-r--r--   0     1001      123     1956 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/gdrive/writer.rs
+-rw-r--r--   0     1001      123    20868 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ghac/backend.rs
+-rw-r--r--   0     1001      123     1908 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ghac/error.rs
+-rw-r--r--   0     1001      123      877 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ghac/mod.rs
+-rw-r--r--   0     1001      123     2375 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ghac/writer.rs
+-rw-r--r--   0     1001      123    13212 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/hdfs/backend.rs
+-rw-r--r--   0     1001      123     2419 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/hdfs/docs.md
+-rw-r--r--   0     1001      123     1497 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/hdfs/error.rs
+-rw-r--r--   0     1001      123      888 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/hdfs/mod.rs
+-rw-r--r--   0     1001      123     3315 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/hdfs/pager.rs
+-rw-r--r--   0     1001      123     2461 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/hdfs/writer.rs
+-rw-r--r--   0     1001      123    16276 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/http/backend.rs
+-rw-r--r--   0     1001      123     1875 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/http/error.rs
+-rw-r--r--   0     1001      123      265 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      865 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/http/mod.rs
+-rw-r--r--   0     1001      123    15935 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ipfs/backend.rs
+-rw-r--r--   0     1001      123      867 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ipfs/docs.md
+-rw-r--r--   0     1001      123     1871 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ipfs/error.rs
+-rw-r--r--   0     1001      123     8200 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ipfs/ipld.rs
+-rw-r--r--   0     1001      123      875 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ipfs/mod.rs
+-rw-r--r--   0     1001      123     9253 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ipmfs/backend.rs
+-rw-r--r--   0     1001      123     3946 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ipmfs/builder.rs
+-rw-r--r--   0     1001      123     2790 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ipmfs/error.rs
+-rw-r--r--   0     1001      123      903 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ipmfs/mod.rs
+-rw-r--r--   0     1001      123     3819 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ipmfs/pager.rs
+-rw-r--r--   0     1001      123     1753 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/ipmfs/writer.rs
+-rw-r--r--   0     1001      123     5712 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/memcached/ascii.rs
+-rw-r--r--   0     1001      123     9177 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/memcached/backend.rs
+-rw-r--r--   0     1001      123      875 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/memcached/mod.rs
+-rw-r--r--   0     1001      123     4224 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/memory/backend.rs
+-rw-r--r--   0     1001      123      511 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/memory/docs.md
+-rw-r--r--   0     1001      123      857 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/memory/mod.rs
+-rw-r--r--   0     1001      123     4157 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/mod.rs
+-rw-r--r--   0     1001      123     8174 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/moka/backend.rs
+-rw-r--r--   0     1001      123      853 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/moka/mod.rs
+-rw-r--r--   0     1001      123    15178 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/obs/backend.rs
+-rw-r--r--   0     1001      123     8411 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/obs/core.rs
+-rw-r--r--   0     1001      123     3492 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/obs/error.rs
+-rw-r--r--   0     1001      123      896 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/obs/mod.rs
+-rw-r--r--   0     1001      123     6027 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/obs/pager.rs
+-rw-r--r--   0     1001      123     2032 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/obs/writer.rs
+-rw-r--r--   0     1001      123    12487 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/backend.rs
+-rw-r--r--   0     1001      123     4177 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/builder.rs
+-rw-r--r--   0     1001      123     1743 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/error.rs
+-rw-r--r--   0     1001      123     9228 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/graph_model.rs
+-rw-r--r--   0     1001      123      926 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/mod.rs
+-rw-r--r--   0     1001      123     4874 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/pager.rs
+-rw-r--r--   0     1001      123     6228 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/writer.rs
+-rw-r--r--   0     1001      123     4869 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/oss/appender.rs
+-rw-r--r--   0     1001      123    23404 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/oss/backend.rs
+-rw-r--r--   0     1001      123    25281 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/oss/core.rs
+-rw-r--r--   0     1001      123     3407 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/oss/error.rs
+-rw-r--r--   0     1001      123      910 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/oss/mod.rs
+-rw-r--r--   0     1001      123     7006 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/oss/pager.rs
+-rw-r--r--   0     1001      123     6651 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/oss/writer.rs
+-rw-r--r--   0     1001      123     9662 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/redis/backend.rs
+-rw-r--r--   0     1001      123      856 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/redis/docs.md
+-rw-r--r--   0     1001      123      855 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/redis/mod.rs
+-rw-r--r--   0     1001      123     4245 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/rocksdb/backend.rs
+-rw-r--r--   0     1001      123     1263 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/rocksdb/docs.md
+-rw-r--r--   0     1001      123      859 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/rocksdb/mod.rs
+-rw-r--r--   0     1001      123    35297 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/s3/backend.rs
+-rw-r--r--   0     1001      123     3427 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/s3/compatible_services.md
+-rw-r--r--   0     1001      123    28632 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/s3/core.rs
+-rw-r--r--   0     1001      123     7050 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/s3/docs.md
+-rw-r--r--   0     1001      123     4749 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/s3/error.rs
+-rw-r--r--   0     1001      123      894 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/s3/mod.rs
+-rw-r--r--   0     1001      123     7387 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/s3/pager.rs
+-rw-r--r--   0     1001      123     7234 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/s3/writer.rs
+-rw-r--r--   0     1001      123    16103 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/sftp/backend.rs
+-rw-r--r--   0     1001      123     1029 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/sftp/docs.md
+-rw-r--r--   0     1001      123     2587 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/sftp/error.rs
+-rw-r--r--   0     1001      123      899 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/sftp/mod.rs
+-rw-r--r--   0     1001      123     2420 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/sftp/pager.rs
+-rw-r--r--   0     1001      123     3641 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/sftp/utils.rs
+-rw-r--r--   0     1001      123     1760 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/sftp/writer.rs
+-rw-r--r--   0     1001      123     4846 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/sled/backend.rs
+-rw-r--r--   0     1001      123      642 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/sled/docs.md
+-rw-r--r--   0     1001      123      854 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/sled/mod.rs
+-rw-r--r--   0     1001      123     9779 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/supabase/backend.rs
+-rw-r--r--   0     1001      123     8021 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/supabase/core.rs
+-rw-r--r--   0     1001      123     2761 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/supabase/error.rs
+-rw-r--r--   0     1001      123      894 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/supabase/mod.rs
+-rw-r--r--   0     1001      123     2357 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/supabase/writer.rs
+-rw-r--r--   0     1001      123     4558 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs
+-rw-r--r--   0     1001      123     3636 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs
+-rw-r--r--   0     1001      123     1743 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/vercel_artifacts/error.rs
+-rw-r--r--   0     1001      123      912 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs
+-rw-r--r--   0     1001      123     2030 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs
+-rw-r--r--   0     1001      123    39341 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/wasabi/backend.rs
+-rw-r--r--   0     1001      123    29752 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/wasabi/core.rs
+-rw-r--r--   0     1001      123     3761 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/wasabi/error.rs
+-rw-r--r--   0     1001      123      902 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/wasabi/mod.rs
+-rw-r--r--   0     1001      123     7061 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/wasabi/pager.rs
+-rw-r--r--   0     1001      123     2025 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/wasabi/writer.rs
+-rw-r--r--   0     1001      123    20966 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webdav/backend.rs
+-rw-r--r--   0     1001      123     1743 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webdav/error.rs
+-rw-r--r--   0     1001      123      130 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
+-rw-r--r--   0     1001      123      626 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
+-rw-r--r--   0     1001      123      990 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
+-rw-r--r--   0     1001      123    16965 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webdav/list_response.rs
+-rw-r--r--   0     1001      123      911 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webdav/mod.rs
+-rw-r--r--   0     1001      123     2560 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webdav/pager.rs
+-rw-r--r--   0     1001      123     2041 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webdav/writer.rs
+-rw-r--r--   0     1001      123    16176 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/backend.rs
+-rw-r--r--   0     1001      123     1864 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/docs.md
+-rw-r--r--   0     1001      123     4085 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/error.rs
+-rw-r--r--   0     1001      123     4679 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/message.rs
+-rw-r--r--   0     1001      123      907 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/mod.rs
+-rw-r--r--   0     1001      123     2452 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/pager.rs
+-rw-r--r--   0     1001      123     2051 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/writer.rs
+-rw-r--r--   0     1001      123     8596 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/appender.rs
+-rw-r--r--   0     1001      123     2649 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/builder.rs
+-rw-r--r--   0     1001      123     6870 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/capability.rs
+-rw-r--r--   0     1001      123     2494 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/entry.rs
+-rw-r--r--   0     1001      123    12002 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/error.rs
+-rw-r--r--   0     1001      123     7417 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/list.rs
+-rw-r--r--   0     1001      123    16556 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/metadata.rs
+-rw-r--r--   0     1001      123     1614 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/mod.rs
+-rw-r--r--   0     1001      123     1747 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/mode.rs
+-rw-r--r--   0     1001      123    24401 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs
+-rw-r--r--   0     1001      123    13497 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/operator/builder.rs
+-rw-r--r--   0     1001      123     3073 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/operator/metadata.rs
+-rw-r--r--   0     1001      123     1153 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/operator/mod.rs
+-rw-r--r--   0     1001      123    49497 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/operator/operator.rs
+-rw-r--r--   0     1001      123     2863 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/operator/operator_functions.rs
+-rw-r--r--   0     1001      123    17117 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/operator/operator_futures.rs
+-rw-r--r--   0     1001      123     9547 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/reader.rs
+-rw-r--r--   0     1001      123     6741 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/scheme.rs
+-rw-r--r--   0     1001      123    10770 2023-06-02 11:16:18.000000 opendal-0.36.1/local_dependencies/opendal/src/types/writer.rs
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 opendal-0.36.1/Cargo.toml
+-rw-r--r--   0     1001      123      709 2023-06-02 11:16:18.000000 opendal-0.36.1/.gitignore
+-rw-r--r--   0     1001      123     2212 2023-06-02 11:16:18.000000 opendal-0.36.1/CONTRIBUTING.md
+-rw-r--r--   0     1001      123      982 2023-06-02 11:16:18.000000 opendal-0.36.1/README.md
+-rw-r--r--   0     1001      123      765 2023-06-02 11:16:18.000000 opendal-0.36.1/benchmark/README.md
+-rw-r--r--   0     1001      123     2426 2023-06-02 11:16:18.000000 opendal-0.36.1/benchmark/async_opendal_benchmark.py
+-rw-r--r--   0     1001      123     2955 2023-06-02 11:16:18.000000 opendal-0.36.1/benchmark/async_origin_s3_benchmark_with_gevent.py
+-rw-r--r--   0     1001      123      917 2023-06-02 11:16:18.000000 opendal-0.36.1/examples/object.ipynb
+-rw-r--r--   0     1001      123     1660 2023-06-02 11:16:18.000000 opendal-0.36.1/pyproject.toml
+-rw-r--r--   0     1001      123      866 2023-06-02 11:16:18.000000 opendal-0.36.1/python/opendal/__init__.py
+-rw-r--r--   0     1001      123     2917 2023-06-02 11:16:18.000000 opendal-0.36.1/python/opendal/__init__.pyi
+-rw-r--r--   0     1001      123      405 2023-06-02 11:16:18.000000 opendal-0.36.1/python/opendal/layers.pyi
+-rw-r--r--   0     1001      123    11963 2023-06-02 11:16:18.000000 opendal-0.36.1/src/asyncio.rs
+-rw-r--r--   0     1001      123     3074 2023-06-02 11:16:18.000000 opendal-0.36.1/src/layers.rs
+-rw-r--r--   0     1001      123    12218 2023-06-02 11:16:18.000000 opendal-0.36.1/src/lib.rs
+-rw-r--r--   0     1001      123     1604 2023-06-02 11:16:18.000000 opendal-0.36.1/tests/binding.feature
+-rw-r--r--   0     1001      123     2942 2023-06-02 11:16:18.000000 opendal-0.36.1/tests/steps/binding.py
+-rw-r--r--   0     1001      123   132202 2023-06-02 11:16:18.000000 opendal-0.36.1/Cargo.lock
+-rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 opendal-0.36.1/PKG-INFO
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/Cargo.toml` & `opendal-0.36.1/local_dependencies/opendal/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.65"
-version= "0.35.0"
+version= "0.36.1"
 
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
 default = [
   "rustls",
@@ -88,14 +88,15 @@
 layers-minitrace = ["dep:minitrace"]
 # Enable layers tracing support.
 layers-tracing = ["dep:tracing"]
 # Enable layers oteltrace support.
 layers-otel-trace = ["dep:opentelemetry"]
 
 services-azblob = [
+  "dep:sha2",
   "dep:reqsign",
   "reqsign?/services-azblob",
   "reqsign?/reqwest_request",
 ]
 services-azdfs = [
   "dep:reqsign",
   "reqsign?/services-azblob",
@@ -198,21 +199,22 @@
 prost = { version = "0.11", optional = true }
 quick-xml = { version = "0.27", features = ["serialize", "overlapped-lists"] }
 rand = { version = "0.8", optional = true }
 redis = { version = "0.22", features = [
   "tokio-comp",
   "connection-manager",
 ], optional = true }
-reqsign = { version = "0.12.0", default-features = false, optional = true }
-reqwest = { version = "0.11.13", features = [
+reqsign = { version = "0.13.0", default-features = false, optional = true }
+reqwest = { version = "0.11.18", features = [
   "stream",
 ], default-features = false }
-rocksdb = { version = "0.20.1", default-features = false, optional = true }
+rocksdb = { version = "0.21.0", default-features = false, optional = true }
 serde = { version = "1", features = ["derive"] }
 serde_json = "1"
+sha2 = { version = "0.10", optional = true }
 sled = { version = "0.34.7", optional = true }
 suppaftp = { version = "4.5", default-features = false, features = [
   "async-secure",
   "async-rustls",
 ], optional = true }
 tokio = "1.27"
 tracing = { version = "0.1", optional = true }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/CHANGELOG.md` & `opendal-0.36.1/local_dependencies/opendal/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,125 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
+## [v0.36.1] - 2023-06-02
+
+### Added
+- feat(services/webdav): support redirection when get 302/307 response during read operation by @Yansongsongsong in https://github.com/apache/incubator-opendal/pull/2256
+- feat: Add Zig Bindings Module by @kassane in https://github.com/apache/incubator-opendal/pull/2374
+- feat: Implement Timeout Layer by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2395
+
+### Changed
+- refactor(bindings/zig): enable tests and more by @tisonkun in https://github.com/apache/incubator-opendal/pull/2375
+- refactor(bindings/zig): add errors handler and module test by @kassane in https://github.com/apache/incubator-opendal/pull/2381
+- refactor(http_util): Adopt reqwest's redirect support by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2390
+
+### Fixed
+- fix(bindings/zig): reflect C interface changes by @tisonkun in https://github.com/apache/incubator-opendal/pull/2378
+- fix(services/azblob): Fix batch delete doesn't work on azure by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2382
+
+### Docs
+- docs: service doc for s3 by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2376
+- docs(bindings/C): The documentation for OpenDAL C binding by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2373
+- docs: add link for c binding by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2380
+- docs: docs for kv services by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2396
+- docs: docs for fs related services by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2397
+- docs(bindings/java): do not release snapshot versions anymore by @tisonkun in https://github.com/apache/incubator-opendal/pull/2398
+
+### CI
+- ci: Enable semantic PRs by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2370
+- ci: improve licenserc settings by @tisonkun in https://github.com/apache/incubator-opendal/pull/2377
+- build(deps): bump reqwest from 0.11.15 to 0.11.18 by @dependabot in https://github.com/apache/incubator-opendal/pull/2389
+- build(deps): bump pyo3 from 0.18.2 to 0.18.3 by @dependabot in https://github.com/apache/incubator-opendal/pull/2388
+- ci: Enable nextest for all behavior tests by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2400
+
+### Chore
+- chore(bindings/python): upgrade maturin to 1.0 by @messense in https://github.com/apache/incubator-opendal/pull/2369
+- chore: Fix license headers for release/labler by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2371
+
+## [v0.36.0] - 2023-05-30
+
+### Added
+
+- feat(service/fs): add append support for fs (#2296)
+- feat(services/sftp): add append support for sftp (#2297)
+- RFC-2299: Chain based Operator API (#2299)
+- feat(services/azblob): add append support (#2302)
+- feat(bindings/nodejs): add append support (#2322)
+- feat(bindings/C): opendal_operator_ptr construction using kvs (#2329)
+- feat(services/cos): append support (#2332)
+- feat(bindings/java): implement Operator#delete (#2345)
+- feat(bindings/java): support append (#2350)
+- feat(bindings/java): save one jni call in the hot path (#2353)
+- feat: server side encryption support for azblob (#2347)
+
+### Changed
+
+- refactor(core): Implement RFC-2299 for stat_with (#2303)
+- refactor(core): Implement RFC-2299 for BlockingOperator::write_with (#2305)
+- refactor(core): Implement RFC-2299 for appender_with (#2307)
+- refactor(core): Implement RFC-2299 for read_with (#2308)
+- refactor(core): Implement RFC-2299 for read_with (#2308)
+- refactor(core): Implement RFC-2299 for append_with (#2312)
+- refactor(core): Implement RFC-2299 for write_with (#2315)
+- refactor(core): Implement RFC-2299 for reader_with (#2316)
+- refactor(core): Implement RFC-2299 for writer_with (#2317)
+- refactor(core): Implement RFC-2299 for presign_read_with (#2314)
+- refactor(core): Implement RFC-2299 for presign_write_with (#2320)
+- refactor(core): Implement RFC-2299 for list_with (#2323)
+- refactor: Move `ops` to `raw::ops` (#2325)
+- refactor(bindings/C): align bdd test with the feature tests (#2340)
+- refactor(bindings/java): narrow unsafe boundary (#2351)
+
+### Fixed
+
+- fix(services/supabase): correctly set retryable (#2295)
+- fix(core): appender complete check (#2298)
+
+### Docs
+
+- docs: add service doc for azdfs (#2310)
+- docs(bidnings/java): how to deploy snapshots (#2311)
+- docs(bidnings/java): how to deploy snapshots (#2311)
+- docs: Fixed links of languages to open in same tab (#2327)
+- docs: Adopt docusaurus pathname protocol (#2330)
+- docs(bindings/nodejs): update lib desc (#2331)
+- docs(bindings/java): update the README file (#2338)
+- docs: add service doc for fs (#2337)
+- docs: add service doc for cos (#2341)
+- docs: add service doc for dashmap (#2342)
+- docs(bindings/java): for BlockingOperator (#2344)
+
+### CI
+
+- build(bindings/java): prepare for snapshot release (#2301)
+- build(bindings/java): support multiple platform java bindings  (#2324)
+- ci(binding/nodejs): Use docker to build nodejs binding (#2328)
+- build(bindings/java): prepare for automatically multiple platform deploy (#2335)
+- ci: add bindings java docs and integrate with website (#2346)
+- ci: avoid copy gitignore to site folder (#2348)
+- ci(bindings/c): Add diff check (#2359)
+- ci: Cache librocksdb to speed up CI (#2360)
+- ci: Don't load rocksdb for all workflows (#2362)
+- ci: Fix Node.js 12 actions deprecated warning (#2363)
+- ci: Speed up python docs build (#2364)
+- ci: Adopt setup-node's cache logic instead (#2365)
+
+### Chore
+
+- chore(test): Avoid test names becoming prefixes of other tests (#2333)
+- chore(bindings/java): improve OpenDALException tests and docs (#2343)
+- chore(bindings/java): post release 0.1.0 (#2352)
+- chore(docs): split docs build into small jobs (#2356)'
+- chore: protect branch gh-pages (#2358)
+
 ## [v0.35.0] - 2023-05-23
 
 ### Added
 
 - feat(services/onedrive): Implement `list`, `create_dir`, `stat` and upload
 ing large files (#2231)
 - feat(bindings/C): Initially support stat in C binding (#2249)
@@ -2156,14 +2267,16 @@
 
 ## v0.0.1 - 2022-02-14
 
 ### Added
 
 Hello, OpenDAL!
 
+[v0.36.1]: https://github.com/apache/incubator-opendal/compare/v0.36.0...v0.36.1
+[v0.36.0]: https://github.com/apache/incubator-opendal/compare/v0.35.0...v0.36.0
 [v0.35.0]: https://github.com/apache/incubator-opendal/compare/v0.34.0...v0.35.0
 [v0.34.0]: https://github.com/apache/incubator-opendal/compare/v0.33.3...v0.34.0
 [v0.33.3]: https://github.com/apache/incubator-opendal/compare/v0.33.2...v0.33.3
 [v0.33.2]: https://github.com/apache/incubator-opendal/compare/v0.33.1...v0.33.2
 [v0.33.1]: https://github.com/apache/incubator-opendal/compare/v0.33.0...v0.33.1
 [v0.33.0]: https://github.com/apache/incubator-opendal/compare/v0.32.0...v0.33.0
 [v0.32.0]: https://github.com/apache/incubator-opendal/compare/v0.31.1...v0.32.0
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/CONTRIBUTING.md` & `opendal-0.36.1/local_dependencies/opendal/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/README.md` & `opendal-0.36.1/local_dependencies/opendal/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/benches/ops/README.md` & `opendal-0.36.1/local_dependencies/opendal/benches/ops/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/benches/ops/main.rs` & `opendal-0.36.1/local_dependencies/opendal/benches/ops/main.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/benches/ops/read.rs` & `opendal-0.36.1/local_dependencies/opendal/benches/ops/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/benches/ops/utils.rs` & `opendal-0.36.1/local_dependencies/opendal/benches/ops/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/benches/ops/write.rs` & `opendal-0.36.1/local_dependencies/opendal/benches/ops/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/examples/object.rs` & `opendal-0.36.1/local_dependencies/opendal/examples/object.rs`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 use log::info;
 use opendal::layers::LoggingLayer;
 use opendal::services;
 use opendal::Operator;
 use opendal::Result;
 
 /// Visit [`opendal::services`] for more service related config.
-/// Visit [`opendal::Object`] for more object level APIs.
+/// Visit [`opendal::Operator`] for more operator level APIs.
 #[tokio::main]
 async fn main() -> Result<()> {
     let _ = tracing_subscriber::fmt()
         .with_env_filter("debug")
         .try_init();
 
     // Pick a builder and configure it.
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/comparisons/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/docs/comparisons/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/concepts.rs` & `opendal-0.36.1/local_dependencies/opendal/src/docs/concepts.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/features.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/features.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/internals/accessor.rs` & `opendal-0.36.1/local_dependencies/opendal/src/docs/internals/accessor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/internals/layer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/docs/internals/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/internals/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/docs/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/docs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/docs/rfcs/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -135,7 +135,10 @@
 pub mod rfc_1735_operation_extension {}
 
 #[doc = include_str!("2083_writer_sink_api.md")]
 pub mod rfc_2083_writer_sink_api {}
 
 #[doc = include_str!("2133_append_api.md")]
 pub mod rfc_2133_append_api {}
+
+#[doc = include_str!("2299_chain_based_operator_api.md")]
+pub mod rfc_2299_chain_based_operator_api {}
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/docs/upgrade.md` & `opendal-0.36.1/local_dependencies/opendal/src/docs/upgrade.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,59 @@
+# Upgrade to v0.36
+
+## Public API
+
+In v0.36, OpenDAL improving the `xxx_with` API by allow it to be called in chain:
+
+After this change, all `xxx_with` alike call will be changed from
+
+```rust
+let bs = op.read_with(
+  "path/to/file",
+  OpRead::new()
+    .with_range(0..=1024)
+    .with_if_match("<etag>")
+    .with_if_none_match("<etag>")
+    .with_override_cache_control("<cache_control>")
+    .with_override_content_disposition("<content_disposition>")
+  ).await?;
+```
+
+to
+
+```rust
+let bs = op.read_with("path/to/file")
+  .range(0..=1024)
+  .if_match("<etag>")
+  .if_none_match("<etag>")
+  .override_cache_control("<cache_control>")
+  .override_content_disposition("<content_disposition>")
+  .await?;
+```
+
+For blocking API calls, we will need a `call()` at the end:
+
+```rust
+let bs = bop.read_with("path/to/file")
+  .range(0..=1024)
+  .if_match("<etag>")
+  .if_none_match("<etag>")
+  .override_cache_control("<cache_control>")
+  .override_content_disposition("<content_disposition>")
+  .call()?;
+```
+
+Along with this change, users don't need to call `OpXxx` anymore so we moved it to `raw` API.
+
+More detailes could be found at [RFC: Chain Based Operator API][crate::docs::rfcs::rfc_2299_chain_based_operator_api].
+
+## Raw API
+
+Migrated `opendal::ops` to `opendal::raw::ops`.
+
 # Upgrade to v0.35
 
 ## Public API
 
 - OpenDAL removes rarely used `Operator::from_env` and `Operator::from_iter` APIs
   - Users can use `Operator::via_map` instead.
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/chaos.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/chaos.rs`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use futures::FutureExt;
 use rand::prelude::*;
 use rand::rngs::StdRng;
 
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Inject chaos into underlying services for robustness test.
 ///
 /// # Chaos
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/complete.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/complete.rs`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 use std::sync::Arc;
 use std::task::Context;
 use std::task::Poll;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 
-use crate::ops::*;
 use crate::raw::oio::into_reader::RangeReader;
 use crate::raw::oio::to_flat_pager;
 use crate::raw::oio::to_hierarchy_pager;
 use crate::raw::oio::Entry;
 use crate::raw::oio::IntoStreamableReader;
 use crate::raw::oio::ToFlatPager;
 use crate::raw::oio::ToHierarchyPager;
@@ -666,15 +665,15 @@
 }
 
 /// Check if the appender has been closed while debug_assertions enabled.
 /// This code will never be executed in release mode.
 #[cfg(debug_assertions)]
 impl<A> Drop for CompleteAppender<A> {
     fn drop(&mut self) {
-        if self.inner.is_none() {
+        if self.inner.is_some() {
             // Do we need to panic here?
             log::warn!("appender has not been closed, must be a bug")
         }
     }
 }
 
 #[async_trait]
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/concurrent_limit.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/concurrent_limit.rs`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 use std::task::Poll;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use tokio::sync::OwnedSemaphorePermit;
 use tokio::sync::Semaphore;
 
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Add concurrent request limit.
 ///
 /// # Notes
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/error_context.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/error_context.rs`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 use std::task::Context;
 use std::task::Poll;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use futures::TryFutureExt;
 
-use crate::ops::*;
 use crate::raw::oio::AppendOperation;
 use crate::raw::oio::PageOperation;
 use crate::raw::oio::ReadOperation;
 use crate::raw::oio::WriteOperation;
 use crate::raw::*;
 use crate::*;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/immutable_index.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/immutable_index.rs`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 use std::collections::HashSet;
 use std::fmt::Debug;
 use std::mem;
 
 use async_trait::async_trait;
 
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Add an immutable in-memory index for underlying storage services.
 ///
 /// Especially useful for services without list capability like HTTP.
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/logging.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/logging.rs`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 use futures::FutureExt;
 use futures::TryFutureExt;
 use log::debug;
 use log::log;
 use log::trace;
 use log::Level;
 
-use crate::ops::*;
 use crate::raw::oio::ReadOperation;
 use crate::raw::oio::WriteOperation;
 use crate::raw::*;
 use crate::*;
 
 /// Add [log](https://docs.rs/log/) for every operations.
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/madsim.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/madsim.rs`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 use async_trait::async_trait;
 use bytes::Bytes;
 #[cfg(madsim)]
 use madsim::net::Endpoint;
 #[cfg(madsim)]
 use madsim::net::Payload;
 
-use crate::ops::*;
 use crate::raw::oio;
 use crate::raw::oio::Entry;
 use crate::raw::*;
 use crate::*;
 
 /// Add deterministic simulation for async operations, powered by [`madsim`](https://docs.rs/madsim/latest/madsim/).
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/metrics.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/metrics.rs`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 use futures::TryFutureExt;
 use metrics::increment_counter;
 use metrics::register_counter;
 use metrics::register_histogram;
 use metrics::Counter;
 use metrics::Histogram;
 
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// requests_total records all successful requests sent via operator.
 static METRIC_REQUESTS_TOTAL: &str = "opendal_requests_total";
 /// requests_duration_seconds records the duration seconds of successful
 /// requests.
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/minitrace.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/minitrace.rs`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 use std::task::Poll;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use futures::FutureExt;
 use minitrace::prelude::*;
 
-use crate::ops::*;
 use crate::raw::oio::PageOperation;
 use crate::raw::oio::ReadOperation;
 use crate::raw::oio::WriteOperation;
 use crate::raw::*;
 use crate::*;
 
 /// Add [minitrace](https://docs.rs/minitrace/) for every operations.
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 mod immutable_index;
 pub use immutable_index::ImmutableIndexLayer;
 
 mod logging;
 pub use logging::LoggingLayer;
 
+mod timeout;
+pub use timeout::TimeoutLayer;
+
 #[cfg(feature = "layers-chaos")]
 mod chaos;
 #[cfg(feature = "layers-chaos")]
 pub use chaos::ChaosLayer;
 
 #[cfg(feature = "layers-metrics")]
 mod metrics;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/oteltrace.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/oteltrace.rs`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 use opentelemetry::trace::FutureExt as TraceFutureExt;
 use opentelemetry::trace::Span;
 use opentelemetry::trace::TraceContextExt;
 use opentelemetry::trace::Tracer;
 use opentelemetry::Context;
 use opentelemetry::KeyValue;
 
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Add [opentelemetry::trace](https://docs.rs/opentelemetry/latest/opentelemetry/trace/index.html) for every operations.
 ///
 /// Examples
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/prometheus.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/prometheus.rs`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 use prometheus::exponential_buckets;
 use prometheus::histogram_opts;
 use prometheus::register_histogram_vec_with_registry;
 use prometheus::register_int_counter_vec_with_registry;
 use prometheus::HistogramVec;
 use prometheus::Registry;
 
-use crate::ops::*;
 use crate::raw::Accessor;
 use crate::raw::*;
 use crate::*;
 /// Add [prometheus](https://docs.rs/prometheus) for every operations.
 ///
 /// # Examples
 ///
@@ -50,15 +49,15 @@
 /// use opendal::layers::PrometheusLayer;
 /// use opendal::services;
 /// use opendal::Operator;
 /// use opendal::Result;
 /// use prometheus::Encoder;
 ///
 /// /// Visit [`opendal::services`] for more service related config.
-/// /// Visit [`opendal::Object`] for more object level APIs.
+/// /// Visit [`opendal::Operator`] for more operator level APIs.
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
 ///     // Pick a builder and configure it.
 ///     let builder = services::Memory::default();
 ///     let registry = prometheus::default_registry();
 ///
 ///     let op = Operator::new(builder)
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/retry.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/retry.rs`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 use backon::ExponentialBackoff;
 use backon::ExponentialBuilder;
 use backon::Retryable;
 use bytes::Bytes;
 use futures::FutureExt;
 use log::warn;
 
-use crate::ops::*;
 use crate::raw::oio::AppendOperation;
 use crate::raw::oio::PageOperation;
 use crate::raw::oio::ReadOperation;
 use crate::raw::oio::WriteOperation;
 use crate::raw::*;
 use crate::*;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/tracing.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/tracing.rs`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 use std::task::Poll;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use futures::FutureExt;
 use tracing::Span;
 
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Add [tracing](https://docs.rs/tracing/) for every operations.
 ///
 /// # Examples
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/layers/type_eraser.rs` & `opendal-0.36.1/local_dependencies/opendal/src/layers/type_eraser.rs`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 // under the License.
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
 
 use async_trait::async_trait;
 
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// TypeEraseLayer will erase the types on internal accessor.
 ///
 /// # Notes
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/lib.rs` & `opendal-0.36.1/local_dependencies/opendal/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/accessor.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/accessor.rs`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 // under the License.
 
 use std::fmt::Debug;
 use std::sync::Arc;
 
 use async_trait::async_trait;
 
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Underlying trait of all backends for implementors.
 ///
 /// The actual data access of storage service happens in Accessor layer.
 /// Every storage supported by OpenDAL must implement [`Accessor`] but not all
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 
 use super::Adapter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Backend of kv service. If the storage service is one k-v-like service, it should implement this kv [`Backend`] by right.
 ///
 /// `Backend` implements one general logic on how to read, write, scan the data from one kv store efficiently.
 /// And the [`Adapter`] held by `Backend` will handle how to communicate with one k-v-like service really and provides
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 
 use super::Adapter;
 use super::Value;
-use crate::ops::*;
 use crate::raw::oio::VectorCursor;
 use crate::raw::*;
 use crate::*;
 
 /// The typed kv backend which implements Accessor for for typed kv adapter.
 #[derive(Debug, Clone)]
 pub struct Backend<S: Adapter> {
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/chrono_util.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/chrono_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/body.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/body.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/client.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/client.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 use std::fmt::Formatter;
 use std::mem;
 use std::str::FromStr;
 
 use futures::TryStreamExt;
 use http::Request;
 use http::Response;
-use reqwest::redirect::Policy;
-use reqwest::Url;
 
 use super::body::IncomingAsyncBody;
 use super::parse_content_length;
 use super::AsyncBody;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
@@ -56,16 +54,14 @@
     pub fn build(mut builder: reqwest::ClientBuilder) -> Result<Self> {
         // Make sure we don't enable auto gzip decompress.
         builder = builder.no_gzip();
         // Make sure we don't enable auto brotli decompress.
         builder = builder.no_brotli();
         // Make sure we don't enable auto deflate decompress.
         builder = builder.no_deflate();
-        // Redirect will be handled by ourselves.
-        builder = builder.redirect(Policy::none());
 
         #[cfg(feature = "trust-dns")]
         let builder = builder.trust_dns(true);
 
         Ok(Self {
             client: builder.build().map_err(|err| {
                 Error::new(ErrorKind::Unexpected, "async client build failed").set_source(err)
@@ -85,15 +81,15 @@
 
         let (parts, body) = req.into_parts();
 
         let mut req_builder = self
             .client
             .request(
                 parts.method,
-                Url::from_str(&url).expect("input request url must be valid"),
+                reqwest::Url::from_str(&url).expect("input request url must be valid"),
             )
             .version(parts.version)
             .headers(parts.headers);
 
         req_builder = match body {
             AsyncBody::Empty => req_builder.body(reqwest::Body::from("")),
             AsyncBody::Bytes(bs) => req_builder.body(reqwest::Body::from(bs)),
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/header.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/header.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/multipart.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/multipart.rs`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 use std::str::FromStr;
 
 use bytes::Bytes;
 use bytes::BytesMut;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
+use http::uri::PathAndQuery;
 use http::HeaderMap;
 use http::HeaderName;
 use http::HeaderValue;
 use http::Method;
 use http::Request;
 use http::Uri;
 use http::Version;
@@ -47,15 +48,15 @@
     }
 }
 
 impl<T: Part> Multipart<T> {
     /// Create a new multipart with random boundary.
     pub fn new() -> Self {
         Multipart {
-            boundary: uuid::Uuid::new_v4().to_string(),
+            boundary: format!("opendal-{}", uuid::Uuid::new_v4()),
             parts: Vec::default(),
         }
     }
 
     /// Set the boundary with given string.
     #[cfg(test)]
     fn with_boundary(mut self, boundary: &str) -> Self {
@@ -232,17 +233,22 @@
             AsyncBody::Empty => Bytes::new(),
             AsyncBody::Bytes(bs) => bs,
         };
 
         Self {
             part_headers,
             method: parts.method,
-            // TODO: Maybe we should support query too?;
-            uri: Uri::from_str(parts.uri.path())
-                .expect("the uri used to build a mixed part must be valid"),
+            uri: Uri::from_str(
+                parts
+                    .uri
+                    .path_and_query()
+                    .unwrap_or(&PathAndQuery::from_static("/"))
+                    .as_str(),
+            )
+            .expect("the uri used to build a mixed part must be valid"),
             version: parts.version,
             headers: parts.headers,
             content,
         }
     }
 
     /// Insert a part header into part.
@@ -280,15 +286,33 @@
     const TYPE: &'static str = "mixed";
 
     fn build(&self) -> Bytes {
         let mut bs = BytesMut::new();
 
         // Write parts headers.
         for (k, v) in self.part_headers.iter() {
-            bs.extend_from_slice(k.as_str().as_bytes());
+            // Trick!
+            //
+            // Azblob could not recognize header names like `content-type`
+            // and requires to use `Content-Type`. So we hardcode the part
+            // headers name here.
+            match k.as_str() {
+                "content-type" => {
+                    bs.extend_from_slice("Content-Type".as_bytes());
+                }
+                "content-id" => {
+                    bs.extend_from_slice("Content-ID".as_bytes());
+                }
+                "content-transfer-encoding" => {
+                    bs.extend_from_slice("Content-Transfer-Encoding".as_bytes());
+                }
+                _ => {
+                    bs.extend_from_slice(k.as_str().as_bytes());
+                }
+            }
             bs.extend_from_slice(b": ");
             bs.extend_from_slice(v.as_bytes());
             bs.extend_from_slice(b"\r\n");
         }
 
         // Write request line: `DELETE /container0/blob0 HTTP/1.1`
         bs.extend_from_slice(b"\r\n");
@@ -484,39 +508,39 @@
                     .header("content-length".parse().unwrap(), "32".parse().unwrap())
                     .content(r#"{"metadata": {"type": "calico"}}"#),
             );
 
         let body = multipart.build();
 
         let expected = r#"--===============7330845974216740156==
-content-type: application/http
-content-transfer-encoding: binary
-content-id: <b29c5de2-0db4-490b-b421-6a51b598bd22+1>
+Content-Type: application/http
+Content-Transfer-Encoding: binary
+Content-ID: <b29c5de2-0db4-490b-b421-6a51b598bd22+1>
 
 PATCH /storage/v1/b/example-bucket/o/obj1 HTTP/1.1
 content-type: application/json
 accept: application/json
 content-length: 31
 
 {"metadata": {"type": "tabby"}}
 --===============7330845974216740156==
-content-type: application/http
-content-transfer-encoding: binary
-content-id: <b29c5de2-0db4-490b-b421-6a51b598bd22+2>
+Content-Type: application/http
+Content-Transfer-Encoding: binary
+Content-ID: <b29c5de2-0db4-490b-b421-6a51b598bd22+2>
 
 PATCH /storage/v1/b/example-bucket/o/obj2 HTTP/1.1
 content-type: application/json
 accept: application/json
 content-length: 32
 
 {"metadata": {"type": "tuxedo"}}
 --===============7330845974216740156==
-content-type: application/http
-content-transfer-encoding: binary
-content-id: <b29c5de2-0db4-490b-b421-6a51b598bd22+3>
+Content-Type: application/http
+Content-Transfer-Encoding: binary
+Content-ID: <b29c5de2-0db4-490b-b421-6a51b598bd22+3>
 
 PATCH /storage/v1/b/example-bucket/o/obj3 HTTP/1.1
 content-type: application/json
 accept: application/json
 content-length: 32
 
 {"metadata": {"type": "calico"}}
@@ -586,37 +610,37 @@
                     )
                     .header("content-length".parse().unwrap(), "0".parse().unwrap()),
             );
 
         let body = multipart.build();
 
         let expected = r#"--batch_357de4f7-6d0b-4e02-8cd2-6361411a9525
-content-type: application/http
-content-transfer-encoding: binary
-content-id: 0
+Content-Type: application/http
+Content-Transfer-Encoding: binary
+Content-ID: 0
 
 DELETE /container0/blob0 HTTP/1.1
 x-ms-date: Thu, 14 Jun 2018 16:46:54 GMT
 authorization: SharedKey account:G4jjBXA7LI/RnWKIOQ8i9xH4p76pAQ+4Fs4R1VxasaE=
 content-length: 0
 
 --batch_357de4f7-6d0b-4e02-8cd2-6361411a9525
-content-type: application/http
-content-transfer-encoding: binary
-content-id: 1
+Content-Type: application/http
+Content-Transfer-Encoding: binary
+Content-ID: 1
 
 DELETE /container1/blob1 HTTP/1.1
 x-ms-date: Thu, 14 Jun 2018 16:46:54 GMT
 authorization: SharedKey account:IvCoYDQ+0VcaA/hKFjUmQmIxXv2RT3XwwTsOTHL39HI=
 content-length: 0
 
 --batch_357de4f7-6d0b-4e02-8cd2-6361411a9525
-content-type: application/http
-content-transfer-encoding: binary
-content-id: 2
+Content-Type: application/http
+Content-Transfer-Encoding: binary
+Content-ID: 2
 
 DELETE /container2/blob2 HTTP/1.1
 x-ms-date: Thu, 14 Jun 2018 16:46:54 GMT
 authorization: SharedKey account:S37N2JTjcmOQVLHLbDmp2johz+KpTJvKhbVc4M7+UqI=
 content-length: 0
 
 --batch_357de4f7-6d0b-4e02-8cd2-6361411a9525--
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/uri.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/http_util/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/layer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/layer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
 
 use async_trait::async_trait;
 
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Layer is used to intercept the operations on the underlying storage.
 ///
 /// Struct that implement this trait must accept input `Arc<dyn Accessor>` as inner,
 /// and returns a new `Arc<dyn Accessor>` as output.
@@ -42,15 +41,14 @@
 ///
 /// # Examples
 ///
 /// ```
 /// use std::sync::Arc;
 ///
 /// use async_trait::async_trait;
-/// use opendal::ops::*;
 /// use opendal::raw::*;
 /// use opendal::*;
 ///
 /// /// Implement the real accessor logic here.
 /// #[derive(Debug)]
 /// struct TraceAccessor<A: Accessor> {
 ///     inner: A,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 
 mod version;
 pub use version::VERSION;
 
 mod rps;
 pub use rps::*;
 
+mod ops;
+pub use ops::*;
+
 mod http_util;
 pub use http_util::*;
 
 mod serde_util;
 pub use serde_util::*;
 
 mod chrono_util;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/append.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/append.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/cursor.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/cursor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/entry.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 use std::task::ready;
 use std::task::Context;
 use std::task::Poll;
 
 use futures::future::BoxFuture;
 use tokio::io::ReadBuf;
 
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Convert given reader into [`oio::Reader`] by range.
 ///
 /// # Notes
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/page.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/page.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/read.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 // under the License.
 
 use std::collections::VecDeque;
 use std::mem;
 
 use async_trait::async_trait;
 
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// to_flat_pager is used to make a hierarchy pager flat.
 pub fn to_flat_pager<A: Accessor, P>(acc: A, path: &str, size: usize) -> ToFlatPager<A, P> {
     #[cfg(debug_assertions)]
     {
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/write.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/oio/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/operation.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/operation.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/path.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/path.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/rps.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/rps.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/serde_util.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/serde_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/raw/version.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/version.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/azblob/backend.rs`

 * *Files 11% similar despite different names*

```diff
@@ -17,26 +17,30 @@
 
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::sync::Arc;
 
 use async_trait::async_trait;
+use base64::prelude::BASE64_STANDARD;
+use base64::Engine;
 use http::header::CONTENT_TYPE;
 use http::StatusCode;
 use log::debug;
 use reqsign::AzureStorageConfig;
 use reqsign::AzureStorageLoader;
 use reqsign::AzureStorageSigner;
+use sha2::Digest;
+use sha2::Sha256;
 
+use super::appender::AzblobAppender;
 use super::batch::parse_batch_delete_response;
 use super::error::parse_error;
 use super::pager::AzblobPager;
 use super::writer::AzblobWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::services::azblob::core::AzblobCore;
 use crate::types::Metadata;
 use crate::*;
 
 /// Known endpoint suffix Azure Storage Blob services resource URI syntax.
 /// Azure public cloud: https://accountname.blob.core.windows.net
@@ -47,23 +51,25 @@
     "blob.core.usgovcloudapi.net",
     "blob.core.chinacloudapi.cn",
 ];
 
 const AZBLOB_BATCH_LIMIT: usize = 256;
 
 /// Azure Storage Blob services support.
-///
 #[doc = include_str!("docs.md")]
 #[derive(Default, Clone)]
 pub struct AzblobBuilder {
     root: Option<String>,
     container: String,
     endpoint: Option<String>,
     account_name: Option<String>,
     account_key: Option<String>,
+    encryption_key: Option<String>,
+    encryption_key_sha256: Option<String>,
+    encryption_algorithm: Option<String>,
     sas_token: Option<String>,
     http_client: Option<HttpClient>,
 }
 
 impl Debug for AzblobBuilder {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         let mut ds = f.debug_struct("Builder");
@@ -140,14 +146,95 @@
         if !account_key.is_empty() {
             self.account_key = Some(account_key.to_string());
         }
 
         self
     }
 
+    /// Set encryption_key of this backend.
+    ///
+    /// # Args
+    ///
+    /// `v`: Base64-encoded key that matches algorithm specified in `encryption_algorithm`.
+    ///
+    /// # Note
+    ///
+    /// This function is the low-level setting for SSE related features.
+    ///
+    /// SSE related options should be set carefully to make them works.
+    /// Please use `server_side_encryption_with_*` helpers if even possible.
+    pub fn encryption_key(&mut self, v: &str) -> &mut Self {
+        if !v.is_empty() {
+            self.encryption_key = Some(v.to_string());
+        }
+
+        self
+    }
+
+    /// Set encryption_key_sha256 of this backend.
+    ///
+    /// # Args
+    ///
+    /// `v`: Base64-encoded SHA256 digest of the key specified in encryption_key.
+    ///
+    /// # Note
+    ///
+    /// This function is the low-level setting for SSE related features.
+    ///
+    /// SSE related options should be set carefully to make them works.
+    /// Please use `server_side_encryption_with_*` helpers if even possible.
+    pub fn encryption_key_sha256(&mut self, v: &str) -> &mut Self {
+        if !v.is_empty() {
+            self.encryption_key_sha256 = Some(v.to_string());
+        }
+
+        self
+    }
+
+    /// Set encryption_algorithm of this backend.
+    ///
+    /// # Args
+    ///
+    /// `v`: server-side encryption algorithm. (Available values: `AES256`)
+    ///
+    /// # Note
+    ///
+    /// This function is the low-level setting for SSE related features.
+    ///
+    /// SSE related options should be set carefully to make them works.
+    /// Please use `server_side_encryption_with_*` helpers if even possible.
+    pub fn encryption_algorithm(&mut self, v: &str) -> &mut Self {
+        if !v.is_empty() {
+            self.encryption_algorithm = Some(v.to_string());
+        }
+
+        self
+    }
+
+    /// Enable server side encryption with customer key.
+    ///
+    /// As known as: CPK
+    ///
+    /// # Args
+    ///
+    /// `key`: Base64-encoded SHA256 digest of the key specified in encryption_key.
+    ///
+    /// # Note
+    ///
+    /// Function that helps the user to set the server-side customer-provided encryption key, the key's SHA256, and the algorithm.
+    /// See [Server-side encryption with customer-provided keys (CPK)](https://learn.microsoft.com/en-us/azure/storage/blobs/encryption-customer-provided-keys)
+    /// for more info.
+    pub fn server_side_encryption_with_customer_key(&mut self, key: &[u8]) -> &mut Self {
+        // Only AES256 is supported for now
+        self.encryption_algorithm = Some("AES256".to_string());
+        self.encryption_key = Some(BASE64_STANDARD.encode(key));
+        self.encryption_key_sha256 = Some(BASE64_STANDARD.encode(Sha256::digest(key).as_slice()));
+        self
+    }
+
     /// Set sas_token of this backend.
     ///
     /// - If sas_token is set, we will take user's input first.
     /// - If not, we will try to load it from environment.
     ///
     /// See [Grant limited access to Azure Storage resources using shared access signatures (SAS)](https://learn.microsoft.com/en-us/azure/storage/common/storage-sas-overview)
     /// for more info.
@@ -263,14 +350,19 @@
         let mut builder = AzblobBuilder::default();
 
         map.get("root").map(|v| builder.root(v));
         map.get("container").map(|v| builder.container(v));
         map.get("endpoint").map(|v| builder.endpoint(v));
         map.get("account_name").map(|v| builder.account_name(v));
         map.get("account_key").map(|v| builder.account_key(v));
+        map.get("encryption_key").map(|v| builder.encryption_key(v));
+        map.get("encryption_key_sha256")
+            .map(|v| builder.encryption_key_sha256(v));
+        map.get("encryption_algorithm")
+            .map(|v| builder.encryption_algorithm(v));
         map.get("sas_token").map(|v| builder.sas_token(v));
 
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         debug!("backend build started: {:?}", &self);
@@ -310,30 +402,62 @@
                 .clone()
                 .or_else(|| infer_storage_name_from_endpoint(endpoint.as_str())),
             account_key: self.account_key.clone(),
             sas_token: self.sas_token.clone(),
             ..Default::default()
         };
 
+        let encryption_key =
+            match &self.encryption_key {
+                None => None,
+                Some(v) => Some(build_header_value(v).map_err(|err| {
+                    err.with_context("key", "server_side_encryption_customer_key")
+                })?),
+            };
+
+        let encryption_key_sha256 = match &self.encryption_key_sha256 {
+            None => None,
+            Some(v) => Some(build_header_value(v).map_err(|err| {
+                err.with_context("key", "server_side_encryption_customer_key_sha256")
+            })?),
+        };
+
+        let encryption_algorithm = match &self.encryption_algorithm {
+            None => None,
+            Some(v) => {
+                if v == "AES256" {
+                    Some(build_header_value(v).map_err(|err| {
+                        err.with_context("key", "server_side_encryption_customer_algorithm")
+                    })?)
+                } else {
+                    return Err(Error::new(
+                        ErrorKind::ConfigInvalid,
+                        "encryption_algorithm value must be AES256",
+                    ));
+                }
+            }
+        };
+
         let cred_loader = AzureStorageLoader::new(config_loader);
 
         let signer = AzureStorageSigner::new();
-        let batch_signer = AzureStorageSigner::new().omit_service_version();
 
         debug!("backend build finished: {:?}", &self);
         Ok(AzblobBackend {
             core: Arc::new(AzblobCore {
                 root,
                 endpoint,
+                encryption_key,
+                encryption_key_sha256,
+                encryption_algorithm,
                 container: self.container.clone(),
 
                 client,
                 loader: cred_loader,
                 signer,
-                batch_signer,
             }),
             has_sas_token: self.sas_token.is_some(),
         })
     }
 }
 
 fn infer_storage_name_from_endpoint(endpoint: &str) -> Option<String> {
@@ -369,15 +493,15 @@
 
 #[async_trait]
 impl Accessor for AzblobBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = AzblobWriter;
     type BlockingWriter = ();
-    type Appender = ();
+    type Appender = AzblobAppender;
     type Pager = AzblobPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Azblob)
             .set_root(&self.core.root)
@@ -394,14 +518,18 @@
                 read_with_if_none_match: true,
                 read_with_override_content_disposition: true,
 
                 write: true,
                 write_with_cache_control: true,
                 write_with_content_type: true,
 
+                append: true,
+                append_with_cache_control: true,
+                append_with_content_type: true,
+
                 delete: true,
                 create_dir: true,
                 copy: true,
 
                 list: true,
                 list_with_delimiter_slash: true,
                 list_without_delimiter: true,
@@ -475,14 +603,21 @@
 
         Ok((
             RpWrite::default(),
             AzblobWriter::new(self.core.clone(), args, path.to_string()),
         ))
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        Ok((
+            RpAppend::default(),
+            AzblobAppender::new(self.core.clone(), path, args),
+        ))
+    }
+
     async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
         let resp = self.core.azblob_copy_blob(from, to).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::ACCEPTED => {
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/batch.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/azblob/batch.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/core.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gcs/core.rs`

 * *Files 21% similar despite different names*

```diff
@@ -11,243 +11,312 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::fmt;
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::fmt::Write;
 use std::time::Duration;
 
-use http::header::HeaderName;
+use backon::ExponentialBuilder;
+use backon::Retryable;
+use bytes::Bytes;
+use bytes::BytesMut;
 use http::header::CONTENT_LENGTH;
+use http::header::CONTENT_RANGE;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
-use reqsign::AzureStorageCredential;
-use reqsign::AzureStorageLoader;
-use reqsign::AzureStorageSigner;
+use once_cell::sync::Lazy;
+use reqsign::GoogleCredential;
+use reqsign::GoogleCredentialLoader;
+use reqsign::GoogleSigner;
+use reqsign::GoogleToken;
+use reqsign::GoogleTokenLoader;
 
+use super::uri::percent_encode_path;
 use crate::raw::*;
 use crate::*;
 
-mod constants {
-    pub const X_MS_BLOB_TYPE: &str = "x-ms-blob-type";
-    pub const X_MS_COPY_SOURCE: &str = "x-ms-copy-source";
-    pub const X_MS_BLOB_CACHE_CONTROL: &str = "x-ms-blob-cache-control";
-}
-
-pub struct AzblobCore {
-    pub container: String,
-    pub root: String,
+pub struct GcsCore {
     pub endpoint: String,
+    pub bucket: String,
+    pub root: String,
 
     pub client: HttpClient,
-    pub loader: AzureStorageLoader,
-    pub signer: AzureStorageSigner,
-    pub batch_signer: AzureStorageSigner,
+    pub signer: GoogleSigner,
+    pub token_loader: GoogleTokenLoader,
+    pub credential_loader: GoogleCredentialLoader,
+
+    pub predefined_acl: Option<String>,
+    pub default_storage_class: Option<String>,
+
+    pub write_fixed_size: usize,
 }
 
-impl Debug for AzblobCore {
-    fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
-        f.debug_struct("AzblobCore")
-            .field("container", &self.container)
+impl Debug for GcsCore {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
+        let mut de = f.debug_struct("Backend");
+        de.field("endpoint", &self.endpoint)
+            .field("bucket", &self.bucket)
             .field("root", &self.root)
-            .field("endpoint", &self.endpoint)
             .finish_non_exhaustive()
     }
 }
 
-impl AzblobCore {
-    async fn load_credential(&self) -> Result<AzureStorageCredential> {
-        let cred = self
-            .loader
-            .load()
+static BACKOFF: Lazy<ExponentialBuilder> =
+    Lazy::new(|| ExponentialBuilder::default().with_jitter());
+
+impl GcsCore {
+    async fn load_token(&self) -> Result<GoogleToken> {
+        let cred = { || self.token_loader.load() }
+            .retry(&*BACKOFF)
             .await
             .map_err(new_request_credential_error)?;
 
         if let Some(cred) = cred {
             Ok(cred)
         } else {
             Err(Error::new(
                 ErrorKind::ConfigInvalid,
                 "no valid credential found",
             ))
         }
     }
 
-    pub async fn sign_query<T>(&self, req: &mut Request<T>) -> Result<()> {
-        let cred = self.load_credential().await?;
+    fn load_credential(&self) -> Result<GoogleCredential> {
+        let cred = self
+            .credential_loader
+            .load()
+            .map_err(new_request_credential_error)?;
 
-        self.signer
-            .sign_query(req, Duration::from_secs(3600), &cred)
-            .map_err(new_request_sign_error)
+        if let Some(cred) = cred {
+            Ok(cred)
+        } else {
+            Err(Error::new(
+                ErrorKind::ConfigInvalid,
+                "no valid credential found",
+            ))
+        }
     }
 
     pub async fn sign<T>(&self, req: &mut Request<T>) -> Result<()> {
-        let cred = self.load_credential().await?;
+        let cred = self.load_token().await?;
+
         self.signer.sign(req, &cred).map_err(new_request_sign_error)
     }
 
-    async fn batch_sign<T>(&self, req: &mut Request<T>) -> Result<()> {
-        let cred = self.load_credential().await?;
-        self.batch_signer
-            .sign(req, &cred)
+    pub async fn sign_query<T>(&self, req: &mut Request<T>, duration: Duration) -> Result<()> {
+        let cred = self.load_credential()?;
+
+        self.signer
+            .sign_query(req, duration, &cred)
             .map_err(new_request_sign_error)
     }
 
     #[inline]
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
         self.client.send(req).await
     }
 }
 
-impl AzblobCore {
-    pub fn azblob_get_blob_request(
+impl GcsCore {
+    pub fn gcs_get_object_request(
         &self,
         path: &str,
         range: BytesRange,
-        if_none_match: Option<&str>,
         if_match: Option<&str>,
-        override_content_disposition: Option<&str>,
+        if_none_match: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
-        let mut url = format!(
-            "{}/{}/{}",
+        let url = format!(
+            "{}/storage/v1/b/{}/o/{}?alt=media",
             self.endpoint,
-            self.container,
+            self.bucket,
             percent_encode_path(&p)
         );
 
-        let mut query_args = Vec::new();
-        if let Some(override_content_disposition) = override_content_disposition {
-            query_args.push(format!(
-                "rscd={}",
-                percent_encode_path(override_content_disposition)
-            ))
-        }
-
-        if !query_args.is_empty() {
-            url.push_str(&format!("?{}", query_args.join("&")));
-        }
-
         let mut req = Request::get(&url);
 
-        if !range.is_full() {
-            // azblob doesn't support read with suffix range.
-            //
-            // ref: https://learn.microsoft.com/en-us/rest/api/storageservices/specifying-the-range-header-for-blob-service-operations
-            if range.offset().is_none() && range.size().is_some() {
-                return Err(Error::new(
-                    ErrorKind::Unsupported,
-                    "azblob doesn't support read with suffix range",
-                ));
-            }
-
-            req = req.header(http::header::RANGE, range.to_header());
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
         }
-
         if let Some(if_none_match) = if_none_match {
             req = req.header(IF_NONE_MATCH, if_none_match);
         }
+        if !range.is_full() {
+            req = req.header(http::header::RANGE, range.to_header());
+        }
+
+        let req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        Ok(req)
+    }
+
+    // It's for presign operation. Gcs only supports query sign over XML API.
+    pub fn gcs_get_object_xml_request(
+        &self,
+        path: &str,
+        range: BytesRange,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!("{}/{}/{}", self.endpoint, self.bucket, p);
+
+        let mut req = Request::get(&url);
 
         if let Some(if_match) = if_match {
             req = req.header(IF_MATCH, if_match);
         }
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+        if !range.is_full() {
+            req = req.header(http::header::RANGE, range.to_header());
+        }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn azblob_get_blob(
+    pub async fn gcs_get_object(
         &self,
         path: &str,
         range: BytesRange,
-        if_none_match: Option<&str>,
         if_match: Option<&str>,
-        override_content_disposition: Option<&str>,
+        if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.azblob_get_blob_request(
-            path,
-            range,
-            if_none_match,
-            if_match,
-            override_content_disposition,
-        )?;
+        let mut req = self.gcs_get_object_request(path, range, if_match, if_none_match)?;
 
         self.sign(&mut req).await?;
-
         self.send(req).await
     }
 
-    pub fn azblob_put_blob_request(
+    pub fn gcs_insert_object_request(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
-        cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
-        let url = format!(
-            "{}/{}/{}",
+        let mut url = format!(
+            "{}/upload/storage/v1/b/{}/o?uploadType={}&name={}",
             self.endpoint,
-            self.container,
+            self.bucket,
+            if self.default_storage_class.is_some() {
+                "multipart"
+            } else {
+                "media"
+            },
             percent_encode_path(&p)
         );
 
-        let mut req = Request::put(&url);
-        if let Some(cache_control) = cache_control {
-            req = req.header(constants::X_MS_BLOB_CACHE_CONTROL, cache_control);
+        if let Some(acl) = &self.predefined_acl {
+            write!(&mut url, "&predefinedAcl={}", acl).unwrap();
         }
-        if let Some(size) = size {
-            req = req.header(CONTENT_LENGTH, size)
+
+        let mut req = Request::post(&url);
+
+        req = req.header(CONTENT_LENGTH, size.unwrap_or_default());
+
+        if let Some(storage_class) = &self.default_storage_class {
+            req = req.header(CONTENT_TYPE, "multipart/related; boundary=my-boundary");
+
+            let mut req_body = BytesMut::with_capacity(100);
+            write!(
+                &mut req_body,
+                "--my-boundary\nContent-Type: application/json; charset=UTF-8\n\n{{\"storageClass\": \"{}\"}}\n\n--my-boundary\n",
+                storage_class
+            ).unwrap();
+
+            if let Some(mime) = content_type {
+                write!(&mut req_body, "Content-Type: {}\n\n", mime).unwrap();
+            } else {
+                write!(&mut req_body, "Content-Type: application/octet-stream\n\n").unwrap();
+            }
+
+            if let AsyncBody::Bytes(bytes) = body {
+                req_body.extend_from_slice(&bytes);
+            }
+            write!(&mut req_body, "\n--my-boundary").unwrap();
+
+            let req_body = AsyncBody::Bytes(req_body.freeze());
+            let req = req.body(req_body).map_err(new_request_build_error)?;
+            Ok(req)
+        } else {
+            if let Some(content_type) = content_type {
+                req = req.header(CONTENT_TYPE, content_type);
+            }
+
+            let req = req.body(body).map_err(new_request_build_error)?;
+            Ok(req)
         }
+    }
+
+    // It's for presign operation. Gcs only supports query sign over XML API.
+    pub fn gcs_insert_object_xml_request(
+        &self,
+        path: &str,
+        content_type: Option<&str>,
+        body: AsyncBody,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
 
-        if let Some(ty) = content_type {
-            req = req.header(CONTENT_TYPE, ty)
+        let url = format!("{}/{}/{}", self.endpoint, self.bucket, p);
+
+        let mut req = Request::put(&url);
+
+        if let Some(content_type) = content_type {
+            req = req.header(CONTENT_TYPE, content_type);
         }
 
-        req = req.header(
-            HeaderName::from_static(constants::X_MS_BLOB_TYPE),
-            "BlockBlob",
-        );
+        if let Some(acl) = &self.predefined_acl {
+            req = req.header("x-goog-acl", acl);
+        }
+
+        if let Some(storage_class) = &self.default_storage_class {
+            req = req.header("x-goog-storage-class", storage_class);
+        }
 
-        // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub fn azblob_head_blob_request(
+    pub fn gcs_head_object_request(
         &self,
         path: &str,
-        if_none_match: Option<&str>,
         if_match: Option<&str>,
+        if_none_match: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
-            "{}/{}/{}",
+            "{}/storage/v1/b/{}/o/{}",
             self.endpoint,
-            self.container,
+            self.bucket,
             percent_encode_path(&p)
         );
 
-        let mut req = Request::head(&url);
+        let mut req = Request::get(&url);
 
         if let Some(if_none_match) = if_none_match {
             req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
         if let Some(if_match) = if_match {
             req = req.header(IF_MATCH, if_match);
@@ -256,136 +325,231 @@
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn azblob_get_blob_properties(
+    // It's for presign operation. Gcs only supports query sign over XML API.
+    pub fn gcs_head_object_xml_request(
         &self,
         path: &str,
+        if_match: Option<&str>,
         if_none_match: Option<&str>,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!("{}/{}/{}", self.endpoint, self.bucket, p);
+
+        let mut req = Request::head(&url);
+
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
+
+        let req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        Ok(req)
+    }
+
+    pub async fn gcs_get_object_metadata(
+        &self,
+        path: &str,
         if_match: Option<&str>,
+        if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.azblob_head_blob_request(path, if_none_match, if_match)?;
+        let mut req = self.gcs_head_object_request(path, if_match, if_none_match)?;
 
         self.sign(&mut req).await?;
+
         self.send(req).await
     }
 
-    pub fn azblob_delete_blob_request(&self, path: &str) -> Result<Request<AsyncBody>> {
+    pub async fn gcs_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
-            "{}/{}/{}",
+            "{}/storage/v1/b/{}/o/{}",
             self.endpoint,
-            self.container,
+            self.bucket,
             percent_encode_path(&p)
         );
 
-        let req = Request::delete(&url);
-
-        req.header(CONTENT_LENGTH, 0)
+        let mut req = Request::delete(&url)
             .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)
-    }
-
-    pub async fn azblob_delete_blob(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.azblob_delete_blob_request(path)?;
+            .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
+
         self.send(req).await
     }
 
-    pub async fn azblob_copy_blob(
+    pub async fn gcs_copy_object(
         &self,
         from: &str,
         to: &str,
     ) -> Result<Response<IncomingAsyncBody>> {
         let source = build_abs_path(&self.root, from);
-        let target = build_abs_path(&self.root, to);
+        let dest = build_abs_path(&self.root, to);
 
-        let source = format!(
-            "{}/{}/{}",
-            self.endpoint,
-            self.container,
-            percent_encode_path(&source)
-        );
-        let target = format!(
-            "{}/{}/{}",
+        let req_uri = format!(
+            "{}/storage/v1/b/{}/o/{}/copyTo/b/{}/o/{}",
             self.endpoint,
-            self.container,
-            percent_encode_path(&target)
+            self.bucket,
+            percent_encode_path(&source),
+            self.bucket,
+            percent_encode_path(&dest)
         );
 
-        let mut req = Request::put(&target)
-            .header(constants::X_MS_COPY_SOURCE, source)
+        let mut req = Request::post(req_uri)
             .header(CONTENT_LENGTH, 0)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
-    pub async fn azblob_list_blobs(
+    pub async fn gcs_list_objects(
         &self,
         path: &str,
-        next_marker: &str,
+        page_token: &str,
         delimiter: &str,
         limit: Option<usize>,
+        start_after: Option<String>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let mut url = format!(
-            "{}/{}?restype=container&comp=list",
-            self.endpoint, self.container
+            "{}/storage/v1/b/{}/o?prefix={}",
+            self.endpoint,
+            self.bucket,
+            percent_encode_path(&p)
         );
-        if !p.is_empty() {
-            write!(url, "&prefix={}", percent_encode_path(&p))
-                .expect("write into string must succeed");
+        if !delimiter.is_empty() {
+            write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
         }
         if let Some(limit) = limit {
-            write!(url, "&maxresults={limit}").expect("write into string must succeed");
+            write!(url, "&maxResults={limit}").expect("write into string must succeed");
         }
-        if !delimiter.is_empty() {
-            write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
+        if let Some(start_after) = start_after {
+            let start_after = build_abs_path(&self.root, &start_after);
+            write!(url, "&startOffset={}", percent_encode_path(&start_after))
+                .expect("write into string must succeed");
         }
-        if !next_marker.is_empty() {
-            write!(url, "&marker={next_marker}").expect("write into string must succeed");
+
+        if !page_token.is_empty() {
+            // NOTE:
+            //
+            // GCS uses pageToken in request and nextPageToken in response
+            //
+            // Don't know how will those tokens be like so this part are copied
+            // directly from AWS S3 service.
+            write!(url, "&pageToken={}", percent_encode_path(page_token))
+                .expect("write into string must succeed");
         }
 
         let mut req = Request::get(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
+
         self.send(req).await
     }
 
-    pub async fn azblob_batch_delete(
+    pub async fn gcs_initiate_resumable_upload(
         &self,
-        paths: &[String],
+        path: &str,
     ) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
         let url = format!(
-            "{}/{}?restype=container&comp=batch",
-            self.endpoint, self.container
+            "{}/upload/storage/v1/b/{}/o?uploadType=resumable&name={}",
+            self.endpoint, self.bucket, p
         );
 
-        let mut multipart = Multipart::new();
+        let mut req = Request::post(&url)
+            .header(CONTENT_LENGTH, 0)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
 
-        for (idx, path) in paths.iter().enumerate() {
-            let mut req = self.azblob_delete_blob_request(path)?;
+        self.sign(&mut req).await?;
+        self.send(req).await
+    }
 
-            self.batch_sign(&mut req).await?;
-            multipart = multipart.part(
-                MixedPart::from_request(req).part_header("content-id".parse().unwrap(), idx.into()),
-            );
-        }
+    pub fn gcs_upload_in_resumable_upload(
+        &self,
+        location: &str,
+        size: u64,
+        written: u64,
+        is_last_part: bool,
+        body: AsyncBody,
+    ) -> Result<Request<AsyncBody>> {
+        let mut req = Request::put(location);
 
-        let req = Request::post(url);
-        let mut req = multipart.apply(req)?;
+        let range_header = if is_last_part {
+            format!(
+                "bytes {}-{}/{}",
+                written,
+                written + size - 1,
+                written + size
+            )
+        } else {
+            format!("bytes {}-{}/*", written, written + size - 1)
+        };
+
+        req = req
+            .header(CONTENT_LENGTH, size)
+            .header(CONTENT_RANGE, range_header);
+
+        // Set body
+        let req = req.body(body).map_err(new_request_build_error)?;
+
+        Ok(req)
+    }
+
+    pub async fn gcs_complete_resumable_upload(
+        &self,
+        location: &str,
+        written_bytes: u64,
+        bs: Bytes,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let size = bs.len() as u64;
+        let mut req = Request::post(location)
+            .header(CONTENT_LENGTH, size)
+            .header(
+                CONTENT_RANGE,
+                format!(
+                    "bytes {}-{}/{}",
+                    written_bytes,
+                    written_bytes + size - 1,
+                    written_bytes + size
+                ),
+            )
+            .body(AsyncBody::Bytes(bs))
+            .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
+
+        self.send(req).await
+    }
+
+    pub async fn gcs_abort_resumable_upload(
+        &self,
+        location: &str,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = Request::delete(location)
+            .header(CONTENT_LENGTH, 0)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        self.sign(&mut req).await?;
+
         self.send(req).await
     }
 }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/docs.md` & `opendal-0.36.1/local_dependencies/opendal/src/services/azblob/docs.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-# Capabilities
+## Capabilities
 
 This service can be used to:
 
 - [x] stat
 - [x] read
 - [x] write
+- [x] append
 - [x] create_dir
 - [x] delete
 - [x] copy
 - [ ] rename
 - [x] list
 - [x] scan
 - [x] presign
 - [ ] blocking
 
-# Configuration
+## Configuration
 
 - `root`: Set the work dir for backend.
 - `container`: Set the container name for backend.
 - `endpoint`: Set the endpoint for backend.
 - `account_name`: Set the account_name for backend.
 - `account_key`: Set the account_key for backend.
 
 Refer to public API docs for more information.
 
-# Examples
+## Examples
 
 This example works on [Azurite](https://github.com/Azure/Azurite) for local developments.
 
-## Start local blob service
+### Start local blob service
 
 ```shell
 docker run -p 10000:10000 mcr.microsoft.com/azure-storage/azurite
 az storage container create --name test --connection-string "DefaultEndpointsProtocol=http;AccountName=devstoreaccount1;AccountKey=Eby8vdM02xNOcqFlqUwJPLlmEtlCDXJ1OUzFT50uSRZ6IFsuFq2UVErCz4I6tq/K1SZFPTOtr/KBHBeksoGMGw==;BlobEndpoint=http://127.0.0.1:10000/devstoreaccount1;"
 ```
 
-## Init OpenDAL Operator
+### Init OpenDAL Operator
 
 ### Via Builder
 
 ```rust
 use std::sync::Arc;
 
 use anyhow::Result;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/azblob/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::AzblobBuilder as Azblob;
+pub use backend::AzdfsBuilder as Azdfs;
 
-mod batch;
 mod core;
 mod error;
 mod pager;
 mod writer;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/azblob/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/cos/writer.rs`

 * *Files 7% similar despite different names*

```diff
@@ -17,37 +17,36 @@
 
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::AzblobCore;
+use super::core::CosCore;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct AzblobWriter {
-    core: Arc<AzblobCore>,
+pub struct CosWriter {
+    core: Arc<CosCore>,
 
     op: OpWrite,
     path: String,
 }
 
-impl AzblobWriter {
-    pub fn new(core: Arc<AzblobCore>, op: OpWrite, path: String) -> Self {
-        AzblobWriter { core, op, path }
+impl CosWriter {
+    pub fn new(core: Arc<CosCore>, op: OpWrite, path: String) -> Self {
+        CosWriter { core, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for AzblobWriter {
+impl oio::Write for CosWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.core.azblob_put_blob_request(
+        let mut req = self.core.cos_put_object_request(
             &self.path,
             Some(bs.len()),
             self.op.content_type(),
             self.op.cache_control(),
             AsyncBody::Bytes(bs),
         )?;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/backend.rs`

 * *Files 14% similar despite different names*

```diff
@@ -27,102 +27,29 @@
 use reqsign::AzureStorageLoader;
 use reqsign::AzureStorageSigner;
 
 use super::core::AzdfsCore;
 use super::error::parse_error;
 use super::pager::AzdfsPager;
 use super::writer::AzdfsWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Known endpoint suffix Azure Data Lake Storage Gen2 URI syntax.
 /// Azure public cloud: https://accountname.dfs.core.windows.net
 /// Azure US Government: https://accountname.dfs.core.usgovcloudapi.net
 /// Azure China: https://accountname.dfs.core.chinacloudapi.cn
 const KNOWN_AZDFS_ENDPOINT_SUFFIX: &[&str] = &[
     "dfs.core.windows.net",
     "dfs.core.usgovcloudapi.net",
     "dfs.core.chinacloudapi.cn",
 ];
 
 /// Azure Data Lake Storage Gen2 Support.
-///
-/// As known as `abfs`, `azdfs` or `azdls`.
-///
-/// This service will visist the [ABFS](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-abfs-driver) URI supported by [Azure Data Lake Storage Gen2](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction).
-///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [ ] copy
-/// - [x] rename
-/// - [x] list
-/// - [ ] ~~scan~~
-/// - [ ] presign
-/// - [ ] blocking
-///
-/// # Configuration
-///
-/// - `root`: Set the work dir for backend.
-/// - `filesystem`: Set the filesystem name for backend.
-/// - `endpoint`: Set the endpoint for backend.
-/// - `account_name`: Set the account_name for backend.
-/// - `account_key`: Set the account_key for backend.
-///
-/// Refer to public API docs for more information.
-///
-/// # Example
-///
-/// ## Init OpenDAL Operator
-///
-/// ### Via Builder
-///
-/// ```no_run
-/// use std::sync::Arc;
-///
-/// use anyhow::Result;
-/// use opendal::services::Azdfs;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     // Create azblob backend builder.
-///     let mut builder = Azdfs::default();
-///     // Set the root for azblob, all operations will happen under this root.
-///     //
-///     // NOTE: the root must be absolute path.
-///     builder.root("/path/to/dir");
-///     // Set the filesystem name, this is required.
-///     builder.filesystem("test");
-///     // Set the endpoint, this is required.
-///     //
-///     // For examples:
-///     // - "https://accountname.dfs.core.windows.net"
-///     builder.endpoint("https://accountname.dfs.core.windows.net");
-///     // Set the account_name and account_key.
-///     //
-///     // OpenDAL will try load credential from the env.
-///     // If credential not set and no valid credential in env, OpenDAL will
-///     // send request without signing like anonymous user.
-///     builder.account_name("account_name");
-///     builder.account_key("account_key");
-///
-///     // `Accessor` provides the low level APIs, we will use `Operator` normally.
-///     let op: Operator = Operator::new(builder)?.finish();
-///
-///     Ok(())
-/// }
-/// ```
+#[doc = include_str!("docs.md")]
 #[derive(Default, Clone)]
 pub struct AzdfsBuilder {
     root: Option<String>,
     filesystem: String,
     endpoint: Option<String>,
     account_name: Option<String>,
     account_key: Option<String>,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/core.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/core.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,27 @@
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::fmt::Write;
 
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
+use http::HeaderName;
+use http::HeaderValue;
 use http::Request;
 use http::Response;
 use reqsign::AzureStorageCredential;
 use reqsign::AzureStorageLoader;
 use reqsign::AzureStorageSigner;
 
 use crate::raw::*;
 use crate::*;
 
 const X_MS_RENAME_SOURCE: &str = "x-ms-rename-source";
+const X_MS_VERSION: &str = "x-ms-version";
 
 pub struct AzdfsCore {
     pub filesystem: String,
     pub root: String,
     pub endpoint: String,
 
     pub client: HttpClient,
@@ -70,14 +73,24 @@
                 "no valid credential found",
             ))
         }
     }
 
     pub async fn sign<T>(&self, req: &mut Request<T>) -> Result<()> {
         let cred = self.load_credential().await?;
+        // Insert x-ms-version header for normal requests.
+        req.headers_mut().insert(
+            HeaderName::from_static(X_MS_VERSION),
+            // 2022-11-02 is the version supported by Azurite V3 and
+            // used by Azure Portal, We use this version to make
+            // sure most our developer happy.
+            //
+            // In the future, we could allow users to configure this value.
+            HeaderValue::from_static("2022-11-02"),
+        );
         self.signer.sign(req, &cred).map_err(new_request_sign_error)
     }
 
     #[inline]
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
         self.client.send(req).await
     }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/fs/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::AzdfsBuilder as Azdfs;
+pub use backend::FsBuilder as Fs;
 
-mod core;
+mod appender;
 mod error;
 mod pager;
 mod writer;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/azdfs/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
 use super::core::AzdfsCore;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct AzdfsWriter {
     core: Arc<AzdfsCore>,
 
     op: OpWrite,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/cos/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/cos/backend.rs`

 * *Files 14% similar despite different names*

```diff
@@ -27,77 +27,20 @@
 use reqsign::TencentCosCredentialLoader;
 use reqsign::TencentCosSigner;
 
 use super::core::CosCore;
 use super::error::parse_error;
 use super::pager::CosPager;
 use super::writer::CosWriter;
-use crate::ops::*;
 use crate::raw::*;
+use crate::services::cos::appender::CosAppender;
 use crate::*;
 
 /// Huawei Cloud COS services support.
-///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [x] copy
-/// - [ ] rename
-/// - [x] list
-/// - [x] scan
-/// - [ ] presign
-/// - [ ] blocking
-///
-/// # Configuration
-///
-/// - `root`: Set the work directory for backend
-/// - `bucket`: Set the container name for backend
-/// - `endpoint`: Customizable endpoint setting
-/// - `access_key_id`: Set the access_key_id for backend.
-/// - `secret_access_key`: Set the secret_access_key for backend.
-///
-/// You can refer to [`CosBuilder`]'s docs for more information
-///
-/// # Example
-///
-/// ## Via Builder
-///
-/// ```no_run
-/// use anyhow::Result;
-/// use opendal::services::Cos;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     // create backend builder
-///     let mut builder = Cos::default();
-///
-///     // set the storage bucket for OpenDAL
-///     builder.bucket("test");
-///     // set the endpoint for OpenDAL
-///     builder.endpoint("https://cos.ap-singapore.myqcloud.com");
-///     // Set the access_key_id and secret_access_key.
-///     //
-///     // OpenDAL will try load credential from the env.
-///     // If credential not set and no valid credential in env, OpenDAL will
-///     // send request without signing like anonymous user.
-///     builder.secret_id("secret_id");
-///     builder.secret_key("secret_access_key");
-///
-///     let op: Operator = Operator::new(builder)?.finish();
-///
-///     Ok(())
-/// }
-/// ```
+#[doc = include_str!("docs.md")]
 #[derive(Default, Clone)]
 pub struct CosBuilder {
     root: Option<String>,
     endpoint: Option<String>,
     secret_id: Option<String>,
     secret_key: Option<String>,
     bucket: Option<String>,
@@ -298,15 +241,15 @@
 
 #[async_trait]
 impl Accessor for CosBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = CosWriter;
     type BlockingWriter = ();
-    type Appender = ();
+    type Appender = CosAppender;
     type Pager = CosPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Cos)
             .set_root(&self.core.root)
@@ -322,14 +265,19 @@
                 read_with_if_match: true,
                 read_with_if_none_match: true,
 
                 write: true,
                 write_with_content_type: true,
                 write_with_cache_control: true,
 
+                append: true,
+                append_with_cache_control: true,
+                append_with_content_disposition: true,
+                append_with_content_type: true,
+
                 delete: true,
                 create_dir: true,
                 copy: true,
 
                 list: true,
                 list_with_delimiter_slash: true,
                 list_without_delimiter: true,
@@ -392,14 +340,21 @@
 
         Ok((
             RpWrite::default(),
             CosWriter::new(self.core.clone(), args, path.to_string()),
         ))
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        Ok((
+            RpAppend::default(),
+            CosAppender::new(self.core.clone(), path, args),
+        ))
+    }
+
     async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
         let resp = self.core.cos_copy_object(from, to).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => {
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/cos/core.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/cos/core.rs`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 // under the License.
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::time::Duration;
 
 use http::header::CACHE_CONTROL;
+use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
 use reqsign::TencentCosCredential;
@@ -225,14 +226,50 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
+    pub fn cos_append_object_request(
+        &self,
+        path: &str,
+        position: u64,
+        size: usize,
+        args: &OpAppend,
+        body: AsyncBody,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+        let url = format!(
+            "{}/{}?append&position={}",
+            self.endpoint,
+            percent_encode_path(&p),
+            position
+        );
+
+        let mut req = Request::post(&url);
+
+        req = req.header(CONTENT_LENGTH, size);
+
+        if let Some(mime) = args.content_type() {
+            req = req.header(CONTENT_TYPE, mime);
+        }
+
+        if let Some(pos) = args.content_disposition() {
+            req = req.header(CONTENT_DISPOSITION, pos);
+        }
+
+        if let Some(cache_control) = args.cache_control() {
+            req = req.header(CACHE_CONTROL, cache_control)
+        }
+
+        let req = req.body(body).map_err(new_request_build_error)?;
+        Ok(req)
+    }
+
     pub async fn cos_copy_object(
         &self,
         from: &str,
         to: &str,
     ) -> Result<Response<IncomingAsyncBody>> {
         let source = build_abs_path(&self.root, from);
         let target = build_abs_path(&self.root, to);
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/cos/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/cos/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/cos/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/cos/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
 pub use backend::CosBuilder as Cos;
 
+mod appender;
 mod core;
 mod error;
 mod pager;
 mod writer;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/cos/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/cos/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/cos/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/wasabi/writer.rs`

 * *Files 8% similar despite different names*

```diff
@@ -17,51 +17,48 @@
 
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::CosCore;
+use super::core::*;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct CosWriter {
-    core: Arc<CosCore>,
+pub struct WasabiWriter {
+    core: Arc<WasabiCore>,
 
     op: OpWrite,
     path: String,
 }
 
-impl CosWriter {
-    pub fn new(core: Arc<CosCore>, op: OpWrite, path: String) -> Self {
-        CosWriter { core, op, path }
+impl WasabiWriter {
+    pub fn new(core: Arc<WasabiCore>, op: OpWrite, path: String) -> Self {
+        WasabiWriter { core, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for CosWriter {
+impl oio::Write for WasabiWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.core.cos_put_object_request(
-            &self.path,
-            Some(bs.len()),
-            self.op.content_type(),
-            self.op.cache_control(),
-            AsyncBody::Bytes(bs),
-        )?;
+        let resp = self
+            .core
+            .put_object(
+                &self.path,
+                Some(bs.len()),
+                self.op.content_type(),
+                self.op.content_disposition(),
+                self.op.cache_control(),
+                AsyncBody::Bytes(bs),
+            )
+            .await?;
 
-        self.core.sign(&mut req).await?;
-
-        let resp = self.core.send(req).await?;
-
-        let status = resp.status();
-
-        match status {
+        match resp.status() {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/dashmap/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/dashmap/backend.rs`

 * *Files 10% similar despite different names*

```diff
@@ -21,30 +21,15 @@
 use async_trait::async_trait;
 use dashmap::DashMap;
 
 use crate::raw::adapters::typed_kv;
 use crate::*;
 
 /// [dashmap](https://github.com/xacrimon/dashmap) backend support.
-///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [ ] copy
-/// - [ ] rename
-/// - [ ] list
-/// - [x] scan
-/// - [ ] presign
-/// - [ ] blocking
+#[doc = include_str!("docs.md")]
 #[derive(Default)]
 pub struct DashmapBuilder {
     root: Option<String>,
 }
 
 impl DashmapBuilder {
     /// Set the root for dashmap.
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/dashmap/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/dashmap/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/fs/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/fs/backend.rs`

 * *Files 6% similar despite different names*

```diff
@@ -23,71 +23,23 @@
 
 use async_compat::Compat;
 use async_trait::async_trait;
 use chrono::DateTime;
 use log::debug;
 use uuid::Uuid;
 
+use super::appender::FsAppender;
 use super::error::parse_io_error;
 use super::pager::FsPager;
 use super::writer::FsWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// POSIX file system support.
-///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [x] copy
-/// - [x] rename
-/// - [x] list
-/// - [ ] ~~scan~~
-/// - [ ] ~~presign~~
-/// - [x] blocking
-///
-/// # Configuration
-///
-/// - `root`: Set the work dir for backend.
-///
-/// Refer to [`FsBuilder`]'s public API docs for more information.
-///
-/// # Example
-///
-/// ## Via Builder
-///
-/// ```
-/// use std::sync::Arc;
-///
-/// use anyhow::Result;
-/// use opendal::services::Fs;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     // Create fs backend builder.
-///     let mut builder = Fs::default();
-///     // Set the root for fs, all operations will happen under this root.
-///     //
-///     // NOTE: the root must be absolute path.
-///     builder.root("/tmp");
-///
-///     // `Accessor` provides the low level APIs, we will use `Operator` normally.
-///     let op: Operator = Operator::new(builder)?.finish();
-///
-///     Ok(())
-/// }
-/// ```
+#[doc = include_str!("docs.md")]
 #[derive(Default, Debug)]
 pub struct FsBuilder {
     root: Option<PathBuf>,
     atomic_write_dir: Option<PathBuf>,
     enable_path_check: bool,
 }
 
@@ -292,15 +244,15 @@
 
 #[async_trait]
 impl Accessor for FsBackend {
     type Reader = oio::into_reader::FdReader<Compat<tokio::fs::File>>;
     type BlockingReader = oio::into_blocking_reader::FdReader<std::fs::File>;
     type Writer = FsWriter<tokio::fs::File>;
     type BlockingWriter = FsWriter<std::fs::File>;
-    type Appender = ();
+    type Appender = FsAppender<tokio::fs::File>;
     type Pager = Option<FsPager<tokio::fs::ReadDir>>;
     type BlockingPager = Option<FsPager<std::fs::ReadDir>>;
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Fs)
             .set_root(&self.root.to_string_lossy())
@@ -312,14 +264,16 @@
                 read_with_range: true,
 
                 write: true,
                 write_without_content_length: true,
                 create_dir: true,
                 delete: true,
 
+                append: true,
+
                 list: true,
                 list_with_delimiter_slash: true,
 
                 copy: true,
                 rename: true,
                 blocking: true,
 
@@ -430,14 +384,28 @@
             .open(tmp_path.as_ref().unwrap_or(&target_path))
             .await
             .map_err(parse_io_error)?;
 
         Ok((RpWrite::new(), FsWriter::new(target_path, tmp_path, f)))
     }
 
+    async fn append(&self, path: &str, _: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        let path = Self::ensure_write_abs_path(&self.root, path).await?;
+
+        let f = tokio::fs::OpenOptions::new()
+            .create(true)
+            .write(true)
+            .append(true)
+            .open(&path)
+            .await
+            .map_err(parse_io_error)?;
+
+        Ok((RpAppend::new(), FsAppender::new(f)))
+    }
+
     async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
         let from = self.root.join(from.trim_end_matches('/'));
 
         // try to get the metadata of the source file to ensure it exists
         tokio::fs::metadata(&from).await.map_err(parse_io_error)?;
 
         let to = Self::ensure_write_abs_path(&self.root, to.trim_end_matches('/')).await?;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/fs/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/fs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/fs/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/redis/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -12,12 +12,8 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::FsBuilder as Fs;
-
-mod error;
-mod pager;
-mod writer;
+pub use backend::RedisBuilder as Redis;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/fs/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/fs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/fs/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/fs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ftp/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ftp/backend.rs`

 * *Files 12% similar despite different names*

```diff
@@ -37,67 +37,20 @@
 use suppaftp::FtpStream;
 use suppaftp::Status;
 use tokio::sync::OnceCell;
 
 use super::pager::FtpPager;
 use super::util::FtpReader;
 use super::writer::FtpWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// FTP and FTPS services support.
 ///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [ ] copy
-/// - [ ] rename
-/// - [x] list
-/// - [ ] ~~scan~~
-/// - [ ] ~~presign~~
-/// - [ ] blocking
-///
-/// # Configuration
-///
-/// - `endpoint`: Set the endpoint for connection
-/// - `root`: Set the work directory for backend
-/// - `user`: Set the login user
-/// - `password`: Set the login password
-///
-/// You can refer to [`FtpBuilder`]'s docs for more information
-///
-/// # Example
-///
-/// ## Via Builder
-///
-/// ```no_run
-/// use anyhow::Result;
-/// use opendal::services::Ftp;
-/// use opendal::Object;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     // create backend builder
-///     let mut builder = Ftp::default();
-///
-///     builder.endpoint("127.0.0.1");
-///
-///     let op: Operator = Operator::new(builder)?.finish();
-///     let _obj: Object = op.object("test_file");
-///     Ok(())
-/// }
-/// ```
+#[doc = include_str!("docs.md")]
 #[derive(Default)]
 pub struct FtpBuilder {
     endpoint: Option<String>,
     root: Option<String>,
     user: Option<String>,
     password: Option<String>,
 }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ftp/err.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ftp/err.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ftp/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ftp/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ftp/util.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ftp/util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ftp/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ftp/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gcs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 use serde::Deserialize;
 use serde_json;
 
 use super::core::GcsCore;
 use super::error::parse_error;
 use super::pager::GcsPager;
 use super::writer::GcsWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 const DEFAULT_GCS_ENDPOINT: &str = "https://storage.googleapis.com";
 const DEFAULT_GCS_SCOPE: &str = "https://www.googleapis.com/auth/devstorage.read_write";
 /// It's recommended that you use at least 8 MiB for the chunk size.
 const DEFAULT_WRITE_FIXED_SIZE: usize = 8 * 1024 * 1024;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/core.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/azblob/core.rs`

 * *Files 24% similar despite different names*

```diff
@@ -11,341 +11,415 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::fmt;
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::fmt::Write;
 use std::time::Duration;
 
-use backon::ExponentialBuilder;
-use backon::Retryable;
-use bytes::Bytes;
-use bytes::BytesMut;
+use http::header::HeaderName;
 use http::header::CONTENT_LENGTH;
-use http::header::CONTENT_RANGE;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
+use http::HeaderValue;
 use http::Request;
 use http::Response;
-use once_cell::sync::Lazy;
-use reqsign::GoogleCredential;
-use reqsign::GoogleCredentialLoader;
-use reqsign::GoogleSigner;
-use reqsign::GoogleToken;
-use reqsign::GoogleTokenLoader;
+use reqsign::AzureStorageCredential;
+use reqsign::AzureStorageLoader;
+use reqsign::AzureStorageSigner;
 
-use super::uri::percent_encode_path;
 use crate::raw::*;
 use crate::*;
 
-pub struct GcsCore {
-    pub endpoint: String,
-    pub bucket: String,
-    pub root: String,
-
-    pub client: HttpClient,
-    pub signer: GoogleSigner,
-    pub token_loader: GoogleTokenLoader,
-    pub credential_loader: GoogleCredentialLoader,
+mod constants {
+    pub const X_MS_VERSION: &str = "x-ms-version";
 
-    pub predefined_acl: Option<String>,
-    pub default_storage_class: Option<String>,
+    pub const X_MS_BLOB_TYPE: &str = "x-ms-blob-type";
+    pub const X_MS_COPY_SOURCE: &str = "x-ms-copy-source";
+    pub const X_MS_BLOB_CACHE_CONTROL: &str = "x-ms-blob-cache-control";
+    pub const X_MS_BLOB_CONDITION_APPENDPOS: &str = "x-ms-blob-condition-appendpos";
+
+    // Server-side encryption with customer-provided headers
+    pub const X_MS_ENCRYPTION_KEY: &str = "x-ms-encryption-key";
+    pub const X_MS_ENCRYPTION_KEY_SHA256: &str = "x-ms-encryption-key-sha256";
+    pub const X_MS_ENCRYPTION_ALGORITHM: &str = "x-ms-encryption-algorithm";
+}
 
-    pub write_fixed_size: usize,
+pub struct AzblobCore {
+    pub container: String,
+    pub root: String,
+    pub endpoint: String,
+    pub encryption_key: Option<HeaderValue>,
+    pub encryption_key_sha256: Option<HeaderValue>,
+    pub encryption_algorithm: Option<HeaderValue>,
+    pub client: HttpClient,
+    pub loader: AzureStorageLoader,
+    pub signer: AzureStorageSigner,
 }
 
-impl Debug for GcsCore {
-    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-        let mut de = f.debug_struct("Backend");
-        de.field("endpoint", &self.endpoint)
-            .field("bucket", &self.bucket)
+impl Debug for AzblobCore {
+    fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
+        f.debug_struct("AzblobCore")
+            .field("container", &self.container)
             .field("root", &self.root)
+            .field("endpoint", &self.endpoint)
             .finish_non_exhaustive()
     }
 }
 
-static BACKOFF: Lazy<ExponentialBuilder> =
-    Lazy::new(|| ExponentialBuilder::default().with_jitter());
-
-impl GcsCore {
-    async fn load_token(&self) -> Result<GoogleToken> {
-        let cred = { || self.token_loader.load() }
-            .retry(&*BACKOFF)
+impl AzblobCore {
+    async fn load_credential(&self) -> Result<AzureStorageCredential> {
+        let cred = self
+            .loader
+            .load()
             .await
             .map_err(new_request_credential_error)?;
 
         if let Some(cred) = cred {
             Ok(cred)
         } else {
             Err(Error::new(
                 ErrorKind::ConfigInvalid,
                 "no valid credential found",
             ))
         }
     }
 
-    fn load_credential(&self) -> Result<GoogleCredential> {
-        let cred = self
-            .credential_loader
-            .load()
-            .map_err(new_request_credential_error)?;
+    pub async fn sign_query<T>(&self, req: &mut Request<T>) -> Result<()> {
+        let cred = self.load_credential().await?;
 
-        if let Some(cred) = cred {
-            Ok(cred)
-        } else {
-            Err(Error::new(
-                ErrorKind::ConfigInvalid,
-                "no valid credential found",
-            ))
-        }
+        self.signer
+            .sign_query(req, Duration::from_secs(3600), &cred)
+            .map_err(new_request_sign_error)
     }
 
     pub async fn sign<T>(&self, req: &mut Request<T>) -> Result<()> {
-        let cred = self.load_token().await?;
-
+        let cred = self.load_credential().await?;
+        // Insert x-ms-version header for normal requests.
+        req.headers_mut().insert(
+            HeaderName::from_static(constants::X_MS_VERSION),
+            // 2022-11-02 is the version supported by Azurite V3 and
+            // used by Azure Portal, We use this version to make
+            // sure most our developer happy.
+            //
+            // In the future, we could allow users to configure this value.
+            HeaderValue::from_static("2022-11-02"),
+        );
         self.signer.sign(req, &cred).map_err(new_request_sign_error)
     }
 
-    pub async fn sign_query<T>(&self, req: &mut Request<T>, duration: Duration) -> Result<()> {
-        let cred = self.load_credential()?;
-
-        self.signer
-            .sign_query(req, duration, &cred)
-            .map_err(new_request_sign_error)
+    async fn batch_sign<T>(&self, req: &mut Request<T>) -> Result<()> {
+        let cred = self.load_credential().await?;
+        self.signer.sign(req, &cred).map_err(new_request_sign_error)
     }
 
     #[inline]
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
         self.client.send(req).await
     }
-}
 
-impl GcsCore {
-    pub fn gcs_get_object_request(
-        &self,
-        path: &str,
-        range: BytesRange,
-        if_match: Option<&str>,
-        if_none_match: Option<&str>,
-    ) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
+    pub fn insert_sse_headers(&self, mut req: http::request::Builder) -> http::request::Builder {
+        if let Some(v) = &self.encryption_key {
+            let mut v = v.clone();
+            v.set_sensitive(true);
 
-        let url = format!(
-            "{}/storage/v1/b/{}/o/{}?alt=media",
-            self.endpoint,
-            self.bucket,
-            percent_encode_path(&p)
-        );
+            req = req.header(HeaderName::from_static(constants::X_MS_ENCRYPTION_KEY), v)
+        }
 
-        let mut req = Request::get(&url);
+        if let Some(v) = &self.encryption_key_sha256 {
+            let mut v = v.clone();
+            v.set_sensitive(true);
 
-        if let Some(if_match) = if_match {
-            req = req.header(IF_MATCH, if_match);
-        }
-        if let Some(if_none_match) = if_none_match {
-            req = req.header(IF_NONE_MATCH, if_none_match);
-        }
-        if !range.is_full() {
-            req = req.header(http::header::RANGE, range.to_header());
+            req = req.header(
+                HeaderName::from_static(constants::X_MS_ENCRYPTION_KEY_SHA256),
+                v,
+            )
         }
 
-        let req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
+        if let Some(v) = &self.encryption_algorithm {
+            let mut v = v.clone();
+            v.set_sensitive(true);
+
+            req = req.header(
+                HeaderName::from_static(constants::X_MS_ENCRYPTION_ALGORITHM),
+                v,
+            )
+        }
 
-        Ok(req)
+        req
     }
+}
 
-    // It's for presign operation. Gcs only supports query sign over XML API.
-    pub fn gcs_get_object_xml_request(
+impl AzblobCore {
+    pub fn azblob_get_blob_request(
         &self,
         path: &str,
         range: BytesRange,
-        if_match: Option<&str>,
         if_none_match: Option<&str>,
+        if_match: Option<&str>,
+        override_content_disposition: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
-        let url = format!("{}/{}/{}", self.endpoint, self.bucket, p);
+        let mut url = format!(
+            "{}/{}/{}",
+            self.endpoint,
+            self.container,
+            percent_encode_path(&p)
+        );
+
+        let mut query_args = Vec::new();
+        if let Some(override_content_disposition) = override_content_disposition {
+            query_args.push(format!(
+                "rscd={}",
+                percent_encode_path(override_content_disposition)
+            ))
+        }
+
+        if !query_args.is_empty() {
+            url.push_str(&format!("?{}", query_args.join("&")));
+        }
 
         let mut req = Request::get(&url);
 
-        if let Some(if_match) = if_match {
-            req = req.header(IF_MATCH, if_match);
+        // Set SSE headers.
+        req = self.insert_sse_headers(req);
+
+        if !range.is_full() {
+            // azblob doesn't support read with suffix range.
+            //
+            // ref: https://learn.microsoft.com/en-us/rest/api/storageservices/specifying-the-range-header-for-blob-service-operations
+            if range.offset().is_none() && range.size().is_some() {
+                return Err(Error::new(
+                    ErrorKind::Unsupported,
+                    "azblob doesn't support read with suffix range",
+                ));
+            }
+
+            req = req.header(http::header::RANGE, range.to_header());
         }
+
         if let Some(if_none_match) = if_none_match {
             req = req.header(IF_NONE_MATCH, if_none_match);
         }
-        if !range.is_full() {
-            req = req.header(http::header::RANGE, range.to_header());
+
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn gcs_get_object(
+    pub async fn azblob_get_blob(
         &self,
         path: &str,
         range: BytesRange,
-        if_match: Option<&str>,
         if_none_match: Option<&str>,
+        if_match: Option<&str>,
+        override_content_disposition: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.gcs_get_object_request(path, range, if_match, if_none_match)?;
+        let mut req = self.azblob_get_blob_request(
+            path,
+            range,
+            if_none_match,
+            if_match,
+            override_content_disposition,
+        )?;
 
         self.sign(&mut req).await?;
+
         self.send(req).await
     }
 
-    pub fn gcs_insert_object_request(
+    pub fn azblob_put_blob_request(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
+        cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
-        let mut url = format!(
-            "{}/upload/storage/v1/b/{}/o?uploadType={}&name={}",
+        let url = format!(
+            "{}/{}/{}",
             self.endpoint,
-            self.bucket,
-            if self.default_storage_class.is_some() {
-                "multipart"
-            } else {
-                "media"
-            },
+            self.container,
             percent_encode_path(&p)
         );
 
-        if let Some(acl) = &self.predefined_acl {
-            write!(&mut url, "&predefinedAcl={}", acl).unwrap();
-        }
-
-        let mut req = Request::post(&url);
-
-        req = req.header(CONTENT_LENGTH, size.unwrap_or_default());
+        let mut req = Request::put(&url);
 
-        if let Some(storage_class) = &self.default_storage_class {
-            req = req.header(CONTENT_TYPE, "multipart/related; boundary=my-boundary");
+        // Set SSE headers.
+        req = self.insert_sse_headers(req);
 
-            let mut req_body = BytesMut::with_capacity(100);
-            write!(
-                &mut req_body,
-                "--my-boundary\nContent-Type: application/json; charset=UTF-8\n\n{{\"storageClass\": \"{}\"}}\n\n--my-boundary\n",
-                storage_class
-            ).unwrap();
+        if let Some(cache_control) = cache_control {
+            req = req.header(constants::X_MS_BLOB_CACHE_CONTROL, cache_control);
+        }
+        if let Some(size) = size {
+            req = req.header(CONTENT_LENGTH, size)
+        }
 
-            if let Some(mime) = content_type {
-                write!(&mut req_body, "Content-Type: {}\n\n", mime).unwrap();
-            } else {
-                write!(&mut req_body, "Content-Type: application/octet-stream\n\n").unwrap();
-            }
+        if let Some(ty) = content_type {
+            req = req.header(CONTENT_TYPE, ty)
+        }
 
-            if let AsyncBody::Bytes(bytes) = body {
-                req_body.extend_from_slice(&bytes);
-            }
-            write!(&mut req_body, "\n--my-boundary").unwrap();
+        req = req.header(
+            HeaderName::from_static(constants::X_MS_BLOB_TYPE),
+            "BlockBlob",
+        );
 
-            let req_body = AsyncBody::Bytes(req_body.freeze());
-            let req = req.body(req_body).map_err(new_request_build_error)?;
-            Ok(req)
-        } else {
-            if let Some(content_type) = content_type {
-                req = req.header(CONTENT_TYPE, content_type);
-            }
+        // Set body
+        let req = req.body(body).map_err(new_request_build_error)?;
 
-            let req = req.body(body).map_err(new_request_build_error)?;
-            Ok(req)
-        }
+        Ok(req)
     }
 
-    // It's for presign operation. Gcs only supports query sign over XML API.
-    pub fn gcs_insert_object_xml_request(
+    /// For appendable object, it could be created by `put` an empty blob
+    /// with `x-ms-blob-type` header set to `AppendBlob`.
+    /// And it's just initialized with empty content.
+    ///
+    /// If want to append content to it, we should use the following method `azblob_append_blob_request`.
+    ///
+    /// # Notes
+    ///
+    /// Appendable blob's custom header could only be set when it's created.
+    ///
+    /// The following custom header could be set:
+    /// - `content-type`
+    /// - `x-ms-blob-cache-control`
+    ///
+    /// # Reference
+    ///
+    /// https://learn.microsoft.com/en-us/rest/api/storageservices/put-blob
+    pub fn azblob_init_appendable_blob_request(
         &self,
         path: &str,
         content_type: Option<&str>,
-        body: AsyncBody,
+        cache_control: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
-        let url = format!("{}/{}/{}", self.endpoint, self.bucket, p);
+        let url = format!(
+            "{}/{}/{}",
+            self.endpoint,
+            self.container,
+            percent_encode_path(&p)
+        );
 
         let mut req = Request::put(&url);
 
-        if let Some(content_type) = content_type {
-            req = req.header(CONTENT_TYPE, content_type);
-        }
+        // Set SSE headers.
+        req = self.insert_sse_headers(req);
+
+        // The content-length header must be set to zero
+        // when creating an appendable blob.
+        req = req.header(CONTENT_LENGTH, 0);
+        req = req.header(
+            HeaderName::from_static(constants::X_MS_BLOB_TYPE),
+            "AppendBlob",
+        );
 
-        if let Some(acl) = &self.predefined_acl {
-            req = req.header("x-goog-acl", acl);
+        if let Some(ty) = content_type {
+            req = req.header(CONTENT_TYPE, ty)
         }
 
-        if let Some(storage_class) = &self.default_storage_class {
-            req = req.header("x-goog-storage-class", storage_class);
+        if let Some(cache_control) = cache_control {
+            req = req.header(constants::X_MS_BLOB_CACHE_CONTROL, cache_control);
         }
 
-        let req = req.body(body).map_err(new_request_build_error)?;
+        let req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub fn gcs_head_object_request(
+    /// Append content to an appendable blob.
+    /// The content will be appended to the end of the blob.
+    ///
+    /// # Notes
+    ///
+    /// - The maximum size of the content could be appended is 4MB.
+    /// - `Append Block` succeeds only if the blob already exists.
+    /// - It does not need to provide append position.
+    /// - But it could use append position to verify the content is appended to the right position.
+    ///
+    /// Since the `appendpos` only returned by the append operation response,
+    /// we could not use it when we want to append content to the blob first time.
+    /// (The first time of the appender, not the blob)
+    ///
+    /// # Reference
+    ///
+    /// https://learn.microsoft.com/en-us/rest/api/storageservices/append-block
+    pub fn azblob_append_blob_request(
         &self,
         path: &str,
-        if_match: Option<&str>,
-        if_none_match: Option<&str>,
+        size: usize,
+        position: Option<u64>,
+        body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
-            "{}/storage/v1/b/{}/o/{}",
+            "{}/{}/{}?comp=appendblock",
             self.endpoint,
-            self.bucket,
+            self.container,
             percent_encode_path(&p)
         );
 
-        let mut req = Request::get(&url);
+        let mut req = Request::put(&url);
 
-        if let Some(if_none_match) = if_none_match {
-            req = req.header(IF_NONE_MATCH, if_none_match);
-        }
+        // Set SSE headers.
+        req = self.insert_sse_headers(req);
 
-        if let Some(if_match) = if_match {
-            req = req.header(IF_MATCH, if_match);
+        req = req.header(CONTENT_LENGTH, size);
+
+        if let Some(pos) = position {
+            req = req.header(
+                HeaderName::from_static(constants::X_MS_BLOB_CONDITION_APPENDPOS),
+                pos.to_string(),
+            );
         }
 
-        let req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
+        let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    // It's for presign operation. Gcs only supports query sign over XML API.
-    pub fn gcs_head_object_xml_request(
+    pub fn azblob_head_blob_request(
         &self,
         path: &str,
-        if_match: Option<&str>,
         if_none_match: Option<&str>,
+        if_match: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
-        let url = format!("{}/{}/{}", self.endpoint, self.bucket, p);
+        let url = format!(
+            "{}/{}/{}",
+            self.endpoint,
+            self.container,
+            percent_encode_path(&p)
+        );
 
         let mut req = Request::head(&url);
 
+        // Set SSE headers.
+        req = self.insert_sse_headers(req);
+
         if let Some(if_none_match) = if_none_match {
             req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
         if let Some(if_match) = if_match {
             req = req.header(IF_MATCH, if_match);
         }
@@ -353,203 +427,136 @@
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn gcs_get_object_metadata(
+    pub async fn azblob_get_blob_properties(
         &self,
         path: &str,
-        if_match: Option<&str>,
         if_none_match: Option<&str>,
+        if_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.gcs_head_object_request(path, if_match, if_none_match)?;
+        let mut req = self.azblob_head_blob_request(path, if_none_match, if_match)?;
 
         self.sign(&mut req).await?;
-
         self.send(req).await
     }
 
-    pub async fn gcs_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    pub fn azblob_delete_blob_request(&self, path: &str) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
-            "{}/storage/v1/b/{}/o/{}",
+            "{}/{}/{}",
             self.endpoint,
-            self.bucket,
+            self.container,
             percent_encode_path(&p)
         );
 
-        let mut req = Request::delete(&url)
+        let req = Request::delete(&url);
+
+        req.header(CONTENT_LENGTH, 0)
             .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
+            .map_err(new_request_build_error)
+    }
 
-        self.sign(&mut req).await?;
+    pub async fn azblob_delete_blob(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.azblob_delete_blob_request(path)?;
 
+        self.sign(&mut req).await?;
         self.send(req).await
     }
 
-    pub async fn gcs_copy_object(
+    pub async fn azblob_copy_blob(
         &self,
         from: &str,
         to: &str,
     ) -> Result<Response<IncomingAsyncBody>> {
         let source = build_abs_path(&self.root, from);
-        let dest = build_abs_path(&self.root, to);
+        let target = build_abs_path(&self.root, to);
 
-        let req_uri = format!(
-            "{}/storage/v1/b/{}/o/{}/copyTo/b/{}/o/{}",
+        let source = format!(
+            "{}/{}/{}",
             self.endpoint,
-            self.bucket,
-            percent_encode_path(&source),
-            self.bucket,
-            percent_encode_path(&dest)
+            self.container,
+            percent_encode_path(&source)
+        );
+        let target = format!(
+            "{}/{}/{}",
+            self.endpoint,
+            self.container,
+            percent_encode_path(&target)
         );
 
-        let mut req = Request::post(req_uri)
+        let mut req = Request::put(&target)
+            .header(constants::X_MS_COPY_SOURCE, source)
             .header(CONTENT_LENGTH, 0)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
-    pub async fn gcs_list_objects(
+    pub async fn azblob_list_blobs(
         &self,
         path: &str,
-        page_token: &str,
+        next_marker: &str,
         delimiter: &str,
         limit: Option<usize>,
-        start_after: Option<String>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let mut url = format!(
-            "{}/storage/v1/b/{}/o?prefix={}",
-            self.endpoint,
-            self.bucket,
-            percent_encode_path(&p)
+            "{}/{}?restype=container&comp=list",
+            self.endpoint, self.container
         );
-        if !delimiter.is_empty() {
-            write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
+        if !p.is_empty() {
+            write!(url, "&prefix={}", percent_encode_path(&p))
+                .expect("write into string must succeed");
         }
         if let Some(limit) = limit {
-            write!(url, "&maxResults={limit}").expect("write into string must succeed");
+            write!(url, "&maxresults={limit}").expect("write into string must succeed");
         }
-        if let Some(start_after) = start_after {
-            let start_after = build_abs_path(&self.root, &start_after);
-            write!(url, "&startOffset={}", percent_encode_path(&start_after))
-                .expect("write into string must succeed");
+        if !delimiter.is_empty() {
+            write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
         }
-
-        if !page_token.is_empty() {
-            // NOTE:
-            //
-            // GCS uses pageToken in request and nextPageToken in response
-            //
-            // Don't know how will those tokens be like so this part are copied
-            // directly from AWS S3 service.
-            write!(url, "&pageToken={}", percent_encode_path(page_token))
-                .expect("write into string must succeed");
+        if !next_marker.is_empty() {
+            write!(url, "&marker={next_marker}").expect("write into string must succeed");
         }
 
         let mut req = Request::get(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
-
         self.send(req).await
     }
 
-    pub async fn gcs_initiate_resumable_upload(
+    pub async fn azblob_batch_delete(
         &self,
-        path: &str,
+        paths: &[String],
     ) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
         let url = format!(
-            "{}/upload/storage/v1/b/{}/o?uploadType=resumable&name={}",
-            self.endpoint, self.bucket, p
+            "{}/{}?restype=container&comp=batch",
+            self.endpoint, self.container
         );
 
-        let mut req = Request::post(&url)
-            .header(CONTENT_LENGTH, 0)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.sign(&mut req).await?;
-        self.send(req).await
-    }
-
-    pub fn gcs_upload_in_resumable_upload(
-        &self,
-        location: &str,
-        size: u64,
-        written: u64,
-        is_last_part: bool,
-        body: AsyncBody,
-    ) -> Result<Request<AsyncBody>> {
-        let mut req = Request::put(location);
-
-        let range_header = if is_last_part {
-            format!(
-                "bytes {}-{}/{}",
-                written,
-                written + size - 1,
-                written + size
-            )
-        } else {
-            format!("bytes {}-{}/*", written, written + size - 1)
-        };
+        let mut multipart = Multipart::new();
 
-        req = req
-            .header(CONTENT_LENGTH, size)
-            .header(CONTENT_RANGE, range_header);
+        for (idx, path) in paths.iter().enumerate() {
+            let mut req = self.azblob_delete_blob_request(path)?;
+            self.batch_sign(&mut req).await?;
 
-        // Set body
-        let req = req.body(body).map_err(new_request_build_error)?;
-
-        Ok(req)
-    }
-
-    pub async fn gcs_complete_resumable_upload(
-        &self,
-        location: &str,
-        written_bytes: u64,
-        bs: Bytes,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let size = bs.len() as u64;
-        let mut req = Request::post(location)
-            .header(CONTENT_LENGTH, size)
-            .header(
-                CONTENT_RANGE,
-                format!(
-                    "bytes {}-{}/{}",
-                    written_bytes,
-                    written_bytes + size - 1,
-                    written_bytes + size
-                ),
-            )
-            .body(AsyncBody::Bytes(bs))
-            .map_err(new_request_build_error)?;
-
-        self.sign(&mut req).await?;
-
-        self.send(req).await
-    }
+            multipart = multipart.part(
+                MixedPart::from_request(req).part_header("content-id".parse().unwrap(), idx.into()),
+            );
+        }
 
-    pub async fn gcs_abort_resumable_upload(
-        &self,
-        location: &str,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = Request::delete(location)
-            .header(CONTENT_LENGTH, 0)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
+        let req = Request::post(url);
+        let mut req = multipart.apply(req)?;
 
         self.sign(&mut req).await?;
-
         self.send(req).await
     }
 }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gcs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gcs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/uri.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gcs/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gcs/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
 use super::core::GcsCore;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct GcsWriter {
     core: Arc<GcsCore>,
     path: String,
     op: OpWrite,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gdrive/backend.rs`

 * *Files 14% similar despite different names*

```diff
@@ -20,25 +20,15 @@
 
 use async_trait::async_trait;
 use http::StatusCode;
 
 use super::core::GdriveCore;
 use super::error::parse_error;
 use super::writer::GdriveWriter;
-use crate::ops::OpDelete;
-use crate::ops::OpRead;
-use crate::ops::OpWrite;
-use crate::raw::parse_into_metadata;
-use crate::raw::Accessor;
-use crate::raw::AccessorInfo;
-use crate::raw::HttpClient;
-use crate::raw::IncomingAsyncBody;
-use crate::raw::RpDelete;
-use crate::raw::RpRead;
-use crate::raw::RpWrite;
+use crate::raw::*;
 use crate::types::Result;
 use crate::Capability;
 use crate::Error;
 use crate::ErrorKind;
 
 #[derive(Clone, Debug)]
 pub struct GdriveBackend {
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/builder.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gdrive/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/core.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gdrive/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gdrive/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gdrive/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/gdrive/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
 use super::core::GdriveCore;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct GdriveWriter {
     core: Arc<GdriveCore>,
     op: OpWrite,
     path: String,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ghac/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ghac/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 use http::StatusCode;
 use log::debug;
 use serde::Deserialize;
 use serde::Serialize;
 
 use super::error::parse_error;
 use super::writer::GhacWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// The base url for cache url.
 const CACHE_URL_BASE: &str = "_apis/artifactcache";
 /// Cache API requires to provide an accept header.
 const CACHE_HEADER_ACCEPT: &str = "application/json;api-version=6.0-preview.1";
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ghac/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ghac/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ghac/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ghac/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ghac/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ghac/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/hdfs/backend.rs`

 * *Files 18% similar despite different names*

```diff
@@ -25,121 +25,20 @@
 
 use async_trait::async_trait;
 use log::debug;
 
 use super::error::parse_io_error;
 use super::pager::HdfsPager;
 use super::writer::HdfsWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// [Hadoop Distributed File System (HDFS™)](https://hadoop.apache.org/) support.
 ///
-/// A distributed file system that provides high-throughput access to application data.
-///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [ ] copy
-/// - [ ] rename
-/// - [x] list
-/// - [ ] ~~scan~~
-/// - [ ] ~~presign~~
-/// - [x] blocking
-///
-/// # Differences with webhdfs
-///
-/// [Webhdfs][crate::services::Webhdfs] is powered by hdfs's RESTful HTTP API.
-///
-/// # Features
-///
-/// HDFS support needs to enable feature `services-hdfs`.
-///
-/// # Configuration
-///
-/// - `root`: Set the work dir for backend.
-/// - `name_node`: Set the name node for backend.
-///
-/// Refer to [`HdfsBuilder`]'s public API docs for more information.
-///
-/// # Environment
-///
-/// HDFS needs some environment set correctly.
-///
-/// - `JAVA_HOME`: the path to java home, could be found via `java -XshowSettings:properties -version`
-/// - `HADOOP_HOME`: the path to hadoop home, opendal relays on this env to discover hadoop jars and set `CLASSPATH` automatically.
-///
-/// Most of the time, setting `JAVA_HOME` and `HADOOP_HOME` is enough. But there are some edge cases:
-///
-/// - If meeting errors like the following:
-///
-/// ```shell
-/// error while loading shared libraries: libjvm.so: cannot open shared object file: No such file or directory
-/// ```
-///
-/// Java's lib are not including in pkg-config find path, please set `LD_LIBRARY_PATH`:
-///
-/// ```shell
-/// export LD_LIBRARY_PATH=${JAVA_HOME}/lib/server:${LD_LIBRARY_PATH}
-/// ```
-///
-/// The path of `libjvm.so` could be different, please keep an eye on it.
-///
-/// - If meeting errors like the following:
-///
-/// ```shell
-/// (unable to get stack trace for java.lang.NoClassDefFoundError exception: ExceptionUtils::getStackTrace error.)
-/// ```
-///
-/// `CLASSPATH` is not set correctly or your hadoop installation is incorrect.
-///
-/// To set `CLASSPATH`:
-/// ```shell
-/// export CLASSPATH=$(find $HADOOP_HOME -iname "*.jar" | xargs echo | tr ' ' ':'):${CLASSPATH}
-/// ```
-///
-/// # Example
-///
-/// ### Via Builder
-///
-/// ```no_run
-/// use std::sync::Arc;
-///
-/// use anyhow::Result;
-/// use opendal::services::Hdfs;
-/// use opendal::Object;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     // Create fs backend builder.
-///     let mut builder = Hdfs::default();
-///     // Set the name node for hdfs.
-///     builder.name_node("hdfs://127.0.0.1:9000");
-///     // Set the root for hdfs, all operations will happen under this root.
-///     //
-///     // NOTE: the root must be absolute path.
-///     builder.root("/tmp");
-///
-///     // `Accessor` provides the low level APIs, we will use `Operator` normally.
-///     let op: Operator = Operator::new(builder)?.finish();
-///
-///     // Create an object handle to start operation on object.
-///     let _: Object = op.object("test_file");
-///
-///     Ok(())
-/// }
-/// ```
+#[doc = include_str!("docs.md")]
 #[derive(Debug, Default)]
 pub struct HdfsBuilder {
     root: Option<String>,
     name_node: Option<String>,
 }
 
 impl HdfsBuilder {
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/hdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/hdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/hdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/hdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/http/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/http/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
 use http::StatusCode;
 use log::debug;
 
 use super::error::parse_error;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// HTTP Read-only service support like Nginx and Caddy.
 ///
 /// # Capabilities
 ///
@@ -530,17 +529,15 @@
             .await;
 
         let mut builder = HttpBuilder::default();
         builder.endpoint(&mock_server.uri());
         builder.root("/");
         let op = Operator::new(builder)?.finish();
 
-        let match_bs = op
-            .read_with("hello", OpRead::new().with_if_none_match("*"))
-            .await?;
+        let match_bs = op.read_with("hello").if_none_match("*").await?;
         assert_eq!(match_bs, b"Hello, World!");
 
         Ok(())
     }
 
     #[tokio::test]
     async fn test_stat_with() -> Result<()> {
@@ -554,16 +551,14 @@
             .mount(&mock_server)
             .await;
 
         let mut builder = HttpBuilder::default();
         builder.endpoint(&mock_server.uri());
         builder.root("/");
         let op = Operator::new(builder)?.finish();
-        let bs = op
-            .stat_with("hello", OpStat::new().with_if_none_match("*"))
-            .await?;
+        let bs = op.stat_with("hello").if_none_match("*").await?;
 
         assert_eq!(bs.mode(), EntryMode::FILE);
         assert_eq!(bs.content_length(), 128);
         Ok(())
     }
 }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/http/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/http/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/http/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/http/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ipfs/backend.rs`

 * *Files 4% similar despite different names*

```diff
@@ -25,71 +25,20 @@
 use http::Response;
 use http::StatusCode;
 use log::debug;
 use prost::Message;
 
 use super::error::parse_error;
 use super::ipld::PBNode;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// IPFS file system support based on [IPFS HTTP Gateway](https://docs.ipfs.tech/concepts/ipfs-gateway/).
 ///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [ ] ~~write~~
-/// - [ ] ~~create_dir~~
-/// - [ ] ~~delete~~
-/// - [ ] ~~copy~~
-/// - [ ] ~~rename~~
-/// - [x] list
-/// - [ ] ~~scan~~
-/// - [ ] presign
-/// - [ ] blocking
-///
-/// # Configuration
-///
-/// - `root`: Set the work directory for backend
-/// - `endpoint`: Customizable endpoint setting
-///
-/// You can refer to [`IpfsBuilder`]'s docs for more information
-///
-/// # Example
-///
-/// ## Via Builder
-///
-/// ```no_run
-/// use anyhow::Result;
-/// use opendal::services::Ipfs;
-/// use opendal::Object;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     // create backend builder
-///     let mut builder = Ipfs::default();
-///
-///     // set the endpoint for OpenDAL
-///     builder.endpoint("https://ipfs.io");
-///     // set the root for OpenDAL
-///     builder.root("/ipfs/QmPpCt1aYGb9JWJRmXRUnmJtVgeFFTJGzWFYEEX7bo9zGJ");
-///
-///     let op: Operator = Operator::new(builder)?.finish();
-///
-///     // Create an object handle to start operation on object.
-///     let _: Object = op.object("test_file");
-///
-///     Ok(())
-/// }
-/// ```
+#[doc = include_str!("docs.md")]
 #[derive(Default, Clone, Debug)]
 pub struct IpfsBuilder {
     endpoint: Option<String>,
     root: Option<String>,
     http_client: Option<HttpClient>,
 }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ipfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/ipld.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ipfs/ipld.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ipfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ipmfs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 use http::Response;
 use http::StatusCode;
 use serde::Deserialize;
 
 use super::error::parse_error;
 use super::pager::IpmfsPager;
 use super::writer::IpmfsWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Backend for IPFS service
 ///
 /// # Capabilities
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/builder.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ipmfs/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ipmfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ipmfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ipmfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/ipmfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/memcached/ascii.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/memcached/ascii.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/memcached/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/memcached/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -57,25 +57,23 @@
 /// # Example
 ///
 /// ## Via Builder
 ///
 /// ```no_run
 /// use anyhow::Result;
 /// use opendal::services::Memcached;
-/// use opendal::Object;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
 ///     let mut builder = Memcached::default();
 ///
 ///     builder.endpoint("tcp://127.0.0.1:11211");
 ///
 ///     let op: Operator = Operator::new(builder)?.finish();
-///     let _: Object = op.object("test_file");
 ///     Ok(())
 /// }
 /// ```
 #[derive(Clone, Default)]
 pub struct MemcachedBuilder {
     /// network address of the memcached service.
     ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/memcached/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/memcached/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/memory/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/memory/backend.rs`

 * *Files 8% similar despite different names*

```diff
@@ -23,29 +23,15 @@
 use parking_lot::Mutex;
 
 use crate::raw::adapters::typed_kv;
 use crate::*;
 
 /// In memory service support. (BTreeMap Based)
 ///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [ ] copy
-/// - [ ] rename
-/// - [ ] list
-/// - [x] scan
-/// - [ ] presign
-/// - [ ] blocking
+#[doc = include_str!("docs.md")]
 #[derive(Default)]
 pub struct MemoryBuilder {
     root: Option<String>,
 }
 
 impl MemoryBuilder {
     /// Set the root for BTreeMap.
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/memory/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/memory/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/moka/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/moka/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/moka/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/obs/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/obs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 use reqsign::HuaweicloudObsCredentialLoader;
 use reqsign::HuaweicloudObsSigner;
 
 use super::core::ObsCore;
 use super::error::parse_error;
 use super::pager::ObsPager;
 use super::writer::ObsWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Huawei Cloud OBS services support.
 ///
 /// # Capabilities
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/obs/core.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/obs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/obs/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/obs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/obs/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/obs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/obs/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/obs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/obs/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/obs/writer.rs`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
 use super::core::ObsCore;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct ObsWriter {
     core: Arc<ObsCore>,
 
     op: OpWrite,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/backend.rs`

 * *Files 13% similar despite different names*

```diff
@@ -27,48 +27,16 @@
 use super::error::parse_error;
 use super::graph_model::CreateDirPayload;
 use super::graph_model::ItemType;
 use super::graph_model::OneDriveUploadSessionCreationRequestBody;
 use super::graph_model::OnedriveGetItemBody;
 use super::pager::OnedrivePager;
 use super::writer::OneDriveWriter;
-use crate::ops::OpCreateDir;
-use crate::ops::OpDelete;
-use crate::ops::OpList;
-use crate::ops::OpRead;
-use crate::ops::OpStat;
-use crate::ops::OpWrite;
-use crate::raw::build_abs_path;
-use crate::raw::build_rooted_abs_path;
-use crate::raw::get_basename;
-use crate::raw::get_parent;
-use crate::raw::new_json_deserialize_error;
-use crate::raw::new_json_serialize_error;
-use crate::raw::new_request_build_error;
-use crate::raw::parse_datetime_from_rfc3339;
-use crate::raw::parse_into_metadata;
-use crate::raw::parse_location;
-use crate::raw::percent_encode_path;
-use crate::raw::Accessor;
-use crate::raw::AccessorInfo;
-use crate::raw::AsyncBody;
-use crate::raw::HttpClient;
-use crate::raw::IncomingAsyncBody;
-use crate::raw::RpCreateDir;
-use crate::raw::RpDelete;
-use crate::raw::RpList;
-use crate::raw::RpRead;
-use crate::raw::RpStat;
-use crate::raw::RpWrite;
-use crate::types::Result;
-use crate::Capability;
-use crate::EntryMode;
-use crate::Error;
-use crate::ErrorKind;
-use crate::Metadata;
+use crate::raw::*;
+use crate::*;
 
 #[derive(Clone)]
 pub struct OnedriveBackend {
     root: String,
     access_token: String,
     client: HttpClient,
 }
@@ -121,39 +89,21 @@
     }
 
     async fn read(&self, path: &str, _args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let resp = self.onedrive_get_content(path).await?;
 
         let status = resp.status();
 
-        if status.is_redirection() {
-            let headers = resp.headers();
-            let location = parse_location(headers)?;
-            match location {
-                None => {
-                    return Err(Error::new(
-                        ErrorKind::ContentIncomplete,
-                        "redirect location not found in response",
-                    ));
-                }
-                Some(location) => {
-                    let resp = self.onedrive_get_redirection(location).await?;
-                    let meta = parse_into_metadata(path, resp.headers())?;
-                    Ok((RpRead::with_metadata(meta), resp.into_body()))
-                }
+        match status {
+            StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
+                let meta = parse_into_metadata(path, resp.headers())?;
+                Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
-        } else {
-            match status {
-                StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
-                    let meta = parse_into_metadata(path, resp.headers())?;
-                    Ok((RpRead::with_metadata(meta), resp.into_body()))
-                }
 
-                _ => Err(parse_error(resp).await?),
-            }
+            _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         if args.content_length().is_none() {
             return Err(Error::new(
                 ErrorKind::Unsupported,
@@ -303,27 +253,14 @@
 
         let auth_header_content = format!("Bearer {}", self.access_token);
         req = req.header(header::AUTHORIZATION, auth_header_content);
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
-
-        self.client.send(req).await
-    }
-
-    async fn onedrive_get_redirection(&self, url: &str) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = Request::get(url);
-
-        let auth_header_content = format!("Bearer {}", self.access_token);
-        req = req.header(header::AUTHORIZATION, auth_header_content);
-
-        let req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
 
         self.client.send(req).await
     }
 
     pub async fn onedrive_upload_simple(
         &self,
         path: &str,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/builder.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/graph_model.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/graph_model.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/onedrive/writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 use bytes::Bytes;
 use http::StatusCode;
 
 use super::backend::OnedriveBackend;
 use super::error::parse_error;
 use super::graph_model::OneDriveUploadSessionCreationRequestBody;
 use super::graph_model::OneDriveUploadSessionCreationResponseBody;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct OneDriveWriter {
     backend: OnedriveBackend,
 
     op: OpWrite,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/oss/appender.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/oss/appender.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
 use super::core::*;
 use super::error::parse_error;
-use crate::ops::OpAppend;
 use crate::raw::*;
 use crate::*;
 
 pub const X_OSS_NEXT_APPEND_POSITION: &str = "x-oss-next-append-position";
 
 pub struct OssAppender {
     core: Arc<OssCore>,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/oss/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/oss/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -31,28 +31,28 @@
 use reqsign::AliyunOssSigner;
 
 use super::appender::OssAppender;
 use super::core::*;
 use super::error::parse_error;
 use super::pager::OssPager;
 use super::writer::OssWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 const DEFAULT_WRITE_MIN_SIZE: usize = 8 * 1024 * 1024;
 /// Aliyun Object Storage Service (OSS) support
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] stat
 /// - [x] read
 /// - [x] write
+/// - [x] append
 /// - [x] create_dir
 /// - [x] delete
 /// - [x] copy
 /// - [ ] rename
 /// - [x] list
 /// - [x] scan
 /// - [x] presign
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/oss/core.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/oss/core.rs`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 use http::Response;
 use reqsign::AliyunCredential;
 use reqsign::AliyunLoader;
 use reqsign::AliyunOssSigner;
 use serde::Deserialize;
 use serde::Serialize;
 
-use crate::ops::OpAppend;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 mod constants {
     pub const X_OSS_SERVER_SIDE_ENCRYPTION: &str = "x-oss-server-side-encryption";
 
     pub const X_OSS_SERVER_SIDE_ENCRYPTION_KEY_ID: &str = "x-oss-server-side-encryption-key-id";
@@ -183,22 +181,14 @@
         // set sse headers
         req = self.insert_sse_headers(req);
 
         let req = req.body(body).map_err(new_request_build_error)?;
         Ok(req)
     }
 
-    /// Oss append object request
-    ///
-    /// # Note
-    ///
-    /// This request is used to append data to an existing object or create an appendable object.
-    /// So we must set the `append` and `position` header.
-    ///
-    /// https://www.alibabacloud.com/help/object-storage-service/latest/appendobject
     pub fn oss_append_object_request(
         &self,
         path: &str,
         position: u64,
         size: usize,
         args: &OpAppend,
         body: AsyncBody,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/oss/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/oss/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/oss/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/oss/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/oss/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/oss/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/oss/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/oss/writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 use async_trait::async_trait;
 use bytes::Buf;
 use bytes::Bytes;
 use http::StatusCode;
 
 use super::core::*;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct OssWriter {
     core: Arc<OssCore>,
 
     op: OpWrite,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/redis/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/redis/backend.rs`

 * *Files 11% similar despite different names*

```diff
@@ -37,60 +37,15 @@
 use crate::*;
 
 const DEFAULT_REDIS_ENDPOINT: &str = "tcp://127.0.0.1:6379";
 const DEFAULT_REDIS_PORT: u16 = 6379;
 
 /// [Redis](https://redis.io/) services support.
 ///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [ ] copy
-/// - [ ] rename
-/// - [ ] ~~list~~
-/// - [ ] scan
-/// - [ ] ~~presign~~
-/// - [ ] blocking
-///
-/// # Configuration
-///
-/// - `root`: Set the working directory of `OpenDAL`
-/// - `endpoint`: Set the network address of redis server
-/// - `username`: Set the username of Redis
-/// - `password`: Set the password for authentication
-/// - `db`: Set the DB of redis
-///
-/// You can refer to [`RedisBuilder`]'s docs for more information
-///
-/// # Example
-///
-/// ## Via Builder
-///
-/// ```no_run
-/// use anyhow::Result;
-/// use opendal::services::Redis;
-/// use opendal::Object;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     let mut builder = Redis::default();
-///
-///     // this will build a Operator accessing Redis which runs on tcp://localhost:6379
-///     let op: Operator = Operator::new(builder)?.finish();
-///     let _: Object = op.object("test_file");
-///     Ok(())
-/// }
-/// ```
+#[doc = include_str!("docs.md")]
 #[derive(Clone, Default)]
 pub struct RedisBuilder {
     /// network address of the Redis service. Can be "tcp://127.0.0.1:6379", e.g.
     ///
     /// default is "tcp://127.0.0.1:6379"
     endpoint: Option<String>,
     /// the username to connect redis service.
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/redis/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/sled/mod.rs`

 * *Files 13% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::RedisBuilder as Redis;
+
+pub use backend::SledBuilder as Sled;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/rocksdb/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/rocksdb/backend.rs`

 * *Files 24% similar despite different names*

```diff
@@ -23,73 +23,17 @@
 use async_trait::async_trait;
 use rocksdb::DB;
 
 use crate::raw::adapters::kv;
 use crate::Result;
 use crate::*;
 
-/// Rocksdb service support.
+/// RocksDB service support.
 ///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [ ] copy
-/// - [ ] rename
-/// - [ ] ~~list~~
-/// - [x] scan
-/// - [ ] ~~presign~~
-/// - [x] blocking
-///
-/// # Note
-///
-/// OpenDAL will build rocksdb from source by default.
-///
-/// To link with existing rocksdb lib, please set one of the following:
-///
-/// - `ROCKSDB_LIB_DIR` to the dir that contains `librocksdb.so`
-/// - `ROCKSDB_STATIC` to the dir that contains `librocksdb.a`
-///
-/// If the version of RocksDB is below 6.0, you may encounter compatibility
-/// issues. It is advisable to follow the steps provided in the [`INSTALL`](https://github.com/facebook/rocksdb/blob/main/INSTALL.md)
-/// file to build rocksdb, rather than relying on system libraries that
-/// may be outdated and incompatible.
-///
-/// # Configuration
-///
-/// - `root`: Set the working directory of `OpenDAL`
-/// - `datadir`: Set the path to the rocksdb data directory
-///
-/// You can refer to [`RocksdbBuilder`]'s docs for more information
-///
-/// # Example
-///
-/// ## Via Builder
-///
-/// ```no_run
-/// use anyhow::Result;
-/// use opendal::services::Rocksdb;
-/// use opendal::Object;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     let mut builder = Rocksdb::default();
-///     builder.datadir("/tmp/opendal/rocksdb");
-///
-///     let op: Operator = Operator::new(builder)?.finish();
-///     let _: Object = op.object("test_file");
-///     Ok(())
-/// }
-/// ```
+#[doc = include_str!("docs.md")]
 #[derive(Clone, Default, Debug)]
 pub struct RocksdbBuilder {
     /// The path to the rocksdb data directory.
     datadir: Option<String>,
     /// the working directory of the service. Can be "/path/to/dir"
     ///
     /// default is "/"
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/rocksdb/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/rocksdb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/s3/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/wasabi/backend.rs`

 * *Files 3% similar despite different names*

```diff
@@ -33,47 +33,43 @@
 use reqsign::AwsConfig;
 use reqsign::AwsCredentialLoad;
 use reqsign::AwsLoader;
 use reqsign::AwsV4Signer;
 
 use super::core::*;
 use super::error::parse_error;
-use super::error::parse_s3_error_code;
-use super::pager::S3Pager;
-use super::writer::S3Writer;
-use crate::ops::*;
+use super::pager::WasabiPager;
+use super::writer::WasabiWriter;
 use crate::raw::*;
 use crate::*;
 
 /// Allow constructing correct region endpoint if user gives a global endpoint.
 static ENDPOINT_TEMPLATES: Lazy<HashMap<&'static str, &'static str>> = Lazy::new(|| {
     let mut m = HashMap::new();
     // AWS S3 Service.
     m.insert(
-        "https://s3.amazonaws.com",
-        "https://s3.{region}.amazonaws.com",
+        "https://s3.wasabisys.com",
+        "https://s3.{region}.wasabisys.com",
     );
     m
 });
 
-const DEFAULT_WRITE_MIN_SIZE: usize = 8 * 1024 * 1024;
-/// Aws S3 and compatible services (including minio, digitalocean space, Tencent Cloud Object Storage(COS) and so on) support.
-/// For more information about s3-compatible services, refer to [Compatible Services](#compatible-services).
+/// Wasabi (an aws S3 compatible service) support
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] stat
 /// - [x] read
 /// - [x] write
 /// - [x] create_dir
 /// - [x] delete
 /// - [x] copy
-/// - [ ] rename
+/// - [x] rename
 /// - [x] list
 /// - [x] scan
 /// - [x] presign
 /// - [ ] blocking
 ///
 /// # Configuration
 ///
@@ -89,15 +85,15 @@
 /// - `server_side_encryption_aws_kms_key_id`: Set the server_side_encryption_aws_kms_key_id for backend.
 /// - `server_side_encryption_customer_algorithm`: Set the server_side_encryption_customer_algorithm for backend.
 /// - `server_side_encryption_customer_key`: Set the server_side_encryption_customer_key for backend.
 /// - `server_side_encryption_customer_key_md5`: Set the server_side_encryption_customer_key_md5 for backend.
 /// - `disable_config_load`: Disable aws config load from env
 /// - `enable_virtual_host_style`: Enable virtual host style.
 ///
-/// Refer to [`S3Builder`]'s public API docs for more information.
+/// Refer to [`WasabiBuilder`]'s public API docs for more information.
 ///
 /// # Temporary security credentials
 ///
 /// OpenDAL now provides support for S3 temporary security credentials in IAM.
 ///
 /// The way to take advantage of this feature is to build your S3 backend with `Builder::security_token`.
 ///
@@ -136,62 +132,62 @@
 ///
 /// ## Basic Setup
 ///
 /// ```no_run
 /// use std::sync::Arc;
 ///
 /// use anyhow::Result;
-/// use opendal::services::S3;
+/// use opendal::services::Wasabi;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
 ///     // Create s3 backend builder.
-///     let mut builder = S3::default();
+///     let mut builder = Wasabi::default();
 ///     // Set the root for s3, all operations will happen under this root.
 ///     //
 ///     // NOTE: the root must be absolute path.
 ///     builder.root("/path/to/dir");
 ///     // Set the bucket name, this is required.
 ///     builder.bucket("test");
 ///     // Set the endpoint.
 ///     //
 ///     // For examples:
-///     // - "https://s3.amazonaws.com"
+///     // - "https://s3.wasabisys.com"
 ///     // - "http://127.0.0.1:9000"
 ///     // - "https://oss-ap-northeast-1.aliyuncs.com"
 ///     // - "https://cos.ap-seoul.myqcloud.com"
 ///     //
-///     // Default to "https://s3.amazonaws.com"
-///     builder.endpoint("https://s3.amazonaws.com");
+///     // Default to "https://s3.wasabisys.com"
+///     builder.endpoint("https://s3.wasabisys.com");
 ///     // Set the access_key_id and secret_access_key.
 ///     //
 ///     // OpenDAL will try load credential from the env.
 ///     // If credential not set and no valid credential in env, OpenDAL will
 ///     // send request without signing like anonymous user.
 ///     builder.access_key_id("access_key_id");
 ///     builder.secret_access_key("secret_access_key");
 ///
 ///     let op: Operator = Operator::new(builder)?.finish();
 ///
 ///     Ok(())
 /// }
 /// ```
 ///
-/// ## S3 with SSE-C
+/// ## Wasabi with SSE-C
 ///
 /// ```no_run
 /// use anyhow::Result;
 /// use log::info;
-/// use opendal::services::S3;
+/// use opendal::services::Wasabi;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
-///     let mut builder = S3::default();
+///     let mut builder = Wasabi::default();
 ///
 ///     // Setup builders
 ///
 ///     // Enable SSE-C
 ///     builder.server_side_encryption_with_customer_key("AES256", "customer_key".as_bytes());
 ///
 ///     let op = Operator::new(builder)?.finish();
@@ -199,25 +195,25 @@
 ///
 ///     // Writing your testing code here.
 ///
 ///     Ok(())
 /// }
 /// ```
 ///
-/// ## S3 with SSE-KMS and aws managed kms key
+/// ## Wasabi with SSE-KMS and aws managed kms key
 ///
 /// ```no_run
 /// use anyhow::Result;
 /// use log::info;
-/// use opendal::services::S3;
+/// use opendal::services::Wasabi;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
-///     let mut builder = S3::default();
+///     let mut builder = Wasabi::default();
 ///
 ///     // Setup builders
 ///
 ///     // Enable SSE-KMS with aws managed kms key
 ///     builder.server_side_encryption_with_aws_managed_kms_key();
 ///
 ///     let op = Operator::new(builder)?.finish();
@@ -225,25 +221,25 @@
 ///
 ///     // Writing your testing code here.
 ///
 ///     Ok(())
 /// }
 /// ```
 ///
-/// ## S3 with SSE-KMS and customer managed kms key
+/// ## Wasabi with SSE-KMS and customer managed kms key
 ///
 /// ```no_run
 /// use anyhow::Result;
 /// use log::info;
-/// use opendal::services::S3;
+/// use opendal::services::Wasabi;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
-///     let mut builder = S3::default();
+///     let mut builder = Wasabi::default();
 ///
 ///     // Setup builders
 ///
 ///     // Enable SSE-KMS with customer managed kms key
 ///     builder.server_side_encryption_with_customer_managed_kms_key("aws_kms_key_id");
 ///
 ///     let op = Operator::new(builder)?.finish();
@@ -251,44 +247,41 @@
 ///
 ///     // Writing your testing code here.
 ///
 ///     Ok(())
 /// }
 /// ```
 ///
-/// ## S3 with SSE-S3
+/// ## Wasabi with SSE-S3
 ///
 /// ```no_run
 /// use anyhow::Result;
 /// use log::info;
-/// use opendal::services::S3;
+/// use opendal::services::Wasabi;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
-///     let mut builder = S3::default();
+///     let mut builder = Wasabi::default();
 ///
 ///     // Setup builders
 ///
 ///     // Enable SSE-S3
 ///     builder.server_side_encryption_with_s3_key();
 ///
 ///     let op = Operator::new(builder)?.finish();
 ///     info!("operator: {:?}", op);
 ///
 ///     // Writing your testing code here.
 ///
 ///     Ok(())
 /// }
 /// ```
-///
-/// # Compatible Services
-#[doc = include_str!("compatible_services.md")]
 #[derive(Default)]
-pub struct S3Builder {
+pub struct WasabiBuilder {
     root: Option<String>,
 
     bucket: String,
     endpoint: Option<String>,
     region: Option<String>,
     role_arn: Option<String>,
     external_id: Option<String>,
@@ -302,39 +295,34 @@
     default_storage_class: Option<String>,
 
     /// temporary credentials, check the official [doc](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp.html) for detail
     security_token: Option<String>,
 
     disable_config_load: bool,
     disable_ec2_metadata: bool,
-    allow_anonymous: bool,
     enable_virtual_host_style: bool,
 
     http_client: Option<HttpClient>,
     customed_credential_load: Option<Box<dyn AwsCredentialLoad>>,
-
-    /// the part size of s3 multipart upload, which should be 5 MiB to 5 GiB.
-    /// There is no minimum size limit on the last part of your multipart upload
-    write_min_size: Option<usize>,
 }
 
-impl Debug for S3Builder {
+impl Debug for WasabiBuilder {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         let mut d = f.debug_struct("Builder");
 
         d.field("root", &self.root)
             .field("bucket", &self.bucket)
             .field("endpoint", &self.endpoint)
             .field("region", &self.region);
 
         d.finish_non_exhaustive()
     }
 }
 
-impl S3Builder {
+impl WasabiBuilder {
     /// Set root of this backend.
     ///
     /// All operations will happen under this root.
     pub fn root(&mut self, root: &str) -> &mut Self {
         self.root = if root.is_empty() {
             None
         } else {
@@ -351,34 +339,29 @@
         self
     }
 
     /// Set endpoint of this backend.
     ///
     /// Endpoint must be full uri, e.g.
     ///
-    /// - AWS S3: `https://s3.amazonaws.com` or `https://s3.{region}.amazonaws.com`
-    /// - Aliyun OSS: `https://{region}.aliyuncs.com`
-    /// - Tencent COS: `https://cos.{region}.myqcloud.com`
-    /// - Minio: `http://127.0.0.1:9000`
+    /// - `https://s3.wasabisys.com` or `https://s3.{region}.wasabisys.com`
     ///
-    /// If user inputs endpoint without scheme like "s3.amazonaws.com", we
+    /// If user inputs endpoint without scheme like "s3.wasabisys.com", we
     /// will prepend "https://" before it.
     pub fn endpoint(&mut self, endpoint: &str) -> &mut Self {
         if !endpoint.is_empty() {
             // Trim trailing `/` so that we can accept `http://127.0.0.1:9000/`
             self.endpoint = Some(endpoint.trim_end_matches('/').to_string())
         }
 
         self
     }
 
-    /// Region represent the signing region of this endpoint. This is required
-    /// if you are using the default AWS S3 endpoint.
+    /// Region represent the signing region of this endpoint.
     ///
-    /// If using a custom endpoint,
     /// - If region is set, we will take user's input first.
     /// - If not, the default `us-east-1` will be used.
     pub fn region(&mut self, region: &str) -> &mut Self {
         if !region.is_empty() {
             self.region = Some(region.to_string())
         }
 
@@ -424,25 +407,20 @@
             self.external_id = Some(v.to_string())
         }
 
         self
     }
 
     /// Set default storage_class for this backend.
+    /// Unlike S3, wasabi only supports one single storage class,
+    /// which is most like standard S3 storage class,
+    /// check `https://docs.wasabi.com/docs/operations-on-objects` for more details.
     ///
     /// Available values:
-    /// - `DEEP_ARCHIVE`
-    /// - `GLACIER`
-    /// - `GLACIER_IR`
-    /// - `INTELLIGENT_TIERING`
-    /// - `ONEZONE_IA`
-    /// - `OUTPOSTS`
-    /// - `REDUCED_REDUNDANCY`
     /// - `STANDARD`
-    /// - `STANDARD_IA`
     pub fn default_storage_class(&mut self, v: &str) -> &mut Self {
         if !v.is_empty() {
             self.default_storage_class = Some(v.to_string())
         }
 
         self
     }
@@ -596,15 +574,15 @@
         self.server_side_encryption_customer_algorithm = Some(algorithm.to_string());
         self.server_side_encryption_customer_key = Some(BASE64_STANDARD.encode(key));
         self.server_side_encryption_customer_key_md5 =
             Some(BASE64_STANDARD.encode(Md5::digest(key).as_slice()));
         self
     }
 
-    /// Set temporary credential used in AWS S3 connections
+    /// Set temporary credential used in service connections
     ///
     /// # Warning
     ///
     /// security token's lifetime is short and requires users to refresh in time.
     pub fn security_token(&mut self, token: &str) -> &mut Self {
         if !token.is_empty() {
             self.security_token = Some(token.to_string());
@@ -629,26 +607,19 @@
     /// This option is used to disable the default behavior of opendal
     /// to load credential from ec2 metadata, a.k.a, IMDSv2
     pub fn disable_ec2_metadata(&mut self) -> &mut Self {
         self.disable_ec2_metadata = true;
         self
     }
 
-    /// Allow anonymous will allow opendal to send request without signing
-    /// when credentail is not loaded.
-    pub fn allow_anonymous(&mut self) -> &mut Self {
-        self.allow_anonymous = true;
-        self
-    }
-
     /// Enable virtual host style so that opendal will send API requests
     /// in virtual host style instead of path style.
     ///
-    /// - By default, opendal will send API to `https://s3.us-east-1.amazonaws.com/bucket_name`
-    /// - Enabled, opendal will send API to `https://bucket_name.s3.us-east-1.amazonaws.com`
+    /// - By default, opendal will send API to `https://s3.us-east-1.wasabisys.com/bucket_name`
+    /// - Enabled, opendal will send API to `https://bucket_name.s3.us-east-1.wasabisys.com`
     pub fn enable_virtual_host_style(&mut self) -> &mut Self {
         self.enable_virtual_host_style = true;
         self
     }
 
     /// Adding a customed credential load for service.
     pub fn customed_credential_load(&mut self, cred: Box<dyn AwsCredentialLoad>) -> &mut Self {
@@ -696,15 +667,15 @@
                 if endpoint.starts_with("http") {
                     endpoint.to_string()
                 } else {
                     // Prefix https if endpoint doesn't start with scheme.
                     format!("https://{endpoint}")
                 }
             }
-            None => "https://s3.amazonaws.com".to_string(),
+            None => "https://s3.wasabisys.com".to_string(),
         };
 
         // If endpoint contains bucket name, we should trim them.
         endpoint = endpoint.replace(&format!("//{bucket}."), "//");
 
         // Update with endpoint templates.
         endpoint = if let Some(template) = ENDPOINT_TEMPLATES.get(endpoint.as_str()) {
@@ -720,30 +691,22 @@
             endpoint = endpoint.replace("//", &format!("//{bucket}."))
         } else {
             write!(endpoint, "/{bucket}").expect("write into string must succeed");
         };
 
         endpoint
     }
-
-    /// set the minimum size of unsized write, it should be greater than 5 MB.
-    /// Reference: [Amazon S3 multipart upload limits](https://docs.aws.amazon.com/AmazonS3/latest/userguide/qfacts.html)
-    pub fn write_min_size(&mut self, write_min_size: usize) -> &mut Self {
-        self.write_min_size = Some(write_min_size);
-
-        self
-    }
 }
 
-impl Builder for S3Builder {
-    const SCHEME: Scheme = Scheme::S3;
-    type Accessor = S3Backend;
+impl Builder for WasabiBuilder {
+    const SCHEME: Scheme = Scheme::Wasabi;
+    type Accessor = WasabiBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
-        let mut builder = S3Builder::default();
+        let mut builder = WasabiBuilder::default();
 
         map.get("root").map(|v| builder.root(v));
         map.get("bucket").map(|v| builder.bucket(v));
         map.get("endpoint").map(|v| builder.endpoint(v));
         map.get("region").map(|v| builder.region(v));
         map.get("access_key_id").map(|v| builder.access_key_id(v));
         map.get("secret_access_key")
@@ -766,17 +729,14 @@
             .map(|_| builder.disable_config_load());
         map.get("disable_ec2_metadata")
             .filter(|v| *v == "on" || *v == "true")
             .map(|_| builder.disable_ec2_metadata());
         map.get("enable_virtual_host_style")
             .filter(|v| *v == "on" || *v == "true")
             .map(|_| builder.enable_virtual_host_style());
-        map.get("allow_anonymous")
-            .filter(|v| *v == "on" || *v == "true")
-            .map(|_| builder.allow_anonymous());
         map.get("default_storage_class")
             .map(|v| builder.default_storage_class(v));
 
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
@@ -875,26 +835,18 @@
             cfg.role_arn = Some(v)
         }
         if let Some(v) = self.external_id.take() {
             cfg.external_id = Some(v)
         }
 
         if cfg.region.is_none() {
-            // AWS S3 requires region to be set.
-            if self.endpoint.is_none()
-                || self.endpoint.as_deref() == Some("https://s3.amazonaws.com")
-            {
-                return Err(Error::new(ErrorKind::ConfigInvalid, "region is missing")
-                    .with_operation("Builder::build")
-                    .with_context("service", Scheme::S3));
-            }
-
-            // For other compatible services, if we don't know region
-            // after loading from builder and env, we can use `us-east-1`
-            // as default.
+            // region is required to make signer work.
+            //
+            // If we don't know region after loading from builder and env.
+            // We will use `us-east-1` as default.
             cfg.region = Some("us-east-1".to_string());
         }
 
         let region = cfg.region.to_owned().unwrap();
         debug!("backend use region: {region}");
 
         // Building endpoint.
@@ -906,111 +858,92 @@
             loader = loader.with_disable_ec2_metadata();
         }
         if let Some(v) = self.customed_credential_load.take() {
             loader = loader.with_customed_credential_loader(v);
         }
 
         let signer = AwsV4Signer::new("s3", &region);
-        let write_min_size = self.write_min_size.unwrap_or(DEFAULT_WRITE_MIN_SIZE);
-        if write_min_size < 5 * 1024 * 1024 {
-            return Err(Error::new(
-                ErrorKind::ConfigInvalid,
-                "The write minimum buffer size is misconfigured",
-            )
-            .with_context("service", Scheme::S3));
-        }
 
         debug!("backend build finished");
-        Ok(S3Backend {
-            core: Arc::new(S3Core {
+        Ok(WasabiBackend {
+            core: Arc::new(WasabiCore {
                 bucket: bucket.to_string(),
                 endpoint,
                 root,
                 server_side_encryption,
                 server_side_encryption_aws_kms_key_id,
                 server_side_encryption_customer_algorithm,
                 server_side_encryption_customer_key,
                 server_side_encryption_customer_key_md5,
                 default_storage_class,
-                allow_anonymous: self.allow_anonymous,
                 signer,
                 loader,
                 client,
-                write_min_size,
             }),
         })
     }
 }
 
-/// Backend for s3 services.
+/// Backend for wasabi service.
 #[derive(Debug, Clone)]
-pub struct S3Backend {
-    core: Arc<S3Core>,
+pub struct WasabiBackend {
+    core: Arc<WasabiCore>,
 }
 
 #[async_trait]
-impl Accessor for S3Backend {
+impl Accessor for WasabiBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
-    type Writer = S3Writer;
+    type Writer = WasabiWriter;
     type BlockingWriter = ();
     type Appender = ();
-    type Pager = S3Pager;
+    type Pager = WasabiPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
-        am.set_scheme(Scheme::S3)
+        am.set_scheme(Scheme::Wasabi)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
             .set_capability(Capability {
                 stat: true,
                 stat_with_if_match: true,
                 stat_with_if_none_match: true,
 
                 read: true,
                 read_can_next: true,
                 read_with_range: true,
-                read_with_if_match: true,
-                read_with_if_none_match: true,
-                read_with_override_cache_control: true,
-                read_with_override_content_disposition: true,
 
                 write: true,
-                write_with_cache_control: true,
-                write_with_content_type: true,
-                write_without_content_length: true,
                 create_dir: true,
                 delete: true,
                 copy: true,
+                rename: true,
 
                 list: true,
-                list_with_limit: true,
-                list_with_start_after: true,
                 list_without_delimiter: true,
                 list_with_delimiter_slash: true,
 
                 presign: true,
                 presign_stat: true,
                 presign_read: true,
                 presign_write: true,
 
                 batch: true,
-                batch_max_operations: Some(1000),
 
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreateDir) -> Result<RpCreateDir> {
         let mut req =
             self.core
-                .s3_put_object_request(path, Some(0), None, None, None, AsyncBody::Empty)?;
+                .put_object_request(path, Some(0), None, None, None, AsyncBody::Empty)?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         let status = resp.status();
 
@@ -1022,43 +955,44 @@
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let resp = self
             .core
-            .s3_get_object(
-                path,
-                args.range(),
-                args.if_none_match(),
-                args.if_match(),
-                args.override_content_disposition(),
-            )
+            .get_object(path, args.range(), args.if_none_match())
             .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
+        if args.content_length().is_none() {
+            return Err(Error::new(
+                ErrorKind::Unsupported,
+                "write without content length is not supported",
+            ));
+        }
+
         Ok((
             RpWrite::default(),
-            S3Writer::new(self.core.clone(), path, args),
+            WasabiWriter::new(self.core.clone(), args, path.to_string()),
         ))
     }
 
     async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
-        let resp = self.core.s3_copy_object(from, to).await?;
+        let resp = self.core.copy_object(from, to).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => {
                 // According to the documentation, when using copy_object, a 200 error may occur and we need to detect it.
                 // https://docs.aws.amazon.com/AmazonS3/latest/API/API_CopyObject.html#API_CopyObject_RequestSyntax
@@ -1072,72 +1006,59 @@
 
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self
-            .core
-            .s3_head_object(path, args.if_none_match(), args.if_match())
-            .await?;
+        let resp = self.core.head_object(path, &args).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             StatusCode::NOT_FOUND if path.ends_with('/') => {
                 Ok(RpStat::new(Metadata::new(EntryMode::DIR)))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
-        let resp = self.core.s3_delete_object(path).await?;
+        let resp = self.core.delete_object(path).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::NO_CONTENT => Ok(RpDelete::default()),
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         Ok((
             RpList::default(),
-            S3Pager::new(
-                self.core.clone(),
-                path,
-                args.delimiter(),
-                args.limit(),
-                args.start_after(),
-            ),
+            WasabiPager::new(self.core.clone(), path, args.delimiter(), args.limit()),
         ))
     }
 
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
-            PresignOperation::Stat(v) => {
-                self.core
-                    .s3_head_object_request(path, v.if_none_match(), v.if_match())?
-            }
-            PresignOperation::Read(v) => self.core.s3_get_object_request(
+            PresignOperation::Stat(v) => self.core.head_object_request(path, v)?,
+            PresignOperation::Read(v) => self.core.get_object_request(
                 path,
                 v.range(),
                 v.override_content_disposition(),
                 v.override_cache_control(),
                 v.if_none_match(),
-                v.if_match(),
             )?,
             PresignOperation::Write(_) => {
                 self.core
-                    .s3_put_object_request(path, None, None, None, None, AsyncBody::Empty)?
+                    .put_object_request(path, None, None, None, None, AsyncBody::Empty)?
             }
         };
 
         self.core.sign_query(&mut req, args.expire()).await?;
 
         // We don't need this request anymore, consume it directly.
         let (parts, _) = req.into_parts();
@@ -1150,22 +1071,22 @@
     }
 
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         let ops = args.into_operation();
         if ops.len() > 1000 {
             return Err(Error::new(
                 ErrorKind::Unsupported,
-                "s3 services only allow delete up to 1000 keys at once",
+                "wasabi services only allow delete up to 1000 keys at once",
             )
             .with_context("length", ops.len().to_string()));
         }
 
         let paths = ops.into_iter().map(|(p, _)| p).collect();
 
-        let resp = self.core.s3_delete_objects(paths).await?;
+        let resp = self.core.delete_objects(paths).await?;
 
         let status = resp.status();
 
         if let StatusCode::OK = status {
             let bs = resp.into_body().bytes().await?;
 
             let result: DeleteObjectsResult =
@@ -1176,30 +1097,38 @@
                 let path = build_rel_path(&self.core.root, &i.key);
                 batched_result.push((path, Ok(RpDelete::default().into())));
             }
             // TODO: we should handle those errors with code.
             for i in result.error {
                 let path = build_rel_path(&self.core.root, &i.key);
 
-                // set the error kind and mark temporary if retryable
-                let (kind, retryable) =
-                    parse_s3_error_code(i.code.as_str()).unwrap_or((ErrorKind::Unexpected, false));
-                let mut err = Error::new(kind, &format!("{i:?}"));
-                if retryable {
-                    err = err.set_temporary();
-                }
-
-                batched_result.push((path, Err(err)));
+                batched_result.push((
+                    path,
+                    Err(Error::new(ErrorKind::Unexpected, &format!("{i:?}"))),
+                ));
             }
 
             Ok(RpBatch::new(batched_result))
         } else {
             Err(parse_error(resp).await?)
         }
     }
+
+    /// Execute rename API call
+    /// Wasabi will auto-create missing path for destination `to` if any
+    async fn rename(&self, from: &str, to: &str, _args: OpRename) -> Result<RpRename> {
+        let resp = self.core.rename_object(from, to).await?;
+
+        let status = resp.status();
+
+        match status {
+            StatusCode::OK => Ok(RpRename::default()),
+            _ => Err(parse_error(resp).await?),
+        }
+    }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
@@ -1210,51 +1139,51 @@
             ("test.xyz", false, true),
             ("", true, false),
             ("test", true, true),
             ("test.xyz", true, false),
         ];
 
         for (bucket, enable_virtual_host_style, expected) in bucket_cases {
-            let mut b = S3Builder::default();
+            let mut b = WasabiBuilder::default();
             b.bucket(bucket);
             if enable_virtual_host_style {
                 b.enable_virtual_host_style();
             }
             assert_eq!(b.is_bucket_valid(), expected)
         }
     }
 
     #[test]
     fn test_build_endpoint() {
         let _ = tracing_subscriber::fmt().with_test_writer().try_init();
 
         let endpoint_cases = vec![
-            Some("s3.amazonaws.com"),
-            Some("https://s3.amazonaws.com"),
-            Some("https://s3.us-east-2.amazonaws.com"),
+            Some("s3.wasabisys.com"),
+            Some("https://s3.wasabisys.com"),
+            Some("https://s3.us-east-2.wasabisys.com"),
             None,
         ];
 
         for endpoint in &endpoint_cases {
-            let mut b = S3Builder::default();
+            let mut b = WasabiBuilder::default();
             b.bucket("test");
             if let Some(endpoint) = endpoint {
                 b.endpoint(endpoint);
             }
 
             let endpoint = b.build_endpoint("us-east-2");
-            assert_eq!(endpoint, "https://s3.us-east-2.amazonaws.com/test");
+            assert_eq!(endpoint, "https://s3.us-east-2.wasabisys.com/test");
         }
 
         for endpoint in &endpoint_cases {
-            let mut b = S3Builder::default();
+            let mut b = WasabiBuilder::default();
             b.bucket("test");
             b.enable_virtual_host_style();
             if let Some(endpoint) = endpoint {
                 b.endpoint(endpoint);
             }
 
             let endpoint = b.build_endpoint("us-east-2");
-            assert_eq!(endpoint, "https://test.s3.us-east-2.amazonaws.com");
+            assert_eq!(endpoint, "https://test.s3.us-east-2.wasabisys.com");
         }
     }
 }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/s3/compatible_services.md` & `opendal-0.36.1/local_dependencies/opendal/src/services/s3/compatible_services.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-## AWS S3
+
+## Compatible Services
+
+### AWS S3
 
 [AWS S3](https://aws.amazon.com/s3/) is the default implementations of s3 services. Only `bucket` is required.
 
 ```rust,ignore
 builder.bucket("<bucket_name>");
 ```
 
-## Alibaba Object Storage Service (OSS)
+### Alibaba Object Storage Service (OSS)
 
 [OSS](https://www.alibabacloud.com/product/object-storage-service) is a s3 compatible service provided by [Alibaba Cloud](https://www.alibabacloud.com).
 
 To connect to OSS, we need to set:
 
 - `endpoint`: The endpoint of oss, for example: `https://oss-cn-hangzhou.aliyuncs.com`
 - `bucket`: The bucket name of oss.
@@ -34,15 +37,15 @@
 ```rust,ignore
 builder.endpoint("https://oss-cn-hangzhou.aliyuncs.com");
 builder.region("<region>");
 builder.bucket("<bucket_name>");
 builder.enable_virtual_host_style();
 ```
 
-## Minio
+### Minio
 
 [minio](https://min.io/) is an open-source s3 compatible services.
 
 To connect to minio, we need to set:
 
 - `endpoint`: The endpoint of minio, for example: `http://127.0.0.1:9000`
 - `region`: The region of minio. If not specified, it could be ignored.
@@ -50,43 +53,43 @@
 
 ```rust,ignore
 builder.endpoint("http://127.0.0.1:9000");
 builder.region("<region>");
 builder.bucket("<bucket_name>");
 ```
 
-## QingStor Object Storage
+### QingStor Object Storage
 
 [QingStor Object Storage](https://www.qingcloud.com/products/qingstor) is a S3-compatible service provided by [QingCloud](https://www.qingcloud.com/).
 
 To connect to QingStor Object Storage, we need to set:
 
 - `endpoint`: The endpoint of QingStor s3 compatible endpoint, for example: `https://s3.pek3b.qingstor.com`
 - `bucket`: The bucket name.
 
-## Scaleway Object Storage
+### Scaleway Object Storage
 
 [Scaleway Object Storage](https://www.scaleway.com/en/object-storage/) is a S3-compatible and multi-AZ redundant object storage service.
 
 To connect to Scaleway Object Storage, we need to set:
 
 - `endpoint`: The endpoint of scaleway, for example: `https://s3.nl-ams.scw.cloud`
 - `region`: The region of scaleway.
 - `bucket`: The bucket name of scaleway.
 
-## Tencent Cloud Object Storage (COS)
+### Tencent Cloud Object Storage (COS)
 
 [COS](https://intl.cloud.tencent.com/products/cos) is a s3 compatible service provided by [Tencent Cloud](https://intl.cloud.tencent.com/).
 
 To connect to COS, we need to set:
 
 - `endpoint`: The endpoint of cos, for example: `https://cos.ap-beijing.myqcloud.com`
 - `bucket`: The bucket name of cos.
 
-## Wasabi Object Storage
+### Wasabi Object Storage
 
 [Wasabi](https://wasabi.com/) is a s3 compatible service.
 
 > Cloud storage pricing that is 80% less than Amazon S3.
 
 To connect to wasabi, we need to set:
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/s3/core.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/s3/core.rs`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
         self.client.send(req).await
     }
 
     /// # Note
     ///
     /// header like X_AMZ_SERVER_SIDE_ENCRYPTION doesn't need to set while
-    //  get or stat.
+    /// get or stat.
     pub fn insert_sse_headers(
         &self,
         mut req: http::request::Builder,
         is_write: bool,
     ) -> http::request::Builder {
         if is_write {
             if let Some(v) = &self.server_side_encryption {
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/s3/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/s3/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/s3/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/s3/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/s3/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/s3/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/s3/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/s3/writer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 use async_trait::async_trait;
 use bytes::Buf;
 use bytes::Bytes;
 use http::StatusCode;
 
 use super::core::*;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct S3Writer {
     core: Arc<S3Core>,
 
     op: OpWrite,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/sftp/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/sftp/backend.rs`

 * *Files 21% similar despite different names*

```diff
@@ -32,76 +32,25 @@
 use openssh_sftp_client::SftpOptions;
 
 use super::error::is_not_found;
 use super::error::is_sftp_protocol_error;
 use super::pager::SftpPager;
 use super::utils::SftpReader;
 use super::writer::SftpWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// SFTP services support. (only works on unix)
 ///
-/// Warning: Maximum number of file holdings is depend on the remote system configuration.
-/// For example, the default value is 255 in macos, and 1024 in linux. If you want to open
-/// lots of files, you should pay attention to close the file after using it.
-///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [x] copy
-/// - [x] rename
-/// - [x] list
-/// - [ ] ~~scan~~
-/// - [ ] ~~presign~~
-/// - [ ] blocking
-///
-/// # Configuration
-///
-/// - `endpoint`: Set the endpoint for connection
-/// - `root`: Set the work directory for backend, default to `/home/$USER/`
-/// - `user`: Set the login user
-/// - `key`: Set the public key for login
-/// - `known_hosts_strategy`: Set the strategy for known hosts, default to `Strict`
-/// - `enable_copy`: Set whether the remote server has copy-file extension
-///
-/// It doesn't support password login, you can use public key instead.
+/// Warning: Maximum number of file holdings is depending on the remote system configuration.
 ///
-/// You can refer to [`SftpBuilder`]'s docs for more information
-///
-/// # Example
-///
-/// ## Via Builder
-///
-/// ```no_run
-/// use anyhow::Result;
-/// use opendal::services::Sftp;
-/// use opendal::Object;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     // create backend builder
-///     let mut builder = Sftp::default();
-///
-///     builder.endpoint("127.0.0.1").user("test").key("test_key");
+/// For example, the default value is 255 in macOS, and 1024 in linux. If you want to open
+/// lots of files, you should pay attention to close the file after using it.
 ///
-///     let op: Operator = Operator::new(builder)?.finish();
-///     let _obj: Object = op.object("test_file");
-///     Ok(())
-/// }
-/// ```
-
+#[doc = include_str!("docs.md")]
 #[derive(Default)]
 pub struct SftpBuilder {
     endpoint: Option<String>,
     root: Option<String>,
     user: Option<String>,
     key: Option<String>,
     known_hosts_strategy: Option<String>,
@@ -273,15 +222,15 @@
 
 #[async_trait]
 impl Accessor for SftpBackend {
     type Reader = SftpReader;
     type BlockingReader = ();
     type Writer = SftpWriter;
     type BlockingWriter = ();
-    type Appender = ();
+    type Appender = SftpWriter;
     type Pager = Option<SftpPager>;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_root(self.root.as_str())
             .set_scheme(Scheme::Sftp)
@@ -299,14 +248,15 @@
 
                 list: true,
                 list_with_limit: true,
                 list_with_delimiter_slash: true,
 
                 copy: self.copyable,
                 rename: true,
+                append: true,
 
                 ..Default::default()
             });
 
         am
     }
 
@@ -383,14 +333,33 @@
         let path = fs.canonicalize(path).await?;
 
         let file = client.create(&path).await?;
 
         Ok((RpWrite::new(), SftpWriter::new(file)))
     }
 
+    async fn append(&self, path: &str, _: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        if let Some((dir, _)) = path.rsplit_once('/') {
+            self.create_dir(dir, OpCreateDir::default()).await?;
+        }
+
+        let client = self.connect().await?;
+
+        let mut fs = client.fs();
+        fs.set_cwd(&self.root);
+        let path = fs.canonicalize(path).await?;
+
+        let mut option = client.options();
+        option.append(true).create(true);
+
+        let file = option.open(path).await?;
+
+        Ok((RpAppend::new(), SftpWriter::new(file)))
+    }
+
     async fn copy(&self, from: &str, to: &str, _: OpCopy) -> Result<RpCopy> {
         let client = self.connect().await?;
 
         let mut fs = client.fs();
         fs.set_cwd(&self.root);
 
         if let Some((dir, _)) = to.rsplit_once('/') {
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/sftp/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/sftp/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/sftp/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/sftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/sftp/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/sftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/sftp/utils.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/sftp/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/sftp/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/sftp/writer.rs`

 * *Files 6% similar despite different names*

```diff
@@ -49,7 +49,20 @@
         ))
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
 }
+
+#[async_trait]
+impl oio::Append for SftpWriter {
+    async fn append(&mut self, bs: Bytes) -> Result<()> {
+        self.file.write_all(&bs).await?;
+
+        Ok(())
+    }
+
+    async fn close(&mut self) -> Result<()> {
+        Ok(())
+    }
+}
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/sled/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/sled/backend.rs`

 * *Files 17% similar despite different names*

```diff
@@ -26,54 +26,15 @@
 use crate::Error;
 use crate::ErrorKind;
 use crate::Scheme;
 use crate::*;
 
 /// Sled service support.
 ///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [ ] copy
-/// - [ ] rename
-/// - [ ] ~~list~~
-/// - [ ] scan
-/// - [ ] ~~presign~~
-/// - [x] blocking
-///
-/// # Configuration
-///
-/// - `datadir`: Set the path to the sled data directory
-///
-/// You can refer to [`SledBuilder`]'s docs for more information
-///
-/// # Example
-///
-/// ## Via Builder
-///
-/// ```no_run
-/// use anyhow::Result;
-/// use opendal::services::Sled;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     let mut builder = Sled::default();
-///     builder.datadir("/tmp/opendal/sled");
-///
-///     let op: Operator = Operator::new(builder)?.finish();
-///     Ok(())
-/// }
-/// ```
+#[doc = include_str!("docs.md")]
 #[derive(Default)]
 pub struct SledBuilder {
     /// That path to the sled data directory.
     datadir: Option<String>,
     root: Option<String>,
 }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/sled/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/webdav/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -12,9 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
+pub use backend::WebdavBuilder as Webdav;
 
-pub use backend::SledBuilder as Sled;
+mod error;
+mod list_response;
+mod pager;
+mod writer;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/supabase/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/supabase/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 use async_trait::async_trait;
 use http::StatusCode;
 use log::debug;
 
 use super::core::*;
 use super::error::parse_error;
 use super::writer::*;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Supabase service
 ///
 /// # Capabilities
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/supabase/core.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/supabase/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/supabase/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/supabase/error.rs`

 * *Files 20% similar despite different names*

```diff
@@ -55,19 +55,22 @@
 
     Ok(err)
 }
 
 // Return the error kind and whether it is retryable
 fn parse_supabase_error(err: &SupabaseError) -> (ErrorKind, bool) {
     let code = err.status_code.parse::<u16>().unwrap();
-    if code == StatusCode::CONFLICT.as_u16() && err.error == "Duplicate" {
-        (ErrorKind::AlreadyExists, false)
-    } else if code == StatusCode::NOT_FOUND.as_u16() {
-        (ErrorKind::NotFound, false)
-    } else if code == StatusCode::FORBIDDEN.as_u16() {
-        (ErrorKind::PermissionDenied, false)
-    } else if code == StatusCode::PRECONDITION_FAILED.as_u16() {
-        (ErrorKind::ConditionNotMatch, false)
-    } else {
-        (ErrorKind::Unexpected, false)
+    let status_code = StatusCode::from_u16(code).unwrap();
+    match status_code {
+        StatusCode::CONFLICT => (ErrorKind::AlreadyExists, false),
+        StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
+        StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
+        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
+            (ErrorKind::ConditionNotMatch, false)
+        }
+        StatusCode::INTERNAL_SERVER_ERROR
+        | StatusCode::BAD_GATEWAY
+        | StatusCode::SERVICE_UNAVAILABLE
+        | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
+        _ => (ErrorKind::Unexpected, false),
     }
 }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/supabase/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/supabase/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/supabase/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/supabase/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
 use super::core::*;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct SupabaseWriter {
     core: Arc<SupabaseCore>,
 
     op: OpWrite,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs`

 * *Files 7% similar despite different names*

```diff
@@ -21,29 +21,16 @@
 use http::header;
 use http::Request;
 use http::Response;
 use http::StatusCode;
 
 use super::error::parse_error;
 use super::writer::VercelArtifactsWriter;
-use crate::ops::OpRead;
-use crate::ops::OpWrite;
-use crate::raw::new_request_build_error;
-use crate::raw::parse_into_metadata;
-use crate::raw::Accessor;
-use crate::raw::AccessorInfo;
-use crate::raw::AsyncBody;
-use crate::raw::HttpClient;
-use crate::raw::IncomingAsyncBody;
-use crate::raw::RpRead;
-use crate::raw::RpWrite;
-use crate::types::Result;
-use crate::Capability;
-use crate::Error;
-use crate::ErrorKind;
+use crate::raw::*;
+use crate::*;
 
 #[derive(Clone)]
 pub struct VercelArtifactsBackend {
     pub(crate) access_token: String,
     pub(crate) client: HttpClient,
 }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/vercel_artifacts/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
 use super::backend::VercelArtifactsBackend;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct VercelArtifactsWriter {
     backend: VercelArtifactsBackend,
     op: OpWrite,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/s3/backend.rs`

 * *Files 20% similar despite different names*

```diff
@@ -33,256 +33,40 @@
 use reqsign::AwsConfig;
 use reqsign::AwsCredentialLoad;
 use reqsign::AwsLoader;
 use reqsign::AwsV4Signer;
 
 use super::core::*;
 use super::error::parse_error;
-use super::pager::WasabiPager;
-use super::writer::WasabiWriter;
-use crate::ops::*;
+use super::error::parse_s3_error_code;
+use super::pager::S3Pager;
+use super::writer::S3Writer;
 use crate::raw::*;
 use crate::*;
 
 /// Allow constructing correct region endpoint if user gives a global endpoint.
 static ENDPOINT_TEMPLATES: Lazy<HashMap<&'static str, &'static str>> = Lazy::new(|| {
     let mut m = HashMap::new();
     // AWS S3 Service.
     m.insert(
-        "https://s3.wasabisys.com",
-        "https://s3.{region}.wasabisys.com",
+        "https://s3.amazonaws.com",
+        "https://s3.{region}.amazonaws.com",
     );
     m
 });
 
-/// Wasabi (an aws S3 compatible service) support
-///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [x] copy
-/// - [x] rename
-/// - [x] list
-/// - [x] scan
-/// - [x] presign
-/// - [ ] blocking
-///
-/// # Configuration
-///
-/// - `root`: Set the work dir for backend.
-/// - `bucket`: Set the container name for backend.
-/// - `endpoint`: Set the endpoint for backend.
-/// - `region`: Set the region for backend.
-/// - `access_key_id`: Set the access_key_id for backend.
-/// - `secret_access_key`: Set the secret_access_key for backend.
-/// - `security_token`: Set the security_token for backend.
-/// - `default_storage_class`: Set the default storage_class for backend.
-/// - `server_side_encryption`: Set the server_side_encryption for backend.
-/// - `server_side_encryption_aws_kms_key_id`: Set the server_side_encryption_aws_kms_key_id for backend.
-/// - `server_side_encryption_customer_algorithm`: Set the server_side_encryption_customer_algorithm for backend.
-/// - `server_side_encryption_customer_key`: Set the server_side_encryption_customer_key for backend.
-/// - `server_side_encryption_customer_key_md5`: Set the server_side_encryption_customer_key_md5 for backend.
-/// - `disable_config_load`: Disable aws config load from env
-/// - `enable_virtual_host_style`: Enable virtual host style.
-///
-/// Refer to [`WasabiBuilder`]'s public API docs for more information.
-///
-/// # Temporary security credentials
-///
-/// OpenDAL now provides support for S3 temporary security credentials in IAM.
-///
-/// The way to take advantage of this feature is to build your S3 backend with `Builder::security_token`.
-///
-/// But OpenDAL will not refresh the temporary security credentials, please keep in mind to refresh those credentials in time.
-///
-/// # Server Side Encryption
-///
-/// OpenDAL provides full support of S3 Server Side Encryption(SSE) features.
-///
-/// The easiest way to configure them is to use helper functions like
-///
-/// - SSE-KMS: `server_side_encryption_with_aws_managed_kms_key`
-/// - SSE-KMS: `server_side_encryption_with_customer_managed_kms_key`
-/// - SSE-S3: `server_side_encryption_with_s3_key`
-/// - SSE-C: `server_side_encryption_with_customer_key`
-///
-/// If those functions don't fulfill need, low-level options are also provided:
-///
-/// - Use service managed kms key
-///   - `server_side_encryption="aws:kms"`
-/// - Use customer provided kms key
-///   - `server_side_encryption="aws:kms"`
-///   - `server_side_encryption_aws_kms_key_id="your-kms-key"`
-/// - Use S3 managed key
-///   - `server_side_encryption="AES256"`
-/// - Use customer key
-///   - `server_side_encryption_customer_algorithm="AES256"`
-///   - `server_side_encryption_customer_key="base64-of-your-aes256-key"`
-///   - `server_side_encryption_customer_key_md5="base64-of-your-aes256-key-md5"`
-///
-/// After SSE have been configured, all requests send by this backed will attach those headers.
-///
-/// Reference: [Protecting data using server-side encryption](https://docs.aws.amazon.com/AmazonS3/latest/userguide/serv-side-encryption.html)
-///
-/// # Example
-///
-/// ## Basic Setup
-///
-/// ```no_run
-/// use std::sync::Arc;
-///
-/// use anyhow::Result;
-/// use opendal::services::Wasabi;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     // Create s3 backend builder.
-///     let mut builder = Wasabi::default();
-///     // Set the root for s3, all operations will happen under this root.
-///     //
-///     // NOTE: the root must be absolute path.
-///     builder.root("/path/to/dir");
-///     // Set the bucket name, this is required.
-///     builder.bucket("test");
-///     // Set the endpoint.
-///     //
-///     // For examples:
-///     // - "https://s3.wasabisys.com"
-///     // - "http://127.0.0.1:9000"
-///     // - "https://oss-ap-northeast-1.aliyuncs.com"
-///     // - "https://cos.ap-seoul.myqcloud.com"
-///     //
-///     // Default to "https://s3.wasabisys.com"
-///     builder.endpoint("https://s3.wasabisys.com");
-///     // Set the access_key_id and secret_access_key.
-///     //
-///     // OpenDAL will try load credential from the env.
-///     // If credential not set and no valid credential in env, OpenDAL will
-///     // send request without signing like anonymous user.
-///     builder.access_key_id("access_key_id");
-///     builder.secret_access_key("secret_access_key");
-///
-///     let op: Operator = Operator::new(builder)?.finish();
-///
-///     Ok(())
-/// }
-/// ```
-///
-/// ## Wasabi with SSE-C
-///
-/// ```no_run
-/// use anyhow::Result;
-/// use log::info;
-/// use opendal::services::Wasabi;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     let mut builder = Wasabi::default();
-///
-///     // Setup builders
-///
-///     // Enable SSE-C
-///     builder.server_side_encryption_with_customer_key("AES256", "customer_key".as_bytes());
-///
-///     let op = Operator::new(builder)?.finish();
-///     info!("operator: {:?}", op);
-///
-///     // Writing your testing code here.
-///
-///     Ok(())
-/// }
-/// ```
-///
-/// ## Wasabi with SSE-KMS and aws managed kms key
-///
-/// ```no_run
-/// use anyhow::Result;
-/// use log::info;
-/// use opendal::services::Wasabi;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     let mut builder = Wasabi::default();
-///
-///     // Setup builders
-///
-///     // Enable SSE-KMS with aws managed kms key
-///     builder.server_side_encryption_with_aws_managed_kms_key();
-///
-///     let op = Operator::new(builder)?.finish();
-///     info!("operator: {:?}", op);
-///
-///     // Writing your testing code here.
-///
-///     Ok(())
-/// }
-/// ```
-///
-/// ## Wasabi with SSE-KMS and customer managed kms key
-///
-/// ```no_run
-/// use anyhow::Result;
-/// use log::info;
-/// use opendal::services::Wasabi;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     let mut builder = Wasabi::default();
-///
-///     // Setup builders
-///
-///     // Enable SSE-KMS with customer managed kms key
-///     builder.server_side_encryption_with_customer_managed_kms_key("aws_kms_key_id");
-///
-///     let op = Operator::new(builder)?.finish();
-///     info!("operator: {:?}", op);
-///
-///     // Writing your testing code here.
-///
-///     Ok(())
-/// }
-/// ```
-///
-/// ## Wasabi with SSE-S3
-///
-/// ```no_run
-/// use anyhow::Result;
-/// use log::info;
-/// use opendal::services::Wasabi;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     let mut builder = Wasabi::default();
-///
-///     // Setup builders
-///
-///     // Enable SSE-S3
-///     builder.server_side_encryption_with_s3_key();
-///
-///     let op = Operator::new(builder)?.finish();
-///     info!("operator: {:?}", op);
-///
-///     // Writing your testing code here.
+const DEFAULT_WRITE_MIN_SIZE: usize = 8 * 1024 * 1024;
+
+/// Aws S3 and compatible services (including minio, digitalocean space, Tencent Cloud Object Storage(COS) and so on) support.
+/// For more information about s3-compatible services, refer to [Compatible Services](#compatible-services).
 ///
-///     Ok(())
-/// }
-/// ```
+#[doc = include_str!("docs.md")]
+#[doc = include_str!("compatible_services.md")]
 #[derive(Default)]
-pub struct WasabiBuilder {
+pub struct S3Builder {
     root: Option<String>,
 
     bucket: String,
     endpoint: Option<String>,
     region: Option<String>,
     role_arn: Option<String>,
     external_id: Option<String>,
@@ -296,34 +80,39 @@
     default_storage_class: Option<String>,
 
     /// temporary credentials, check the official [doc](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp.html) for detail
     security_token: Option<String>,
 
     disable_config_load: bool,
     disable_ec2_metadata: bool,
+    allow_anonymous: bool,
     enable_virtual_host_style: bool,
 
     http_client: Option<HttpClient>,
     customed_credential_load: Option<Box<dyn AwsCredentialLoad>>,
+
+    /// the part size of s3 multipart upload, which should be 5 MiB to 5 GiB.
+    /// There is no minimum size limit on the last part of your multipart upload
+    write_min_size: Option<usize>,
 }
 
-impl Debug for WasabiBuilder {
+impl Debug for S3Builder {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         let mut d = f.debug_struct("Builder");
 
         d.field("root", &self.root)
             .field("bucket", &self.bucket)
             .field("endpoint", &self.endpoint)
             .field("region", &self.region);
 
         d.finish_non_exhaustive()
     }
 }
 
-impl WasabiBuilder {
+impl S3Builder {
     /// Set root of this backend.
     ///
     /// All operations will happen under this root.
     pub fn root(&mut self, root: &str) -> &mut Self {
         self.root = if root.is_empty() {
             None
         } else {
@@ -340,29 +129,34 @@
         self
     }
 
     /// Set endpoint of this backend.
     ///
     /// Endpoint must be full uri, e.g.
     ///
-    /// - `https://s3.wasabisys.com` or `https://s3.{region}.wasabisys.com`
+    /// - AWS S3: `https://s3.amazonaws.com` or `https://s3.{region}.amazonaws.com`
+    /// - Aliyun OSS: `https://{region}.aliyuncs.com`
+    /// - Tencent COS: `https://cos.{region}.myqcloud.com`
+    /// - Minio: `http://127.0.0.1:9000`
     ///
-    /// If user inputs endpoint without scheme like "s3.wasabisys.com", we
+    /// If user inputs endpoint without scheme like "s3.amazonaws.com", we
     /// will prepend "https://" before it.
     pub fn endpoint(&mut self, endpoint: &str) -> &mut Self {
         if !endpoint.is_empty() {
             // Trim trailing `/` so that we can accept `http://127.0.0.1:9000/`
             self.endpoint = Some(endpoint.trim_end_matches('/').to_string())
         }
 
         self
     }
 
-    /// Region represent the signing region of this endpoint.
+    /// Region represent the signing region of this endpoint. This is required
+    /// if you are using the default AWS S3 endpoint.
     ///
+    /// If using a custom endpoint,
     /// - If region is set, we will take user's input first.
     /// - If not, the default `us-east-1` will be used.
     pub fn region(&mut self, region: &str) -> &mut Self {
         if !region.is_empty() {
             self.region = Some(region.to_string())
         }
 
@@ -408,20 +202,25 @@
             self.external_id = Some(v.to_string())
         }
 
         self
     }
 
     /// Set default storage_class for this backend.
-    /// Unlike S3, wasabi only supports one single storage class,
-    /// which is most like standard S3 storage class,
-    /// check `https://docs.wasabi.com/docs/operations-on-objects` for more details.
     ///
     /// Available values:
+    /// - `DEEP_ARCHIVE`
+    /// - `GLACIER`
+    /// - `GLACIER_IR`
+    /// - `INTELLIGENT_TIERING`
+    /// - `ONEZONE_IA`
+    /// - `OUTPOSTS`
+    /// - `REDUCED_REDUNDANCY`
     /// - `STANDARD`
+    /// - `STANDARD_IA`
     pub fn default_storage_class(&mut self, v: &str) -> &mut Self {
         if !v.is_empty() {
             self.default_storage_class = Some(v.to_string())
         }
 
         self
     }
@@ -575,15 +374,15 @@
         self.server_side_encryption_customer_algorithm = Some(algorithm.to_string());
         self.server_side_encryption_customer_key = Some(BASE64_STANDARD.encode(key));
         self.server_side_encryption_customer_key_md5 =
             Some(BASE64_STANDARD.encode(Md5::digest(key).as_slice()));
         self
     }
 
-    /// Set temporary credential used in service connections
+    /// Set temporary credential used in AWS S3 connections
     ///
     /// # Warning
     ///
     /// security token's lifetime is short and requires users to refresh in time.
     pub fn security_token(&mut self, token: &str) -> &mut Self {
         if !token.is_empty() {
             self.security_token = Some(token.to_string());
@@ -608,19 +407,26 @@
     /// This option is used to disable the default behavior of opendal
     /// to load credential from ec2 metadata, a.k.a, IMDSv2
     pub fn disable_ec2_metadata(&mut self) -> &mut Self {
         self.disable_ec2_metadata = true;
         self
     }
 
+    /// Allow anonymous will allow opendal to send request without signing
+    /// when credentail is not loaded.
+    pub fn allow_anonymous(&mut self) -> &mut Self {
+        self.allow_anonymous = true;
+        self
+    }
+
     /// Enable virtual host style so that opendal will send API requests
     /// in virtual host style instead of path style.
     ///
-    /// - By default, opendal will send API to `https://s3.us-east-1.wasabisys.com/bucket_name`
-    /// - Enabled, opendal will send API to `https://bucket_name.s3.us-east-1.wasabisys.com`
+    /// - By default, opendal will send API to `https://s3.us-east-1.amazonaws.com/bucket_name`
+    /// - Enabled, opendal will send API to `https://bucket_name.s3.us-east-1.amazonaws.com`
     pub fn enable_virtual_host_style(&mut self) -> &mut Self {
         self.enable_virtual_host_style = true;
         self
     }
 
     /// Adding a customed credential load for service.
     pub fn customed_credential_load(&mut self, cred: Box<dyn AwsCredentialLoad>) -> &mut Self {
@@ -668,15 +474,15 @@
                 if endpoint.starts_with("http") {
                     endpoint.to_string()
                 } else {
                     // Prefix https if endpoint doesn't start with scheme.
                     format!("https://{endpoint}")
                 }
             }
-            None => "https://s3.wasabisys.com".to_string(),
+            None => "https://s3.amazonaws.com".to_string(),
         };
 
         // If endpoint contains bucket name, we should trim them.
         endpoint = endpoint.replace(&format!("//{bucket}."), "//");
 
         // Update with endpoint templates.
         endpoint = if let Some(template) = ENDPOINT_TEMPLATES.get(endpoint.as_str()) {
@@ -692,22 +498,30 @@
             endpoint = endpoint.replace("//", &format!("//{bucket}."))
         } else {
             write!(endpoint, "/{bucket}").expect("write into string must succeed");
         };
 
         endpoint
     }
+
+    /// set the minimum size of unsized write, it should be greater than 5 MB.
+    /// Reference: [Amazon S3 multipart upload limits](https://docs.aws.amazon.com/AmazonS3/latest/userguide/qfacts.html)
+    pub fn write_min_size(&mut self, write_min_size: usize) -> &mut Self {
+        self.write_min_size = Some(write_min_size);
+
+        self
+    }
 }
 
-impl Builder for WasabiBuilder {
-    const SCHEME: Scheme = Scheme::Wasabi;
-    type Accessor = WasabiBackend;
+impl Builder for S3Builder {
+    const SCHEME: Scheme = Scheme::S3;
+    type Accessor = S3Backend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
-        let mut builder = WasabiBuilder::default();
+        let mut builder = S3Builder::default();
 
         map.get("root").map(|v| builder.root(v));
         map.get("bucket").map(|v| builder.bucket(v));
         map.get("endpoint").map(|v| builder.endpoint(v));
         map.get("region").map(|v| builder.region(v));
         map.get("access_key_id").map(|v| builder.access_key_id(v));
         map.get("secret_access_key")
@@ -730,14 +544,17 @@
             .map(|_| builder.disable_config_load());
         map.get("disable_ec2_metadata")
             .filter(|v| *v == "on" || *v == "true")
             .map(|_| builder.disable_ec2_metadata());
         map.get("enable_virtual_host_style")
             .filter(|v| *v == "on" || *v == "true")
             .map(|_| builder.enable_virtual_host_style());
+        map.get("allow_anonymous")
+            .filter(|v| *v == "on" || *v == "true")
+            .map(|_| builder.allow_anonymous());
         map.get("default_storage_class")
             .map(|v| builder.default_storage_class(v));
 
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
@@ -836,18 +653,26 @@
             cfg.role_arn = Some(v)
         }
         if let Some(v) = self.external_id.take() {
             cfg.external_id = Some(v)
         }
 
         if cfg.region.is_none() {
-            // region is required to make signer work.
-            //
-            // If we don't know region after loading from builder and env.
-            // We will use `us-east-1` as default.
+            // AWS S3 requires region to be set.
+            if self.endpoint.is_none()
+                || self.endpoint.as_deref() == Some("https://s3.amazonaws.com")
+            {
+                return Err(Error::new(ErrorKind::ConfigInvalid, "region is missing")
+                    .with_operation("Builder::build")
+                    .with_context("service", Scheme::S3));
+            }
+
+            // For other compatible services, if we don't know region
+            // after loading from builder and env, we can use `us-east-1`
+            // as default.
             cfg.region = Some("us-east-1".to_string());
         }
 
         let region = cfg.region.to_owned().unwrap();
         debug!("backend use region: {region}");
 
         // Building endpoint.
@@ -859,92 +684,111 @@
             loader = loader.with_disable_ec2_metadata();
         }
         if let Some(v) = self.customed_credential_load.take() {
             loader = loader.with_customed_credential_loader(v);
         }
 
         let signer = AwsV4Signer::new("s3", &region);
+        let write_min_size = self.write_min_size.unwrap_or(DEFAULT_WRITE_MIN_SIZE);
+        if write_min_size < 5 * 1024 * 1024 {
+            return Err(Error::new(
+                ErrorKind::ConfigInvalid,
+                "The write minimum buffer size is misconfigured",
+            )
+            .with_context("service", Scheme::S3));
+        }
 
         debug!("backend build finished");
-        Ok(WasabiBackend {
-            core: Arc::new(WasabiCore {
+        Ok(S3Backend {
+            core: Arc::new(S3Core {
                 bucket: bucket.to_string(),
                 endpoint,
                 root,
                 server_side_encryption,
                 server_side_encryption_aws_kms_key_id,
                 server_side_encryption_customer_algorithm,
                 server_side_encryption_customer_key,
                 server_side_encryption_customer_key_md5,
                 default_storage_class,
+                allow_anonymous: self.allow_anonymous,
                 signer,
                 loader,
                 client,
+                write_min_size,
             }),
         })
     }
 }
 
-/// Backend for wasabi service.
+/// Backend for s3 services.
 #[derive(Debug, Clone)]
-pub struct WasabiBackend {
-    core: Arc<WasabiCore>,
+pub struct S3Backend {
+    core: Arc<S3Core>,
 }
 
 #[async_trait]
-impl Accessor for WasabiBackend {
+impl Accessor for S3Backend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
-    type Writer = WasabiWriter;
+    type Writer = S3Writer;
     type BlockingWriter = ();
     type Appender = ();
-    type Pager = WasabiPager;
+    type Pager = S3Pager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
-        am.set_scheme(Scheme::Wasabi)
+        am.set_scheme(Scheme::S3)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
             .set_capability(Capability {
                 stat: true,
                 stat_with_if_match: true,
                 stat_with_if_none_match: true,
 
                 read: true,
                 read_can_next: true,
                 read_with_range: true,
+                read_with_if_match: true,
+                read_with_if_none_match: true,
+                read_with_override_cache_control: true,
+                read_with_override_content_disposition: true,
 
                 write: true,
+                write_with_cache_control: true,
+                write_with_content_type: true,
+                write_without_content_length: true,
                 create_dir: true,
                 delete: true,
                 copy: true,
-                rename: true,
 
                 list: true,
+                list_with_limit: true,
+                list_with_start_after: true,
                 list_without_delimiter: true,
                 list_with_delimiter_slash: true,
 
                 presign: true,
                 presign_stat: true,
                 presign_read: true,
                 presign_write: true,
 
                 batch: true,
+                batch_max_operations: Some(1000),
 
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreateDir) -> Result<RpCreateDir> {
         let mut req =
             self.core
-                .put_object_request(path, Some(0), None, None, None, AsyncBody::Empty)?;
+                .s3_put_object_request(path, Some(0), None, None, None, AsyncBody::Empty)?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         let status = resp.status();
 
@@ -956,44 +800,43 @@
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let resp = self
             .core
-            .get_object(path, args.range(), args.if_none_match())
+            .s3_get_object(
+                path,
+                args.range(),
+                args.if_none_match(),
+                args.if_match(),
+                args.override_content_disposition(),
+            )
             .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.content_length().is_none() {
-            return Err(Error::new(
-                ErrorKind::Unsupported,
-                "write without content length is not supported",
-            ));
-        }
-
         Ok((
             RpWrite::default(),
-            WasabiWriter::new(self.core.clone(), args, path.to_string()),
+            S3Writer::new(self.core.clone(), path, args),
         ))
     }
 
     async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
-        let resp = self.core.copy_object(from, to).await?;
+        let resp = self.core.s3_copy_object(from, to).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => {
                 // According to the documentation, when using copy_object, a 200 error may occur and we need to detect it.
                 // https://docs.aws.amazon.com/AmazonS3/latest/API/API_CopyObject.html#API_CopyObject_RequestSyntax
@@ -1007,59 +850,72 @@
 
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self.core.head_object(path, &args).await?;
+        let resp = self
+            .core
+            .s3_head_object(path, args.if_none_match(), args.if_match())
+            .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             StatusCode::NOT_FOUND if path.ends_with('/') => {
                 Ok(RpStat::new(Metadata::new(EntryMode::DIR)))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
-        let resp = self.core.delete_object(path).await?;
+        let resp = self.core.s3_delete_object(path).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::NO_CONTENT => Ok(RpDelete::default()),
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         Ok((
             RpList::default(),
-            WasabiPager::new(self.core.clone(), path, args.delimiter(), args.limit()),
+            S3Pager::new(
+                self.core.clone(),
+                path,
+                args.delimiter(),
+                args.limit(),
+                args.start_after(),
+            ),
         ))
     }
 
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
-            PresignOperation::Stat(v) => self.core.head_object_request(path, v)?,
-            PresignOperation::Read(v) => self.core.get_object_request(
+            PresignOperation::Stat(v) => {
+                self.core
+                    .s3_head_object_request(path, v.if_none_match(), v.if_match())?
+            }
+            PresignOperation::Read(v) => self.core.s3_get_object_request(
                 path,
                 v.range(),
                 v.override_content_disposition(),
                 v.override_cache_control(),
                 v.if_none_match(),
+                v.if_match(),
             )?,
             PresignOperation::Write(_) => {
                 self.core
-                    .put_object_request(path, None, None, None, None, AsyncBody::Empty)?
+                    .s3_put_object_request(path, None, None, None, None, AsyncBody::Empty)?
             }
         };
 
         self.core.sign_query(&mut req, args.expire()).await?;
 
         // We don't need this request anymore, consume it directly.
         let (parts, _) = req.into_parts();
@@ -1072,22 +928,22 @@
     }
 
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         let ops = args.into_operation();
         if ops.len() > 1000 {
             return Err(Error::new(
                 ErrorKind::Unsupported,
-                "wasabi services only allow delete up to 1000 keys at once",
+                "s3 services only allow delete up to 1000 keys at once",
             )
             .with_context("length", ops.len().to_string()));
         }
 
         let paths = ops.into_iter().map(|(p, _)| p).collect();
 
-        let resp = self.core.delete_objects(paths).await?;
+        let resp = self.core.s3_delete_objects(paths).await?;
 
         let status = resp.status();
 
         if let StatusCode::OK = status {
             let bs = resp.into_body().bytes().await?;
 
             let result: DeleteObjectsResult =
@@ -1098,38 +954,30 @@
                 let path = build_rel_path(&self.core.root, &i.key);
                 batched_result.push((path, Ok(RpDelete::default().into())));
             }
             // TODO: we should handle those errors with code.
             for i in result.error {
                 let path = build_rel_path(&self.core.root, &i.key);
 
-                batched_result.push((
-                    path,
-                    Err(Error::new(ErrorKind::Unexpected, &format!("{i:?}"))),
-                ));
+                // set the error kind and mark temporary if retryable
+                let (kind, retryable) =
+                    parse_s3_error_code(i.code.as_str()).unwrap_or((ErrorKind::Unexpected, false));
+                let mut err = Error::new(kind, &format!("{i:?}"));
+                if retryable {
+                    err = err.set_temporary();
+                }
+
+                batched_result.push((path, Err(err)));
             }
 
             Ok(RpBatch::new(batched_result))
         } else {
             Err(parse_error(resp).await?)
         }
     }
-
-    /// Execute rename API call
-    /// Wasabi will auto-create missing path for destination `to` if any
-    async fn rename(&self, from: &str, to: &str, _args: OpRename) -> Result<RpRename> {
-        let resp = self.core.rename_object(from, to).await?;
-
-        let status = resp.status();
-
-        match status {
-            StatusCode::OK => Ok(RpRename::default()),
-            _ => Err(parse_error(resp).await?),
-        }
-    }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
@@ -1140,51 +988,51 @@
             ("test.xyz", false, true),
             ("", true, false),
             ("test", true, true),
             ("test.xyz", true, false),
         ];
 
         for (bucket, enable_virtual_host_style, expected) in bucket_cases {
-            let mut b = WasabiBuilder::default();
+            let mut b = S3Builder::default();
             b.bucket(bucket);
             if enable_virtual_host_style {
                 b.enable_virtual_host_style();
             }
             assert_eq!(b.is_bucket_valid(), expected)
         }
     }
 
     #[test]
     fn test_build_endpoint() {
         let _ = tracing_subscriber::fmt().with_test_writer().try_init();
 
         let endpoint_cases = vec![
-            Some("s3.wasabisys.com"),
-            Some("https://s3.wasabisys.com"),
-            Some("https://s3.us-east-2.wasabisys.com"),
+            Some("s3.amazonaws.com"),
+            Some("https://s3.amazonaws.com"),
+            Some("https://s3.us-east-2.amazonaws.com"),
             None,
         ];
 
         for endpoint in &endpoint_cases {
-            let mut b = WasabiBuilder::default();
+            let mut b = S3Builder::default();
             b.bucket("test");
             if let Some(endpoint) = endpoint {
                 b.endpoint(endpoint);
             }
 
             let endpoint = b.build_endpoint("us-east-2");
-            assert_eq!(endpoint, "https://s3.us-east-2.wasabisys.com/test");
+            assert_eq!(endpoint, "https://s3.us-east-2.amazonaws.com/test");
         }
 
         for endpoint in &endpoint_cases {
-            let mut b = WasabiBuilder::default();
+            let mut b = S3Builder::default();
             b.bucket("test");
             b.enable_virtual_host_style();
             if let Some(endpoint) = endpoint {
                 b.endpoint(endpoint);
             }
 
             let endpoint = b.build_endpoint("us-east-2");
-            assert_eq!(endpoint, "https://test.s3.us-east-2.wasabisys.com");
+            assert_eq!(endpoint, "https://test.s3.us-east-2.amazonaws.com");
         }
     }
 }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/core.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/wasabi/core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 use http::Response;
 use reqsign::AwsCredential;
 use reqsign::AwsLoader;
 use reqsign::AwsV4Signer;
 use serde::Deserialize;
 use serde::Serialize;
 
-use crate::ops::OpStat;
 use crate::raw::*;
 use crate::*;
 
 mod constants {
     pub const X_AMZ_COPY_SOURCE: &str = "x-amz-copy-source";
 
     pub const X_AMZ_SERVER_SIDE_ENCRYPTION: &str = "x-amz-server-side-encryption";
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/wasabi/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/wasabi/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/wasabi/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/writer.rs`

 * *Files 10% similar despite different names*

```diff
@@ -11,55 +11,53 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::sync::Arc;
-
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::*;
+use super::backend::WebhdfsBackend;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct WasabiWriter {
-    core: Arc<WasabiCore>,
+pub struct WebhdfsWriter {
+    backend: WebhdfsBackend,
 
     op: OpWrite,
     path: String,
 }
 
-impl WasabiWriter {
-    pub fn new(core: Arc<WasabiCore>, op: OpWrite, path: String) -> Self {
-        WasabiWriter { core, op, path }
+impl WebhdfsWriter {
+    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
+        WebhdfsWriter { backend, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for WasabiWriter {
+impl oio::Write for WebhdfsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let resp = self
-            .core
-            .put_object(
+        let req = self
+            .backend
+            .webhdfs_create_object_request(
                 &self.path,
                 Some(bs.len()),
                 self.op.content_type(),
-                self.op.content_disposition(),
-                self.op.cache_control(),
                 AsyncBody::Bytes(bs),
             )
             .await?;
 
-        match resp.status() {
+        let resp = self.backend.client.send(req).await?;
+
+        let status = resp.status();
+        match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/webdav/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 use http::StatusCode;
 use log::debug;
 
 use super::error::parse_error;
 use super::list_response::Multistatus;
 use super::pager::WebdavPager;
 use super::writer::WebdavWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// [WebDAV](https://datatracker.ietf.org/doc/html/rfc4918) backend support.
 ///
 /// # Capabilities
 ///
@@ -195,15 +194,15 @@
     fn build(&mut self) -> Result<Self::Accessor> {
         debug!("backend build started: {:?}", &self);
 
         let endpoint = match &self.endpoint {
             Some(v) => v,
             None => {
                 return Err(Error::new(ErrorKind::ConfigInvalid, "endpoint is empty")
-                    .with_context("service", Scheme::Webdav))
+                    .with_context("service", Scheme::Webdav));
             }
         };
 
         let root = normalize_root(&self.root.take().unwrap_or_default());
         debug!("backend use root {}", root);
 
         let client = if let Some(client) = self.http_client.take() {
@@ -297,17 +296,15 @@
 
         let abs_path = build_abs_path(&self.root, path);
         self.create_internal(&abs_path).await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let resp = self.webdav_get(path, args.range()).await?;
-
         let status = resp.status();
-
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
@@ -448,15 +445,14 @@
 impl WebdavBackend {
     async fn webdav_get(
         &self,
         path: &str,
         range: BytesRange,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
-
         let url: String = format!("{}{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::get(&url);
 
         if let Some(auth) = &self.authorization {
             req = req.header(header::AUTHORIZATION, auth.clone())
         }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/webdav/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf` & `opendal-0.36.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/list_response.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/webdav/list_response.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/mod.rs`

 * *Files 16% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::WebdavBuilder as Webdav;
+pub use backend::WebhdfsBuilder as Webhdfs;
 
 mod error;
-mod list_response;
+mod message;
 mod pager;
 mod writer;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/webdav/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/webdav/writer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
 use super::backend::WebdavBackend;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct WebdavWriter {
     backend: WebdavBackend,
 
     op: OpWrite,
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/backend.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/backend.rs`

 * *Files 14% similar despite different names*

```diff
@@ -30,88 +30,22 @@
 use super::error::parse_error;
 use super::message::BooleanResp;
 use super::message::FileStatusType;
 use super::message::FileStatusWrapper;
 use super::message::FileStatusesWrapper;
 use super::pager::WebhdfsPager;
 use super::writer::WebhdfsWriter;
-use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 const WEBHDFS_DEFAULT_ENDPOINT: &str = "http://127.0.0.1:9870";
 
 /// [WebHDFS](https://hadoop.apache.org/docs/stable/hadoop-project-dist/hadoop-hdfs/WebHDFS.html)'s REST API support.
 ///
-/// There two implementations of WebHDFS REST API:
-///
-/// - Native via HDFS Namenode and Datanode, data are transferred between nodes directly.
-/// - [HttpFS](https://hadoop.apache.org/docs/stable/hadoop-hdfs-httpfs/index.html) is a gateway before hdfs nodes, data are proxied.
-///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [ ] copy
-/// - [ ] rename
-/// - [x] list
-/// - [ ] ~~scan~~
-/// - [ ] ~~presign~~
-/// - [ ] blocking
-///
-/// # Differences with hdfs
-///
-/// [Hdfs][crate::services::Hdfs] is powered by HDFS's native java client. Users need to setup the hdfs services correctly. But webhdfs can access from HTTP API and no extra setup needed.
-///
-/// # Configurations
-///
-/// - `root`: The root path of the WebHDFS service.
-/// - `endpoint`: The endpoint of the WebHDFS service.
-/// - `delegation`: The delegation token for WebHDFS.
-///
-/// Refer to [`Builder`]'s public API docs for more information
-///
-/// # Examples
-///
-/// ## Via Builder
-///
-/// ```no_run
-/// use std::sync::Arc;
-///
-/// use anyhow::Result;
-/// use opendal::services::Webhdfs;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     let mut builder = Webhdfs::default();
-///     // set the root for WebHDFS, all operations will happen under this root
-///     //
-///     // Note:
-///     // if the root is not exists, the builder will automatically create the
-///     // root directory for you
-///     // if the root exists and is a directory, the builder will continue working
-///     // if the root exists and is a folder, the builder will fail on building backend
-///     builder.root("/path/to/dir");
-///     // set the endpoint of webhdfs namenode, controlled by dfs.namenode.http-address
-///     // default is http://127.0.0.1:9870
-///     builder.endpoint("http://127.0.0.1:9870");
-///     // set the delegation_token for builder
-///     builder.delegation("delegation_token");
-///
-///     let op: Operator = Operator::new(builder)?.finish();
-///
-///     Ok(())
-/// }
-/// ```
+#[doc = include_str!("docs.md")]
 #[derive(Default, Clone)]
 pub struct WebhdfsBuilder {
     root: Option<String>,
     endpoint: Option<String>,
     delegation: Option<String>,
 }
 
@@ -265,40 +199,29 @@
             percent_encode_path(&p),
             op,
         );
         if let Some(auth) = &self.auth {
             url += format!("&{auth}").as_str();
         }
 
-        let req = Request::put(&url)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
+        let mut req = Request::put(&url);
 
         // mkdir does not redirect
         if path.ends_with('/') {
-            return Ok(req);
-        }
-
-        let resp = self.client.send(req).await?;
-
-        // should be a 307 TEMPORARY_REDIRECT
-        if resp.status() != StatusCode::TEMPORARY_REDIRECT {
-            return Err(parse_error(resp).await?);
+            return req.body(AsyncBody::Empty).map_err(new_request_build_error);
         }
-        let re_url = self.follow_redirect(resp)?;
 
-        let mut re_builder = Request::put(re_url);
         if let Some(size) = size {
-            re_builder = re_builder.header(CONTENT_LENGTH, size.to_string());
+            req = req.header(CONTENT_LENGTH, size.to_string());
         }
         if let Some(content_type) = content_type {
-            re_builder = re_builder.header(CONTENT_TYPE, content_type);
+            req = req.header(CONTENT_TYPE, content_type);
         }
 
-        re_builder.body(body).map_err(new_request_build_error)
+        req.body(body).map_err(new_request_build_error)
     }
 
     async fn webhdfs_open_request(
         &self,
         path: &str,
         range: &BytesRange,
     ) -> Result<Request<AsyncBody>> {
@@ -355,25 +278,14 @@
 
     async fn webhdfs_read_file(
         &self,
         path: &str,
         range: BytesRange,
     ) -> Result<Response<IncomingAsyncBody>> {
         let req = self.webhdfs_open_request(path, &range).await?;
-        let resp = self.client.send(req).await?;
-
-        // webhdfs namenode will redirect us to datanode for data transfer.
-        if resp.status() != StatusCode::TEMPORARY_REDIRECT {
-            return Err(parse_error(resp).await?);
-        }
-
-        let location = self.follow_redirect(resp)?;
-        let req = Request::get(&location)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
         self.client.send(req).await
     }
 
     async fn webhdfs_get_file_status(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let mut url = format!(
             "{}/webhdfs/v1/{}?op=GETFILESTATUS",
@@ -406,35 +318,14 @@
         let req = Request::delete(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.client.send(req).await
     }
 
-    /// get redirect destination from 307 TEMPORARY_REDIRECT http response
-    fn follow_redirect(&self, resp: Response<IncomingAsyncBody>) -> Result<String> {
-        let location = parse_location(resp.headers())?.ok_or_else(|| {
-            Error::new(
-                ErrorKind::Unexpected,
-                "webhdfs expect to have redirect location but got none",
-            )
-        })?;
-
-        let location = if location.starts_with('/') {
-            // location starts with `/` means it's a relative path to current
-            // endpoint. We should prepend the endpoint to it so that we can
-            // send request to the correct location.
-            format!("{}/{location}", self.endpoint)
-        } else {
-            location.to_string()
-        };
-
-        Ok(location)
-    }
-
     async fn check_root(&self) -> Result<()> {
         let resp = self.webhdfs_get_file_status("/").await?;
         match resp.status() {
             StatusCode::OK => {
                 let bs = resp.into_body().bytes().await?;
 
                 let file_status = serde_json::from_slice::<FileStatusWrapper>(&bs)
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/message.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/message.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/operator/mod.rs`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-mod backend;
-pub use backend::WebhdfsBuilder as Webhdfs;
+//! Operator's API will be split into different mods.
 
-mod error;
-mod message;
-mod pager;
-mod writer;
+#[allow(clippy::module_inception)]
+mod operator;
+pub use operator::Operator;
+
+mod blocking_operator;
+pub use blocking_operator::BlockingOperator;
+
+mod builder;
+pub use builder::OperatorBuilder;
+
+mod metadata;
+pub use metadata::OperatorInfo;
+
+pub mod operator_functions;
+pub mod operator_futures;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/pager.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/webhdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/services/azblob/writer.rs`

 * *Files 16% similar despite different names*

```diff
@@ -11,53 +11,55 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::sync::Arc;
+
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::WebhdfsBackend;
+use super::core::AzblobCore;
 use super::error::parse_error;
-use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct WebhdfsWriter {
-    backend: WebhdfsBackend,
+pub struct AzblobWriter {
+    core: Arc<AzblobCore>,
 
     op: OpWrite,
     path: String,
 }
 
-impl WebhdfsWriter {
-    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
-        WebhdfsWriter { backend, op, path }
+impl AzblobWriter {
+    pub fn new(core: Arc<AzblobCore>, op: OpWrite, path: String) -> Self {
+        AzblobWriter { core, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for WebhdfsWriter {
+impl oio::Write for AzblobWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let req = self
-            .backend
-            .webhdfs_create_object_request(
-                &self.path,
-                Some(bs.len()),
-                self.op.content_type(),
-                AsyncBody::Bytes(bs),
-            )
-            .await?;
+        let mut req = self.core.azblob_put_blob_request(
+            &self.path,
+            Some(bs.len()),
+            self.op.content_type(),
+            self.op.cache_control(),
+            AsyncBody::Bytes(bs),
+        )?;
+
+        self.core.sign(&mut req).await?;
 
-        let resp = self.backend.client.send(req).await?;
+        let resp = self.core.send(req).await?;
 
         let status = resp.status();
+
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/appender.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/appender.rs`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 use std::task::Poll;
 
 use bytes::Bytes;
 use futures::future::BoxFuture;
 use futures::AsyncWrite;
 use futures::FutureExt;
 
-use crate::ops::OpAppend;
 use crate::raw::oio::Append;
 use crate::raw::*;
 use crate::*;
 
 /// Appender is designed to append data into given path in an asynchronous
 /// manner.
 ///
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/builder.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/capability.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/capability.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/entry.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/error.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/list.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/list.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/metadata.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/metadata.rs`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 use chrono::prelude::*;
 use flagset::flags;
 use flagset::FlagSet;
 
 use crate::raw::*;
 use crate::*;
 
-/// Metadata carries all metadata associated with an path.
+/// Metadata carries all metadata associated with a path.
 ///
 /// # Notes
 ///
 /// mode and content_length are required metadata that all services
 /// should provide during `stat` operation. But in `list` operation,
 /// a.k.a., `Entry`'s content length could be `None`.
 #[derive(Debug, Clone, Eq, PartialEq)]
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/mod.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 pub use appender::Appender;
 
 mod list;
 pub use list::BlockingLister;
 pub use list::Lister;
 
 mod operator;
+pub use operator::operator_functions;
+pub use operator::operator_futures;
 pub use operator::BlockingOperator;
 pub use operator::Operator;
 pub use operator::OperatorBuilder;
 pub use operator::OperatorInfo;
 
 mod builder;
 pub use builder::Builder;
@@ -55,9 +57,7 @@
 pub use error::Result;
 
 mod scheme;
 pub use scheme::Scheme;
 
 mod capability;
 pub use capability::Capability;
-
-pub mod ops;
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/mode.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/mode.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 use std::io::Read;
 use std::ops::RangeBounds;
 
 use bytes::Bytes;
 use flagset::FlagSet;
 
-use crate::ops::*;
+use super::operator_functions::*;
 use crate::raw::*;
 use crate::*;
 
 /// BlockingOperator is the entry for all public blocking APIs.
 ///
 /// Read [`concepts`][docs::concepts] for know more about [`Operator`].
 ///
@@ -444,20 +444,15 @@
     ///
     /// # fn test(op: BlockingOperator) -> Result<()> {
     /// op.write("path/to/file", vec![0; 4096])?;
     /// # Ok(())
     /// # }
     /// ```
     pub fn write(&self, path: &str, bs: impl Into<Bytes>) -> Result<()> {
-        let bs = bs.into();
-        self.write_with(
-            path,
-            OpWrite::new().with_content_length(bs.len() as u64),
-            bs,
-        )
+        self.write_with(path, bs).call()
     }
 
     /// Copy a file from `from` to `to`.
     ///
     /// # Notes
     ///
     /// - `from` and `to` must be a file.
@@ -579,43 +574,50 @@
     ///
     /// # Examples
     ///
     /// ```no_run
     /// # use opendal::Result;
     /// # use opendal::BlockingOperator;
     /// use bytes::Bytes;
-    /// use opendal::ops::OpWrite;
     ///
     /// # async fn test(op: BlockingOperator) -> Result<()> {
     /// let bs = b"hello, world!".to_vec();
-    /// let ow = OpWrite::new().with_content_type("text/plain");
-    /// let _ = op.write_with("hello.txt", ow, bs)?;
+    /// let _ = op
+    ///     .write_with("hello.txt", bs)
+    ///     .content_type("text/plain")
+    ///     .call()?;
     /// # Ok(())
     /// # }
     /// ```
-    pub fn write_with(&self, path: &str, args: OpWrite, bs: impl Into<Bytes>) -> Result<()> {
+    pub fn write_with(&self, path: &str, bs: impl Into<Bytes>) -> FunctionWrite {
         let path = normalize_path(path);
 
-        if !validate_path(&path, EntryMode::FILE) {
-            return Err(
-                Error::new(ErrorKind::IsADirectory, "write path is a directory")
-                    .with_operation("BlockingOperator::write_with")
-                    .with_context("service", self.info().scheme().into_static())
-                    .with_context("path", &path),
-            );
-        }
-
         let bs = bs.into();
-        let (_, mut w) = self
-            .inner()
-            .blocking_write(&path, args.with_content_length(bs.len() as u64))?;
-        w.write(bs)?;
-        w.close()?;
 
-        Ok(())
+        FunctionWrite(OperatorFunction::new(
+            self.inner().clone(),
+            path,
+            (OpWrite::default().with_content_length(bs.len() as u64), bs),
+            |inner, path, (args, bs)| {
+                if !validate_path(&path, EntryMode::FILE) {
+                    return Err(
+                        Error::new(ErrorKind::IsADirectory, "write path is a directory")
+                            .with_operation("BlockingOperator::write_with")
+                            .with_context("service", inner.info().scheme().into_static())
+                            .with_context("path", &path),
+                    );
+                }
+
+                let (_, mut w) = inner.blocking_write(&path, args)?;
+                w.write(bs)?;
+                w.close()?;
+
+                Ok(())
+            },
+        ))
     }
 
     /// Write multiple bytes into given path.
     ///
     /// # Notes
     ///
     /// - Write will make sure all bytes has been written, or an error will be returned.
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/operator/builder.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/operator/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/operator/metadata.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/operator/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/operator/operator.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/operator/operator.rs`

 * *Files 9% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 use futures::AsyncReadExt;
 use futures::Stream;
 use futures::StreamExt;
 use futures::TryStreamExt;
 use tokio::io::ReadBuf;
 
 use super::BlockingOperator;
-use crate::ops::*;
+use crate::operator_futures::*;
 use crate::raw::*;
 use crate::*;
 
 /// Operator is the entry for all public async APIs.
+///
 /// Developer should manipulate the data from storage service through Operator only by right.
 ///
 /// We will usually do some general checks and data transformations in this layer,
 /// like normalizing path from input, checking whether the path refers to one file or one directory, and so on.
 /// Read [`concepts`][docs::concepts] for more about [`Operator`].
 ///
 /// # Examples
@@ -186,15 +187,15 @@
     ///         println!("file not exist")
     ///     }
     /// }
     /// # Ok(())
     /// # }
     /// ```
     pub async fn stat(&self, path: &str) -> Result<Metadata> {
-        self.stat_with(path, OpStat::new()).await
+        self.stat_with(path).await
     }
 
     /// Get current path's metadata **without cache** directly with extra options.
     ///
     /// # Notes
     ///
     /// Use `stat` if you:
@@ -208,34 +209,44 @@
     ///
     /// # Examples
     ///
     /// ```
     /// # use anyhow::Result;
     /// # use futures::io;
     /// # use opendal::Operator;
-    /// # use opendal::ops::OpStat;
     /// use opendal::ErrorKind;
     /// #
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
-    /// if let Err(e) = op.stat_with("test", OpStat::new()).await {
+    /// if let Err(e) = op.stat_with("test").if_match("<etag>").await {
     ///     if e.kind() == ErrorKind::NotFound {
     ///         println!("file not exist")
     ///     }
     /// }
     /// # Ok(())
     /// # }
     /// ```
-    pub async fn stat_with(&self, path: &str, args: OpStat) -> Result<Metadata> {
+    pub fn stat_with(&self, path: &str) -> FutureStat {
         let path = normalize_path(path);
 
-        let rp = self.inner().stat(&path, args).await?;
-        let meta = rp.into_metadata();
+        let fut = FutureStat(OperatorFuture::new(
+            self.inner().clone(),
+            path,
+            OpStat::default(),
+            |inner, path, args| {
+                let fut = async move {
+                    let rp = inner.stat(&path, args).await?;
+                    Ok(rp.into_metadata())
+                };
 
-        Ok(meta)
+                Box::pin(fut)
+            },
+        ));
+
+        fut
     }
 
     /// Get current metadata with cache.
     ///
     /// `metadata` will check the given query with already cached metadata
     ///  first. And query from storage if not found.
     ///
@@ -432,24 +443,73 @@
     /// reading data lazily, please use [`Operator::reader`]
     ///
     /// # Examples
     ///
     /// ```
     /// # use std::io::Result;
     /// # use opendal::Operator;
-    /// # use opendal::ops::OpRead;
     /// # use futures::TryStreamExt;
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
-    /// let bs = op.read_with("path/to/file", OpRead::new()).await?;
+    /// let bs = op.read_with("path/to/file").await?;
     /// # Ok(())
     /// # }
     /// ```
-    pub async fn read_with(&self, path: &str, args: OpRead) -> Result<Vec<u8>> {
-        self.range_read_with(path, .., args).await
+    pub fn read_with(&self, path: &str) -> FutureRead {
+        let path = normalize_path(path);
+
+        let fut = FutureRead(OperatorFuture::new(
+            self.inner().clone(),
+            path,
+            OpRead::default(),
+            |inner, path, args| {
+                let fut = async move {
+                    if !validate_path(&path, EntryMode::FILE) {
+                        return Err(Error::new(
+                            ErrorKind::IsADirectory,
+                            "read path is a directory",
+                        )
+                        .with_operation("range_read")
+                        .with_context("service", inner.info().scheme())
+                        .with_context("path", &path));
+                    }
+
+                    let br = args.range();
+                    let (rp, mut s) = inner.read(&path, args).await?;
+
+                    let length = rp.into_metadata().content_length() as usize;
+                    let mut buffer = Vec::with_capacity(length);
+
+                    let dst = buffer.spare_capacity_mut();
+                    let mut buf = ReadBuf::uninit(dst);
+
+                    // Safety: the input buffer is created with_capacity(length).
+                    unsafe { buf.assume_init(length) };
+
+                    // TODO: use native read api
+                    s.read_exact(buf.initialized_mut()).await.map_err(|err| {
+                        Error::new(ErrorKind::Unexpected, "read from storage")
+                            .with_operation("range_read")
+                            .with_context("service", inner.info().scheme().into_static())
+                            .with_context("path", &path)
+                            .with_context("range", br.to_string())
+                            .set_source(err)
+                    })?;
+
+                    // Safety: read_exact makes sure this buffer has been filled.
+                    unsafe { buffer.set_len(length) }
+
+                    Ok(buffer)
+                };
+
+                Box::pin(fut)
+            },
+        ));
+
+        fut
     }
 
     /// Read the specified range of path into a bytes.
     ///
     /// This function will allocate a new bytes internally. For more precise memory control or
     /// reading data lazily, please use [`Operator::range_reader`]
     ///
@@ -458,94 +518,23 @@
     /// - The returning content's length may be smaller than the range specified.
     ///
     /// # Examples
     ///
     /// ```
     /// # use std::io::Result;
     /// # use opendal::Operator;
-    /// # use opendal::ops::OpRead;
     /// # use futures::TryStreamExt;
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
     /// let bs = op.range_read("path/to/file", 1024..2048).await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn range_read(&self, path: &str, range: impl RangeBounds<u64>) -> Result<Vec<u8>> {
-        self.range_read_with(path, range, OpRead::new()).await
-    }
-
-    /// Read the specified range of path into a bytes with extra options..
-    ///
-    /// This function will allocate a new bytes internally. For more precise memory control or
-    /// reading data lazily, please use [`Operator::range_reader`]
-    ///
-    /// # Notes
-    ///
-    /// - The returning content's length may be smaller than the range specified.
-    ///
-    /// # Examples
-    ///
-    /// ```
-    /// # use std::io::Result;
-    /// # use opendal::Operator;
-    /// # use opendal::ops::OpRead;
-    /// # use futures::TryStreamExt;
-    /// # #[tokio::main]
-    /// # async fn test(op: Operator) -> Result<()> {
-    /// let bs = op
-    ///     .range_read_with("path/to/file", 1024..2048, OpRead::new())
-    ///     .await?;
-    /// # Ok(())
-    /// # }
-    /// ```
-    pub async fn range_read_with(
-        &self,
-        path: &str,
-        range: impl RangeBounds<u64>,
-        args: OpRead,
-    ) -> Result<Vec<u8>> {
-        let path = normalize_path(path);
-
-        if !validate_path(&path, EntryMode::FILE) {
-            return Err(
-                Error::new(ErrorKind::IsADirectory, "read path is a directory")
-                    .with_operation("range_read")
-                    .with_context("service", self.inner().info().scheme())
-                    .with_context("path", &path),
-            );
-        }
-
-        let br = BytesRange::from(range);
-
-        let (rp, mut s) = self.inner().read(&path, args.with_range(br)).await?;
-
-        let length = rp.into_metadata().content_length() as usize;
-        let mut buffer = Vec::with_capacity(length);
-
-        let dst = buffer.spare_capacity_mut();
-        let mut buf = ReadBuf::uninit(dst);
-
-        // Safety: the input buffer is created with_capacity(length).
-        unsafe { buf.assume_init(length) };
-
-        // TODO: use native read api
-        s.read_exact(buf.initialized_mut()).await.map_err(|err| {
-            Error::new(ErrorKind::Unexpected, "read from storage")
-                .with_operation("range_read")
-                .with_context("service", self.inner().info().scheme().into_static())
-                .with_context("path", &path)
-                .with_context("range", br.to_string())
-                .set_source(err)
-        })?;
-
-        // Safety: read_exact makes sure this buffer has been filled.
-        unsafe { buffer.set_len(length) }
-
-        Ok(buffer)
+        self.read_with(path).range(range).await
     }
 
     /// Create a new reader which can read the whole path.
     ///
     /// # Examples
     ///
     /// ```no_run
@@ -556,15 +545,15 @@
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
     /// let r = op.reader("path/to/file").await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn reader(&self, path: &str) -> Result<Reader> {
-        self.reader_with(path, OpRead::default()).await
+        self.reader_with(path).await
     }
 
     /// Create a new reader which can read the specified range.
     ///
     /// # Notes
     ///
     /// - The returning content's length may be smaller than the range specified.
@@ -578,49 +567,58 @@
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
     /// let r = op.range_reader("path/to/file", 1024..2048).await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn range_reader(&self, path: &str, range: impl RangeBounds<u64>) -> Result<Reader> {
-        self.reader_with(path, OpRead::new().with_range(range.into()))
-            .await
+        self.reader_with(path).range(range).await
     }
 
     /// Create a new reader with extra options
     ///
     /// # Examples
     ///
     /// ```no_run
     /// # use std::io::Result;
     /// # use opendal::Operator;
     /// # use futures::TryStreamExt;
     /// # use opendal::Scheme;
-    /// # use opendal::ops::OpRead;
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
-    /// let r = op
-    ///     .reader_with("path/to/file", OpRead::default().with_range((0..10).into()))
-    ///     .await?;
+    /// let r = op.reader_with("path/to/file").range((0..10)).await?;
     /// # Ok(())
     /// # }
     /// ```
-    pub async fn reader_with(&self, path: &str, args: OpRead) -> Result<Reader> {
+    pub fn reader_with(&self, path: &str) -> FutureReader {
         let path = normalize_path(path);
 
-        if !validate_path(&path, EntryMode::FILE) {
-            return Err(
-                Error::new(ErrorKind::IsADirectory, "read path is a directory")
-                    .with_operation("Operator::range_reader")
-                    .with_context("service", self.info().scheme())
-                    .with_context("path", path),
-            );
-        }
+        let fut = FutureReader(OperatorFuture::new(
+            self.inner().clone(),
+            path,
+            OpRead::default(),
+            |inner, path, args| {
+                let fut = async move {
+                    if !validate_path(&path, EntryMode::FILE) {
+                        return Err(Error::new(
+                            ErrorKind::IsADirectory,
+                            "read path is a directory",
+                        )
+                        .with_operation("Operator::range_reader")
+                        .with_context("service", inner.info().scheme())
+                        .with_context("path", path));
+                    }
+
+                    Reader::create_dir(inner.clone(), &path, args).await
+                };
 
-        Reader::create_dir(self.inner().clone(), &path, args).await
+                Box::pin(fut)
+            },
+        ));
+        fut
     }
 
     /// Write bytes into path.
     ///
     /// # Notes
     ///
     /// - Write will make sure all bytes has been written, or an error will be returned.
@@ -638,20 +636,15 @@
     /// # async fn test(op: Operator) -> Result<()> {
     /// op.write("path/to/file", vec![0; 4096]).await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn write(&self, path: &str, bs: impl Into<Bytes>) -> Result<()> {
         let bs = bs.into();
-        self.write_with(
-            path,
-            OpWrite::new().with_content_length(bs.len() as u64),
-            bs,
-        )
-        .await
+        self.write_with(path, bs).await
     }
 
     /// Append bytes into path.
     ///
     /// # Notes
     ///
     /// - Append will make sure all bytes has been written, or an error will be returned.
@@ -669,15 +662,15 @@
     /// # async fn test(op: Operator) -> Result<()> {
     /// op.append("path/to/file", vec![0; 4096]).await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn append(&self, path: &str, bs: impl Into<Bytes>) -> Result<()> {
         let bs = bs.into();
-        self.append_with(path, OpAppend::new(), bs).await
+        self.append_with(path, bs).await
     }
 
     /// Copy a file from `from` to `to`.
     ///
     /// # Notes
     ///
     /// - `from` and `to` must be a file.
@@ -812,99 +805,123 @@
     /// w.write(vec![0; 4096]).await?;
     /// w.write(vec![1; 4096]).await?;
     /// w.close().await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn writer(&self, path: &str) -> Result<Writer> {
-        self.writer_with(path, OpWrite::default()).await
+        self.writer_with(path).await
     }
 
     /// Write multiple bytes into path with extra options.
     ///
     /// Refer to [`Writer`] for more details.
     ///
     /// # Examples
     ///
     /// ```
     /// # use std::io::Result;
     /// # use opendal::Operator;
     /// # use futures::StreamExt;
     /// # use futures::SinkExt;
     /// use bytes::Bytes;
-    /// use opendal::ops::OpWrite;
     ///
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
-    /// let args = OpWrite::new().with_content_type("application/octet-stream");
-    /// let mut w = op.writer_with("path/to/file", args).await?;
+    /// let mut w = op
+    ///     .writer_with("path/to/file")
+    ///     .content_type("application/octet-stream")
+    ///     .await?;
     /// w.write(vec![0; 4096]).await?;
     /// w.write(vec![1; 4096]).await?;
     /// w.close().await?;
     /// # Ok(())
     /// # }
     /// ```
-    pub async fn writer_with(&self, path: &str, args: OpWrite) -> Result<Writer> {
+    pub fn writer_with(&self, path: &str) -> FutureWriter {
         let path = normalize_path(path);
 
-        if !validate_path(&path, EntryMode::FILE) {
-            return Err(
-                Error::new(ErrorKind::IsADirectory, "write path is a directory")
-                    .with_operation("Operator::writer")
-                    .with_context("service", self.inner().info().scheme().into_static())
-                    .with_context("path", &path),
-            );
-        }
+        let fut = FutureWriter(OperatorFuture::new(
+            self.inner().clone(),
+            path,
+            OpWrite::default(),
+            |inner, path, args| {
+                let fut = async move {
+                    if !validate_path(&path, EntryMode::FILE) {
+                        return Err(Error::new(
+                            ErrorKind::IsADirectory,
+                            "write path is a directory",
+                        )
+                        .with_operation("Operator::writer")
+                        .with_context("service", inner.info().scheme().into_static())
+                        .with_context("path", &path));
+                    }
+
+                    Writer::create(inner, &path, args).await
+                };
+                Box::pin(fut)
+            },
+        ));
 
-        Writer::create(self.inner().clone(), &path, args).await
+        fut
     }
 
     /// Write data with extra options.
     ///
     /// # Notes
     ///
     /// - Write will make sure all bytes has been written, or an error will be returned.
     ///
     /// # Examples
     ///
     /// ```no_run
     /// # use std::io::Result;
     /// # use opendal::Operator;
     /// use bytes::Bytes;
-    /// use opendal::ops::OpWrite;
     ///
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
     /// let bs = b"hello, world!".to_vec();
-    /// let args = OpWrite::new().with_content_type("text/plain");
-    /// let _ = op.write_with("path/to/file", args, bs).await?;
+    /// let _ = op
+    ///     .write_with("path/to/file", bs)
+    ///     .content_type("text/plain")
+    ///     .await?;
     /// # Ok(())
     /// # }
     /// ```
-    pub async fn write_with(&self, path: &str, args: OpWrite, bs: impl Into<Bytes>) -> Result<()> {
+    pub fn write_with(&self, path: &str, bs: impl Into<Bytes>) -> FutureWrite {
         let path = normalize_path(path);
-
-        if !validate_path(&path, EntryMode::FILE) {
-            return Err(
-                Error::new(ErrorKind::IsADirectory, "write path is a directory")
-                    .with_operation("Operator::write_with")
-                    .with_context("service", self.info().scheme().into_static())
-                    .with_context("path", &path),
-            );
-        }
-
         let bs = bs.into();
-        let (_, mut w) = self
-            .inner()
-            .write(&path, args.with_content_length(bs.len() as u64))
-            .await?;
-        w.write(bs).await?;
-        w.close().await?;
 
-        Ok(())
+        let fut = FutureWrite(OperatorFuture::new(
+            self.inner().clone(),
+            path,
+            (OpWrite::default().with_content_length(bs.len() as u64), bs),
+            |inner, path, (args, bs)| {
+                let fut = async move {
+                    if !validate_path(&path, EntryMode::FILE) {
+                        return Err(Error::new(
+                            ErrorKind::IsADirectory,
+                            "write path is a directory",
+                        )
+                        .with_operation("Operator::write_with")
+                        .with_context("service", inner.info().scheme().into_static())
+                        .with_context("path", &path));
+                    }
+
+                    let (_, mut w) = inner.write(&path, args).await?;
+                    w.write(bs).await?;
+                    w.close().await?;
+
+                    Ok(())
+                };
+                Box::pin(fut)
+            },
+        ));
+        fut
     }
 
     /// Append multiple bytes into path.
     ///
     /// Refer to [`Appender`] for more details.
     ///
     /// # Examples
@@ -920,52 +937,67 @@
     /// a.append(vec![0; 4096]).await?;
     /// a.append(vec![1; 4096]).await?;
     /// a.close().await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn appender(&self, path: &str) -> Result<Appender> {
-        self.appender_with(path, OpAppend::default()).await
+        self.appender_with(path).await
     }
 
     /// Append multiple bytes into path with extra options.
     ///
     /// Refer to [`Appender`] for more details.
     ///
     /// # Examples
     ///
     /// ```
     /// # use std::io::Result;
     /// # use opendal::Operator;
     /// use bytes::Bytes;
-    /// use opendal::ops::OpAppend;
     ///
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
-    /// let args = OpAppend::new().with_content_type("application/octet-stream");
-    /// let mut a = op.appender_with("path/to/file", args).await?;
+    /// let mut a = op
+    ///     .appender_with("path/to/file")
+    ///     .content_type("application/octet-stream")
+    ///     .await?;
     /// a.append(vec![0; 4096]).await?;
     /// a.append(vec![1; 4096]).await?;
     /// a.close().await?;
     /// # Ok(())
     /// # }
     /// ```
-    pub async fn appender_with(&self, path: &str, args: OpAppend) -> Result<Appender> {
+    pub fn appender_with(&self, path: &str) -> FutureAppender {
         let path = normalize_path(path);
 
-        if !validate_path(&path, EntryMode::FILE) {
-            return Err(
-                Error::new(ErrorKind::IsADirectory, "append path is a directory")
-                    .with_operation("Operator::appender")
-                    .with_context("service", self.inner().info().scheme().into_static())
-                    .with_context("path", &path),
-            );
-        }
+        let fut = FutureAppender(OperatorFuture::new(
+            self.inner().clone(),
+            path,
+            OpAppend::default(),
+            |inner, path, args| {
+                let fut = async move {
+                    if !validate_path(&path, EntryMode::FILE) {
+                        return Err(Error::new(
+                            ErrorKind::IsADirectory,
+                            "append path is a directory",
+                        )
+                        .with_operation("Operator::appender")
+                        .with_context("service", inner.info().scheme().into_static())
+                        .with_context("path", &path));
+                    }
+                    let ap = Appender::create(inner, &path, args).await?;
+                    Ok(ap)
+                };
 
-        Appender::create(self.inner().clone(), &path, args).await
+                Box::pin(fut)
+            },
+        ));
+
+        fut
     }
 
     /// Append bytes with extra options.
     ///
     /// # Notes
     ///
     /// - Append will make sure all bytes has been written, or an error will be returned.
@@ -974,47 +1006,56 @@
     ///
     /// # Examples
     ///
     /// ```
     /// # use std::io::Result;
     /// # use opendal::Operator;
     /// use bytes::Bytes;
-    /// use opendal::ops::OpAppend;
     ///
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
     /// let bs = b"hello, world!".to_vec();
-    /// let args = OpAppend::new().with_content_type("text/plain");
-    /// let _ = op.append_with("path/to/file", args, bs).await?;
+    /// let _ = op
+    ///     .append_with("path/to/file", bs)
+    ///     .content_type("text/plain")
+    ///     .await?;
     /// # Ok(())
     /// # }
     /// ```
-    pub async fn append_with(
-        &self,
-        path: &str,
-        args: OpAppend,
-        bs: impl Into<Bytes>,
-    ) -> Result<()> {
+    pub fn append_with(&self, path: &str, bs: impl Into<Bytes>) -> FutureAppend {
         let path = normalize_path(path);
+        let bs = bs.into();
 
-        if !validate_path(&path, EntryMode::FILE) {
-            return Err(
-                Error::new(ErrorKind::IsADirectory, "append path is a directory")
-                    .with_operation("Operator::append_with")
-                    .with_context("service", self.info().scheme().into_static())
-                    .with_context("path", &path),
-            );
-        }
+        let fut = FutureAppend(OperatorFuture::new(
+            self.inner().clone(),
+            path,
+            (OpAppend::default(), bs),
+            |inner, path, (args, bs)| {
+                let fut = async move {
+                    if !validate_path(&path, EntryMode::FILE) {
+                        return Err(Error::new(
+                            ErrorKind::IsADirectory,
+                            "append path is a directory",
+                        )
+                        .with_operation("Operator::append_with")
+                        .with_context("service", inner.info().scheme().into_static())
+                        .with_context("path", &path));
+                    }
+                    let (_, mut a) = inner.append(&path, args).await?;
+                    a.append(bs).await?;
+                    a.close().await?;
 
-        let bs = bs.into();
-        let (_, mut a) = self.inner().append(&path, args).await?;
-        a.append(bs).await?;
-        a.close().await?;
+                    Ok(())
+                };
 
-        Ok(())
+                Box::pin(fut)
+            },
+        ));
+
+        fut
     }
 
     /// Delete the given path.
     ///
     /// # Notes
     ///
     /// - Deleting a file that does not exist won't return errors.
@@ -1220,15 +1261,15 @@
     ///         EntryMode::Unknown => continue,
     ///     }
     /// }
     /// # Ok(())
     /// # }
     /// ```
     pub async fn list(&self, path: &str) -> Result<Lister> {
-        self.list_with(path, OpList::new()).await
+        self.list_with(path).await
     }
 
     /// List given path with OpList.
     ///
     /// This function will create a new handle to list entries.
     ///
     /// An error will be returned if given path doesn't end with `/`.
@@ -1237,22 +1278,24 @@
     ///
     /// ## List current dir
     ///
     /// ```no_run
     /// # use anyhow::Result;
     /// # use futures::io;
     /// use futures::TryStreamExt;
-    /// use opendal::ops::OpList;
     /// use opendal::EntryMode;
     /// use opendal::Metakey;
     /// use opendal::Operator;
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
-    /// let option = OpList::new().with_limit(10).with_start_after("start");
-    /// let mut ds = op.list_with("path/to/dir/", option).await?;
+    /// let mut ds = op
+    ///     .list_with("path/to/dir/")
+    ///     .limit(10)
+    ///     .start_after("start")
+    ///     .await?;
     /// while let Some(mut de) = ds.try_next().await? {
     ///     let meta = op.metadata(&de, Metakey::Mode).await?;
     ///     match meta.mode() {
     ///         EntryMode::FILE => {
     ///             println!("Handling file")
     ///         }
     ///         EntryMode::DIR => {
@@ -1269,22 +1312,20 @@
     ///
     /// We can use `op.scan()` as a shorter alias.
     ///
     /// ```no_run
     /// # use anyhow::Result;
     /// # use futures::io;
     /// use futures::TryStreamExt;
-    /// use opendal::ops::OpList;
     /// use opendal::EntryMode;
     /// use opendal::Metakey;
     /// use opendal::Operator;
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
-    /// let option = OpList::new().with_delimiter("");
-    /// let mut ds = op.list_with("path/to/dir/", option).await?;
+    /// let mut ds = op.list_with("path/to/dir/").delimiter("").await?;
     /// while let Some(mut de) = ds.try_next().await? {
     ///     let meta = op.metadata(&de, Metakey::Mode).await?;
     ///     match meta.mode() {
     ///         EntryMode::FILE => {
     ///             println!("Handling file")
     ///         }
     ///         EntryMode::DIR => {
@@ -1292,42 +1333,53 @@
     ///         }
     ///         EntryMode::Unknown => continue,
     ///     }
     /// }
     /// # Ok(())
     /// # }
     /// ```
-    pub async fn list_with(&self, path: &str, op: OpList) -> Result<Lister> {
+    pub fn list_with(&self, path: &str) -> FutureList {
         let path = normalize_path(path);
 
-        if !validate_path(&path, EntryMode::DIR) {
-            return Err(Error::new(
-                ErrorKind::NotADirectory,
-                "the path trying to list should end with `/`",
-            )
-            .with_operation("Operator::list")
-            .with_context("service", self.info().scheme().into_static())
-            .with_context("path", &path));
-        }
-
-        let (_, pager) = self.inner().list(&path, op).await?;
-
-        Ok(Lister::new(pager))
+        let fut = FutureList(OperatorFuture::new(
+            self.inner().clone(),
+            path,
+            OpList::default(),
+            |inner, path, args| {
+                let fut = async move {
+                    if !validate_path(&path, EntryMode::DIR) {
+                        return Err(Error::new(
+                            ErrorKind::NotADirectory,
+                            "the path trying to list should end with `/`",
+                        )
+                        .with_operation("Operator::list")
+                        .with_context("service", inner.info().scheme().into_static())
+                        .with_context("path", &path));
+                    }
+
+                    let (_, pager) = inner.list(&path, args).await?;
+
+                    Ok(Lister::new(pager))
+                };
+                Box::pin(fut)
+            },
+        ));
+        fut
     }
 
     /// List dir in flat way.
     ///
     /// Also, this function can be used to list a prefix.
     ///
     /// An error will be returned if given path doesn't end with `/`.
     ///
     /// # Notes
     ///
     /// - `scan` will not return the prefix itself.
-    /// - `scan` is an alias of `list_with(OpList::new().with_delimiter(""))`
+    /// - `scan` is an alias of `list_with(path).delimiter("")`
     ///
     /// # Examples
     ///
     /// ```no_run
     /// # use anyhow::Result;
     /// # use futures::io;
     /// use futures::TryStreamExt;
@@ -1350,35 +1402,17 @@
     ///         EntryMode::Unknown => continue,
     ///     }
     /// }
     /// # Ok(())
     /// # }
     /// ```
     pub async fn scan(&self, path: &str) -> Result<Lister> {
-        let path = normalize_path(path);
-
-        if !validate_path(&path, EntryMode::DIR) {
-            return Err(Error::new(
-                ErrorKind::NotADirectory,
-                "the path trying to scan should end with `/`",
-            )
-            .with_operation("list")
-            .with_context("service", self.info().scheme().into_static())
-            .with_context("path", &path));
-        }
-
-        let (_, pager) = self
-            .inner()
-            .list(&path, OpList::new().with_delimiter(""))
-            .await?;
-
-        Ok(Lister::new(pager))
+        self.list_with(path).delimiter("").await
     }
 }
-
 /// Operator presign API.
 impl Operator {
     /// Presign an operation for stat(head).
     ///
     /// # Example
     ///
     /// ```no_run
@@ -1449,36 +1483,41 @@
     /// # Example
     ///
     /// ```no_run
     /// use anyhow::Result;
     /// use futures::io;
     /// use opendal::Operator;
     /// use std::time::Duration;
-    /// use opendal::ops::OpRead;
     ///
     /// #[tokio::main]
     /// async fn test(op: Operator) -> Result<()> {
-    ///     let args = OpRead::new()
-    ///         .with_override_content_disposition("attachment; filename=\"othertext.txt\"");
-    ///     let signed_req = op.presign_read_with("test.txt", args, Duration::from_secs(3600)).await?;
+    ///     let signed_req = op
+    ///         .presign_read_with("test.txt", Duration::from_secs(3600))
+    ///         .override_content_disposition("attachment; filename=\"othertext.txt\"")
+    ///         .await?;
     /// #    Ok(())
     /// # }
     /// ```
-    pub async fn presign_read_with(
-        &self,
-        path: &str,
-        op: OpRead,
-        expire: Duration,
-    ) -> Result<PresignedRequest> {
+    pub fn presign_read_with(&self, path: &str, expire: Duration) -> FuturePresignRead {
         let path = normalize_path(path);
 
-        let op = OpPresign::new(op, expire);
-
-        let rp = self.inner().presign(&path, op).await?;
-        Ok(rp.into_presigned_request())
+        let fut = FuturePresignRead(OperatorFuture::new(
+            self.inner().clone(),
+            path,
+            (OpRead::default(), expire),
+            |inner, path, (args, dur)| {
+                let fut = async move {
+                    let op = OpPresign::new(args, dur);
+                    let rp = inner.presign(&path, op).await?;
+                    Ok(rp.into_presigned_request())
+                };
+                Box::pin(fut)
+            },
+        ));
+        fut
     }
 
     /// Presign an operation for write.
     ///
     /// # Example
     ///
     /// ```no_run
@@ -1500,49 +1539,53 @@
     ///
     /// We can upload file as this file via `curl` or other tools without credential:
     ///
     /// ```shell
     /// curl -X PUT "https://s3.amazonaws.com/examplebucket/test.txt?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=access_key_id/20130721/us-east-1/s3/aws4_request&X-Amz-Date=20130721T201207Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=<signature-value>" -d "Hello, World!"
     /// ```
     pub async fn presign_write(&self, path: &str, expire: Duration) -> Result<PresignedRequest> {
-        self.presign_write_with(path, OpWrite::new(), expire).await
+        self.presign_write_with(path, expire).await
     }
 
     /// Presign an operation for write with option described in OpenDAL [rfc-0661](../../docs/rfcs/0661-path-in-accessor.md)
     ///
     /// You can pass `OpWrite` to this method to specify the content length and content type.
     ///
     /// # Example
     ///
     /// ```no_run
     /// use anyhow::Result;
     /// use futures::io;
-    /// use opendal::ops::OpWrite;
     /// use opendal::Operator;
     /// use std::time::Duration;
     ///
     /// #[tokio::main]
     /// async fn test(op: Operator) -> Result<()> {
-    ///     let args = OpWrite::new().with_content_type("text/csv");
-    ///     let signed_req = op.presign_write_with("test", args, Duration::from_secs(3600)).await?;
+    ///     let signed_req = op.presign_write_with("test", Duration::from_secs(3600))
+    ///                        .content_type("text/csv").await?;
     ///     let req = http::Request::builder()
     ///         .method(signed_req.method())
     ///         .uri(signed_req.uri())
     ///         .body(())?;
     ///
     /// #    Ok(())
     /// # }
     /// ```
-    pub async fn presign_write_with(
-        &self,
-        path: &str,
-        op: OpWrite,
-        expire: Duration,
-    ) -> Result<PresignedRequest> {
+    pub fn presign_write_with(&self, path: &str, expire: Duration) -> FuturePresignWrite {
         let path = normalize_path(path);
 
-        let op = OpPresign::new(op, expire);
-
-        let rp = self.inner().presign(&path, op).await?;
-        Ok(rp.into_presigned_request())
+        let fut = FuturePresignWrite(OperatorFuture::new(
+            self.inner().clone(),
+            path,
+            (OpWrite::default(), expire),
+            |inner, path, (args, dur)| {
+                let fut = async move {
+                    let op = OpPresign::new(args, dur);
+                    let rp = inner.presign(&path, op).await?;
+                    Ok(rp.into_presigned_request())
+                };
+                Box::pin(fut)
+            },
+        ));
+        fut
     }
 }
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/ops.rs` & `opendal-0.36.1/local_dependencies/opendal/src/raw/ops.rs`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
     }
 
     /// Get the cache control from option
     pub fn cache_control(&self) -> Option<&str> {
         self.cache_control.as_deref()
     }
 
-    /// Set the content type of option
+    /// Set the cache control of option
     pub fn with_cache_control(mut self, cache_control: &str) -> Self {
         self.cache_control = Some(cache_control.to_string());
         self
     }
 }
 
 /// Args for `copy` operation.
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/reader.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/reader.rs`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 use std::task::Poll;
 
 use bytes::Bytes;
 use futures::AsyncRead;
 use futures::AsyncSeek;
 use futures::Stream;
 
-use crate::ops::OpRead;
 use crate::raw::*;
 use crate::*;
 
 /// Reader is designed to read data from given path in an asynchronous
 /// manner.
 ///
 /// # Usage
```

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/scheme.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/scheme.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/local_dependencies/opendal/src/types/writer.rs` & `opendal-0.36.1/local_dependencies/opendal/src/types/writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 use std::task::Poll;
 
 use bytes::Bytes;
 use futures::future::BoxFuture;
 use futures::AsyncWrite;
 use futures::FutureExt;
 
-use crate::ops::OpWrite;
 use crate::raw::oio::Write;
 use crate::raw::*;
 use crate::*;
 
 /// Writer is designed to write data into given path in an asynchronous
 /// manner.
 ///
```

### Comparing `opendal-0.35.0/Cargo.toml` & `opendal-0.36.1/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.65"
-version= "0.35.0"
+version= "0.36.1"
 
 [lib]
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 futures = "0.3.28"
```

### Comparing `opendal-0.35.0/.gitignore` & `opendal-0.36.1/.gitignore`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/CONTRIBUTING.md` & `opendal-0.36.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/README.md` & `opendal-0.36.1/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/benchmark/README.md` & `opendal-0.36.1/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/benchmark/async_opendal_benchmark.py` & `opendal-0.36.1/benchmark/async_opendal_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/benchmark/async_origin_s3_benchmark_with_gevent.py` & `opendal-0.36.1/benchmark/async_origin_s3_benchmark_with_gevent.py`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/examples/object.ipynb` & `opendal-0.36.1/examples/object.ipynb`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/pyproject.toml` & `opendal-0.36.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [build-system]
 build-backend = "maturin"
-requires = ["maturin>=0.14.16,<0.15"]
+requires = ["maturin>=1.0,<2.0"]
 
 [project]
 classifiers = [
   "Programming Language :: Rust",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
```

### Comparing `opendal-0.35.0/python/opendal/__init__.py` & `opendal-0.36.1/python/opendal/__init__.py`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/python/opendal/__init__.pyi` & `opendal-0.36.1/python/opendal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/src/asyncio.rs` & `opendal-0.36.1/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/src/layers.rs` & `opendal-0.36.1/src/layers.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/src/lib.rs` & `opendal-0.36.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/tests/binding.feature` & `opendal-0.36.1/tests/binding.feature`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/tests/steps/binding.py` & `opendal-0.36.1/tests/steps/binding.py`

 * *Files identical despite different names*

### Comparing `opendal-0.35.0/Cargo.lock` & `opendal-0.36.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -276,15 +276,15 @@
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f23d769dbf1838d5df5156e7b1ad404f4c463d1ac2c6aeb6cd943630f8a8400"
 dependencies = [
  "futures-core",
  "futures-io",
  "rustls 0.19.1",
- "webpki 0.21.4",
+ "webpki",
  "webpki-roots",
 ]
 
 [[package]]
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -452,30 +452,31 @@
  "regex",
  "rustc-hash",
  "shlex",
 ]
 
 [[package]]
 name = "bindgen"
-version = "0.64.0"
+version = "0.65.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4243e6031260db77ede97ad86c27e501d646a27ab57b59a574f725d98ab1fb4"
+checksum = "cfdf7b466f9a4903edc73f95d6d2bcd5baf8ae620638762244d3f60143643cc5"
 dependencies = [
  "bitflags 1.3.2",
  "cexpr",
  "clang-sys",
  "lazy_static",
  "lazycell",
  "peeking_take_while",
+ "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 1.0.109",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
@@ -1739,21 +1740,21 @@
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
 name = "hyper-rustls"
-version = "0.23.2"
+version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1788965e61b367cd03a62950836d5cd41560c3577d90e40e0819373194d1661c"
+checksum = "0646026eb1b3eea4cd9ba47912ea5ce9cc07713d105b1a14698f4e6433d348b7"
 dependencies = [
  "http",
  "hyper",
- "rustls 0.20.8",
+ "rustls 0.21.1",
  "tokio",
  "tokio-rustls",
 ]
 
 [[package]]
 name = "hyper-tls"
 version = "0.5.0"
@@ -2032,19 +2033,19 @@
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
 [[package]]
 name = "librocksdb-sys"
-version = "0.10.0+7.9.2"
+version = "0.11.0+8.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fe4d5874f5ff2bc616e55e8c6086d478fcda13faf9495768a4aa1c22042d30b"
+checksum = "d3386f101bcb4bd252d8e9d2fb41ec3b0862a15a62b478c355b2982efa469e3e"
 dependencies = [
- "bindgen 0.64.0",
+ "bindgen 0.65.1",
  "bzip2-sys",
  "cc",
  "glob",
  "libc",
  "libz-sys",
 ]
 
@@ -2528,15 +2529,15 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "oay"
-version = "0.35.0"
+version = "0.36.1"
 dependencies = [
  "anyhow",
  "axum",
  "chrono",
  "clap 4.2.5",
  "dirs 5.0.1",
  "futures",
@@ -2571,27 +2572,27 @@
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "object_store_opendal"
-version = "0.35.0"
+version = "0.36.1"
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
-version = "0.35.0"
+version = "0.36.1"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "clap 4.2.5",
  "dirs 5.0.1",
  "env_logger",
  "futures",
@@ -2614,15 +2615,15 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opendal"
-version = "0.35.0"
+version = "0.36.1"
 dependencies = [
  "anyhow",
  "async-compat",
  "async-tls",
  "async-trait",
  "backon",
  "base64 0.21.0",
@@ -2675,47 +2676,47 @@
  "tracing-subscriber",
  "uuid",
  "wiremock",
 ]
 
 [[package]]
 name = "opendal-c"
-version = "0.1.0"
+version = "0.36.1"
 dependencies = [
  "bytes",
  "cbindgen",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-java"
-version = "0.1.0"
+version = "0.36.1"
 dependencies = [
  "anyhow",
  "jni",
  "num_cpus",
  "once_cell",
  "opendal",
  "tokio",
 ]
 
 [[package]]
 name = "opendal-nodejs"
-version = "0.35.0"
+version = "0.36.1"
 dependencies = [
  "futures",
  "napi",
  "napi-build",
  "napi-derive",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-python"
-version = "0.35.0"
+version = "0.36.1"
 dependencies = [
  "futures",
  "opendal",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
 ]
@@ -3268,14 +3269,24 @@
  "ctor",
  "diff",
  "output_vt100",
  "yansi",
 ]
 
 [[package]]
+name = "prettyplease"
+version = "0.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b69d39aab54d069e7f2fe8cb970493e7834601ca2d8c65fd7bbd183578080d1"
+dependencies = [
+ "proc-macro2",
+ "syn 2.0.16",
+]
+
+[[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
@@ -3378,17 +3389,17 @@
  "bitflags 1.3.2",
  "memchr",
  "unicase",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot 0.12.1",
  "pyo3-build-config",
@@ -3408,49 +3419,49 @@
  "pin-project-lite",
  "pyo3",
  "tokio",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -3711,17 +3722,17 @@
 name = "regex-syntax"
 version = "0.6.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
 
 [[package]]
 name = "reqsign"
-version = "0.12.0"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b04f5fccb94d61c154f0d8520ec42e79afdc145f4b1a392faa269874995fda66"
+checksum = "b6cb65eb3405f9c2de5c18bfc37338d6bbdb2c35eb8eb0e946208cbb564e4833"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.0",
  "chrono",
  "form_urlencoded",
  "hex",
@@ -3742,17 +3753,17 @@
  "sha1",
  "sha2",
  "tokio",
 ]
 
 [[package]]
 name = "reqwest"
-version = "0.11.15"
+version = "0.11.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ba30cc2c0cd02af1222ed216ba659cdb2f879dfe3181852fe7c50b1d0005949"
+checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
 dependencies = [
  "base64 0.21.0",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
@@ -3765,15 +3776,15 @@
  "js-sys",
  "log",
  "mime",
  "native-tls",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls 0.20.8",
+ "rustls 0.21.1",
  "rustls-native-certs",
  "rustls-pemfile",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "tokio",
  "tokio-native-tls",
@@ -3818,17 +3829,17 @@
  "untrusted",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "rocksdb"
-version = "0.20.1"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "015439787fce1e75d55f279078d33ff14b4af5d93d995e8838ee4631301c8a99"
+checksum = "bb6f170a4041d50a0ce04b0d2e14916d6ca863ea2e422689a5b694395d299ffe"
 dependencies = [
  "libc",
  "librocksdb-sys",
 ]
 
 [[package]]
 name = "rsa"
@@ -3897,27 +3908,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35edb675feee39aec9c99fa5ff985081995a06d594114ae14cbe797ad7b7a6d7"
 dependencies = [
  "base64 0.13.1",
  "log",
  "ring",
  "sct 0.6.1",
- "webpki 0.21.4",
+ "webpki",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.20.8"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fff78fc74d175294f4e83b28343315ffcfb114b156f0185e9741cb5570f50e2f"
+checksum = "c911ba11bc8433e811ce56fde130ccf32f5127cab0e0194e9c68c5a5b671791e"
 dependencies = [
  "log",
  "ring",
+ "rustls-webpki",
  "sct 0.7.0",
- "webpki 0.22.0",
 ]
 
 [[package]]
 name = "rustls-native-certs"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0167bac7a9f490495f3c33013e7722b53cb087ecbe082fb0c6387c96f634ea50"
@@ -3934,14 +3945,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
 dependencies = [
  "base64 0.21.0",
 ]
 
 [[package]]
+name = "rustls-webpki"
+version = "0.100.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d6207cd5ed3d8dca7816f8f3725513a34609c0c765bf652b8c3cb4cfd87db46b"
+dependencies = [
+ "ring",
+ "untrusted",
+]
+
+[[package]]
 name = "rustversion"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
 
 [[package]]
 name = "ryu"
@@ -4622,21 +4643,20 @@
 dependencies = [
  "libc",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-rustls"
-version = "0.23.4"
+version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c43ee83903113e03984cb9e5cebe6c04a5116269e900e3ddba8f068a62adda59"
+checksum = "e0d409377ff5b1e3ca6437aa86c1eb7d40c134bfec254e44c830defa92669db5"
 dependencies = [
- "rustls 0.20.8",
+ "rustls 0.21.1",
  "tokio",
- "webpki 0.22.0",
 ]
 
 [[package]]
 name = "tokio-util"
 version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
@@ -5166,30 +5186,20 @@
 checksum = "b8e38c0608262c46d4a56202ebabdeb094cef7e560ca7a226c6bf055188aa4ea"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
-name = "webpki"
-version = "0.22.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f095d78192e208183081cc07bc5515ef55216397af48b873e5edcd72637fa1bd"
-dependencies = [
- "ring",
- "untrusted",
-]
-
-[[package]]
 name = "webpki-roots"
 version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aabe153544e473b775453675851ecc86863d2a81d786d741f6b76778f2a48940"
 dependencies = [
- "webpki 0.21.4",
+ "webpki",
 ]
 
 [[package]]
 name = "widestring"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17882f045410753661207383517a6f62ec3dbeb6a4ed2acce01f0728238d1983"
```

### Comparing `opendal-0.35.0/PKG-INFO` & `opendal-0.36.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendal
-Version: 0.35.0
+Version: 0.36.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: gevent ; extra == 'benchmark'
 Requires-Dist: greenify ; extra == 'benchmark'
 Requires-Dist: greenlet ; extra == 'benchmark'
 Requires-Dist: boto3 ; extra == 'benchmark'
```

