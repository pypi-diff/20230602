# Comparing `tmp/astrohack-0.1.4.tar.gz` & `tmp/astrohack-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.1.4.tar", last modified: Fri May 19 21:50:06 2023, max compression
+gzip compressed data, was "astrohack-0.1.5.tar", last modified: Fri Jun  2 16:07:46 2023, max compression
```

## Comparing `astrohack-0.1.4.tar` & `astrohack-0.1.5.tar`

### file list

```diff
@@ -1,102 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.439236 astrohack-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 21:49:49.000000 astrohack-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:49:49.000000 astrohack-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-19 21:50:06.435236 astrohack-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-19 21:49:49.000000 astrohack-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:49:49.000000 astrohack-0.1.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-19 21:49:49.000000 astrohack-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:50:06.439236 astrohack-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.427236 astrohack-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.427236 astrohack-0.1.4/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.431236 astrohack-0.1.4/src/astrohack/_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    32566 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20815 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.431236 astrohack-0.1.4/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_dask_graph_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.431236 astrohack-0.1.4/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    22921 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_extract_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.431236 astrohack-0.1.4/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    32810 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.431236 astrohack-0.1.4/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/_utils/_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/astrohack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.427236 astrohack-0.1.4/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.435236 astrohack-0.1.4/src/astrohack/data/.file_meta_data/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.435236 astrohack-0.1.4/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.435236 astrohack-0.1.4/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.435236 astrohack-0.1.4/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.435236 astrohack-0.1.4/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.435236 astrohack-0.1.4/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.435236 astrohack-0.1.4/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.435236 astrohack-0.1.4/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)    19985 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    21859 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.435236 astrohack-0.1.4/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-19 21:49:49.000000 astrohack-0.1.4/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.431236 astrohack-0.1.4/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-19 21:50:06.000000 astrohack-0.1.4/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-19 21:50:06.000000 astrohack-0.1.4/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:50:06.000000 astrohack-0.1.4/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-19 21:50:06.000000 astrohack-0.1.4/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 21:50:06.000000 astrohack-0.1.4/src/astrohack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:06.435236 astrohack-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-19 21:49:49.000000 astrohack-0.1.4/tests/test_class_antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-05-19 21:49:49.000000 astrohack-0.1.4/tests/test_class_base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-19 21:49:49.000000 astrohack-0.1.4/tests/test_class_ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-19 21:49:49.000000 astrohack-0.1.4/tests/test_class_telescope.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-05-19 21:49:49.000000 astrohack-0.1.4/tests/test_stakeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.963994 astrohack-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 16:07:27.000000 astrohack-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:07:27.000000 astrohack-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-02 16:07:46.963994 astrohack-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-02 16:07:27.000000 astrohack-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:27.000000 astrohack-0.1.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-02 16:07:27.000000 astrohack-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:07:46.963994 astrohack-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.951994 astrohack-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.951994 astrohack-0.1.5/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.955994 astrohack-0.1.5/src/astrohack/_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    36119 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.955994 astrohack-0.1.5/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_dask_graph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18308 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22923 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22919 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_imaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42581 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_mds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_phase_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/_utils/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/astrohack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.951994 astrohack-0.1.5/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/.file_meta_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.959994 astrohack-0.1.5/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22518 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.963994 astrohack-0.1.5/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-02 16:07:27.000000 astrohack-0.1.5/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.955994 astrohack-0.1.5/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-02 16:07:46.000000 astrohack-0.1.5/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-02 16:07:46.000000 astrohack-0.1.5/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:07:46.000000 astrohack-0.1.5/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-02 16:07:46.000000 astrohack-0.1.5/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 16:07:46.000000 astrohack-0.1.5/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:07:46.963994 astrohack-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-02 16:07:27.000000 astrohack-0.1.5/tests/test_class_antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-06-02 16:07:27.000000 astrohack-0.1.5/tests/test_class_base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-02 16:07:27.000000 astrohack-0.1.5/tests/test_class_ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-02 16:07:27.000000 astrohack-0.1.5/tests/test_class_telescope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-06-02 16:07:27.000000 astrohack-0.1.5/tests/test_stakeholder.py
```

### Comparing `astrohack-0.1.4/LICENSE` & `astrohack-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/PKG-INFO` & `astrohack-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.4
+Version: 0.1.5
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.1.4/README.md` & `astrohack-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/pyproject.toml` & `astrohack-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.1.4"
+version = "0.1.5"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
```

### Comparing `astrohack-0.1.4/src/astrohack/_classes/antenna_surface.py` & `astrohack-0.1.5/src/astrohack/_classes/antenna_surface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import xarray as xr
 from matplotlib import pyplot as plt
 from matplotlib import colormaps as cmaps
+from matplotlib import patches
 
 from astrohack._classes.base_panel import panel_models, irigid
 from astrohack._classes.ring_panel import RingPanel
 from astrohack._utils._constants import *
 from astrohack._utils._conversion import _convert_to_db
 from astrohack._utils._conversion import _convert_unit
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._tools import _add_prefix, _well_positioned_colorbar, _axis_to_fits_header
-from astrohack._utils._io import _write_fits
+from astrohack._utils._tools import _add_prefix, _well_positioned_colorbar, _axis_to_fits_header, _resolution_to_fits_header
+from astrohack._utils._dio import _write_fits
 
 lnbr = "\n"
-figsize = [5, 4]
 
 
 class AntennaSurface:
-    def __init__(self, inputxds, telescope, cutoff=None, pmodel=None, crop=False, panel_margins=None, reread=False):
+    def __init__(self, inputxds, telescope, cutoff=None, pmodel=None, crop=False, nan_out_of_bounds=True, panel_margins=None, reread=False):
         """
         Antenna Surface description capable of computing RMS, Gains, and fitting the surface to obtain screw adjustments
         Args:
             inputxds: Input xarray dataset
             telescope: Telescope object
             cutoff: fractional cutoff on the amplitude image to exclude regions with weak amplitude from the panel,
                     defaults to 20% if None
             pmodel: model of panel surface fitting, if is None defaults to telescope default
             crop: Crop apertures to slightly larger frames than the antenna diameter
+            nan_out_of_bounds: Should the region outside the dish be replaced with NaNs?
             panel_margins: Margin to be ignored at edges of panels when fitting, defaults to 20% if None
             reread: Read a previously processed holography
         """
         self.reread = reread
         self._nullify()
         self._read_xds(inputxds)
         self.telescope = telescope
@@ -55,28 +56,30 @@
             self._init_ringed()
         if not self.reread:
             if self.computephase:
                 self.phase = self._deviation_to_phase(self.deviation)
             else:
                 self.deviation = self._phase_to_deviation(self.phase)
 
-            self.phase = self._nan_out_of_bounds(self.phase)
-            self.amplitude = self._nan_out_of_bounds(self.amplitude)
-            self.deviation = self._nan_out_of_bounds(self.deviation)
+            if nan_out_of_bounds:
+                self.phase = self._nan_out_of_bounds(self.phase)
+                self.amplitude = self._nan_out_of_bounds(self.amplitude)
+                self.deviation = self._nan_out_of_bounds(self.deviation)
 
     def _read_aips_xds(self, inputxds):
         self.amplitude = np.flipud(inputxds["AMPLITUDE"].values)
         self.deviation = np.flipud(inputxds["DEVIATION"].values)
         self.npoint = inputxds.attrs['npoint']
         self.wavelength = inputxds.attrs['wavelength']
         self.amp_unit = inputxds.attrs['amp_unit']
         self.u_axis = inputxds.u.values
         self.v_axis = inputxds.v.values
         self.computephase = True
         self.processed = False
+        self.resolution = None
 
     def _read_holog_xds(self, inputxds):
         if 'chan' in inputxds.dims:
             if inputxds.dims['chan'] != 1:
                 raise Exception("Only single channel holographies supported")
             self.wavelength = clight / inputxds.chan.values[0]
         else:
@@ -87,14 +90,22 @@
 
         self.npoint = np.sqrt(inputxds.dims['l'] ** 2 + inputxds.dims['m'] ** 2)
         self.amp_unit = 'V'
         self.u_axis = inputxds.u_prime.values * self.wavelength
         self.v_axis = inputxds.v_prime.values * self.wavelength
         self.computephase = False
 
+        try:
+            self.resolution = inputxds.attrs['aperture_resolution']
+        except KeyError:
+            logger = _get_astrohack_logger()
+            logger.warning("[_read_holog_xds] holog image does not have resolution information")
+            logger.warning("[_read_holog_xds] Rerun holog with astrohack v>0.1.5 for aperture resolution information")
+            self.resolution = None
+
     def _read_panel_xds(self, inputxds):
         self.wavelength = inputxds.attrs['wavelength']
         self.amp_unit = inputxds.attrs['amp_unit']
         self.panelmodel = inputxds.attrs['panel_model']
         self.panel_margins = inputxds.attrs['panel_margin']
         self.cut = inputxds.attrs['cutoff']
         self.solved = inputxds.attrs['solved']
@@ -103,14 +114,21 @@
         self.amplitude = inputxds['AMPLITUDE'].values
         self.phase = inputxds['PHASE'].values
         self.deviation = inputxds['DEVIATION'].values
         self.mask = inputxds['MASK']
         self.u_axis = inputxds.u.values
         self.v_axis = inputxds.u.values
         self.panel_distribution = inputxds['PANEL_DISTRIBUTION'].values
+        try:
+            self.resolution = inputxds.attrs['aperture_resolution']
+        except KeyError:
+            logger = _get_astrohack_logger()
+            logger.warning("[_read_panel_xds] Input panel file does not have resolution information")
+            logger.warning("[_read_panel_xds] Rerun holog with astrohack v>0.1.5 for aperture resolution information")
+            self.resolution = None
 
         if self.solved:
             self.phase_residuals = inputxds['PHASE_RESIDUALS'].values
             self.residuals = inputxds['RESIDUALS'].values
             self.phase_corrections = inputxds['PHASE_CORRECTIONS'].values
             self.corrections = inputxds['CORRECTIONS'].values
             self.panel_pars = inputxds['PANEL_PARAMETERS'].values
@@ -441,185 +459,219 @@
     def print_misc(self):
         """
         Print miscelaneous information on the panels in the antenna surface
         """
         for panel in self.panels:
             panel.print_misc()
 
-    def plot_mask(self, basename, screws=False, colormap=None, figuresize=None, dpi=300):
+    def plot_mask(self, basename, screws=False, colormap=None, figuresize=None, dpi=300, caller='panel', display=True):
         """
         Plot mask used in the selection of points to be fitted
         Args:
             basename: basename for the plot, the prefix 'ancillary_mask' will be added to it
             screws: Are screw positions to be shown in plot?
             colormap: Colormap for amplitude plot
             figuresize: 2 element array with the image sizes in inches
             dpi: Plot resolution
+            caller: Which mds called this plotting function
+            display: display plot inline in notebook
         """
         plotmask = np.where(self.mask, 1, np.nan)
         plotname = _add_prefix(basename, 'mask')
         self._plot_map(plotname, plotmask, 'Mask', 0, 1, None, screws=screws, colormap=colormap, figuresize=figuresize,
-                       dpi=dpi, colorbar=False)
+                       dpi=dpi, colorbar=False, caller=caller, display=display)
 
-    def plot_amplitude(self, basename, screws=False, colormap=None, figuresize=None, dpi=300):
+    def plot_amplitude(self, basename, screws=False, colormap=None, figuresize=None, dpi=300, caller='panel',
+                       display=True):
         """
         Plot Amplitude map
         Args:
             basename: basename for the plot, the prefix 'ancillary_amplitude' will be added to it
             screws: Are screw positions to be shown in plot?
             colormap: Colormap for amplitude plot
             figuresize: 2 element array with the image sizes in inches
             dpi: Plot resolution
+            caller: Which mds called this plotting function
+            display: display plot inline in notebook
         """
         vmin, vmax = np.nanmin(self.amplitude), np.nanmax(self.amplitude)
-        title = "Amplitude min={0:.5f}, max ={1:.5f} V".format(vmin, vmax)
+        title = "Amplitude, min={0:.5f}, max ={1:.5f} V".format(vmin, vmax)
         plotname = _add_prefix(basename, 'amplitude')
         self._plot_map(plotname, self.amplitude, title, vmin, vmax, self.amp_unit, screws=screws, colormap=colormap,
-                       figuresize=figuresize, dpi=dpi)
+                       figuresize=figuresize, dpi=dpi, caller=caller, display=display)
 
-    def plot_phase(self, basename, screws=False, colormap=None, figuresize=None, dpi=300, unit=None):
+    def plot_phase(self, basename, screws=False, colormap=None, figuresize=None, dpi=300, unit=None, caller='panel',
+                   display=True):
         """
         Plot phase map(s)
         Args:
             basename: basename for the plot(s), the prefix 'phase_{original|corrections|residuals}' will be added to it/them
             screws: Are screw positions to be shown in plot(s)?
             colormap: Colormap for phase plots
             figuresize: 2 element array with the image sizes in inches
             dpi: Plot resolution
             unit: Angle unit for plot(s)
+            caller: Which mds called this plotting function
+            display: display plot inline in notebook
         """
         if unit is None:
             unit = 'deg'
         fac = _convert_unit('rad', unit, 'trigonometric')
         prefix = 'phase'
-        if self.residuals is None:
+        if caller == 'image':
+            prefix = 'corrected'
             maps = [self.phase]
-            labels = ['original']
+            labels = ['phase']
         else:
-            maps = [self.phase, self.phase_corrections, self.phase_residuals]
-            labels = ['original', 'corrections', 'residuals']
-        self._multi_plot(maps, labels, prefix, basename, unit, fac, screws, colormap, figuresize, dpi)
+            if self.residuals is None:
+                maps = [self.phase]
+                labels = ['original']
+            else:
+                maps = [self.phase, self.phase_corrections, self.phase_residuals]
+                labels = ['original', 'correction', 'residual']
+        self._multi_plot(maps, labels, prefix, basename, unit, fac, screws, colormap, figuresize, dpi, caller, display)
 
-    def plot_deviation(self, basename, screws=False, colormap=None, figuresize=None, dpi=300, unit=None):
+    def plot_deviation(self, basename, screws=False, colormap=None, figuresize=None, dpi=300, unit=None, caller='panel',
+                       display=True):
         """
         Plot deviation map(s)
         Args:
             basename: basename for the plot(s), the prefix 'deviation_{original|corrections|residuals}' will be added to it/them
             screws: Are screw positions to be shown in plot(s)?
             colormap: Colormap for deviation plots
             figuresize: 2 element array with the image sizes in inches
             dpi: Plot resolution
             unit: Length unit for plot(s)
+            caller: Which mds called this plotting function
+            display: display plot inline in notebook
         """
         if unit is None:
             unit = 'mm'
         fac = _convert_unit('m', unit, 'length')
         prefix = 'deviation'
+        rms = self.get_rms(unit=unit)
         if self.residuals is None:
             maps = [self.deviation]
-            labels = ['original']
+            labels = [f'original RMS={rms:.2f} {unit}']
         else:
             maps = [self.deviation, self.corrections, self.residuals]
-            labels = ['original', 'corrections', 'residuals']
-        self._multi_plot(maps, labels, prefix, basename, unit, fac, screws, colormap, figuresize, dpi)
+            labels = [f'original RMS={rms[0]:.2f} {unit}', 'correction', f'residual RMS={rms[1]:.2f} {unit}']
+        self._multi_plot(maps, labels, prefix, basename, unit, fac, screws, colormap, figuresize, dpi, caller, display)
 
     def _multi_plot(self, maps, labels, prefix, basename, unit, conversion, screws, colormap=None, figuresize=None,
-                    dpi=300):
+                    dpi=300, caller='panel', display=True):
         if len(maps) != len(labels):
             raise Exception('Map list and label list must be of the same size')
         nplots = len(maps)
         vmax = np.nanmax(np.abs(conversion*maps[0]))
         vmin = -vmax
         for iplot in range(nplots):
             title = f'{prefix.capitalize()} {labels[iplot]}'
-            plotname = _add_prefix(basename, labels[iplot])
+            plotname = _add_prefix(basename, labels[iplot].split()[0])
             plotname = _add_prefix(plotname, prefix)
             self._plot_map(plotname, conversion*maps[iplot], title, vmin, vmax, unit, screws=screws, dpi=dpi,
-                           colormap=colormap, figuresize=figuresize)
+                           colormap=colormap, figuresize=figuresize, caller=caller, display=display)
 
     def _plot_map(self, filename, data, title, vmin, vmax, unit, screws=False, colormap=None, figuresize=None, dpi=300,
-                  colorbar=True):
+                  colorbar=True, caller='panel', display=True):
         if colormap is None:
             colormap = 'viridis'
         if figuresize is None:
             figuresize = figsize
         if figuresize is None or figuresize == 'None':
             fig, ax = plt.subplots(1, 1, figsize=figsize)
         else:
             fig, ax = plt.subplots(1, 1, figsize=figuresize)
         ax.set_title(title)
         # set the limits of the plot to the limits of the data
-        xmin = np.min(self.u_axis)
-        xmax = np.max(self.u_axis)
-        ymin = np.min(self.v_axis)
-        ymax = np.max(self.v_axis)
-        im = ax.imshow(data, cmap=colormap, interpolation="nearest", extent=[xmin, xmax, ymin, ymax],
+        extent = [np.min(self.u_axis), np.max(self.u_axis), np.min(self.v_axis), np.max(self.v_axis)]
+        im = ax.imshow(data, cmap=colormap, interpolation="nearest", extent=extent,
                        vmin=vmin, vmax=vmax,)
+        self._add_resolution_to_plot(ax, extent)
         if colorbar:
             _well_positioned_colorbar(ax, fig, im, "Z Scale [" + unit + "]")
+        self._add_resolution_to_plot(ax, extent)
         ax.set_xlabel("X axis [m]")
         ax.set_ylabel("Y axis [m]")
         for panel in self.panels:
             panel.plot(ax, screws=screws)
+        fig.suptitle(f'Antenna: {self.antenna_name}, DDI: {self.ddi.split("_")[-1]}')
         fig.tight_layout()
-        plt.savefig(filename, dpi=dpi)
-        plt.close()
+        plt.savefig(_add_prefix(filename, caller), dpi=dpi)
+        if not display:
+            plt.close()
+
+    def _add_resolution_to_plot(self, ax, extent, xpos=0.9, ypos=0.1):
+        lw = 0.5
+        if self.resolution is None:
+            return
+        dx = extent[1]-extent[0]
+        dy = extent[3]-extent[2]
+        center = (extent[0]+xpos*dx, extent[2]+ypos*dy)
+        resolution = patches.Ellipse(center, self.resolution[0], self.resolution[1], angle=0.0, linewidth=lw,
+                                     color='black', zorder=2, fill=False)
+        ax.add_patch(resolution)
+        halfbeam = self.resolution/dy/2
+        ax.axvline(x=center[0], ymin=ypos - halfbeam[1], ymax=ypos + halfbeam[1], color='black', lw=lw / 2)
+        ax.axhline(y=center[1], xmin=xpos - halfbeam[0], xmax=xpos + halfbeam[0], color='black', lw=lw / 2)
 
-    def plot_screw_adjustments(self, filename, unit, threshold=None, colormap=None, figuresize=None, dpi=300):
+    def plot_screw_adjustments(self, filename, unit, threshold=None, colormap=None, figuresize=None, dpi=300,
+                               display=True):
         """
         Plot screw adjustments as circles over a blank canvas with the panel layout
         Args:
             filename: Name of the output filename for the plot
             unit: Unit to display the screw adjustments
             threshold: Threshold below which data is considered negligable, value is assumed to be in the same unit as the plot, if not given defaults to 10% of the maximal deviation
             colormap: Colormap to display the screw adjustments
             figuresize: 2 element array with the image sizes in inches
             dpi: Resolution in pixels per inch
+            display: display plot inline in notebook
         """
         if colormap is None:
             cmap = cmaps['RdBu_r']
         else:
             cmap = cmaps[colormap]
         if figuresize is None or figuresize == 'None':
             fig, ax = plt.subplots(1, 1, figsize=figsize)
         else:
             fig, ax = plt.subplots(1, 1, figsize=figuresize)
         fac = _convert_unit('m', unit, 'length')
         vmax = np.nanmax(np.abs(fac * self.screw_adjustments))
         vmin = -vmax
-        if threshold is None:
+        if threshold is None or threshold == 'None':
             threshold = 0.1*vmax
         else:
             threshold = np.abs(threshold)
 
         fig.suptitle('Screw corrections', y=0.92, fontsize='large')
         ax.set_title(f'\nThreshold = {threshold:.2f} {unit}', fontsize='small')
         # set the limits of the plot to the limits of the data
-        xmin = np.min(self.u_axis)
-        xmax = np.max(self.u_axis)
-        ymin = np.min(self.v_axis)
-        ymax = np.max(self.v_axis)
+        extent = [np.min(self.u_axis), np.max(self.u_axis), np.min(self.v_axis), np.max(self.v_axis)]
         im = ax.imshow(np.full_like(self.deviation, fill_value=np.nan), cmap=cmap, interpolation="nearest",
-                       extent=[xmin, xmax, ymin, ymax], vmin=vmin, vmax=vmax)
+                       extent=extent, vmin=vmin, vmax=vmax)
+        self._add_resolution_to_plot(ax, extent)
         colorbar = _well_positioned_colorbar(ax, fig, im, "Screw adjustments [" + unit + "]")
         if threshold > 0:
             line = threshold
             while line < vmax:
                 colorbar.ax.axhline(y=line, color='black', linestyle='-', lw=0.2)
                 colorbar.ax.axhline(y=-line, color='black', linestyle='-', lw=0.2)
                 line += threshold
         ax.set_xlabel("X axis [m]")
         ax.set_ylabel("Y axis [m]")
 
         for ipanel in range(len(self.panels)):
             self.panels[ipanel].plot(ax, screws=False)
             self.panels[ipanel].plot_corrections(ax, cmap, fac*self.screw_adjustments[ipanel], threshold, vmin, vmax)
