# Comparing `tmp/static-frame-1.4.4.tar.gz` & `tmp/static-frame-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-1.4.4.tar", last modified: Sun May 28 22:20:41 2023, max compression
+gzip compressed data, was "static-frame-1.4.5.tar", last modified: Fri Jun  2 14:29:23 2023, max compression
```

## Comparing `static-frame-1.4.4.tar` & `static-frame-1.4.5.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-28 22:20:41.709879 static-frame-1.4.4/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2022-09-18 23:42:20.000000 static-frame-1.4.4/LICENSE.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-08-07 22:56:47.000000 static-frame-1.4.4/MANIFEST.in
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23101 2023-05-28 22:20:41.713878 static-frame-1.4.4/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23810 2023-05-27 18:00:43.000000 static-frame-1.4.4/README.rst
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2022-09-18 23:42:20.000000 static-frame-1.4.4/requirements-extras.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      363 2023-05-27 18:00:43.000000 static-frame-1.4.4/requirements-test.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-05-27 18:00:43.000000 static-frame-1.4.4/requirements.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-05-28 22:20:41.713878 static-frame-1.4.4/setup.cfg
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-01-27 15:25:04.000000 static-frame-1.4.4/setup.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-28 22:20:41.645880 static-frame-1.4.4/static_frame/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7638 2023-05-28 21:56:36.000000 static-frame-1.4.4/static_frame/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/__main__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-28 22:20:41.681879 static-frame-1.4.4/static_frame/core/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.4/static_frame/core/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-01-27 15:25:04.000000 static-frame-1.4.4/static_frame/core/archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/assign.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5475 2023-05-16 21:05:11.000000 static-frame-1.4.4/static_frame/core/axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    58179 2023-02-23 20:10:49.000000 static-frame-1.4.4/static_frame/core/batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-01-27 15:25:04.000000 static-frame-1.4.4/static_frame/core/bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-02-27 23:01:10.000000 static-frame-1.4.4/static_frame/core/container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    70680 2023-05-27 18:00:43.000000 static-frame-1.4.4/static_frame/core/container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2022-10-01 15:52:09.000000 static-frame-1.4.4/static_frame/core/display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-08-07 22:56:47.000000 static-frame-1.4.4/static_frame/core/display_html_datatables.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/display_visidata.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-03-28 21:18:03.000000 static-frame-1.4.4/static_frame/core/doc_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3447 2023-05-27 18:00:43.000000 static-frame-1.4.4/static_frame/core/exception.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2022-08-07 22:56:47.000000 static-frame-1.4.4/static_frame/core/fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   378509 2023-05-27 18:00:43.000000 static-frame-1.4.4/static_frame/core/frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-01-27 15:25:04.000000 static-frame-1.4.4/static_frame/core/hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    56897 2023-05-27 18:00:43.000000 static-frame-1.4.4/static_frame/core/index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-01-27 15:25:04.000000 static-frame-1.4.4/static_frame/core/index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-01-27 15:25:04.000000 static-frame-1.4.4/static_frame/core/index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21196 2023-05-04 22:17:10.000000 static-frame-1.4.4/static_frame/core/index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   107732 2023-05-27 18:00:43.000000 static-frame-1.4.4/static_frame/core/index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-02-01 00:09:42.000000 static-frame-1.4.4/static_frame/core/index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-01-28 23:33:40.000000 static-frame-1.4.4/static_frame/core/interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/interface_meta.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-01-27 15:25:04.000000 static-frame-1.4.4/static_frame/core/join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23859 2023-05-04 22:17:10.000000 static-frame-1.4.4/static_frame/core/loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-01-28 23:33:40.000000 static-frame-1.4.4/static_frame/core/memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35827 2023-05-17 22:07:47.000000 static-frame-1.4.4/static_frame/core/node_dt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24236 2023-05-17 22:07:47.000000 static-frame-1.4.4/static_frame/core/node_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-01-27 15:25:04.000000 static-frame-1.4.4/static_frame/core/node_hashlib.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31896 2023-05-02 20:46:35.000000 static-frame-1.4.4/static_frame/core/node_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-03-28 21:18:03.000000 static-frame-1.4.4/static_frame/core/node_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-02-28 22:54:13.000000 static-frame-1.4.4/static_frame/core/node_selector.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2022-11-10 00:09:54.000000 static-frame-1.4.4/static_frame/core/node_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/node_transpose.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10018 2023-05-27 18:00:43.000000 static-frame-1.4.4/static_frame/core/node_values.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2022-10-13 03:47:27.000000 static-frame-1.4.4/static_frame/core/pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2022-09-29 04:16:16.000000 static-frame-1.4.4/static_frame/core/protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2022-09-29 04:16:16.000000 static-frame-1.4.4/static_frame/core/protocol_dfi_abc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-03-31 18:53:08.000000 static-frame-1.4.4/static_frame/core/quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   127343 2023-05-17 22:07:47.000000 static-frame-1.4.4/static_frame/core/series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-02-21 22:37:54.000000 static-frame-1.4.4/static_frame/core/store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/store_client_mixin.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14881 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/store_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14880 2023-05-08 23:21:40.000000 static-frame-1.4.4/static_frame/core/store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-02-03 19:24:20.000000 static-frame-1.4.4/static_frame/core/store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21183 2023-02-23 22:39:48.000000 static-frame-1.4.4/static_frame/core/store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/core/style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   177922 2023-05-28 21:54:57.000000 static-frame-1.4.4/static_frame/core/type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   129082 2023-05-27 18:00:43.000000 static-frame-1.4.4/static_frame/core/util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2022-12-20 03:10:29.000000 static-frame-1.4.4/static_frame/core/www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-02-28 22:54:13.000000 static-frame-1.4.4/static_frame/core/yarn.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.4/static_frame/py.typed
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-28 22:20:41.681879 static-frame-1.4.4/static_frame/test/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.4/static_frame/test/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-01-30 03:11:00.000000 static-frame-1.4.4/static_frame/test/test_case.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-28 22:20:41.709879 static-frame-1.4.4/static_frame/test/unit/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.4/static_frame/test/unit/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-02-23 22:39:48.000000 static-frame-1.4.4/static_frame/test/unit/test_batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-02-21 22:37:54.000000 static-frame-1.4.4/static_frame/test/unit/test_bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35989 2023-05-27 18:00:43.000000 static-frame-1.4.4/static_frame/test/unit/test_container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-01-27 15:25:04.000000 static-frame-1.4.4/static_frame/test/unit/test_doc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   642225 2023-05-27 18:00:43.000000 static-frame-1.4.4/static_frame/test/unit/test_frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-08-07 22:56:47.000000 static-frame-1.4.4/static_frame/test/unit/test_frame_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-05-02 20:46:35.000000 static-frame-1.4.4/static_frame/test/unit/test_frame_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-01-27 15:25:04.000000 static-frame-1.4.4/static_frame/test/unit/test_frame_join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2022-08-07 22:56:47.000000 static-frame-1.4.4/static_frame/test/unit/test_frame_via_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-08-07 22:56:47.000000 static-frame-1.4.4/static_frame/test/unit/test_frame_via_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    64304 2023-05-04 22:17:10.000000 static-frame-1.4.4/static_frame/test/unit/test_index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-01-27 15:25:04.000000 static-frame-1.4.4/static_frame/test/unit/test_index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-05-04 22:17:10.000000 static-frame-1.4.4/static_frame/test/unit/test_index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    41844 2023-05-04 22:17:10.000000 static-frame-1.4.4/static_frame/test/unit/test_index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   164692 2023-05-16 21:05:11.000000 static-frame-1.4.4/static_frame/test/unit/test_index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-01-27 15:25:04.000000 static-frame-1.4.4/static_frame/test/unit/test_index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-05-09 00:42:47.000000 static-frame-1.4.4/static_frame/test/unit/test_interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    19608 2023-05-04 22:17:10.000000 static-frame-1.4.4/static_frame/test/unit/test_loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16279 2023-05-04 22:17:10.000000 static-frame-1.4.4/static_frame/test/unit/test_memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22632 2023-05-27 18:00:43.000000 static-frame-1.4.4/static_frame/test/unit/test_memory_measure_getsizeof.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-08-07 22:56:47.000000 static-frame-1.4.4/static_frame/test/unit/test_platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2022-09-29 04:16:16.000000 static-frame-1.4.4/static_frame/test/unit/test_protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    74931 2023-05-16 21:05:11.000000 static-frame-1.4.4/static_frame/test/unit/test_quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   244185 2023-05-17 22:07:47.000000 static-frame-1.4.4/static_frame/test/unit/test_series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_series_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-02-21 22:37:54.000000 static-frame-1.4.4/static_frame/test/unit/test_store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14506 2023-05-08 23:21:40.000000 static-frame-1.4.4/static_frame/test/unit/test_store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2022-09-18 23:42:20.000000 static-frame-1.4.4/static_frame/test/unit/test_style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   161330 2023-05-27 18:00:43.000000 static-frame-1.4.4/static_frame/test/unit/test_type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   114907 2023-05-27 18:00:43.000000 static-frame-1.4.4/static_frame/test/unit/test_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10401 2023-05-09 00:42:47.000000 static-frame-1.4.4/static_frame/test/unit/test_www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47732 2023-05-04 22:17:10.000000 static-frame-1.4.4/static_frame/test/unit/test_yarn.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-28 22:20:41.649880 static-frame-1.4.4/static_frame.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23101 2023-05-28 22:20:41.000000 static-frame-1.4.4/static_frame.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-05-28 22:20:41.000000 static-frame-1.4.4/static_frame.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-05-28 22:20:41.000000 static-frame-1.4.4/static_frame.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-05-28 22:20:41.000000 static-frame-1.4.4/static_frame.egg-info/requires.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-05-28 22:20:41.000000 static-frame-1.4.4/static_frame.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 14:29:23.803140 static-frame-1.4.5/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2022-09-18 23:42:20.000000 static-frame-1.4.5/LICENSE.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-08-07 22:56:47.000000 static-frame-1.4.5/MANIFEST.in
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23224 2023-06-02 14:29:23.803140 static-frame-1.4.5/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23901 2023-05-28 22:47:27.000000 static-frame-1.4.5/README.rst
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2022-09-18 23:42:20.000000 static-frame-1.4.5/requirements-extras.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      363 2023-05-27 18:00:43.000000 static-frame-1.4.5/requirements-test.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-05-27 18:00:43.000000 static-frame-1.4.5/requirements.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-06-02 14:29:23.807140 static-frame-1.4.5/setup.cfg
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-01-27 15:25:04.000000 static-frame-1.4.5/setup.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 14:29:23.755144 static-frame-1.4.5/static_frame/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7638 2023-06-02 13:56:30.000000 static-frame-1.4.5/static_frame/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/__main__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 14:29:23.779142 static-frame-1.4.5/static_frame/core/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/core/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/assign.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5475 2023-05-16 21:05:11.000000 static-frame-1.4.5/static_frame/core/axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    59324 2023-06-02 13:49:52.000000 static-frame-1.4.5/static_frame/core/batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-02-27 23:01:10.000000 static-frame-1.4.5/static_frame/core/container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    70680 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/core/container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2022-10-01 15:52:09.000000 static-frame-1.4.5/static_frame/core/display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/core/display_html_datatables.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/display_visidata.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-03-28 21:18:03.000000 static-frame-1.4.5/static_frame/core/doc_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3447 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/core/exception.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/core/fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   378509 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/core/frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    56897 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/core/index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21196 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/core/index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   107732 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/core/index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-02-01 00:09:42.000000 static-frame-1.4.5/static_frame/core/index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-01-28 23:33:40.000000 static-frame-1.4.5/static_frame/core/interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/interface_meta.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23859 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/core/loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-01-28 23:33:40.000000 static-frame-1.4.5/static_frame/core/memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35827 2023-05-17 22:07:47.000000 static-frame-1.4.5/static_frame/core/node_dt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24236 2023-05-17 22:07:47.000000 static-frame-1.4.5/static_frame/core/node_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/core/node_hashlib.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    32016 2023-06-02 13:49:52.000000 static-frame-1.4.5/static_frame/core/node_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-03-28 21:18:03.000000 static-frame-1.4.5/static_frame/core/node_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-02-28 22:54:13.000000 static-frame-1.4.5/static_frame/core/node_selector.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2022-11-10 00:09:54.000000 static-frame-1.4.5/static_frame/core/node_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/node_transpose.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10018 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/core/node_values.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2022-10-13 03:47:27.000000 static-frame-1.4.5/static_frame/core/pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2022-09-29 04:16:16.000000 static-frame-1.4.5/static_frame/core/protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2022-09-29 04:16:16.000000 static-frame-1.4.5/static_frame/core/protocol_dfi_abc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-03-31 18:53:08.000000 static-frame-1.4.5/static_frame/core/quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   127343 2023-05-17 22:07:47.000000 static-frame-1.4.5/static_frame/core/series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-02-21 22:37:54.000000 static-frame-1.4.5/static_frame/core/store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/store_client_mixin.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15150 2023-06-02 13:49:52.000000 static-frame-1.4.5/static_frame/core/store_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14880 2023-05-08 23:21:40.000000 static-frame-1.4.5/static_frame/core/store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-02-03 19:24:20.000000 static-frame-1.4.5/static_frame/core/store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21484 2023-06-02 13:49:52.000000 static-frame-1.4.5/static_frame/core/store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/core/style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   177922 2023-05-28 21:54:57.000000 static-frame-1.4.5/static_frame/core/type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   129931 2023-06-02 13:49:52.000000 static-frame-1.4.5/static_frame/core/util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2022-12-20 03:10:29.000000 static-frame-1.4.5/static_frame/core/www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-02-28 22:54:13.000000 static-frame-1.4.5/static_frame/core/yarn.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/py.typed
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 14:29:23.783142 static-frame-1.4.5/static_frame/test/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/test/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-01-30 03:11:00.000000 static-frame-1.4.5/static_frame/test/test_case.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 14:29:23.803140 static-frame-1.4.5/static_frame/test/unit/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/test/unit/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-02-23 22:39:48.000000 static-frame-1.4.5/static_frame/test/unit/test_batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-02-21 22:37:54.000000 static-frame-1.4.5/static_frame/test/unit/test_bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35989 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/test/unit/test_container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/test/unit/test_doc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   642225 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/test/unit/test_frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/test/unit/test_frame_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-05-02 20:46:35.000000 static-frame-1.4.5/static_frame/test/unit/test_frame_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/test/unit/test_frame_join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/test/unit/test_frame_via_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/test/unit/test_frame_via_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    64304 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/test/unit/test_index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/test/unit/test_index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/test/unit/test_index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    41844 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/test/unit/test_index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   164692 2023-05-16 21:05:11.000000 static-frame-1.4.5/static_frame/test/unit/test_index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-01-27 15:25:04.000000 static-frame-1.4.5/static_frame/test/unit/test_index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-05-09 00:42:47.000000 static-frame-1.4.5/static_frame/test/unit/test_interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    19608 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/test/unit/test_loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16279 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/test/unit/test_memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22632 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/test/unit/test_memory_measure_getsizeof.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-08-07 22:56:47.000000 static-frame-1.4.5/static_frame/test/unit/test_platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2022-09-29 04:16:16.000000 static-frame-1.4.5/static_frame/test/unit/test_protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    74931 2023-05-16 21:05:11.000000 static-frame-1.4.5/static_frame/test/unit/test_quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   244185 2023-05-17 22:07:47.000000 static-frame-1.4.5/static_frame/test/unit/test_series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_series_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-02-21 22:37:54.000000 static-frame-1.4.5/static_frame/test/unit/test_store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14506 2023-05-08 23:21:40.000000 static-frame-1.4.5/static_frame/test/unit/test_store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2022-09-18 23:42:20.000000 static-frame-1.4.5/static_frame/test/unit/test_style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   161330 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/test/unit/test_type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   114907 2023-05-27 18:00:43.000000 static-frame-1.4.5/static_frame/test/unit/test_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10401 2023-05-09 00:42:47.000000 static-frame-1.4.5/static_frame/test/unit/test_www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47732 2023-05-04 22:17:10.000000 static-frame-1.4.5/static_frame/test/unit/test_yarn.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 14:29:23.759143 static-frame-1.4.5/static_frame.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23224 2023-06-02 14:29:23.000000 static-frame-1.4.5/static_frame.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-06-02 14:29:23.000000 static-frame-1.4.5/static_frame.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-02 14:29:23.000000 static-frame-1.4.5/static_frame.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-06-02 14:29:23.000000 static-frame-1.4.5/static_frame.egg-info/requires.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-06-02 14:29:23.000000 static-frame-1.4.5/static_frame.egg-info/top_level.txt
```

### Comparing `static-frame-1.4.4/LICENSE.txt` & `static-frame-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/PKG-INFO` & `static-frame-1.4.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.4.4
+Version: 1.4.5
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -22,27 +22,31 @@
         
         API Search: https://staticframe.dev
         
         Jupyter Notebook Tutorial: `Launch Binder <https://mybinder.org/v2/gh/static-frame/static-frame-ftgu/default?urlpath=tree/index.ipynb>`_
         
         
         
