# Comparing `tmp/fusion-engine-client-1.19.0.tar.gz` & `tmp/fusion-engine-client-1.20.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-client-1.19.0.tar", last modified: Fri May  5 22:20:30 2023, max compression
+gzip compressed data, was "fusion-engine-client-1.20.0rc1.tar", last modified: Fri Jun  2 20:03:05 2023, max compression
```

## Comparing `fusion-engine-client-1.19.0.tar` & `fusion-engine-client-1.20.0rc1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.386067 fusion-engine-client-1.19.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-05 22:20:30.382067 fusion-engine-client-1.19.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.378066 fusion-engine-client-1.19.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/bin/p1_display
--rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/bin/p1_extract
--rwxr-xr-x   0 runner    (1001) docker     (123)    13349 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/bin/p1_print
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.378066 fusion-engine-client-1.19.0/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.378066 fusion-engine-client-1.19.0/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   107613 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    41032 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.382067 fusion-engine-client-1.19.0/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55470 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/measurement_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.382067 fusion-engine-client-1.19.0/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22860 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.382067 fusion-engine-client-1.19.0/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23392 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.378066 fusion-engine-client-1.19.0/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-05 22:20:30.000000 fusion-engine-client-1.19.0/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-05 22:20:30.000000 fusion-engine-client-1.19.0/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:20:30.000000 fusion-engine-client-1.19.0/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-05 22:20:30.000000 fusion-engine-client-1.19.0/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 22:20:30.000000 fusion-engine-client-1.19.0/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:20:30.386067 fusion-engine-client-1.19.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.382067 fusion-engine-client-1.19.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.525266 fusion-engine-client-1.20.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-02 20:03:05.525266 fusion-engine-client-1.20.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.517266 fusion-engine-client-1.20.0rc1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/bin/p1_display
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/bin/p1_extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14038 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/bin/p1_print
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.517266 fusion-engine-client-1.20.0rc1/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.517266 fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   110311 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41032 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.521266 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56191 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26067 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.521266 fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22860 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.521266 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.517266 fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-02 20:03:05.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-02 20:03:05.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 20:03:05.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-02 20:03:05.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 20:03:05.000000 fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 20:03:05.525266 fusion-engine-client-1.20.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:03:05.525266 fusion-engine-client-1.20.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-06-02 20:02:30.000000 fusion-engine-client-1.20.0rc1/tests/test_time_range.py
```

### Comparing `fusion-engine-client-1.19.0/PKG-INFO` & `fusion-engine-client-1.20.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.19.0
+Version: 1.20.0rc1
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.19.0/README.md` & `fusion-engine-client-1.20.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/bin/p1_extract` & `fusion-engine-client-1.20.0rc1/bin/p1_extract`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/bin/p1_print` & `fusion-engine-client-1.20.0rc1/bin/p1_print`

 * *Files 2% similar despite different names*

```diff
@@ -222,29 +222,38 @@
                     p1_time = message.get_p1_time()
                     if p1_time is not None:
                         if first_p1_time_sec is None:
                             first_p1_time_sec = float(p1_time)
                             last_p1_time_sec = float(p1_time)
                             newest_p1_time = p1_time
                         else:
-                            if p1_time < newest_p1_time:
-                                _logger.warning('P1 time restart detected after %s.' % str(newest_p1_time))
+                            # For P1 time, we allow a small tolerance to account for normal latency between measurements
+                            # and computed data like pose solutions.
+                            dt_sec = float(newest_p1_time - p1_time)
+                            if dt_sec < -0.2:
+                                _logger.warning(
+                                    'P1 time restart detected after %s. [message=%s, p1_time=%s, offset=%d B]' %
+                                    (str(newest_p1_time), header.get_type_string(), str(p1_time), offset_bytes))
                             last_p1_time_sec = max(last_p1_time_sec, float(p1_time))
                             newest_p1_time = p1_time
 
                     system_time_sec = message.get_system_time_sec()
                     if system_time_sec is not None:
                         if first_system_time_sec is None:
                             first_system_time_sec = system_time_sec
                             last_system_time_sec = system_time_sec
                             newest_system_time_sec = system_time_sec
                         else:
                             if system_time_sec < newest_system_time_sec:
-                                _logger.warning('System time restart detected after %s.' %
-                                                system_time_to_str(newest_system_time_sec, is_seconds=True))
+                                _logger.warning(
+                                    'System time restart detected after %s. [message=%s, system_time=%s, offset=%d B]' %
+                                    (system_time_to_str(newest_system_time_sec, is_seconds=True),
+                                     header.get_type_string(),
+                                     system_time_to_str(system_time_sec, is_seconds=True),
+                                     offset_bytes))
                             last_system_time_sec = max(last_system_time_sec, system_time_sec)
                             newest_system_time_sec = system_time_sec
             else:
                 print_message(header, message, offset_bytes, format=options.format)
     except (BrokenPipeError, KeyboardInterrupt) as e:
         sys.exit(1)
```

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/analysis/analyzer.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
             return
 
         # Setup the figure.
         figure = make_subplots(rows=2, cols=1, print_grid=False, shared_xaxes=True,
                                subplot_titles=['Device Time vs. Relative Time',
                                                'Pose Message Interval vs. Relative Time'])
 
-        figure['layout'].update(showlegend=True)
+        figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
         for i in range(2):
             figure['layout']['xaxis%d' % (i + 1)].update(title="Relative Time (sec)", showticklabels=True)
         figure['layout']['yaxis1'].update(title="Absolute Time",
                                           ticktext=['P1/GPS Time', 'System Time'],
                                           tickvals=[1, 2])
         figure['layout']['yaxis2'].update(title="Interval (sec)", rangemode="tozero")
 
@@ -297,15 +297,15 @@
         c_enu_ecef = get_enu_rotation_matrix(*pose_data.lla_deg[0:2, first_idx], deg=True)
 
         # Setup the figure.
         figure = make_subplots(rows=2, cols=3, print_grid=False, shared_xaxes=True,
                                subplot_titles=['Attitude (YPR)', 'ENU Displacement', 'Body Velocity',
                                                'Attitude Std', 'ENU Position Std', 'Velocity Std'])
 
-        figure['layout'].update(showlegend=True)
+        figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
         for i in range(6):
             figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True, matches='x')
         figure['layout']['yaxis1'].update(title="Degrees")
         figure['layout']['yaxis2'].update(title="Meters")
         figure['layout']['yaxis3'].update(title="Meters/Second")
         figure['layout']['yaxis4'].update(title="Degrees")
         figure['layout']['yaxis5'].update(title="Meters")
@@ -404,15 +404,15 @@
 
         # Setup the figure.
         figure = make_subplots(rows=4, cols=1, print_grid=False, shared_xaxes=True,
                                subplot_titles=['<- Percent Complete // Stage ->', 'Mounting Angles',
                                                'Mounting Angle Standard Deviation', 'Travel Distance'],
                                specs=[[{"secondary_y": True}], [{}], [{}], [{}]])
 
-        figure['layout'].update(showlegend=True)
+        figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
         for i in range(4):
             figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True)
         figure['layout']['yaxis1'].update(title="Percent Complete", range=[0, 100])
         figure['layout']['yaxis2'].update(ticktext=['%s' % e.name for e in CalibrationStage],
                                           tickvals=list(range(len(stage_map))))
         figure['layout']['yaxis3'].update(title="Degrees")
         figure['layout']['yaxis4'].update(title="Degrees")