+        fig.suptitle(f'Antenna: {self.antenna_name}, DDI: {self.ddi.split("_")[-1]}')
         fig.tight_layout()
         plt.savefig(filename, dpi=dpi)
-        plt.close()
+        if not display:
+            plt.close()
 
     def _build_panel_data_arrays(self):
         """
         Build arrays with data from the panels so that they can be stored on the XDS
         Returns:
             List with panel labels, panel fitting parameters, screw_adjustments
         """
@@ -679,14 +731,15 @@
         xds.attrs['wavelength'] = self.wavelength
         xds.attrs['amp_unit'] = self.amp_unit
         xds.attrs['panel_model'] = self.panelmodel
         xds.attrs['panel_margin'] = self.panel_margins
         xds.attrs['cutoff'] = self.cut
         xds.attrs['solved'] = self.solved
         xds.attrs['fitted'] = self.fitted
+        xds.attrs['aperture_resolution'] = self.resolution
         xds['AMPLITUDE'] = xr.DataArray(self.amplitude, dims=["u", "v"])
         xds['PHASE'] = xr.DataArray(self.phase, dims=["u", "v"])
         xds['DEVIATION'] = xr.DataArray(self.deviation, dims=["u", "v"])
         xds['MASK'] = xr.DataArray(self.mask, dims=["u", "v"])
         xds['PANEL_DISTRIBUTION'] = xr.DataArray(self.panel_distribution, dims=["u", "v"])
         if self.solved:
             xds['PHASE_RESIDUALS'] = xr.DataArray(self.phase_residuals, dims=["u", "v"])
@@ -721,26 +774,28 @@
         head = {
             'PMODEL'  : self.panelmodel,
             'PMARGIN' : self.panel_margins,
             'CUTOFF'  : self.cut,
             'TELESCOP': self.antenna_name,
             'INSTRUME': self.telescope.name,
             'WAVELENG': self.wavelength,
-            'FREQUENC': clight/self.wavelength
+            'FREQUENC': clight/self.wavelength,
         }
         head = _axis_to_fits_header(head, self.u_axis, 1, 'X', 'm')
         head = _axis_to_fits_header(head, self.v_axis, 2, 'Y', 'm')
+        head = _resolution_to_fits_header(head, self.resolution)
 
-        _write_fits(head, 'Amplitude', self.amplitude, basename + '_amplitude.fits', self.amp_unit, 'panel')
-        _write_fits(head, 'Mask', np.where(self.mask, 1.0, np.nan), basename + '_mask.fits', '', 'panel')
-        _write_fits(head, 'Original Phase', self.phase, basename + '_phase_original.fits', 'rad', 'panel')
-        _write_fits(head, 'Phase Corrections', self.phase_corrections, basename + '_phase_correction.fits', 'rad',
-                    'panel')
-        _write_fits(head, 'Phase residuals', self.phase_residuals, basename + '_phase_residual.fits', 'rad',
-                    'panel')
-        _write_fits(head, 'Original Deviation', self.deviation, basename + '_deviation_original.fits', 'm',
-                    'panel')
-        _write_fits(head, 'Deviation Corrections', self.corrections, basename + '_deviation_correction.fits', 'm',
-                    'panel')
-        _write_fits(head, 'Deviation residuals', self.residuals, basename + '_deviation_residual.fits', 'm',
+        _write_fits(head, 'Amplitude', self.amplitude, _add_prefix(basename, 'amplitude')+'.fits', self.amp_unit,
                     'panel')
+        _write_fits(head, 'Mask', np.where(self.mask, 1.0, np.nan), _add_prefix(basename, 'mask')+'.fits', '', 'panel')
+        _write_fits(head, 'Original Phase', self.phase, _add_prefix(basename, 'phase_original')+'.fits', 'rad', 'panel')
+        _write_fits(head, 'Phase Corrections', self.phase_corrections,
+                    _add_prefix(basename, 'phase_correction')+'.fits', 'rad', 'panel')
+        _write_fits(head, 'Phase residuals', self.phase_residuals, _add_prefix(basename, 'phase_residual')+'.fits',
+                    'rad', 'panel')
+        _write_fits(head, 'Original Deviation', self.deviation, _add_prefix(basename, 'deviation_original')+'.fits',
+                    'm', 'panel')
+        _write_fits(head, 'Deviation Corrections', self.corrections,
+                    _add_prefix(basename, 'deviation_correction')+'.fits', 'm', 'panel')
+        _write_fits(head, 'Deviation residuals', self.residuals, _add_prefix(basename, 'deviation_residual')+'.fits',
+                    'm', 'panel')
```

### Comparing `astrohack-0.1.4/src/astrohack/_classes/base_panel.py` & `astrohack-0.1.5/src/astrohack/_classes/base_panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,17 +31,15 @@
     global warned
     warned = value
 
 
 class BasePanel:
     markers = ['X', 'o', '*', 'P', 'D']
     colors = ['g', 'g', 'r', 'r', 'b']
-    fontsize = 4
     linewidth = 0.5
-    markersize = 2
     linecolor = 'black'
 
     def __init__(self, model, screws, plot_screw_pos, plot_screw_size, label, center=None, zeta=None):
         """
         Initializes the base panel with the appropriated fitting methods and providing basic functionality
         Fitting method models are:
         AIPS fitting models:
@@ -520,26 +518,26 @@
             ax: matplotlib axes instance
             rotate: Rotate label for better display
         """
         if rotate:
             angle = (-self.zeta % pi - pi/2)*_convert_unit('rad', 'deg', 'trigonometric')
         else:
             angle = 0
-        ax.text(self.center[1], self.center[0], self.label, fontsize=self.fontsize, ha='center', va='center',
+        ax.text(self.center[1], self.center[0], self.label, fontsize=fontsize, ha='center', va='center',
                 rotation=angle)
 
     def plot_screws(self, ax):
         """
         Plots panel screws to ax
         Args:
             ax: matplotlib axes instance
         """
         for iscrew in range(self.screws.shape[0]):
             screw = self.screws[iscrew, ]
-            ax.scatter(screw[1], screw[0], marker=self.markers[iscrew], lw=self.linewidth, s=self.markersize,
+            ax.scatter(screw[1], screw[0], marker=self.markers[iscrew], lw=self.linewidth, s=markersize,
                        color=self.colors[iscrew])
 
     def plot_corrections(self, ax, cmap, corrections, threshold, vmin, vmax):
         """
         Plot screw corrections onto an axis
         Args:
             ax: axis for plot
```

### Comparing `astrohack-0.1.4/src/astrohack/_classes/polygon_panel.py` & `astrohack-0.1.5/src/astrohack/_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/_classes/ring_panel.py` & `astrohack-0.1.5/src/astrohack/_classes/ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/_classes/telescope.py` & `astrohack-0.1.5/src/astrohack/_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_algorithms.py` & `astrohack-0.1.5/src/astrohack/_utils/_algorithms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_combine.py` & `astrohack-0.1.5/src/astrohack/_utils/_combine.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,48 @@
 import numpy as np
 import os
 import xarray as xr
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._io import _load_image_xds
+from astrohack._utils._dio import _load_image_xds
 from scipy.interpolate import griddata
 from astrohack._utils._constants import clight
+from astrohack._utils._tools import _parm_to_list
 
 
 def _combine_chunk(combine_chunk_params):
     """
     Process a combine chunk
     Args:
         combine_chunk_params: Param dictionary for combine chunk
     """
     logger = _get_astrohack_logger()
-
-    data_path = combine_chunk_params['image_file']+'/'+combine_chunk_params['antenna']
-    if combine_chunk_params['ddi_list'] == 'all':
-        ddi_list = os.listdir(data_path)
-    else:
-        ddi_list = combine_chunk_params['ddi_list']
+    antenna = combine_chunk_params['this_ant']
+    ddi_dict = combine_chunk_params['image_mds'][antenna]
+    fname = 'combine'
+    ddi_list = _parm_to_list(fname, combine_chunk_params['ddi'], ddi_dict, 'ddi')
+    print("DDI_LIST:", ddi_list)
 
     nddi = len(ddi_list)
-    out_xds_name = combine_chunk_params['combine_file'] + '/' + combine_chunk_params['antenna'] + '/' + ddi_list[0]
+    out_xds_name = '/'.join([combine_chunk_params['combine_file'], antenna, ddi_list[0]])
     if nddi == 0:
-        logger.warning('Nothing to process for ant_id: '+combine_chunk_params['antenna'])
+        logger.warning(f'[{fname}]: Nothing to process for {antenna}')
         return
     elif nddi == 1:
-        logger.info(combine_chunk_params['antenna']+' has a single ddi to be combined, data copied from input file')
-
-        out_xds = _load_image_xds(combine_chunk_params['image_file'],
-                                  combine_chunk_params['antenna'],
-                                  ddi_list[0],
-                                  dask_load=False)
+        logger.info(f'[{fname}]: {antenna} has a single ddi to be combined, data copied from input file')
+        out_xds = ddi_dict[ddi_list[0]]
         out_xds.to_zarr(out_xds_name, mode='w')
     else:
-        out_xds = _load_image_xds(combine_chunk_params['image_file'],
-                                  combine_chunk_params['antenna'],
-                                  ddi_list[0],
-                                  dask_load=False)
+        out_xds = _load_image_xds(combine_chunk_params['image_file'], antenna, ddi_list[0], dask_load=False)
         nddi = len(ddi_list)
         shape = list(out_xds['CORRECTED_PHASE'].values.shape)
         if out_xds.dims['chan'] != 1:
-            raise Exception("Only single channel holographies supported")
+            msg = f'[{fname}]: Only single channel holographies supported'
+            logger.error(msg)
+            raise Exception(msg)
         npol = shape[2]
         npoints = shape[3]*shape[4]
         amp_sum = np.zeros((npol, npoints))
         pha_sum = np.zeros((npol, npoints))
         for ipol in range(npol):
             amp_sum[ipol, :] = out_xds['AMPLITUDE'].values[0, 0, ipol, :, :].ravel()
             if combine_chunk_params['weighted']:
@@ -55,19 +50,16 @@
             else:
                 pha_sum[ipol, :] = out_xds['CORRECTED_PHASE'].values[0, 0, ipol, :, :].ravel()
         wavelength = clight / out_xds.chan.values[0]
         u, v = np.meshgrid(out_xds.u_prime.values * wavelength, out_xds.v_prime.values * wavelength)
         dest_u_axis = u.ravel()
         dest_v_axis = v.ravel()
         for iddi in range(1, nddi):
-            print(iddi)
-            this_xds = _load_image_xds(combine_chunk_params['image_file'],
-                                       combine_chunk_params['antenna'],
-                                       ddi_list[iddi],
-                                       dask_load=False)
+            logger.info(f'[{fname}]: Regridding {antenna} {ddi_list[iddi]}')
+            this_xds = _load_image_xds(combine_chunk_params['image_file'], antenna, ddi_list[iddi], dask_load=False)
             wavelength = clight / this_xds.chan.values[0]
             u, v = np.meshgrid(this_xds.u_prime.values * wavelength, this_xds.v_prime.values * wavelength)
             loca_u_axis = u.ravel()
             loca_v_axis = v.ravel()
             for ipol in range(npol):
                 thispha = this_xds['CORRECTED_PHASE'].values[0, 0, ipol, :, :].ravel()
                 thisamp = this_xds['AMPLITUDE'].values[0, 0, ipol, :, :].ravel()
```

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_constants.py` & `astrohack-0.1.5/src/astrohack/_utils/_constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,9 +31,15 @@
 fourpi = 4.0*constants.pi
 
 # https://github.com/casacore/casacore/blob/dbf28794ef446bbf4e6150653dbe404379a3c429/measures/Measures/Stokes.h
 pol_codes_RL = np.array([5, 6, 7, 8]) #'RR','RL','LR','LL'
 pol_codes_XY = np.array([9, 10, 11, 12]) #['XX','XY','YX','YY']
 pol_str = np.array(['0','I','Q','U','V','RR','RL','LR','LL','XX','XY','YX','YY'])
 
-#Plot types
+# possible complex splits:
+possible_splits = ['cartesian', 'polar']
+
+# Plot convenience
 plot_types = ['deviation', 'phase', 'ancillary', 'all']
+figsize = [8, 6.4]
+fontsize = 6.4
+markersize = 3.2
```

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_conversion.py` & `astrohack-0.1.5/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.1.5/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.1.5/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_extract_holog.py` & `astrohack-0.1.5/src/astrohack/_utils/_extract_holog.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import astropy
 from numba import njit
 from numba.core import types
 
 from casacore import tables as ctables
 from astrohack._utils._imaging import _calculate_parallactic_angle_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._io import _write_meta_data
+from astrohack._utils._dio import _write_meta_data
 from astrohack._utils._algorithms import _get_grid_parms, _significant_digits
 
-from astrohack._utils._io import _load_point_file
+from astrohack._utils._dio import _load_point_file
 
 
 def _extract_holog_chunk(extract_holog_params):
     """Perform data query on holography data chunk and get unique time and state_ids/
 
     Args:
         ms_name (str): Measurementset name
```

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_extract_point.py` & `astrohack-0.1.5/src/astrohack/_utils/_extract_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from casacore import tables
 
 from astropy.time import Time
 
 from astrohack._utils._conversion import convert_dict_from_numba
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
-from astrohack._utils._io import _load_point_file
+from astrohack._utils._dio import _load_point_file
 
 from casacore import tables as ctables
 
 def _extract_pointing(ms_name, pnt_name, parallel=True):
     """Top level function to extract subset of pointing table data into a dictionary of xarray dataarrays.
 
     Args:
@@ -227,16 +227,18 @@
     time_tree = spatial.KDTree(direction_time[:,None]) #Use for nearest interpolation
     mapping_scans_obs_dict = {}
     for ddi_id, ddi in scan_time_dict.items():
         map_scans_dict = {}
         map_id = 0
         
         for scan_id, scan_time in ddi.items():
-            _, time_index = time_tree.query(scan_time[:,None])
+            _, time_index = time_tree.query(scan_time[:, None])
+            
             pointing_offset_scan_slice = pnt_xds["POINTING_OFFSET"].isel(time=slice(time_index[0],time_index[1]))
+            
             r = (np.sqrt(pointing_offset_scan_slice.isel(az_el=0)**2 + pointing_offset_scan_slice.isel(az_el=1)**2)).mean()
             
             if r > 10**-12: #Antenna is mapping since lm is non-zero
                 if ('map_' + str(map_id)) in map_scans_dict:
                     map_scans_dict['map_' + str(map_id)].append(scan_id)
                 else:
                     map_scans_dict['map_' + str(map_id)] = [scan_id]
```

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_gaussfitter.py` & `astrohack-0.1.5/src/astrohack/_utils/_gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_holog.py` & `astrohack-0.1.5/src/astrohack/_utils/_holog.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,66 @@
-import scipy
 import numpy as np
 import xarray as xr
-
+from matplotlib import pyplot as plt
 from scipy.interpolate import griddata
 
 from astrohack._classes.telescope import Telescope
 
-from astrohack._utils._io import _load_holog_file, _load_image_xds
-from astrohack._utils._io import _read_meta_data, _write_meta_data, _write_fits
+from astrohack._utils._dio import _load_holog_file
+from astrohack._utils._dio import _read_meta_data, _write_meta_data, _write_fits
 
-from astrohack._utils._panel import _phase_fitting_block
+from astrohack._utils._phase_fitting import _phase_fitting_block
 
 from astrohack._utils._algorithms import _chunked_average
 from astrohack._utils._algorithms import _find_peak_beam_value
 from astrohack._utils._algorithms import _find_nearest
 from astrohack._utils._algorithms import _calc_coords
 
 from astrohack._utils._conversion import _to_stokes
-from astrohack._utils._constants import clight
-from astrohack._utils._tools import _bool_to_string, _axis_to_fits_header, _stokes_axis_to_fits_header
+from astrohack._utils._constants import clight, figsize
+from astrohack._utils._tools import _bool_to_string, _axis_to_fits_header, _stokes_axis_to_fits_header, \
+    _resolution_to_fits_header, _add_prefix, _well_positioned_colorbar
 
 from astrohack._utils._imaging import _parallactic_derotation
 from astrohack._utils._imaging import _mask_circular_disk
 from astrohack._utils._imaging import _calculate_aperture_pattern
 
+from astrohack._utils._panel import _get_correct_telescope_from_name
+from astrohack._classes.antenna_surface import AntennaSurface
+
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
 
 def _holog_chunk(holog_chunk_params):
     """ Process chunk holography data along the antenna axis. Works with holography file to properly grid , normalize, average and correct data
         and returns the aperture pattern.
 
     Args:
         holog_chunk_params (dict): Dictionary containing holography parameters.
     """
     logger = _get_astrohack_logger()
-    
-    c = scipy.constants.speed_of_light
-    
+    fname = 'holog'
 
     holog_file, ant_data_dict = _load_holog_file(
         holog_chunk_params["holog_file"],
         dask_load=False,
         load_pnt_dict=False,
-        ant_id=holog_chunk_params["ant_id"],
-        ddi_id=holog_chunk_params["ddi_id"]
+        ant_id=holog_chunk_params["this_ant"],
+        ddi_id=holog_chunk_params["this_ddi"]
     )
 
     meta_data = _read_meta_data(holog_chunk_params["holog_file"], 'holog', 'extract_holog')
 
     # Calculate lm coordinates
     l, m = _calc_coords(holog_chunk_params["grid_size"], holog_chunk_params["cell_size"])
     grid_l, grid_m = list(map(np.transpose, np.meshgrid(l, m)))
     
     to_stokes = holog_chunk_params["to_stokes"]
 
-    ddi = holog_chunk_params["ddi_id"]
+    ddi = holog_chunk_params["this_ddi"]
     n_holog_map = len(ant_data_dict[ddi].keys())
     
     # For a fixed ddi the frequency axis should not change over holog_maps, consequently we only have to consider the first holog_map.
     map0 = list(ant_data_dict[ddi].keys())[0]
     
     freq_chan = ant_data_dict[ddi][map0].chan.values
     n_chan = ant_data_dict[ddi][map0].dims["chan"]
@@ -81,15 +82,15 @@
     for holog_map_index, holog_map in enumerate(ant_data_dict[ddi].keys()):
         ant_xds = ant_data_dict[ddi][holog_map]
         
         ###To Do: Add flagging code
 
         # Grid the data
         vis = ant_xds.VIS.values
-        vis[vis==np.nan] = 0.0
+        vis[vis == np.nan] = 0.0
         lm = ant_xds.DIRECTIONAL_COSINES.values
         weight = ant_xds.WEIGHT.values
 
         if holog_chunk_params["chan_average"]:
             vis_avg, weight_sum = _chunked_average(vis, weight, avg_chan_map, avg_freq)
             lm_freq_scaled = lm[:, :, None] * (avg_freq / reference_scaling_frequency)
 
@@ -102,16 +103,15 @@
                 beam_grid[holog_map_index, 0, :, :, :] = (beam_grid[holog_map_index, 0, :, :, :] + np.moveaxis(griddata(lm_freq_scaled[:, :, chan_index], vis_avg[:, chan_index, :], (grid_l, grid_m), method=holog_chunk_params["grid_interpolation_mode"],fill_value=0.0),(2),(0)))
 
             # Avergaing now complete
             n_chan =  1
             
             freq_chan = [np.mean(avg_freq)]
         else:
-            beam_grid[holog_map_index, ...] = np.moveaxis(griddata(lm, vis, (grid_l, grid_m), method=holog_chunk_params["grid_interpolation_mode"],fill_value=0.0), (0,1), (2,3))
-
+            beam_grid[holog_map_index, ...] = np.moveaxis(griddata(lm, vis, (grid_l, grid_m), method=holog_chunk_params["grid_interpolation_mode"], fill_value=0.0), (0,1), (2,3))
 
         time_centroid_index = ant_data_dict[ddi][holog_map].dims["time"] // 2
         time_centroid.append(ant_data_dict[ddi][holog_map].coords["time"][time_centroid_index].values)
 
         for chan in range(n_chan): ### Todo: Vectorize holog_map and channel axis
             try:
                 xx_peak = _find_peak_beam_value(beam_grid[holog_map_index, chan, 0, ...], scaling=0.25)
@@ -126,16 +126,16 @@
 
     beam_grid = _parallactic_derotation(data=beam_grid, parallactic_angle_dict=ant_data_dict[ddi])
     
 
     ###############
     pol = beam_grid,ant_data_dict[ddi][holog_map].pol.values
     if to_stokes:
-        beam_grid = _to_stokes(beam_grid,ant_data_dict[ddi][holog_map].pol.values)
-        pol=['I','Q','U','V']
+        beam_grid = _to_stokes(beam_grid, ant_data_dict[ddi][holog_map].pol.values)
+        pol = ['I', 'Q', 'U', 'V']
     ###############
     
     if holog_chunk_params["scan_average"]:
         beam_grid = np.mean(beam_grid,axis=0)[None,...]
         time_centroid = np.mean(np.array(time_centroid))
     
     # Current bottleneck
@@ -158,15 +158,15 @@
         telescope_name = 'VLA'
 
     else:
         raise Exception("Antenna type not found: {}".format(meta_data['ant_name']))
 
     telescope = Telescope(telescope_name)
 
-    min_wavelength = scipy.constants.speed_of_light/freq_chan[0]
+    min_wavelength = clight/freq_chan[0]
     max_aperture_radius = (0.5*telescope.diam)/min_wavelength
     
     image_slice = aperture_grid[0, 0, 0, ...]
     center_pixel = np.array(image_slice.shape[0:2])//2
     radius_u = int(np.where(np.abs(u) < max_aperture_radius*1.1)[0].max() - center_pixel[0]) # Factor of 1.1: Let's not be too aggresive
     radius_v = int(np.where(np.abs(v) < max_aperture_radius*1.1)[0].max() - center_pixel[1]) # Factor of 1.1: Let's not be too aggresive
         
@@ -203,83 +203,83 @@
         do_cass_off = True
         if telescope.name == 'VLA' or telescope.name == 'VLBA':
             do_sub_til = True
         else:
             do_sub_til = False
     elif isinstance(phase_fit_par, (np.ndarray, list, tuple)):
         if len(phase_fit_par) != 5:
-            logger.error("Phase fit parameter must have 5 elements")
+            logger.error(f'[{fname}]: Phase fit parameter must have 5 elements')
             raise Exception
         else:
             if np.sum(phase_fit_par) == 0:
                 do_phase_fit = False
             else:
                 do_phase_fit = True
                 do_pnt_off, do_xy_foc_off, do_z_foc_off, do_sub_til, do_cass_off = phase_fit_par
     else:
-        logger.error("Phase fit parameter is neither a boolean nor an array of booleans")
+        logger.error(f'[{fname}]: Phase fit parameter is neither a boolean nor an array of booleans.')
         raise Exception
 
     if do_phase_fit:
-        logger.info("Applying phase correction ...")
+        logger.info(f'[{fname}]: Applying phase correction')
         
         if to_stokes:
-            pols=(0,)
+            pols = (0,)
         else:
-            pols=(0, 3)
+            pols = (0, 3)
         
         #? Wavelength
-        max_wavelength = scipy.constants.speed_of_light/freq_chan[-1]
+        max_wavelength = clight/freq_chan[-1]
         
         results, errors, phase_corrected_angle, _, in_rms, out_rms = _phase_fitting_block(
                     pols=pols,
                     wavelength=max_wavelength,
                     telescope=telescope,
                     cellxy=uv_cell_size[0]*max_wavelength, # THIS HAS TO BE CHANGES, (X, Y) CELL SIZE ARE NOT THE SAME.
                     amplitude_image=amplitude,
                     phase_image=phase,
                     pointing_offset=do_pnt_off,
                     focus_xy_offsets=do_xy_foc_off,
                     focus_z_offset=do_z_foc_off,
                     subreflector_tilt=do_sub_til,
                     cassegrain_offset=do_cass_off)
     else:
-        logger.info("Skipping phase correction ...")
+        logger.info('[{fname}]: Skipping phase correction')
 
+    # Here we compute the aperture resolution from Equation 7 In EVLA memo 212
+    # https://library.nrao.edu/public/memos/evla/EVLAM_212.pdf
+    deltal = np.max(l) - np.min(l)
+    deltam = np.max(m) - np.min(m)
+    aperture_resolution = np.array([1/deltal, 1/deltam])
+    aperture_resolution *= 1.27*min_wavelength
     
     ###To Do: Add Paralactic angle as a non-dimension coordinate dependant on time.
     xds = xr.Dataset()
 
     xds["BEAM"] = xr.DataArray(beam_grid, dims=["time", "chan", "pol", "l", "m"])
     xds["APERTURE"] = xr.DataArray(aperture_grid, dims=["time", "chan", "pol", "u", "v"])
     
     xds["AMPLITUDE"] = xr.DataArray(amplitude, dims=["time", "chan", "pol", "u_prime", "v_prime"])
     xds["CORRECTED_PHASE"] = xr.DataArray(phase_corrected_angle, dims=["time", "chan", "pol", "u_prime", "v_prime"])
 
-    xds.attrs["ant_id"] = holog_chunk_params["ant_id"]
+    xds.attrs["aperture_resolution"] = aperture_resolution
+    xds.attrs["ant_id"] = holog_chunk_params["this_ant"]
     xds.attrs["ant_name"] = ant_name
     xds.attrs["telescope_name"] = meta_data['telescope_name']
     xds.attrs["time_centroid"] = np.array(time_centroid)
     xds.attrs["ddi"] = ddi
 
-    coords = {}
+    coords = {"ddi": list(ant_data_dict.keys()), "pol": pol, "l": l, "m": m, "u": u, "v": v, "u_prime": u_prime,
+              "v_prime": v_prime, "chan": freq_chan}
     #coords["time"] = np.array(time_centroid)
-    coords["ddi"] = list(ant_data_dict.keys())
-    coords["pol"] = pol
-    coords["l"] = l
-    coords["m"] = m
-    coords["u"] = u
-    coords["v"] = v
-    coords["u_prime"] = u_prime
-    coords["v_prime"] = v_prime
-    coords["chan"] = freq_chan
 
     xds = xds.assign_coords(coords)
 
-    xds.to_zarr("{name}/{ant}/{ddi}".format(name= holog_chunk_params["image_file"], ant=holog_chunk_params["ant_id"], ddi=ddi), mode="w", compute=True, consolidated=True)
+    xds.to_zarr("{name}/{ant}/{ddi}".format(name=holog_chunk_params["image_file"], ant=holog_chunk_params["this_ant"],
+                                            ddi=ddi), mode="w", compute=True, consolidated=True)
 
 
 def _create_average_chan_map(freq_chan, chan_tolerance_factor):
     n_chan = len(freq_chan)
     cf_chan_map = np.zeros((n_chan,), dtype=int)
 
     orig_width = (np.max(freq_chan) - np.min(freq_chan)) / len(freq_chan)
@@ -325,23 +325,31 @@
     """
     Holog side chunk function for the user facing function export_to_fits
     Args:
         parm_dict: parameter dictionary
     """
     logger = _get_astrohack_logger()
 
-    inputxds = _load_image_xds(parm_dict['filename'], parm_dict['this_antenna'], parm_dict['this_ddi'], dask_load=False)
-    metadata = parm_dict['holog_mds']._meta_data
+    inputxds = parm_dict['xds_data']
+    metadata = parm_dict['metadata']
 
-    antenna = parm_dict['this_antenna']
+    antenna = parm_dict['this_ant']
     ddi = parm_dict['this_ddi']
     destination = parm_dict['destination']
-    basename = f'{destination}/image_{antenna}_{ddi}'
+    basename = f'{destination}/{antenna}_{ddi}'
+    fname = 'export_to_fits'
+
+    logger.info(f'[{fname}]: Exporting image contents of {antenna} {ddi} to FITS files in {destination}')
 
-    logger.info(f'Exporting image contents of {antenna} {ddi} to FITS files in {destination}')
+    try:
+        aperture_resolution = inputxds.attrs["aperture_resolution"]
+    except KeyError:
+        logger.warning(f"[{fname}]: holog image does not have resolution information")
+        logger.warning(f"[{fname}]: Rerun holog with astrohack v>0.1.5 for aperture resolution information")
+        aperture_resolution = None
 
     nchan = len(inputxds.chan)
     if nchan == 1:
         reffreq = inputxds.chan.values[0]
     else:
         reffreq = inputxds.chan.values[nchan//2]
     telname = inputxds.attrs['telescope_name']
@@ -362,52 +370,172 @@
         'CHAN_AVE': _bool_to_string(metadata['chan_average']),
         'CHAN_TOL': metadata['chan_tolerance_factor'],
         'SCAN_AVE': _bool_to_string(metadata['scan_average']),
         'TO_STOKE': _bool_to_string(metadata['to_stokes']),
     }
     ntime = len(inputxds.time)
     if ntime != 1:
-        logger.error("Data with multiple times not supported for FITS export")
-        raise Exception("Data with multiple times not supported for FITS export")
+        logger.error(f"[{fname}]: Data with multiple times not supported for FITS export")
+        raise Exception(f"[{fname}]: Data with multiple times not supported for FITS export")
 
     carta_dim_order = (1, 0, 2, 3, )
 
     baseheader = _axis_to_fits_header(baseheader, inputxds.chan.values, 3, 'Frequency', 'Hz')
     baseheader = _stokes_axis_to_fits_header(baseheader, 4)
 
     beamheader = _axis_to_fits_header(baseheader, inputxds.l.values, 1, 'L', 'rad')
     beamheader = _axis_to_fits_header(beamheader, inputxds.m.values, 2, 'M', 'rad')
     transpobeam = np.transpose(inputxds['BEAM'][0, ...].values, carta_dim_order)
     if parm_dict['complex_split'] == 'cartesian':
-        _write_fits(beamheader, 'Complex beam real part', transpobeam.real, basename + '_beam_real.fits', 'Normalized',
-                    'image')
-        _write_fits(beamheader, 'Complex beam imag part', transpobeam.imag, basename + '_beam_imag.fits', 'Normalized',
-                    'image')
+        _write_fits(beamheader, 'Complex beam real part', transpobeam.real, _add_prefix(basename, 'beam_real')+'.fits',
+                    'Normalized', 'image')
+        _write_fits(beamheader, 'Complex beam imag part', transpobeam.imag, _add_prefix(basename, 'beam_imag')+'.fits',
+                    'Normalized', 'image')
     else:
         _write_fits(beamheader, 'Complex beam amplitude', np.absolute(transpobeam),
-                    basename + '_beam_amplitude.fits', 'Normalized', 'image')
-        _write_fits(beamheader, 'Complex beam phase', np.angle(transpobeam), basename + '_beam_phase.fits',
-                    'Radians', 'image')
+                    _add_prefix(basename, 'beam_amplitude')+'.fits', 'Normalized', 'image')
+        _write_fits(beamheader, 'Complex beam phase', np.angle(transpobeam),
+                    _add_prefix(basename, 'beam_phase')+'.fits', 'Radians', 'image')
 
     apertureheader = _axis_to_fits_header(baseheader, inputxds.u.values, 1, 'X', 'm')
     apertureheader = _axis_to_fits_header(apertureheader, inputxds.v.values, 2, 'Y', 'm')
+    apertureheader = _resolution_to_fits_header(apertureheader, aperture_resolution)
     transpoaper = np.transpose(inputxds['APERTURE'][0, ...].values, carta_dim_order)
     if parm_dict['complex_split'] == 'cartesian':
         _write_fits(apertureheader, 'Complex aperture real part', transpoaper.real,
-                    basename + '_aperture_real.fits', 'Normalized', 'image')
+                    _add_prefix(basename, 'aperture_real')+'.fits', 'Normalized', 'image')
         _write_fits(apertureheader, 'Complex aperture imag part', transpoaper.imag,
-                    basename + '_aperture_imag.fits', 'Normalized', 'image')
+                    _add_prefix(basename, 'aperture_imag')+'.fits', 'Normalized', 'image')
     else:
         _write_fits(apertureheader, 'Complex aperture amplitude', np.absolute(transpoaper),
-                    basename + '_aperture_amplitude.fits', 'Normalized', 'image')
+                    _add_prefix(basename, 'aperture_amplitude')+'.fits', 'Normalized', 'image')
         _write_fits(apertureheader, 'Complex aperture phase', np.angle(transpoaper),
-                    basename + '_aperture_phase.fits', 'rad', 'image')
+                    _add_prefix(basename, 'aperture_phase')+'.fits', 'rad', 'image')
 
     phase_amp_header = _axis_to_fits_header(baseheader, inputxds.u_prime.values, 1, 'X', 'm')
     phase_amp_header = _axis_to_fits_header(phase_amp_header, inputxds.v_prime.values, 2, 'Y', 'm')