-        Installation
+        Installation via ``pip``
         -------------------------------
         
-        Install StaticFrame via PIP::
+        Install StaticFrame with ``pip``::
         
             pip install static-frame
         
-        To install full support of input and output routines via PIP::
+        To install optional dependencies for full support of input and output formats (such as XLSX and HDF5) via ``pip``::
         
             pip install static-frame [extras]
         
         
-        Older StaticFrame is available via ``conda-forge``; note, however, that most-recent versions are not available due to ``conda-forge`` slow adoption of new StaticFrame dependencies (``arraymap``). Using ``pip`` with the available pre-built wheels is a better alternative for all platforms ::
+        
+        Installation via ``conda``
+        -------------------------------
+        
+        StaticFrame can be installed via ``conda`` with the ``conda-forge`` channel. Note that pre-built wheels of StaticFrame and all compiled dependencies are available through ``pip`` and may offer more compatibility than a ``conda``-based installation ::
         
             conda install -c conda-forge static-frame
         
         
         
         Dependencies
         --------------
```

### Comparing `static-frame-1.4.4/README.rst` & `static-frame-1.4.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -64,27 +64,31 @@
 
 API Search: https://staticframe.dev
 
 Jupyter Notebook Tutorial: `Launch Binder <https://mybinder.org/v2/gh/static-frame/static-frame-ftgu/default?urlpath=tree/index.ipynb>`_
 
 
 