@@ -524,15 +524,15 @@
         topo_figure = make_subplots(rows=1, cols=1, print_grid=False, shared_xaxes=False,
                                     subplot_titles=['Displacement'])
         topo_figure['layout']['xaxis1'].update(title="East (m)")
         topo_figure['layout']['yaxis1'].update(title="North (m)")
 
         time_figure = make_subplots(rows=4, cols=1, print_grid=False, shared_xaxes=True,
                                     subplot_titles=['3D', 'East', 'North', 'Up'])
-        time_figure['layout'].update(showlegend=True)
+        time_figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
         for i in range(4):
             time_figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True)
         time_figure['layout']['yaxis1'].update(title="Displacement (m)")
         time_figure['layout']['yaxis2'].update(title="Displacement (m)")
         time_figure['layout']['yaxis3'].update(title="Displacement (m)")
         time_figure['layout']['yaxis4'].update(title="Displacement (m)")
 
@@ -1056,15 +1056,15 @@
         figure = make_subplots(
             rows=4, cols=1,  print_grid=False, shared_xaxes=True,
             subplot_titles=['Distance To Station', 'Corrections Age'],
             specs=[[{'rowspan': 3}],
                    [None],
                    [None],
                    [{}]])
-        figure['layout'].update(showlegend=True)
+        figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
         for i in range(2):
             figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True, matches='x')
         figure['layout']['yaxis1'].update(title="Baseline Distance (km)")
         figure['layout']['yaxis2'].update(title="Age (sec)")
 
         # Find all base stations present in the data and assign a color to each.
         station_ids = np.unique([s for s in data.reference_station_id
@@ -1215,15 +1215,15 @@
                titles[0] += '<br>Messages: '
            titles[0] += f'{vehicle_measurement_type.__name__}'
         if raw_vehicle_data is not None and vehicle_measurement_type != raw_vehicle_measurement_type:
             titles[0] += f', {raw_vehicle_measurement_type.__name__}'
 
         figure = make_subplots(rows=len(titles), cols=1, print_grid=False, shared_xaxes=True, subplot_titles=titles)
 
-        figure['layout'].update(showlegend=True, modebar_add=['v1hovermode', 'toggleSpikelines'])
+        figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
         for i in range(len(titles)):
             figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True)
 
         if type == 'tick':
             figure['layout']['yaxis1'].update(title="Tick Count")
             figure['layout']['yaxis2'].update(title="Tick Rate (ticks/s)")
         else:
@@ -1477,28 +1477,29 @@
                     return
 
         # Read the data.
         result = self.reader.read(message_types=[message_cls], **self.params)
         data = result[message_cls.MESSAGE_TYPE]
 
         if len(data.p1_time) == 0:
-            self.logger.info('No IMU data available. Skipping plot.')
+            self.logger.info('No %s data available. Skipping plot.' %
+                             ('IMU' if message_cls is IMUOutput else 'raw IMU'))
             return
 
         time = data.p1_time - float(self.t0)
 
         titles = ['Acceleration', 'Gyro']
         if message_cls == RawIMUOutput:
             titles = [t + ' (Uncorrected)' for t in titles]
         else:
             titles = [t + ' (Corrected)' for t in titles]
 
         figure = make_subplots(rows=2, cols=1, print_grid=False, shared_xaxes=True, subplot_titles=titles)
 
-        figure['layout'].update(showlegend=True)
+        figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
         figure['layout']['xaxis1'].update(title="Time (sec)", showticklabels=True)
         figure['layout']['xaxis2'].update(title="Time (sec)", showticklabels=True)
         figure['layout']['yaxis1'].update(title="Acceleration (m/s^2)")
         figure['layout']['yaxis2'].update(title="Rotation Rate (rad/s)")
 
         figure.add_trace(go.Scattergl(x=time, y=data.accel_mps2[0, :], name='X', legendgroup='x',
                                       mode='lines', line={'color': 'red'}),
@@ -1526,21 +1527,20 @@
         """!
         @brief Generate time series plots for heading (degrees) and baseline distance (meters) data.
         """
         if self.output_dir is None:
             return
 
         # Read the heading measurement data.
-        result = self.reader.read(message_types=[HeadingMeasurement], **self.params)
-        heading_data = result[HeadingMeasurement.MESSAGE_TYPE]
-
-        result = self.reader.read(message_types=[PoseMessage], **self.params)
+        result = self.reader.read(message_types=[RawHeadingOutput, HeadingOutput, PoseMessage], **self.params)
+        raw_heading_data = result[RawHeadingOutput.MESSAGE_TYPE]
+        heading_data = result[HeadingOutput.MESSAGE_TYPE]
         primary_pose_data = result[PoseMessage.MESSAGE_TYPE]
 
-        if len(heading_data.p1_time) == 0:
+        if (len(heading_data.p1_time) == 0) and (len(raw_heading_data.p1_time) == 0):
             self.logger.info('No heading measurement data available. Skipping plot.')
             return
 
         # Setup the figure.
         fig = make_subplots(
             rows=3, cols=1,
             subplot_titles=(
@@ -1559,146 +1559,167 @@
             tickvals=[e.value for e in SolutionType],
             title_text='Solution Type',
             row=3, col=1
         )
 
         fig.update_layout(title='Heading Plots', legend_traceorder='normal')
 
-        # First plot - heading in degrees with error bar
-        # calculate uncertainty envelope for heading
-        denom = heading_data.relative_position_enu_m[0]**2 + heading_data.relative_position_enu_m[1]**2
-        dh_e = heading_data.relative_position_enu_m[0] / denom
-        dh_n = heading_data.relative_position_enu_m[2] / denom
-
-        heading_std = np.sqrt(
-            (dh_e * heading_data.position_std_enu_m[0]) ** 2 +
-            (dh_n * heading_data.position_std_enu_m[1]) ** 2
-        )
-
-        envelope = np.arctan(
-            (2 * heading_std / heading_data.baseline_distance_m)
-        )
-        envelope *= 180. / np.pi
 
         # Display the navigation engine's heading estimate, if available, for comparison with the heading sensor
         # measurement.
         if primary_pose_data is not None:
-            pose_heading_deg = 90.0 - primary_pose_data.ypr_deg[0]
-            pose_heading_deg[pose_heading_deg < 0.0] += 360.0
+            invalid_idx = primary_pose_data.solution_type[primary_pose_data.solution_type != SolutionType.Invalid]
+            yaw_deg = primary_pose_data.ypr_deg[0][invalid_idx]
+            if len(yaw_deg) > 0:
+                pose_heading_deg = 90.0 - yaw_deg
+                pose_heading_deg[pose_heading_deg < 0.0] += 360.0
+                fig.add_trace(
+                    go.Scatter(
+                        x=primary_pose_data.p1_time - float(self.t0),
+                        y=pose_heading_deg,
+                        customdata=primary_pose_data.p1_time,
+                        mode='lines',
+                        line={'color': 'yellow'},
+                        name='Primary Device Heading Estimate',
+                        hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
+                                      '<br><b>Heading</b>: %{y:.2f} deg'
+                    ),
+                    row=1, col=1
+                )
+
+        # Corrected heading plot
+        if len(heading_data.p1_time) > 0:
+            heading_time = heading_data.p1_time - float(self.t0)
             fig.add_trace(
                 go.Scatter(
-                    x=primary_pose_data.p1_time - float(self.t0),
-                    y=pose_heading_deg,
-                    customdata=primary_pose_data.p1_time,
-                    mode='lines',
-                    line={'color': 'yellow'},
-                    name='Primary Device Heading Estimate',
+                    x=heading_time,
+                    y=heading_data.heading_true_north_deg,
+                    customdata=heading_data.p1_time,
+                    mode='markers',
+                    marker={'size': 2, "color": "green"},
+                    name='Corrected Heading Data',
                     hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
-                                  '<br><b>Heading</b>: %{y:.2f} deg'
+                                  '<br><b>Heading</b>: %{y:.2f} deg',
+                    legendgroup='heading'
                 ),
                 row=1, col=1
             )
 
-        heading_time = heading_data.p1_time - float(self.t0)
-
-        fig.add_trace(
-            go.Scatter(
-                x=heading_time,
-                y=heading_data.heading_true_north_deg,
-                customdata=heading_data.p1_time,
-                mode='markers',
-                marker={'size': 2},
-                name='Secondary Device Heading Measurement',
-                hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
-                              '<br><b>Heading</b>: %{y:.2f} deg',
-                legendgroup='heading'
-            ),
-            row=1, col=1
-        )
+        # Uncorrected heading plot
+        if len(raw_heading_data.p1_time) > 0:
+            raw_heading_time = raw_heading_data.p1_time - float(self.t0)
+            # Compute heading uncertainty envelop.
+            denom = raw_heading_data.relative_position_enu_m[0]**2 + raw_heading_data.relative_position_enu_m[1]**2
+            dh_e = raw_heading_data.relative_position_enu_m[0] / denom
+            dh_n = raw_heading_data.relative_position_enu_m[2] / denom
+
+            heading_std = np.sqrt(
+                (dh_e * raw_heading_data.position_std_enu_m[0]) ** 2 +
+                (dh_n * raw_heading_data.position_std_enu_m[1]) ** 2
+            )
 
-        idx = ~np.isnan(heading_data.heading_true_north_deg)
+            envelope = np.arctan(
+                (2 * heading_std / raw_heading_data.baseline_distance_m)
+            )
+            envelope *= 180. / np.pi
+            fig.add_trace(
+                go.Scatter(
+                    x=raw_heading_time,
+                    y=raw_heading_data.heading_true_north_deg,
+                    customdata=raw_heading_data.p1_time,
+                    mode='markers',
+                    marker={'size': 2, "color": "red"},
+                    name='Uncorrected Heading Data',
+                    hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
+                                  '<br><b>Heading</b>: %{y:.2f} deg',
+                    legendgroup='heading'
+                ),
+                row=1, col=1
+            )
+            idx = ~np.isnan(raw_heading_data.heading_true_north_deg)
 
-        fig.add_trace(
-            go.Scatter(
-                x=heading_time[idx],
-                y=heading_data.heading_true_north_deg[idx] + envelope[idx],
-                mode='lines',
-                marker=dict(color="#444"),
-                line=dict(width=0),
-                legendgroup='heading',
-                showlegend=False,
-                hoverinfo='skip'
-            ),
-            row=1, col=1
-        )
+            fig.add_trace(
+                go.Scatter(
+                    x=raw_heading_time[idx],
+                    y=raw_heading_data.heading_true_north_deg[idx] + envelope[idx],
+                    mode='lines',
+                    marker={'size': 2, "color": "red"},
+                    line=dict(width=0),
+                    legendgroup='heading',
+                    showlegend=False,
+                    hoverinfo='skip'
+                ),
+                row=1, col=1
+            )
 
-        fig.add_trace(
-            go.Scatter(
-                x=heading_time[idx],
-                y=heading_data.heading_true_north_deg[idx] - envelope[idx],
-                mode='lines',
-                marker=dict(color="#444"),
-                line=dict(width=0),
-                fillcolor='rgba(68, 68, 68, 0.3)',
-                fill='tonexty',
-                legendgroup='heading',
-                showlegend=False,
-                hoverinfo='skip'
-            ),
-            row=1, col=1
-        )
+            fig.add_trace(
+                go.Scatter(
+                    x=raw_heading_time[idx],
+                    y=raw_heading_data.heading_true_north_deg[idx] - envelope[idx],
+                    mode='lines',
+                    marker={'size': 2, "color": "red"},
+                    line=dict(width=0),
+                    fillcolor='rgba(68, 68, 68, 0.3)',
+                    fill='tonexty',
+                    legendgroup='heading',
+                    showlegend=False,
+                    hoverinfo='skip'
+                ),
+                row=1, col=1
+            )
 
-        # Second plot - baseline, ENU components
-        fig.add_trace(
-            go.Scatter(
-                x=heading_time,
-                y=heading_data.relative_position_enu_m[0],
-                customdata=heading_data.p1_time,
-                hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
-                              '<br><b>East</b>: %{y:.2f} m',
-                name='East'
-            ),
-            row=2, col=1
-        )
+            # Second plot - baseline, ENU components
+            fig.add_trace(
+                go.Scatter(
+                    x=raw_heading_time,
+                    y=raw_heading_data.relative_position_enu_m[0],
+                    customdata=raw_heading_data.p1_time,
+                    hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
+                                  '<br><b>East</b>: %{y:.2f} m',
+                    name='East'
+                ),
+                row=2, col=1
+            )
 
-        fig.add_trace(
-            go.Scatter(
-                x=heading_time,
-                y=heading_data.relative_position_enu_m[1],
-                customdata=heading_data.p1_time,
-                hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
-                              '<br><b>North</b>: %{y:.2f} m',
-                name='North'
-            ),
-            row=2, col=1
-        )
+            fig.add_trace(
+                go.Scatter(
+                    x=raw_heading_time,
+                    y=raw_heading_data.relative_position_enu_m[1],
+                    customdata=raw_heading_data.p1_time,
+                    hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
+                                  '<br><b>North</b>: %{y:.2f} m',
+                    name='North'
+                ),
+                row=2, col=1
+            )
 
-        fig.add_trace(
-            go.Scatter(
-                x=heading_time,
-                y=heading_data.relative_position_enu_m[2],
-                customdata=heading_data.p1_time,
-                hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
-                              '<br><b>Up</b>: %{y:.2f} m',
-                name='Up'
-            ),
-            row=2, col=1
-        )
+            fig.add_trace(
+                go.Scatter(
+                    x=raw_heading_time,
+                    y=raw_heading_data.relative_position_enu_m[2],
+                    customdata=raw_heading_data.p1_time,
+                    hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
+                                  '<br><b>Up</b>: %{y:.2f} m',
+                    name='Up'
+                ),
+                row=2, col=1
+            )
 
-        fig.add_trace(
-            go.Scatter(
-                x=heading_time,
-                y=heading_data.baseline_distance_m,
-                customdata=heading_data.p1_time,
-                hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
-                              '<br><b>Baseline</b>: %{y:.2f} m',
-                name='Baseline'
-            ),
-            row=2, col=1
-        )
+            fig.add_trace(
+                go.Scatter(
+                    x=raw_heading_time,
+                    y=raw_heading_data.baseline_distance_m,
+                    customdata=raw_heading_data.p1_time,
+                    marker={'size': 2, "color": "red"},
+                    hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
+                                  '<br><b>Baseline</b>: %{y:.2f} m',
+                    name='Baseline'
+                ),
+                row=2, col=1
+            )
 
         # 3rd plot - solution type
         if primary_pose_data is not None:
             fig.add_trace(
                 go.Scatter(
                     x=primary_pose_data.p1_time - float(self.t0),
                     y=primary_pose_data.solution_type,
@@ -1709,27 +1730,43 @@
                                   '<br><b>Solution</b>: %{text}',
                     text=[str(SolutionType(s)) for s in primary_pose_data.solution_type],
                     name='Primary Solution Type'
                 ),
                 row=3, col=1
             )
 
-        fig.add_trace(
-            go.Scatter(
-                x=heading_time,
-                y=heading_data.solution_type,
-                customdata=heading_data.p1_time,
-                mode='markers',
-                hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
-                              '<br><b>Solution</b>: %{text}',
-                text=[str(SolutionType(s)) for s in heading_data.solution_type],
-                name='Secondary Solution Type'
-            ),
-            row=3, col=1
-        )
+        if len(raw_heading_data.p1_time) > 0:
+            fig.add_trace(
+                go.Scatter(
+                    x=raw_heading_time,
+                    y=raw_heading_data.solution_type,
+                    customdata=raw_heading_data.p1_time,
+                    marker={'color': 'red'},
+                    hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
+                                  '<br><b>Solution</b>: %{text}',
+                    text=[str(SolutionType(s)) for s in raw_heading_data.solution_type],
+                    name='Uncorrected Heading Solution Type'
+                ),
+                row=3, col=1
+            )
+
+        if len(heading_data.p1_time) > 0:
+            fig.add_trace(
+                go.Scatter(
+                    x=heading_time,
+                    y=heading_data.solution_type,
+                    customdata=heading_data.p1_time,
+                    marker={'color': 'green'},
+                    hovertemplate='<b>Time</b>: %{x:.3f} sec (%{customdata:.3f} sec)'
+                                  '<br><b>Solution</b>: %{text}',
+                    text=[str(SolutionType(s)) for s in raw_heading_data.solution_type],
+                    name='Corrected Heading Solution Type'
+                ),
+                row=3, col=1
+            )
 
         self._add_figure(name='heading_measurement', figure=fig, title='Measurements: Heading')
 
     def plot_events(self):
         """!
         @brief Generate a table of event notifications.
         """
@@ -1908,16 +1945,16 @@
             'Start Time',
             '',
             '',
             'Processed Duration',
             'Total Log Duration',
         ]
         times = [
-            str(self.t0),
-            system_time_to_str(self.system_t0, is_seconds=True).replace(' time', ':'),
+            str(self.reader.t0),
+            system_time_to_str(self.reader.get_system_t0(), is_seconds=True).replace(' time', ':'),
             # Note: Temporarily replacing <br> so it doesn't get stripped by _data_to_table().
             self._gps_sec_to_string(t0_gps) \
                 .replace('<br>', (' (approximated)' if t0_is_approx else '') + '<brbak>') \
                 .replace('<brbak>', '<br>'),
             '%.1f seconds' % processing_duration_sec,
             log_duration_sec,
         ]
```

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/analysis/attitude.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/analysis/data_loader.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/analysis/data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/messages/configuration.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     DEVICE_LEVER_ARM = 16
     DEVICE_COARSE_ORIENTATION = 17
     GNSS_LEVER_ARM = 18
     OUTPUT_LEVER_ARM = 19
     VEHICLE_DETAILS = 20
     WHEEL_CONFIG = 21
     HARDWARE_TICK_CONFIG = 22
+    HEADING_BIAS = 23
     ENABLED_GNSS_SYSTEMS = 50
     ENABLED_GNSS_FREQUENCY_BANDS = 51
     LEAP_SECOND = 52
     GPS_WEEK_ROLLOVER = 53
     IONOSPHERE_CONFIG = 54
     TROPOSPHERE_CONFIG = 55
     INTERFACE_CONFIG = 200
@@ -570,14 +571,27 @@
     HardwareTickConfigConstruct = Struct(
         "tick_mode" / AutoEnum(Int8ul, TickMode),
         "tick_direction" / AutoEnum(Int8ul, TickDirection),
         Padding(2),
         "wheel_ticks_to_m" / Float32l,
     )
 
+    class HeadingBias(NamedTuple):
+        """!
+        @brief Horizontal and vertical heading bias configuration settings.
+        """
+        horizontal_bias_deg: float = math.nan
+        vertical_bias_deg: float = math.nan
+
+
+    HeadingBiasConstruct = Struct(
+        "horizontal_bias_deg" / Float32l,
+        "vertical_bias_deg" / Float32l,
+    )
+
     class IonosphereConfig(NamedTuple):
         """!
         @brief Ionospheric delay model configuration.
         """
         ## The ionospheric delay model to use.
         iono_delay_model: IonoDelayModel = IonoDelayModel.AUTO
 
@@ -775,14 +789,21 @@
 class HardwareTickConfig(_conf_gen.HardwareTickConfig):
     """!
     @brief Tick configuration settings.
     """
     pass
 
 
+@_conf_gen.create_config_class(ConfigType.HEADING_BIAS, _conf_gen.HeadingBiasConstruct)
+class HeadingBias(_conf_gen.HeadingBias):
+    """!
+    @brief Horizontal and vertical heading bias.
+    """
+    pass
+
 @_conf_gen.create_interface_config_class(InterfaceConfigType.BAUD_RATE, _conf_gen.UInt32Construct)
 class InterfaceBaudRateConfig(_conf_gen.IntegerVal):
     """!
     @brief Interface baud configuration settings.
     """
     pass
 
@@ -1245,15 +1266,16 @@
         parsed = self.SetMessageRateConstruct.parse(buffer[offset:])
         self.__dict__.update(parsed)
         return parsed._io.tell()
 
     def __repr__(self):
         result = super().__repr__()[:-1]
         result += f', interface={self.output_interface}, flags=0x{self.flags:02X}, protocol={self.protocol}, ' \
-                  f'message_id={self.message_id}, rate={self.rate}]'
+                  f'message_id={get_message_type_string(protocol=self.protocol, message_id=self.message_id)}, ' \
+                  f'rate={self.rate}]'
         return result
 
     def __str__(self):
         return construct_message_to_string(
             message=self, construct=self.SetMessageRateConstruct,
             title=f'Set Message Output Rate Command',
             fields=['output_interface', 'protocol', 'message_id', 'rate', 'flags'],
@@ -1265,15 +1287,15 @@
     @classmethod
     def calcsize(cls) -> int:
         return cls.SetMessageRateConstruct.sizeof()
 
 
 class GetMessageRate(MessagePayload):
     """!
-    @brief Get the configured output rate for the he requested message type on  the specified interface.
+    @brief Get the configured output rate for the requested message type on  the specified interface.
     """
     MESSAGE_TYPE = MessageType.GET_MESSAGE_RATE
     MESSAGE_VERSION = 0
 
     GetMessageRateConstruct = Struct(
         "output_interface" / _InterfaceIDConstruct,
         "protocol" / AutoEnum(Int8ul, ProtocolType),
@@ -1307,15 +1329,15 @@
         parsed = self.GetMessageRateConstruct.parse(buffer[offset:])
         self.__dict__.update(parsed)
         return parsed._io.tell()
 
     def __repr__(self):
         result = super().__repr__()[:-1]
         result += f', interface={self.output_interface}, source={self.request_source}, protocol={self.protocol}, ' \
-                  f'message_id={self.message_id}]'
+                  f'message_id={get_message_type_string(protocol=self.protocol, message_id=self.message_id)}]'
         return result
 
     def __str__(self):
         return construct_message_to_string(
             message=self, construct=self.GetMessageRateConstruct,
             title=f'Get Message Output Rate Command',
             fields=['output_interface', 'protocol', 'request_source', 'message_id'],
```

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/messages/control.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/control.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import string
 import struct
 
 from construct import (Struct, Int64ul, Int16ul, Int8ul, Padding, this, Bytes, PaddedString)
 
 from ..utils.construct_utils import AutoEnum, construct_message_to_string
 from ..utils.enum_utils import IntEnum
 from .defs import *
@@ -405,14 +406,88 @@
         string += f'  GNSS receiver: {self.rx_version_str}'
         return string
 
     def calcsize(self) -> int:
         return len(self.pack())
 
 
+class DeviceType(IntEnum):
+    UNKNOWN = 0
+    ATLAS = 1
+    LG69T_AM = 2
+    LG69T_AP = 3
+    LG69T_AH = 4
+
+
+class DeviceIDMessage(MessagePayload):
+    """!
+    @brief Device identifiers.
+    """
+    MESSAGE_TYPE = MessageType.DEVICE_ID
+    MESSAGE_VERSION = 0
+    _PRINTABLE_CHARS = bytes(string.printable, 'ascii')
+
+    DeviceIDMessageConstruct = Struct(
+        "system_time_ns" / Int64ul,
+        "device_type" / AutoEnum(Int8ul, DeviceType),
+        "hw_id_length" / Int8ul,
+        "user_id_length" / Int8ul,
+        "receiver_id_length" / Int8ul,
+        Padding(4),
+        "hw_id_data" / Bytes(this.hw_id_length),
+        "user_id_data" / Bytes(this.user_id_length),
+        "receiver_id_data" / Bytes(this.receiver_id_length),
+    )
+
+    def __init__(self):
+        self.system_time_ns = 0
+        self.device_type = DeviceType.UNKNOWN
+        self.hw_id_data = b""
+        self.user_id_data = b""
+        self.receiver_id_data = b""
+
+    def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
+        values = dict(self.__dict__)
+        values['hw_id_length'] = len(self.hw_id_length)
+        values['user_id_length'] = len(self.user_id_length)
+        values['receiver_id_length'] = len(self.receiver_id_length)
+        packed_data = self.DeviceIDMessageConstruct.build(values)
+        return PackedDataToBuffer(packed_data, buffer, offset, return_buffer)
+
+    def unpack(self, buffer: bytes, offset: int = 0, message_version: int = MessagePayload._UNSPECIFIED_VERSION) -> int:
+        parsed = self.DeviceIDMessageConstruct.parse(buffer[offset:])
+        self.__dict__.update(parsed)
+        return parsed._io.tell()
+
+    @staticmethod
+    def _get_str(msg: bytes) -> str:
+        is_printable = all(b in DeviceIDMessage.__PRINTABLE_CHARS for b in msg)
+        if is_printable:
+            return msg.decode('ascii')
+        else:
+            return '[' + ' '.join(f'{b:02X}' for b in msg) + ']'
+
+    def __repr__(self):
+        result = super().__repr__()[:-1]
+        result += f'type={self.device_type}, hw={self._get_str(self.hw_id_data)}, user={self._get_str(self.user_id_data)},\
+            rx={self._get_str(self.receiver_id_data)}'
+        return result
+
+    def __str__(self):
+        string = f'Device ID Info @ %s\n' % system_time_to_str(self.system_time_ns)
+        string += f'  Device Type: {device_type}\n'
+        string += f'  HW ID: {self._get_str(self.hw_id_data)}\n'
+        string += f'  User ID: {self._get_str(self.user_id_data)}\n'
+        string += f'  Receiver ID: {self._get_str(self.receiver_id_data)}'
+        return string
+
+    def calcsize(self) -> int:
+        return len(self.pack())
+
+
 class EventType(IntEnum):
     LOG = 0
     RESET = 1
     CONFIG_CHANGE = 2
     COMMAND = 3
     COMMAND_RESPONSE = 4
```

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/messages/defs.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,17 @@
     RELATIVE_ENU_POSITION = 10005
 
     # Device status messages.
     SYSTEM_STATUS = 10500
 
     # Sensor measurement messages.
     IMU_OUTPUT = 11000
-    HEADING_MEASUREMENT = 11001
+    RAW_HEADING_OUTPUT = 11001
     RAW_IMU_MEASUREMENT = 11002
+    HEADING_OUTPUT = 11003
 
     # Vehicle measurement messages.
     DEPRECATED_WHEEL_SPEED_MEASUREMENT = 11101
     DEPRECATED_VEHICLE_SPEED_MEASUREMENT = 11102
 
     WHEEL_TICK_INPUT = 11103
     VEHICLE_TICK_INPUT = 11104
@@ -127,14 +128,15 @@
     COMMAND_RESPONSE = 13000
     MESSAGE_REQUEST = 13001
     RESET_REQUEST = 13002
     VERSION_INFO = 13003
     EVENT_NOTIFICATION = 13004
     SHUTDOWN_REQUEST = 13005
     FAULT_CONTROL = 13006
+    DEVICE_ID = 13007
 
     SET_CONFIG = 13100
     GET_CONFIG = 13101
     SAVE_CONFIG = 13102
     CONFIG_RESPONSE = 13103
 
     IMPORT_DATA = 13110
```

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/messages/device.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/device.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/messages/fault_control.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/fault_control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/messages/measurement_details.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/measurement_details.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/messages/measurements.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/measurements.py`

 * *Files 5% similar despite different names*

```diff
@@ -886,134 +886,226 @@
             'is_signed': np.array([m.is_signed for m in messages], dtype=bool),
             'gear': np.array([m.gear for m in messages], dtype=int),
         }
         result.update(MeasurementDetails.to_numpy([m.details for m in messages]))
         return result
 
 ################################################################################
-# Meading Measurements
+# Heading Sensor Definitions
 ################################################################################
 
 
-class HeadingMeasurement(MessagePayload):
+class HeadingOutput(MessagePayload):
     """!
-     @brief The heading angle (in degrees) with respect to true north,
-            pointing from the primary antenna to the secondary antenna.
-     @ingroup solution_messages
-
-     @note
-     All data is timestamped using the P1 Time values, which is a monotonic
-     timestamp referenced to the start of the device. Corresponding messages (@ref
-     PoseMessage, @ref GNSSSatelliteMessage, etc.) may be associated using
-     their @ref timestamps.
+     @brief Corrected heading sensor measurement output.
     """
-    MESSAGE_TYPE = MessageType.HEADING_MEASUREMENT
+    MESSAGE_TYPE = MessageType.HEADING_OUTPUT
     MESSAGE_VERSION = 0
 
-    _STRUCT = struct.Struct('<B3xL3f3fff')
+    _STRUCT = struct.Struct('<B3xL3ff')
 
     def __init__(self):
         ## Measurement timestamps, if available. See @ref measurement_messages.
         self.details = MeasurementDetails()
 
-        # The type of this position solution.
+        ## Set to @ref SolutionType::RTKFixed when heading is available, or @ref SolutionType::Invalid otherwise.
         self.solution_type = SolutionType.Invalid
-        # A bitmask of flags associated with the solution
+        ## A bitmask of flags associated with the solution
         self.flags = 0
-        # The ID of the differential base station, if used.
+        ## The measured YPR vector (in degrees), resolved in the ENU frame.
+        self.ypr_deg = np.full((3,), np.nan)
+
         ##
-        # The relative position (in meters), resolved in the local ENU frame.
+        # The corrected heading between the primary device antenna and the secondary (in degrees) with
+        # respect to true north.
         #
         # @note
-        # If a differential solution to the base station is not available, these
-        # values will be `NAN`.
+        # Reported in the range [0, 360).
+        self.heading_true_north_deg = np.nan
+
+    def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
+        if buffer is None:
+            buffer = bytearray(self.calcsize())
+
+        initial_offset = offset
+
+        buffer = self.details.pack(buffer)
+        offset += self.details.calcsize()
+
+        self._STRUCT.pack_into(
+            buffer, offset,
+            int(self.solution_type),
+            self.flags,
+            self.ypr_deg[0],
+            self.ypr_deg[1],
+            self.ypr_deg[2],
+            self.heading_true_north_deg)
+        offset += self._STRUCT.size
+
+        if return_buffer:
+            return buffer
+        else:
+            return offset - initial_offset
+
+    def unpack(self, buffer: bytes, offset: int = 0, message_version: int = MessagePayload._UNSPECIFIED_VERSION) -> int:
+        initial_offset = offset
+
+        offset += self.details.unpack(buffer, offset)
+
+        (solution_type_int,
+         self.flags,
+         self.ypr_deg[0],
+         self.ypr_deg[1],
+         self.ypr_deg[2],
+         self.heading_true_north_deg) = self._STRUCT.unpack_from(buffer, offset)
+        offset += self._STRUCT.size
+
+        self.solution_type = SolutionType(solution_type_int)
+
+        return offset - initial_offset
+
+    def __repr__(self):
+        result = super().__repr__()[:-1]
+        ypr_str = ['%.1f' % v for v in self.ypr_deg]
+        result += f', solution_type={self.solution_type}, ypr=[{ypr_str}] deg]'
+        return result
+
+    def __str__(self):
+        return f"""\
+Heading Output @ {str(self.details.p1_time)}
+  Solution Type: {self.solution_type}
+  YPR (ENU) (deg): {self.ypr_deg[0]:.2f}, {self.ypr_deg[1]:.2f}, {self.ypr_deg[2]:.2f}
+  Heading (deg): {self.heading_true_north_deg:.2f}
+  """
+
+    @classmethod
+    def calcsize(cls) -> int:
+        return cls._STRUCT.size + MeasurementDetails.calcsize()
+
+    @classmethod
+    def to_numpy(cls, messages: Sequence['HeadingOutput']):
+        result = {
+            'solution_type': np.array([int(m.solution_type) for m in messages], dtype=int),
+            'flags': np.array([int(m.flags) for m in messages], dtype=int),
+            'ypr_deg': np.array([m.ypr_deg for m in messages]).T,
+            'heading_true_north_deg': np.array([m.heading_true_north_deg for m in messages], dtype=float).T,
+        }
+        result.update(MeasurementDetails.to_numpy([m.details for m in messages]))
+        return result
+
+
+class RawHeadingOutput(MessagePayload):
+    """!
+     @brief Raw (uncorrected) heading sensor measurement output.
+    """
+    MESSAGE_TYPE = MessageType.RAW_HEADING_OUTPUT
+    MESSAGE_VERSION = 0
+
+    _STRUCT = struct.Struct('<B3xL3f3fff')
+
+    def __init__(self):
+        ## Measurement timestamps, if available. See @ref measurement_messages.
+        self.details = MeasurementDetails()
+
+        ## Set to @ref SolutionType::RTKFixed when heading is available, or @ref SolutionType::Invalid otherwise.
+        self.solution_type = SolutionType.Invalid
+        ## A bitmask of flags associated with the solution.
+        self.flags = 0
+
         ##
+        # The position of the secondary GNSS antenna relative to the primary antenna (in meters), resolved with respect
+        # to the local ENU tangent plane: east, north, up.
         self.relative_position_enu_m = np.full((3,), np.nan)
         ##
         # The position standard deviation (in meters), resolved with respect to the
         # local ENU tangent plane: east, north, up.
-        #
-        # @note
-        # If a differential solution to the base station is not available, these
-        # values will be `NAN`.
-        ##
         self.position_std_enu_m = np.full((3,), np.nan)
 
         ##
         # The heading between the primary device antenna and the secondary (in degrees) with
         # respect to true north.
         #
         # @note
         # Reported in the range [0, 360).
-        #
-        ##
         self.heading_true_north_deg = np.nan
 
         ##
-        # The estmated distance between primary and secondary antennas (in meters)
-        #
-        ##
+        # The estimated distance between primary and secondary antennas (in meters).
         self.baseline_distance_m = np.nan
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
-        initial_offset = offset
-        if (buffer is None):
+        if buffer is None:
             buffer = bytearray(self.calcsize())
+
+        initial_offset = offset
+
         buffer = self.details.pack(buffer)
         offset += self.details.calcsize()
-        self._STRUCT.pack_into(buffer, offset,
-            self.solution_type,
+
+        self._STRUCT.pack_into(
+            buffer, offset,
+            int(self.solution_type),
             self.flags,
             self.relative_position_enu_m[0],
             self.relative_position_enu_m[1],
             self.relative_position_enu_m[2],
             self.position_std_enu_m[0],
             self.position_std_enu_m[1],
             self.position_std_enu_m[2],
             self.heading_true_north_deg,
             self.baseline_distance_m)
         offset += self._STRUCT.size
+
         if return_buffer:
             return buffer
         else:
             return offset - initial_offset
 
     def unpack(self, buffer: bytes, offset: int = 0, message_version: int = MessagePayload._UNSPECIFIED_VERSION) -> int:
         initial_offset = offset
 
         offset += self.details.unpack(buffer, offset)
+
         (solution_type_int,
-            self.flags,
-            self.relative_position_enu_m[0],
-            self.relative_position_enu_m[1],
-            self.relative_position_enu_m[2],
-            self.position_std_enu_m[0],
-            self.position_std_enu_m[1],
-            self.position_std_enu_m[2],
-            self.heading_true_north_deg,
-            self.baseline_distance_m) = self._STRUCT.unpack_from(buffer, offset)
+         self.flags,
+         self.relative_position_enu_m[0],
+         self.relative_position_enu_m[1],
+         self.relative_position_enu_m[2],
+         self.position_std_enu_m[0],
+         self.position_std_enu_m[1],
+         self.position_std_enu_m[2],
+         self.heading_true_north_deg,
+         self.baseline_distance_m) = self._STRUCT.unpack_from(buffer, offset)
         offset += self._STRUCT.size
+
         self.solution_type = SolutionType(solution_type_int)
+
         return offset - initial_offset
 
+    def __repr__(self):
+        result = super().__repr__()[:-1]
+        result += f', solution_type={self.solution_type}, heading={self.heading_true_north_deg:.1f} deg, ' \
+                  f'baseline={self.baseline_distance_m} m]'
+        return result
+
     def __str__(self):
         return f"""\
-HeadingMeasurement @ {str(self.details.p1_time)}
-  Solution Type: {SolutionType(self.solution_type).to_string()}
+Raw Heading Output @ {str(self.details.p1_time)}
+  Solution Type: {self.solution_type}
   Relative position (ENU) (m): {self.relative_position_enu_m[0]:.2f}, {self.relative_position_enu_m[1]:.2f}, {self.relative_position_enu_m[2]:.2f}
   Position std (ENU) (m): {self.position_std_enu_m[0]:.2f}, {self.position_std_enu_m[1]:.2f}, {self.position_std_enu_m[2]:.2f}
   Heading (deg): {self.heading_true_north_deg:.2f}
   Baseline distance (m): {self.baseline_distance_m:.2f}"""
 
     @classmethod
     def calcsize(cls) -> int:
         return cls._STRUCT.size + MeasurementDetails.calcsize()
 
     @classmethod
-    def to_numpy(cls, messages: Sequence['HeadingMeasurement']):
+    def to_numpy(cls, messages: Sequence['RawHeadingOutput']):
         result = {
             'solution_type': np.array([int(m.solution_type) for m in messages], dtype=int),
             'flags': np.array([int(m.flags) for m in messages], dtype=int),
             'relative_position_enu_m': np.array([m.relative_position_enu_m for m in messages]).T,
             'position_std_enu_m': np.array([m.position_std_enu_m for m in messages]).T,
             'heading_true_north_deg': np.array([float(m.heading_true_north_deg) for m in messages]),
             'baseline_distance_m': np.array([float(m.baseline_distance_m) for m in messages]),
```

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/messages/ros.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/ros.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/messages/signal_defs.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/signal_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/messages/solution.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/solution.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/messages/timestamp.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/messages/timestamp.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/parsers/decoder.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/parsers/encoder.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/parsers/file_index.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/utils/argument_parser.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/utils/bin_utils.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/utils/construct_utils.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/utils/enum_utils.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/utils/log.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 import fnmatch
+import glob
 import os
 
 from . import trace as logging
 from ..messages import MessageType
 from ..parsers.file_index import FileIndexBuilder, FileIndex
 from ..parsers.mixed_log_reader import MixedLogReader
 
 _logger = logging.getLogger('point_one.utils.log')
 
 # Note: The spelling here is intentional.
 MANIFEST_FILE_NAME = 'maniphest.json'
 
+# The following files are listed order of priority. The first located file will be returned.
+CANDIDATE_P1LOG_FILES = [
+    # v- Typically captured at the time the log is recorded, or embedded in a mixed-binary log file and extracted
+    # by extract_fusion_engine_log().
+    'input.p1log',
+    'fusion_engine.p1log',
+]
+
 CANDIDATE_MIXED_FILES = ['input.raw', 'input.bin', 'input.rtcm3']
 
 # Determine the default log base directory in the following order of priority:
 # - P1_LOG_BASE_DIR environment variable
 # - If Windows, set to `My Documents/logs`
 # - Otherwise (Linux/Mac):
 #   - Use `/logs` if it exists
@@ -126,30 +135,29 @@
         for m in matches:
             if os.path.basename(m[0]) == pattern:
                 exact_matches.append(m)
 
         if len(exact_matches) == 1:
             matches = exact_matches
         else:
-            e = RuntimeError("Found multiple logs that match pattern '%s'. Please be more specific." % pattern)
-            _logger.error(str(e))
-            _logger.error('Matches:\n  %s' % ('\n  '.join([m[0] for m in matches])))
-            raise e
+            raise RuntimeError(
+                "Found multiple logs that match pattern '%s'. Please be more specific.\n  %s" %
+                (pattern, '\n  '.join([m[0] for m in matches])))
     elif len(matches) == 0:
         message = "Found no logs that match pattern '%s'." % pattern
         if not allow_multiple:
             raise FileNotFoundError(message)
         else:
             _logger.warning(message)
 
     return matches
 
 
 def find_log_file(input_path, candidate_files=None, return_output_dir=False, return_log_id=False,
-                  log_base_dir=DEFAULT_LOG_BASE_DIR, check_exact_match=True):
+                  log_base_dir=DEFAULT_LOG_BASE_DIR, check_exact_match=True, check_pattern_match=True):
     """!
     @brief Locate a log directory containing the specified file(s).
 
     `input_path` may be a file, a directory, or a pattern to be matched to a parent directory within `log_base_dir`.
 
     If `input_path` is a directory or pattern, this function will attempt to locate a log directory containing a data
     file from a list of candidate filenames (`candidate_files`).
@@ -175,14 +183,16 @@
     @param candidate_files A list of one or more data files to be located within the log directory, in order of
            priority. If `None`, defaults to `fusion_engine.p1log`.
     @param return_output_dir If `True`, return the output directory associated with the located input file.
     @param return_log_id If `True`, return the ID of the log if the requested path is a FusionEngine log.
     @param log_base_dir The base directory to be searched when performing a pattern match for a log directory.
     @param check_exact_match If `True`, check if `input_path` is the path to a data file. Otherwise, skip this check and
            only perform a pattern search.
+    @param check_pattern_match If `True` and `input_path` does not refer to a log file or directory, perform a pattern
+           match using `input_path` as the pattern.
 
     @return The path to the located file or a tuple containing:
             - The path to the located file.
             - The path to the located output directory. Only provided if `return_output_dir` is `True`.
             - The log ID string, or `None` if the requested file is not part of a FusionEngine log. Only provided if
               `return_log_id` is `True`.
     """
@@ -203,34 +213,68 @@
             # User specified a string, not a list. Convert to a list.
             candidate_files = [candidate_files]
 
         # First, see if the user's path is an existing log directory containing a data file. If so, use that.
         log_dir = None
         log_id = None
 
+        def _search_directory(dir_path):
+            for f in candidate_files:
+                if f is None:
+                    continue
+
+                test_path = os.path.join(dir_path, f)
+                if os.path.exists(test_path):
+                    return test_path, dir_path, os.path.basename(dir_path)
+            return None, None, None
+
         if check_exact_match:
             dir_exists = os.path.isdir(input_path)
             if dir_exists:
-                for f in candidate_files:
-                    if f is None:
-                        continue
-
-                    test_path = os.path.join(input_path, f)
-                    if os.path.exists(test_path):
-                        log_dir = input_path
-                        log_id = os.path.basename(log_dir)
-                        input_path = test_path
-                        break
+                matching_input_path, log_dir, log_id = _search_directory(input_path)
+                if matching_input_path is not None:
+                    input_path = matching_input_path
         else:
             dir_exists = False
 
+        # If we didn't find an exact match and the path contains a *, try a glob search in the current directory first.
+        # For example, if they specified 'abc*', search for './abc*'.
+        if log_dir is None and '*' in input_path:
+            pattern = input_path
+            matches = glob.glob(pattern)
+            matching_input_path = None
+            matching_log_dir = None
+            matching_log_id = None
+            for m in matches:
+                if os.path.isdir(m):
+                    matching_input_path, matching_log_dir, matching_log_id = _search_directory(m)
+                    if matching_input_path is not None:
+                        break
+                else:
+                    matching_input_path = m
+                    matching_log_dir = os.path.dirname(matching_input_path)
+                    if matching_log_dir == "":
+                        matching_log_dir = "."
+                    matching_log_id = None
+                    break
+
+            if matching_input_path is not None:
+                if len(matches) == 1:
+                    input_path = matching_input_path
+                    log_dir = matching_log_dir
+                    log_id = matching_log_id
+                else:
+                    raise RuntimeError(
+                        "Found multiple logs that match pattern '%s'. Please be more specific.\n  %s" %
+                        (pattern, '\n  '.join(matches)))
+
         # If the user didn't specify a directory, or the directory wasn't considered a valid log (i.e., didn't have any
         # of the candidate files in it), check if they provided a pattern match to a log (i.e., a partial log ID or a
         # search pattern (foo*/partial_id*)).
-        if log_dir is None:
+        if log_dir is None and check_pattern_match and not (input_path.startswith('./') or input_path.startswith('/')):
             if check_exact_match:
                 if dir_exists:
                     _logger.info("Directory '%s' does not contain a data file. Attempting a pattern match." %
                                  input_path)
                 else:
                     _logger.info("File '%s' not found. Searching for a matching log." % input_path)
 
@@ -286,21 +330,15 @@
     @return The path to the located file or a tuple containing:
             - The path to the located file.
             - The path to the located output directory. Only provided if `return_output_dir` is `True`.
             - The log ID string, or `None` if the requested file is not part of a FusionEngine log. Only provided if
               `return_log_id` is `True`.
     """
     # The following files are listed order of priority. The first located file will be returned.
-    candidate_files = [
-        # v- Typically captured at the time the log is recorded, or embedded in a mixed-binary log file and extracted
-        # by extract_fusion_engine_log().
-        'fusion_engine.p1log',
-        # Legacy path, maintained for backwards compatibility.
-        'filter/output/fe_service/output.p1bin',
-    ]
+    candidate_files = CANDIDATE_P1LOG_FILES
     result = find_log_file(input_path, candidate_files=candidate_files, return_output_dir=return_output_dir,
                            return_log_id=return_log_id, log_base_dir=log_base_dir)
     if isinstance(result, tuple):
         p1log_path = result[0]
     else:
         p1log_path = result
 
@@ -394,85 +432,66 @@
             - The path to the located (or extracted) `*.p1log` file
             - The path to the located output directory. Only provided if `return_output_dir` is `True`.
             - The log ID string, or `None` if the requested file is not part of a FusionEngine log. Only provided if
               `return_log_id` is `True`.
     """
     input_path = os.path.expanduser(input_path)
 
-    # Try to find the log normally (look for a directory containing a .p1log file).
+    def _populate_result(input_file, output_dir, log_id):
+        result = [input_file]
+        if return_output_dir:
+            result.append(output_dir)
+        if return_log_id:
+            result.append(log_id)
+
+        if len(result) == 1:
+            return result[0]
+        else:
+            return tuple(result)
+
+    # Look for a log file/directory in the following order of priority:
+    # 1. A file referred to by `input_path`.
+    # 2. A directory referred to by `input_path` containing one of the possible candidate filenames (input.p1log,
+    #    input.raw, etc.).
+    # 3. If `input_path` contains a `*`, a file the specified pattern (e.g., `abc*` matches
+    #    `abc123.p1log`, `/home/**/abc*` matches `/home/user/abc123.p1log`).
+    # 4. If `input_path` contains a `*`, a directory matching the specified pattern and containing one of the candidate
+    #    filenames (e.g., `abc*` matches `abc123/input.p1log`, `/home/**/abc*` matches `/home/user/abc123/input.p1log`).
+    # 5. A directory under `log_base_dir` matching a pattern specified by `input_path` and containing one of the
+    #    candidate filenames (e.g., `<log_base_dir>/<input_path>*/input.p1log`).
+    #
+    # The log file may contain exclusively FusionEngine messages, or may contain mixed binary content.
     try:
-        result = find_p1log_file(input_path, log_base_dir=log_base_dir,
-                                 return_output_dir=return_output_dir, return_log_id=return_log_id)
-        return result
-    except FileNotFoundError as e:
-        is_mixed_file = False
-    except RuntimeError as e:
-        is_mixed_file = False
+        candidate_files = CANDIDATE_P1LOG_FILES
+        candidate_files += CANDIDATE_MIXED_FILES
+        log_file_path, output_dir, log_id = find_log_file(
+            input_path, candidate_files=candidate_files, log_base_dir=log_base_dir,
+            return_output_dir=True, return_log_id=True)
+    except (FileNotFoundError, RuntimeError) as e:
         _logger.error(str(e))
-    except FileExistsError as e:
-        is_mixed_file = True
+        return _populate_result(None, None, None)
 
-    # If that fails, see if we can find a directory containing a mixed content binary file. If found, try to extract
-    # FusionEngine messages from it.
-    if is_mixed_file:
-        # We already know where the file is, but we call find_log_file() anyway just to populate a result tuple for us.
-        result = find_log_file(input_path, return_output_dir=return_output_dir, return_log_id=return_log_id)
-        mixed_file_path = input_path
-    else:
-        _logger.info('Could not find a FusionEngine log directory containing a .p1log file. Searching for a P1 log '
-                     'with mixed binary data.')
-        try:
-            result = find_log_file(input_path, candidate_files=CANDIDATE_MIXED_FILES, log_base_dir=log_base_dir,
-                                   return_output_dir=return_output_dir, return_log_id=return_log_id,
-                                   check_exact_match=False)
-            if isinstance(result, tuple):
-                mixed_file_path = result[0]
-            else:
-                mixed_file_path = result
-        except (FileNotFoundError, RuntimeError) as e:
-            _logger.error(str(e))
-            result = [None]
-            if return_output_dir:
-                result.append(None)
-            if return_log_id:
-                result.append(None)
-
-            if len(result) == 1:
-                return result[0]
-            else:
-                return tuple(result)
+    # Found a log file.
+    _logger.info("Found log file '%s'." % log_file_path)
 
     # Now, search for and extract FusionEngine messages within the mixed binary data to create a *.p1log file if
     # requested, or simply return the path to the mixed content file.
-    _logger.info("Found mixed-content log file '%s'." % mixed_file_path)
-    if extract_fusion_engine_data:
+    parts = os.path.splitext(log_file_path)
+    if parts[1] != '.p1log' and extract_fusion_engine_data:
         # If the user specified an actual file, use its name to set the *.p1log file name.
-        if is_mixed_file:
-            fe_path = os.path.splitext(mixed_file_path)[0] + '.p1log'
+        if os.path.isfile(input_path):
+            fe_path = parts[0] + '.p1log'
         # Otherwise, if they specified a pattern and searched for a log directory, save the output as
         # fusion_engine.p1log.
         else:
-            log_dir = os.path.dirname(mixed_file_path)
-            fe_path = os.path.join(log_dir, "fusion_engine.p1log")
+            fe_path = os.path.join(output_dir, "fusion_engine.p1log")
 
         _logger.info("Extracting FusionEngine content to '%s'." % fe_path)
-        num_messages = extract_fusion_engine_log(input_path=mixed_file_path, output_path=fe_path)
+        num_messages = extract_fusion_engine_log(input_path=log_file_path, output_path=fe_path)
         if num_messages > 0:
-            if isinstance(result, tuple):
-                result = list(result)
-                result[0] = fe_path
-                return tuple(result)
-            else:
-                return result
+            log_file_path = fe_path
         else:
             _logger.warning('No FusionEngine data extracted from mixed data file.')
-            if isinstance(result, tuple):
-                return [None for _ in result]
-            else:
-                return None
-    else:
-        if isinstance(result, tuple):
-            result = list(result)
-            result[0] = mixed_file_path
-            return tuple(result)
-        else:
-            return result
+            return _populate_result(None, None, None)
+
+    # Search successful.
+    return _populate_result(log_file_path, output_dir, log_id)
```

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/utils/numpy_utils.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/utils/time_range.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/time_range.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client/utils/trace.py` & `fusion-engine-client-1.20.0rc1/fusion_engine_client/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client.egg-info/PKG-INFO` & `fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.19.0
+Version: 1.20.0rc1
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.19.0/fusion_engine_client.egg-info/SOURCES.txt` & `fusion-engine-client-1.20.0rc1/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/setup.py` & `fusion-engine-client-1.20.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/tests/test_config.py` & `fusion-engine-client-1.20.0rc1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/tests/test_construct_utils.py` & `fusion-engine-client-1.20.0rc1/tests/test_construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/tests/test_data_loader.py` & `fusion-engine-client-1.20.0rc1/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/tests/test_decoder.py` & `fusion-engine-client-1.20.0rc1/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/tests/test_encoder.py` & `fusion-engine-client-1.20.0rc1/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/tests/test_enum_utils.py` & `fusion-engine-client-1.20.0rc1/tests/test_enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/tests/test_file_index.py` & `fusion-engine-client-1.20.0rc1/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/tests/test_message_defs.py` & `fusion-engine-client-1.20.0rc1/tests/test_message_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/tests/test_mixed_log_reader.py` & `fusion-engine-client-1.20.0rc1/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.19.0/tests/test_time_range.py` & `fusion-engine-client-1.20.0rc1/tests/test_time_range.py`

 * *Files identical despite different names*