+    phase_amp_header = _resolution_to_fits_header(phase_amp_header, aperture_resolution)
     transpoamp = np.transpose(inputxds['AMPLITUDE'][0, ...].values, carta_dim_order)
-    _write_fits(phase_amp_header, 'Cropped aperture amplitude', transpoamp, basename + '_amplitude.fits',
+    _write_fits(phase_amp_header, 'Cropped aperture amplitude', transpoamp, _add_prefix(basename, 'amplitude')+'.fits',
                 'Normalized', 'image')
     transpopha = np.transpose(inputxds['CORRECTED_PHASE'][0, ...].values, carta_dim_order)
-    _write_fits(phase_amp_header, 'Cropped aperture corrected phase', transpopha, basename + '_corrected_phase.fits',
-                'rad', 'image')
+    _write_fits(phase_amp_header, 'Cropped aperture corrected phase', transpopha,
+                _add_prefix(basename, 'corrected_phase')+'.fits', 'rad', 'image')
+    return
+
+
+def _plot_aperture_chunk(parm_dict):
+    """
+    Chunk function for the user facing function plot_apertures
+    Args:
+        parm_dict: parameter dictionary
+    """
+    antenna = parm_dict['this_ant']
+    ddi = parm_dict['this_ddi']
+    destination = parm_dict['destination']
+    basename = f'{destination}/{antenna}_{ddi}'
+    inputxds = parm_dict['xds_data']
+    inputxds.attrs['AIPS'] = False
+    telescope = _get_correct_telescope_from_name(inputxds)
+    surface = AntennaSurface(inputxds, telescope, nan_out_of_bounds=False)
+
+    surface.plot_phase(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'],
+                       colormap=parm_dict['colormap'], figuresize=parm_dict['figuresize'], caller='image',
+                       display=parm_dict['display'])
+    surface.plot_amplitude(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'],
+                           colormap=parm_dict['colormap'], figuresize=parm_dict['figuresize'], caller='image',
+                           display=parm_dict['display'])
+
+
+def _plot_beam_chunk(parm_dict):
+    """
+    Chunk function for the user facing function plot_beams
+    Args:
+        parm_dict: parameter dictionary
+    """
+    antenna = parm_dict['this_ant']
+    ddi = parm_dict['this_ddi']
+    destination = parm_dict['destination']
+    basename = f'{destination}/{antenna}_{ddi}'
+    inputxds = parm_dict['xds_data']
+    laxis = inputxds.l.values
+    maxis = inputxds.m.values
+    if inputxds.dims['chan'] != 1:
+        raise Exception("Only single channel holographies supported")
+    if inputxds.dims['time'] != 1:
+        raise Exception("Only single mapping holographies supported")
+    full_beam = inputxds.BEAM.isel(time=0, chan=0).values
+    pol_axis = inputxds.pol.values
+    if parm_dict['complex_split'] == 'cartesian':
+        realpart = full_beam.real
+        imagpart = full_beam.imag
+        _plot_beam(laxis, maxis, pol_axis, realpart, basename, 'real', antenna, ddi, 'normalized',
+                   figuresize=parm_dict['figuresize'], dpi=parm_dict['dpi'], colormap=parm_dict['colormap'],
+                   display=parm_dict['display'])
+        _plot_beam(laxis, maxis, pol_axis, imagpart, basename, 'real', antenna, ddi, 'normalized',
+                   figuresize=parm_dict['figuresize'], dpi=parm_dict['dpi'], colormap=parm_dict['colormap'],
+                   display=parm_dict['display'])
+    else:
+        ampli = np.absolute(full_beam)
+        phase = np.angle(full_beam)
+        _plot_beam(laxis, maxis, pol_axis, ampli, basename, 'amplitude', antenna, ddi, 'normalized',
+                   figuresize=parm_dict['figuresize'], dpi=parm_dict['dpi'], colormap=parm_dict['colormap'],
+                   display=parm_dict['display'])
+        _plot_beam(laxis, maxis, pol_axis, phase, basename, 'phase', antenna, ddi, 'rad',
+                   figuresize=parm_dict['figuresize'], dpi=parm_dict['dpi'], colormap=parm_dict['colormap'],
+                   display=parm_dict['display'])
+
+
+def _plot_beam(laxis, maxis, pol_axis, data, basename, label, antenna, ddi, unit, figuresize, dpi, colormap, display):
+    """
+    Plot a beam
+    Args:
+        laxis: L axis
+        maxis: M axis
+        pol_axis: Polarization axis
+        data: Beam data
+        basename: Basename for output file
+        label: data label
+        antenna: which antenna
+        ddi: which DDI
+        unit: data unit
+        figuresize: Figure size
+        dpi: DPI
+        colormap: Colormap for plot
+        display: Display plots?
+    """
+    fname = 'plot_beams'
+    logger = _get_astrohack_logger()
+    if colormap is None:
+        colormap = 'viridis'
+    if figuresize is None or figuresize == 'None':
+        figuresize = figsize
+    n_pol = len(pol_axis)
+    if n_pol == 4:
+        fig, axes = plt.subplots(2, 2, figsize=figuresize)
+        axes = axes.flat
+    elif n_pol == 2:
+        fig, axes = plt.subplots(2, 1, figsize=figuresize)
+    elif n_pol == 1:
+        fig, ax = plt.subplots(1, 1, figsize=figuresize)
+        axes = [ax]
+    else:
+        msg = f'[{fname}]: Do not know how to handle polarization axis with {n_pol} elements'
+        logger.error(msg)
+        raise Exception(msg)
+
+    extent = [laxis[0], laxis[-1], maxis[0], maxis[-1]]
+    for ipol, pol, in enumerate(pol_axis):
+        axis = axes[ipol]
+        axis.set_title(f'Polarization: {pol}')
+        im = axis.imshow(data[ipol, ...], cmap=colormap, interpolation="nearest", extent=extent)
+        _well_positioned_colorbar(axis, fig, im, f"Z Scale [{unit}]")
+        axis.set_xlabel('L axis ["]')
+        axis.set_ylabel('M axis ["]')
+
+    fig.suptitle(f'Beam {label}, Antenna: {antenna.split("_")[1]}, DDI: {ddi.split("_")[1]}')
+    fig.tight_layout()
+    fname = _add_prefix(_add_prefix(basename, label), 'image_beam')
+    plt.savefig(fname, dpi=dpi)
+    if not display:
+        plt.close()
     return
```

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_imaging.py` & `astrohack-0.1.5/src/astrohack/_utils/_imaging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 import math
 import scipy
-
 import numpy as np
-
 import astropy.units as u
 import astropy.coordinates as coord
-
 from skimage.draw import disk
-
 from astrohack._utils._algorithms import _calc_coords
-
-from memory_profiler import profile
-
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
+
 def _parallactic_derotation(data, parallactic_angle_dict):
     """ Uses samples of parallactic angle (PA) values to correct differences in PA between maps. The reference PA is selected
         to be the first maps median parallactic angle. All values are rotated to this PA value using scypi.ndimage.rotate(...)
 
     Args:
         data (numpy.ndarray): beam data grid (map, chan, pol, l, m)
         parallactic_angle_dict (dict): dictionary containing antenna selected xds from which the aprallactic angle samples 
@@ -44,57 +38,57 @@
         
         #parallactic_angle = 360 - parallactic_angle_dict[map_value].parallactic_samples[median_index]*180/np.pi
         
         data[map] = scipy.ndimage.rotate(input=data[map, ...], angle=90, axes=(3, 2), reshape=False)
         
     return data
 
+
 def _mask_circular_disk(center, radius, array, mask_value=np.nan):
     """ Create a mask to trim an image
 
     Args:
         center (tuple): tuple describing the center of the image
         radius (int): disk radius
         array (numpy.ndarray): data array to mask
         mask_value (int, optional): Value to set masked value to. Defaults to 1.
-        make_nan (bool, optional): Set maked values to NaN. Defaults to True.
 
     Returns:
         _type_: _description_
     """
     shape = np.array(array.shape[-2:])
 
-    if center == None:
+    if center is None:
         center = shape//2
 
     r, c = disk(center, radius, shape=shape)
     mask = np.zeros(shape, dtype=array.dtype)   
     mask[r, c] = 1
     
     mask = np.tile(mask, reps=(array.shape[:-2] + (1, 1)))
     
-    mask[mask==0] = mask_value
+    mask[mask == 0] = mask_value
     
     return mask
 
+
 def _calculate_aperture_pattern(grid, delta, padding_factor=50):
     """ Calcualtes the aperture illumination pattern from the beam data.
 
     Args:
         grid (numpy.ndarray): gridded beam data
-        frequency (float): channel frequency
         delta (float): incremental spacing between lm values, ie. delta_l = l_(n+1) - l_(n)
         padding_factor (int, optional): Padding to apply to beam data grid before FFT. Padding is applied on outer edged of 
                                         each beam data grid and not between layers. Defaults to 20.
 
     Returns:
         numpy.ndarray, numpy.ndarray, numpy.ndarray: aperture grid, u-coordinate array, v-coordinate array
     """
     logger = _get_astrohack_logger()
-    logger.info("Calculating aperture illumination pattern ...")
+    logger.info("[holog]: Calculating aperture illumination pattern ...")
 
     assert grid.shape[-1] == grid.shape[-2] ###To do: why is this expected that l.shape == m.shape
     initial_dimension = grid.shape[-1]
 
     # Calculate padding as the nearest power of 2
     # k log (2) = log(N) => k = log(N)/log(2)
     # New shape => K = math.ceil(k) => shape = (K, K)
@@ -124,14 +118,15 @@
 
     cell_size = 1 / (image_size * delta)
 
     u, v = _calc_coords(image_size, cell_size)
 
     return aperture_grid, u, v, cell_size
 
+
 def _calculate_parallactic_angle_chunk(
     time_samples,
     observing_location,
     direction,
     dir_frame="FK5",
     zenith_frame="FK5",
 ):
```

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_io.py` & `astrohack-0.1.5/src/astrohack/_utils/_dio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 import os
 import json
 import zarr
 import copy
+import datetime
+import shutil
 import numpy as np
 import xarray as xr
-import datetime
 
 from astropy.io import fits
 from astrohack import __version__ as code_version
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._tools import _numpy_to_json
+from astrohack._utils._tools import _numpy_to_json, _add_prefix
 
 DIMENSION_KEY = "_ARRAY_DIMENSIONS"
 
 
-def check_if_file_exists(file):
+def check_if_file_exists(caller, file):
     logger = _get_astrohack_logger()
 
     if os.path.exists(file) is False:
-        logger.error(
-            " File " + file + " does not exists."
-            )
+        logger.error(f'[{caller}]: File {file} does not exists.')
         raise FileNotFoundError
 
 
-def check_if_file_will_be_overwritten(file,overwrite):
+def check_if_file_will_be_overwritten(caller, file, overwrite):
     logger = _get_astrohack_logger()
     if (os.path.exists(file) is True) and (overwrite is False):
-        logger.error(
-            " {file} already exists. To overwite set the overwrite=True option in extract_holog or remove current file.".format(
-                file=file
-            )
-        )
+        logger.error(f'[{caller}]: {file} already exists. To overwite set overwrite to True, or remove current file.')
         raise FileExistsError
+        
     elif  (os.path.exists(file) is True) and (overwrite is True):
-        logger.warning(
-            file + " will be overwritten."
-        )
+        if file.endswith(".zarr"):
+            logger.warning(f'[{caller}]: {file} will be overwritten.')
+            shutil.rmtree(file)
+        else:
+            logger.warning(f'[{caller}]: {file} may not be valid hack file. Check the file name again.')
+            raise Exception(f"IncorrectFileType: {file}")
 
 
 def _load_panel_file(file=None, panel_dict=None, dask_load=True):
     """ Open panel file.
 
     Args:
         file (str, optional): Path to panel file. Defaults to None.
@@ -68,16 +67,14 @@
                             panel_data_dict[ant][ddi] = xr.open_zarr("{name}/{ant}/{ddi}".format(name=file, ant=ant, ddi=ddi))
                         else:
                             panel_data_dict[ant][ddi] = _open_no_dask_zarr("{name}/{ant}/{ddi}".format(name=file, ant=ant, ddi=ddi))
     
     except Exception as e:
             logger.error(str(e))
             raise
-
-    
     return panel_data_dict
 
 
 def _load_image_file(file=None, image_dict=None,  dask_load=True):
         """ Open hologgraphy file.
 
         Args:s
@@ -125,26 +122,26 @@
     """
     
     logger = _get_astrohack_logger()
     
     if holog_dict is None:
         holog_dict = {}
 
-    if load_pnt_dict == True:
+    if load_pnt_dict:
         logger.info("Loading pointing dictionary to holog ...")
         holog_dict["pnt_dict"] = _load_point_file(file=holog_file, ant_list=None, dask_load=dask_load)
 
     for ddi in os.listdir(holog_file):
         if "ddi_" in ddi:
             
             if ddi_id is None:
                 if ddi not in holog_dict:
                     holog_dict[ddi] = {}
             else:
-                if (ddi == ddi_id):
+                if ddi == ddi_id:
                     holog_dict[ddi] = {}
                 else:
                     continue
                 
             for holog_map in os.listdir(os.path.join(holog_file, ddi)):
                 if "map_" in holog_map:
                     if holog_map not in holog_dict[ddi]:
@@ -158,15 +155,14 @@
 
                                 if dask_load:
                                     holog_dict[ddi][holog_map][ant] = xr.open_zarr(
                                         mapping_ant_vis_holog_data_name
                                     )
                                 else:
                                     holog_dict[ddi][holog_map][ant] = _open_no_dask_zarr(mapping_ant_vis_holog_data_name)
-
     
     if ant_id is None:
         return holog_dict
         
     return holog_dict, _read_data_from_holog_json(holog_file=holog_file, holog_dict=holog_dict, ant_id=ant_id, ddi_id=ddi_id)
 
 
@@ -200,27 +196,42 @@
     Write a dictionary and a dataset to a FITS file
     Args:
         header: The dictionary containing the header
         imagetype: Type to be added to FITS header
         data: The dataset
         filename: The name of the output file
         unit: to be set to bunit
+        origin: Which astrohack mds has created the FITS being written
     """
 
     header['BUNIT'] = unit
     header['TYPE'] = imagetype
     header['ORIGIN'] = f'Astrohack v{code_version}: {origin}'
     header['DATE'] = datetime.datetime.now().strftime('%b %d %Y, %H:%M:%S')
     hdu = fits.PrimaryHDU(data)
     for key in header.keys():
         hdu.header.set(key, header[key])
-    hdu.writeto(filename, overwrite=True)
+    hdu.writeto(_add_prefix(filename, origin), overwrite=True)
     return
 
 
+def _create_destination_folder(caller, destination):
+    """
+    Try to create a folder if it already exists raise a warning
+    Args:
+        caller: Calling function
+        destination: the folder to be created
+    """
+    logger = _get_astrohack_logger()
+    try:
+        os.mkdir(destination)
+    except FileExistsError:
+        logger.warning(f'[{caller}]: Destination folder already exists, results may be overwritten')
+
+
 def _aips_holog_to_xds(ampname, devname):
     """
     Read amplitude and deviation FITS files onto a common Xarray dataset
     Args:
         ampname: Name of the amplitude FITS file
         devname: Name of the deviation FITS file
 
@@ -313,21 +324,23 @@
         file_type (str): astrohack file type
         origin (str, list): Astrohack expected origin(s)
 
     Returns:
         dict: dictionary containing dimension data.
     """
     logger = _get_astrohack_logger()
+    
     try:
         with open(f'{file_name}/.{file_type}_attr') as json_file:
             json_dict = json.load(json_file)
 
     except Exception as error:
         logger.error(str(error))
         raise
+        
 
     try:
         metadataorigin = json_dict['origin']
     except KeyError:
         logger.error("[_read_meta_data]: Badly formatted metadata in input file")
         raise Exception('Bad metadata')
     if isinstance(origin, str):
```

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.1.5/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_panel.py` & `astrohack-0.1.5/src/astrohack/_utils/_phase_fitting.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,12 @@
 import numpy as np
-
 from numba import njit
 
-from astrohack._utils._conversion import _convert_unit
 from astrohack._utils._algorithms import _least_squares_fit_block
-from astrohack._utils._constants import plot_types
-from astrohack._utils._io import _load_image_xds
-
-from astrohack._classes.telescope import Telescope
-from astrohack._classes.antenna_surface import AntennaSurface
-from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-
-# global constants
-NPAR = 10
-
-
-def _panel_chunk(panel_chunk_params):
-    """
-    Process a chunk of the holographies, usually a chunk consists of an antenna over a ddi
-    Args:
-        panel_chunk_params: dictionary of inputs
-    """
-    logger = _get_astrohack_logger()
-    if panel_chunk_params['origin'] == 'AIPS':
-        inputxds = xr.open_zarr(panel_chunk_params['image_name'])
-        telescope = Telescope(inputxds.attrs['telescope_name'])
-        panel_chunk_params['antenna'] = inputxds.attrs['ant_name']
-
-    else:
-        ddi = panel_chunk_params['this_ddi']
-        antenna = panel_chunk_params['this_antenna']
-        inputxds = _load_image_xds(panel_chunk_params['image_name'], antenna, ddi, dask_load=False)
-
-        logger.info(f'[panel]: processing antenna {antenna} DDI {ddi}')
-        inputxds.attrs['AIPS'] = False
-
-        if inputxds.attrs['telescope_name'] == "ALMA":
-            tname = inputxds.attrs['telescope_name']+'_'+inputxds.attrs['ant_name'][0:2]
-            telescope = Telescope(tname)
-        elif inputxds.attrs['telescope_name'] == "EVLA":
-            tname = "VLA"
-            telescope = Telescope(tname)
-        else:
-            raise ValueError('Unsuported telescope {0:s}'.format(inputxds.attrs['telescope_name']))
-
-    surface = AntennaSurface(inputxds, telescope, panel_chunk_params['cutoff'], panel_chunk_params['panel_kind'],
-                             panel_margins=panel_chunk_params['panel_margins'])
-
-    surface.compile_panel_points()
-    surface.fit_surface()
-    surface.correct_surface()
-    
-    xds_name = panel_chunk_params['panel_name'] + f'/{antenna}/{ddi}'
-    xds = surface.export_xds()
-    xds.to_zarr(xds_name, mode='w')
+from astrohack._utils._conversion import _convert_unit
 
 
 def _create_phase_model(npix, parameters, wavelength, telescope, cellxy):
     """
     Create a phase model with npix by npix size according to the given parameters
     Args:
         npix: Number of pixels in each size of the model
@@ -73,14 +22,17 @@
     dummyphase = np.zeros((npix, npix))
 
     _, model = _correct_phase(dummyphase, cellxy, iNPARameters, telescope.magnification, telescope.focus,
                               telescope.surp_slope)
     return model
 
 
+NPAR = 10
+
+
 def _phase_fitting_block(pols, wavelength, telescope, cellxy, amplitude_image, phase_image, pointing_offset,
                          focus_xy_offsets, focus_z_offset, subreflector_tilt, cassegrain_offset):
     """
     Corrects the grading phase for pointing, focus, and feed offset errors using the least squares method, and a model
     incorporating subreflector position errors.  Includes reference pointing
 
     This is a revised version of the task, offering a two-reflector solution.  M. Kesteven, 6/12/1994
@@ -200,15 +152,15 @@
     iNPARameters[3:] /= scaling
     # Sub-reflector tilt from degrees
     rad2deg = _convert_unit('rad', 'deg', 'trigonometric')
     iNPARameters[6:8] /= rad2deg / (1000.0 * telescope.secondary_dist)
     # rescale phase ramp to pointing offset
     iNPARameters[1:3] /= wavelength * rad2deg / 6. / cellxy
     iNPARameters /= rad2deg
-    
+
     return iNPARameters
 
 
 def _ignore_non_fitted(ignored, matrix, vector):
     """
     Disable the fitting of certain parameters by removing rows and columns from the design matrix and its associated
     vector
@@ -346,15 +298,15 @@
 
     matrix = np.zeros((ntime, nchan, npols, NPAR, NPAR))
     vector = np.zeros((ntime, nchan, npols, NPAR))
     ixymin = abs(xymin/cellxy)
     ixymax = abs(xymax/cellxy)
     min_squared_pix_radius = (xymin*xymin)/(cellxy*cellxy)
     max_squared_pix_radius = (xymax*xymax)/(cellxy*cellxy)
-    
+
     for time in range(ntime):
         for chan in range(nchan):
             for pol in pols:
                 for ix in range(npix):
                     x_delta_pix = abs(ix - ix0)
                     #   check absolute limits.
                     if xymin > 0.0 and x_delta_pix < ixymin:
@@ -383,21 +335,21 @@
                         #   outer limits.
                         if xymax > 0.0:
                             if y_delta_pix > ixymax:
                                 continue
                         elif xymax < 0.0:
                             if radius_pix_squared > max_squared_pix_radius:
                                 continue
-                        
+
                         #   evaluate variables (in cells)
                         weight = amplitude_image[time, chan, pol, ix, iy]
-                        
+
                         x_delta_pix = ix - ix0
                         y_delta_pix = iy - iy0
-                        
+
                         x_focus, y_focus, z_focus, x_tilt, y_tilt, x_cass, y_cass = _matrix_coeffs(x_delta_pix, y_delta_pix,
                                                                                                    magnification, focal_length,
                                                                                                    cellxy, phase_slope)
 
                         #  build the design matrix.
                         vector[time, chan, ipol, 0] += phase * weight
                         vector[time, chan, ipol, 1] += phase * x_delta_pix * weight
@@ -628,67 +580,7 @@
     ntime, nchan, npol = phase_image.shape[:3]
     rms = np.zeros((ntime, nchan, npol))
     for time in range(ntime):
         for chan in range(nchan):
             for pol in range(npol):
                 rms[time, chan, pol] = np.sqrt(np.nanmean(phase_image[time, chan, pol] ** 2))
     return rms
-
-
-def _plot_antenna_chunk(parm_dict):
-    """
-    Chunk function for the user facing function plot_antenna
-    Args:
-        parm_dict: parameter dictionary
-    """
-    antenna = parm_dict['this_antenna']
-    ddi = parm_dict['this_ddi']
-    destination = parm_dict['destination']
-    plot_type = parm_dict['plot_type']
-    basename = f'{destination}/{antenna}_{ddi}'
-    surface = parm_dict['panel_mds'].get_antenna(antenna, ddi, dask_load=False)
-    if plot_type == plot_types[0]:  # deviation plot
-        surface.plot_deviation(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'])
-    elif plot_type == plot_types[1]:  # phase plot
-        surface.plot_phase(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'])
-    elif plot_type == plot_types[2]:  # Ancillary plot
-        surface.plot_mask(basename=basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'])
-        surface.plot_amplitude(basename=basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'])
-    else: # all plots
-        surface.plot_deviation(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'])
-        surface.plot_phase(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'])
-        surface.plot_mask(basename=basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'])
-        surface.plot_amplitude(basename=basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'])
-
-
-def _export_to_fits_panel_chunk(parm_dict):
-    """
-    Panel side chunk function for the user facing function export_to_fits
-    Args:
-        parm_dict: parameter dictionary
-    """
-    logger = _get_astrohack_logger()
-    antenna = parm_dict['this_antenna']
-    ddi = parm_dict['this_ddi']
-    destination = parm_dict['destination']
-    logger.info(f'Exporting panel contents of {antenna} {ddi} to FITS files in {destination}')
-    surface = parm_dict['panel_mds'].get_antenna(antenna, ddi, dask_load=False)
-    basename = f'{destination}/panel_{antenna}_{ddi}'
-    surface.export_to_fits(basename)
-    return
-
-
-def _export_screws_chunk(parm_dict):
-    """
-    Chunk function for the user facing function export_screws
-    Args:
-        parm_dict: parameter dictionary
-    """
-    antenna = parm_dict['this_antenna']
-    ddi = parm_dict['this_ddi']
-    export_name = parm_dict['destination'] + f'/screws_{antenna}_{ddi}.'
-    surface = parm_dict['panel_mds'].get_antenna(antenna, ddi, dask_load=False)
-    surface.export_screws(export_name + 'csv', unit=parm_dict['unit'])
-    if parm_dict['plot_map']:
-        surface.plot_screw_adjustments(export_name + 'png', unit=parm_dict['unit'], threshold=parm_dict['threshold'],
-                                       colormap=parm_dict['colormap'], figuresize=parm_dict['figuresize'],
-                                       dpi=parm_dict['dpi'])
```

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.1.5/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,34 +13,30 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 #ducting - code is complex and might fail after some time if parameters is wrong. Sensable values are also checked. Gives printout of all wrong parameters.
 
 import numpy as np
-from  ._check_parms import _check_parms
+from ._check_parms import _check_parms
 
 
 def _check_logger_parms(logger_parms):
-    import numbers
     parms_passed = True
-    arc_sec_to_rad = np.pi / (3600 * 180)
-    
-    if not(_check_parms(logger_parms, 'log_to_term', [bool],default=True)): parms_passed = False
-    if not(_check_parms(logger_parms, 'log_to_file', [bool],default=False)): parms_passed = False
-    if not(_check_parms(logger_parms, 'log_file', [str],default='hack_')): parms_passed = False
-    if not(_check_parms(logger_parms, 'log_level', [str],default='INFO',acceptable_data=['DEBUG','INFO','WARNING','ERROR'])): parms_passed = False
+    fname = '_check_logger_parms'
+    if not(_check_parms(fname, logger_parms, 'log_to_term', [bool],default=True)): parms_passed = False
+    if not(_check_parms(fname, logger_parms, 'log_to_file', [bool],default=False)): parms_passed = False
+    if not(_check_parms(fname, logger_parms, 'log_file', [str],default='hack_')): parms_passed = False
+    if not(_check_parms(fname, logger_parms, 'log_level', [str],default='INFO',acceptable_data=['DEBUG','INFO','WARNING','ERROR'])): parms_passed = False
     
     return parms_passed
 
 
 def _check_worker_logger_parms(logger_parms):
-    import numbers
     parms_passed = True
-    arc_sec_to_rad = np.pi / (3600 * 180)
-    
-    if not(_check_parms(logger_parms, 'log_to_term', [bool],default=False)): parms_passed = False
-    if not(_check_parms(logger_parms, 'log_to_file', [bool],default=False)): parms_passed = False
-    if not(_check_parms(logger_parms, 'log_file', [str],default='hack_')): parms_passed = False
-    if not(_check_parms(logger_parms, 'log_level', [str],default='INFO',acceptable_data=['DEBUG','INFO','WARNING','ERROR'])): parms_passed = False
+    fname = '_check_worker_logger_parms'
+    if not(_check_parms(fname, logger_parms, 'log_to_term', [bool],default=False)): parms_passed = False
+    if not(_check_parms(fname, logger_parms, 'log_to_file', [bool],default=False)): parms_passed = False
+    if not(_check_parms(fname, logger_parms, 'log_file', [str],default='hack_')): parms_passed = False
+    if not(_check_parms(fname, logger_parms, 'log_level', [str],default='INFO',acceptable_data=['DEBUG','INFO','WARNING','ERROR'])): parms_passed = False
     
     return parms_passed
```

### Comparing `astrohack-0.1.4/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.1.5/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,118 +13,138 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 import numpy as np
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
 
-def _check_parm(parm, parm_name, acceptable_data_types, acceptable_data = None, acceptable_range = None, list_acceptable_data_types=None, list_len=None, default=None):
+def _check_parm(parm, parm_name, acceptable_data_types, acceptable_data=None, acceptable_range=None,
+                list_acceptable_data_types=None, list_len=None, default=None):
     parm_dict = {parm_name:parm}
-    parm_passed =  _check_parms(parm_dict, parm_name, acceptable_data_types, acceptable_data, acceptable_range, list_acceptable_data_types, list_len, default)
+    parm_passed = _check_parms(parm_dict, parm_name, acceptable_data_types, acceptable_data, acceptable_range,
+                               list_acceptable_data_types, list_len, default)
     
     parm = parm_dict[parm_name]
     
     return parm_passed, parm
 
-def _check_parms(parm_dict, string_key, acceptable_data_types, acceptable_data = None, acceptable_range = None, list_acceptable_data_types=None, list_len=None, default=None, log_default_setting=True):
+
+def _check_parms(caller, parm_dict, string_key, acceptable_data_types, acceptable_data=None, acceptable_range=None,
+                 list_acceptable_data_types=None, list_len=None, default=None, log_default_setting=True):
     """
 
     Parameters
     ----------
     parm_dict: dict
-        The dictionary in which the a parameter will be checked
+        The dictionary in which the parameter will be checked
     string_key :
     acceptable_data_types : list
     acceptable_data : list
     acceptable_range : list (length of 2)
     list_acceptable_data_types : list
     list_len : int
         If list_len is -1 than the list can be any length.
     default :
     Returns
     -------
     parm_passed : bool
         
     """
-
-    import numpy as np
     logger = _get_astrohack_logger()
-    
 
     if (string_key in parm_dict) and (parm_dict[string_key] is not None):
-        if (list in acceptable_data_types) or (np.ndarray in acceptable_data_types):
-            if (len(parm_dict[string_key]) != list_len) and (list_len is not None):
-                logger.error('Parameter ' + str(string_key) + ' must be a list of '+ str(list_acceptable_data_types) + ' and length'+ str(list_len) + '. Wrong length.')
-                return False
-            else:
-                list_len = len(parm_dict[string_key])
-                for i in range(list_len):
-                    type_check = False
-                    for lt in list_acceptable_data_types:
-                        if isinstance(parm_dict[string_key][i], lt):
-                            type_check = True
-                    if not(type_check):
-                          logger.error('Parameter '+ str(string_key)+ ' must be a list of '+ str(list_acceptable_data_types)+ ' and length '+ str(list_len)+ '. Wrong type of'+str(type(parm_dict[string_key][i])))
-                          return False
-                          
-                    if acceptable_data is not None:
-                        if not(parm_dict[string_key][i] in acceptable_data):
-                            logger.error('Invalid '+ str(string_key)+'. Can only be one of '+str(acceptable_data)+'.')
-                            return False
-                            
-                    if acceptable_range is not None:
-                        if (parm_dict[string_key][i] < acceptable_range[0]) or (parm_dict[string_key][i] > acceptable_range[1]):
-                            logger.error('Invalid '+ str(string_key) +'. Must be within the range '+ str(acceptable_range)+'.')
+        parm_type = type(parm_dict[string_key])
+        if parm_type in acceptable_data_types:
+            if (parm_type is list) or (parm_type is np.ndarray):
+                if (len(parm_dict[string_key]) != list_len) and (list_len is not None):
+                    logger.error(f'[{caller}]: Parameter {str(string_key)} must be a list of '
+                                 f'{str(list_acceptable_data_types)} and length {str(list_len)}. Wrong length.')
+                    return False
+                else:
+                    list_len = len(parm_dict[string_key])
+                    for i in range(list_len):
+                        type_check = False
+                        for lt in list_acceptable_data_types:
+                            if isinstance(parm_dict[string_key][i], lt):
+                                type_check = True
+                        if not type_check:
+                            logger.error(f'[{caller}]: Parameter {str(string_key)} must be a list of '
+                                         f'{str(list_acceptable_data_types)} and length {str(list_len)}. Wrong type of '
+                                         f'{str(type(parm_dict[string_key][i]))}.')
                             return False
-        elif (dict in acceptable_data_types):
-            parms_passed = True
 
-            if default is None:
-                logger.error('Dictionary parameters must have a default. Please report bug.')
-                return False
-            for default_element in default:
-                if default_element in parm_dict[string_key]:
-                    if not(_check_parms(parm_dict[string_key], default_element, [type(default[default_element])], default=default[default_element])): parms_passed = False
-                else:
-                    parm_dict[string_key][default_element] = default[default_element]
-                    
-                    if log_default_setting:
-                        logger.info('Setting default '+ str(string_key)+ '[\''+str(default_element)+'\']'+ ' to '+ str(default[default_element]))
-                    
-            return parms_passed
-                    
-        else:
+                        if acceptable_data is not None:
+                            if not(parm_dict[string_key][i] in acceptable_data):
+                                logger.error(f'[{caller}]: Invalid {str(string_key)}. Can only be one of '
+                                             f'{+str(acceptable_data)}.')
+                                return False
+
+                        if acceptable_range is not None:
+                            if (parm_dict[string_key][i] < acceptable_range[0]) or (parm_dict[string_key][i] >
+                                                                                    acceptable_range[1]):
+                                logger.error(f'[{caller}]: Invalid {str(string_key)}. Must be within the range '
+                                             f'{str(acceptable_range)}.')
+                                return False
+            elif parm_type is dict:
+                parms_passed = True
 
-            type_check = False
-            for adt in acceptable_data_types:
-                if isinstance(parm_dict[string_key], adt):
-                    type_check = True
-            if not(type_check):
-                logger.error('Parameter '+ str(string_key) + ' must be of type '+ str(acceptable_data_types))
-                return False
-                    
-            if acceptable_data is not None:
-                if not(parm_dict[string_key] in acceptable_data):
-                    logger.error('Invalid '+ str(string_key) +'. Can only be one of '+ str(acceptable_data) +'.')
+                if default is None:
+                    logger.error(f'[{caller}]: Dictionary parameters must have a default. Please report bug.')
                     return False
-                    
-            if acceptable_range is not None:
-                if (parm_dict[string_key] < acceptable_range[0]) or (parm_dict[string_key] > acceptable_range[1]):
-                    logger.error('Invalid '+ str(string_key) +'. Must be within the range '+ str(acceptable_range)+'.')
+                for default_element in default:
+                    if default_element in parm_dict[string_key]:
+                        if not(_check_parm(parm_dict[string_key], default_element, [type(default[default_element])],
+                                           default=default[default_element])):
+                            parms_passed = False
+                    else:
+                        parm_dict[string_key][default_element] = default[default_element]
+
+                        if log_default_setting:
+                            logger.info(f'[{caller}]: Setting default {str(string_key)} [\'{str(default_element)}\'] to '
+                                        f'{str(default[default_element])}.')
+
+                return parms_passed
+
+            else:
+
+                type_check = False
+                for adt in acceptable_data_types:
+                    if isinstance(parm_dict[string_key], adt):
+                        type_check = True
+                if not type_check:
+                    logger.error(f'[{caller}]: Parameter {str(string_key)} must be of type {str(acceptable_data_types)}.')
                     return False
+
+                if acceptable_data is not None:
+                    if not(parm_dict[string_key] in acceptable_data):
+                        logger.error(f'[{caller}]: Invalid {str(string_key)}. Can only be one of {str(acceptable_data)}.')
+                        return False
+
+                if acceptable_range is not None:
+                    if (parm_dict[string_key] < acceptable_range[0]) or (parm_dict[string_key] > acceptable_range[1]):
+                        logger.error(f'[{caller}]: Invalid {str(string_key)}. Must be within the range '
+                                     f'{str(acceptable_range)}.')
+                        return False
+        else:
+            logger.error(f'[{caller}]: Parameter {str(string_key)} is not of correct type.')
+            return False
     else:
         if default is not None:
-            parm_dict[string_key] =  default
+            parm_dict[string_key] = default
             
             if log_default_setting:
-                logger.info('Setting default '+ str(string_key)+ ' to '+ str(parm_dict[string_key]))
+                logger.info(f'[{caller}]: Setting default {str(string_key)} to {str(parm_dict[string_key])}.')
         else:
-            logger.error('Parameter '+ str(string_key)+ ' must be specified')
+            logger.error(f'[{caller}]: Parameter {str(string_key)} must be specified.')
             return False
     
     return True
 
 
-    
+def _parm_check_passed(caller, parms_passed):
+    logger = _get_astrohack_logger()
+    if not parms_passed:
+        logger.error(f"{caller} parameter checking failed.")
+        raise Exception(f"{caller} parameter checking failed.")
```

### Comparing `astrohack-0.1.4/src/astrohack/astrohack_client.py` & `astrohack-0.1.5/src/astrohack/astrohack_client.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/combine.py` & `astrohack-0.1.5/src/astrohack/combine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-import os
-import dask
 import numpy as np
 
 from astrohack._utils._combine import _combine_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._parm_utils._check_parms import _check_parms
+from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
-from astrohack._utils._io import check_if_file_will_be_overwritten, check_if_file_exists, _write_meta_data
-from astrohack._utils._dio import AstrohackImageFile
+from astrohack._utils._dio import check_if_file_will_be_overwritten, check_if_file_exists, _write_meta_data
+from astrohack._utils._mds import AstrohackImageFile
+from astrohack._utils._dask_graph_tools import _dask_general_compute
 
 
-def combine_image_ddi(image_name, combine_name=None, ant_list=None, ddi_list=None, weighted=False, parallel=False,
-                      overwrite=False):
+def combine(image_name, combine_name=None, ant_id=None, ddi=None, weighted=False, parallel=False,
+            overwrite=False):
     """Combine DDIs in a Holography image to increase SNR
 
     :param image_name: Input holography data file name. Accepted data format is the output from ``astrohack.holog.holog``
     :type image_name: str
     :param combine_name: Name of output file; File name will be appended with suffix *.combine.zarr*. Defaults to *basename* of input file plus holography panel file suffix.
     :type combine_name: str, optional
-    :param ant_list: List of Antennae to be processed. None will use all antennae. Defaults to None
-    :type ant_list: list, optional, ex. [ant_ea25 ... ant_ea04]
-    :param ddi_list: List of DDIs to be combined. None will use all DDIs. Defaults to None.
-    :type ddi_list: list, optional, ex. [ddi_0 ... ddi_N]
-    :param weighted: Weight phases by the corresponding amplitudes
+    :param ant_id: List of Antennae to be processed. None will use all antennae. Defaults to None, ex. ea25.
+    :type ant_id: list or str, optional
+    :param ddi: List of DDIs to be combined. None will use all DDIs. Defaults to None, ex. [0, ..., 8].
+    :type ddi: list of int, optional
+    :param weighted: Weight phases by the corresponding amplitudes.
     :type weighted: bool, optional
     :param parallel: Run in parallel. Defaults to False.
     :type parallel: bool, optional
     :param overwrite: Overwrite files on disk. Defaults to False.
     :type overwrite: bool, optional
 
     :return: Holography image object.
@@ -46,70 +45,57 @@
                 ddi_m: image_ds
             },
             ⋮
             ant_n: …
         }
     """
     logger = _get_astrohack_logger()
-
-    combine_params = _check_combine_parms(image_name, combine_name, ant_list, ddi_list, weighted, parallel,  overwrite)
+    fname = 'combine'
+    combine_params = _check_combine_parms(fname, image_name, combine_name, ant_id, ddi, weighted, parallel,
+                                          overwrite)
     input_params = combine_params.copy()
 
-    check_if_file_exists(combine_params['image_file'])
-    check_if_file_will_be_overwritten(combine_params['combine_file'], combine_params['overwrite'])
+    check_if_file_exists(fname, combine_params['image_file'])
+    check_if_file_will_be_overwritten(fname, combine_params['combine_file'], combine_params['overwrite'])
 
-    if combine_params['ant_list'] == 'all':
-        antennae = os.listdir(combine_params['image_file'])
+    image_mds = AstrohackImageFile(combine_params['image_file'])
+    image_mds._open()
+    combine_params['image_mds'] = image_mds
+
+    if _dask_general_compute(fname, image_mds, _combine_chunk, combine_params, ['ant'], parallel=parallel):
+        logger.info(f"[{fname}]: Finished processing")
+        output_attr_file = "{name}/{ext}".format(name=combine_params['combine_file'], ext=".image_attr")
+        _write_meta_data('combine', output_attr_file, input_params)
+        combine_mds = AstrohackImageFile(combine_params['combine_file'])
+        combine_mds._open()
+        return combine_mds
     else:
-        antennae = combine_params['ant_list']
-
-    delayed_list = []
-    combine_chunk_params = combine_params
-    for antenna in antennae:
-        combine_chunk_params['antenna'] = antenna
-        logger.info("Processing ant_id: " + str(antenna))
-        if parallel:
-            delayed_list.append(dask.delayed(_combine_chunk)(dask.delayed(combine_chunk_params)))
-        else:
-            _combine_chunk(combine_chunk_params)
-
-    if parallel:
-        dask.compute(delayed_list)
-
-    output_attr_file = "{name}/{ext}".format(name=combine_params['combine_file'], ext=".image_attr")
-    _write_meta_data('combine', output_attr_file, input_params)
-
-    combine_mds = AstrohackImageFile(combine_chunk_params['combine_file'])
-    combine_mds.open()
+        logger.warning(f"[{fname}]: No data to process")
+        return None
 
-    return combine_mds
 
-
-def _check_combine_parms(image_name, combine_name, ant_list, ddi_list, weighted, parallel,  overwrite):
+def _check_combine_parms(fname, image_name, combine_name, ant_id, ddi_list, weighted, parallel, overwrite):
 
     combine_params = {"image_file": image_name,
                       "combine_file": combine_name,
-                      "ant_list": ant_list,
-                      "ddi_list": ddi_list,
+                      "ant": ant_id,
+                      "ddi": ddi_list,
                       "weighted": weighted,
                       "parallel": parallel,
                       "overwrite": overwrite}
 
     #### Parameter Checking ####
-    logger = _get_astrohack_logger()
-
-    parms_passed = _check_parms(combine_params, 'image_file', [str], default=None)
+    parms_passed = _check_parms(fname, combine_params, 'image_file', [str], default=None)
     base_name = _remove_suffix(combine_params['image_file'], '.image.zarr')
-    parms_passed = parms_passed and _check_parms(combine_params, 'combine_file', [str], default=base_name+'.combine.zarr')
-    parms_passed = parms_passed and _check_parms(combine_params, 'ant_list', [list, np.ndarray],
+    parms_passed = parms_passed and _check_parms(fname, combine_params, 'combine_file', [str],
+                                                 default=base_name+'.combine.zarr')
+    parms_passed = parms_passed and _check_parms(fname, combine_params, 'ant', [str, list],
                                                  list_acceptable_data_types=[str], default='all')
-    parms_passed = parms_passed and _check_parms(combine_params, 'ddi_list', [list, np.ndarray],
-                                                 list_acceptable_data_types=[str], default='all')
-    parms_passed = parms_passed and _check_parms(combine_params, 'parallel', [bool], default=False)
-    parms_passed = parms_passed and _check_parms(combine_params, 'weighted', [bool], default=False)
-    parms_passed = parms_passed and _check_parms(combine_params, 'overwrite', [bool], default=False)
-
-    if not parms_passed:
-        logger.error("extract_combine parameter checking failed.")
-        raise Exception("extract_combine parameter checking failed.")
+    parms_passed = parms_passed and _check_parms(fname, combine_params, 'ddi', [int, list],
+                                                 list_acceptable_data_types=[int], default='all')
+    parms_passed = parms_passed and _check_parms(fname, combine_params, 'parallel', [bool], default=False)
+    parms_passed = parms_passed and _check_parms(fname, combine_params, 'weighted', [bool], default=False)
+    parms_passed = parms_passed and _check_parms(fname, combine_params, 'overwrite', [bool], default=False)
+
+    _parm_check_passed(fname, parms_passed)
     #### End Parameter Checking ####
     return combine_params
```

### Comparing `astrohack-0.1.4/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json` & `astrohack-0.1.5/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'notes'": "'The pointing table for this measurement set has been corrected => for all reference "*

 * *            'antennas, pointing_offset=0; target=direction. In addition, this file has been split, '*

 * *            "including the pointing table, to include only antennas ea04, ea25, ea06'"}*

```diff
@@ -5,15 +5,15 @@
     "channels": 57,
     "corrs": "RR RL LR LL",
     "dec": "+16.08.53.56089",
     "elapsed time": "10792 seconds",
     "epoch": "J2000",
     "frame": "TOPO",
     "name": "EVLA_KU#A0C0#1",
-    "notes": "ant_ea25 panels shifted. The pointing table for this measurement set has been corrected => for all reference antennas, pointing_offset=0; target=direction",
+    "notes": "The pointing table for this measurement set has been corrected => for all reference antennas, pointing_offset=0; target=direction. In addition, this file has been split, including the pointing table, to include only antennas ea04, ea25, ea06",
     "observed": "13-Sep-2022/02:40:29.0 to 13-Sep-2022/05:40:21.0 (UTC)",
     "observer": "Bryan Butler",
     "project": "uid://evla/pdb/4538748",
     "ra": "22:53:57.747932",
     "spwID": 0,
     "total-bandwidth": 114000
 }
```

### Comparing `astrohack-0.1.4/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json` & `astrohack-0.1.5/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6764705882352942%*

 * *Differences: {"'center-frequency'": '109994.575',*

 * * "'chan-width'": '31250.0',*

 * * "'chan0'": '109010.2',*

 * * "'channels'": '64',*

 * * "'corrs'": "'XX XY YX YY'",*

 * * "'dec'": "'-29.14.30.12106'",*

 * * "'epoch'": "'ICRS'",*

 * * "'name'": "'X0000000000#ALMA_RB_03#BB_4#SW-01#FULL_RES'",*

 * * "'notes'": "'The pointing table for this measurement set has been corrected => for all reference "*

 * *            'antennas, pointing_offset=0; target=direction. In addition, this file has been split, '*

 * *            "including the pointing table, to include only a […]*

```diff
@@ -1,19 +1,19 @@
 {
-    "center-frequency": 14168.0,
-    "chan-width": 2000.0,
-    "chan0": 14112.0,
-    "channels": 57,
-    "corrs": "RR RL LR LL",
-    "dec": "+16.08.53.56089",
+    "center-frequency": 109994.575,
+    "chan-width": 31250.0,
+    "chan0": 109010.2,
+    "channels": 64,
+    "corrs": "XX XY YX YY",
+    "dec": "-29.14.30.12106",
     "elapsed time": "10791 seconds",
-    "epoch": "J2000",
+    "epoch": "ICRS",
     "frame": "TOPO",
-    "name": "EVLA_KU#A0C0#1",
-    "notes": "The pointing table for this measurement set has been corrected => for all reference antennas, pointing_offset=0; target=direction",
+    "name": "X0000000000#ALMA_RB_03#BB_4#SW-01#FULL_RES",
+    "notes": "The pointing table for this measurement set has been corrected => for all reference antennas, pointing_offset=0; target=direction. In addition, this file has been split, including the pointing table, to include only antennas ea04, ea25, ea06",
     "observed": "20-Sep-2022/01:28:37.0 to 20-Sep-2022/04:28:28.0 (UTC)",
     "observer": "Bryan Butler",
     "project": "uid://evla/pdb/4538748",
-    "ra": "22:53:57.747932",
+    "ra": "19:24:51.055956",
     "spwID": 0,
-    "total-bandwidth": 114000
+    "total-bandwidth": 2000000.0
 }
```

### Comparing `astrohack-0.1.4/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.1.5/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.1.5/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.1.5/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.1.5/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.1.5/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.1.5/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.1.5/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.1.5/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.1.5/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.1.5/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.1.5/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.1.5/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/extract_holog.py` & `astrohack-0.1.5/src/astrohack/extract_holog.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,95 +1,70 @@
 import os
 import dask
-import sys
 import json
 import copy
-
-import xarray as xr
 import numpy as np
 import numbers
+from astropy.time import Time
 
-from casacore import tables as ctables
+from pprint import pformat
 
-from astropy.time import Time
+from casacore import tables as ctables
 
 from astrohack._utils._constants import pol_str
-
 from astrohack._utils._conversion import _convert_ant_name_to_id
-
 from astrohack._utils._extract_holog import _create_holog_meta_data
 from astrohack._utils._extract_point import _extract_pointing
-
-from astrohack._utils._io import _load_point_file
-from astrohack._utils._io import _open_no_dask_zarr
-from astrohack._utils._io import _read_data_from_holog_json
-from astrohack._utils._io import _read_meta_data
-from astrohack._utils._io import _load_holog_file
-from astrohack._utils._io import  check_if_file_will_be_overwritten, check_if_file_exists
-from astrohack._utils._io import _load_holog_file
-
+from astrohack._utils._dio import _load_point_file
+from astrohack._utils._dio import  check_if_file_will_be_overwritten, check_if_file_exists
+from astrohack._utils._dio import _load_holog_file
 from astrohack._utils._extract_holog import _extract_holog_chunk
-
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._parm_utils._check_parms import _check_parms
-
+from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
 from astrohack._utils._tools import _jsonify
+from astrohack._utils._mds import AstrohackHologFile
 
-from astrohack._utils._dio import AstrohackHologFile
 
 def extract_holog(
     ms_name,
     holog_obs_dict=None,
-    ddi_sel=None,
+    ddi=None,
     baseline_average_distance=None,
     baseline_average_nearest=None,
     holog_name=None,
     point_name=None,
     data_column="CORRECTED_DATA",
     parallel=False,
     reuse_point_zarr=False,
     overwrite=False,
 ):
     """
     Extract holography and optionally pointing data, from measurement set. Creates holography output file.
 
     :param ms_name: Name of input measurement file name.
     :type ms_name: str
-
     :param holog_obs_dict: The *holog_obs_dict* describes which scan and antenna data to extract from the measurement set. As detailed below, this compound dictionary also includes important meta data needed for preprocessing and extraction of the holography data from the measurement set. If not specified holog_obs_dict will be generated. For auto generation of the holog_obs_dict the assumtion is made that the same antanna beam is not mapped twice in a row (alternating sets of antennas is fine).
     :type holog_obs_dict: dict, optional
-    
-    :param ddi_sel:  Value(s) of DDI that should be extracted from the measurement set. Defaults to all DDI's in the ms.
-    :type ddi_sel: int numpy.ndarray | int list, optional
-       
+    :param ddi:  DDI(s) that should be extracted from the measurement set. Defaults to all DDI's in the ms.
+    :type ddi: int numpy.ndarray | int list, optional
     :param baseline_average_distance: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_distance is the acceptable distance between a mapping antenna and a reference antenna. The baseline_average_distance is only used if the holog_obs_dict is not specified. If no distance is specified all reference antennas will be used. baseline_average_distance and baseline_average_nearest can not be used together.
     :type holog_obs_dict: float, optional
-    
     :param baseline_average_nearest: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_nearest is the number of nearest reference antennas to use. The baseline_average_nearest is only used if the holog_obs_dict is not specified.  baseline_average_distance and baseline_average_nearest can not be used together.
     :type holog_obs_dict: int, optional
-
     :param holog_name: Name of *<holog_name>.holog.zarr* file to create. Defaults to measurement set name with *holog.zarr* extension.
     :type holog_name: str, optional
-
     :param point_name: Name of *<point_name>.point.zarr* file to create. Defaults to measurement set name with *point.zarr* extension.
     :type point_name: str, optional
-
-    :param data_column: Determines the data column to pull from the measurement set. Defaults to "CORRECTED_DATA"
+    :param data_column: Determines the data column to pull from the measurement set. Defaults to "CORRECTED_DATA".
     :type data_column: str, optional, ex. DATA, CORRECTED_DATA
-
     :param parallel: Boolean for whether to process in parallel. Defaults to False
     :type parallel: bool, optional
-    
     :param reuse_point_zarr: If true the point.zarr specified in point_name is reused.
     :type reuse_point_zarr: bool, optional
-
-    :param test_mode: Boolean for whether to writeholog dictionary to disk. This is solely for testing., defaults to False
-    :type overwrite: bool, optional
-
     :param overwrite: Boolean for whether to overwrite current holog.zarr and point.zarr files., defaults to False
     :type overwrite: bool, optional
 
     :return: Holography holog object.
     :rtype: AstrohackHologFile
 
     .. _Description:
@@ -150,42 +125,46 @@
                     }
                 }
             }
 
     """
     logger = _get_astrohack_logger()
     
-    
+    fname = 'extract_holog'
     ######### Parameter Checking #########
-    extract_holog_parms = _check_extract_holog_parms(ms_name,
-                                holog_obs_dict,
-                                ddi_sel,
-                                baseline_average_distance,
-                                baseline_average_nearest,
-                                holog_name,
-                                point_name,
-                                data_column,
-                                parallel,
-                                reuse_point_zarr,
-                                overwrite)
+    extract_holog_parms = _check_extract_holog_parms(fname,
+                                                     ms_name,
+                                                     holog_obs_dict,
+                                                     ddi,
+                                                     baseline_average_distance,
+                                                     baseline_average_nearest,
+                                                     holog_name,
+                                                     point_name,
+                                                     data_column,
+                                                     parallel,
+                                                     reuse_point_zarr,
+                                                     overwrite)
     input_params = extract_holog_parms.copy()
     
-    check_if_file_exists(extract_holog_parms['ms_name'])
-    check_if_file_will_be_overwritten(extract_holog_parms['holog_name'],extract_holog_parms['overwrite'])
-    check_if_file_will_be_overwritten(extract_holog_parms['point_name'],extract_holog_parms['overwrite'])
+    check_if_file_exists(fname, extract_holog_parms['ms_name'])
+    check_if_file_will_be_overwritten(fname, extract_holog_parms['holog_name'], extract_holog_parms['overwrite'])
+    check_if_file_will_be_overwritten(fname, extract_holog_parms['point_name'], extract_holog_parms['overwrite'])
         
     ############# Exstract pointing infromation and save to point.zarr #############
     if extract_holog_parms["reuse_point_zarr"]:
         try:
             pnt_dict = _load_point_file(extract_holog_parms['point_name'])
         except:
-            logger.warning('Could not find ' + extract_holog_parms['point_name'] + ', creating point new point.zarr .')
-            pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
+            logger.warning(f'[{fname}]: Could not find {extract_holog_parms["point_name"]}, creating point new '
+                           f'point.zarr.')
+            pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'],
+                                         parallel=extract_holog_parms['parallel'])
     else:
-        pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
+        pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'],
+                                     parallel=extract_holog_parms['parallel'])
 
     ######## Get Spectral Windows ########
     ctb = ctables.table(
         os.path.join(extract_holog_parms['ms_name'], "DATA_DESCRIPTION"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
@@ -205,15 +184,14 @@
 
     ant_names = np.array(ctb.getcol("NAME"))
     ant_id = np.arange(len(ant_names))
     ant_pos = ctb.getcol("POSITION")
 
     ctb.close()
     
-    
     ######## Get Antenna IDs that are in the main table########
     ctb = ctables.table(
         extract_holog_parms['ms_name'],
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
@@ -222,41 +200,42 @@
     ant2 = np.unique(ctb.getcol("ANTENNA2"))
     ant_id_main = np.unique(np.append(ant1,ant2))
     
     ant_names_main = ant_names[ant_id_main]
     ctb.close()
     
     # Create holog_obs_dict or modify user supplied holog_obs_dict.
-    ddi_sel = extract_holog_parms['ddi_sel']
+    ddi = extract_holog_parms['ddi_sel']
     if holog_obs_dict is None: #Automatically create holog_obs_dict
         from astrohack._utils._extract_holog import _create_holog_obs_dict
-        holog_obs_dict = _create_holog_obs_dict(pnt_dict, extract_holog_parms['baseline_average_distance'], extract_holog_parms['baseline_average_nearest'], ant_names,ant_pos,ant_names_main)
+        holog_obs_dict = _create_holog_obs_dict(pnt_dict, extract_holog_parms['baseline_average_distance'],
+                                                extract_holog_parms['baseline_average_nearest'], ant_names, ant_pos,
+                                                ant_names_main)
         
         #From the generated holog_obs_dict subselect user supplied ddis.
-        if ddi_sel != 'all':
+        if ddi != 'all':
             holog_obs_dict_keys = list(holog_obs_dict.keys())
             for ddi_key in holog_obs_dict_keys:
                 if 'ddi' in ddi_key:
                     ddi_id = int(ddi_key.replace('ddi_',''))
-                    if ddi_id not in ddi_sel:
+                    if ddi_id not in ddi:
                         del holog_obs_dict[ddi_key]
     else:
         #If a user defines a holog_obs_dict it needs to be duplicated for each ddi.
         holog_obs_dict_with_ddi = {}
-        if ddi_sel == 'all':
+        if ddi == 'all':
             for ddi_id in ms_ddi:
                 holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
         else:
-            for ddi_id in ddi_sel:
+            for ddi_id in ddi:
                 holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
         
         holog_obs_dict = holog_obs_dict_with_ddi
             
-    from pprint import pformat
-    logger.info("holog_obs_dict: \n%s", pformat(list(holog_obs_dict.values())[0],indent=2,width=2))
+    logger.info(f"[{fname}]: holog_obs_dict: \n%s", pformat(list(holog_obs_dict.values())[0], indent=2, width=2))
 
 
     outfile_obj = copy.deepcopy(holog_obs_dict)
 
     _jsonify(outfile_obj)
 
     with open(".holog_obs_dict.json", "w") as outfile:
@@ -320,66 +299,61 @@
         his_ctb = ctables.table(
             os.path.join(extract_holog_parms['ms_name'], "HISTORY"),
             readonly=True,
             lockoptions={"option": "usernoread"},
             ack=False,
         )
     
-        assert ("pnt_tbl:fixed" in his_ctb.getcol("MESSAGE")), "Pointing table not corrected, users should apply function astrohack.dio.fix_pointing_table() to remedy this."
+        assert ("pnt_tbl:fixed" in his_ctb.getcol("MESSAGE")), \
+            "Pointing table not corrected, users should apply function astrohack.dio.fix_pointing_table() to " \
+            "remedy this."
         
         his_ctb.close()
 
-
+    count = 0
     delayed_list = []
-    
     for ddi_name in holog_obs_dict.keys():
         ddi = int(ddi_name.replace('ddi_',''))
         spw_setup_id = ddi_spw[ddi]
         pol_setup_id = ddpol_indexol[ddi]
         
         extract_holog_parms["ddi"] = ddi
         extract_holog_parms["chan_setup"] = {}
         extract_holog_parms["pol_setup"] = {}
-        
         extract_holog_parms["chan_setup"]["chan_freq"] = spw_ctb.getcol("CHAN_FREQ", startrow=spw_setup_id, nrow=1)[0, :]
         extract_holog_parms["chan_setup"]["chan_width"] = spw_ctb.getcol("CHAN_WIDTH", startrow=spw_setup_id, nrow=1)[0, :]
         extract_holog_parms["chan_setup"]["eff_bw"] = spw_ctb.getcol("EFFECTIVE_BW", startrow=spw_setup_id, nrow=1)[0, :]
         extract_holog_parms["chan_setup"]["ref_freq"] = spw_ctb.getcol("REF_FREQUENCY", startrow=spw_setup_id, nrow=1)[0]
         extract_holog_parms["chan_setup"]["total_bw"] = spw_ctb.getcol("TOTAL_BANDWIDTH", startrow=spw_setup_id, nrow=1)[0]
-
         extract_holog_parms["pol_setup"]["pol"] = pol_str[pol_ctb.getcol("CORR_TYPE", startrow=pol_setup_id, nrow=1)[0, :]]
-                
         
         extract_holog_parms["telescope_name"] = obs_ctb.getcol("TELESCOPE_NAME")[0]
-        
 
         for holog_map_key in holog_obs_dict[ddi_name].keys(): #loop over all beam_scan_ids, a beam_scan_id can conist out of more than one scan in an ms (this is the case for the VLA pointed mosiacs).
 
             if 'map' in holog_map_key:
                 scans = holog_obs_dict[ddi_name][holog_map_key]["scans"]
-                logger.info("Processing ddi: {ddi}, scans: {scans}".format(ddi=ddi, scans=scans))
+                logger.info(f"[{fname}]: Processing ddi: {ddi}, scans: {scans}")
                 
                 if len(list(holog_obs_dict[ddi_name][holog_map_key]['ant'].keys())) != 0:
                     map_ant_list = []
-                    ref_ant_per_map_ant_list = [] #
+                    ref_ant_per_map_ant_list = []
                     
                     map_ant_name_list = []
-                    ref_ant_per_map_ant_name_list = [] #
+                    ref_ant_per_map_ant_name_list = []
                     for map_ant_str in holog_obs_dict[ddi_name][holog_map_key]['ant'].keys():
                         ref_ant_ids = np.array(_convert_ant_name_to_id(ant_names,list(holog_obs_dict[ddi_name][holog_map_key]['ant'][map_ant_str])))
                         
                         map_ant_id = _convert_ant_name_to_id(ant_names,map_ant_str)[0]
 
                         ref_ant_per_map_ant_list.append(ref_ant_ids)
                         map_ant_list.append(map_ant_id)
                         
                         ref_ant_per_map_ant_name_list.append(list(holog_obs_dict[ddi_name][holog_map_key]['ant'][map_ant_str]))
                         map_ant_name_list.append(map_ant_str)
-                        
-                   
 
                     extract_holog_parms["ref_ant_per_map_ant_tuple"] = tuple(ref_ant_per_map_ant_list)
                     extract_holog_parms["map_ant_tuple"] = tuple(map_ant_list)
                     
                     extract_holog_parms["ref_ant_per_map_ant_name_tuple"] = tuple(ref_ant_per_map_ant_name_list)
                     extract_holog_parms["map_ant_name_tuple"] = tuple(map_ant_name_list)
                     
@@ -392,102 +366,100 @@
                         delayed_list.append(
                             dask.delayed(_extract_holog_chunk)(
                                 dask.delayed(extract_holog_parms)
                             )
                         )
                     else:
                         _extract_holog_chunk(extract_holog_parms)
+                    count += 1
                 else:
-                    logger.warning('DDI ' + str(ddi) + ' has no holography data to extract.')
-                     
-     
-    
+                    logger.warning(f'[{fname}]: DDI ' + str(ddi) + ' has no holography data to extract.')
 
     spw_ctb.close()
     pol_ctb.close()
     obs_ctb.close()
 
     if parallel:
         dask.compute(delayed_list)    
 
-    holog_dict = _load_holog_file(holog_file=extract_holog_parms["holog_name"], dask_load=True, load_pnt_dict=False)
-
-    extract_holog_parms['telescope_name'] = telescope_name
-    _create_holog_meta_data(holog_file=extract_holog_parms['holog_name'], holog_dict=holog_dict,
-                            input_params=input_params)
-    
-    holog_mds = AstrohackHologFile(extract_holog_parms['holog_name'])
-    holog_mds.open()
-    
-    return holog_mds
+    if count > 0:
+        logger.info(f"[{fname}]: Finished processing")
+        holog_dict = _load_holog_file(holog_file=extract_holog_parms["holog_name"], dask_load=True, load_pnt_dict=False)
+        extract_holog_parms['telescope_name'] = telescope_name
+        _create_holog_meta_data(holog_file=extract_holog_parms['holog_name'], holog_dict=holog_dict,
+                                input_params=input_params)
+        holog_mds = AstrohackHologFile(extract_holog_parms['holog_name'])
+        holog_mds._open()
+        return holog_mds
+    else:
+        logger.warning(f"[{fname}]: No data to process")
+        return None
 
+    holog_mds._open()
 
+    return holog_mds
 
-def _check_extract_holog_parms(
-    ms_name,
-    holog_obs_dict,
-    ddi_sel,
-    baseline_average_distance,
-    baseline_average_nearest,
-    holog_name,
-    point_name,
-    data_column,
-    parallel,
-    reuse_point_zarr,
-    overwrite):
-    
-    extract_holog_parms = {}
-    extract_holog_parms["ms_name"] = ms_name
-    extract_holog_parms["holog_name"] = holog_name
-    extract_holog_parms["ddi_sel"] = ddi_sel
-    extract_holog_parms["point_name"] = point_name
-    extract_holog_parms["data_column"] = data_column
-    extract_holog_parms["parallel"] = parallel
-    extract_holog_parms["overwrite"] = overwrite
-    extract_holog_parms["reuse_point_zarr"] = reuse_point_zarr
-    extract_holog_parms["baseline_average_distance"] = baseline_average_distance
-    extract_holog_parms["baseline_average_nearest"] = baseline_average_nearest
+def _check_extract_holog_parms(fname,
+                               ms_name,
+                               holog_obs_dict,
+                               ddi_sel,
+                               baseline_average_distance,
+                               baseline_average_nearest,
+                               holog_name,
+                               point_name,
+                               data_column,
+                               parallel,
+                               reuse_point_zarr,
+                               overwrite):
+
+    extract_holog_parms = {"ms_name": ms_name, "holog_name": holog_name, "ddi_sel": ddi_sel, "point_name": point_name,
+                           "data_column": data_column, "parallel": parallel, "overwrite": overwrite,
+                           "reuse_point_zarr": reuse_point_zarr, "baseline_average_distance": baseline_average_distance,
+                           "baseline_average_nearest": baseline_average_nearest}
 
-    
     #### Parameter Checking ####
     logger = _get_astrohack_logger()
     parms_passed = True
     
-    parms_passed = parms_passed and _check_parms(extract_holog_parms, 'ms_name', [str],default=None)
+    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'ms_name', [str], default=None)
 
-    base_name = _remove_suffix(ms_name,'.ms')
-    parms_passed = parms_passed and _check_parms(extract_holog_parms,'holog_name', [str],default=base_name+'.holog.zarr')
-  
-    
-    point_base_name = _remove_suffix(extract_holog_parms['holog_name'],'.holog.zarr')
-    parms_passed = parms_passed and _check_parms(extract_holog_parms,'point_name', [str],default=point_base_name+'.point.zarr')
+    base_name = _remove_suffix(ms_name, '.ms')
+    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms,'holog_name', [str],
+                                                 default=base_name+'.holog.zarr')
+
+    point_base_name = _remove_suffix(extract_holog_parms['holog_name'], '.holog.zarr')
+    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'point_name', [str],
+                                                 default=point_base_name+'.point.zarr')
     