-Installation
+Installation via ``pip``
 -------------------------------
 
-Install StaticFrame via PIP::
+Install StaticFrame with ``pip``::
 
     pip install static-frame
 
-To install full support of input and output routines via PIP::
+To install optional dependencies for full support of input and output formats (such as XLSX and HDF5) via ``pip``::
 
     pip install static-frame [extras]
 
 
-Older StaticFrame is available via ``conda-forge``; note, however, that most-recent versions are not available due to ``conda-forge`` slow adoption of new StaticFrame dependencies (``arraymap``). Using ``pip`` with the available pre-built wheels is a better alternative for all platforms ::
+
+Installation via ``conda``
+-------------------------------
+
+StaticFrame can be installed via ``conda`` with the ``conda-forge`` channel. Note that pre-built wheels of StaticFrame and all compiled dependencies are available through ``pip`` and may offer more compatibility than a ``conda``-based installation ::
 
     conda install -c conda-forge static-frame
 
 
 
 Dependencies
 --------------
```

### Comparing `static-frame-1.4.4/setup.py` & `static-frame-1.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/__init__.py` & `static-frame-1.4.5/static_frame/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,8 +115,8 @@
 from static_frame.core.util import IndexSpecifier as IndexSpecifier
 from static_frame.core.util import KeyOrKeys as KeyOrKeys
 from static_frame.core.util import PathSpecifierOrFileLike as PathSpecifierOrFileLike
 from static_frame.core.util import SeriesInitializer as SeriesInitializer
 from static_frame.core.www import WWW
 from static_frame.core.yarn import Yarn as Yarn
 
-__version__ = '1.4.4'
+__version__ = '1.4.5'
```

### Comparing `static-frame-1.4.4/static_frame/__main__.py` & `static-frame-1.4.5/static_frame/__main__.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/archive_npy.py` & `static-frame-1.4.5/static_frame/core/archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/axis_map.py` & `static-frame-1.4.5/static_frame/core/axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/batch.py` & `static-frame-1.4.5/static_frame/core/batch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import typing as tp
-from concurrent.futures import ProcessPoolExecutor
-from concurrent.futures import ThreadPoolExecutor
 
 import numpy as np
 
 from static_frame.core.bus import Bus
 from static_frame.core.container import ContainerOperand
 from static_frame.core.display import Display
 from static_frame.core.display import DisplayActive