-    parms_passed = parms_passed and _check_parms(extract_holog_parms,'ddi_sel', [list,np.ndarray], list_acceptable_data_types=[int], default='all')
+    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'ddi_sel', [list, int],
+                                                 list_acceptable_data_types=[int], default='all')
   
     #To Do: special function needed to check holog_obs_dict.
     parm_check = isinstance(holog_obs_dict,dict) or (holog_obs_dict is None)
     parms_passed = parms_passed and parm_check
     if not parm_check:
-        logger.error('Parameter holog_obs_dict must be of type '+ str(dict))
+        logger.error(f'[{fname}]: Parameter holog_obs_dict must be of type {str(dict)}.')
         
-    parms_passed = parms_passed and _check_parms(extract_holog_parms,'baseline_average_distance',[numbers.Number],default='all')
+    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'baseline_average_distance',
+                                                 [numbers.Number], default='all')
     
-    parms_passed = parms_passed and _check_parms(extract_holog_parms,'baseline_average_nearest',[int], default='all')
+    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'baseline_average_nearest', [int],
+                                                 default='all')
     
-    if (extract_holog_parms['baseline_average_distance'] != 'all') and (extract_holog_parms['baseline_average_nearest'] != 'all'):
-        logger.error('baseline_average_distance: ' + str(baseline_average_distance ) + ' and baseline_average_nearest: ' + str(baseline_average_distance ) + ' can not both be specified.')
+    if (extract_holog_parms['baseline_average_distance'] != 'all') and \
+            (extract_holog_parms['baseline_average_nearest'] != 'all'):
+        logger.error(f'[{fname}]: baseline_average_distance: {str(baseline_average_distance)} and '
+                     f'baseline_average_nearest: {str(baseline_average_distance)} can not both be specified.')
         parms_passed = False
  
-    parms_passed = parms_passed and _check_parms(extract_holog_parms,'data_column', [str],default='CORRECTED_DATA')
+    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'data_column', [str],
+                                                 default='CORRECTED_DATA')
 
-    parms_passed = parms_passed and _check_parms(extract_holog_parms, 'parallel', [bool],default=False)
+    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'parallel', [bool], default=False)
     
-    parms_passed = parms_passed and _check_parms(extract_holog_parms, 'reuse_point_zarr', [bool],default=False)
+    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'reuse_point_zarr', [bool], default=False)
 
-    parms_passed = parms_passed and _check_parms(extract_holog_parms, 'overwrite', [bool],default=False)
+    parms_passed = parms_passed and _check_parms(fname, extract_holog_parms, 'overwrite', [bool],default=False)
+
+    _parm_check_passed(fname, parms_passed)
 
-    if not parms_passed:
-        logger.error("extract_holog parameter checking failed.")
-        raise Exception("extract_holog parameter checking failed.")
-    
-    
     return extract_holog_parms
```

### Comparing `astrohack-0.1.4/src/astrohack/gdown_utils.py` & `astrohack-0.1.5/src/astrohack/gdown_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 import shutil
 import json
 
 from prettytable import PrettyTable
 from prettytable import DOUBLE_BORDER
 
 gdown_ids = {
-    'ea25_cal_small_spw1_4_60_ea04_before.ms': '1-v1foZ4G-kHTOS2idylx-3S4snKgRHmM',
-    'ea25_cal_small_spw1_4_60_ea04_after.ms': '1PmWvPA0rUtAfegVu9wOb4AGJXiQIp3Cp',
-    'ea25_cal_small_spw1_4_60_ea04_before_fixed.ms': '1dV4e8FiVRdAw2NLNzSuPVvjwyqXPNXTf',
-    'ea25_cal_small_spw1_4_60_ea04_after_fixed.ms': '1Gn5GEJ3V43bl2vXxznHk6oXF5LtWOMzj',
     'ea25_cal_small_before_fixed.split.ms':'1oydlR7kA7F4n0i9KF9HgRc2jq1ziUslt',
-    'ea25_cal_small_after_fixed.split.ms':'1TATMxKTFYIEO-l9L3jdYj62lZ8TZex4T'
+    'ea25_cal_small_after_fixed.split.ms':'1TATMxKTFYIEO-l9L3jdYj62lZ8TZex4T',
+    'J1924-2914.ms.calibrated.split.SPW3': '1OSDjWM1IskPOlC0w1wVBqsTp8JAbNGzL',
+    'extract_holog_verification.json':'1Wd79KCl-wxlUwBRxYFUnofG8mN0Xfzga',
+    'holog_numerical_verification.json':'16kl_DMHWVb0TwxuHq1dRr1TbIor_IU-a'
 }
 
 def check_download(name, folder, id):
     fullname = os.path.join(folder,name)
     if not os.path.exists(fullname):
         url = 'https://drive.google.com/u/0/uc?id='+id+'&export=download'
         gdown.download(url, fullname+'.zip')