@@ -52,17 +50,15 @@
 from static_frame.core.util import IndexConstructor
 from static_frame.core.util import IndexConstructors
 from static_frame.core.util import IndexInitializer
 from static_frame.core.util import KeyOrKeys
 from static_frame.core.util import NameType
 from static_frame.core.util import PathSpecifier
 from static_frame.core.util import UFunc
-
-# import multiprocessing as mp
-# mp_context = mp.get_context('spawn')
+from static_frame.core.util import get_concurrent_executor
 
 FrameOrSeries = tp.Union[Frame, Series]
 IteratorFrameItems = tp.Iterator[tp.Tuple[tp.Hashable, FrameOrSeries]]
 GeneratorFrameItems = tp.Callable[..., IteratorFrameItems]
 
 
 #-------------------------------------------------------------------------------
@@ -107,297 +103,322 @@
     __slots__ = (
             '_items',
             '_name',
             '_config',
             '_max_workers',
             '_chunksize',
             '_use_threads',
+            '_mp_context',
             )
 
     _config: StoreConfigMap
 
     @classmethod
     def from_frames(cls,
             frames: tp.Iterable[Frame],
             *,
             name: NameType = None,
             config: StoreConfigMapInitializer = None,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> 'Batch':
         '''Return a :obj:`Batch` from an iterable of :obj:`Frame`; labels will be drawn from :obj:`Frame.name`.
         '''
         return cls(((f.name, f) for f in frames),
                 name=name,
                 config=config,
                 max_workers=max_workers,
                 chunksize=chunksize,
                 use_threads=use_threads,
+                mp_context=mp_context,
                 )
 
     #---------------------------------------------------------------------------
     # constructors by data format
 
     @classmethod
     def _from_store(cls,
             store: Store,
             *,
             config: StoreConfigMapInitializer = None,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> 'Batch':
         config_map = StoreConfigMap.from_initializer(config)
 
         items = ((label, store.read(label, config=config_map[label]))
                 for label in store.labels(config=config_map))
 
         return cls(items,
                 config=config,
                 max_workers=max_workers,
                 chunksize=chunksize,
                 use_threads=use_threads,
+                mp_context=mp_context,
                 )
 
     @classmethod
     @doc_inject(selector='batch_constructor')
     def from_zip_tsv(cls,
             fp: PathSpecifier,
             *,
             config: StoreConfigMapInitializer = None,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> 'Batch':
         '''
         Given a file path to zipped TSV :obj:`Batch` store, return a :obj:`Batch` instance.
 
         {args}
         '''
         store = StoreZipTSV(fp)
         return cls._from_store(store,
                 config=config,
                 max_workers=max_workers,
                 chunksize=chunksize,
                 use_threads=use_threads,
+                mp_context=mp_context,
                 )
 
     @classmethod
     @doc_inject(selector='batch_constructor')
     def from_zip_csv(cls,
             fp: PathSpecifier,
             *,
             config: StoreConfigMapInitializer = None,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> 'Batch':
         '''
         Given a file path to zipped CSV :obj:`Batch` store, return a :obj:`Batch` instance.
 
         {args}
         '''
         store = StoreZipCSV(fp)
         return cls._from_store(store,
                 config=config,
                 max_workers=max_workers,
                 chunksize=chunksize,
                 use_threads=use_threads,
+                mp_context=mp_context,
                 )
 
     @classmethod
     @doc_inject(selector='batch_constructor')
     def from_zip_pickle(cls,
             fp: PathSpecifier,
             *,
             config: StoreConfigMapInitializer = None,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> 'Batch':
         '''
         Given a file path to zipped pickle :obj:`Batch` store, return a :obj:`Batch` instance.
 
         {args}
         '''
         store = StoreZipPickle(fp)
         return cls._from_store(store,
                 config=config,
                 max_workers=max_workers,
                 chunksize=chunksize,
                 use_threads=use_threads,
+                mp_context=mp_context,
                 )
 
     @classmethod
     @doc_inject(selector='batch_constructor')
     def from_zip_npz(cls,
             fp: PathSpecifier,
             *,
             config: StoreConfigMapInitializer = None,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> 'Batch':
         '''
         Given a file path to zipped NPZ :obj:`Batch` store, return a :obj:`Batch` instance.
 
         {args}
         '''
         store = StoreZipNPZ(fp)
         return cls._from_store(store,
                 config=config,
                 max_workers=max_workers,
                 chunksize=chunksize,
                 use_threads=use_threads,
+                mp_context=mp_context,
                 )
 
     @classmethod
     @doc_inject(selector='batch_constructor')
     def from_zip_npy(cls,
             fp: PathSpecifier,
             *,
             config: StoreConfigMapInitializer = None,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> 'Batch':
         '''
         Given a file path to zipped NPY :obj:`Batch` store, return a :obj:`Batch` instance.
 
         {args}
         '''
         store = StoreZipNPY(fp)
         return cls._from_store(store,
                 config=config,
                 max_workers=max_workers,
                 chunksize=chunksize,
                 use_threads=use_threads,
+                mp_context=mp_context,
                 )
 
     @classmethod
     @doc_inject(selector='batch_constructor')
     def from_zip_parquet(cls,
             fp: PathSpecifier,
             *,
             config: StoreConfigMapInitializer = None,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> 'Batch':
         '''
         Given a file path to zipped parquet :obj:`Batch` store, return a :obj:`Batch` instance.
 
         {args}
         '''
         store = StoreZipParquet(fp)
         return cls._from_store(store,
                 config=config,
                 max_workers=max_workers,
                 chunksize=chunksize,
                 use_threads=use_threads,
+                mp_context=mp_context,
                 )
 
 
     @classmethod
     @doc_inject(selector='batch_constructor')
     def from_xlsx(cls,
             fp: PathSpecifier,
             *,
             config: StoreConfigMapInitializer = None,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> 'Batch':
         '''
         Given a file path to an XLSX :obj:`Batch` store, return a :obj:`Batch` instance.
 
         {args}
         '''
         # how to pass configuration for multiple sheets?
         store = StoreXLSX(fp)
         return cls._from_store(store,
                 config=config,
                 max_workers=max_workers,
                 chunksize=chunksize,
                 use_threads=use_threads,
+                mp_context=mp_context,
                 )
 
 
     @classmethod
     @doc_inject(selector='batch_constructor')
     def from_sqlite(cls,
             fp: PathSpecifier,
             *,
             config: StoreConfigMapInitializer = None,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> 'Batch':
         '''
         Given a file path to an SQLite :obj:`Batch` store, return a :obj:`Batch` instance.
 
         {args}
         '''
         store = StoreSQLite(fp)
         return cls._from_store(store,
                 config=config,
                 max_workers=max_workers,
                 chunksize=chunksize,
                 use_threads=use_threads,
+                mp_context=mp_context,
                 )
 
 
     @classmethod
     @doc_inject(selector='batch_constructor')
     def from_hdf5(cls,
             fp: PathSpecifier,
             *,
             config: StoreConfigMapInitializer = None,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> 'Batch':
         '''
         Given a file path to a HDF5 :obj:`Batch` store, return a :obj:`Batch` instance.
 
         {args}
         '''
         store = StoreHDF5(fp)
         return cls._from_store(store,
                 config=config,
                 max_workers=max_workers,
                 chunksize=chunksize,
                 use_threads=use_threads,
+                mp_context=mp_context,
                 )
 
     #---------------------------------------------------------------------------
     @doc_inject(selector='batch_init')
     def __init__(self,
             items: IteratorFrameItems,
             *,
             name: NameType = None,
             config: StoreConfigMapInitializer = None,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ):
         '''
         Default constructor of a :obj:`Batch`.
 
         {args}
         '''
         self._items = items # might be a generator!
         self._name = name
 
         self._config = StoreConfigMap.from_initializer(config)
 
         self._max_workers = max_workers
         self._chunksize = chunksize
         self._use_threads = use_threads
+        self._mp_context = mp_context
 
     #---------------------------------------------------------------------------
     def _derive(self,
             gen: GeneratorFrameItems,
             name: NameType = None,
             ) -> 'Batch':
         '''Utility for creating derived Batch
@@ -485,18 +506,22 @@
 
     def _apply_pool(self,
             labels: tp.List[tp.Hashable],
             arg_iter: tp.Iterator[tp.Tuple[tp.Any, ...]],
             caller: tp.Callable[..., FrameOrSeries],
             ) -> 'Batch':
 
-        pool_executor = ThreadPoolExecutor if self._use_threads else ProcessPoolExecutor
+        pool_executor = get_concurrent_executor(
+                use_threads=self._use_threads,
+                max_workers=self._max_workers,
+                mp_context=self._mp_context,
+                )
 
         def gen_pool() -> IteratorFrameItems:
-            with pool_executor(max_workers=self._max_workers) as executor:
+            with pool_executor() as executor:
                 yield from zip(labels,
                         executor.map(caller, arg_iter, chunksize=self._chunksize)
                         )
         return self._derive(gen_pool)
 
     def _apply_pool_except(self,
             labels: tp.List[tp.Hashable],
@@ -504,19 +529,23 @@
             caller: tp.Callable[..., FrameOrSeries],
             exception: tp.Type[Exception],
             ) -> 'Batch':
 
         if self._chunksize != 1:
             raise NotImplementedError('Cannot use apply_except idioms with chunksize other than 1')
 
-        pool_executor = ThreadPoolExecutor if self._use_threads else ProcessPoolExecutor
+        pool_executor = get_concurrent_executor(
+                use_threads=self._use_threads,
+                max_workers=self._max_workers,
+                mp_context=self._mp_context,
+                )
 
         def gen_pool() -> IteratorFrameItems:
             futures = []
-            with pool_executor(max_workers=self._max_workers) as executor:
+            with pool_executor() as executor:
                 for args in arg_iter:
                     futures.append(executor.submit(caller, args))
 
                 for label, future in zip(labels, futures):
                     try:
                         container = future.result()
                     except exception:
```

### Comparing `static-frame-1.4.4/static_frame/core/bus.py` & `static-frame-1.4.5/static_frame/core/bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/container.py` & `static-frame-1.4.5/static_frame/core/container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/container_util.py` & `static-frame-1.4.5/static_frame/core/container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/display.py` & `static-frame-1.4.5/static_frame/core/display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/display_color.py` & `static-frame-1.4.5/static_frame/core/display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/display_config.py` & `static-frame-1.4.5/static_frame/core/display_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/display_html_datatables.py` & `static-frame-1.4.5/static_frame/core/display_html_datatables.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/display_visidata.py` & `static-frame-1.4.5/static_frame/core/display_visidata.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/doc_str.py` & `static-frame-1.4.5/static_frame/core/doc_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/exception.py` & `static-frame-1.4.5/static_frame/core/exception.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/fill_value_auto.py` & `static-frame-1.4.5/static_frame/core/fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/frame.py` & `static-frame-1.4.5/static_frame/core/frame.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/hloc.py` & `static-frame-1.4.5/static_frame/core/hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/index.py` & `static-frame-1.4.5/static_frame/core/index.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/index_auto.py` & `static-frame-1.4.5/static_frame/core/index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/index_base.py` & `static-frame-1.4.5/static_frame/core/index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/index_correspondence.py` & `static-frame-1.4.5/static_frame/core/index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/index_datetime.py` & `static-frame-1.4.5/static_frame/core/index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/index_hierarchy.py` & `static-frame-1.4.5/static_frame/core/index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/index_hierarchy_set_utils.py` & `static-frame-1.4.5/static_frame/core/index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/interface.py` & `static-frame-1.4.5/static_frame/core/interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/interface_meta.py` & `static-frame-1.4.5/static_frame/core/interface_meta.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/join.py` & `static-frame-1.4.5/static_frame/core/join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/loc_map.py` & `static-frame-1.4.5/static_frame/core/loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/memory_measure.py` & `static-frame-1.4.5/static_frame/core/memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/node_dt.py` & `static-frame-1.4.5/static_frame/core/node_dt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/node_fill_value.py` & `static-frame-1.4.5/static_frame/core/node_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/node_hashlib.py` & `static-frame-1.4.5/static_frame/core/node_hashlib.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/node_iter.py` & `static-frame-1.4.5/static_frame/core/node_iter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 '''
 Tools for iterators in Series and Frame. These components are imported by both series.py and frame.py; these components also need to be able to return Series and Frame, and thus use deferred, function-based imports.
 '''
 
 import typing as tp
-from concurrent.futures import ProcessPoolExecutor
-from concurrent.futures import ThreadPoolExecutor
 from enum import Enum
 from functools import partial
 
 import numpy as np
 from arraykit import name_filter
 
 from static_frame.core.container_util import group_from_container
@@ -17,23 +15,17 @@
 from static_frame.core.util import AnyCallable
 from static_frame.core.util import DepthLevelSpecifier
 from static_frame.core.util import DtypeSpecifier
 from static_frame.core.util import IndexConstructor
 from static_frame.core.util import Mapping
 from static_frame.core.util import NameType
 from static_frame.core.util import TupleConstructorType
+from static_frame.core.util import get_concurrent_executor
 from static_frame.core.util import iterable_to_array_1d
 
-# import multiprocessing as mp
-# mp_context = mp.get_context('spawn')
-
-
-# from static_frame.core.util import array_from_iterator
-
-
 if tp.TYPE_CHECKING:
     from static_frame.core.bus import Bus  # pylint: disable=W0611 #pragma: no cover
     from static_frame.core.frame import Frame  # pylint: disable=W0611 #pragma: no cover
     from static_frame.core.index import Index  # pylint: disable=W0611 #pragma: no cover
     from static_frame.core.quilt import Quilt  # pylint: disable=W0611 #pragma: no cover
     from static_frame.core.series import Series  # pylint: disable=W0611 #pragma: no cover
     from static_frame.core.yarn import Yarn  # pylint: disable=W0611 #pragma: no cover
@@ -106,21 +98,21 @@
         self._apply_constructor: tp.Callable[..., FrameOrSeries] = apply_constructor
         self._apply_type = apply_type
 
     #---------------------------------------------------------------------------
 
     def _apply_iter_items_parallel(self,
             func: AnyCallable,
+            *,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> tp.Iterator[tp.Tuple[tp.Any, tp.Any]]:
 
-        pool_executor = ThreadPoolExecutor if use_threads else ProcessPoolExecutor
-
         if not callable(func): # support array, Series mapping
             func = getattr(func, '__getitem__')
 
         # use side effect list population to create keys when iterating over values
         func_keys = []
         arg_gen: PoolArgGen
 
@@ -131,35 +123,48 @@
                     yield v
         else:
             def arg_gen() -> tp.Iterator[tp.Tuple[tp.Any, tp.Any]]: #pylint: disable=E0102
                 for k, v in self._func_items():
                     func_keys.append(k)
                     yield k, v
 
-        with pool_executor(max_workers=max_workers) as executor:
+        pool_executor = get_concurrent_executor(
+                use_threads=use_threads,
+                max_workers=max_workers,
+                mp_context=mp_context,
+                )
+
+        with pool_executor() as executor:
             yield from zip(func_keys,
                     executor.map(func, arg_gen(), chunksize=chunksize)
                     )
 
     def _apply_iter_parallel(self,
             func: AnyCallable,
+            *,
             max_workers: tp.Optional[int] = None,
             chunksize: int = 1,
             use_threads: bool = False,
+            mp_context: tp.Optional[str] = None,
             ) -> tp.Iterator[tp.Any]:
 
-        pool_executor = ThreadPoolExecutor if use_threads else ProcessPoolExecutor
         if not callable(func): # support array, Series mapping
             func = getattr(func, '__getitem__')
 
         # use side effect list population to create keys when iterating over values
         arg_gen = (self._func_values if self._yield_type is IterNodeType.VALUES
                 else self._func_items)
 
-        with pool_executor(max_workers=max_workers) as executor:
+        pool_executor = get_concurrent_executor(
+                use_threads=use_threads,
+                max_workers=max_workers,
+                mp_context=mp_context,
+                )
+
+        with pool_executor() as executor:
             yield from executor.map(func, arg_gen(), chunksize=chunksize)
 
     #---------------------------------------------------------------------------
     @doc_inject(selector='apply')
     def apply_iter_items(self,
             func: AnyCallable,
             ) -> tp.Iterator[tp.Tuple[tp.Any, tp.Any]]:
```

### Comparing `static-frame-1.4.4/static_frame/core/node_re.py` & `static-frame-1.4.5/static_frame/core/node_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/node_selector.py` & `static-frame-1.4.5/static_frame/core/node_selector.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/node_str.py` & `static-frame-1.4.5/static_frame/core/node_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/node_transpose.py` & `static-frame-1.4.5/static_frame/core/node_transpose.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/node_values.py` & `static-frame-1.4.5/static_frame/core/node_values.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/pivot.py` & `static-frame-1.4.5/static_frame/core/pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/platform.py` & `static-frame-1.4.5/static_frame/core/platform.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/protocol_dfi.py` & `static-frame-1.4.5/static_frame/core/protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/protocol_dfi_abc.py` & `static-frame-1.4.5/static_frame/core/protocol_dfi_abc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/quilt.py` & `static-frame-1.4.5/static_frame/core/quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/rank.py` & `static-frame-1.4.5/static_frame/core/rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/series.py` & `static-frame-1.4.5/static_frame/core/series.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/store.py` & `static-frame-1.4.5/static_frame/core/store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/store_client_mixin.py` & `static-frame-1.4.5/static_frame/core/store_client_mixin.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/store_config.py` & `static-frame-1.4.5/static_frame/core/store_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     include_columns: bool
     include_columns_name: bool
     merge_hierarchical_labels: bool
     read_max_workers: tp.Optional[int]
     read_chunksize: int
     write_max_workers: tp.Optional[int]
     write_chunksize: int
+    mp_context: tp.Optional[str]
     _hash: tp.Optional[int]
 
     __slots__ = (
             'index_depth',
             'index_name_depth_level',
             'index_constructors',
             'columns_depth',
@@ -56,14 +57,15 @@
             'include_columns',
             'include_columns_name',
             'merge_hierarchical_labels',
             'read_max_workers',
             'read_chunksize',
             'write_max_workers',
             'write_chunksize',
+            'mp_context',
             '_hash'
             )
 
     def __init__(self, *,
             # constructors
             index_depth: int = 0, # this default does not permit round trip
             index_name_depth_level: tp.Optional[DepthLevelSpecifier] = None,
@@ -86,14 +88,15 @@
             # not used by all exporters
             merge_hierarchical_labels: bool = True,
             # multiprocessing configuration
             read_max_workers: tp.Optional[int] = None,
             read_chunksize: int = 1,
             write_max_workers: tp.Optional[int] = None,
             write_chunksize: int = 1,
+            mp_context: tp.Optional[str] = None,
             ):
         '''
         Args:
             include_index: Boolean to determine if the ``index`` is included in output.
             include_columns: Boolean to determine if the ``columns`` is included in output.
         '''
         # constructor
@@ -119,15 +122,15 @@
         # self.format_columns = format_columns
         self.merge_hierarchical_labels = merge_hierarchical_labels
 
         self.read_max_workers = read_max_workers
         self.read_chunksize = read_chunksize
         self.write_max_workers = write_max_workers
         self.write_chunksize = write_chunksize
-
+        self.mp_context = mp_context
         self._hash = None
 
     def __eq__(self, other: tp.Any) -> bool:
         if not isinstance(other, StoreConfigHE):
             return False
 
         for attr in self.__slots__:
@@ -177,14 +180,15 @@
                     self.include_columns, # bool
                     self.include_columns_name, # bool
                     self.merge_hierarchical_labels, # bool
                     self.read_max_workers, # Optional[int]
                     self.read_chunksize, # int
                     self.write_max_workers, # Optional[int]
                     self.write_chunksize, # int
+                    self.mp_context,
             ))
         return self._hash
 
 
 class StoreConfig(StoreConfigHE):
     '''
     A read-only container of parameters used by :obj:`Store` subclasses for reading from and writing to multi-table storage formats.
@@ -234,14 +238,15 @@
             merge_hierarchical_labels: bool = True,
             label_encoder: tp.Optional[tp.Callable[[tp.Hashable], str]] = None,
             label_decoder: tp.Optional[tp.Callable[[str], tp.Hashable]] = None,
             read_max_workers: tp.Optional[int] = None,
             read_chunksize: int = 1,
             write_max_workers: tp.Optional[int] = None,
             write_chunksize: int = 1,
+            mp_context: tp.Optional[str] = None,
             ):
         StoreConfigHE.__init__(self,
                 index_depth=index_depth,
                 index_name_depth_level=index_name_depth_level,
                 index_constructors=index_constructors,
                 columns_depth=columns_depth,
                 columns_name_depth_level=columns_name_depth_level,
@@ -257,14 +262,15 @@
                 include_columns=include_columns,
                 include_columns_name=include_columns_name,
                 merge_hierarchical_labels=merge_hierarchical_labels,
                 read_max_workers=read_max_workers,
                 read_chunksize=read_chunksize,
                 write_max_workers=write_max_workers,
                 write_chunksize=write_chunksize,
+                mp_context=mp_context,
         )
         self.label_encoder = label_encoder
         self.label_decoder = label_decoder
 
     def label_encode(self, label: tp.Hashable) -> str:
         if self.label_encoder:
             label = self.label_encoder(label)
```

### Comparing `static-frame-1.4.4/static_frame/core/store_filter.py` & `static-frame-1.4.5/static_frame/core/store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/store_hdf5.py` & `static-frame-1.4.5/static_frame/core/store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/store_sqlite.py` & `static-frame-1.4.5/static_frame/core/store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/store_xlsx.py` & `static-frame-1.4.5/static_frame/core/store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/store_zip.py` & `static-frame-1.4.5/static_frame/core/store_zip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import pickle
 import typing as tp
 import zipfile
-from concurrent.futures import ProcessPoolExecutor
 from io import BytesIO
 from io import StringIO
 
 from static_frame.core.archive_npy import ArchiveFrameConverter
 from static_frame.core.archive_npy import ArchiveZipWrapper
 from static_frame.core.container_util import container_to_exporter_attr
 from static_frame.core.exception import ErrorNPYEncode
@@ -17,17 +16,15 @@
 from static_frame.core.store import store_coherent_write
 from static_frame.core.store_config import StoreConfig
 from static_frame.core.store_config import StoreConfigHE
 from static_frame.core.store_config import StoreConfigMap
 from static_frame.core.store_config import StoreConfigMapInitializer
 from static_frame.core.util import NOT_IN_CACHE_SENTINEL
 from static_frame.core.util import AnyCallable
-
-# import multiprocessing as mp
-# mp_context = mp.get_context('spawn')
+from static_frame.core.util import get_concurrent_executor
 
 FrameExporter = AnyCallable # Protocol not supported yet...
 FrameConstructor = tp.Callable[[tp.Any], Frame]
 LabelAndBytes = tp.Tuple[tp.Hashable, tp.Union[str, bytes]]
 IteratorItemsLabelOptionalFrame = tp.Iterator[tp.Tuple[tp.Hashable, tp.Optional[Frame]]]
 
 class PayloadBytesToFrame(tp.NamedTuple):
@@ -209,16 +206,21 @@
                             src=src,
                             name=label,
                             config=c.to_store_config_he(),
                             constructor=constructor,
                             )
 
         chunksize = config_map.default.read_chunksize
+        pool_executor = get_concurrent_executor(
+                use_threads=False,
+                max_workers=config_map.default.read_max_workers,
+                mp_context=config_map.default.mp_context,
+                )
 
-        with ProcessPoolExecutor(max_workers=config_map.default.read_max_workers) as executor:
+        with pool_executor() as executor:
             frame_gen = executor.map(self._payload_to_frame, gen(), chunksize=chunksize)
 
             for label, cached_frame in results_items():
                 if cached_frame is not None:
                     yield cached_frame
                 else:
                     frame = next(frame_gen)
@@ -249,16 +251,21 @@
                         name=label,
                         config=config_map[label].to_store_config_he(),
                         frame=frame,
                         exporter=self.__class__._EXPORTER,
                         )
 
         if multiprocess:
+            pool_executor = get_concurrent_executor(
+                    use_threads=False,
+                    max_workers=config_map.default.write_max_workers,
+                    mp_context=config_map.default.mp_context,
+                    )
             def label_and_bytes() -> tp.Iterator[LabelAndBytes]:
-                with ProcessPoolExecutor(max_workers=config_map.default.write_max_workers) as executor:
+                with pool_executor() as executor:
                     yield from executor.map(self._payload_to_bytes,
                             gen(),
                             chunksize=config_map.default.write_chunksize)
         else:
             label_and_bytes = lambda: (self._payload_to_bytes(x) for x in gen())
 
         labels_encoded = set() # track uniqueness post encoding
```

### Comparing `static-frame-1.4.4/static_frame/core/style_config.py` & `static-frame-1.4.5/static_frame/core/style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/type_blocks.py` & `static-frame-1.4.5/static_frame/core/type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/util.py` & `static-frame-1.4.5/static_frame/core/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import ast
 import contextlib
 import datetime
 import math
 import operator
 import os
 import re
@@ -32,21 +34,24 @@
 
 from static_frame.core.exception import ErrorNotTruthy
 from static_frame.core.exception import InvalidDatetime64Comparison
 from static_frame.core.exception import InvalidDatetime64Initializer
 from static_frame.core.exception import LocInvalid
 
 if tp.TYPE_CHECKING:
+    from concurrent.futures import Executor  # pylint: disable=W0611 #pragma: no cover
+
     from static_frame.core.frame import Frame  # pylint: disable=W0611 #pragma: no cover
     from static_frame.core.frame import FrameAsType  # pylint: disable=W0611 #pragma: no cover
     from static_frame.core.index import Index  # pylint: disable=W0611 #pragma: no cover
     from static_frame.core.index_base import IndexBase  # pylint: disable=W0611 #pragma: no cover
     from static_frame.core.series import Series  # pylint: disable=W0611 #pragma: no cover
     from static_frame.core.type_blocks import TypeBlocks  # pylint: disable=W0611 #pragma: no cover
 
+
 # dtype.kind
 #     A character code (one of ‘biufcmMOSUV’) identifying the general kind of data.
 #     b 	boolean
 #     i 	signed integer
 #     u 	unsigned integer
 #     f 	floating-point
 #     c 	complex floating-point
@@ -466,25 +471,21 @@
     OPERATORS[rattr] = rfunc
 
 UFUNC_TO_REVERSE_OPERATOR: tp.Dict[UFunc, UFunc] = {
     # '__pos__': operator.__pos__,
     # '__neg__': operator.__neg__,
     # '__abs__': operator.__abs__,
     # '__invert__': operator.__invert__,
-
     np.add: OPERATORS['__radd__'],
     np.subtract: OPERATORS['__rsub__'],
     np.multiply: OPERATORS['__rmul__'],
     np.matmul: OPERATORS['__rmatmul__'],
     np.true_divide: OPERATORS['__rtruediv__'],
     np.floor_divide: OPERATORS['__rfloordiv__'],
-
-
     # '__mod__': operator.__mod__,
-
     # '__pow__': operator.__pow__,
     # '__lshift__': operator.__lshift__,
     # '__rshift__': operator.__rshift__,
     # '__and__': operator.__and__,
     # '__xor__': operator.__xor__,
     # '__or__': operator.__or__,
     np.less: OPERATORS['__gt__'],
@@ -647,14 +648,33 @@
                 try:
                     self._src.append(next(self._gen))
                 except StopIteration:
                     raise IndexError(k) from None
         return self._src[key]
 
 #-------------------------------------------------------------------------------
+def get_concurrent_executor(
+        *,
+        use_threads: bool,
+        max_workers: tp.Optional[int],
+        mp_context: tp.Optional[str],
+        ) -> tp.Type[Executor]:
+    # NOTE: these imports are conditional as these modules are not supported in pyodide
+    if use_threads:
+        from concurrent.futures import ThreadPoolExecutor
+        exe = partial(ThreadPoolExecutor,
+                max_workers=max_workers)
+    else:
+        from concurrent.futures import ProcessPoolExecutor
+        exe = partial(ProcessPoolExecutor,
+                max_workers=max_workers,
+                mp_context=mp_context)
+    return exe #type: ignore
+
+#-------------------------------------------------------------------------------
 # join utils
 
 class Join(Enum):
     INNER = 0
     LEFT = 1
     RIGHT = 2
     OUTER = 3
```

### Comparing `static-frame-1.4.4/static_frame/core/www.py` & `static-frame-1.4.5/static_frame/core/www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/core/yarn.py` & `static-frame-1.4.5/static_frame/core/yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/test_case.py` & `static-frame-1.4.5/static_frame/test/test_case.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_archive_npy.py` & `static-frame-1.4.5/static_frame/test/unit/test_archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_axis_map.py` & `static-frame-1.4.5/static_frame/test/unit/test_axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_batch.py` & `static-frame-1.4.5/static_frame/test/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_bus.py` & `static-frame-1.4.5/static_frame/test/unit/test_bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_container.py` & `static-frame-1.4.5/static_frame/test/unit/test_container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_container_util.py` & `static-frame-1.4.5/static_frame/test/unit/test_container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_display.py` & `static-frame-1.4.5/static_frame/test/unit/test_display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_display_color.py` & `static-frame-1.4.5/static_frame/test/unit/test_display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_doc.py` & `static-frame-1.4.5/static_frame/test/unit/test_doc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_fill_value_auto.py` & `static-frame-1.4.5/static_frame/test/unit/test_fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_frame.py` & `static-frame-1.4.5/static_frame/test/unit/test_frame.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_frame_he.py` & `static-frame-1.4.5/static_frame/test/unit/test_frame_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_frame_iter.py` & `static-frame-1.4.5/static_frame/test/unit/test_frame_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_frame_join.py` & `static-frame-1.4.5/static_frame/test/unit/test_frame_join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_frame_via_fill_value.py` & `static-frame-1.4.5/static_frame/test/unit/test_frame_via_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_frame_via_re.py` & `static-frame-1.4.5/static_frame/test/unit/test_frame_via_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_hloc.py` & `static-frame-1.4.5/static_frame/test/unit/test_hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_index.py` & `static-frame-1.4.5/static_frame/test/unit/test_index.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_index_auto.py` & `static-frame-1.4.5/static_frame/test/unit/test_index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_index_base.py` & `static-frame-1.4.5/static_frame/test/unit/test_index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_index_correspondence.py` & `static-frame-1.4.5/static_frame/test/unit/test_index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_index_datetime.py` & `static-frame-1.4.5/static_frame/test/unit/test_index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_index_hierarchy.py` & `static-frame-1.4.5/static_frame/test/unit/test_index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_index_hierarchy_set_utils.py` & `static-frame-1.4.5/static_frame/test/unit/test_index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_interface.py` & `static-frame-1.4.5/static_frame/test/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_loc_map.py` & `static-frame-1.4.5/static_frame/test/unit/test_loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_memory_measure.py` & `static-frame-1.4.5/static_frame/test/unit/test_memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_memory_measure_getsizeof.py` & `static-frame-1.4.5/static_frame/test/unit/test_memory_measure_getsizeof.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_pivot.py` & `static-frame-1.4.5/static_frame/test/unit/test_pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_protocol_dfi.py` & `static-frame-1.4.5/static_frame/test/unit/test_protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_quilt.py` & `static-frame-1.4.5/static_frame/test/unit/test_quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_rank.py` & `static-frame-1.4.5/static_frame/test/unit/test_rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_series.py` & `static-frame-1.4.5/static_frame/test/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_series_he.py` & `static-frame-1.4.5/static_frame/test/unit/test_series_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_store.py` & `static-frame-1.4.5/static_frame/test/unit/test_store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_store_filter.py` & `static-frame-1.4.5/static_frame/test/unit/test_store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_store_hdf5.py` & `static-frame-1.4.5/static_frame/test/unit/test_store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_store_sqlite.py` & `static-frame-1.4.5/static_frame/test/unit/test_store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_store_xlsx.py` & `static-frame-1.4.5/static_frame/test/unit/test_store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_store_zip.py` & `static-frame-1.4.5/static_frame/test/unit/test_store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_style_config.py` & `static-frame-1.4.5/static_frame/test/unit/test_style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_type_blocks.py` & `static-frame-1.4.5/static_frame/test/unit/test_type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_util.py` & `static-frame-1.4.5/static_frame/test/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_www.py` & `static-frame-1.4.5/static_frame/test/unit/test_www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame/test/unit/test_yarn.py` & `static-frame-1.4.5/static_frame/test/unit/test_yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.4/static_frame.egg-info/PKG-INFO` & `static-frame-1.4.5/static_frame.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.4.4
+Version: 1.4.5
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -22,27 +22,31 @@
         
         API Search: https://staticframe.dev
         
         Jupyter Notebook Tutorial: `Launch Binder <https://mybinder.org/v2/gh/static-frame/static-frame-ftgu/default?urlpath=tree/index.ipynb>`_
         
         
         
-        Installation
+        Installation via ``pip``
         -------------------------------
         
-        Install StaticFrame via PIP::
+        Install StaticFrame with ``pip``::
         
             pip install static-frame
         
-        To install full support of input and output routines via PIP::
+        To install optional dependencies for full support of input and output formats (such as XLSX and HDF5) via ``pip``::
         
             pip install static-frame [extras]
         
         
-        Older StaticFrame is available via ``conda-forge``; note, however, that most-recent versions are not available due to ``conda-forge`` slow adoption of new StaticFrame dependencies (``arraymap``). Using ``pip`` with the available pre-built wheels is a better alternative for all platforms ::
+        
+        Installation via ``conda``
+        -------------------------------
+        
+        StaticFrame can be installed via ``conda`` with the ``conda-forge`` channel. Note that pre-built wheels of StaticFrame and all compiled dependencies are available through ``pip`` and may offer more compatibility than a ``conda``-based installation ::
         
             conda install -c conda-forge static-frame
         
         
         
         Dependencies
         --------------
```

### Comparing `static-frame-1.4.4/static_frame.egg-info/SOURCES.txt` & `static-frame-1.4.5/static_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