@@ -26,14 +25,30 @@
     if not os.path.exists(path):
         os.makedirs(path)
         
 def build_folder_structure(dataname, resultname):
     create_folder(dataname)
     create_folder(resultname)
 
+def download(file, folder='.', unpack=False):
+    assert file in gdown_ids, "File not available. Available files are:" + str(gdown_ids.keys())
+    
+    id = gdown_ids[file]
+    create_folder(folder)
+
+    if unpack: file = file+'.zip'
+        
+    fullname = os.path.join(folder, file)
+
+    if not os.path.exists(fullname):
+        url = 'https://drive.google.com/u/0/uc?id=' + id + '&export=download'
+        gdown.download(url, fullname)
+
+    if unpack: shutil.unpack_archive(filename=fullname, extract_dir=folder)
+
 def gdown_data(ms_name, download_folder='.'):
     assert ms_name in gdown_ids, "Measurement set not available. Available measurement sets are:" + str(gdown_ids.keys())
     
     id = gdown_ids[ms_name]
     create_folder(download_folder)
     check_download(ms_name, download_folder, id)
```

### Comparing `astrohack-0.1.4/src/astrohack/holog.py` & `astrohack-0.1.5/src/astrohack/holog.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,53 @@
 import json
-import os
-
-import dask
-import dask.distributed
 import numpy as np
 import numbers
 
 from astrohack._utils._holog import _holog_chunk, _create_image_meta_data
-
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._parm_utils._check_parms import _check_parms
+from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
-   
-from astrohack._utils._io import check_if_file_will_be_overwritten, check_if_file_exists, _read_meta_data
-from astrohack._utils._dio import AstrohackImageFile
-
-def holog(
-    holog_name,
-    grid_size=None,
-    cell_size=None,
-    image_name=None,
-    padding_factor=50,
-    grid_interpolation_mode="linear",
-    chan_average=True,
-    chan_tolerance_factor=0.005,
-    scan_average=True,
-    ant_list=None,
-    to_stokes=True,
-    apply_mask=True,
-    phase_fit=True,
-    overwrite=False,
-    parallel=True, 
-    ):
+from astrohack._utils._dio import check_if_file_will_be_overwritten, check_if_file_exists, _read_meta_data
+from astrohack._utils._mds import AstrohackImageFile
+from astrohack._utils._dask_graph_tools import _dask_general_compute
+
+
+def holog(holog_name, grid_size=None, cell_size=None, image_name=None, padding_factor=50,
+          grid_interpolation_mode="linear", chan_average=True, chan_tolerance_factor=0.005, scan_average=True,
+          ant_id=None, ddi=None, to_stokes=True, apply_mask=True, phase_fit=True, overwrite=False, parallel=False):
     """ Process holography data and derive aperture illumination pattern.
 
     :param holog_name: Name of holography .holog.zarr file to process.
     :type holog_name: str
-
     :param grid_size: Numpy array specifying the dimensions of the grid used in data gridding. If not specified grid_size is calculated using POINTING_OFFSET in pointing table.
     :type grid_size: numpy.ndarray, dtype int, optional
-
     :param cell_size: Numpy array defining the cell size of each grid bin. If not specified cell_size is calculated using POINTING_OFFSET in pointing table.
     :type cell_size: numpy.ndarray, dtype float, optional
-
     :param image_name: Defines the name of the output image name. If value is None, the name will be set to <base_name>.image.zarr, defaults to None
     :type image_name: str, optional
-
     :param padding_factor: Padding factor applied to beam grid before computing the fast-fourier transform. The default has been set for operation on most systems. The user should be aware of memory constraints before increasing this parameter significatly., defaults to 50
     :type padding_factor: int, optional
-
-    :param parallel: Run in parallel with Dask or in serial., defaults to True
+    :param parallel: Run in parallel with Dask or in serial., defaults to False
     :type parallel: bool, optional
-
     :param grid_interpolation_mode: Method of interpolation used when gridding data. This is done using the `scipy.interpolate.griddata` method. For more information on the interpolation see `scipy.interploate <https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.griddata.html#scipy.interpolate.griddata>`_, defaults to "linear"
-    :type grid_interpolation_mode: str, optional. Available options: {"linear", "nearest", "cubic"} 
-
+    :type grid_interpolation_mode: str, optional. Available options: {"linear", "nearest", "cubic"}
     :param chan_average: Boolean dictating whether the channel average is computed and written to the output holog file., defaults to True
     :type chan_average: bool, optional
-
     :param chan_tolerance_factor: Tolerance used in channel averaging to determine the number of primary beam channels., defaults to 0.005
     :type chan_tolerance_factor: float, optional
-
     :param scan_average: Boolean dicating whether averagin is done over scan., defaults to True
     :type scan_average: bool, optional
-
-    :param ant_list: Optional list of sub-antennas to use when the user doesn't to do holography for all antennas, defaults to all antennas.
-    :type ant_list: list, optional
-
+    :param ant_id: List of antennae/antenna to be processed, defaults to "all" when None, ex. ea25
+    :type ant_id: list or str, optional
+    :param ddi: List of ddis/ddi to be processed, defaults to "all" when None, ex. 0
+    :type ddi: list or int, optional
     :param to_stokes: Dictates whether polarization is computed according to stokes values., defaults to True
     :type to_stokes: bool, optional
-
     :param apply_mask: If True applies a mask to the aperture setting values outside of the aperture to zero., defaults to True
     :type apply_mask: bool, optional
-
     :param phase_fit: If a boolean array is given each element controls one aspect of phase fitting. defaults to True.
         
         Phase fitting:
         
         - [0]: pointing offset; 
         - [1]: focus xy offsets; 
         - [2]: focus z offset; 
@@ -107,158 +78,111 @@
             ⋮
             ant_n: …
         }
 
     """
     
     logger = _get_astrohack_logger()
-    
-    holog_params = _check_holog_parms(
-        holog_name, 
-        grid_size,
-        cell_size, 
-        image_name, 
-        padding_factor, 
-        parallel, 
-        grid_interpolation_mode, 
-        chan_average, 
-        chan_tolerance_factor, 
-        scan_average,
-        ant_list, 
-        to_stokes, 
-        apply_mask, 
-        phase_fit,
-        overwrite
-    )
+    fname = 'holog'
+    holog_params = _check_holog_parms(fname, holog_name, grid_size, cell_size, image_name, padding_factor, parallel,
+                                      grid_interpolation_mode, chan_average, chan_tolerance_factor, scan_average,
+                                      ant_id, ddi, to_stokes, apply_mask, phase_fit, overwrite)
     input_params = holog_params.copy()
     
-    check_if_file_exists(holog_params['holog_file'])
-    check_if_file_will_be_overwritten(holog_params['image_file'],holog_params['overwrite'])
+    check_if_file_exists(fname, holog_params['holog_file'])
+    check_if_file_will_be_overwritten(fname, holog_params['image_file'], holog_params['overwrite'])
 
     json_data = "/".join((holog_params['holog_file'], ".holog_json"))
     with open(json_data, "r") as json_file:
         holog_json = json.load(json_file)
     meta_data = _read_meta_data(holog_params['holog_file'], 'holog', 'extract_holog')
 
-    if  holog_params['ant_list'] == 'all':
-        holog_params['ant_list'] = list(holog_json.keys())
-        
-    logger.info('Mapping antennas ' + str(holog_params['ant_list']))
-
-    if (holog_params["cell_size"] is None):
+    if holog_params["cell_size"] is None:
         cell_size = np.array([-meta_data["cell_size"], meta_data["cell_size"]])
         holog_params["cell_size"] = cell_size
     
-    if  (holog_params["grid_size"] is None):
+    if holog_params["grid_size"] is None:
         n_pix = int(np.sqrt(meta_data["n_pix"]))
         grid_size = np.array([n_pix, n_pix])
         holog_params["grid_size"] = grid_size
-    
-    
-    logger.info("Cell size: " + str(cell_size) + " Grid size " + str(grid_size))
+
+    logger.info(f'[{fname}]: Cell size: {str(cell_size)}, Grid size {str(grid_size)}')
     json_data = {
             "cell_size": holog_params["cell_size"].tolist(),
             "grid_size": holog_params["grid_size"].tolist()
     }
     
-    print(holog_params["grid_size"])
-    
     with open(".holog_diagnostic.json", "w") as out_file:
         json.dump(json_data, out_file)
 
-    
-    holog_chunk_params =  holog_params
-    delayed_list = []
-    
-    
-    for ant_id in holog_chunk_params['ant_list']:
-        for ddi in list(holog_json[ant_id].keys()):
-            logger.info("Processing ant_id: " + str(ant_id)  + " and " + ddi)
-            holog_chunk_params["ant_id"] = ant_id
-            holog_chunk_params["ddi_id"] = ddi
-            
-            if parallel:
-                delayed_list.append(
-                    dask.delayed(_holog_chunk)(dask.delayed(holog_chunk_params))
-                )
-
-            else:
-                _holog_chunk(holog_chunk_params)
-            
-
-    if holog_chunk_params['parallel']:
-        dask.compute(delayed_list)
+    if _dask_general_compute(fname, holog_json, _holog_chunk, holog_params, ['ant', 'ddi'], parallel=parallel):
+        _create_image_meta_data(holog_params['image_file'], input_params)
+        image_mds = AstrohackImageFile(holog_params['image_file'])
+        image_mds._open()
+        logger.info(f'[{fname}]: Finished processing')
+        return image_mds
+    else:
+        logger.warning(f"[{fname}]: No data to process")
+        return None
 
-    _create_image_meta_data(holog_params['image_file'], input_params)
-        
-    image_mds = AstrohackImageFile(holog_chunk_params['image_file'])
-    image_mds.open()
-    
-    return image_mds
 
+def _check_holog_parms(fname, holog_name, grid_size, cell_size, image_name, padding_factor, parallel,
+                       grid_interpolation_mode, chan_average, chan_tolerance_factor, scan_average, ant_id, ddi,
+                       to_stokes, apply_mask, phase_fit, overwrite):
+
+    holog_params = {"holog_file": holog_name, "grid_size": grid_size, "cell_size": cell_size, "image_file": image_name,
+                    "padding_factor": padding_factor, "parallel": parallel,
+                    "grid_interpolation_mode": grid_interpolation_mode, "chan_average": chan_average, "ddi": ddi,
+                    "chan_tolerance_factor": chan_tolerance_factor, "scan_average": scan_average, "ant": ant_id,
+                    "to_stokes": to_stokes, "apply_mask": apply_mask, "phase_fit": phase_fit, "overwrite": overwrite}
 
-def _check_holog_parms(holog_name,grid_size,cell_size,image_name,
-                      padding_factor,parallel,grid_interpolation_mode,
-                      chan_average,chan_tolerance_factor,
-                      scan_average,ant_list,to_stokes,apply_mask,phase_fit,overwrite):
-
-    holog_params = {}
-    holog_params["holog_file"] = holog_name
-    holog_params["grid_size"] = grid_size
-    holog_params["cell_size"] = cell_size
-    holog_params["image_file"] = image_name
-    holog_params["padding_factor"] = padding_factor
-    holog_params["parallel"] = parallel
-    holog_params["grid_interpolation_mode"] = grid_interpolation_mode
-    holog_params["chan_average"] = chan_average
-    holog_params["chan_tolerance_factor"] = chan_tolerance_factor
-    holog_params["scan_average"] = scan_average
-    holog_params["ant_list"] = ant_list
-    holog_params["to_stokes"] = to_stokes
-    holog_params["apply_mask"] = apply_mask
-    holog_params["phase_fit"] = phase_fit
-    holog_params["overwrite"] = overwrite
-    
     #### Parameter Checking ####
-    logger = _get_astrohack_logger()
     parms_passed = True
     
-    parms_passed = parms_passed and _check_parms(holog_params, 'holog_file', [str],default=None)
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'holog_file', [str], default=None)
 
-    parms_passed = parms_passed and _check_parms(holog_params, 'grid_size', [list, np.ndarray], list_acceptable_data_types=[np.int64, int], list_len=2, default='None',log_default_setting=False)
-    if (isinstance(holog_params['grid_size'],str)) and (holog_params['grid_size'] == 'None'):
-        holog_params['grid_size'] =  None
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'grid_size', [list, np.ndarray],
+                                                 list_acceptable_data_types=[np.int64, int], list_len=2, default='None',
+                                                 log_default_setting=False)
+    if (isinstance(holog_params['grid_size'], str)) and (holog_params['grid_size'] == 'None'):
+        holog_params['grid_size'] = None
     else:
         holog_params['grid_size'] = np.array(holog_params['grid_size'])
 
-    parms_passed = parms_passed and _check_parms(holog_params, 'cell_size', [list,np.ndarray], list_acceptable_data_types=[numbers.Number], list_len=2, default='None',log_default_setting=False)
-    if (isinstance(holog_params['cell_size'],str)) and (holog_params['cell_size'] == 'None'):
-        holog_params['cell_size'] =  None
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'cell_size', [list, np.ndarray],
+                                                 list_acceptable_data_types=[numbers.Number], list_len=2,
+                                                 default='None', log_default_setting=False)
+    if (isinstance(holog_params['cell_size'], str)) and (holog_params['cell_size'] == 'None'):
+        holog_params['cell_size'] = None
     else:
         holog_params['cell_size'] = np.array(holog_params['cell_size'])
 
-    
-    base_name = _remove_suffix(holog_params['holog_file'],'.holog.zarr')
-    parms_passed = parms_passed and _check_parms(holog_params,'image_file', [str],default=base_name+'.image.zarr')
-    parms_passed = parms_passed and _check_parms(holog_params, 'padding_factor', [int], default=50)
-    parms_passed = parms_passed and _check_parms(holog_params, 'parallel', [bool],default=False)
-    parms_passed = parms_passed and _check_parms(holog_params,'grid_interpolation_mode', [str],acceptable_data=["nearest","linear","cubic"],default="nearest")
-    parms_passed = parms_passed and _check_parms(holog_params, 'chan_average', [bool],default=True)
-    parms_passed = parms_passed and _check_parms(holog_params, 'chan_tolerance_factor', [float], acceptable_range=[0,1], default=0.005)
-    parms_passed = parms_passed and _check_parms(holog_params, 'scan_average', [bool],default=True)
-    parms_passed = parms_passed and _check_parms(holog_params, 'ant_list', [list,np.ndarray], list_acceptable_data_types=[str], default='all')
-    parms_passed = parms_passed and _check_parms(holog_params, 'to_stokes', [bool],default=True)
-
-    if isinstance(holog_params['phase_fit'],list) or isinstance(holog_params['phase_fit'],type(np.ndarray)):
-        parms_passed = parms_passed and _check_parms(holog_params, 'phase_fit', [list,type(np.ndarray)], list_acceptable_data_types=[bool], list_len=5)
+    base_name = _remove_suffix(holog_params['holog_file'], '.holog.zarr')
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'image_file', [str],
+                                                 default=base_name+'.image.zarr')
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'padding_factor', [int], default=50)
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'parallel', [bool], default=False)
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'grid_interpolation_mode', [str],
+                                                 acceptable_data=["nearest", "linear", "cubic"], default="nearest")
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'chan_average', [bool], default=True)
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'chan_tolerance_factor', [float],
+                                                 acceptable_range=[0, 1], default=0.005)
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'scan_average', [bool], default=True)
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'ant', [list, str],
+                                                 list_acceptable_data_types=[str], default='all')
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'ddi', [list, int],
+                                                 list_acceptable_data_types=[int], default='all')
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'to_stokes', [bool], default=True)
+
+    if isinstance(holog_params['phase_fit'], list) or isinstance(holog_params['phase_fit'], type(np.ndarray)):
+        parms_passed = parms_passed and _check_parms(fname, holog_params, 'phase_fit', [list, type(np.ndarray)],
+                                                     list_acceptable_data_types=[bool], list_len=5)
     else:
-        parms_passed = parms_passed and _check_parms(holog_params, 'phase_fit', [bool], default=True)
+        parms_passed = parms_passed and _check_parms(fname, holog_params, 'phase_fit', [bool], default=True)
 
-    parms_passed = parms_passed and _check_parms(holog_params, 'apply_mask', [bool],default=True)
-    parms_passed = parms_passed and _check_parms(holog_params, 'overwrite', [bool],default=False)
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'apply_mask', [bool], default=True)
+    parms_passed = parms_passed and _check_parms(fname, holog_params, 'overwrite', [bool], default=False)
 
-    if not parms_passed:
-        logger.error("extract_holog parameter checking failed.")
-        raise Exception("extract_holog parameter checking failed.")
+    _parm_check_passed(fname, parms_passed)
 
     return holog_params
```

### Comparing `astrohack-0.1.4/src/astrohack/panel.py` & `astrohack-0.1.5/src/astrohack/panel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 import os
-import dask
 import shutil
 
-import numpy as np
-
 from astrohack._classes.base_panel import panel_models
-from astrohack._utils._io import _aips_holog_to_xds, check_if_file_will_be_overwritten, check_if_file_exists, _write_meta_data
+from astrohack._utils._dio import _aips_holog_to_xds, check_if_file_will_be_overwritten, check_if_file_exists, _write_meta_data
 from astrohack._utils._panel import _panel_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._parm_utils._check_parms import _check_parms
+from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
-from astrohack._utils._dask_graph_tools import _generate_antenna_ddi_graph_and_compute
+from astrohack._utils._dask_graph_tools import _dask_general_compute
 
-from astrohack._utils._dio import AstrohackPanelFile
+from astrohack._utils._mds import AstrohackPanelFile, AstrohackImageFile
 
 
-def panel(image_name, panel_name=None, cutoff=0.2, panel_model=None, panel_margins=0.2, ant_name=None, ddi=None,
+def panel(image_name, panel_name=None, cutoff=0.2, panel_model=None, panel_margins=0.2, ant_id=None, ddi=None,
           parallel=False, overwrite=False):
     """Analyze holography images to derive panel adjustments
 
     :param image_name: Input holography data file name. Accepted data formats are the output from ``astrohack.holog.holog`` and AIPS holography data prepackaged using ``astrohack.panel.aips_holog_to_astrohack``.
     :type image_name: str
     :param panel_name: Name of output file; File name will be appended with suffix *.panel.zarr*. Defaults to *basename* of input file plus holography panel file suffix.
     :type panel_name: str, optional
     :param cutoff: Relative amplitude cut-off which defines fitting mask. Defaults to 0.2.
     :type cutoff: float, optional
     :param panel_model: Model of surface fitting function used to fit panel surfaces, None will default to "rigid". Possible models are listed below.
     :type panel_model: str, optional
     :param panel_margins: Relative margin from the edge of the panel used to decide which points are margin points or internal points of each panel. Defaults to 0.2.
     :type panel_margins: float, optional
+    :param ant_id: List of antennae/antenna to be processed, defaults to "all" when None, ex. ea25
+    :type ant_id: list or str, optional
+    :param ddi: List of ddis/ddi to be processed, defaults to "all" when None, ex. 0
+    :type ddi: list or int, optional
     :param parallel: Run in parallel. Defaults to False.
     :type parallel: bool, optional
-    :param ant_name: List of antennae to be processed. None will use all antennae. Defaults to None.
-    :type ant_name: list, optional, ex. [ant_ea25 ... ant_ea06]
-    :param ddi: List of DDIs to be processed. None will use all DDIs. Defaults to None.
-    :type ddi: list, optional, ex. [ddi_0 ... ddi_N]
     :param overwrite: Overwrite files on disk. Defaults to False.
     :type overwrite: bool, optional
 
     :return: Holography panel object.
     :rtype: AstrohackPanelFile
 
     .. _Description:
@@ -89,50 +86,50 @@
             ⋮
             ant_n: …
         }
 
     """
     
     logger = _get_astrohack_logger()
-    
-    panel_params = _check_panel_parms(image_name, panel_name, cutoff, panel_model, panel_margins, ant_name, ddi,
+    fname = 'panel'
+    panel_params = _check_panel_parms(fname, image_name, panel_name, cutoff, panel_model, panel_margins, ant_id, ddi,
                                       parallel, overwrite)
     input_params = panel_params.copy()
     # Doubled this entry for compatibility with the factorized antenna ddi loop
     panel_params['filename'] = panel_params['image_name']
-    check_if_file_exists(panel_params['image_name'])
-    check_if_file_will_be_overwritten(panel_params['panel_name'], panel_params['overwrite'])
+    check_if_file_exists(fname, panel_params['image_name'])
+    image_mds = AstrohackImageFile(panel_params['image_name'])
+    image_mds._open()
+    check_if_file_will_be_overwritten(fname, panel_params['panel_name'], panel_params['overwrite'])
 
     if os.path.exists(panel_params['image_name']+'/.aips'):
         panel_params['origin'] = 'AIPS'
         _panel_chunk(panel_params)
 
     else:
         panel_params['origin'] = 'astrohack'
-        count = _generate_antenna_ddi_graph_and_compute('panel', _panel_chunk, panel_params, parallel)
-        if count == 0:
-            logger.warning("No data to process")
-            return None
-        else:
-            logger.info("[panel] Finished processing")
-
+        if _dask_general_compute(fname, image_mds, _panel_chunk, panel_params, ['ant', 'ddi'], parallel=parallel):
+            logger.info(f"[{fname}]: Finished processing")
             output_attr_file = "{name}/{ext}".format(name=panel_params['panel_name'], ext=".panel_attr")
             _write_meta_data('panel', output_attr_file, input_params)
             panel_mds = AstrohackPanelFile(panel_params['panel_name'])
-            panel_mds.open()
+            panel_mds._open()
             return panel_mds
+        else:
+            logger.warning(f"[{fname}]: No data to process")
+            return None
 
 
 def aips_holog_to_astrohack(amp_image, dev_image, telescope_name, holog_name, overwrite=False):
     """
     Package AIPS HOLOG products in a .image.zarr file compatible with astrohack.panel.panel
 
     This function reads amplitude and deviation FITS files produced by AIPS's HOLOG task and transfers their data onto a
     .image.zarr file that can be read by panel.
-    Most of the meta data can be inferred from the FITS headers, but it remains necessary to specify the telescope name
+    Most of the metadata can be inferred from the FITS headers, but it remains necessary to specify the telescope name
     to be included on the .image.zarr file
 
     Args:
         amp_image: Full path to amplitude image
         dev_image: Full path to deviation image
         telescope_name: Telescope name to be added to the .zarr file
         holog_name: Name of the output .zarr file
@@ -147,60 +144,61 @@
     if os.path.exists(holog_name):
         shutil.rmtree(holog_name, ignore_errors=False, onerror=None)
     xds.to_zarr(holog_name, mode='w', compute=True, consolidated=True)
     aips_mark = open(holog_name+'/.aips', 'w')
     aips_mark.close()
 
 
-def _check_panel_parms(image_name, panel_name, cutoff, panel_kind, panel_margins, ant_name, ddi, parallel, overwrite):
+def _check_panel_parms(fname, image_name, panel_name, cutoff, panel_kind, panel_margins, ant_id, ddi, parallel,
+                       overwrite):
     """
     Tests inputs to panel function
     Args:
+        fname: Caller's name
         image_name: Input holography data, can be from astrohack.holog, but also preprocessed AIPS data
         panel_name: Name for the output directory structure containing the products
 
         cutoff: Cut off in amplitude for the physical deviation fitting, None means 20%
         panel_kind: Type of fitting function used to fit panel surfaces, defaults to corotated_paraboloid for ringed
                     telescopes
-        ant_name: Which Antennae are to be processed by panel, None means all of them
+        ant_id: Which Antennae are to be processed by panel, None means all of them
         ddi: Which DDIs are to be processed by panel, None means all of them
         parallel: Run chunks of processing in parallel
         panel_margins: Margin to be ignored at edges of panels when fitting
 
         overwrite: Overwrite previous hack_file of same name?
     """
 
     panel_params = {'image_name': image_name,
                     'panel_name': panel_name,
                     'cutoff': cutoff,
                     'panel_kind': panel_kind,
                     'panel_margins': panel_margins,
                     'parallel': parallel,
                     'ddi': ddi,
-                    'ant_name': ant_name,
+                    'ant': ant_id,
                     'overwrite': overwrite
                     }
                           
     #### Parameter Checking ####
-    logger = _get_astrohack_logger()
-    parms_passed = True
-    
-    parms_passed = parms_passed and _check_parms(panel_params, 'image_name', [str], default=None)
+
+    parms_passed = _check_parms(fname, panel_params, 'image_name', [str], default=None)
     base_name = _remove_suffix(panel_params['image_name'], '.image.zarr')
     base_name = _remove_suffix(base_name, '.combine.zarr')
-    parms_passed = parms_passed and _check_parms(panel_params, 'panel_name', [str], default=base_name+'.panel.zarr')
-    parms_passed = parms_passed and _check_parms(panel_params, 'ant_name', [list], list_acceptable_data_types=[str],
-                                                 default='all')
-    parms_passed = parms_passed and _check_parms(panel_params, 'ddi', [list], list_acceptable_data_types=[str],
-                                                 default='all')
-    parms_passed = parms_passed and _check_parms(panel_params, 'cutoff', [float], acceptable_range=[0, 1], default=0.2)
-    parms_passed = parms_passed and _check_parms(panel_params, 'panel_kind', [str], acceptable_data=panel_models, default="rigid")
-    parms_passed = parms_passed and _check_parms(panel_params, 'panel_margins', [float], acceptable_range=[0, 0.5], default=0.2)
-    parms_passed = parms_passed and _check_parms(panel_params, 'parallel', [bool], default=False)
-    parms_passed = parms_passed and _check_parms(panel_params, 'overwrite', [bool], default=False)
+    parms_passed = parms_passed and _check_parms(fname, panel_params, 'panel_name', [str],
+                                                 default=base_name+'.panel.zarr')
+    parms_passed = parms_passed and _check_parms(fname, panel_params, 'ant', [list, str],
+                                                 list_acceptable_data_types=[str], default='all')
+    parms_passed = parms_passed and _check_parms(fname, panel_params, 'ddi', [list, int],
+                                                 list_acceptable_data_types=[int], default='all')
+    parms_passed = parms_passed and _check_parms(fname, panel_params, 'cutoff', [float], acceptable_range=[0, 1],
+                                                 default=0.2)
+    parms_passed = parms_passed and _check_parms(fname, panel_params, 'panel_kind', [str], acceptable_data=panel_models,
+                                                 default="rigid")
+    parms_passed = parms_passed and _check_parms(fname, panel_params, 'panel_margins', [float],
+                                                 acceptable_range=[0, 0.5], default=0.2)
+    parms_passed = parms_passed and _check_parms(fname, panel_params, 'parallel', [bool], default=False)
+    parms_passed = parms_passed and _check_parms(fname, panel_params, 'overwrite', [bool], default=False)
 
+    _parm_check_passed(fname, parms_passed)
 
-    if not parms_passed:
-        logger.error("panel parameter checking failed.")
-        raise Exception("panel parameter checking failed.")
-    
     return panel_params
```

### Comparing `astrohack-0.1.4/src/astrohack/profiling.py` & `astrohack-0.1.5/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/src/astrohack/visualization/viewer.py` & `astrohack-0.1.5/src/astrohack/visualization/viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     type = param.ObjectSelector(label="Type")
 
     
     def __init__(self, data_file, **kwargs):
         super().__init__(**kwargs)
         self.data_dict = data_file
         
-        if self.data_dict.image.is_open() == False:
-            self.data_dict.image.open()
+        if self.data_dict.image._is_open() == False:
+            self.data_dict.image._open()
 
         self.param.antenna.objects = list(self.data_dict.image.keys())
         self.antenna = list(self.data_dict.image.keys())[0]
         
         index = list(self.data_dict.image.keys())[0]
         
         self.param.ddi.objects = list(self.data_dict.image[index].keys())
```

### Comparing `astrohack-0.1.4/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.1.5/src/astrohack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.4
+Version: 0.1.5
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.1.4/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.1.5/src/astrohack.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,36 +25,35 @@
 src/astrohack/_classes/telescope.py
 src/astrohack/_utils/__init__.py
 src/astrohack/_utils/_algorithms.py
 src/astrohack/_utils/_combine.py
 src/astrohack/_utils/_constants.py
 src/astrohack/_utils/_conversion.py
 src/astrohack/_utils/_dask_graph_tools.py
+src/astrohack/_utils/_diagnostics.py
 src/astrohack/_utils/_dio.py
 src/astrohack/_utils/_extract_holog.py
 src/astrohack/_utils/_extract_point.py
 src/astrohack/_utils/_gaussfitter.py
 src/astrohack/_utils/_holog.py
 src/astrohack/_utils/_imaging.py
-src/astrohack/_utils/_io.py
+src/astrohack/_utils/_mds.py
 src/astrohack/_utils/_panel.py
+src/astrohack/_utils/_phase_fitting.py
 src/astrohack/_utils/_tools.py
 src/astrohack/_utils/_dask_plugins/__init__.py
 src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
 src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
 src/astrohack/_utils/_logger/__init__.py
 src/astrohack/_utils/_logger/_astrohack_logger.py
 src/astrohack/_utils/_parm_utils/__init__.py
 src/astrohack/_utils/_parm_utils/_check_logger_parms.py
 src/astrohack/_utils/_parm_utils/_check_parms.py
-src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json
-src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json
+src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
 src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
-src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json
-src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json
 src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
 src/astrohack/data/telescopes/__init__.py
 src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
 src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
 src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
 src/astrohack/data/telescopes/alma_da.zarr/.zattrs
 src/astrohack/data/telescopes/alma_da.zarr/.zgroup
```

### Comparing `astrohack-0.1.4/src/astrohack.egg-info/requires.txt` & `astrohack-0.1.5/src/astrohack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/tests/test_class_antenna_surface.py` & `astrohack-0.1.5/tests/test_class_antenna_surface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from astrohack._classes.antenna_surface import AntennaSurface
 from astrohack._classes.telescope import Telescope
-from astrohack._utils._io import _aips_holog_to_xds
+from astrohack._utils._dio import _aips_holog_to_xds
 from astrohack._utils._conversion import _convert_unit
 
 import numpy as np
 import gdown
 import shutil
 import os
```

### Comparing `astrohack-0.1.4/tests/test_class_base_panel.py` & `astrohack-0.1.5/tests/test_class_base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/tests/test_class_ring_panel.py` & `astrohack-0.1.5/tests/test_class_ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/tests/test_class_telescope.py` & `astrohack-0.1.5/tests/test_class_telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.4/tests/test_stakeholder.py` & `astrohack-0.1.5/tests/test_stakeholder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,68 @@
 import pytest
 
 import shutil
 import os
 import json
 import copy
+import astrohack
 
 import numpy as np
 
 from astrohack.gdown_utils import gdown_data
 
 from astrohack._utils._tools import _jsonify
 
 from astrohack.extract_holog import extract_holog
 from astrohack.holog import holog
 from astrohack.panel import panel
 
+from astrohack.dio import open_panel
+
 from astrohack.astrohack_client import astrohack_local_client
 
 base_name = 'ea25_cal_small_'
 
 client = astrohack_local_client(cores=2, memory_limit='8GB', log_parms={'log_level':'DEBUG'})
 
 @pytest.fixture(scope='session')
 def set_data(tmp_path_factory):
   data_dir = tmp_path_factory.mktemp("data")
-
-  gdown_data(ms_name='ea25_cal_small_before_fixed.split.ms', download_folder=str(data_dir))
-  gdown_data(ms_name='ea25_cal_small_after_fixed.split.ms', download_folder=str(data_dir))
+    
+  # Data files
+  astrohack.gdown_utils.download('ea25_cal_small_before_fixed.split.ms', folder=str(data_dir), unpack=True)
+  astrohack.gdown_utils.download('ea25_cal_small_after_fixed.split.ms', folder=str(data_dir), unpack=True)
+  astrohack.gdown_utils.download('J1924-2914.ms.calibrated.split.SPW3', folder=str(data_dir), unpack=True)
+
+  # Verification json information
+  astrohack.gdown_utils.download(file='extract_holog_verification.json', folder=str(data_dir))
+  astrohack.gdown_utils.download(file='holog_numerical_verification.json', folder=str(data_dir))
 
   return data_dir
 
-from astrohack.dio import open_panel
+def verify_panel_positions(
+    data_dir="",
+    panel_list=['3-11', '5-31', '7-52', '11-62'], 
+    reference_position = np.array([-2.39678052, -0.87024129, 0.89391852, 0.48643069]),
+    antenna='ant_DV13',
+    ddi='ddi_0'
+):
+  def relative_difference(mean, expected):  
+      return 2*np.abs(mean - expected)/(abs(mean) + abs(expected))
+    
+  M_TO_MILS = 39370.1
+    
+  panel_mds = open_panel('{data}/alma.split.panel.zarr'.format(data=data_dir))
+
+    
+  panel_position = np.mean(panel_mds[antenna][ddi].sel(labels=panel_list).PANEL_SCREWS.values*M_TO_MILS, axis=1)
+
+  relative_position = relative_difference(panel_position, reference_position)
+    
+  return np.any(relative_position < 1e-6)
 
 def verify_panel_shifts(
   data_dir="",
   panel_list=['3-4', '5-27', '5-37', '5-38'], 
   expected_shift=np.array([-100, 75, 0, 150]),
   ref_mean_shift = np.array([-112.17789033, 73.22619286, -1.53666468, 138.99617087]),
   antenna='ant_ea25',
@@ -57,33 +85,43 @@
 
     delta_mean_shift = np.abs(mean_shift - expected_shift)
     delta_ref_shift = np.abs(ref_mean_shift - expected_shift)
         
     delta_shift = delta_mean_shift - delta_ref_shift   # New corrections - old corrections --> delta if delta < 0 ==> we improved.
     relative_shift = relative_difference(delta_mean_shift, delta_ref_shift)
     
-    return np.all(relative_shift <= 1e-6)
+    return np.all(relative_shift < 1e-6)
 
-def verify_center_pixels(file, reference_center_pixels, number_of_digits=7):
+def verify_center_pixels(file, antenna, ddi, reference_center_pixels, number_of_digits=7):
     from astrohack.dio import open_image
     
-    mds = open_image(file)['ant_ea25']['ddi_0']
+    mds = open_image(file)[antenna][ddi]
     
     aperture_shape = mds.APERTURE.values.shape[-2], mds.APERTURE.values.shape[-1]
     beam_shape = mds.BEAM.values.shape[-2], mds.BEAM.values.shape[-1]    
     
-    aperture_center_pixels = mds.APERTURE.values[..., aperture_shape[0]//2, aperture_shape[1]//2]
-    beam_center_pixels = mds.BEAM.values[..., beam_shape[0]//2, beam_shape[1]//2]
+    aperture_center_pixels = np.squeeze(mds.APERTURE.values[..., aperture_shape[0]//2, aperture_shape[1]//2])
+    beam_center_pixels = np.squeeze(mds.BEAM.values[..., beam_shape[0]//2, beam_shape[1]//2])
     
-    aperture_check = np.all(np.round(reference_center_pixels['aperture'], number_of_digits) == np.round(aperture_center_pixels, number_of_digits))
-    beam_check = np.all(np.round(reference_center_pixels['beam'], number_of_digits) == np.round(beam_center_pixels, number_of_digits))
-
-    return aperture_check and beam_check
+    aperture_ref = list(map(complex, reference_center_pixels['aperture']))
+    beam_ref = list(map(complex, reference_center_pixels['beam']))
     
+    for i in range(len(aperture_ref)):
+        # Should probably write a custom round function here
+        aperture_check = round(aperture_ref[i].real, number_of_digits) == round(aperture_center_pixels[i].real, number_of_digits)
+        beam_check = round(beam_ref[i].real, number_of_digits) == round(beam_center_pixels[i].real, number_of_digits)
     
+        real_check = aperture_check and beam_check
+
+        aperture_check = round(aperture_ref[i].imag, number_of_digits) == round(aperture_center_pixels[i].imag, number_of_digits)
+        beam_check = round(beam_ref[i].imag, number_of_digits) == round(beam_center_pixels[i].imag, number_of_digits)
+
+        imag_check = aperture_check and beam_check
+
+    return real_check and imag_check   
                 
 def verify_holog_obs_dictionary(holog_obs_dict):
 
     ref_holog_obj = {}
     ref_holog_obj = copy.deepcopy(holog_obs_dict)
 
     _jsonify(ref_holog_obj)
@@ -104,157 +142,92 @@
 
 def test_holog_obs_dict(set_data):
     before_ms = str(set_data/"".join((base_name,"before_fixed.split.ms")))
     before_holog = str(set_data/"before.split.holog.zarr")
     after_ms =  str(set_data/"".join((base_name, "after_fixed.split.ms")))
     after_holog = str(set_data/"after.split.holog.zarr")
 
-    holog_obs_dict = {
-      'ddi_0': {
-        'map_0': {
-            'ant': {
-                'ea06': np.array(['ea04']),
-                'ea25': np.array(['ea04'])
-            },
-            'scans': np.array([
-                8, 9, 10, 12, 13, 14, 16, 17, 18, 23, 24, 
-                25, 27, 28, 29, 31, 32, 33, 38, 39, 40, 
-                42, 43, 44, 46, 47, 48, 53, 54, 55, 57
-            ])
-          }
-        }
-    }
-
+    with open(str(set_data/"extract_holog_verification.json")) as file:
+      holog_obs_dict = json_dict = json.load(file)
 
     extract_holog(
       ms_name=before_ms, 
       holog_name=before_holog, 
-      ddi_sel=[0],
+      ddi=[0],
       data_column='CORRECTED_DATA',
       parallel=False,
       overwrite=True,
       reuse_point_zarr=False
     )
 
-    assert verify_holog_obs_dictionary(holog_obs_dict)
-
-    holog_obs_dict = {
-      'ddi_0': {
-          'map_0': {
-              'ant': {
-                  'ea06': np.array(['ea04']),
-                  'ea25': np.array(['ea04'])
-              },
-              'scans': np.array([
-                8,  9, 10, 12, 13, 14, 16, 17, 18, 
-                23, 24, 25, 27, 28, 29, 31, 32, 33, 
-                38, 39, 40, 42, 43, 44, 46, 47, 48, 
-                53, 54, 55, 57
-              ])
-            }
-        },
-        'ddi_1': {
-          'map_0': {
-              'ant': {
-                'ea06': np.array(['ea04']),
-                'ea25': np.array(['ea04'])
-              },
-              'scans': np.array([
-                8,  9, 10, 12, 13, 14, 16, 17, 18, 
-                23, 24, 25, 27, 28, 29, 31, 32, 33, 
-                38, 39, 40, 42, 43, 44, 46, 47, 48, 
-                53, 54, 55, 57
-              ])
-            }
-        }
-    }
+    assert verify_holog_obs_dictionary(holog_obs_dict["vla"]["before"])
 
 
     holog_mds_after, _ = extract_holog(
         ms_name=after_ms, 
         holog_name=after_holog,
         data_column='CORRECTED_DATA',
         parallel=False,
         overwrite=True,
         reuse_point_zarr=False
     )
 
-    assert verify_holog_obs_dictionary(holog_obs_dict)
+    assert verify_holog_obs_dictionary(holog_obs_dict["vla"]["after"])
+
+    alma_ms = str(set_data/"J1924-2914.ms.calibrated.split.SPW3")
+    alma_holog = str(set_data/"alma.split.holog.zarr")
+
+    extract_holog(
+      ms_name=alma_ms,
+      holog_name=alma_holog,
+      data_column='DATA',
+      parallel=False,
+      overwrite=True,
+      reuse_point_zarr=False
+    )
+
+    verify_holog_obs_dictionary(holog_obs_dict["alma"])
 
 def test_holog(set_data):
-  reference_before_dict = {
-    'aperture': np.array([
-        [
-            [ 
-                0.225725131776915+0.12054326352090801j, 
-                0.016838151657196862-0.011171227001989446j, 
-                0.048663223170791664-0.024197325651061738j, 
-                -0.09340400975688747-0.045923630603716084j
-            ]
-        ]
-    ]),
-    'beam': np.array([
-        [
-            [ 
-                0.993988815582417+0.10948166283475885j,
-                0.005367471552903289+0.01583907120584613j,
-                0.014425807274417096+0.0059018780911659395j,
-                -0.004021223235578464+0.00040825140567029433j
-            ]
-        ]
-    ])
-  }
-
-  reference_after_dict = {
-    'aperture': np.array([
-        [
-            [ 
-                0.12300077664655817-0.06757802469840296j,
-                -0.062129865145786264+0.15643752202705213j,
-                0.012563562045357843+0.1010680231104541j,
-                0.016046659386512153-0.008623951102220646j
-            ]
-        ]
-    ]),
-    'beam': np.array([
-        [
-            [ 
-                0.9979274427989393+0.06434919509030099j,
-                0.00894231045479574+0.022065573193509103j,
-                0.02131330222465877+0.0051265326714060675j,
-                0.00271048218206843-0.005807650531399505j
-            ]
-        ]
-    ])
-  }
+  
+  with open(str(set_data/"holog_numerical_verification.json")) as file:
+    reference_dict = json.load(file)
+
 
   before_holog = str(set_data/"before.split.holog.zarr")
   after_holog = str(set_data/"after.split.holog.zarr")
 
   before_image = str(set_data/"before.split.image.zarr")
   after_image = str(set_data/"after.split.image.zarr")
+
+  alma_ms = str(set_data/"J1924-2914.ms.calibrated.split.SPW3")
+  alma_holog = str(set_data/"alma.split.holog.zarr")
   
   holog(
     holog_name=before_holog, 
     padding_factor=50, 
     grid_interpolation_mode='linear',
     chan_average = True,
     scan_average = True,
     overwrite=True,
     phase_fit=True,
     apply_mask=True,
     to_stokes=True,
     parallel=True
   )
   
-  assert verify_center_pixels(file=before_image, reference_center_pixels=reference_before_dict)
+  assert verify_center_pixels(
+    file=before_image, 
+    antenna='ant_ea25',
+    ddi='ddi_0',
+    reference_center_pixels=reference_dict["vla"]["pixels"]["before"])
 
   assert verify_holog_diagnostics(
-    cell_size = np.array([-0.0006442, 0.0006442]),
-    grid_size = np.array([31, 31]),
+    cell_size = np.array(reference_dict["vla"]['cell_size']),
+    grid_size = np.array(reference_dict["vla"]['grid_size']),
     number_of_digits=7
   )
 
   holog(
     holog_name=after_holog, 
     padding_factor=50, 
     grid_interpolation_mode='linear',
@@ -263,25 +236,57 @@
     overwrite=True,
     phase_fit=True,
     apply_mask=True,
     to_stokes=True,
     parallel=True
   )
 
-  assert verify_center_pixels(file=after_image, reference_center_pixels=reference_after_dict)
+  assert verify_center_pixels(
+    file=after_image, 
+    antenna='ant_ea25',
+    ddi='ddi_0',
+    reference_center_pixels=reference_dict["vla"]["pixels"]["after"]
+  )
 
   assert verify_holog_diagnostics(
-    cell_size = np.array([-0.0006442, 0.0006442]),
-    grid_size = np.array([31, 31]),
+    cell_size = np.array(reference_dict["vla"]['cell_size']),
+    grid_size = np.array(reference_dict["vla"]['grid_size']),
     number_of_digits=7
   )
 
+  holog(
+    holog_name=alma_holog, 
+    padding_factor=50, 
+    grid_interpolation_mode="linear",
+    chan_average = True,
+    scan_average = True,
+    overwrite=True,
+    phase_fit=True,
+    apply_mask=True,
+    to_stokes=True,
+    parallel=True
+)
+    
+  verify_center_pixels(
+    file=str(set_data/"alma.split.image.zarr"), 
+    antenna="ant_DV13", 
+    ddi="ddi_0", 
+    reference_center_pixels=reference_dict["alma"]['pixels']
+  )
+
+  verify_holog_diagnostics(
+    cell_size = np.array(reference_dict["alma"]['cell_size']),
+    grid_size = np.array(reference_dict["alma"]['grid_size']),
+    number_of_digits=6
+  )
+
 def test_screw_adjustments(set_data):
   before_image = str(set_data/"before.split.image.zarr")
   after_image = str(set_data/"after.split.image.zarr")
+  alma_image = str(set_data/"alma.split.image.zarr")
 
   before_panel = panel(
     image_name=before_image, 
     panel_model='rigid',
     parallel=True,
     overwrite=True
   )
@@ -289,7 +294,17 @@
     image_name=after_image, 
     panel_model='rigid',
     parallel=True,
     overwrite=True
   )
 
   assert verify_panel_shifts(data_dir=str(set_data))
+
+  alma_panel = panel(
+    image_name=alma_image, 
+    panel_model='rigid',
+    parallel=True,
+    overwrite=True
+  )
+
+
+  assert verify_panel_positions(data_dir=str(set_data))
```

